---
book: alg
book_title: Algebra
chapter: II
chapter_title: ALGÈBRE LINÉAIRE
section: 1
section_title: Modules
lang: fr
source: alg-i-iii-fr
pdf_pages: 0178-0212, 0355-0360
extraction: ocr
subsections:
    - "no": 1
      title: Modules; espaces vectoriels; combinaisons linéaires
      page: 0
      pdf_page: 178
    - "no": 2
      title: Applications linéaires
      page: 4
      pdf_page: 181
    - "no": 3
      title: Sous-modules; modules quotients
      page: 6
      pdf_page: 183
    - "no": 4
      title: Suites exactes
      page: 8
      pdf_page: 185
    - "no": 5
      title: Produits de modules
      page: 10
      pdf_page: 187
    - "no": 6
      title: Somme directe de modules
      page: 12
      pdf_page: 189
    - "no": 7
      title: Intersection et somme de sous-modules
      page: 15
      pdf_page: 192
    - "no": 8
      title: Sommes directes de sous-modules
      page: 17
      pdf_page: 194
    - "no": 9
      title: Sous-modules supplémentaires
      page: 19
      pdf_page: 196
    - "no": 10
      title: Modules de longueur finie
      page: 21
      pdf_page: 198
    - "no": 11
      title: Familles libres. Bases
      page: 24
      pdf_page: 201
    - "no": 12
      title: Annulateurs. Modules fidèles. Modules monogènes
      page: 28
      pdf_page: 205
    - "no": 13
      title: Changement de l’anneau des scalaires
      page: 30
      pdf_page: 207
    - "no": 14
      title: Multimodules
      page: 33
      pdf_page: 210
statements: 96
exercises: 27
content_sha256: 70660bee3256308a3ef902dfb46e26259e40fb888e027c7207e49c6d0d0b3f0e
---

## § 1. MODULES

### 1. Modules; espaces vectoriels; combinaisons linéaires

#### Définition 1 {#alg-ii-s1-def-1 .statement}

Étant donné un anneau $\mathbf{A}$, on appelle module à gauche sur $\mathbf{A}$ (ou $\mathbf{A}$-module à gauche), un ensemble $\mathbf{E}$ muni d’une structure algébrique définie par la donnée:
$1^\circ$ d’une loi de groupe commutatif dans $\mathbf{E}$ (notée additivement dans ce qui suit);
$2^\circ$ d’une loi d’action $(\alpha, x) \mapsto \alpha \top x$, dont le domaine d’opérateurs est l’anneau $\mathbf{A}$, et qui satisfait aux axiomes suivants:
$$
\begin{align*}
(\mathbf{M_I})\ \alpha \top (x + y) &= (\alpha \top x) + (\alpha \top y)\ \text{quels que soient}\ \alpha \in \mathbf{A},\ x \in \mathbf{E},\ y \in \mathbf{E}; \\
(\mathbf{M_{II}})\ (\alpha + \beta) \top x &= (\alpha \top x) + (\beta \top x)\ \text{quels que soient}\ \alpha \in \mathbf{A},\ \beta \in \mathbf{A},\ x \in \mathbf{E}; \\
(\mathbf{M_{III}})\ \alpha \top (\beta \top x) &= (\alpha \beta) \top x\ \text{quels que soient}\ \alpha \in \mathbf{A},\ \beta \in \mathbf{A},\ x \in \mathbf{E}; \\
(\mathbf{M_{IV}})\ 1 \top x &= x\ \text{pour tout}\ x \in \mathbf{E}.
\end{align*}
$$

L’axiome $(M_I)$ signifie que la loi d’action de $A$ sur $E$ est *distributive* par rapport à l’addition dans $E$; un module est donc un groupe commutatif à opérateurs.

Si dans la déf. 1, on remplace l’axiome $(M_{III})$ par

$$(M'_{III})\ \alpha \top (\beta \top x) = (\beta \alpha) \top x\ quels\ que\ soient\ \alpha \in A,\ \beta \in A,\ x \in E,$$

on dit que $E$, muni de la structure algébrique ainsi définie, est un *module à droite sur* $A$, ou encore un *A-module à droite*.

Lorsqu’on parle de $A$-modules (à gauche ou à droite), les éléments de l’anneau $A$ sont souvent appelés *scalaires*.

Le plus souvent, la loi d’action d’un module à gauche (resp. d’un module à droite) se note *multiplicativement*, en écrivant l’opérateur à gauche (resp. à droite); la condition $(M_{III})$ s’écrit alors $\alpha(\beta x) = (\alpha \beta)x$, la condition $(M'_{III})$ s’écrit $(x \beta)\alpha = x(\beta \alpha)$.

Si $A^0$ désigne l’anneau *opposé* à $A$ (I, p. 96), tout module *à droite* $E$ sur l’anneau $A$ est un module *à gauche* sur l’anneau $A^0$. Il en résulte que l’on peut exposer les propriétés des modules en se bornant systématiquement, soit aux modules à gauche, soit aux modules à droite; dans les §§ 1 et 2, nous ferons en général cet exposé pour les modules *à gauche*, et lorsque nous parlerons d’un *module* (sans préciser), il s’agira d’un module à gauche, dont la loi d’action sera notée multiplicativement. Lorsque l’anneau $A$ est *commutatif*, les notions de module à droite et de module à gauche par rapport à $A$ sont identiques.

Pour tout $\alpha \in A$, l’application $x \mapsto \alpha x$ d’un $A$-module $E$ dans lui-même s’appelle l’*homothétie de rapport* $\alpha$ de $E$ (I, p. 30); d’après $(M_I)$, une homothétie est un endomorphisme de la structure de groupe commutatif (*sans opérateur*) de $E$, mais *non* en général de la structure de module de $E$ (I, p. 30; cf. II, p. 4 et II, p. 32). On a donc $\alpha 0 = 0$ et $\alpha(-x) = -(\alpha x)$; si $\alpha$ est un élément *inversible* de $A$, l’homothétie $x \mapsto \alpha x$ est un *automorphisme* de la structure de groupe commutatif (*sans opérateur*) de $E$, car de la relation $y = \alpha x$, on tire, en vertu de $(M_{IV})$, $x = \alpha^{-1}(\alpha x) = \alpha^{-1}y$.

De même, en vertu de $(M_{II})$, pour tout $x \in E$, l’application $\alpha \mapsto \alpha x$ est un homomorphisme du groupe additif $A$ dans le groupe commutatif (*sans opérateur*) $E$; on a donc $0x = 0$ et $(- \alpha)x = -(\alpha x)$; en outre, d’après $(M_{IV})$, on a, pour tout entier $n \in \mathbf{Z}$, $n.x = (n.1)x$.

Lorsque l’anneau $A$ est réduit au seul élément 0, *tout* $A$-module $E$ est aussi réduit à l’élément 0, car on a alors $1 = 0$ dans $A$, d’où, pour tout $x \in E$, $x = 1.x = 0.x = 0$.

#### Exemple 1 {#alg-ii-s1-n1-exa-1 .statement}

Soit $\varphi$ un homomorphisme d’un anneau $A$ dans un anneau $B$; l’application $(a, x) \mapsto \varphi(a)x$ (resp. $(a, x) \mapsto x \varphi(a)$) de $A \times B$ dans $B$ définit sur $B$ une structure de $A$-module à gauche (resp. à droite). Quand on prend en particulier pour $\varphi$ l’application identique de $A$ on obtient sur $A$ une structure canonique de A-module à gauche (resp. à droite); on notera $A_s$ (resp. $A_d$) l’ensemble A muni de cette structure, pour éviter des confusions.

#### Exemple 2 {#alg-ii-s1-n1-exa-2 .statement}

Sur un groupe commutatif G (noté additivement), la structure de groupe à opérateurs définie par la loi d’action $(n, x) \mapsto n.x$ (I, p. 24) est une structure de module sur l’anneau $\mathbf{Z}$ des entiers rationnels.

#### Exemple 3 {#alg-ii-s1-n1-exa-3 .statement}

Soient E un groupe commutatif noté additivement, $\mathcal{E}$ l’anneau des endomorphismes de E (I, p. 96: on rappelle que le produit $fg$ de deux endomorphismes est par définition l’endomorphisme composé $f \circ g$). La loi d’action $(f, x) \mapsto f(x)$ entre opérateurs $f \in \mathcal{E}$ et éléments $x \in E$ définit sur E une structure canonique de $\mathcal{E}$-module à gauche.

Considérons maintenant un anneau A et supposons donnée sur E une structure de A-module à gauche (resp. à droite); pour tout $\alpha \in A$, l’homothétie $h_\alpha : x \mapsto \alpha x$ (resp. $x \mapsto x\alpha$) appartient à $\mathcal{E}$; l’application $\varphi : \alpha \mapsto h_\alpha$ est un homomorphisme de l’anneau A (resp. de l’anneau opposé $A^0$) dans l’anneau $\mathcal{E}$ et on a par définition $\alpha x = (\varphi(\alpha))(x)$ (resp. $x\alpha = (\varphi(\alpha))(x)$). Réciproquement, la donnée d’un homomorphisme d’anneaux $\varphi : A \to \mathcal{E}$ (resp. $\varphi : A^0 \to \mathcal{E}$) définit sur E une structure de A-module à gauche (resp. à droite) par les formules précédentes. Autrement dit, se donner une structure de A-module à gauche (resp. à droite) sur un groupe additif E, ayant pour loi additive la loi de groupe donnée, équivaut à se donner un homomorphisme d’anneaux $A \to \mathcal{E}$ (resp. $A^0 \to \mathcal{E}$).

#### Définition 2 {#alg-ii-s1-def-2 .statement}

On appelle espace vectoriel à gauche (resp. à droite) sur un corps K, un K-module à gauche (resp. à droite).

Les éléments d’un espace vectoriel sont parfois appelés vecteurs.

#### Exemple 4 {#alg-ii-s1-n1-exa-4 .statement}

Un corps est à la fois espace vectoriel à gauche et à droite par rapport à un quelconque de ses sous-corps.

#### Exemple 5 {#alg-ii-s1-n1-exa-5 .statement}

L’espace numérique à 3 dimensions $\mathbf{R}^3$ est un espace vectoriel par rapport au corps des nombres réels $\mathbf{R}$, le produit $tx$ d’un nombre réel t et d’un point x de coordonnées $x_1, x_2, x_3$ étant le point de coordonnées $tx_1, tx_2, tx_3$. De même, l’ensemble des fonctions numériques définies dans un ensemble quelconque F est un espace vectoriel par rapport à $\mathbf{R}$, le produit $tf$ d’un nombre réel t et d’une fonction f étant la fonction numérique $x \mapsto tf(x)$*

Pour deux familles $(x_i)_{i \in I}, (y_i)_{i \in I}$ d’éléments d’un A-module E, de support fini (I, p. 13), on a les formules

(1)
$$
\sum_{i \in I} (x_i + y_i) = \sum_{i \in I} x_i + \sum_{i \in I} y_i
$$

(2)
$$
\alpha \sum_{i \in I} x_i = \sum_{i \in I} (\alpha x_i) \quad \text{pour tout } \alpha \in A;
$$

on se ramène en effet aussitôt aux formules analogues pour les sommes finies en considérant une partie finie H de I contenant les supports de $(x_i)$ et $(y_i)$.

#### Définition 3 {#alg-ii-s1-def-3 .statement}

On dit qu’un élément x d’un A-module E est une combinaison linéaire, à coefficients dans $A$, d’une famille $(a_i)_{i \in I}$ d’éléments de $E$, s’il existe une famille $(\lambda_i)_{i \in I}$ d’éléments de $A$, de support fini, telle que $x = \sum_{i \in I} \lambda_i a_i$.

En général il y a plusieurs familles distinctes $(\lambda_i)$ vérifiant cette condition (cf. II, p. 25).

On notera que 0 est la seule combinaison linéaire de la famille vide d’éléments de $E$ (d’après la convention de I, p. 13).

### 2. Applications linéaires

#### Définition 4 {#alg-ii-s1-def-4 .statement}

Soient $E$ et $F$ deux modules (à gauche) par rapport au même anneau $A$. On appelle application linéaire (ou application A-linéaire, ou homomorphisme, ou A-homomorphisme) de $E$ dans $F$ toute application $u : E \to F$ telle que:

(3) $$
u(x + y) = u(x) + u(y) \quad \text{pour } x \in E, y \in E;
$$
(4G) $$
u(\lambda \cdot x) = \lambda \cdot u(x) \quad \text{pour } \lambda \in A, x \in E.
$$

Si $E$ et $F$ sont deux $A$-modules à droite, une application linéaire $u : E \to F$ est une application vérifiant (3) et
(4D) $$
u(x \cdot \lambda) = u(x) \cdot \lambda \quad \text{pour } \lambda \in A, x \in E.
$$

#### Remarque {#alg-ii-s1-n2-rem-1 .statement}

Lorsque $E$ et $F$ sont deux groupes commutatifs, considérés comme modules sur l’anneau $\mathbf{Z}$ (II, p. 3), tout homomorphisme $u$ du groupe $E$ (sans opérateur) dans le groupe $F$ (sans opérateur) est aussi une application linéaire de $E$ dans $F$, car pour $n$ entier $> 0$ la relation $u(n \cdot x) = n \cdot u(x)$ se déduit de $u(x + y) = u(x) + u(y)$ par récurrence sur $n$, et pour $n = -m < 0$, on a encore $u(n \cdot x) = u(-(m \cdot x)) = -u(m \cdot x) = -(m \cdot u(x)) = n \cdot u(x)$.

#### Exemple 1 {#alg-ii-s1-n2-exa-1 .statement}

Soient $E$ un $A$-module, $a$ un élément de $E$; l’application $\lambda \mapsto \lambda a$ du $A$-module $A_s$ dans $E$ est une application linéaire $\theta_a$, telle que $\theta_a(1) = a$.
\* 2) Soient $I$ un intervalle ouvert de la droite numérique $\mathbf{R}$, $E$ l’espace vectoriel des fonctions numériques dérivables dans $I$, $F$ l’espace vectoriel de toutes les fonctions numériques définies dans $I$. L’application $x \mapsto x'$ qui, à toute fonction dérivable $x$, fait correspondre sa dérivée, est une application linéaire de $E$ dans $F$*

On notera qu’une homothétie $x \mapsto \alpha x$ dans un $A$-module $E$ n’est pas nécessairement une application linéaire: en d’autres termes, on n’a pas nécessairement la relation $\alpha(\lambda x) = \lambda(\alpha x)$ quels que soient $\lambda \in A$ et $x \in E$. Cette relation est toutefois vraie lorsque $\alpha$ appartient au centre de $A$; on dit alors que $x \mapsto \alpha x$ est une homothétie centrale (cf. II, p. 32).

Si $u : E \to F$ est une application linéaire, on a, pour toute famille $(x_i)_{i \in I}$ d’éléments de $E$ et toute famille $(\lambda_i)_{i \in I}$ d’éléments de $A$, telles que le support de la famille $(\lambda_i x_i)_{i \in I}$ soit fini,
(5) $$
u\left( \sum_{i \in I} \lambda_i x_i \right) = \sum_{i \in I} \lambda_i u(x_i)
$$

comme il résulte aussitôt de (3) et (4G) par récurrence sur le cardinal du support de la famille $(\lambda_i x_i)$.

#### Proposition 1 {#alg-ii-s1-prop-1 .statement}

*Soient E, F, G trois A-modules, u une application linéaire de E dans F, v une application linéaire de F dans G. Alors l’application composée $v \circ u$ est linéaire.*

#### Proposition 2 {#alg-ii-s1-prop-2 .statement}

*Soient E, F deux A-modules.
1° Si $u : E \to F$ et $v : F \to E$ sont deux applications linéaires telles que $v \circ u$ soit l’application identique de E et $u \circ v$ l’application identique de F, u est un isomorphisme de E sur F et v l’isomorphisme réciproque.
2° Toute application linéaire bijective $u : E \to F$ est un isomorphisme de E sur F.*
Ces propositions découlent aussitôt de la déf. 4.

Les prop. 1 et 2 montrent que l’on peut prendre pour *morphismes* de l’espèce de structure de A-module les applications linéaires (E, IV, p. 11); nous supposerons toujours par la suite que l’on a fait ce choix de morphismes.

Étant donnés deux A-modules à gauche (resp. à droite) E et F, on notera Hom(E, F) ou Hom_A(E, F) l’ensemble des applications linéaires de E dans F.

L’ensemble Hom(E, F) est un *groupe commutatif*, sous-groupe du groupe commutatif produit $F^E$ de toutes les applications de E dans F (I, p. 43); on rappelle en effet que l’on a pour deux éléments $u, v$ de $F^E$, et pour tout $x \in E$,

$$(u + v)(x) = u(x) + v(x), \quad (-u)(x) = -u(x)$$

d’où résulte aussitôt que si $u$ et $v$ sont linéaires, il en est de même de $u + v$ et de $-u$. Si G est un troisième A-module à gauche (resp. à droite), $f, f_1, f_2$ des éléments de Hom(E, F), $g, g_1, g_2$ des éléments de Hom(F, G), on vérifie aussitôt les relations

(6) $$g \circ (f_1 + f_2) = g \circ f_1 + g \circ f_2$$
(7) $$(g_1 + g_2) \circ f = g_1 \circ f + g_2 \circ f$$
(8) $$g \circ (-f) = (-g) \circ f = -(g \circ f).$$

En particulier, la loi de composition $(f, g) \mapsto f \circ g$ sur Hom(E, E) définit, avec la structure de groupe additif précédente, une structure d’*anneau* sur Hom(E, E), dont l’élément unité, noté $1_E$ ou Id_E, est l’application identique de E; les applications linéaires de E dans lui-même sont encore appelées *endomorphismes* du A-module E et l’anneau Hom(E, E) se note encore End(E) ou End_A(E). Les *automorphismes* du A-module E ne sont autres que les éléments *inversibles* de End(E) (prop. 2); ils forment un *groupe* multiplicatif, noté Aut(E) ou $\mathbf{GL}(E)$, que l’on appelle aussi le *groupe linéaire* relatif à E.

Il résulte de (6) et (7) que pour deux A-modules E, F, Hom(E, F) est muni canoniquement d’une structure de module à gauche sur l’anneau Hom(F, F) et de module à droite sur l’anneau Hom(E, E).

Soient E, F, E', F' quatre A-modules (à gauche), u : E' → E et v : F → F' des applications A-linéaires. Si, à tout élément f ∈ Hom(E, F), on fait correspondre l’élément v ∘ f ∘ u ∈ Hom(E', F'), on définit une application

$$
\operatorname{Hom}(E, F) \to \operatorname{Hom}(E', F')
$$

qui est $\mathbf{Z}$-linéaire et que nous noterons $\operatorname{Hom}(u, v)$ ou $\operatorname{Hom}_A(u, v)$. Si $u, u_1, u_2$ appartiennent à $\operatorname{Hom}(E', E)$, $v, v_1, v_2$ à $\operatorname{Hom}(F, F')$, on a

$$
\begin{cases}
\operatorname{Hom}(u_1 + u_2, v) = \operatorname{Hom}(u_1, v) + \operatorname{Hom}(u_2, v) \\
\operatorname{Hom}(u, v_1 + v_2) = \operatorname{Hom}(u, v_1) + \operatorname{Hom}(u, v_2).
\end{cases}
$$

(9)

Soient E", F" deux A-modules, $u' : E'' \to E'$, $v' : F' \to F''$ des applications linéaires. On a

$$
\operatorname{Hom}(u \circ u', v' \circ v) = \operatorname{Hom}(u', v') \circ \operatorname{Hom}(u, v).
$$

(10)

Si $u$ est un isomorphisme de E' sur E et $v$ un isomorphisme de F sur F', $\operatorname{Hom}(u, v)$ est un isomorphisme de $\operatorname{Hom}(E, F)$ sur $\operatorname{Hom}(E', F')$, dont l’isomorphisme réciproque est $\operatorname{Hom}(u^{-1}, v^{-1})$ d’après (10).

Si $h$ (resp. $k$) est un endomorphisme de E (resp. F), $\operatorname{Hom}(h, 1_F)$ (resp. $\operatorname{Hom}(1_E, k)$) n’est autre que l’homothétie de rapport $h$ (resp. $k$) pour la structure de module à droite (resp. à gauche) sur l’anneau End(E) (resp. End(F)) définie plus haut.

### 3. Sous-modules; modules quotients

Soient E un A-module, M une partie de E ; pour que la structure de A-module de E induise sur M une structure de A-module, il faut et il suffit que M soit un sous-groupe stable de E (I, p. 31), car lorsqu’il en est ainsi, la structure de groupe à opérateurs induite sur M vérifie évidemment les axiomes (M_{II}), (M_{III}) et (M_{IV}) ; alors M, muni de cette structure (ou, par abus de langage, l’ensemble M lui-même) est appelé sous-module de E ; l’injection canonique M → E est une application linéaire. Lorsque E est un espace vectoriel, ses sous-modules s’appellent aussi sous-espaces vectoriels (ou simplement sous-espaces si aucune confusion n’en résulte).

#### Exemple 1 {#alg-ii-s1-n3-exa-1 .statement}

Dans un module quelconque E, l’ensemble réduit à 0 est un sous-module (sous-module nul, souvent noté 0 par abus de notation).
2) Soit A un anneau. Les sous-modules de A_s (resp. A_d) ne sont autres que les idéaux à gauche (resp. idéaux à droite) de l’anneau A (I, p. 98).
3) Soient E un A-module, x un élément de E, a un idéal à gauche de A. L’ensemble des éléments $\alpha x$, où $\alpha$ parcourt a, est un sous-module de E, qu’on note $\alpha x$.

