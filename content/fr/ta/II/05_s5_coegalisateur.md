---
book: ta
book_title: Topologie algébrique
chapter: II
chapter_title: GROUPOÏDES
section: 5
section_title: Coégalisateur
lang: fr
source: ta-i-iv-fr
book_pages: A II.196-A II.228
pdf_pages: 0212-0244
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
exercises: 0
content_sha256: be4ef73c46da7909f606648dd78c737fb170b08f05b42bd206dba0ebd6ae023b
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

(ii) Pour tout $(z_1, . . . , z_n)\in$ Z, on a $(z_n, . . . , z_2, z_1)\in$ Z et $(z_n, z_1, . . . , z_{n-1})\in Z$ ;

(iii) Soient $\mathbf{z}= (z_1, . . . , z_n)$ et $\mathbf{z}'= (z'_1, . . . , z'_m)$ des éléments de Z tels que $t(z_n) =o(z_1')$. Posons $\mathbf{z}\mathbf{z}'= (z_1, . . . , z_n, z_1', . . . , z'_m)$. Si deux éléments parmi $\mathbf{z},\mathbf{z}',\mathbf{z}\mathbf{z}'$ appartiennent à Z, il en est de même du troisième ;

(iv) Pour toute flèche $f$ de H, posons $\widetilde{\varphi}(f,1) =\widetilde{\psi}(f,-1) =$ $\varphi (f)$ et $\widetilde{\varphi}(f,-1) =\widetilde{\psi}(f,1) =\psi (f)$. Soient $n$ un entier $\geqslant$ 1 et $(f_1, \varepsilon_1), . . . ,(f_n, \varepsilon_n)$ une suite d’éléments de Fl(H) $\times  \{-1,1\}$ telle que $\widetilde{\psi}(f_i, \varepsilon_i) =\widetilde{\varphi}(f_{i+1}, \varepsilon_{i+1})$ pour $1\leqslant i < n$ et $\widetilde{\psi}(f_n, \varepsilon_n) =\widetilde{\varphi}(f_1, \varepsilon_1)$ ; notons $a_i$ l’origine de $f_i$ et $b_i$ son terme. Pour que $((a_1, \varepsilon_1), . . . ,(a_n, \varepsilon_n))$ appartienne à Z, il faut et il suffit que $((b_1, \varepsilon_1), . . . ,(b_n, \varepsilon_n))$ appartienne à Z.

L’intersection dans $\Omega (\widetilde{\Gamma})$ de toute famille de parties distinguées (relativement à $(\varphi , \psi )$) l’est encore. En particulier, il existe une plus petite partie distinguée contenant une partie Z donnée de $\Omega (\widetilde{\Gamma})$.

#### Proposition 2 {#ta-ii-s5-prop-2 .statement tag=01UK}

Si N est un sous-groupe distingué de $G_a$, l’ensemble des éléments $\mathbf{z}\in \Omega (\widetilde{\Gamma})$ tels que $c(\mathbf{z})$ soit contenu dans N est une partie distinguée de $\Omega (\widetilde{\Gamma})$.

Notons Z l’ensemble des éléments $\mathbf{z}\in \Omega (\widetilde{\Gamma})$ tels que $c(\mathbf{z})\subset N$.

Soit $z\in$ Fl($\widetilde{\Gamma}$). On a $c(z, z) =\{e_a\}$ par définition, d’où $(z, z)\in Z$.

Soit $(z_1, . . . , z_n)\in Z$. Par définition de $c$, la classe de conjugaison $c(z_1, . . . , z_n)$ est égale à $c(z_n, z_1, . . . , z_{n-1})$ et est formée des inverses des éléments de $c(z_n, . . . , z_1)$. Cela montre que Z vérifie la condition (ii).

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

b) Soient $G'$ un groupoïde et $\theta : G\rightarrow G'$ un morphisme de groupoïdes tel que $\theta \circ \varphi =\theta \circ \psi$. Il existe un unique morphisme de groupoïdes $\theta :$ Coeg($\varphi , \psi$ )$\rightarrow G'$ tel que $\theta \circ \gamma =\theta$.

Soit $a$ un sommet de H. La flèche $h(a)$ de Coh($\varphi , \psi$ ) relie $\alpha (\varphi (a))$ à $\alpha (\psi (a))$. Par définition du groupoïde Coeg($\varphi , \psi$ ), l’origine et le terme de la flèche $\beta (h(a))$ sont égaux ; on a donc $\gamma (\varphi (a)) =\gamma (\psi (a))$.

Soit $f$ une flèche de H ; si $a$ désigne son origine et $b$ son terme, on a ainsi

$$
\alpha (\varphi (f))\cdot h(b) =h(a)\cdot \alpha (\psi (b))
$$

En prenant l’image par $\beta$ des deux membres de cette égalité, on obtient la relation $\gamma (\varphi (f)) =\gamma (\psi (f))$. Cela démontre l’assertion a).

Démontrons b). L’application $\eta :$ Som(H) $\rightarrow$ Fl(G$')$ qui à tout sommet $a$ de H associe la flèche $e_{\theta(\varphi(a))}$ de $G'$ est une homotopie reliant $\theta \circ \varphi$ à $\theta \circ \psi$. D’après la propriété universelle des cohomotopeurs (II, p. 185, prop. 3), il existe un unique morphisme de groupoïdes $\theta_1:$ Coh($\varphi , \psi$ )$\rightarrow G'$ tel que $\theta_1\circ \alpha =\theta$ et $\theta_1(h(a)) =e_{\theta(\varphi(a))}$ pour tout sommet $a$ de H. D’après la prop. 7 de II, p. 176, cette dernière propriété implique l’existence d’un unique morphisme de groupoïdes $\theta :$ Coeg($\varphi , \psi$ )$\rightarrow G'$ tel que $\theta \circ \beta =\theta_1$. On a alors $\theta \circ \gamma =\theta_1\circ \alpha =\theta$.

Inversement, si $\theta ':$ Coeg($\varphi , \psi$ )$\rightarrow G'$ est un morphisme de groupoïdes tel que $\theta '\circ \gamma =\theta$, on a $(\theta '\circ \beta )\circ \alpha = (\theta \circ \beta )\circ \alpha$, d’où $\theta '\circ \beta =\theta \circ \beta$ d’après II, p. 185, prop. 3, d’où $\theta '=\theta$ d’après la prop. 7 de II, p. 176. Cela démontre l’unicité de $\theta$, d’où l’assertion b).

#### Corollaire {#ta-ii-s5-n2-cor-1 .statement tag=01UO}

Le groupoïde Coeg($\varphi , \psi$ ) est engendré par l’image du morphisme $\gamma$.

Soit C le sous-groupoïde de Coeg($\varphi , \psi$ ) engendré par l’image de G ; notons $i$ le morphisme canonique de C dans Coeg($\varphi , \psi$ ) et $\theta : G\rightarrow C$ le morphisme tel que $i\circ \theta =\gamma$. D’après la proposition 2, il existe un unique morphisme de groupoïdes $\theta :$ Coeg($\varphi , \psi$ )$\rightarrow C$ tel que $\theta \circ \gamma =\theta$. Alors, $\gamma =i\circ \theta \circ \gamma$, donc $i\circ \theta$ est le morphisme identique de Coeg($\varphi , \psi$ ) (loc. cit.). En particulier, les applications Som($i$) et Fl($i$) sont surjectives, donc C = Coeg($\varphi , \psi$ ).

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

($R_3'$)$r_3'(k, a) = [k](c^{-1}_kk^*(f_{(a,k)})^{-1}f_{(a,k)}))$

pour $k\in K-\{e\}$ et $a\in A_k$

($R_3''$)$r_3''(k, h) = [kh]^{-1}[k][h](c^{-1}_hh^*(c^{-1}_k)c_{kh})$

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

Les éléments $r_3'(e, a)$ donnés par les relations ($R'_3$) pour $k=e$ sont tous égaux à $[e]c^{-1}_e$, élément du groupe $G_o*F(K)$ qu’on obtient en appliquant la relation ($R''_3$) à $k=h=e$. Compte tenu des relations (3), (4) et (5), la proposition résulte donc de II, p. 208, prop. 5.

#### Corollaire 1 {#ta-ii-s5-prop-6-cor-1 .statement tag=01V0}

Supposons que le groupe K soit engendré par les fixateurs des sommets de G. Alors, l’homomorphisme de groupes $\gamma_o: G_o\rightarrow (G/K)_{\gamma(o)}$ est surjectif. En outre, si le groupoïde G est simplement transitif, il en est de même du groupoïde $G/K$.

La relation ($R''_3$) implique $\lambda ([e]) =\lambda (c_e) =\gamma_o(c_e)$. Les relations ($R''_3$) entraînent alors que l’ensemble des $k\in K$ tels que $\lambda ([k])$ appartienne à l’image de $\gamma_o$ est un sous-groupe de K. Enfin, les relations ($R'_3$) montrent que, pour tout élément $k\in K$ dont le fixateur n’est pas vide, $\lambda ([k])$ appartient à l’image de $\gamma_o$. Le corollaire en résulte.

#### Remarque 1 {#ta-ii-s5-n5-rem-1 .statement tag=01V1}

On peut donner une autre description, parfois plus commode, du groupe $(G/K)_{\gamma(o)}$. Pour cela, posons $M = K\times G_o$ et définissons une loi de composition dans M par la formule

$$
(k, a)\cdot (h, b) = (kh, c^{-1}_{kh}h^*(c_ka)c_hb)
$$

pour $k,h\in K$ et $a,b\in G_o$. On vérifie que cette loi de composition est associative, que $(e, c^{-1}_e)$ est un élément neutre et que l’élément $(k^{-1}, c^{-1_1}_{k^-}(k^{-1})^*(c_ka)^{-1}c_e)$ est l’inverse de $(k, a)$. Elle munit donc M d’une structure de groupe. En outre, l’application $\lambda ': M\rightarrow (G/K)_{\gamma(o)}$ définie par $(k, a)\mapsto \lambda ([k]a)$ est un homomorphisme de groupes. Soit $\alpha '$ l’unique morphisme de groupes de $G_o*F(K)$ dans M tel que $\alpha '(f) =$ $(e, f)$ si $f\in G_o$ et $\alpha '([k]) = (k, e_o)$ si $k\in K$ ; on a $\lambda '\circ \alpha '=\lambda$.

Les relations ($R_2$) et ($R_3''$) montrent que tout élément de $(G/K)_{\gamma(o)}$ est l’image par l’homomorphisme $\lambda$ d’un élément de $G_o*F(K)$ de la forme $[k]f$, avec $f\in G_o$ et $k\in K$. Par suite, l’homomorphisme $\lambda '$ est surjectif. On vérifie en outre que l’image par $\alpha '$ d’un élément de $G_o*$ F(K) de la forme $(R_2)$ ou $(R''_3)$ est nulle. Par conséquent, le noyau de l’homomorphisme $\lambda '$ est le plus petit sous-groupe distingué de M contenant les images par $\alpha '$ des éléments de $G_o*F(K)$ de la forme ($R_3'$).

#### Corollaire 2 {#ta-ii-s5-prop-6-cor-2 .statement tag=01V2}

Supposons que le groupe K opère librement dans Som(G). Il existe alors un unique morphisme de groupes $\pi : (G/K)_{\gamma(o)}\rightarrow$ K dont le noyau contient l’image de $\gamma_o$ et tel que $\pi (\lambda ([k])) =k$ pour tout $k\in K$. De plus, $G_o\longrightarrow^{\gamma_o}(G/K)_{\gamma(o)}-\rightarrow^{\pi}$ K est une extension de K par $G_o$.

Si un tel homomorphisme de groupes $\pi$ existe, l’homomorphisme de groupes $\pi \circ \lambda$ est nécessairement égal à l’unique homomorphisme de groupes $p$ de $G_o*F(K)$ dans K tel que $p(f) =e$ pour $f\in G_o$ et $p([k]) =k$. Il est immédiat de vérifier que les éléments de $G_o*F(K)$ définis par les formules ($R_2$) et ($R''_3$) appartiennent au noyau de $p$. Par hypothèse, il n’y a pas d’élément du type ($R_3'$). Ainsi, le noyau du morphisme $\lambda$ contient celui de $p$. Par suite, il existe un unique homomorphisme de groupes $\pi : (G/K)_{\gamma(o)}\rightarrow K$ tel que $\pi \circ \lambda =p$.

Il est évident que l’homomorphisme $\pi$ est surjectif. Pour montrer que l’homomorphisme $\gamma_o$ est injectif et que son image est exactement le noyau de $\pi$, remarquons que l’homomorphisme $\lambda ': M\rightarrow (G/K)_{\gamma(o)}$ (II, p. 213, remarque 1) est un isomorphisme, car on a supposé que K opère librement dans Som(G). L’homomorphisme composé $(\lambda ')^{-1}\circ \gamma_o$ de $G_o$ dans M est donné par $f\mapsto (e, f)$, tandis l’homomorphisme $\pi \circ \lambda ': M\rightarrow K$ applique $(k, f)$ sur $k$. Le corollaire en résulte.

#### Corollaire 3 {#ta-ii-s5-prop-6-cor-3 .statement tag=01V3}

Supposons que le groupoïde G soit simplement transitif. Soit $K_0$ le sous-groupe de K engendré par les fixateurs des sommets de G. L’application de K dans $(G/K)_{\gamma(o)}$ qui à $k\in K$ associe $\gamma (c_k)$ est un homomorphisme de groupes surjectif, de noyau $K_0$.

Si un élément $k\in K$ fixe un sommet $a$ de G, l’élément $g^{-1}kg$ fixe le sommet $g^*a$; cela entraîne que $K_0$ est un sous-groupe distingué de K.

D’après la proposition 5, l’unique homomorphisme $\lambda : F(K)\rightarrow$ $(G/K)_{\gamma(o)}$ tel que $\lambda ([k]) =\gamma (c_k)$ est surjectif, et son noyau est le plus petit sous-groupe distingué de F(K) contenant les éléments $[k]$, où $k$ est un élément de K qui fixe un sommet de G, et les éléments $[kh]^{-1}[k][h]$, où $(k, h)\in K^2$. En particulier, l’application $\lambda ': K\rightarrow (G/K)_{\gamma(o)}$, définie par $\lambda '(k) =\gamma (c_k) =\lambda ([k])$ pour $k\in K$, est un homomorphisme de groupes. On a $\lambda =\lambda '\circ p$, où $p: F(K)\rightarrow K$ désigne l’homomorphisme de groupes surjectif canonique. Par suite, l’homomorphisme $\lambda '$ est surjectif et son noyau est le plus petit sous-groupe distingué de K qui contient les éléments $k$, pour $k$ fixant un sommet de G, c’est-à-dire $K_0$. Cela démontre la proposition.

# Exercices

§1

1) Soit $(Q_i)_{i\in I}$ une famille de carquois. On note S l’ensemble somme de la famille (Som(Q$_i))$, F l’ensemble somme de la famille (Fl(Q$_i)),o$ et $t$ les applications de F dans S déduites des application origine et terme des carquois $Q_i$. a) Démontrer que $Q = (S,F, o, t)$ est un carquois. On dit que c’est le carquois somme de la famille $(Q_i)$.