4) Dans un groupe commutatif G, considéré comme $\mathbf{Z}$-module (II, p. 3), tout sous-groupe de G est aussi un sous-module.

\* 5) Soit I un intervalle ouvert de la droite numérique $\mathbf{R}$; l’ensemble C des fonctions numériques définies et continues dans I est un sous-espace vectoriel de l’espace vectoriel $\mathbf{R}^I$ de toutes les fonctions numériques définies dans I. De même, l’ensemble D des fonctions dérivables dans I est un sous-espace vectoriel de C.*

Soit E un A-module. Toute relation d’équivalence compatible (I, p. 11) avec la structure de module de E est de la forme $x - y \in M$, où M est un sous-groupe stable de E (I, p. 33), c’est-à-dire un sous-module de E. On vérifie immédiatement que la structure de groupe à opérateurs du groupe quotient E/M (I, p. 35) est une structure de A-module, pour laquelle l’application canonique $E \to E/M$ est linéaire; muni de cette structure, E/M est appelé module quotient de E par le sous-module M. Un module quotient d’un espace vectoriel E s’appelle espace vectoriel quotient (ou simplement espace quotient) de E.

Exemple 6). — Tout idéal à gauche $a$ dans un anneau A définit un module quotient $A_s/a$ du A-module à gauche $A_s$; par abus de notation, ce module quotient s’écrit souvent $A/a$.

Soient E, F deux A-modules. Il résulte des propriétés générales des groupes à opérateurs (I, p. 36) (ou directement des définitions) que si $u : E \to F$ est une application linéaire, l’image par u de tout sous-module de E est un sous-module de F et l’image réciproque par u de tout sous-module de F est un sous-module de E. En particulier, le noyau $N = \overline{u}^{-1}(0)$ est un sous-module de E et l’image $u(E)$ de E par u est un sous-module de F (I, p. 37, prop. 7); on dit par abus de langage que $u(E)$ est l’image de u. Le module quotient $E/N$ s’appelle aussi la coïmage de u et le module quotient $F/u(E)$ le conoyau de u. Dans la décomposition canonique de u (I, p. 37)

$$
u : E \xrightarrow{\rho} E/N \xrightarrow{v} u(E) \xrightarrow{i} F
$$

$v$ est un isomorphisme de la coïmage de u sur l’image de u (II, p. 5, prop. 2). Pour que u soit injective, il faut et il suffit que son noyau soit nul; pour que u soit surjective, il faut et il suffit que son conoyau soit nul.

Le noyau, l’image, la coïmage et le conoyau de u se notent respectivement Ker $u$, Im $u$, Coïm $u$, Coker $u$.

#### Remarque {#alg-ii-s1-n3-rem-1 .statement}

Soient M un sous-module d’un A-module E, $\varphi : E \to E/M$ l’homomorphisme canonique. Pour qu’une application A-linéaire $u : E \to F$ soit de la forme $v \circ \varphi$, où $v$ est une application linéaire de $E/M$ dans F, il faut et il suffit que $M \subset \mathrm{Ker}(u)$; en effet, si cette condition est vérifiée, la relation $x - y \in M$ entraîne $u(x) = u(y)$, donc u est compatible avec cette relation d’équivalence et il est clair que l’application $v : E/M \to F$ déduite de u par passage au quotient est linéaire.

### 4. Suites exactes

#### Définition 5 {#alg-ii-s1-def-5 .statement}

Soient F, G, H trois A-modules; soit f un homomorphisme de F dans G et soit g un homomorphisme de G dans H. On dit que le couple (f, g) est une suite exacte si l’on a

$$
\overline{g}^{-1}(0) = f(F)
$$

autrement dit, si le noyau de g est égal à l’image de f.

On dit aussi que le diagramme

(12)

$$
\begin{array}{ccc}
F & \xrightarrow{f} & G \\
& & \xrightarrow{g} \\
& & H
\end{array}
$$

est une suite exacte.

Considérons de même un diagramme formé de quatre A-modules et de trois homomorphismes:

(13)

$$
E \xrightarrow{f} F \xrightarrow{g} G \xrightarrow{h} H.
$$

On dit que ce diagramme est exact en F si le diagramme E $\xrightarrow{f} F \xrightarrow{g} G$ est exact; on dit qu’il est exact en G si F $\xrightarrow{g} G \xrightarrow{h} H$ est exact. Si le diagramme (13) est exact en F et en G, on dit simplement qu’il est exact, ou encore que c’est une suite exacte. On définit de même les suites exactes à un nombre quelconque de termes.

Remarque 1). — Si le couple (f, g) est une suite exacte, on a $g \circ f = 0$; mais bien entendu, cette propriété ne caractérise pas les suites exactes, car elle signifie seulement que l’image de f est contenue dans le noyau de g.

Dans les énoncés ci-dessous, E, F, G désignent des A-modules, 0 un A-module réduit à son élément neutre; les flèches représentent des homomorphismes de A-modules. Comme il n’y a qu’un seul homomorphisme du module 0 dans un module E (resp. de E dans 0), il sera inutile de désigner les homomorphismes de ce type plus explicitement dans les suites exactes où ils figurent.

#### Proposition 3 {#alg-ii-s1-prop-3 .statement}

a) Pour que

$$
\begin{array}{ccc}
0 & \longrightarrow & E \\
& & \xrightarrow{f} \\
& & F
\end{array}
$$

soit une suite exacte, il faut et il suffit que f soit injectif.

b) Pour que

$$
\begin{array}{ccc}
E & \xrightarrow{f} & F \\
& & \longrightarrow \\
& & 0
\end{array}
$$

soit une suite exacte, il faut et il suffit que f soit surjectif.

c) Pour que

$$
\begin{array}{ccc}
0 & \longrightarrow & E \\
& & \xrightarrow{f} \\
& & F \\
& & \longrightarrow \\
& & 0
\end{array}
$$

soit une suite exacte, il faut et il suffit que f soit bijectif (autrement dit (II, p. 5, prop. 2) que f soit un isomorphisme de E sur F).

d) Si F est un sous-module de E, et si i : F → E est l’injection canonique, p : E → E/F l’homomorphisme canonique, le diagramme

(14)
$$
0 \longrightarrow F \xrightarrow{i} E \xrightarrow{p} E/F \longrightarrow 0.
$$
est une suite exacte.

e) Si f : E → F est un homomorphisme, le diagramme
$$
0 \longrightarrow \overline{f}^{-1}(0) \xrightarrow{i} E \xrightarrow{f} F \xrightarrow{p} F/f(E) \longrightarrow 0
$$
(où i est l’injection canonique et p la surjection canonique) est une suite exacte.

La proposition résulte aussitôt des définitions et de la prop. 2 de II, p. 5.

#### Remarque 2 {#alg-ii-s1-n4-rem-2 .statement}

Dire qu’on a une suite exacte
$$
0 \longrightarrow E \xrightarrow{f} F \xrightarrow{g} G \longrightarrow 0
$$
signifie que f est injectif, g surjectif et que la bijection canonique associée à g est un isomorphisme de F/f(E) sur G. On dit encore alors que le triplet (F, f, g) est une extension du module G par le module E (I, p. 62).

#### Remarque 3 {#alg-ii-s1-n4-rem-3 .statement}

Si on a une suite exacte à 4 termes
$$
E \xrightarrow{f} F \xrightarrow{g} G \xrightarrow{h} H
$$
le conoyau de f est F/f(E) = F/\overline{g}^{-1}(0) et le noyau de h est g(F); la bijection canonique associée à g est donc un isomorphisme
$$
\operatorname{Coker} f \to \operatorname{Ker} h.
$$

#### Remarque 4 {#alg-ii-s1-n4-rem-4 .statement}

Considérons un couple d’homomorphismes de A-modules
(15)
$$
E \xrightarrow{f} F \xrightarrow{g} G.
$$
Pour que le diagramme (15) soit une suite exacte, il faut et il suffit qu’il existe deux A-modules S, T et des homomorphismes a : E → S, b : S → F, c : F → T, d : T → G tels que les trois suites
(16)
$$
\begin{cases}
E \xrightarrow{a} S \longrightarrow 0 \\
0 \longrightarrow S \xrightarrow{b} F \xrightarrow{c} T \longrightarrow 0 \\
0 \longrightarrow T \xrightarrow{d} G
\end{cases}
$$
soient exactes, et que l’on ait f = b ∘ a et g = d ∘ c.

En effet, si (15) est une suite exacte, on prend S = f(E) = \overline{g}^{-1}(0) et T = g(F), b et d étant les injections canoniques, a (resp. c) l’homomorphisme ayant même graphe que f (resp. g). Réciproquement, si S, T, a, b, c, d vérifient les conditions ci-dessus, on a f(E) = b(a(E)) = b(S) et \overline{g}^{-1}(0) = \overline{c}^{-1}(\overline{d}^{-1}(0)) = \overline{c}^{-1}(0), donc l’exactitude de (16) montre que f(E) = \overline{g}^{-1}(0).

On se dispensera souvent de désigner explicitement par des lettres les homomorphismes d’une suite exacte, lorsque cela n’est pas nécessaire dans les raisonnements.

Remarque 5). — La définition d’une suite exacte s’étend aussitôt aux groupes non nécessairement commutatifs; on utilisera naturellement dans ce cas la notation multiplicative, 0 étant remplacé par 1 dans les formules (si aucune confusion n’en résulte). Les parties $a), b), c)$ de la prop. 3 sont encore valables, ainsi que d) lorsque F est un sous-groupe distingué de E. La Remarque 2 et la prop. 3 e) subsistent lorsqu’on ajoute que $f(E)$ doit être un sous-groupe distingué de F; les Remarques 3 et 4 sont valables sans modification.

### 5. Produits de modules

Soit $(E_i)_{i \in I}$ une famille de modules sur un même anneau A. On vérifie immédiatement que, sur l’ensemble produit $E = \prod_{i \in I} E_i$, le produit des structures de module des $E_i$ (I, p. 43) est une structure de A-module. Muni de cette structure, l’ensemble E est appelé le module produit des modules $E_i$; si $x = (x_i), y = (y_i)$ sont deux éléments de E, on a donc

$$
\begin{cases}
x + y = (x_i + y_i) \\
\lambda x = (\lambda x_i)
\end{cases}
$$
pour tout $\lambda \in A$.

Les formules (17) expriment que les projections $pr_i : E \to E_i$ sont des applications linéaires; ces applications sont évidemment surjectives.

Rappelons que si l’ensemble d’indices I est vide, l’ensemble produit $\prod_{i \in I} E_i$ est alors réduit à un seul élément; la structure de module produit sur cet ensemble est alors celle pour laquelle cet unique élément est 0.

#### Proposition 4 {#alg-ii-s1-prop-4 .statement}

Soit $E = \prod_{i \in I} E_i$ le produit d’une famille de A-modules $(E_i)_{i \in I}$. Pour tout A-module F et toute famille d’applications linéaires $f_i : F \to E_i$, il existe une application f de F dans E et une seule, telle que $pr_i \circ f = f_i$ pour tout $i \in I$ et cette application est linéaire.

Cela résulte directement des définitions.

Le produit de modules est « associatif »: si $(J_\lambda)_{\lambda \in L}$ est une partition de I, l’application canonique

$$
\prod_{i \in I} E_i \to \prod_{\lambda \in L} \left( \prod_{i \in J_\lambda} E_i \right)
$$

est un isomorphisme.

#### Proposition 5 {#alg-ii-s1-prop-5 .statement}

(i) Soient $(E_i)_{i \in I}, (F_i)_{i \in I}$ deux familles de A-modules ayant même ensemble d’indices I; pour toute famille d’applications linéaires $f_i : E_i \to F_i$ ($i \in I$), l’application $f : (x_i) \mapsto (f_i(x_i))$ de $\prod_i E_i$ dans $\prod_i F_i$ (parfois notée $\prod_i f_i$) est linéaire.

(ii) Soit $(G_i)_{i \in I}$ une troisième famille de A-modules ayant I pour ensemble d’indices, et pour tout $i \in I$, soit $g_i : F_i \to G_i$ une application linéaire; posons $g = \prod_i g_i$. Pour que chacune des suites $E_i \xrightarrow{f_i} F_i \xrightarrow{g_i} G_i$ soit exacte, il faut et il suffit que la suite

$$
\prod_i E_i \xrightarrow{f} \prod_i F_i \xrightarrow{g} \prod_i G_i
$$

soit exacte.

L’assertion de (i) résulte aussitôt des définitions. D’autre part, dire que $y = (y_i)$ appartient à $\mathrm{Ker}(g)$ signifie que $g_i(y_i) = 0$ pour tout $i \in I$, donc que $y_i \in \mathrm{Ker}(g_i)$ pour tout $i \in I$; de même, dire que $y$ appartient à $\mathrm{Im}(f)$ signifie qu’il existe $x = (x_i) \in \prod_i E_i$ tel que $y = f(x)$, ce qui équivaut à dire que $y_i = f_i(x_i)$ pour tout $i \in I$, ou encore que $y_i \in \mathrm{Im}(f_i)$ pour tout $i \in I$; d’où (ii).

#### Corollaire {#alg-ii-s1-n5-cor-1 .statement}

Sous les conditions de la prop. 5, (i), on a

(18)
$$
\mathrm{Ker}(f) = \prod_{i \in I} \mathrm{Ker}(f_i), \quad \mathrm{Im}(f) = \prod_{i \in I} \mathrm{Im}(f_i)
$$
et on a des isomorphismes canoniques
$$
\mathrm{Coim}(f) \to \prod_{i \in I} \mathrm{Coim}(f_i), \quad \mathrm{Coker}(f) \to \prod_{i \in I} \mathrm{Coker}(f_i)
$$
obtenus en faisant respectivement correspondre à la classe d’un élément $x = (x_i)$ de $\prod_i E_i$, mod. $\mathrm{Ker}(f)$, (resp. à la classe d’un élément $y = (y_i)$ de $\prod_i F_i$, mod. $\mathrm{Im}(f)$), la famille des classes des $x_i$ mod. $\mathrm{Ker}(f_i)$ (resp. la famille des classes des $y_i$ mod. $\mathrm{Im}(f_i)$).

En particulier, pour que $f$ soit injective (resp. surjective, bijective, nulle), il faut et il suffit que, pour tout $i \in I$, $f_i$ soit injective (resp. surjective, bijective, nulle).

Si, pour tout $i \in I$, on considère un sous-module $F_i$ de $E_i$, le module $\prod_{i \in I} F_i$ est un sous-module de $\prod_{i \in I} E_i$, et en vertu du cor. de la prop. 5, on a un isomorphisme canonique

(19)
$$
\prod_{i \in I} (E_i/F_i) \to (\prod_{i \in I} E_i)/(\prod_{i \in I} F_i).
$$

Un exemple important de produit de modules est celui où tous les modules facteurs sont identiques à un même module $F$; leur produit $F^I$ n’est autre alors que l’ensemble des applications de $I$ dans $F$. L’application diagonale $F \to F^I$ faisant correspondre à tout $x \in F$ la fonction constante égale à $x$ dans $I$ est linéaire. Si $(E_i)_{i \in I}$ est une famille de $A$-modules, et pour tout $i \in I$, $f_i : F \to E_i$ est une application linéaire, alors l’application linéaire $x \mapsto (f_i(x))$ de $F$ dans $\prod_{i \in I} E_i$ est composée de l’application $(x_i) \mapsto (f_i(x_i))$ de $F^I$ dans $\prod_{i \in I} E_i$, et de l’application diagonale $F \to F^I$.

### 6. Somme directe de modules

Soient $(E_i)_{i \in I}$ une famille de $A$-modules, $F = \prod_{i \in I} E_i$ leur produit. L’ensemble $E$ des $x \in F$ tels que $\mathrm{pr}_i x = 0$ sauf pour un nombre *fini* d’indices est évidemment un *sous-module* de $F$, qu’on appelle la *somme directe externe* (ou simplement *somme directe*) de la famille de modules $(E_i)$ et que l’on note $\bigoplus_{i \in I} E_i$ (I, p. 46). Lorsque $I$ est *fini*, on a donc $\bigoplus_{i \in I} E_i = \prod_{i \in I} E_i$; si $I = \{p, q\}$ (intervalle de $\mathbf{Z}$), on écrit aussi $\bigoplus_{i \in I} E_i = E_p \oplus E_{p+1} \oplus \cdots \oplus E_q$.

Pour tout $\kappa \in I$, soit $j_\kappa$ l’application $E_\kappa \to F$ qui, à tout $x_\kappa \in E_\kappa$, fait correspondre l’élément de $F$ tel que $\mathrm{pr}_i(j_\kappa(x_\kappa)) = 0$ pour $i \neq \kappa$ et $\mathrm{pr}_\kappa(j_\kappa(x_\kappa)) = x_\kappa$; il est immédiat que $j_\kappa$ est une application linéaire injective de $E_\kappa$ dans la *somme directe* $E$ des $E_i$, que nous appellerons l’*injection canonique*; le sous-module $j_\kappa(E_\kappa)$ de $E$, isomorphe à $E_\kappa$, est appelé le sous-module *composant* d’indice $\kappa$ de $E$. On l’identifie souvent à $E_\kappa$ au moyen de $j_\kappa$.

Pour tout $x \in E = \bigoplus_{i \in I} E_i$, on a donc
$$
x = \sum_{i \in I} j_i(\mathrm{pr}_i x).
$$
(20)

#### Proposition 6 {#alg-ii-s1-prop-6 .statement}

*Soient* $(E_i)_{i \in I}$ *une famille de* $A$*-modules*, $M$ *un* $A$*-module*, et *pour tout* $i \in I$, *soit* $f_i : E_i \to M$ *une application linéaire*. *Il existe alors une application linéaire* $g : \bigoplus_{i \in I} E_i \to M$ *et une seule telle que*, *pour tout* $i \in I$, *on ait*:
$$
g \circ j_i = f_i.
$$
(21)

En vertu de (20), si $g$ existe, on a nécessairement, pour tout $x \in \bigoplus_{i \in I} E_i$, $g(x) = \sum_i g(j_i(\mathrm{pr}_i(x))) = \sum_i f_i(\mathrm{pr}_i(x))$, d’où l’unicité de $g$. Inversement, en posant $g(x) = \sum_i f_i(\mathrm{pr}_i(x))$ pour tout $x \in \bigoplus_{i \in I} E_i$, on vérifie aussitôt qu’on définit une application linéaire satisfaisant aux conditions de l’énoncé.

Lorsque aucune confusion n’en résulte, on pose $g = \sum_{i \in I} f_i$ (ce qui est contraire aux conventions de I, p. 14, lorsque la famille $(f_i)$ n’est pas à support fini).