b) Pour $i\in I$, il existe un unique morphisme de carquois $j_i$ de $Q_i$ dans Q tel que l’application Som($j_i$) soit l’application canonique de Som(Q$_i)$ dans S et l’application Fl($j_i$) soit l’application canonique de Fl(Q$_i)$ dans S.

c) Soit K un carquois et, pour tout $i\in I$, soit $\varphi_i$ un morphisme de carquois de $Q_i$ dans K. Démontrer qu’il existe un unique morphisme de carquois $\varphi$ de Q dans K tel que l’on ait $\varphi \circ j_i=\varphi_i$ pour tout $i\in I$.

2) Soit $Q = (S,F, o, t)$ un carquois. Pour tout $s\in S$ on appelle degré sortant (resp. entrant) de Q en $s$ et on note $d_+(s)$ (resp. $d_-(s)$) le cardinal de l’ensemble $\{f\in F|o(f) =s\}$ (resp. $\{f\in F|t(f) =s\}$. On dit que Q est localement fini si $d_+(s)$ et $d_-(s)$ sont finis, pour tout $s\in S$, et qu’il est fini si les ensembles F et S sont finis.

Démontrer les égalités $\sum_{s\in S}d_+(s) =\sum_{s\in S}d_-(s) =$ Card(F).

3) Soit $Q = (S,F, o, t)$ un carquois localement fini. On définit la matrice $M_Q= (m_{i,j})$, de type $(S,S)$ à éléments dans $\mathbf{Z}$, par

$m_{i,j}=$ Card$\{f\in F|o(f) =i$ et $t(f) =j\}$. La matrice $M_Q$ est appelée la matrice d’adjacence de Q.

a) Étant donnés des carquois Q et $Q'$, donner une condition nécessaire et suffisante sur leurs matrices d’adjacence pour que les carquois Q et $Q'$ soient isomorphes.

b) Exprimer en termes de la matrice d’adjacence $M_Q$ le nombre de chemins de longueur $n$ dans Q dont l’origine et le terme sont donnés.

c) *Démontrer que la matrice d’adjacence du carquois sous-jacent à un graphe est symétrique.*

4) Soit $Q = (S,F, o, t)$ un carquois. On note I l’ensemble somme de la famille $(S,F)$; on identifie S et F à des parties de I. Soit $k$ un anneau commutatif. On appelle $k$-algèbre du carquois Q le quotient $A_Q$ de la $k$-algèbre associative libre sur l’ensemble I par l’idéal bilatère engendré par les éléments $X^2_s-X_s$ (pour $s\in S$), $X_uX_v-X_vX_u$ (pour $u, v\in S$), $X_fX_{t(f)}-X_f$ et $X_{o(f)}X_f-X_f$ (pour $f\in F$). Pour $i\in I$, on note $x_i$ l’image de $X_i$ dans l’algèbre $A_Q$.

a) Démontrer que l’on a $\sum_{s\in S}x_s= 1$.

b) Prouver que l’on a $x_fx_g= 0$ si $f$ et $g$ sont des flèches de Q qui ne sont pas composables.

c) Pour tout chemin $c= (a_0, f_1, . . . , f_n, a_n)$ dans Q, on pose $x_c$ = $x_{a_0}x_{f_1}. . . x_{f_n}$. Soient $c$ et $c'$ des chemins dans Q; démontrer que l’on a $x_cx_{c'}=x_{cc'}$ si $c$ et $c'$ sont composables, et $x_c=x_{c'}$ sinon.

d) Soit C l’ensemble des chemins dans le carquois Q; démontrer que la famille $(x_c)_{c\in C}$ est une base du $k$-module $A_Q$.

e) Soit $J_Q$ l’idéal bilatère de $A_Q$ engendré par les éléments de la forme $x_f$, pour $f\in F$. Démontrer que l’algèbre $A_Q/J_Q$ est isomorphe à $k^{(S)}$.

f) Pour que la $k$-algèbre $A_Q$ soit un $k$-module de type fini, il faut et il suffit que l’ensemble des sommets de Q soit fini et que tout lacet dans Q soit de longueur nulle. L’idéal $J_Q$ est alors nilpotent.

Nous conservons ces notations pour la suite des exercices du §1. Lorsque nous parlons d’un $A_Q$-module (sans préciser), il s’agit d’un module à droite. Si A est un anneau, un A-module M (sans préciser) sera un A-module à droite ; si $a$ est un élément de A, on note $a_M$ ou $(a)_M$ l’homothétie $x\mapsto xa$ de M.

5) a) Démontrer que le quadruplet $Q^{\circ}= (S,F, t, o)$ est un carquois. On dit que c’est le carquois opposé de Q.

b) L’algèbre $A_{Q^{\circ}}$ est isomorphe à l’algèbre opposée de l’algèbre $A_Q$.

6) a) Soit $(M_s)_{s\in Som(Q)}$ une famille de $k$-modules et soit $(u_f)_{f\in Fl(Q)}$ une famille où, pour tout $f\in$ Fl(Q)$,u_f$ est une application linéaire de $M_{o(f)}$ dans $M_{t(f)}$. Soit M la somme directe de la famille $(M_s)$ ; pour $s\in S$, notons $j_s$ l’injection canonique de $M_s$ dans M et $p_s$ la projection canonique de M sur $M_s$. Démontrer qu’il existe une unique structure de $A_Q$-module sur M telle que l’on ait $(x_s)_M=j_s\circ p_s$ et $(x_f)_M=j_{t(f)}\circ u_f\circ p_{o(f)}$ pour tout $s\in$ Som(Q) et tout $f\in$ Fl(Q).

Inversement, tout $A_Q$-module est de cette forme.

b) Si Λ est un $k$-module et $s\in$ Som(Q), on note $\Lambda (s)$ le $A_Q$-module associé à la famille $(M_i)_{i\in Som(Q)}$ de $k$-modules donnée par $M_i= \Lambda$ si $i=s$ et $M_i= 0$ sinon, et à la famille $(u_f)_{f\in Fl(Q)}$ d’applications linéaires, où $u_f$ = 0 pour tout $f\in$ Fl(Q).

Soient Λ et $\Lambda '$ des $k$-modules non nuls. Soient $s$ et $s'$ des sommets de Q. Démontrer que $\Lambda (s)$ est isomorphe à $\Lambda '(s')$ si et seulement si Λ et $\Lambda '$ sont des $k$-modules isomorphes et si $s=s'$.

c) Si Λ est un $k$-module simple, alors $\Lambda (s)$ est un $A_Q$-module simple pour tout sommet $s$.

d) On suppose de plus que tout lacet dans Q est de longueur nulle. Démontrer que tout $A_Q$-module simple est de la forme $\Lambda (s)$, où Λ est un $k$-module simple et $s$ un sommet de Q.

7) On suppose que $k$ est un corps algébriquement clos. Pour tout $s\in$ Som(Q), on pose $P(s) =x_sA_Q$.

a) Démontrer que $P(s)$ est un $A_Q$-module projectif et indécomposable, et que son socle est isomorphe au $A_Q$-module $k(s)$. Prouver aussi que $P(s)/P(s)J_Q$ est isomorphe à $k(s)$.

b) On suppose que tout lacet de Q est de longueur nulle. Démontrer que, pour tout $s\in$ Som(Q), l’homomorphisme canonique de $k$ dans End(P($s$)) est un isomorphisme. Démontrer que, pour tout $A_Q$-module P qui est projectif et indécomposable, il existe un unique sommet $s$ de Q tel que P soit isomorphe à $P(s)$.