En particulier, si $J$ est une partie quelconque de $I$, les injections canoniques $j_i$ pour $i \in J$ définissent une application linéaire canonique $j_J : \bigoplus_{i \in J} E_i \to \bigoplus_{i \in I} E_i$ qui à tout $(x_i)_{i \in J}$ fait correspondre l’élément $(x'_i)_{i \in I}$ tel que $x'_i = x_i$ pour $i \in J$, $x'_i = 0$ pour $i \notin J$; cette application est évidemment injective. En outre, si $(J_\lambda)_{\lambda \in L}$ est une partition de $I$, l’application $i : \bigoplus_{\lambda \in L} (\bigoplus_{i \in J_\lambda} E_i) \to \bigoplus_{i \in I} E_i$ correspondant à la famille $(j_{J_\lambda})$ par la prop. 6 est un *isomorphisme*, dit canonique (*« associativité »* de la somme directe).

#### Corollaire 1 {#alg-ii-s1-prop-6-cor-1 .statement}

Soient $(E_i)_{i \in I}, (F_\lambda)_{\lambda \in L}$ deux familles de $A$-modules. L’application
$$
\text{Hom}_A\left(\bigoplus_{i \in I} E_i, \prod_{\lambda \in L} F_\lambda\right) \to \prod_{(i, \lambda) \in I \times L} \text{Hom}_A(E_i, F_\lambda)
$$
qui, à tout $g \in \text{Hom}_A\left(\bigoplus_{i \in L} E_i, \prod_{\lambda \in L} F_\lambda\right)$, fait correspondre la famille $(\operatorname{pr}_\lambda \circ g \circ j_i)$, est un isomorphisme (dit canonique) de $\mathbf{Z}$-modules.
Cela résulte de la prop. 6 et de II, p. 10, prop. 4.

#### Corollaire 2 {#alg-ii-s1-prop-6-cor-2 .statement}

Soient $(E_i)_{i \in I}$ une famille de $A$-modules, $F$ un $A$-module, et pour chaque $i \in I$, soit $f_i : E_i \to F$ une application linéaire. Pour que $f = \sum_{i \in I} f_i$ soit un isomorphisme de $E = \bigoplus_{i \in I} E_i$ sur $F$, il faut et il suffit qu’il existe pour chaque $i \in I$ une application linéaire $g_i : F \to E_i$ vérifiant les propriétés suivantes:
$1^\circ$ $g_i \circ f_i = 1_{E_i}$ pour tout $i \in I$.
$2^\circ$ $g_i \circ f_\kappa = 0$ pour $i \neq \kappa$.
$3^\circ$ Pour tout $y \in F$, la famille $(g_i(y))$ a un support fini et l’on a
$$
y = \sum_{i \in I} f_i(g_i(y)).
$$
On notera que si $I$ est fini, la dernière condition s’écrit aussi
$$
\sum_{i \in I} f_i \circ g_i = 1_F.
$$
Il est évident que les conditions sont nécessaires, car elles sont vérifiées par les $g_i = \operatorname{pr}_i \circ f_i^{-1}$. Inversement, si elles sont vérifiées, pour tout $y \in F$, $g(y) = \sum_i j_i(g_i(y))$ est défini, et il est immédiat que $g$ est une application linéaire de $F$ dans $E$. Pour tout $y \in F$, on a $f(g(y)) = \sum_i f_i(g_i(y)) = y$ par hypothèse. D’autre part, pour tout $x \in E$, on a $g_\kappa(f(x)) = g_\kappa\left(\sum_i f_i(\operatorname{pr}_i(x))\right) = g_\kappa(f_\kappa(\operatorname{pr}_\kappa(x))) = \operatorname{pr}_\kappa(x)$ par hypothèse; par suite $g(f(x)) = \sum_i j_i(g_i(f(x))) = \sum_i j_i(\operatorname{pr}_i(x)) = x$, ce qui démontre le corollaire.

#### Proposition 7 {#alg-ii-s1-prop-7 .statement}

(i) Soient $(E_i)_{i \in I}, (F_i)_{i \in I}$ deux familles de $A$-modules ayant même ensemble d’indices $I$; pour toute famille d’applications linéaires $f_i : E_i \to F_i$ ($i \in I$), la restriction à $\bigoplus_{i \in I} E_i$ de l’application linéaire $(x_i) \mapsto (f_i(x_i))$ est une application linéaire $f : \bigoplus_{i \in I} E_i \to \bigoplus_{i \in I} F_i$ que l’on note $\bigoplus_{i \in I} f_i$ ou $\bigoplus_i f_i$ (ou $f = f_p \oplus f_{p+1} \oplus \cdots \oplus f_q$ si $I = [p, q]$ est un intervalle de $\mathbf{Z}$).
(ii) Soit $(G_i)_{i \in I}$ une troisième famille de $A$-modules ayant $I$ pour ensemble d’indices, et pour tout $i \in I$, soit $g_i : F_i \to G_i$ une application linéaire; posons $g = \bigoplus_i g_i$. Pour que chacune des suites $E_i \xrightarrow{f_i} F_i \xrightarrow{g_i} G_i$ soit exacte, il faut et il suffit que la suite
$$
\bigoplus_i E_i \xrightarrow{f} \bigoplus_i F_i \xrightarrow{g} \bigoplus_i G_i
$$
soit exacte.

Il est évident que, pour tout $(x_i) \in \bigoplus_i E_i$, la famille $(f_i(x_i))$ a un support fini, d’où (i). D’autre part, dire qu’un élément $y = (y_i)$ de $\bigoplus_i F_i$ appartient à $\mathrm{Ker}(g)$ signifie que $y_i \in \mathrm{Ker}(g_i)$ pour tout $i \in I$ (II, p. 10, prop. 5); de même, si $y_i \in \mathrm{Im}(f_i)$ pour tout $i \in I$, il existe, pour chaque $i \in I$ un $x_i \in E_i$ tel que $y_i = f_i(x_i)$, et lorsque $y_i = 0$ on peut supposer $x_i = 0$; on a donc bien $y \in \mathrm{Im}(f)$, et la réciproque est évidente.

#### Corollaire 1 {#alg-ii-s1-prop-7-cor-1 .statement}

Sous les conditions de la prop. 7, (i), on a
$$
\mathrm{Ker}(f) = \bigoplus_{i \in I} \mathrm{Ker}(f_i), \qquad \mathrm{Im}(f) = \bigoplus_{i \in I} \mathrm{Im}(f_i)
$$
et on a des isomorphismes canoniques
$$
\mathrm{Coïm}(f) \to \bigoplus_{i \in I} \mathrm{Coïm}(f_i), \qquad \mathrm{Coker}(f) \to \bigoplus_{i \in I} \mathrm{Coker}(f_i)
$$
définis comme dans II, p. 11, corollaire. En particulier, pour que $f$ soit injective (resp. surjective, bijective, nulle), il faut et il suffit que chacune des $f_i$ soit injective (resp. surjective, bijective, nulle).

Si, pour tout $i \in I$, on considère un sous-module $F_i$ de $E_i$, le module $\bigoplus_{i \in I} F_i$ est un sous-module de $\bigoplus_{i \in I} E_i$, et en vertu du cor. 1 de la prop. 7, on a un isomorphisme canonique
$$
\bigoplus_{i \in I} (E_i/F_i) \to (\bigoplus_{i \in I} E_i)/(\bigoplus_{i \in I} F_i).
$$

#### Corollaire 2 {#alg-ii-s1-prop-7-cor-2 .statement}

Soient $(E_i)_{i \in I}$, $(E'_i)_{i \in I}$, $(F_\lambda)_{\lambda \in L}$, $(F'_\lambda)_{\lambda \in L}$ quatre familles de A-modules, et pour chaque $i \in I$ (resp. chaque $\lambda \in L$) soit $u_i : E'_i \to E_i$ (resp. $v_\lambda : F_\lambda \to F'_\lambda$) une application linéaire. Alors le diagramme
$$
\begin{array}{ccc}
\mathrm{Hom}(\bigoplus_{i \in I} E'_i, \prod_{\lambda \in L} F'_\lambda) & \xrightarrow{\varphi'} & \prod_{(i, \lambda) \in I \times L} \mathrm{Hom}(E'_i, F'_\lambda) \\
\uparrow \mathrm{Hom}(\bigoplus_{i} u_i, \prod_{\lambda} v_\lambda) & & \uparrow \prod \mathrm{Hom}(u_i, v_\lambda) \\
\mathrm{Hom}(\bigoplus_{i \in I} E_i, \prod_{\lambda \in L} F_\lambda) & \xrightarrow{\varphi} & \prod_{(i, \lambda) \in I \times L} \mathrm{Hom}(E_i, F_\lambda)
\end{array}
$$
(où $\varphi$ et $\varphi'$ sont les isomorphismes canoniques définis dans II, p. 13, corollaire 1) est commutatif.

La vérification découle immédiatement des définitions.

Lorsque tous les $E_i$ sont identiques à un même A-module $E$, la somme directe $\bigoplus_{i \in I} E_i$ se note aussi $E^{(I)}$: ses éléments sont les applications de $I$ dans $E$, de support fini. Si, pour tout $i$, on prend pour $f_i$ l’application identique $E \to E$, on obtient par la prop. 6 de II, p. 12, une application linéaire canonique $E^{(I)} \to E$, dite application *codiagonale*, et qui à toute famille $(x_i)_{i \in I}$ d’éléments de $E$, de support fini, fait correspondre sa *somme* $\sum_{i \in I} x_i$.

#### Remarque {#alg-ii-s1-n6-rem-1 .statement}

Rappelons que la définition de la somme directe s’étend aussitôt à une famille $(E_i)_{i \in I}$ de *groupes* non nécessairement commutatifs, la notation multiplicative remplaçant bien entendu la notation additive; on dit alors « *somme restreinte* » au lieu de « *somme directe* » (I, p. 45). On notera que $E$ est sous-groupe *distingué* du produit $F = \prod_{i \in I} E_i$, et chacun des $j_k(E_k)$ est un sous-groupe *distingué* de $F$; en outre, pour deux indices distincts $\lambda, \mu$, tout élément de $j_\lambda(E_\lambda)$ est *permutable* à tout élément de $j_\mu(E_\mu)$. La prop. 6 (II p. 12) s’étend au cas général moyennant l’hypothèse que pour deux indices distincts $\lambda, \mu$, tout élément de $f_\lambda(E_\lambda)$ soit *permutable* dans $M$ à tout élément de $f_\mu(E_\mu)$ (I, p. 45, prop. 12). On en déduit aussitôt la propriété d’« associativité » de la somme restreinte. La prop. 7 et ses corollaires 1 et 2 (II, p. 13–14) subsistent sans modification.

### 7. Intersection et somme de sous-modules

Pour toute famille $(M_i)_{i \in I}$ de sous-modules d’un A-module $E$, l’intersection $\bigcap_{i \in I} M_i$ est un sous-module de $E$. Si, pour chaque $i \in I$, on désigne par $\varphi_i$ l’homomorphisme canonique $E \to E/M_i$, $\bigcap_{i \in I} M_i$ est le *noyau* de l’homomorphisme $\varphi : x \mapsto (\varphi_i(x))$ de $E$ dans $\prod_{i \in I} (E/M_i)$, autrement dit, on a une *suite exacte*

$$
0 \longrightarrow \bigcap_{i \in I} M_i \longrightarrow E \overset{\varphi}{\longrightarrow} \prod_{i \in I} (E/M_i).
$$

L’application linéaire $\varphi$ et l’application
$$
E/(\bigcap_{i \in I} M_i) \to \prod_{i \in I} (E/M_i)
$$
qu’on en déduit par passage au quotient, sont dites *canoniques*.

En particulier:
**Proposition 8.** — *Si une famille* $(M_i)_{i \in I}$ *de sous-modules de* $E$ *a une intersection réduite à* $0$, *E est canoniquement isomorphe à un sous-module de* $\prod_{i \in I} (E/M_i)$.

Étant donnée une partie $X$ d’un A-module $E$, l’intersection $F$ des sous-modules de $E$ contenant $X$ est appelée le sous-module *engendré* par $X$ et on dit que $X$ est un *ensemble générateur* (ou un *système générateur*) de $F$ (I, p. 32); pour une famille $(a_i)_{i \in I}$ d’éléments de $E$, on appelle sous-module engendré par la famille $(a_i)$ le sous-module engendré par l’ensemble des $a_i$.

On dit qu’un A-module est *de type fini* s’il possède un ensemble générateur *fini*.

#### Proposition 9 {#alg-ii-s1-prop-9 .statement}

*Le sous-module engendré par une famille* $(a_i)_{i \in I}$ *d’éléments d’un A-module E est l’ensemble des combinaisons linéaires de la famille* $(a_i)$.

En effet, tout sous-module de E qui contient tous les $a_i$ contient aussi les combinaisons linéaires des $a_i$. Inversement, les formules (1) et (2) de II, p. 3 prouvent que l’ensemble des combinaisons linéaires des $a_i$ est un sous-module de E qui contient évidemment tous les $a_i$, et est donc le plus petit sous-module les contenant.

#### Corollaire 1 {#alg-ii-s1-prop-9-cor-1 .statement}

*Soient* $u : E \to F$ *une application linéaire, S une partie de E, M le sous-module de E engendré par S. Alors* $u(M)$ *est le sous-module de F engendré par* $u(S)$.

En particulier, l’image par $u$ de tout sous-module de type fini de E est un sous-module de type fini de F.

#### Remarque {#alg-ii-s1-n7-rem-1 .statement}

Si l’on a $u(x) = 0$ pour tout $x \in S$, on a aussi $u(x) = 0$ pour tout $x \in M$. Nous nous référerons parfois à ce résultat sous le nom de « principe de prolongement des identités linéaires » ou « principe de prolongement par linéarité ».

En particulier, pour vérifier qu’une application linéaire $u : E \to F$ est de la forme $v \circ \varphi$, où $v : E/M \to F$ est linéaire et $\varphi : E \to E/M$ est l’application canonique, il suffit de vérifier que $u(S) = 0$.

#### Corollaire 2 {#alg-ii-s1-prop-9-cor-2 .statement}

*Le sous-module engendré par la réunion d’une famille* $(M_i)_{i \in I}$ *de sous-modules d’un module E, est identique à l’ensemble des sommes* $\sum_{i \in I} x_i$, *où* $(x_i)_{i \in I}$ *parcourt l’ensemble des familles d’éléments de E, de support fini et telles que* $x_i \in M_i$ *pour tout* $i \in I$.

En effet, il est clair que toute combinaison linéaire d’éléments de $\bigcup_{i \in I} M_i$ a la forme ci-dessus, la réciproque étant évidente.

On dit que le sous-module de E engendré par la réunion d’une famille $(M_i)_{i \in I}$ de sous-modules de E est la *somme* de la famille $(M_i)$ et on le note $\sum_{i \in I} M_i$. Si pour tout $i \in I$, $h_i$ est l’injection canonique $M_i \to E$, et $h : (x_i) \mapsto \sum_i h_i(x_i)$ l’application linéaire de $\bigoplus_{i \in I} M_i$ dans E correspondant à la famille $(h_i)$ (II, p. 12, prop. 6), $\sum_{i \in I} M_i$ est l’*image* de $h$; autrement dit, on a une *suite exacte*

$$
\bigoplus_{i \in I} M_i \xrightarrow{h} E \longrightarrow E / (\sum_{i \in I} M_i) \longrightarrow 0.
$$

(28)

#### Corollaire 3 {#alg-ii-s1-prop-9-cor-3 .statement}

*Si* $(M_\lambda)_{\lambda \in L}$ *est une famille filtrante croissante de sous-modules d’un A-module E, la somme* $\sum_{\lambda \in L} M_\lambda$ *est identique à la réunion* $\bigcup_{\lambda \in L} M_\lambda$.

En effet, on a toujours $\bigcup_{\lambda \in L} M_\lambda \subset \sum_{\lambda \in L} M_\lambda$ sans hypothèse; en outre, pour toute sous-famille finie $(M_\lambda)_{\lambda \in J}$ de $(M_\lambda)_{\lambda \in L}$, il existe par hypothèse un $\mu \in L$ tel que $M_\lambda \subset M_\mu$ pour tout $\lambda \in J$, donc $\sum_{\lambda \in J} M_\lambda \subset M_\mu$, et il résulte donc du cor. 2 que $\sum_{\lambda \in L} M_\lambda \subset \bigcup_{\lambda \in L} M_\lambda$.

#### Corollaire 4 {#alg-ii-s1-prop-9-cor-4 .statement}

Soient $0 \longrightarrow E \longrightarrow F \xrightarrow{g} G \longrightarrow 0$ une suite exacte de A-modules, S un système générateur de E, T un système générateur de G. Si T' est une partie de F telle que $g(T') = T, T' \cup f(S)$ est un système générateur de F.

En effet, le sous-module F' de F engendré par T' $\cup f(S)$ contient $f(E)$, et comme $g(F')$ contient T, on a $g(F') = G$; d'où $F' = F$.

#### Corollaire 5 {#alg-ii-s1-prop-9-cor-5 .statement}

Dans une suite exacte $0 \to E \to F \to G \to 0$ de A-modules, si E et G sont de type fini, il en est de même de F.

#### Proposition 10 {#alg-ii-s1-prop-10 .statement}

Soient M, N deux sous-modules d'un A-module E. On a alors deux suites exactes

$$
(29) \quad 0 \longrightarrow M \cap N \xrightarrow{u} M \oplus N \xrightarrow{i-j} M + N \longrightarrow 0
$$
$$
(30) \quad 0 \longrightarrow E/(M \cap N) \xrightarrow{v} (E/M) \oplus (E/N) \xrightarrow{p-q} E/(M + N) \longrightarrow 0
$$

où $i : M \to M + N, j : N \to M + N$ sont les injections canoniques,

$$
p : E/M \to E/(M + N) \text{ et } q : E/N \to E/(M + N)
$$

les surjections canoniques, et où les homomorphismes u et v sont définis comme suit: si $f : M \cap N \to M \to M \oplus N$ et $g : M \cap N \to N \to M \oplus N$ sont les injections canoniques, $u = f + g$, et si $r : E/(M \cap N) \to E/M \to (E/M) \oplus (E/N)$ et
$$
s : E/(M \cap N) \to E/N \to (E/M) \oplus (E/N)
$$
sont les applications canoniques, $v = r + s$.

Prouvons l'exactitude de (29): il est évident que $i - j$ est surjective et que u est injective. En outre, dire que $(i - j)(x, y) = 0$, où $x \in M$ et $y \in N$, signifie que $i(x) - j(y) = 0$, donc $i(x) = j(y) = z \in M \cap N$, d'où par définition $x = f(z)$, $y = g(z)$, ce qui prouve que $\operatorname{Ker}(i - j) = \operatorname{Im} u$.

Prouvons l'exactitude de (30): il est clair que $p - q$ est surjective. D'autre part, dire que $v(t) = 0$ pour $t \in E/(M \cap N)$ signifie que $r(t) = s(t) = 0$, donc que t est la classe mod. (M $\cap$ N) d'un élément $z \in E$ dont les classes mod. M et mod. N sont nulles, ce qui entraîne $z \in M \cap N$ et $t = 0$. Enfin, dire que $(p - q)(x, y) = 0$ où $x \in E/M, y \in E/N$ signifie que $p(x) = q(y)$, ou encore qu'il existe deux éléments $z', z''$ de E dont les classes mod. M et mod. N respectivement sont x et y et qui sont tels que $z' - z'' \in M + N$. Il existe donc $t' \in M, t'' \in N$ tels que $z' - z'' = t' - t''$, d'où $z' - t' = z'' - t'' = z$. Soit w la classe mod. (M $\cap$ N) de z; $r(w)$ est la classe mod. M de z, donc aussi celle de $z'$, c'est-à-dire x; de même $s(w) = y$, ce qui achève de prouver que $\operatorname{Ker}(p - q) = \operatorname{Im} v$.

### 8. Sommes directes de sous-modules

#### Définition 6 {#alg-ii-s1-def-6 .statement}

On dit qu'un A-module E est somme directe d'une famille $(M_i)_{i \in I}$ de sous-modules de E si l'application canonique $\bigoplus_{i \in I} M_i \to E$ (II, p. 12) est un isomorphisme.

Il revient au même de dire que tout $x \in E$ peut s'écrire d'une seule manière sous la forme $x = \sum_{\iota \in I} x_\iota$, où $x_\iota \in E_\iota$ pour tout $\iota \in I$; l’élément $x_\iota$ correspondant ainsi à $x$ est appelé le *composant* de $x$ dans $E_\iota$; l’application $x \mapsto x_\iota$ est *linéaire*.

#### Remarque 1 {#alg-ii-s1-n8-rem-1 .statement}

Soient $(M_\iota)_{\iota \in I}$, $(N_\iota)_{\iota \in I}$ deux familles de sous-modules d’un module $E$, ayant même ensemble d’indices; supposons que $E$ soit *à la fois* somme directe de la famille $(M_\iota)$ et de la famille $(N_\iota)$, *et que l’on ait* $N_\iota \subset M_\iota$ pour tout $\iota \in I$. Alors *on a* $N_\iota = M_\iota$ *pour tout* $\iota \in I$, comme il résulte aussitôt du cor. 1 de II, p. 14 appliqué aux injections canoniques $f_\iota : N_\iota \to M_\iota$.

#### Proposition 11 {#alg-ii-s1-prop-11 .statement}

*Soit* $(M_\iota)_{\iota \in I}$ *une famille de sous-modules d’un A-module* $E$. *Les propriétés suivantes sont équivalentes*:

a) *Le sous-module* $\sum_{\iota \in I} M_\iota$ *est somme directe de la famille* $(M_\iota)_{\iota \in I}$.

b) *La relation* $\sum_{\iota \in I} x_\iota = 0$, *où* $x_\iota \in M_\iota$ *pour tout* $\iota \in I$, *entraîne* $x_\iota = 0$ *pour tout* $\iota \in I$.

c) *Pour tout* $\kappa \in I$, *l’intersection de* $M_\kappa$ *et de* $\sum_{\iota \neq \kappa} M_\iota$ *est réduite à* 0.

Il est immédiat que a) et b) sont équivalentes, puisque la relation $\sum_\iota x_\iota = \sum_\iota y_\iota$ est équivalente à $\sum_\iota (x_\iota - y_\iota) = 0$. D’autre part, en vertu de la déf. 6, a) entraîne c) puisque l’expression d’un élément de $\bigoplus_{\iota \in I} M_\iota$ comme somme d’éléments $x_\iota \in M_\iota$ est unique. Enfin, la relation $\sum_\iota x_\iota = 0$, où $x_\iota \in M_\iota$ pour tout $\iota$, s’écrit, pour tout $\kappa \in I$, $x_\kappa = \sum_{\iota \neq \kappa} (-x_\iota)$; la condition c) entraîne alors $x_\kappa = 0$ pour tout $\kappa \in I$, donc c) entraîne b).

#### Définition 7 {#alg-ii-s1-def-7 .statement}

*On dit qu’un endomorphisme* $e$ *d’un A-module* $E$ *est un projecteur si* $e \circ e = e$ *(autrement dit, si* $e$ *est un idempotent dans l’anneau* $\mathrm{End}(E)$*).* *Dans* $\mathrm{End}(E)$, *on dit qu’une famille* $(e_\lambda)_{\lambda \in L}$ *de projecteurs est orthogonale si l’on a* $e_\lambda \circ e_\mu = 0$ *pour* $\lambda \neq \mu$.

#### Proposition 12 {#alg-ii-s1-prop-12 .statement}

*Soit* $E$ *un A-module*.

(i) *Si* $E$ *est somme directe d’une famille* $(M_\lambda)_{\lambda \in L}$ *de sous-modules et si, pour tout* $x \in E$, $e_\lambda(x)$ *est le composant de* $x$ *dans* $M_\lambda$, $(e_\lambda)$ *est une famille orthogonale de projecteurs telle que* $x = \sum_{\lambda \in L} e_\lambda(x)$ *pour tout* $x \in E$.

(ii) *Inversement, si* $(e_\lambda)_{\lambda \in L}$ *est une famille orthogonale de projecteurs dans* $\mathrm{End}(E)$ *telle que* $x = \sum_{\lambda \in L} e_\lambda(x)$ *pour tout* $x \in E$, $E$ *est somme directe de la famille des sous-modules* $M_\lambda = e_\lambda(E)$.

La propriété (i) découle des définitions, et (ii) est un cas particulier du cor. 2 de II, p. 13, appliqué aux injections canoniques $M_\lambda \to E$ et aux applications $e_\lambda : E \to M_\lambda$.

On notera que lorsque L est fini, la condition $x = \sum_{\lambda \in L} e_\lambda(x)$ pour tout $x \in E$ s’écrit aussi dans End (E)

(31)
$$
1_E = \sum_{\lambda \in L} e_\lambda.
$$

#### Corollaire {#alg-ii-s1-n8-cor-1 .statement}

*Pour tout projecteur e de E, E est somme directe de l’image M = e(E) et du noyau N = \overline{e}^{-1}(0) de e; pour tout x = x_1 + x_2 \in E avec x_1 \in M et x_2 \in N, on a x_1 = e(x); 1 - e est un projecteur de E, d’image N et de noyau M.*