8) Pour $s\in$ Som(Q), on pose $P(s) =x_sA_Q$. Soit M un $A_Q$-module.

a) Soit $f\in$ Fl(Q), notons $u=o(f)$ et $v=t(f)$. Démontrer qu’il existe un unique couple $(\varphi '_f, \varphi ''_f)$ d’homomorphismes de $A_Q$-modules

$$
\varphi '_f: Mx_u\otimes_kP(v)\rightarrow Mx_u\otimes_kP(u),\varphi ''_f: Mx_u\otimes_kP(v)\rightarrow Mx_v\otimes_kP(v)
$$

tel que $\varphi '_f(m\otimes p) =m\otimes x_fp$ et $\varphi ''_f(m\otimes p) =mx_f\otimes p$ pour tout $m\in Mx_u$ et tout $p\in P(v)$.

b) Soit $s\in$ Som(Q). Démontrer qu’il existe un unique homomorphisme de $A_Q$-modules $\psi_s: Mx_s\otimes_kP(s)\rightarrow M$ tel que $\psi_s(m\otimes p) =mp$ pour $p\in P(s)$ et $m\in Mx_s$. c) On pose $\varphi =\bigoplus\varphi '_f-\bigoplus\varphi ''_f$ et $\psi =\sum\psi_s$. Démontrer que l’on a une suite exacte de $A_Q$-modules

$$
0\rightarrow \bigoplus Mx_{o(f)}\otimes_kP(t(f))-\rightarrow^{\varphi}\bigoplus Mx_s\otimes_kP(s)-^{\psi}\rightarrow M\rightarrow 0
$$

$f\in$Fl(Q) $s\in$Som(Q)

d) Démontrer que tout idéal à droite de l’algèbre $A_Q$ est projectif.

9) a) Soient M et N des $A_Q$-modules ; pour $s\in$ Som(Q), on pose $M_s=$ $Mx_s$ et $N_s= Nx_s$. Pour $\varphi = (\varphi_s)_{s\in Som(Q)}$ et $f\in$ Fl(Q), on définit une application $\theta_f(\varphi ): Mx_{o(f)}\rightarrow Nx_{t(f)}$ en posant

$$
\theta_f(\varphi )(m) =\varphi_{o(f)}(m)x_f-\varphi_{t(f)}(mx_f)
$$

Démontrer que l’application

$\theta :\prod$ Hom$_k(M_s,N_s)\rightarrow \prod$ Hom(M$_{o(f)},N_{t(f)})$

$s\in$Som(Q) $f\in$Fl(Q)

donnée par $\varphi \mapsto (\theta_f(\varphi ))_{f\in Fl(Q)}$ est linéaire.

b) Démontrer que Ker($\theta$ ) est isomorphe à Hom$_{A_Q}(M,N)$ et que Coker($\theta$ ) est isomorphe à Ext$^1_{A_Q}(M,N)$. Démontrer que Ext$^p_{A_Q}(M,N) = 0$ pour tout entier $p\geqslant 2$.

c) On suppose que $k$ est un corps commutatif et que le carquois Q est fini Si M et N sont des $k$-espaces vectoriels de dimension finie, alors Ext$^p_{A_Q}(M,N)$ est un $k$-espace vectoriel de dimension finie pour tout entier $p\geqslant 0$, nulle pour $p\geqslant 2$, et

dim$_k$(Hom$_{A_Q}(M,N))-$ dim$_k$(Ext$^1_{A_Q}(M,N))$

= $\sum$ dim(M$_s)$ dim(N$_s)-\sum$ dim(M$_{o(f)})$ dim(N$_{t(f)})$.

$s\in$Som(Q) $f\in$Fl(Q)

d) On suppose que $k$ est un corps commutatif. Démontrer que pour tout couple $(u, v)$ de sommets de Q, la dimension de l’espace vectoriel Ext$^1_{A_Q}(k(u), k(v))$ est égale au cardinal de l’ensemble des flèches de Q d’origine $v$ et de terme $u$.

10) On suppose que $k$ est un corps algébriquement clos. Soient Q et $Q'$ des carquois finis dont tout lacet est de longueur nulle. Prouver que l’algèbre $A_{Q'}$ est équivalente au sens de Morita (A, VIII, §6) à l’algèbre $A_Q$ si et seulement si les carquois Q et $Q'$ sont isomorphes. (Prendre pour modules $M,N$ les $k$-modules simples $k(s)$, pour $s\in$ Som(Q).)

§2

1) Soit G un graphe et soit $Q = (S,F, o, t)$ son carquois sous-jacent.

a) Démontrer que l’on a $d_+(s) =d_-(s)$ pour tout $s\in S$. Cet entier est alors appelé degré de G en $s$ et noté $d(s)$.

b) On suppose que G est fini. Pour qu’il existe un lacet $(a_0, f_1, . . . , f_n, a_n)$ dans G tel que, pour toute arête $\varphi$ de G, il existe un unique entier $n$ tel que $\varphi =\{f_n, f_n\}$, il faut et il suffit que G soit connexe et que $d(s)$ soit pair, pour tout $s\in$ Som(G).

2) Soit $G = (S,F, o, t)$ un carquois. On dit que G est un carquois bipartite s’il existe une partition $P =\{S_1,S_2\}$ en sous-ensembles de S telle que pour toute flèche $f\in F$, l’origine $o(f)$ et le terme $t(f)$ sont dans des parties différentes de la partition P.

a) On suppose que G est connexe. Démontrer qu’il existe au plus une partition P comme ci-dessus.

b) Démontrer qu’un graphe G est bipartite si et seulement si tout lacet dans G est de longueur paire.

3) Soit G un graphe connexe localement fini dont l’ensemble des sommets est infini. Démontrer qu’il existe une suite composable $(f_n)_{n\in\mathbf{N}}$ de flèches de G dont les origines soient deux à deux distinctes (théorème de König).

4) Soit G un graphe fini et soit $Q = (S,F, o, t)$ son carquois sous-jacent. On munit l’espace $\mathbf{C}^S$ de l’unique structure d’espace hermitien pour laquelle sa base canonique est orthonormale. Soit $L:\mathbf{C}^S\rightarrow \mathbf{C}^S$ l’application donnée par $L(u)(x) =\sum_{o(f)=x}(u(t(f))-u(x))$ pour $x\in S$ et $u\in \mathbf{C}^S$.

a) Démontrer que l’endomorphisme L de $\mathbf{C}^S$ est positif (EVT, V, p. 45, déf. 6).

b) Démontrer que le noyau de L est constitué des fonctions $u\in \mathbf{C}^S$ qui sont constantes sur chaque composante connexe de G.

c) Soit $F_1$ une orientation de G. Soit E $= (e_{s,f})$ la matrice de type $(S,F_1)$ donnée par

1 si $o(f) =s$ et $t(f)=\not s$;

$e_{s,f}=-1$ si $o(f)=\not s$ et $t(f) =s$;

0 sinon.

Démontrer que la matrice Λ de L dans la base canonique de $\mathbf{C}^S$ est donnée par Λ = $E\cdot^tE$.