On a en effet $(1 - e)^2 = 1 - 2e + e^2 = 1 - e$ dans End(E), donc $1 - e$ est un projecteur; comme en outre $e(1 - e) = (1 - e)e = e - e^2 = 0$, E est somme directe des images M et N de e et $1 - e$ en vertu de la prop. 12. Enfin, pour tout $x \in E$, la relation $x \in M$ est équivalente à $x = e(x)$; en effet, $x = e(x)$ entraîne par définition $x \in M$, et inversement, si $x = e(x')$ avec $x' \in E$, on a $e(x) = e^2(x') = e(x') = x$; ceci montre donc que M est le noyau de $1 - e$; en échangeant les rôles de e et de $1 - e$, on voit de même que N est le noyau de e.

*Remarque 2).* — Soient E, F deux A-modules, tels que E soit somme directe d’une famille $(M_i)$ de sous-modules, et F somme directe d’une famille *finie* $(N_j)_{1 \leq j \leq n}$ de sous-modules. On sait alors (II, p. 13, cor. 1) que $\mathrm{Hom}_A(E, F)$ s’identifie canoniquement au produit $\prod_{i,j} \mathrm{Hom}_A(M_i, N_j)$; de façon précise, à une famille $(u_{ji})$, où $u_{ji} \in \mathrm{Hom}_A(M_i, N_j)$ correspond l’application linéaire $u : E \to F$ définie de la façon suivante. Il suffit de définir la restriction de $u$ à chacun des $M_i$, et pour $x_i \in M_i$, on a
$$
u(x_i) = \sum_{j=1}^n u_{ji}(x_i).
$$
Soit maintenant G un troisième A-module, somme directe d’une famille *finie* $(P_k)_{1 \leq k \leq p}$ de sous-modules; soit $v$ une application linéaire de F dans G et soit $(v_{kj}) \in \prod_{j, k} \mathrm{Hom}_A(N_j, P_k)$ la famille qui lui correspond canoniquement. Pour tout $x_i \in M_i$, on a
$$
v(u(x_i)) = \sum_{j=1}^n v(u_{ji}(x_i)) = \sum_{k=1}^p \sum_{j=1}^n v_{kj}(u_{ji}(x_i)).
$$
On voit donc que, si l’on pose
(32)
$$
w_{ki} = \sum_{j=1}^n v_{kj} \circ u_{ji} \in \mathrm{Hom}_A(M_i, P_k)
$$
la famille $(w_{ki})$ correspond canoniquement à l’application linéaire *composée* $w = v \circ u$ de E dans G (cf. II, p. 147).

### 9. Sous-modules supplémentaires

#### Définition 8 {#alg-ii-s1-def-8 .statement}

*Dans un A-module E, on dit que deux sous-modules $M_1, M_2$ sont supplémentaires si E est somme directe de $M_1$ et $M_2$.*

La prop. 11 de II, p. 18 montre que, pour que $M_1$ et $M_2$ soient supplémentaires, il faut et il suffit que $M_1 + M_2 = E$ et $M_1 \cap M_2 = \{0\}$ (cf. I, p. 46, prop. 15).

#### Proposition 13 {#alg-ii-s1-prop-13 .statement}

Soient $M_1, M_2$ deux sous-modules supplémentaires dans un A-module E. La restriction à $M_1$ de l’application canonique $E \to E/M_2$ est un isomorphisme de $M_1$ sur $E/M_2$.

En effet, cette application linéaire est surjective puisque $M_1 + M_2 = E$, et elle est injective puisque son noyau est l’intersection de $M_1$ et du noyau $M_2$ de $E \to E/M_2$, donc est réduit à 0.

#### Corollaire {#alg-ii-s1-n9-cor-1 .statement}

Si $M_2$ et $M'_2$ sont tous deux supplémentaires d’un même sous-module $M_1$ de E, l’ensemble des couples $(x, x') \in M_2 \times M'_2$ tels que $x - x' \in M_1$ est le graphe d’un isomorphisme de $M_2$ sur $M'_2$.

Il est immédiat en effet que c’est le graphe de l’isomorphisme composé $M_2 \to E/M_1 \to M'_2$.

#### Définition 9 {#alg-ii-s1-def-9 .statement}

On dit qu’un sous-module M d’un A-module E est facteur direct de E s’il possède un sous-module supplémentaire dans E.

Lorsqu’il en est ainsi, $E/M$ est isomorphe à un supplémentaire de M (prop. 13).

Un sous-module n’admet pas nécessairement de supplémentaire (II, p. 180, exerc. 11). Lorsqu’un sous-module est facteur direct, il a en général plusieurs supplémentaires distincts ; ces supplémentaires sont toutefois deux à deux canoniquement isomorphes (cor. de la prop. 13).

#### Proposition 14 {#alg-ii-s1-prop-14 .statement}

Pour qu’un sous-module M d’un module E soit facteur direct, il faut et il suffit qu’il existe un projecteur de E dont l’image soit M, ou un projecteur de E dont le noyau soit M.

Cela résulte immédiatement de II, p. 18–19, prop. 12 et corollaire.

#### Proposition 15 {#alg-ii-s1-prop-15 .statement}

Étant donnée une suite exacte de A-modules

$$
0 \longrightarrow E \xrightarrow{f} F \xrightarrow{g} G \longrightarrow 0
$$

les conditions suivantes sont équivalentes:

a) Le sous-module $f(E)$ de F est facteur direct.

b) Il existe une rétraction linéaire $r : F \to E$ associée à $f$ (E, II, p. 18, déf. 11).

c) Il existe une section linéaire $s : G \to F$ associée à $g$ (E, II, p. 18, déf. 11).

Lorsqu’il en est ainsi, $f + s : E \oplus G \to F$ est un isomorphisme.

S’il existe un projecteur $e$ dans $\mathrm{End}(F)$ tel que $e(F) = f(E)$, l’homomorphisme $f^{-1} \circ e : F \to E$ est une rétraction linéaire associée à $f$; inversement, s’il existe une telle rétraction $r$, il est immédiat que $f \circ r$ est un projecteur dans F dont $f(E)$ est l’image, donc a) et b) sont équivalentes (prop. 14). Si $f(E)$ admet un supplémentaire $E'$ dans F et si $j : E' \to F$ est l’injection canonique, $g \circ j$ est un isomorphisme de $E'$ sur G et l’isomorphisme réciproque, considéré comme application de G dans F, est une section linéaire associée à $g$. Inversement, s’il existe une telle section $s$, $s \circ g$ est un projecteur dans F dont $f(E)$ est le noyau, donc a) et c) sont équivalentes (prop. 14). En outre s est une bijection de G sur s(G), et comme s(G) est supplémentaire de f(E), f + s est un isomorphisme.

On notera que la donnée de r (resp. s) équivaut à la donnée d’un supplémentaire de f(E) dans F, savoir le noyau de r (resp. l’image de s).

Lorsque la suite exacte (33) vérifie les conditions de la prop. 15, on dit qu’elle est scindée ou que (F, f, g) est une extension triviale de G par E (I, p. 63).

#### Corollaire 1 {#alg-ii-s1-prop-15-cor-1 .statement}

Soit u : E → F une application linéaire. Pour qu’il existe une application linéaire v : F → E telle que u ◦ v = 1_F (cas où on dit que u est inversible à droite et que v est inverse à droite de u), il faut et il suffit que u soit surjective et que son noyau soit facteur direct dans E. Le sous-module Im(v) de E est alors supplémentaire de Ker(u).

Il est évidemment nécessaire que u soit surjective; comme v est alors une section associée à u, la conclusion résulte de la prop. 15.

#### Corollaire 2 {#alg-ii-s1-prop-15-cor-2 .statement}

Soit u : E → F une application linéaire. Pour qu’il existe une application linéaire v : F → E telle que v ◦ u = 1_E (cas où on dit que u est inversible à gauche et que v est inverse à gauche de u), il faut et il suffit que u soit injective et que son image soit facteur direct dans F. Le sous-module Ker(v) de F est alors supplémentaire de Im(u).

Il est évidemment nécessaire que u soit injective; comme v est alors une rétraction associée à u, la conclusion résulte encore de la prop. 15.

#### Remarque 1 {#alg-ii-s1-n9-rem-1 .statement}

Soient M, N deux sous-modules supplémentaires dans un A-module E, p, q les projecteurs de E sur M et N respectivement, correspondant à la décomposition de E en somme directe de M et N. On sait (II, p. 13, cor. 1) que, pour tout A-module F, l’application (u, v) ↦ u ◦ p + v ◦ q est un isomorphisme de
$$
\operatorname{Hom}_A(M, F) \oplus \operatorname{Hom}_A(N, F)
$$
sur $\operatorname{Hom}_A(E, F)$. L’image de $\operatorname{Hom}_A(M, F)$ par cet isomorphisme est l’ensemble des applications linéaires $w : E \to F$ telles que $w(x) = 0$ pour tout $x \in N$.

#### Remarque 2 {#alg-ii-s1-n9-rem-2 .statement}

Si M, N sont deux sous-modules de E tels que $M \cap N$ soit facteur direct de M et de N, alors $M \cap N$ est aussi facteur direct de $M + N$: en effet, si P (resp. Q) est un supplémentaire de $M \cap N$ dans M (resp. N), $M + N$ est somme directe de $M \cap N$, P et Q, comme on le vérifie aussitôt.

### 10. Modules de longueur finie

Rappelons (I, p. 36, déf. 7) qu’un A-module M est dit simple s’il n’est pas réduit à 0 et s’il ne contient aucun sous-module distinct de M et de {0}. Un A-module M est dit de longueur finie s’il possède une suite de Jordan-Hölder $(M_i)_{0 \leq i \leq n}$, et le nombre n des quotients de cette suite (qui ne dépend pas de la suite de Jordan-Hölder de M considérée) est alors appelé la longueur de M (I, p. 42, déf. 11); nous le noterons $\operatorname{long}(M)$, ou $\operatorname{long}_A(M)$. Un A-module réduit à 0 est de longueur 0; si M est un A-module de longueur finie non réduit à 0, on a $\operatorname{long}(M) > 0$.

#### Proposition 16 {#alg-ii-s1-prop-16 .statement}

Soient M un A-module, N un sous-module de M; pour que M soit de longueur finie, il faut et il suffit que N et $M/N$ le soient, et l’on a

(34) $$ \operatorname{long}(N) + \operatorname{long}(M/N) = \operatorname{long}(M). $$

La démonstration a été donnée dans I, p. 42, prop. 10.

#### Corollaire 1 {#alg-ii-s1-prop-16-cor-1 .statement}

Soit $M$ un $A$-module de longueur finie; pour qu’un sous-module $N$ de $M$ soit égal à $M$, il faut et il suffit que $\operatorname{long}(N) = \operatorname{long}(M)$.

#### Corollaire 2 {#alg-ii-s1-prop-16-cor-2 .statement}

Soit $u : M \to N$ un homomorphisme de $A$-modules. Si $M$ ou $N$ est de longueur finie, il en est de même de $\operatorname{Im}(u)$. Si $M$ est de longueur finie, il en est de même de $\operatorname{Ker}(u)$ et l’on a

(35) $$ \operatorname{long}(\operatorname{Im}(u)) + \operatorname{long}(\operatorname{Ker}(u)) = \operatorname{long}(M). $$

Si $N$ est de longueur finie, il en est de même de $\operatorname{Coker}(u)$ et l’on a

(36) $$ \operatorname{long}(\operatorname{Im}(u)) + \operatorname{long}(\operatorname{Coker}(u)) = \operatorname{long}(N). $$

#### Corollaire 3 {#alg-ii-s1-prop-16-cor-3 .statement}

Soit $(M_i)_{0 \leq i \leq n}$ une famille finie de $A$-modules de longueur finie. S’il existe une suite exacte d’applications linéaires

(37) $$
\begin{array}{cccccccccccccc}
0 & \longrightarrow & M_0 & \xrightarrow{u_0} & M_1 & \xrightarrow{u_1} & M_2 & \longrightarrow & \cdots \longrightarrow & M_{n-1} & \xrightarrow{u_{n-1}} & M_n & \longrightarrow & 0
\end{array}
$$

on a la relation

(38) $$
\sum_{k=0}^{n} (-1)^k \operatorname{long}(M_k) = 0.
$$

Le corollaire est évident pour $n = 1$ et n’est autre que la prop. 16 pour $n = 2$; raisonnons par récurrence sur $n$. Si $M'_{n-1} = \operatorname{Im}(u_{n-2})$, on a, par l’hypothèse de récurrence,

$$
\sum_{k=0}^{n-2} (-1)^k \operatorname{long}(M_k) + (-1)^{n-1} \operatorname{long}(M'_{n-1}) = 0.
$$

D’autre part, la suite exacte $0 \to M'_{n-1} \to M_{n-1} \to M_n \to 0$ donne

$$
\operatorname{long}(M'_{n-1}) + \operatorname{long}(M_n) = \operatorname{long}(M_{n-1}),
$$

d’où la relation (38).

#### Corollaire 4 {#alg-ii-s1-prop-16-cor-4 .statement}

Soient $M$ et $N$ deux sous-modules de longueur finie d’un $A$-module $E$; alors $M + N$ est de longueur finie et l’on a

(39) $$ \operatorname{long}(M + N) + \operatorname{long}(M \cap N) = \operatorname{long}(M) + \operatorname{long}(N). $$

Il suffit d’appliquer le cor. 3 à la suite exacte (29) (II, p. 17)

$$
0 \to M \cap N \to M \oplus N \to M + N \to 0
$$

en tenant compte de ce que $\operatorname{long}(M \oplus N) = \operatorname{long}(M) + \operatorname{long}(N)$ d’après (34).

#### Corollaire 5 {#alg-ii-s1-prop-16-cor-5 .statement}

Soit $M$ un $A$-module somme d’une famille finie $(N_i)$ de sous-modules de longueur finie. Alors $M$ est de longueur finie et on a

$$
\text{long}(M) \leq \sum_i \text{long}(N_i).
$$

En outre, pour que les deux membres de (40) soient égaux, il faut et il suffit que $M$ soit somme directe des $N_i$.

En effet, on a vu (II, p. 16, formule (28)) que l’on a une application linéaire surjective canonique $h : \bigoplus_i N_i \to M$; le corollaire résulte donc de (35) (II, p. 22).

#### Corollaire 6 {#alg-ii-s1-prop-16-cor-6 .statement}

Soient $M$ et $N$ deux sous-modules d’un $A$-module $E$ tels que $E/M$ et $E/N$ soient des modules de longueur finie; alors $E/(M \cap N)$ est de longueur finie et l’on a

$$
\text{long}(E/(M \cap N)) + \text{long}(E/(M + N)) = \text{long}(E/M) + \text{long}(E/N).
$$

Il suffit d’appliquer le cor. 3 (II, p. 22) à la suite exacte (30) (II, p. 17)

$$
0 \to E/(M \cap N) \to (E/M) \oplus (E/N) \to E/(M + N) \to 0
$$

en tenant compte de ce que

$$
\text{long}((E/M) \oplus (E/N)) = \text{long}(E/M) + \text{long}(E/N).
$$

#### Corollaire 7 {#alg-ii-s1-prop-16-cor-7 .statement}

Soit $(M_i)$ une famille finie de sous-modules d’un $A$-module $E$, tels que les $E/M_i$ soient des modules de longueur finie. Alors $E/(\bigcap_i M_i)$ est de longueur finie, et l’on a

$$
\text{long}(E/(\bigcap_i M_i)) \leq \sum_i \text{long}(E/M_i).
$$

En effet, on a vu (II, p. 15, formule (27)) que l’on a une application linéaire injective canonique $E/(\bigcap_i M_i) \to \bigoplus_i (E/M_i)$.

#### Remarque {#alg-ii-s1-n10-rem-1 .statement}

A l’exception de II, p. 16, prop. 9, tous les résultats des n°s 2 à 10 sont valables pour les groupes commutatifs à opérateurs quelconques, les sous-modules (resp. les modules quotients) étant remplacés dans les énoncés par les sous-groupes stables (resp. par les groupes quotients par des sous-groupes stables); on convient d’appeler encore « applications linéaires » les homomorphismes de groupes à opérateurs. Les corollaires de II, p. 16, prop. 9 sont encore valables pour les groupes commutatifs à opérateurs: c’est évident pour les cor. 4 et 5, ainsi que pour le cor. 2, puisque $\alpha \left( \sum_{i \in I} x_i \right) = \sum_{i \in I} \alpha x_i$ pour tout opérateur $\alpha$, et le cor. 3 s’en déduit. Quant au cor. 1, il suffit de remarquer que si $N$ est un sous-groupe stable de $F$ contenant $u(S)$, $\bar{u}^1(N)$ est un sous-groupe stable de $E$ contenant $S$, donc $\bar{u}^1(N)$ contient $M$ et par suite $u(M) \subset N$.

### 11. Familles libres. Bases

Soient $A$ un anneau, $T$ un ensemble, et considérons le $A$-module $A_s^{(T)}$. Par définition, c’est la somme directe externe d’une famille $(M_t)_{t \in T}$ de $A$-modules tous égaux à $A_s$ et pour tout $t \in T$ on a une injection canonique $j_t : A_s \to A_s^{(T)}$ (II, p. 12). Posons $j_t(1) = e_t$, de sorte que $e_t = (\delta_{tt'})_{t' \in T}$, où $\delta_{tt'}$ est égal à 0 si $t' \neq t$, à 1 si $t' = t$ (« symbole de Kronecker »; $(t, t') \mapsto \delta_{tt'}$ n’est autre que la fonction caractéristique de la diagonale de $T \times T$); tout $x = (\xi_t)_{t \in T} \in A_s^{(T)}$ s’écrit donc d’une seule manière: $x = \sum_{t \in T} \xi_t e_t$. L’application $\varphi : t \mapsto e_t$ de $T$ dans $A_s^{(T)}$ est dite canonique; elle est injective si $A$ n’est pas réduit à 0. Nous allons voir que le couple $(A_s^{(T)}, \varphi)$ est solution d’un problème d’application universelle (E, IV, p. 22).

#### Proposition 17 {#alg-ii-s1-prop-17 .statement}

Pour tout $A$-module $E$ et toute application $f : T \to E$ il existe une application $A$-linéaire et une seule $g : A_s^{(T)} \to E$ telle que $f = g \circ \varphi$.

En effet, la condition $f = g \circ \varphi$ signifie que $g(e_t) = f(t)$ pour tout $t \in T$, ce qui équivaut à $g(\xi_t e_t) = \xi_t f(t)$ pour tout $\xi \in A$ et tout $t \in T$ et signifie encore que $g \circ j_t$ est l’application linéaire $\xi \mapsto \xi f(t)$ de $A_s$ dans $E$ pour tout $t \in T$; la proposition est donc cas particulier de II, p. 12, prop. 6.

On dit que l’application linéaire $g$ est déterminée par la famille $(f(t))_{t \in T}$ d’éléments de $E$; on a par définition

$$
g\left( \sum_{t \in T} \xi_t e_t \right) = \sum_{t \in T} \xi_t f(t).
$$

Le noyau $R$ de $g$ est l’ensemble des $(\xi_t) \in A_s^{(T)}$ tels que l’on ait $\sum_t \xi_t f(t) = 0$; on dit parfois que le module $R$ est le module des relations linéaires entre les éléments de la famille $(f(t))_{t \in T}$. On dit que la suite exacte

$$
0 \longrightarrow R \longrightarrow A_s^{(T)} \xrightarrow{g} E
$$

est déterminée par la famille $(f(t))_{t \in T}$.

#### Corollaire 1 {#alg-ii-s1-prop-17-cor-1 .statement}

Soient $T, T'$ deux ensembles, $g : T \to T'$ une application. Il existe alors une application $A$-linéaire $f : A^{(T)} \to A^{(T')}$ et une seule rendant commutatif le diagramme

$$
\begin{array}{ccc}
T & \xrightarrow{g} & T' \\
\downarrow \varphi & & \downarrow \varphi' \\
A^{(T)} & \xrightarrow{f} & A^{(T')}
\end{array}
$$

où $\varphi$ et $\varphi'$ sont les applications canoniques.

Il suffit d’appliquer la prop. 17 à l’application composée $T \xrightarrow{g} T' \xrightarrow{\varphi'} A^{(T')}$.

#### Corollaire 2 {#alg-ii-s1-prop-17-cor-2 .statement}

Pour qu’une famille $(a_t)_{t \in T}$ d’éléments d’un $A$-module $E$ soit un système générateur de E, il faut et il suffit que l’application linéaire $A_s^{(T)} \to E$ déterminée par cette famille soit surjective.

Ce n’est qu’une autre manière d’exprimer la prop. 9 de II, p. 16.

#### Définition 10 {#alg-ii-s1-def-10 .statement}

On dit qu’une famille $(a_t)_{t \in T}$ d’éléments d’un A-module E est une famille libre (resp. est une base de E) si l’application linéaire $A_s^{(T)} \to E$ déterminée par cette famille est injective (resp. bijective). On dit qu’un module est libre s’il possède une base.

En particulier, on dira qu’un groupe commutatif G est libre si G (noté additivement) est un $\mathbf{Z}$-module libre (cf. I, p. 87).

La déf. 10, jointe au cor. 2 de la prop. 17, montre qu’une base d’un A-module E est une famille libre génératrice de E. Toute famille libre d’éléments de E est donc une base du sous-module qu’elle engendre.

Par définition, le A-module $A_s^{(T)}$ est libre et la famille $(e_t)_{t \in T}$ est une base (dite canonique) de ce A-module. Lorsque $A \neq \{0\}$, on identifie souvent T à l’ensemble des $e_t$ par la bijection canonique $t \mapsto e_t$; cela revient à écrire $\sum_{t \in T} \xi_t \cdot t$ au lieu de $\sum_{t \in T} \xi_t e_t$ les éléments de $A_s^{(T)}$. Lorsqu’on adopte cette convention, les éléments de $A_s^{(T)}$ sont appelés combinaisons linéaires formelles (à coefficients dans A) des éléments de T.

La définition 10 et la prop. 17 donnent aussitôt le résultat suivant:

#### Corollaire 3 {#alg-ii-s1-def-10-cor-3 .statement}

Soient E un A-module libre, $(a_t)_{t \in T}$ une base de E, F un A-module, $(b_t)_{t \in T}$ une famille d’éléments de F. Il existe une application linéaire $f : E \to F$ et une seule telle que l’on ait

$$
f(a_t) = b_t \quad \text{pour tout } t \in T.
$$

Pour que f soit injective (resp. surjective), il faut et il suffit que $(b_t)$ soit une famille libre dans F (resp. un système générateur de F).

Lorsqu’une famille $(a_t)_{t \in T}$ n’est pas libre, on dit qu’elle est liée. La déf. 10 s’exprime encore comme suit: dire que la famille $(a_t)_{t \in T}$ est libre signifie que la relation $\sum_{t \in T} \lambda_t a_t = 0$ (où la famille $(\lambda_t)$ est à support fini) entraîne $\lambda_t = 0$ pour tout $t \in T$; dire que $(a_t)_{t \in T}$ est une base de E signifie que tout $x \in E$ s’écrit d’une manière et d’une seule sous la forme $x = \sum_{t \in T} \xi_t a_t$; pour tout $t \in T$, on dit alors que $\xi_t$ est la composante (ou la coordonnée) d’indice t de x par rapport à la base $(a_t)$; l’application $x \mapsto \xi_t$ de E dans $A_s$ est linéaire.

Supposons $A \neq \{0\}$; alors, dans un A-module E, deux éléments d’une famille libre $(a_t)_{t \in T}$ dont les indices sont distincts, sont eux-mêmes distincts: car si on avait $a_{t'} = a_{t''}$ pour $t' \neq t''$, on en déduirait $\sum_{t \in T} \lambda_t a_t = 0$ avec $\lambda_{t'} = 1, \lambda_{t''} = -1$ et $\lambda_t = 0$ pour les éléments de T distincts de $t'$ et de $t''$. On dira qu’une partie S de

E est une partie libre (resp. une base de E) si la famille définie par l’application identique de S sur elle-même est libre (resp. une base de E); toute famille définie par une application bijective d’un ensemble d’indices sur S est alors libre (resp. une base). Les éléments d’une partie libre de E sont encore dits linéairement indépendants.

Si une partie de E n’est pas libre, on dit qu’elle est liée, ou est un système lié, et que ses éléments sont linéairement dépendants.

Toute partie d’une partie libre de E est libre; en particulier la partie vide est libre et est une base du sous-module {0} de E.

#### Proposition 18 {#alg-ii-s1-prop-18 .statement}

Pour qu’une famille $(a_t)_{t \in T}$ d’éléments d’un module E soit libre, il faut et il suffit que toute sous-famille finie de $(a_t)_{t \in T}$ soit libre.

Cela résulte aussitôt de la définition.

La prop. 18 montre que l’ensemble des parties libres de E, ordonné par inclusion, est inductif (E, III, p. 20); comme il n’est pas vide (puisque $\varnothing$ lui appartient), il possède un élément maximal $(a_i)_{i \in I}$ en vertu du th. de Zorn. On en déduit (si $A \neq \{0\}$) que pour tout $x \in E$, il existe un élément $\mu \neq 0$ de A et une famille $(\xi_i)$ d’éléments de A tels que $\mu x = \sum_i \xi_i a_i$ (cf. II, p. 95–96).

#### Proposition 19 {#alg-ii-s1-prop-19 .statement}

Soit E un A-module, somme directe d’une famille $(M_\lambda)_{\lambda \in L}$ de sous-modules. Si, pour chaque $\lambda \in L$, $S_\lambda$ est une partie libre (resp. un ensemble générateur, une base) de $M_\lambda$, alors $S = \bigcup_{\lambda \in L} S_\lambda$ est une partie libre (resp. un ensemble générateur, une base) de E.

La proposition résulte des définitions et de la relation $A_s^{(S)} = \bigoplus_{\lambda \in L} A_s^{(S_\lambda)}$ (associativité de la somme directe, cf. II, p. 12).

Remarque 1). — D’après la déf. 10 (II, p. 25), si $A \neq \{0\}$ et si $(a_t)_{t \in I}$ est une famille libre, aucun élément $a_\kappa$ ne peut être égal à une combinaison linéaire des $a_t$ d’indice $t \neq \kappa$. Mais inversement, une famille $(a_t)$ qui vérifie cette condition n’est pas nécessairement une famille libre. Par exemple, soit A un anneau intègre, et soient $a, b$ deux éléments distincts et non nuls; dans A, considéré comme A-module, $a$ et $b$ forment un système lié, puisque l’on a $(-b)a + ab = 0$. Mais en général il n’existe pas d’élément $x \in A$ tel que l’on ait $a = xb$ ou $b = xa$ (cf. toutefois II, p. 96, Remarque).

On dit qu’un élément $x$ d’un module E est libre si $\{x\}$ est une partie libre, c’est-à-dire si la relation $\alpha x = 0$ entraîne $\alpha = 0$. Tout élément d’une partie libre est libre, et en particulier 0 ne peut appartenir à aucune partie libre lorsque $A \neq \{0\}$.

#### Remarque 2 {#alg-ii-s1-n11-rem-2 .statement}

Un module libre peut avoir des éléments $\neq 0$ qui ne sont pas libres: par exemple, le A-module $A_s$ est libre mais les diviseurs de zéro à droite dans A ne sont pas des éléments libres de $A_s$.

#### Remarque 3 {#alg-ii-s1-n11-rem-3 .statement}

Dans le groupe additif $\mathbf{Z}/(n)$ ($n$ entier $\geqslant 2$) considéré comme $\mathbf{Z}$-module, aucun élément n’est libre, et $a$ fortiori $\mathbf{Z}/(n)$ n’est pas un module libre.

#### Remarque 4 {#alg-ii-s1-n11-rem-4 .statement}

Il peut se faire que tout élément $\neq 0$ d’un A-module soit libre, sans que ce module soit libre. Par exemple, le corps $\mathbf{Q}$ des nombres rationnels est un $\mathbf{Z}$-module qui possède cette propriété, car deux éléments $\neq 0$ de $\mathbf{Q}$ forment toujours un système lié, et une base de $\mathbf{Q}$ ne pourrait donc comporter qu’un seul élément $a$; mais les éléments de $\mathbf{Q}$ ne sont pas tous de la forme $na$, avec $n \in \mathbf{Z}$ (cf. VII, § 3).

#### Proposition 20 {#alg-ii-s1-prop-20 .statement}

*Tout A-module E est isomorphe à un module quotient d’un A-module libre.*

En effet, si T est un ensemble générateur de E, il existe une application linéaire surjective $A_s^{(T)} \to E$ (II, p. 24, cor. 2), et si R est le noyau de cette application, E est isomorphe à $A_s^{(T)}/R$.

On peut en particulier prendre $T = E$; on a donc une application linéaire surjective $A_s^{(E)} \to E$, dite *canonique*.

En particulier, dire qu’un A-module E est *de type fini* (II, p. 15) signifie qu’il est isomorphe à un quotient d’un A-module libre ayant une *base finie*, ou encore qu’il existe une suite exacte de la forme

$$
A_s^n \to E \to 0 \qquad (n \text{ entier } > 0).
$$

On notera que si $A \neq \{0\}$, toute base d’un module libre *de type fini* E est nécessairement *finie*, car si S est un système générateur fini et B une base de E, chaque élément de S est combinaison linéaire d’un nombre fini d’éléments de B, et si B’ est l’ensemble de tous les éléments de B qui figurent ainsi dans l’expression des éléments de S, B’ est fini et tout $x \in E$ est combinaison linéaire d’éléments de B’, donc $B' = B$.

#### Proposition 21 {#alg-ii-s1-prop-21 .statement}

*Toute suite exacte de A-modules*

$$
0 \longrightarrow G \xrightarrow{g} E \xrightarrow{f} F \longrightarrow 0
$$

*dans laquelle F est un A-module libre, est scindée* (II, p. 21). *De façon précise, si* $(b_\lambda)_{\lambda \in L}$ *est une base de F, et, pour chaque* $\lambda \in L$, $a_\lambda$ *un élément de E tel que* $f(a_\lambda) = b_\lambda$, *la famille* $(a_\lambda)_{\lambda \in L}$ *est libre et engendre un sous-module supplémentaire de* $g(G)$.

Il existe en effet une application linéaire $h : F \to E$ et une seule telle que $h(b_\lambda) = a_\lambda$ pour tout $\lambda \in L$ (II, p. 25, cor. 3). Comme $h$ est une section linéaire associée à $f$, la proposition résulte de I, p. 46, prop. 15.

*Remarque 5).* — Soit $(a_i)_{1 \leq i \leq n}$ une *base* d’un A-module E, et soit $(b_i)_{1 \leq i \leq n}$ une famille d’éléments de E donnée par les relations
$$
b_i = \lambda_{1i} a_1 + \cdots + \lambda_{ii} a_i \qquad (1 \leq i \leq n)
$$
où $\lambda_{ii}$ est *inversible* dans A; alors $(b_i)_{1 \leq i \leq n}$ est une *base* de E. Il suffit de raisonner par récurrence sur $n$, la proposition étant évidente pour $n = 1$. Si E’ est le sous-module de E engendré par la famille $(a_i)_{1 \leq i \leq n-1}$, il résulte de l’hypothèse de récurrence que $(b_i)_{1 \leq i \leq n-1}$ est une base de E’; d’autre part, on déduit de (46) que si l’on avait $\mu b_n \in E'$ avec $\mu \in A$, on aurait aussi $\mu \lambda_{nn} a_n \in E'$, d’où $\mu = 0$ puisque $\lambda_{nn}$ est inversible. La famille $(b_i)_{1 \leq i \leq n}$ est donc libre, et comme on a
$$
a_n = -\lambda_{nn}^{-1} \lambda_{1n} a_1 - \cdots - \lambda_{nn}^{-1} \lambda_{n-1,n} a_{n-1} + \lambda_{nn}^{-1} b_n
$$
on voit que $(b_i)_{1 \leq i \leq n}$ est un système générateur de E, ce qui achève la démonstration. On généralise aisément ce résultat à une famille $(a_i)_{i \in I}$ dont l’ensemble d’indices I est bien ordonné.

### 12. Annulateurs. Modules fidèles. Modules monogènes

#### Définition 11 {#alg-ii-s1-def-11 .statement}

On appelle annulateur d’une partie S d’un A-module E l’ensemble des éléments $\alpha \in A$ tels que $\alpha x = 0$ pour tout $x \in S$.

L’annulateur de S se note souvent Ann(S); pour une partie S réduite à un seul élément $x$, on écrit Ann(x) au lieu de Ann(\{x\}) et on dit que Ann(x) est l’annulateur de $x$.

La relation $\alpha x = 0$ s’exprime encore en disant que $x$ est annulé par $\alpha$.

Il est immédiat que l’annulateur d’une partie quelconque S de E est un idéal à gauche de A; pour qu’il soit égal à A, il faut et il suffit (en vertu de (M_{IV})) que S = \{0\}. Si deux parties S, T de E sont telles que S $\subset$ T, l’annulateur de T est contenu dans l’annulateur de S. Si $(S_t)_{t \in I}$ est une famille quelconque de parties de E, l’annulateur de la réunion $\bigcup_t S_t$ est l’intersection des annulateurs des $S_t$. En particulier, l’annulateur d’une partie S de E est l’intersection des annulateurs des éléments de S. Dire qu’un élément de E est libre équivaut à dire que son annulateur est \{0\}. Pour tout $x \in E$ et tout $\alpha \in A$, l’annulateur de $\alpha x$ est l’ensemble des $\beta \in A$ tels que $\beta \alpha \in \mathrm{Ann}(x)$.

L’annulateur d’un sous-module M de E est un idéal bilatère de A; en effet, si $\alpha x = 0$ pour tout $x \in M$, on a aussi $\alpha (\beta x) = 0$ pour tout $x \in M$ et tout $\beta \in A$, donc $\alpha \beta$ appartient à l’annulateur de M pour tout $\beta \in A$. En particulier l’annulateur de E est un idéal bilatère de A.

Pour tout $\alpha \in A$, soit $h_\alpha$ l’homothétie $x \mapsto \alpha x$; on sait que l’application $\alpha \mapsto h_\alpha$ de A dans l’anneau $\mathcal{E} = \mathrm{Hom}_\mathbf{Z}(E, E)$ des endomorphismes du groupe commutatif (sans opérateur) E, est un homomorphisme d’anneaux (II, p. 43). L’image réciproque de 0 par cet homomorphisme est l’annulateur $a$ de E; l’image de A par l’homomorphisme $\alpha \mapsto h_\alpha$ est donc isomorphe à l’anneau quotient $A/a$. On dit que le module E est fidèle si son annulateur $a$ est réduit à 0.

Soient E un A-module quelconque, $a$ un idéal bilatère de A contenu dans Ann(E), et soit $\dot{\alpha}$ un élément de l’anneau quotient $A/a$; pour tout $x \in E$, l’élément $\alpha x$ est le même pour tous les $\alpha \in A$ appartenant à la classe $\dot{\alpha}$ mod. $a$; si on désigne cet élément par $\dot{\alpha} x$, on voit aussitôt que l’application $(\dot{\alpha}, x) \mapsto \dot{\alpha} x$ définit (avec l’addition dans E) une structure de $(A/a)$-module sur E. Lorsqu’on prend $a = \mathrm{Ann}(E)$, le $(A/a)$-module E ainsi défini est fidèle; nous dirons que c’est le module fidèle associé au A-module E. On observera que tout sous-module d’un A-module E est aussi un sous-module du module fidèle associé, et réciproquement.

#### Définition 12 {#alg-ii-s1-def-12 .statement}

On dit qu’un module est monogène s’il est engendré par un seul élément.

La prop. 9 de II, p. 16 montre que, si E est un A-module monogène, et si $a$ est un élément engendrant E, E est identique à l’ensemble $A.a$ des $\xi a$, où $\xi$ parcourt A.

#### Exemple 1 {#alg-ii-s1-n12-exa-1 .statement}

Tout groupe monogène étant commutatif (I, p. 47, prop. 18) est un $\mathbf{Z}$-module monogène.

#### Exemple 2 {#alg-ii-s1-n12-exa-2 .statement}

Si $A$ est un anneau commutatif, les sous-modules monogènes du $A$-module $A$ ne sont autres que les *idéaux principaux* (I, p. 99) de l’anneau $A$.

#### Exemple 3 {#alg-ii-s1-n12-exa-3 .statement}

Tout $A$-module *simple* $E$ est monogène, puisque le sous-module de $E$ engendré par un élément $\neq 0$ de $E$ est nécessairement égal à $E$.

#### Proposition 22 {#alg-ii-s1-prop-22 .statement}

*Soit $A$ un anneau. Tout module quotient de $A_s$ est monogène. Inversement, soient $E$ un $A$-module monogène, $c$ un générateur de $E$, et $a$ son annulateur; l’application linéaire $\xi \mapsto \xi c$ définit, par passage au quotient, un isomorphisme de $A_s/a$ sur $E$.*

Comme $A_s$ est lui-même monogène, étant engendré par 1, la première assertion résulte de II, p. 16, cor. 1. La seconde est évidente, puisque $\xi \mapsto \xi c$ est par hypothèse surjective et a pour noyau $a$.

On notera que si $A$ n’est pas commutatif, les annulateurs de deux générateurs distincts $c, c'$ d’un $A$-module monogène $E$ sont en général *distincts*, et sont aussi distincts de l’annulateur du module $E$. Au contraire, si $A$ est *commutatif*, l’annulateur d’un générateur $c$ de $E$ est contenu dans l’annulateur de tout élément de $E$, donc est l’annulateur de $E$ tout entier.

#### Corollaire {#alg-ii-s1-n12-cor-1 .statement}

*Tout sous-module d’un $A$-module monogène $E$ est isomorphe à un module quotient $b/a$, où $a$ et $b$ sont deux idéaux à gauche de $A$ tels que $a \subset b$. Tout module quotient d’un $A$-module monogène est monogène.*

La seconde assertion est immédiate, et la première résulte de la prop. 22 et de I, p. 39, th. 4.

On notera par contre qu’un sous-module d’un module monogène n’est pas nécessairement monogène. Par exemple, si $A$ est un anneau commutatif dans lequel il existe des idéaux non principaux (VII, § 1, no 1), ces idéaux sont des sous-modules non monogènes du $A$-module monogène $A$.

Il résulte des définitions que le sous-module d’un $A$-module $E$ engendré par une famille $(a_i)$ d’éléments de $E$ est la *somme* des sous-modules monogènes $Aa_i$ de $E$; pour que $(a_i)$ soit une *base* de $E$, il faut et il suffit que chacun des $a_i$ soit un élément *libre* de $E$ et que la somme des $Aa_i$ soit *directe*.

#### Proposition 23 {#alg-ii-s1-prop-23 .statement}

*Soit $E$ un $A$-module, somme directe d’une famille infinie $(M_i)_{i \in I}$ de sous-modules non réduits à 0. Pour tout système générateur $S$ de $E$, on a $\mathrm{Card}(S) \geqslant \mathrm{Card}(I)$.*

Pour $x \in S$, soit $C_x$ l’ensemble fini des indices $i \in I$ tels que le composant de $x$ dans $M_i$ soit $\neq 0$, et posons $C = \bigcup_{x \in S} C_x$. Tout $x \in S$ appartient par définition au sous-module de $E$ somme directe des $M_i$ pour $i \in C$, et l’hypothèse que $S$ engendre $E$ entraîne donc $C = I$; comme $I$ est infini par hypothèse, il en est de même de $S$ (E, III, p. 36, cor. 1); on a par suite $\mathrm{Card}(I) = \mathrm{Card}(C) \leqslant \mathrm{Card}(S)$ (E, III, p. 49, cor. 3).

#### Corollaire 1 {#alg-ii-s1-prop-23-cor-1 .statement}

*Les hypothèses étant celles de la prop. 23, supposons que chaque $M_i$ soit monogène, et que $E$ soit somme directe d’une seconde famille $(N_\lambda)_{\lambda \in L}$ de sous-modules monogènes non réduits à 0. Alors, on a $\mathrm{Card}(L) = \mathrm{Card}(I)$.*

En effet, si $b_\lambda$ est un générateur de $N_\lambda$, l’ensemble des $b_\lambda$ est un système générateur de $E$, donc $\mathrm{Card}(L) \geqslant \mathrm{Card}(I)$. En particulier $L$ est infini, et en échangeant les rôles de $(M_i)$ et de $(N_\lambda)$, on a de même $\mathrm{Card}(I) \geqslant \mathrm{Card}(L)$, d’où le corollaire.

#### Corollaire 2 {#alg-ii-s1-prop-23-cor-2 .statement}

*Si un module $E$ admet une base infinie $B$, tout système générateur de $E$ a un cardinal $\geqslant \mathrm{Card}(B)$, et toute base de $E$ est équipotente à $B$.*

### 13. Changement de l’anneau des scalaires

Soient $A, B$ deux anneaux, $\rho$ un homomorphisme de l’anneau $B$ dans l’anneau $A$. Pour tout $A$-module $E$, la loi externe $(\beta, x) \mapsto \rho(\beta)x$ définit (avec l’addition) une structure de *B-module*, dit *associée* à $\rho$ et à la structure de $A$-module de $E$; on notera ce $B$-module $\rho_*(E)$ ou $E_{[B]}$ (et même simplement $E$) si aucune confusion n’en résulte. En particulier, si $B$ est un *sous-anneau* de $A$ et $\rho : B \to A$ l’injection canonique, on dit que $E_{[B]}$ est le $B$-module obtenu par *restriction* à $B$ de l’anneau des scalaires $A$; par abus de langage, on emploie encore cette expression lorsque l’homomorphisme $\rho$ est quelconque.

Si $F$ est un sous-module du $A$-module $E$, $\rho_*(F)$ est un sous-module de $\rho_*(E)$, et $\rho_*(E/F)$ est égal à $\rho_*(E)/\rho_*(F)$.

Soient $E, F$ deux $A$-modules; toute application $A$-linéaire $u : E \to F$ est aussi une application $B$-linéaire $E_{[B]} \to F_{[B]}$ que l’on note $\rho_*(u)$; autrement dit, on a une *injection canonique* de $\mathbf{Z}$-modules

$$
\mathrm{Hom}_A(E, F) \to \mathrm{Hom}_B(E_{[B]}, F_{[B]}).
$$

Cette application n’est pas nécessairement bijective; autrement dit une application $B$-linéaire $E_{[B]} \to F_{[B]}$ n’est pas nécessairement $A$-linéaire. En outre, un sous-$B$-module de $E_{[B]}$ n’est pas nécessairement un sous-$A$-module de $E$: c’est ainsi que si $A$ est un corps et $B$ un sous-corps de $A$, le sous-espace vectoriel $B_s$ du $B$-espace vectoriel $(A_s)_{[B]}$ n’est pas un sous-$A$-espace vectoriel si $B \neq A$.

Il est immédiat que pour toute famille $(E_t)_{t \in I}$ de $A$-modules, le $B$-module $\rho_*\left( \prod_{t \in I} E_t \right)$ (resp. $\rho_*\left( \bigoplus_{t \in I} E_t \right)$) est égal à $\prod_{t \in I} \rho_*(E_t)$ (resp. $\bigoplus_{t \in I} \rho_*(E_t)$).

Tout système générateur de $\rho_*(E)$ est un système générateur de $E$, la réciproque n’étant pas nécessairement vraie.

#### Proposition 24 {#alg-ii-s1-prop-24 .statement}

*Soient $A, B$ deux anneaux, $\rho : B \to A$ un homomorphisme d’anneaux.*

(i) *Si $\rho$ est surjectif, l’application canonique (47) est bijective. Pour tout $A$-module $E$, tout sous-$B$-module de $\rho_*(E)$ est un sous-$A$-module de $E$; tout système générateur de $E$ est un système générateur de $\rho_*(E)$.*

(ii) *Si $\rho$ est injectif, toute famille libre dans le $A$-module $E$ est une famille libre dans le $B$-module $\rho_*(E)$.*

La proposition résulte aussitôt des définitions.

On notera que même si $\rho$ est injectif, une famille libre dans $\rho_*(E)$ n’est pas nécessairement libre dans $E$.

\* Par exemple, 1 et $\sqrt{2}$ ne forment pas un système libre dans $\mathbf{R}$ considéré comme $\mathbf{R}$-espace vectoriel, bien qu’ils forment un système libre dans $\mathbf{R}$ considéré comme $\mathbf{Q}$-espace vectoriel (cf. Remarque 1).*

#### Proposition 25 {#alg-ii-s1-prop-25 .statement}

*Soient $A, B$ deux anneaux, $\varphi : B \to A$ un homomorphisme d’anneaux, $E$ un $A$-module. Soit $(\alpha_\lambda)_{\lambda \in L}$ un système générateur (resp. une famille libre d’éléments, une base) de $A$ considéré comme $B$-module à gauche. Soit $(a_\mu)_{\mu \in M}$ un système générateur (resp. une famille libre d’éléments, une base) du $A$-module $E$. Alors $(\alpha_\lambda a_\mu)_{(\lambda, \mu) \in L \times M}$ est un système générateur (resp. (lorsque $\varphi$ est injectif) une famille libre d’éléments, une base) du $B$-module $\rho_*(E)$.*

En effet, si $x = \sum_{\mu \in M} \gamma_\mu a_\mu$, où $\gamma_\mu \in A$, et si $(\alpha_\lambda)$ est un système générateur de $A$, on peut écrire $\gamma_\mu = \sum_{\lambda \in L} \rho(\beta_{\lambda \mu}) \alpha_\lambda$, avec $\beta_{\lambda \mu} \in B$, pour tout $\mu \in M$, d’où $x = \sum_{\mu, \lambda} \rho(\beta_{\lambda \mu}) \alpha_\lambda a_\mu$. D’autre part, si $(\alpha_\lambda)$ et $(a_\mu)$ sont des familles libres, une relation $\sum_{\lambda, \mu} \rho(\beta_{\lambda \mu}) \alpha_\lambda a_\mu = 0$, avec $\beta_{\lambda \mu} \in B$, s’écrit $\sum_{\mu \in M} \left( \sum_{\lambda \in L} \rho(\beta_{\lambda \mu}) \alpha_\lambda \right) a_\mu = 0$; elle entraîne donc $\sum_{\lambda \in L} \rho(\beta_{\lambda \mu}) \alpha_\lambda = 0$ pour tout $\mu \in M$, et par suite $\beta_{\lambda \mu} = 0$ quels que soient $\lambda, \mu$ si $\rho$ est injectif.

#### Corollaire {#alg-ii-s1-n13-cor-1 .statement}

*Si $A$ est un $B$-module à gauche de type fini et $E$ un $A$-module à gauche de type fini, $\rho_*(E)$ est un $B$-module à gauche de type fini.*

Soient $C$ un troisième anneau, $\rho' : C \to B$ un homomorphisme d’anneau, $\rho'' = \rho \circ \rho'$ l’homomorphisme composé. Il résulte aussitôt des définitions que l’on a $\rho''_*(E) = \rho'_*(\rho_*(E))$ pour tout $A$-module $E$. En particulier si $\rho$ est un *isomorphisme* de $B$ sur $A$, on a $E = \rho'_*(\rho_*(E))$, en désignant par $\rho'$ l’isomorphisme réciproque de $\rho$.

#### Remarque 1 {#alg-ii-s1-n13-rem-1 .statement}

Soient $K$ un corps, $A$ un sous-anneau de $K$ ayant la propriété suivante: pour toute famille finie $(\xi_i)_{1 \leq i \leq n}$ d’éléments de $K$, il existe un $\gamma \in A$, non nul et tel que $\gamma \xi_i \in A$ pour $1 \leq i \leq n$ (hypothèse toujours vérifiée lorsque $A$ est *commutatif* et $K$ le corps des fractions de $A$). Soient $E$ un espace vectoriel sur $K$, $E_{[A]}$ le $A$-module obtenu par restriction à $A$ de l’anneau des scalaires. Alors, si une famille $(x_\lambda)_{\lambda \in L}$ est *libre dans* $E_{[A]}$, elle est aussi *libre dans* $E$. On peut en effet se borner au cas où $L = \{1, n\}$; si on avait une relation $\sum_{i=1}^n \xi_i x_i = 0$ avec $\xi_i \in K$, $\xi_i$ non tous nuls, on en déduirait, pour tout $\beta \in A$, $\sum_{i=1}^n (\beta \xi_i) x_i = 0$. Par hypothèse on peut trouver $\beta \neq 0$ dans $A$ tel que $\beta \xi_i = \alpha_i$ appartienne à $A$ pour tout $i$; mais la relation $\sum_{i=1}^n \alpha_i x_i = 0$ est contraire à l’hypothèse, les $\alpha_i$ n’étant pas tous nuls.

#### Remarque 2 {#alg-ii-s1-n13-rem-2 .statement}

Si l’homomorphisme d’anneaux $\rho : B \to A$ est surjectif, et si $b$ est son noyau (de sorte que $A$ s’identifie canoniquement à $B/b$), alors, pour tout $A$-module $E$, $b$ est contenu dans l’annulateur de $\rho_*(E)$, et $E$ est le $A$-module déduit de $\rho_*(E)$ par le procédé défini dans II, p. 28.

Soient $A, B$ deux anneaux, $\rho : B \to A$ un homomorphisme. Soient $E$ un $A$-module, $F$ un $B$-module; une application $B$-linéaire $u : F \to \rho_*(E)$ (dite aussi *application B-linéaire de F dans E* si aucune confusion n’en résulte) est encore appelée *application semi-linéaire* (relative à $\rho$) du $B$-module $F$ dans le $A$-module $E$; on dit aussi que le couple $(u, \rho)$ est un *dimorphisme* de $F$ dans $E$; cela signifie donc que pour $x \in F, y \in F$ et $\beta \in B$, on a

$$
\begin{cases}
u(x + y) = u(x) + u(y) \\
u(\beta x) = \rho(\beta)u(x).
\end{cases}
$$

L’ensemble $\mathrm{Hom}_B(F, \rho_*(E))$ des applications $B$-linéaires de $F$ dans $E$ s’écrit aussi $\mathrm{Hom}_B(F, E)$ si cela n’entraîne pas confusion.

Lorsque $\rho$ est un *isomorphisme* de $B$ sur $A$, la relation $u(\beta x) = \rho(\beta)u(x)$ pour tout $\beta \in B$ s’écrit aussi $u(\rho'(\alpha)x) = \alpha u(x)$ pour tout $\alpha \in A$, en désignant par $\rho'$ l’isomorphisme réciproque de $\rho$; dire que $u$ est semi-linéaire pour $\rho$ équivaut alors à dire que $u$ est une application $A$-linéaire de $\rho'_*(F)$ *dans* $E$.

#### Exemple {#alg-ii-s1-n13-exa-1 .statement}

On a vu (II, p. 2) qu’une homothétie $h_\alpha : x \mapsto \alpha x$ dans un $A$-module $E$ n’est pas nécessairement une application linéaire. Mais si $\alpha$ est *inversible*, $h_\alpha$ est une application *semi-linéaire* (d’ailleurs bijective) relative à l’automorphisme intérieur $\xi \mapsto \alpha \xi \alpha^{-1}$ de $A$, car on a $\alpha (\lambda x) = (\alpha \lambda \alpha^{-1})(\alpha x)$.

Soient $C$ un troisième anneau, $\rho' : C \to B$ un homomorphisme, $G$ un $C$-module. Si $v : G \to F$ est une application semi-linéaire relative à $\rho'$, la composée $w = u \circ v$ est une application semi-linéaire de $G$ dans $E$ relative à l’homomorphisme $\rho'' = \rho \circ \rho'$. Si $\rho$ est un *isomorphisme* et si $u : F \to E$ est une application semi-linéaire *bijective* relative à $\rho$, l’application réciproque $u' : E \to F$ est une application semi-linéaire *relative à l’isomorphisme réciproque* $\rho' : A \to B$ de $\rho$.

On voit donc que pour l’espèce de structure définie par la donnée sur un couple $(A, E)$ d’ensembles, d’une structure d’anneau sur $A$ et d’une structure de $A$-module à gauche sur $E$, les *dimorphismes* $(u, \rho)$ peuvent être pris pour *morphismes* (E, IV, p. 11); nous supposerons toujours par la suite qu’on a fait ce choix de morphismes.

*Remarque 3).* — Soient $A_1, A_2$ deux anneaux, $A = A_1 \times A_2$ leur produit, et posons $e_1 = (1, 0), e_2 = (0, 1)$ dans $A$, de sorte que $A_1$ et $A_2$ s’identifient canoniquement aux idéaux bilatères $Ae_1$ et $Ae_2$ de $A$. Pour tout $A$-module $E$, $e_1 E$ et $e_2 E$ sont des sous-$A$-modules $E_1, E_2$ de $E$, annulés respectivement par $e_2$ et $e_1$, de sorte qu’en identifiant canoniquement $A/Ae_2$ à $A_1$ et $A/Ae_1$ à $A_2$, $E_1$ (resp. $E_2$) est muni d’une structure de $A_1$-module (resp. de $A_2$-module). En outre, $E$ est *somme directe* de $E_1$ et $E_2$, car tout $x \in E$ s’écrit $x = e_1 x + e_2 x$, et la relation $e_1 x = e_2 y$ entraîne $e_1 x = e_1^2 x = e_1 e_2 y = 0$. Inversement, pour tout couple formé d’un $A_1$-module $F_1$ et d’un $A_2$-module $F_2$, soient $E_1$ le $A$-module $(p_1)_*(F_1)$, $E_2$ le $A$-module $(p_2)_*(F_2)$, $p_1$ et $p_2$ étant les projections de $A$ sur $A_1$ et $A_2$ respectivement; alors, dans le $A$-module $E = E_1 \oplus E_2$, on a $E_1 = e_1 E$, $E_2 = e_2 E$. L’étude des $A$-modules est ainsi ramenée à celle des $A_1$-modules et à celle des $A_2$-modules. En particulier, tout sous-module $M$ de $E$ est de la forme $M_1 \oplus M_2$, où $M_1 = e_1 M$ et $M_2 = e_2 M$.

### 14. Multimodules

Soient $A$, $B$ deux anneaux, et considérons sur un ensemble $E$ deux structures de module à gauche ayant la même loi additive, et dont les anneaux d’opérateurs sont respectivement $A$ et $B$; soit $\mathcal{E}$ l’anneau des endomorphismes du groupe additif $E$, et pour tout $\alpha \in A$ (resp. $\beta \in B$) désignons par $h_\alpha$ (resp. $h'_\beta$) l’élément $x \mapsto \alpha x$ (resp. $x \mapsto \beta x$) de $\mathcal{E}$. Il est clair que les trois propriétés suivantes sont équivalentes :
a) $h_\alpha \circ h'_\beta = h'_\beta \circ h_\alpha$ quels que soient $\alpha$ et $\beta$; b) l’image de $A$ par l’homomorphisme $\alpha \mapsto h_\alpha$ est contenue dans $\mathrm{Hom}_B(E, E)$; c) l’image de $B$ par l’homomorphisme $\beta \mapsto h'_\beta$ est contenue dans $\mathrm{Hom}_A(E, E)$. Lorsque la structure de $A$-module (resp. de $B$-module) considérée est une structure de module à droite, il faut remplacer dans b) (resp. c)) l’anneau $A$ par $A^0$ (resp. $B^0$). On exprime les propriétés précédentes en disant que les deux structures de module (à droite ou à gauche) définies sur $E$ sont compatibles.

#### Définition 13 {#alg-ii-s1-def-13 .statement}

Soient $(A_\lambda)_{\lambda \in L}$, $(B_\mu)_{\mu \in M}$ deux familles d’anneaux; on appelle $((A_\lambda), (B_\mu))$-multimodule (ou multimodule sur les familles d’anneaux $(A_\lambda)_{\lambda \in L}$, $(B_\mu)_{\mu \in M}$) un ensemble $E$ muni, pour chaque $\lambda \in L$, d’une structure de $A_\lambda$-module à gauche, et pour chaque $\mu \in M$ d’une structure de $B_\mu$-module à droite, toutes ces structures de module étant deux à deux compatibles.

Lorsque la famille $(B_\mu)$ (resp. $(A_\lambda)$) est vide, on dit que $E$ est un multimodule à gauche (resp. à droite). Lorsque $\mathrm{Card}(L) + \mathrm{Card}(M) = 2$, on dit « bimodule » au lieu de « multimodule »; il est souvent commode alors de considérer (comme on peut toujours le faire en remplaçant un des anneaux d’opérateurs par son opposé, cf. II, p. 2) un bimodule comme muni d’une structure de module à gauche par rapport à un anneau $A$ et de module à droite par rapport à un anneau $B$, la compatibilité des structures s’exprimant donc par la relation

$$
\alpha(x \beta) = (\alpha x) \beta \quad \text{pour } x \in E, \alpha \in A, \beta \in B.
$$

On dit alors aussi que $E$ est un $(A, B)$-bimodule.

On dit que deux structures de multimodule sur un ensemble $E$ sont compatibles si toutes les structures de module sur $E$ qui définissent l’une ou l’autre de ces structures de multimodule sont deux à deux compatibles.

#### Exemple 1 {#alg-ii-s1-n14-exa-1 .statement}

Sur un anneau A, les structures de module de $A_s$ et $A_d$ sont compatibles, et A peut donc être canoniquement considéré comme un $(A, A)$-bimodule.

#### Exemple 2 {#alg-ii-s1-n14-exa-2 .statement}

Un A-module à gauche E est canoniquement muni d’une structure de module à gauche sur l’anneau $\mathrm{End}_A(E)$, et sur E la structure de A-module et celle de $\mathrm{End}_A(E)$-module sont compatibles.

Il est clair que lorsque E est un multimodule sur deux familles $(A_\lambda)_{\lambda \in L}$, $(B_\mu)_{\mu \in M}$ d’anneaux, E est aussi un multimodule sur deux sous-familles quelconques $(A_{\lambda'})_{\lambda' \in L'}$, $(B_{\mu'})_{\mu' \in M'}$, étant entendu que les structures de $A_\lambda$-module et de $B_\mu$-module pour $\lambda \in L'$ et $\mu \in M'$ sont celles initialement données.

Les multimodules étant des groupes commutatifs à opérateurs particuliers, on peut leur appliquer les résultats des n°s 2 à 10 (cf. II, p. 23, Remarque); en particulier, si E, F sont deux $((A_\lambda), (B_\mu))$-multimodules, un homomorphisme $u : E \to F$ est une application qui est un $A_\lambda$-homomorphisme pour tout $\lambda \in L$ et un $B_\mu$-homomorphisme pour tout $\mu \in M$. Les sous-groupes stables d’un $((A_\lambda), (B_\mu))$-multimodule sont des $((A_\lambda), (B_\mu))$-multimodules (dits sous-multimodules), ainsi que les quotients par de tels sous-groupes (dits multimodules quotients); de même pour les produits et sommes directes.

Soient E un $((A_\lambda), (B_\mu))$-multimodule, et pour chaque $\lambda \in L$ (resp. chaque $\mu \in M$) soit $\varphi_\lambda : A'_\lambda \to A_\lambda$ (resp. $\psi_\mu : B'_\mu \to B_\mu$) un homomorphisme d’anneaux; il est clair que les structures de $A'_\lambda$-module associées aux $\varphi_\lambda$ et aux structures de $A_\lambda$-module données sur E, et les structures de $B'_\mu$-module associées aux $\psi_\mu$ et aux structures de $B_\mu$-modules données sur E, sont deux à deux compatibles, donc définissent sur E une structure de $((A'_\lambda), (B'_\mu))$-multimodule, dite associée à la structure de $((A_\lambda), (B_\mu))$-multimodule donnée et aux $\varphi_\lambda$ et aux $\psi_\mu$.

Si E, F sont deux $((A_\lambda), (B_\mu))$-multimodules, on désigne par $\mathrm{Hom}_{(A_\lambda), (B_\mu)}(E, F)$ (ou simplement $\mathrm{Hom}(E, F)$) le groupe additif des homomorphismes de E dans F. Les formules (6) à (8) de II, p. 5 sont évidemment valables pour des homomorphismes de $((A_\lambda), (B_\mu))$-multimodules, et en particulier $\mathrm{Hom}(E, E) = \mathrm{End}(E)$ est muni d’une structure d’anneau; en outre $\mathrm{Hom}(E, F)$ est canoniquement muni d’une structure de $\mathrm{End}(F)$-module à gauche et de $\mathrm{End}(E)$-module à droite, ces deux structures étant compatibles; autrement dit, $\mathrm{Hom}(E, F)$ est canoniquement muni d’une structure de $(\mathrm{End}(F), \mathrm{End}(E))$-bimodule.

Supposons maintenant E muni d’une structure de multimodule dont les anneaux d’opérateurs à gauche (resp. à droite) sont d’une part les $A_\lambda$ pour $\lambda \in L$ (resp. les $B_\mu$ pour $\mu \in M$), d’autre part les anneaux d’une autre famille $(A'_{\lambda'})_{\lambda' \in L'}$ (resp. $(B'_{\mu'})_{\mu' \in M'}$). Supposons de même F muni d’une structure de multimodule dont les anneaux d’opérateurs à gauche (resp. à droite) sont d’une part les $A_\lambda$ pour $\lambda \in L$ (resp. les $B_\mu$ pour $\mu \in M$), d’autre part les anneaux d’une autre famille $(A''_{\lambda''})_{\lambda'' \in L''}$ (resp. $(B''_{\mu''})_{\mu'' \in M''}$); nous dirons pour abréger que E est un $((A_\lambda), (A'_{\lambda'}); (B_\mu), (B'_{\mu'}))$-multimodule, F un $((A_\lambda), (A''_{\lambda''}); (B_\mu), (B''_{\mu''}))$-multimodule. Considérons E et F comme des $((A_\lambda), (B_\mu))$-multimodules, en restreignant donc les opérateurs aux sous-familles $(A_\lambda)$ et $(B_\mu)$. En vertu de ce qu’on a vu au début ce n°, les structures de multimodules données sur E et F définissent canoniquement des homomorphismes d’anneaux $A'_{\lambda'} \to \mathrm{End}_{(A_{\lambda}), (B_{\mu})}(E)$, ${B'_{\mu'}}^0 \to \mathrm{End}_{(A_{\lambda}), (B_{\mu})}(E)$, $A''_{\lambda''} \to \mathrm{End}_{(A_{\lambda}), (B_{\mu})}(F)$, ${B''_{\mu''}}^0 \to \mathrm{End}_{(A_{\lambda}), (B_{\mu})}(F)$; en outre, deux éléments de $\mathrm{End}_{(A_{\lambda}), (B_{\mu})}(E)$ (resp. $\mathrm{End}_{(A_{\lambda}), (B_{\mu})}(F)$) images respectives d’éléments de deux anneaux distincts pris parmi les $A'_{\lambda'}$ ou les ${B'_{\mu'}}^0$ (resp. les $A''_{\lambda''}$ ou les ${B''_{\mu''}}^0$) sont permutables; on en conclut que les homomorphismes précédents définissent sur $\mathrm{Hom}_{(A_{\lambda}), (B_{\mu})}(E, F)$ une structure de *multimodule*, dont les anneaux d’opérateurs *à gauche* sont les $A''_{\lambda''} (\lambda'' \in L'')$ et les $B'_{\mu'} (\mu' \in M')$, et les anneaux d’opérateurs *à droite* sont les $A'_{\lambda'} (\lambda' \in L')$ et les $B''_{\mu''} (\mu'' \in M'')$.