d) On suppose que G est connexe et que l’ensemble de ses sommets n’est pas vide ; soit $x$ un sommet de G et soit $S'= S-\{x\}$. Soit T un sous-ensemble de F de cardinal Card(S$')$. Démontrer que T est l’ensemble des flèches d’un sous-arbre orienté maximal de G (muni de l’orientation $F_1)$ si et seulement si le rang de la matrice $E_T'$ de type $(S',T)$ déduite de E est égal à Card(S$')$. En déduire alors que le déterminant de la matrice $\Lambda_{S',S'}$ est égal au nombre de sous-arbres orientés maximaux de G. (Utiliser l’exercice 6 de A, III, §8, p. 192.)

e) Soit W l’orthogonal de Ker(L). Démontrer que W est un sous-espace de $\mathbf{C}^S$ qui est stable par W et que det(L$|_W)$ est égal au nombre de forêts maximales du graphe G (théorème de Kirchhoff).

5) a) Soit $n$ un entier naturel $\geqslant 1$ et soit G un graphe dont l’ensemble des sommets est l’ensemble $\mathbf{Z}/n\mathbf{Z}$ et tel que deux sommets $i$ et $j$ sont reliés par une flèche si et seulement si $i-j=\pm 1$ (mod$. n)$. Expliciter l’ensemble des forêts maximales de G.

b) Soit G un graphe et soit S l’ensemble de ses sommets. On suppose que pour tout couple $(x, y)$ de sommets de G, l’ensemble des flèches de G d’origine $x$ et de terme $y$ est de cardinal 1 si $x=\not y$ et 0 sinon (« graphe complet »). Calculer le cardinal de l’ensemble des forêts maximales de G.

c) Soit G un graphe et soit S l’ensemble de ses sommets. Soit $(S_1,S_2)$ une partition de S ; on suppose que pour tout couple $(x, y)$ de sommets de G, l’ensemble des flèches de G d’origine $x$ et de terme $y$ est de cardinal 1 si $(x, y)\in S_1\times S_2$ et 0 sinon (« graphe bipartite complet »). Calculer le cardinal de l’ensemble des forêts maximales de G.

6) Soit $c$ un entier naturel.

a) Il existe une unique famille d’applications $R_c: (\mathbf{N}^*)^c\rightarrow \mathbf{N}^*$, pour $c\geqslant 2$, vérifiant les propriétés suivantes :

(i) S’il existe $i$ tel que $n_i= 1$, alors $R_c(n_1, . . . , n_c) = 1$ ;

(ii) On a $R_2(m, n) = R_2(m-1, n) + R_2(m, n-1)$ si $m$ et $n$ sont des entiers $\geqslant 2$ ;

(iii) Si $c\geqslant 3$, on a $R_c(n_1, . . . , n_c) = R_{c-1}(n_1, . . . , n_{c-2},R_2(n_{c-1}, n_c))$ pour tout $(n_1, . . . , n_c)\in \mathbf{N}^c$.

b) On a $R_2(m, n) =^{m+n-2}_{m-1}$ pour tout couple $(m, n)$ d’entiers $\geqslant 1$.

c) Pour toute suite finie $(n_1, . . . , n_c)$ d’entiers naturels $\geqslant 1$ et tout entier naturel $R\geqslant 1$, on dit que la propriété $\mathbf{R}(n_1, . . . , n_c; R)$ est satisfaite si, pour tout graphe complet dont l’ensemble des sommets S est de cardinal $\geqslant R$ et toute partition $P = (F_1, . . . ,F_c)$ de l’ensemble F de ses flèches, il existe un entier $i\in  \{1, . . . , c\}$ et une partie A de S de cardinal $n_i$ tels que toute flèche de G reliant deux éléments de A appartienne à $F_i$.

Démontrer la propriété $\mathbf{R}(n_1, . . . , n_c; R_c(n_1, . . . , n_c))$. d) On note $R(n_1, . . . , n_c)$ le plus petit entier $R\geqslant 1$ tel que la propriété $\mathbf{R}(n_1, . . . , n_c; R)$ soit vérifiée (« nombres de Ramsey »).

e) On a $R(n,2) =n$ pour tout entier $n\geqslant 2$ ; on a $R(3,3) = 6$.

f) Démontrer que $R(4,3) = 9$.

¶ g) Calculer $R(5,5)$ ; calculer $R(6,6)$.

7) Soit G un groupe opérant à droite sur un ensemble X et soit A une partie de G. Le carquois de Schreier $\mathscr{G}_G(X,A)$ est le carquois $(S,F, o, t)$ défini par :

– L’ensemble de ses sommets est S = X ;

– L’ensemble de ses flèches est $F = X\times A$ ;

– Les applications $o$ et $t$ sont données par $o(x, a) =x$ et $t(x, a) =x\cdot a$ pour tout $(x, a)\in X\times A$.

Lorsque X = G sur lequel G opère par multiplication à droite, on note $\mathscr{G}(G,A)$ ce carquois et on l’appelle le carquois de Cayley de G par rapport à A.

On appelle graphe de Schreier (resp. graphe de Cayley) le graphe associé à ce carquois.

a) Démontrer que le carquois $\mathscr{G}_G(X,A)$ est connexe si et seulement si le sous-groupe H de G engendré par A a au plus une orbite sur X.

b) On suppose que A engendre G. Montrer que le graphe de Cayley $\mathscr{G}(G,A)$ est connexe et qu’il est bipartite si et seulement si il existe un homomorphisme de groupe $\varphi : G\rightarrow \mathbf{Z}/2\mathbf{Z}$ tel que $\varphi (a) = 1$ pour tout $a\in A$.

c) Montrer qu’il existe une unique action de G sur le graphe de Cayley $\mathscr{G}(G,A)$ telle que l’action de G induite sur les sommets de ce graphe soit l’action de G sur lui-même par multiplication à gauche.

8) On dit qu’un lacet $(a_0, f_1, . . . , f_n, a_n)$ dans un graphe G est hamiltonien si pour tout sommet $s$ de G, il existe un unique entier $m\in  \{1, . . . , n\}$ tel que $a_m=s$. On dit qu’un graphe est hamiltonien s’il existe un lacet hamiltonien dans G.

a) Soit S un ensemble fini de cardinal $\geqslant 3$ et soit $K_S$ un graphe complet d’ensemble de sommets S. Démontrer que le graphe $K_S$ est hamiltonien. Plus précisément, démontrer que pour toute orientation A de G, il existe un lacet hamiltonien dans $K_S$ dont toute flèche appartient à A.

b) On note $\mathscr{G}_S$ l’ensemble des sous-graphes de $K_S$ dont l’ensemble des sommets est égal à S. Soit $\preccurlyeq$ la relation d’ordre la moins fine dans l’ensemble $\mathscr{G}_S$ pour laquelle $G\preccurlyeq G'$ s’il existe des éléments $u, v$ de S tels que deg($u$) $+$ deg($v$)$\geqslant$ Card(S) et tels que Fl(G$')$ soit la réunion de Fl(G) et des deux flèches de $K_S$ d’extrémités $u$ et $v$.

Démontrer que, pour tout $G\in \mathscr{G}_S$, l’ensemble des éléments H de $\mathscr{G}_S$ tels que $G\preccurlyeq H$ possède un unique élément maximal ; on le note $c(G)$.

c) Soit G un sous-graphe de $K_S$ d’ensemble de sommets S. Démontrer que le graphe G est hamiltonien si et seulement s’il en est de même du graphe $c(G)$. d) Soit G un sous-graphe de $K_S$ dont l’ensemble des sommets est S et dont le degré en chaque sommet est $\geqslant$ Card(S)$/2$. Démontrer que $c(G)$ est égal à $K_S$. En déduire que G est un graphe hamiltonien (théorème de G. Dirac).

9) Soit $(W,S)$ un système de Coxeter (LIE, IV, §1, p. 11, déf. 3) ; on suppose que le groupe W est fini.