Si maintenant $E'$ est un $((A_{\lambda}), (A'_{\lambda'}); (B_{\mu}), (B'_{\mu'}))$-multimodule, $F'$ un $((A_{\lambda}), (A''_{\lambda''}); (B_{\mu}), (B''_{\mu''}))$-multimodule, $\mathrm{Hom}_{(A_{\lambda}), (B_{\mu})}(E', F')$ est un $((A''_{\lambda''}), (B'_{\mu'}); (A'_{\lambda'}), (B''_{\mu''}))$-multimodule; si $u : E' \to E, v : F \to F'$ sont des homomorphismes de multimodules,

$$
\mathrm{Hom}(u, v) : \mathrm{Hom}_{(A_{\lambda}), (B_{\mu})}(E, F) \to \mathrm{Hom}_{(A_{\lambda}), (B_{\mu})}(E', F')
$$

est défini comme dans II, p. 6 et est un homomorphisme de *multimodules*.

#### Remarque 1 {#alg-ii-s1-n14-rem-1 .statement}

Soient F un A-module, C le *centre* de l’anneau A; comme les homothéties centrales permutent à toutes les homothéties, F est muni d’une structure de *bimodule* dont les anneaux d’opérateurs à gauche sont A et C. Si E est un second A-module, $\mathrm{Hom}_A(E, F)$ est donc muni canoniquement d’une structure de C-*module* (où, pour $f \in \mathrm{Hom}_A(E, F)$ et $\gamma \in C$, $\gamma f$ est l’homomorphisme $x \mapsto \gamma f(x)$); si E’, F’ sont deux A-modules, $u : E' \to E, v : F \to F'$ deux A-homomorphismes, l’application $\mathrm{Hom}(u, v)$ est C-*linéaire*.