a) On suppose que $(W,S)$ est irréductible et a au plus deux sommets. Démontrer que le graphe de Cayley $\mathscr{G}(W,S)$ est hamiltonien.

b) On suppose que $(W,S)$ est irréductible et a au moins trois sommets. Soit $s\in S$ un sommet terminal (LIE IV, annexe) du graphe de Coxeter associé à $(W,S)$. On pose $S'= S-\{s\}$ et on note $W'$ le sous-groupe de W engendré par $S'$. Soit Γ le graphe dont l’ensemble des sommets est l’ensemble des classes à gauche modulo $W'$ dans W et tel que deux sommets distincts A et B sont reliés par une arête exactement si et seulement si $As\cap B$ n’est pas vide. À l’aide d’un sous-arbre maximal du graphe Γ, démontrer que si le graphe de Cayley $\mathscr{G}(W',S')$ est hamiltonien, il en est de même du graphe $\mathscr{G}(W,S)$.

c) Démontrer que le graphe de Cayley $\mathscr{G}(W,S)$ est hamiltonien (théorème de Conway–Sloane–Wilks).

10) Soit G un graphe connexe dont S est l’ensemble des sommets. Pour $x, y\in S$, on pose

$d_G(x, y) =$ inf$\{\ell \in \mathbf{N}:$ il existe un chemin de longueur $\ell$ reliant $x$ à $y\}$.

a) Démontrer que $d_G$ est une distance sur l’ensemble S.

b) Soient $G_1$ et $G_2$ des graphes et $\varphi : G_1\rightarrow G_2$ un morphisme de graphes. Montrer que $d_{G_2}(\varphi (x), \varphi (y))\leqslant d_{G_1}(x, y)$ pour tout couple $(x, y)$ de sommets de $G_1$.

11) Soit G un graphe connexe dont l’ensemble S des sommets n’est pas vide. On appelle diamètre de G le diamètre diam(G) de l’espace métrique $(S, d_G)$. a) Démontrer que diam(G) $\leqslant$ Card(S)$-1$. Pour quels graphes cette inégalité est-elle une égalité ?

b) Soit $v$ un entier $\geqslant 2$ tel que tout sommet de G soit de degré au plus $v$. Démontrer que Card(S) $\leqslant v^{diam(G)}$. Pour quels graphes cette inégalité est-elle une égalité ? c) Soit $n$ un entier tel que $n\geqslant 2$. Soit $T_n$ la partie de $\mathfrak{S}_n$ formée des transpositions de support $\{m, m+ 1\}$, pour $m\in  \{1, . . . , n-1\}$. Démontrer que le diamètre du graphe de Cayley $\mathscr{G}(\mathfrak{S}_n,T_n)$ est égal à $n(n-1)/2$.

d) Soit $n$ un entier tel que $n\geqslant 2$. Soient $\tau$ la transposition de support $\{1,2\}$ et $\sigma$ le cycle $(1,2, . . . , n)\mapsto (2,3, . . . , n,1)$ dans le groupe $\mathfrak{S}_n$. Soit alors $G_n$ le graphe de Cayley $\mathscr{G}(\mathfrak{S}_n,\{\sigma , \tau \})$. Démontrer que $n(n-1)/6\leqslant$ diam(G$_n)\leqslant 3n(n-1)/2$. (Soit T l’ensemble des suites $(x, y, z)$ d’éléments de $\{1, . . . , n\}$ telles que $x < y < z$. Si $t= (x, y, z)\in T$, on dit qu’une permutation $\lambda \in \mathfrak{S}_n$ préserve l’ordre cyclique de $t$ si l’on a $\lambda (x)< \lambda (y)< \lambda (z)$, ou $\lambda (y)< \lambda (z)< \lambda (x)$, ou $\lambda (z)< \lambda (x)< \lambda (y)$. Observer que la permutation $\sigma$ préserve l’ordre cyclique de tout élément de T, et que la permutation $\tau$ préserve l’ordre cyclique de tout élément de T qui n’est pas de la forme $(1,2, x)$. En déduire que la distance de la permutation identique à la permutation $(1, . . . , n)\mapsto (n, n-1, . . . ,1)$ est au moins égale à $n(n-1)/6$.)

12) Soit $n$ un entier $\geqslant 2$ et soit $p$ un nombre premier $> n/2$. Soit H un sous-groupe de $\mathfrak{S}_n$ qui agit transitivement sur $\{1, . . . , n\}$, contient une transposition et un cycle d’ordre $p$. Soit G un graphe tel que

– L’ensemble de ses sommets est $S =\{1, . . . , n\}$;

– L’ensemble F de ses flèches est l’ensemble des couples $(i, j)\in S\times S$ telles que la transposition $\tau_{i,j}$ appartienne à H ;

– On a $o((i, j)) =i,t((i, j)) =j$ et $(i, j) = (j, i)$ pour tout $(i, j)\in F$. a) Démontrer que toute composante connexe de G est un graphe complet. b) Démontrer que si G est connexe, alors $H =\mathfrak{S}_n$.

c) Démontrer qu’il existe un homomorphisme de groupes de $\mathfrak{S}_n$ dans Aut(G) tel que, pour tout $\sigma \in \mathfrak{S}_n$, l’application Som($\sigma$ ) soit égale à la permutation $\sigma$. Démontrer alors que $\mathfrak{S}_n$ agit transitivement sur l’ensemble des composantes connexes de G, et que celles-ci sont deux à deux isomorphes.

d) Soit $\sigma \in H$ un cycle d’ordre $p$. Démontrer que $\sigma$ stabilise chaque composante connexe de G. En conclure que $H =\mathfrak{S}_n$.

§3

1) Soit $(C_i)_{i\in I}$ une famille de catégories. Soit C le carquois somme de la famille de carquois sous-jacents aux catégories $C_i$.

a) Montrer que le carquois C, muni de la loi de composition déduite des lois de composition des catégories $C_i$, est une catégorie. On dit que c’est la catégorie somme de la famille $(C_i)$. b) Démontrer que le morphisme canonique de $C_i$ dans C est un foncteur. c) Si les $C_i$ sont des groupoïdes, démontrer que la catégorie C est un groupoïde.

2) Soit $(C_i)_{i\in I}$ une famille de catégories. Soit C le produit des carquois sous-jacents aux catégories $C_i$.

a) Montrer que le carquois C, muni de la loi de composition déduite des lois de composition des catégories $C_i$, est une catégorie. On dit que c’est la catégorie produit de la famille $(C_i)$.

b) Démontrer que le morphisme canonique pr$_i: C\rightarrow C_i$ est un foncteur. c) Si les $C_i$ sont des groupoïdes, démontrer que la catégorie C est un groupoïde.

3) Soit C une catégorie ; on note $m$ sa loi de composition. Soit $C^{\circ}$ le graphe orienté opposé muni de la loi de composition donnée par $m^{\circ}(f, g) =m(g, f)$ pour tout couple $(f, g)$ de flèches composables de C.

a) Démontrer que $C^{\circ}$ est une catégorie. On dit que c’est la catégorie opposée de C.

b) Si C est un groupoïde, démontrer que $C^{\circ}$ est un groupoïde isomorphe à C.

4) On définit la masse $\mu(G)$ d’un groupoïde G comme la borne supérieure des sommes $\sum_{a\in A}$ Card(G$_a)^{-1}$, où A parcourt l’ensemble des parties de Som(G) qui rencontrent chaque orbite de G en au plus un point. On dit que G est de masse finie si l’on a $\mu(G)\in \mathbf{R}$; on dit que G est essentiellement fini si l’ensemble de ses orbites est fini et si le groupe d’isotropie en chacun de ses points est fini.

a) Démontrer qu’un groupoïde essentiellement fini est de masse finie.

b) Soit G le groupoïde associé à un groupe fini Γ. Il est essentiellement fini et l’on a $\mu(G) = 1/$ Card(Γ).

c) Soit Γ un groupe fini, soit X un ensemble fini muni d’une opération à droite de Γ et soit G le groupoïde associé. Il est essentiellement fini et l’on a $\mu(G) =$ Card(X)$/$ Card(Γ).

d) Soient $(G_i)_{i\in I}$ une famille de groupoïdes de masse finie. Le groupoïde somme et le groupoïde produit de la famille $(G_i)$ ont pour masse $\sum\mu(G_i)$ et $\prod\mu(G_i)$ respectivement.

e) Soit X un ensemble. On définit un groupoïde G dont l’ensemble des sommets est l’ensemble des sous-ensembles finis de X et tel que, pour tout couple $(Y_1,Y_2)$ de parties finies de X, l’ensemble des flèches d’origine $Y_1$ et de terme $Y_2$ soit l’ensemble des bijections de $Y_1$ dans $Y_2$, la composition des flèches étant donnée par la composition des applications. Montrer que G est essentiellement fini et calculer sa masse.

5) a) Soit $\varphi : G\rightarrow G'$ un morphisme de groupoïdes tel que l’application Som($\varphi$ ) soit injective. Démontrer que $\varphi (G)$ est un sous-groupoïde de $G'$.

b) Soit G un groupoïde non transitif dont l’ensemble de sommets Som(G) est un ensemble $\{a, b\}$ à deux éléments. Soit $G'$ le groupoïde associé au produit libre $G_a*G_b$. Il existe un unique morphisme de groupoïdes $\varphi : G\rightarrow G'$ tel que les applications $\varphi_a$ et $\varphi_b$ soient les applications canoniques de $G_a$ et $G_b$ dans $G_a*G_b$. Si $G_a$ ou $G_b$ n’est pas le groupe trivial, l’image $\varphi (G)$ de ce morphisme de groupoïdes n’est pas un sous-groupoïde de $G'$.

6) Soient G et $G'$ des graphes et soit $\varphi : G'\rightarrow G$. On dit que $(G', \varphi )$ est un revêtement de G si, pour tout sommet $a\in$ Som(G$')$ et toute flèche $f\in$ Fl(G) d’origine Som($\varphi$ )$(a)$, il existe une unique flèche $f'\in$ Fl(G$')$ d’origine $a$ telle que Fl($\varphi$ )$(f') =f$.

On suppose que $(G', \varphi )$ est un revêtement de G.

a) Démontrer qu’il existe une unique opération de Grp(G) dans Som(G$')$, relativement à l’application Som($\varphi$ ), telle que $x\cdot$ Fl($\varphi$ )$(f) =t(f)$, pour tout sommet $x\in$ Som(G$')$ et toute flèche $f\in$ Fl(G$')$ d’origine $x$.

b) En déduire que si $x$ et $y$ sont des sommets de G appartenant à une même composante connexe de G, on a Card(Som($\varphi$ )$^{-1}(x)) =$ Card(Som($\varphi$ )$^{-1}(y))$.

7) Soit G un graphe et soient $(G_1, \varphi_1)$, $(G_2, \varphi_2)$ des revêtements du graphe G.

a) Soit $\psi : G_1\rightarrow G_2$ un morphisme de graphes tel que $\varphi_2\circ \psi =\varphi_1$. Démontrer que l’on a $\psi (x\cdot \gamma ) =\psi (x)\cdot \gamma$ pour tout $x\in$ Som(G$_1)$ et toute flèche $\gamma$ de $\varpi_G$ d’origine $\varphi_1(x)$.

b) Soit $u:$ Som(G$_1)\rightarrow$ Som(G$_2)$ une application telle que $u(x\cdot \gamma ) =u(x)\cdot \gamma$ pour tout $x\in$ Som(G$_1)$ et toute flèche $\gamma$ de $\varpi_G$ d’origine $\varphi_1(x)$. Démontrer qu’il existe un unique morphisme de graphes $\psi : G_1\rightarrow G_2$ tel que $\varphi_2\circ \psi =\varphi_1$ et Som($\psi$ ) $=u$.

c) Soit X un ensemble et soit $p: X\rightarrow$ Som(G) une application. Supposons donnée une opération de $\varpi_G$ dans l’ensemble X relativement à l’application $p$. Démontrer qu’il existe un graphe $G'$ d’ensemble de sommets X et un morphisme de graphes $\varphi : G'\rightarrow G$ tel que Som($\varphi$ ) $=p$, de sorte que $(G', \varphi )$ soit un revêtement de G et que l’opération de $\varpi_G$ dans Som(G$')$ coïncide avec l’opération donnée.

8) Soit G un graphe connexe et soit $a$ un sommet de G.

a) Soient $(G_1, \varphi_1)$ et $(G_2, \varphi_2)$ des revêtements du graphe G. Soit $u:$ Som(G$_1)\rightarrow$ Som(G$_2)$ une application telle que $u(x)\cdot \gamma$ = $u(x\cdot \gamma )$ pour tout $\gamma \in \varpi_{G,a}$ et tout sommet $x$ de $G_1$ tel que Som($\varphi_1$)$(x) =a$. Démontrer qu’il existe un unique morphisme de graphes $\psi : G_1\rightarrow G_2$ tel que $\psi =$ Som($u$).

b) Soit X un ensemble muni d’une opération du groupe $\varpi_{G,a}$. Démontrer qu’il existe un revêtement $(G', \varphi )$ du graphe G tel que Som($\varphi$ )$^{-1}(a) = X$ et tel que l’opération de $\varpi_G$ dans Som(G$')$ induise l’opération donnée de $\varpi_{G,a}$ dans X.

9) Soient G et $G'$ des graphes et soit $\varphi : G'\rightarrow G$ un morphisme de graphes tel que $(G', \varphi )$ est un revêtement de G.

a) Démontrer que le graphe $\varphi$(Grp(G$'))$ est un sous-groupoïde du groupoïde Grp(G).

b) Démontrer que, pour tout sommet $a$ de $G'$, l’homomorphisme de groupes $\pi_1(\varphi , a)$ est injectif.

c) On suppose que G est connexe et on fixe un sommet $a$ de G. Soit K un sous-groupe de $\varpi_{G,a}$. Démontrer qu’il existe un revêtement $(H, \psi )$ du graphe G et un sommet $b$ de H tel que $\psi (b) =a$ et K soit l’image du morphisme $\pi_1(\psi , a)$.

d) Démontrer qu’un sous-groupe d’un groupe libre est libre (voir aussi IV, p. 417, exemple 2).

e) Soient $n$ et $q$ des entiers ; si F est un groupe libre à $n$ générateurs et K un sous-groupe de F d’indice $q$, démontrer que K est un groupe libre à $1+q(n-1)$ générateurs.

10) Soient F un ensemble, C une partie de $F\times F$ et $m: C\rightarrow F$ une application. On fait les hypothèses suivantes :

(i) Les applications de C dans $F\times F$ données par $(f, g)\mapsto (f, m(f, g))$ et $(f, g)\mapsto (m(f, g), g)$ sont injectives ;

(ii) Si $f,g,h\in F$ sont tels que les couples $(f, g)$ et $(g, h)$ appartiennent à C, alors les couples $(f, m(g, h))$ et $(m(f, g), h)$ appartiennent à C et l’on a $m(f, m(g, h)) =m(m(f, g), h)$ ;