#### Remarque 2 {#alg-ii-s1-n14-rem-2 .statement}

Soit E un A-module à gauche; comme A est canoniquement muni d’une structure de (A, A)-bimodule, il en est de même de la somme directe $A^{(T)}$ pour tout ensemble d’indices T; d’après ce qui précède, $\mathrm{Hom}_A(A_s^{(T)}, E)$ est canoniquement muni d’une structure de A-*module à gauche* provenant de la structure de A-module *à droite* de $A_s^{(T)}$: pour $f \in \mathrm{Hom}_A(A_s^{(T)}, E)$ et $\alpha \in A$, $\alpha f$ est l’application linéaire $x \mapsto f(x \alpha)$. Le cor. 2 de II, p. 24 définit une application canonique $j_{E, T}$ du module produit $E^T$ dans $\mathrm{Hom}_A(A_s^{(T)}, E)$, l’image par $j_{E, T}$ d’une famille $(x_t)_{t \in T}$ étant l’application linéaire $f : A_s^{(T)} \to E$ telle que $f(e_t) = x_t$ pour tout $t \in T$ (où $(e_t)$ est la base canonique de $A_s^{(T)}$); on sait (*loc. cit.*) que $j_{E, T}$ est *bijective* et il résulte de la définition donnée ci-dessus de la structure de A-module de $\mathrm{Hom}_A(A_s^{(T)}, E)$ que $j_{E, T}$ est A-*linéaire*. Enfin, si $u : E \to F$ est un homomorphisme de A-modules, le diagramme

$$
\begin{array}{ccc}
E^T & \xrightarrow{j_{E, T}} & \mathrm{Hom}_A(A_s^{(T)}, E) \\
\downarrow^{u^T} & & \downarrow^{\mathrm{Hom}(1, u)} \\
F^T & \xrightarrow{j_{F, T}} & \mathrm{Hom}_A(A_s^{(T)}, F)
\end{array}
$$

est *commutatif*.

On notera que pour T réduit à un seul élément, $j_E : E \to \mathrm{Hom}_A(A_s, E)$ n’est autre que l’application $x \mapsto \theta_x$ définie dans II, p. 4, *Exemple* 1.

## EXERCICES {#alg-ii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