(iii) Pour tout $f\in F$, il existe des éléments $o(f),t(f)$ et $f\in F$, nécessairement uniques en vertu de (i), tels que les couples $(f, t(f))$, $(o(f), f)$, $(f, f)$, $(f , f)$ appartiennent à C et que l’on ait $m(f, t(f)) =f=m(o(f), f)$ et $m(f, f) =o(f)$.

a) Démontrer que, pour tout $f\in F$, on a $(f , f)\in C$ et $m(f , f) =t(f)$. En déduire que $(o(f), o(f))\in C$ et $m(o(f), o(f)) =o(f)$. Démontrer aussi que $o(f) =t(f)$ et $f=f$.

b) Soit S l’ensemble des éléments $e$ de F tels que $(e, e)\in C$ et $m(e, e) =e$; notons $o$ et $t$ les applications de F dans S données par $f\mapsto o(f)$ et $f\mapsto t(f)$.

Démontrer que le quadruplet $\Gamma  = (S,F, o, t)$ est un carquois et que l’application $m$ est une loi de composition dans Γ qui en fait un groupoïde. (Cette construction est due à H. Brandt ; cf. « Über eine Verallgemeinerung des Gruppenbegriffes », Mathematische Annalen (1926), vol. 96, p. 360–366.)

11) Soit G un groupoïde ; soit C l’ensemble des couples de flèches composables de G et soit $m: C\rightarrow$ Fl(G) la loi de composition de G.

a) Démontrer que C et $m$ vérifient les hypothèses (i), (ii), (iii) de l’exercice 10. On note Γ le groupoïde fourni par la construction de cet exercice. b) Démontrer que le couple formé de l’application $e\mapsto o(e)$ de Som(Γ) dans Som(G) et de l’application identique de l’ensemble Fl(G) dans lui-même est un isomorphisme de groupoïdes de Γ sur G.

Cela démontre qu’un groupoïde est déterminé par l’ensemble de ses flèches et sa loi de composition.

12) Soit G un groupe, soit S l’ensemble des sous-groupes de G et soit F l’ensemble des sous-ensembles X de G tels qu’il existe un sous-groupe H de G et un élément $g$ de G tel que $X =gH$.

a) Soit $\mu$ l’application de $G\times G\times G$ dans G définie par $\mu(x, y, z) =xy^{-1}z$. Démontrer qu’un sous-ensemble non vide X de G appartient à l’ensemble F si et seulement si $\mu(X\times X\times X)\subset X$.

b) Montrer qu’en posant $o(X) =g^{-1}X$ et $t(X) = Xg^{-1}$, pour un élément $g$ de X quelconque, on définit des applications $o: F\rightarrow S$ et $t: F\rightarrow S$.

c) Si $X_1$ et $X_2$ sont des éléments de S tels que $t(X_1) =o(X_2)$, on pose $m(X_1,X_2) = X_1X_2$. Démontrer que l’application $m$ est une loi de composition dans le carquois $(S,F, o, t)$ qui en fait un groupoïde (« groupoïde de Baer »). On le note Ba(G).

d) Démontrer que les orbites de Ba(G) sont les classes de conjugaison de sous-groupes de G.

e) Démontrer que le groupe d’isotropie de Ba(G) en un élément H de S est isomorphe au groupe quotient $N(H)/H$.

§5

1) Soient G un groupoïde, X un ensemble et $f$ une application de Som(G) dans X.

a) Démontrer qu’il existe un couple $(K, \alpha )$, où K est un groupoïde d’ensemble de sommets X et $\alpha : G\rightarrow K$ est un morphisme de groupoïdes tel que Som($\alpha$ ) $=f$, vérifiant la propriété universelle suivante : pour tout groupoïde H d’ensemble de sommets X et tout morphisme $\varphi : G\rightarrow H$ tel que Som($\varphi$ ) $=f$, il existe un unique morphisme de groupoïdes $\psi : K\rightarrow H$ tel que $\alpha \circ \psi =\varphi$. (Si S est un ensemble, on note $S_d$ un groupoïde d’ensemble de sommets S dont les orbites et les groupes d’isotropie sont réduits à un élément. Soit $G'$ le groupoïde somme disjointe de la famille $(G,X_d)$, soient $\varphi$ et $\psi$ les morphismes du groupoïde Som(G)$_d$ dans $G'$ tels que Som($\varphi$ ) soit l’injection canonique de Som(G) dans Som(G$')$ et Som($\psi$ ) $=f$ respectivement. Poser K = Coeg($\varphi , \psi$ ).)

b) En déduire une bijection de Hom(G$, f^*H)$ sur Hom(K$,H)$, pour tout groupoïde H d’ensemble de sommets X.

2) Soient H et G des groupes, soient $\mathscr{H}$ et $\mathscr{G}$ les groupoïdes qui leur sont associés ; soient $\varphi$ et $\psi$ des morphismes de groupoïdes de $\mathscr{H}$ dans $\mathscr{G}$.

a) Démontrer que l’ensemble des sommets du cohomotopeur (resp. du coégalisateur) du couple $(\varphi , \psi )$ est réduit à un élément ; on note K (resp. L) son groupe d’isotropie en ce point.

b) Démontrer que le groupe K est le quotient du produit libre $G*\mathbf{Z}$ par le plus petit sous-groupe distingué de $G*\mathbf{Z}$ qui contient les éléments $\varphi (g)t\psi (g)^{-1}t^{-1}$, pour $g\in G$, où $t$ désigne l’élément 1 de $\mathbf{Z}$.

c) Démontrer que le groupe L est le quotient du groupe G par le plus petit sous-groupe distingué contenant les éléments $\varphi (g)\psi (g)^{-1}$, pour $g\in G$.

3) Soit I un ensemble préordonné et soit $(G_i)_{i\in I}$ une famille de groupoïdes. Pour tout couple $(i, j)$ d’éléments de I tels que $i\leqslant j$, soit $\varphi_{ji}$ un morphisme de groupoïdes de $G_i$ dans $G_j$. On suppose que les $\varphi_{ji}$ vérifient les conditions suivantes (cf. E, III, p. 61) :

(i) Les relations $i\leqslant j\leqslant k$ entraînent $\varphi_{ki}=\varphi_{kj}\circ \varphi_{ji}$;

(ii) Pour tout $i\in I,f_{ii}$ est le morphisme identique de $G_i$.

Soit G le groupoïde somme de la famille $(G_i)$, soit H le groupoïde somme de la famille $(H_{ji})_{i\leqslant j}$, où l’on a posé $H_{ji}= G_i$ pour tout couple $(i, j)$. Soit $\varphi$ (resp. $\psi )$ le morphisme de H dans G induit par la famille $(\varphi_{ji})_{i\leqslant j}$ (resp. (Id$_{G_i})_{i\leqslant j})$ et soit C le coégalisateur du couple $(\varphi , \psi )$. Pour $i\in I$, soit $\varphi_i$ le morphisme de $G_i$ dans C, composé du morphisme canonique de $G_i$ dans G et du morphisme canonique de G dans C.

a) Démontrer que l’on a $\varphi_j\circ \varphi_{ji}=\varphi_i$ pour tout couple $(i, j)$ tel que $i\leqslant j$. b) Démontrer que, pour tout groupoïde D et toute famille $(g_i)$, où $g_i$ est un morphisme de $G_i$ dans D tel que $g_j\circ \varphi_{ji}=g_i$ pour tout couple $(i, j)$ tel que $i\leqslant j$, il existe un unique morphisme de groupoïdes $g: C\rightarrow D$ tel que $g\circ \varphi_i=g_i$ pour tout $i\in I$.
