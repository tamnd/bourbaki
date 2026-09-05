---
book: fvr
book_title: Functions of a Real Variable
chapter: I
chapter_title: DÉRIVÉES
section: 1
section_title: Dérivée première
lang: fr
source: fvr-i-vii-fr
pdf_pages: 0009-0018, 0040-0041
extraction: ocr
subsections:
    - "no": 1
      title: Dérivée d’une fonction vectorielle
      page: 0
      pdf_page: 9
    - "no": 2
      title: Linéarité de la dérivation
      page: 13
      pdf_page: 11
    - "no": 3
      title: Dérivée d’un produit
      page: 14
      pdf_page: 12
    - "no": 4
      title: Dérivée de l’inverse d’une fonction
      page: 16
      pdf_page: 14
    - "no": 5
      title: Dérivée d’une fonction composée
      page: 17
      pdf_page: 15
    - "no": 6
      title: Dérivée d’une fonction réciproque
      page: 17
      pdf_page: 15
    - "no": 7
      title: Dérivées des fonctions numériques
      page: 18
      pdf_page: 16
statements: 37
exercises: 9
content_sha256: affe3213f341ff8fde732fe4ba642c8423e564e35a98a1fff0abe93a7ff567af
---

## § 1. DÉRIVÉE PREMIÈRE

Ainsi qu’il a été dit dans l’Introduction, nous étudierons dans ce chapitre et le suivant les propriétés infinitésimales des fonctions définies dans une partie du corps $\mathbf{R}$ des nombres réels, et prenant leurs valeurs dans un espace vectoriel topologique $E$ sur le corps $\mathbf{R}$; nous dirons pour abréger qu’une telle fonction est une fonction vectorielle d’une variable réelle. Le cas le plus important est celui où $E = \mathbf{R}$ (fonctions numériques finies d’une variable réelle). Lorsque $E = \mathbf{R}^n$, la considération d’une fonction vectorielle à valeurs-dans $E$ revient-à la considération simultanée de $n$ fonctions numériques finies.

Beaucoup des définitions et propriétés énoncées dans le chapitre I s’étendent aux fonctions définies dans une partie du corps $\mathbf{C}$ des nombres complexes, et prenant leurs valeurs dans un espace vectoriel topologique sur $\mathbf{C}$ (fonctions vectorielles d’une variable complexe). Certaines de ces définitions et propriété s’étendent même aux fonctions définies sur une partie d’un corps topologique commutatif quelconque $K$, et prenant leurs valeurs dans un espace vectoriel topologique sur $K$.

Nous signalerons ces généralisations au passage (voir en particulier I, p. 8, Remarque 2), en insistant surtout sur le cas des fonctions d’une variable complexe, de beaucoup le plus important avec celui des fonctions d’une variable réelle, et qui sera étudié de manière plus approfondie dans un Livre ultérieur.

### 1. Dérivée d’une fonction vectorielle

#### Définition 1 {#fvr-i-s1-def-1 .statement}

Soit $f$ une fonction vectorielle définie dans un intervalle $I \subset \mathbf{R}$, non réduit à un point. On dit que $f$ est dérivable en un point $x_0 \in I$ si
$$
\lim_{x \to x_0, x \in I, x \neq x_0} \frac{f(x) - f(x_0)}{x - x_0}
$$

existe (dans l’espace vectoriel où $\mathbf{f}$ prend ses valeurs); la valeur de cette de limite s’appelle dérivée première (ou simplement dérivée) de $\mathbf{f}$ au point $x_0$, et se note $\mathbf{f}'(x_0)$ ou $\mathrm{D}\mathbf{f}(x_0)$.

Si $\mathbf{f}$ est dérivable au point $x_0$, il en est de même de la restriction de $\mathbf{f}$ à tout intervalle $J \subset I$, non réduit à un point et tel que $x_0 \in J$, et la dérivée de cette restriction est égale à $\mathbf{f}'(x_0)$. Réciproquement, soit $J$ un intervalle contenu dans $I$ et contenant un voisinage de $x_0$ par rapport à $I$; si la restriction de $\mathbf{f}$ à $J$ admet une dérivée au point $x_0$, il en est de même de $\mathbf{f}$.

On exprime ces propriétés en disant que la notion de dérivée est une notion locale.

#### Remarque 1 {#fvr-i-s1-n1-rem-1 .statement}

En Cinématique, si le point $\mathbf{f}(t)$ est la position d’un point mobile dans l’espace $\mathbf{R}^3$ à l’instant $t$, $\frac{\mathbf{f}(t) - \mathbf{f}(t_0)}{t - t_0}$ est ce qu’on appelle la vitesse moyenne du mobile entre les instants $t_0$ et $t$, et sa limite $\mathbf{f}'(t_0)$ la vitesse instantanée (ou simplement vitesse) à l’instant $t_0$ (lorsque cette limite existe).*

#### Remarque 2 {#fvr-i-s1-n1-rem-2 .statement}

Si une fonction $\mathbf{f}$, définie dans $I$, est dérivable en un point $x_0 \in I$, elle est nécessairement continue par rapport à $I$ en ce point.

#### Définition 2 {#fvr-i-s1-def-2 .statement}

Soit $\mathbf{f}$ une fonction vectorielle définie dans un intervalle $I \subset \mathbf{R}$, et soit $x_0$ un point de $I$ tel que l’intervalle $I \cap (x_0, +\infty[$ (resp. $I \cap ]-\infty, x_0]$) ne soit pas réduit à un point. On dit que $\mathbf{f}$ est dérivable à droite (resp. à gauche) au point $x_0$ si la restriction de $\mathbf{f}$ à l’intervalle $I \cap (x_0, +\infty[$ (resp. $I \cap ]-\infty, x_0]$) est dérivable au point $x_0$; la valeur de la dérivée de cette restriction au point $x_0$, s’appelle dérivée à droite (resp. à gauche) de $\mathbf{f}$ au point $x_0$, et se note $\mathbf{f}'_d(x_0)$ (resp. $\mathbf{f}'_g(x_0)$).

Soit $\mathbf{f}$ une fonction vectorielle définie dans $I$, $x_0$ un point intérieur à $I$ et tel que $\mathbf{f}$ soit continue en ce point; il résulte des déf. 1 et 2 que, pour que $\mathbf{f}$ soit dérivable au point $x_0$, il faut et il suffit que $\mathbf{f}$ admette en ce point une dérivée à droite et une dérivée à gauche, et que ces dérivées soient égales; on a alors

$$
\mathbf{f}'(x_0) = \mathbf{f}'_d(x_0) = \mathbf{f}'_g(x_0).
$$

#### Exemple 1 {#fvr-i-s1-n1-exa-1 .statement}

Une fonction constante a en tout point une dérivée nulle.

#### Exemple 2 {#fvr-i-s1-n1-exa-2 .statement}

Une fonction linéaire affine $x \mapsto ax + b$ a en tout point une dérivée égale à $a$, donc constante.

#### Exemple 3 {#fvr-i-s1-n1-exa-3 .statement}

La fonction numérique $1/x$ (définie pour $x \neq 0$) est dérivable en tout point $x_0 \neq 0$, car on a $\left( \frac{1}{x} - \frac{1}{x_0} \right)/(x - x_0) = -\frac{1}{xx_0}$, et comme $1/x$ est continue au point $x_0$, la limite de l’expression précédente est $-1/x_0^2$.

#### Exemple 4 {#fvr-i-s1-n1-exa-4 .statement}

La fonction numérique $|x|$, définie dans $\mathbf{R}$, admet au point $x = 0$ une dérivée à droite égale à $+1$ et une dérivée à gauche égale à $-1$; elle n’est donc pas dérivable en ce point.

#### Exemple 5 {#fvr-i-s1-n1-exa-5 .statement}

La fonction numérique égale à 0 pour $x = 0$, à $x \sin 1/x$ pour $x \neq 0$, est définie et continue dans $\mathbf{R}$, mais elle n’admet ni dérivée à droite ni dérivée à gauche au point $x = 0$.* On peut donner des exemples de fonctions continues dans un intervalle et n’ayant de dérivée en aucun point de l’intervalle (I, p. 42, exerc. 2 et 3).

#### Définition 3 {#fvr-i-s1-def-3 .statement}

On dit qu’une fonction vectorielle $\mathbf{f}$ définie dans un intervalle $I \subset \mathbf{R}$ est dérivable (resp. dérivable à droite, dérivable à gauche) dans $I$ si elle est dérivable (resp.

dérivable à droite, dérivable à gauche) en tout point de $I$; la fonction $x \mapsto f'(x)$ (resp. $x \mapsto f'_d(x), x \mapsto f'_g(x)$) définie dans $I$, est appelée fonction dérivée ou (par abus de langage) dérivée (resp. dérivée à droite, dérivée à gauche) de $f$, et se note $f'$ ou $Df$ ou $df/dx$ (resp. $f'_d, f'_g$).

#### Remarque {#fvr-i-s1-n1-rem-3 .statement}

Une fonction peut être dérivable dans un intervalle, sans que sa dérivée soit continue en tout point de cet intervalle (cf. I, p. 43, exerc. 5); \* c’est ce que montre l’exemple de la fonction égale à 0 pour $x = 0$, à $x^2 \sin 1/x$ pour $x \neq 0$; elle a partout une dérivée, mais cette dérivée est discontinue au point $x = 0$.*

### 2. Linéarité de la dérivation

#### Proposition 1 {#fvr-i-s1-prop-1 .statement}

L’ensemble des fonctions vectorielles définies dans un intervalle $I \subset \mathbf{R}$, prenant leurs valeurs dans un même espace vectoriel topologique $E$, et dérivables au point $x_0$, est un espace vectoriel sur $\mathbf{R}$, et $f \mapsto Df(x_0)$ est une application linéaire de cet espace dans $E$.

En d’autres termes, si $f$ et $g$ sont définies dans $I$ et dérivables au point $x_0$, $f + g$ et $fa$ (a scalaire quelconque) sont dérivables au point $x_0$, et ont respectivement pour dérivées en ce point $f'(x_0) + g'(x_0)$ et $f'(x_0)a$. Cela résulte aussitôt de la continuité de $x + y$ et de $xa$ dans $E \times E$ et dans $E$ respectivement.

#### Corollaire {#fvr-i-s1-n2-cor-1 .statement}

L’ensemble des fonctions vectorielles définies dans un intervalle $I$, prenant leurs valeurs dans un même espace vectoriel topologique $E$, et dérivables dans $I$, est un espace vectoriel sur $\mathbf{R}$, et $f \mapsto Df$ est une application linéaire de cet espace dans l’espace vectoriel des applications de $I$ dans $E$.

#### Remarque {#fvr-i-s1-n2-rem-1 .statement}

Si on munit de la topologie de la convergence simple (ou de la topologie de la convergence uniforme) l’espace vectoriel des applications de $I$ dans $E$ et le sous-espace des applications dérivables (cf. TG, X, p. 4), l’application linéaire $f \mapsto Df$ n’est pas continue en général); \* par exemple, la suite des fonctions $f_n(x) = \sin n^2 x / n$ converge uniformément vers 0 dans $\mathbf{R}$, mais la suite des dérivées $f'_n(x) = n \cos n^2 x$ ne converge pas simplement vers 0. \*

#### Proposition 2 {#fvr-i-s1-prop-2 .statement}

Soient $E$ et $F$ deux espaces vectoriels topologiques sur $\mathbf{R}$, $u$ une application linéaire continue de $E$ dans $F$. Si $f$ est une fonction vectorielle définie dans un intervalle $I \subset \mathbf{R}$, prenant ses valeurs dans $E$ et dérivable au point $x_0 \in I$, la fonction composée $u \circ f$ admet au point $x_0$ une dérivée égale à $u(f'(x_0))$.

En effet, comme $\frac{u(f(x)) - u(f(x_0))}{x - x_0} = u \left( \frac{f(x) - f(x_0)}{x - x_0} \right)$, cela résulte de la continuité de $u$.

#### Corollaire {#fvr-i-s1-n2-cor-2 .statement}

Si $\varphi$ est une forme linéaire continue dans $E$, la fonction numérique $\varphi \circ f$ admet au point $x_0$ une dérivée égale à $\varphi(f'(x_0))$.

#### Exemple 1 {#fvr-i-s1-n2-exa-1 .statement}

Soit $f = (f_i)_{1 \leq i \leq n}$ une fonction à valeurs dans $\mathbf{R}^n$, définie dans un intervalle $I \subset \mathbf{R}$; chacune des fonctions numériques $f_i$ n’est autre que la fonction composée $\mathrm{pr}_i \circ f$, donc est dérivable au point $x_0$ si $f$ l’est, et on a alors $f'(x_0) = (f'_i(x_0))_{1 \leq i \leq n}$.

#### Exemple 2 {#fvr-i-s1-n2-exa-2 .statement}

\* En Cinématique, si $f(t)$ est la position d’un mobile M à l’instant t, $g(t)$ la position au même instant de la projection M’ de M sur un plan P (resp. une droite D) parallèlement à une droite (resp. un plan) non parallèle à P (resp. à D), g est composée de la projection u de $\mathbf{R}^3$ sur P (resp. D) et de f; comme u est une application linéaire (continue), on voit que la projection de la vitesse d’un mobile sur un plan (resp. une droite) est égale à la vitesse de la projection du mobile sur le plan (resp. la droite).*

#### Exemple 3 {#fvr-i-s1-n2-exa-3 .statement}

Soit f une fonction à valeurs complexes, définie dans un intervalle $I \subset \mathbf{R}$, et soit a un nombre complexe quelconque; la prop. 2 montre que si f est dérivable en un point $x_0 \in I$, il en est de même de af, et la dérivée de cette fonction au point $x_0$ est égale à $af''(x_0)$.

### 3. Dérivée d’un produit

Considérons maintenant $p$ espaces vectoriels topologiques $E_i$ ($1 \leq i \leq p$) sur $\mathbf{R}$, et une application multilinéaire¹ continue (que nous noterons
$$
(x_1, x_2 \ldots, x_p) \mapsto [x_1, x_2 \ldots x_p])
$$
de $E_1 \times E_2 \ldots \times E_p$ dans un espace vectoriel topologique F sur $\mathbf{R}$.

#### Proposition 3 {#fvr-i-s1-prop-3 .statement}

Pour chaque indice i ($1 \leq i \leq p$), soit $f_i$ une fonction définie dans un intervalle $I \subset \mathbf{R}$, prenant ses valeurs dans $E_i$, dérivable au point $x_0 \in I$. Alors la fonction
$$
x \mapsto [f_1(x) . f_2(x) \ldots f_p(x)]
$$
définie dans I et à valeurs dans F, admet au point $x_0$ une dérivée égale à
$$
\sum_{i=1}^p [f_1(x) \ldots f_{i-1}(x_0) . f_i'(x_0) . f_{i+1}(x_0) \ldots f_p(x_0)].
$$
Posons en effet $h(x) = [f_1(x) . f_2(x) \ldots f_p(x)]$; en vertu de l’identité
$$
[b_1 . b_2 \ldots b_p] - [a_1 . a_2 \ldots a_p] = \sum_{i=1}^p [b_1 \ldots b_{i-1} . (b_i - a_i) . a_{i+1} \ldots a_p],
$$
on peut écrire
$$
h(x) - h(x_0) = \sum_{i=1}^p [f_1(x) \ldots f_{i-1}(x) . (f_i(x) - f_i(x_0)) . f_{i+1}(x_0) \ldots f_p(x_0)].
$$
Multipliant les deux membres $\frac{1}{x - x_0}$ et faisant tendre x vers $x_0$ dans I, on obtient bien l’expression (1), en tenant compte de la continuité de
$$
(x_1, x_2, \ldots, x_p) \mapsto [x_1, x_2 \ldots x_p]
$$
et de la continuité de l’addition dans F.

¹ Rappelons (A, II, p. 71) qu’une application f de $E_1 \times E_2 \times \cdots \times E_p$ dans F est dite multilinéaire si toute application partielle
$$
x_i \mapsto f(a_1, \ldots, a_{i-1}, x_i, a_{i+1}, \ldots, a_p)
$$
de $E_i$ dans F ($1 \leq i \leq p$), les $a_j$ d’indice $\neq$ étant quelconques dans les $E_j$, est une application linéaire. On notera que si les $E_i$ et F sont des espaces de dimension finie sur $\mathbf{R}$, toute application multilinéaire de $E_1 \times E_2 \times \cdots \times E_p$ dans F est nécessairement continue; il n’en est pas de même si certains de ces espaces sont des espaces vectoriels topologiques de dimension infinie.

Lorsque certaines des fonctions $f_i$ sont des constantes, les termes de l’expression (1) contenant les dérivées $f_i'(x_0)$ de ces fonctions sont nuls.

Nous explicitons le cas particulier $p = 2$, le plus important pour les applications : si $(\mathbf{x}, \mathbf{y}) \mapsto [\mathbf{x}, \mathbf{y}]$ est une application bilinéaire continue de $E \times F$ dans $G$ (E, F, G espaces vectoriels topologiques sur $\mathbf{R}$), $f$ et g deux fonctions vectorielles dérivables au point $x_0$, prenant leurs valeurs respectivement dans E et F, la fonction vectorielle $x \mapsto [f(x), g(x)]$ (qu’on note encore $[f, g]$) admet au point $x_0$ une dérivée égale à $[f'(x_0), g(x_0)] + [f(x_0), g'(x_0)]$. En particulier, si $\mathbf{a}$ est un vecteur constant, $[\mathbf{a}, f]$ (resp. $[f, \mathbf{a}]$) admet au point $x_0$ une dérivée égale à $[\mathbf{a}, f'(x_0)]$ (resp. $[f'(x_0), \mathbf{a}]$).

Si $f$ et $g$ sont toutes deux dérivables dans I, il en est donc de même de $[f, g]$, et on a

$$
[f, g]' = [f', g] + [f, g'].
$$

#### Exemple 1 {#fvr-i-s1-n3-exa-1 .statement}

Soient $f$ une fonction numérique, $g$ une fonction vectorielle, toutes deux dérivables en un point $x_0$; la fonction $g/f$ admet au point $x_0$ une dérivée égale à $g'(x_0)f(x_0) + g(x_0)f'(x_0)$. En particulier, si $\mathbf{a}$ est un vecteur constant, $af$ admet une dérivée égale à $af'(x_0)$. Cette dernière remarque, jointe à l’exemple 1 de I, p. 13, prouve que si $\mathbf{f} = (f_i)_{1 \leq i \leq n}$ est une fonction vectorielle à valeurs dans $\mathbf{R}^n$, pour que $\mathbf{f}$ soit dérivable au point $x_0$, il faut et il suffit que chacune des fonctions numériques $f_i (1 \leq i \leq n)$ le soit : car, si $(e_i)_{1 \leq i \leq n}$ est la base canonique de $\mathbf{R}^n$, on peut écrire

$$
\mathbf{f} = \sum_{i=1}^n e_i f_i.
$$

#### Exemple 2 {#fvr-i-s1-n3-exa-2 .statement}

La fonction numérique $x^n$ provient de la fonction multilinéaire

$$
(x_1, x_2, \ldots, x_n) \mapsto x_1 x_2 \ldots x_n
$$

définie dans $\mathbf{R}^n$, par substitution de $x$ à chacun des $x_i$; la prop. 3 montre donc que $x^n$ est dérivable dans $\mathbf{R}$ et a pour dérivée $nx^{n-1}$. Il en résulte que la fonction polynôme $a_0 x^n + a_1 x^{n-1} + \cdots + a_{n-1} x + a_n$ (a_i vecteurs constants) a pour dérivée

$$
na_0 x^{n-1} + (n-1)a_1 x^{n-2} + \cdots + a_{n-1};
$$

lorsque les $a_i$ sont des nombres réels, cette fonction coïncide avec la dérivée d’une fonction polynôme définie en Algèbre (A, IV).

#### Exemple 3 {#fvr-i-s1-n3-exa-3 .statement}

Le produit scalaire euclidien $(\mathbf{x}| \mathbf{y})$ (TG, VI, p. 8) est une application bilinéaire (nécessairement continue) de $\mathbf{R}^n \times \mathbf{R}^n$ dans $\mathbf{R}$. Si $f$ et $g$ sont deux fonctions vectorielles à valeurs dans $\mathbf{R}^n$, dérivables au point $x_0$, la fonction numérique $x \mapsto (f(x) | g(x))$ a au point $x_0$ une dérivée égale à $(f'(x_0) | g(x_0)) + (f(x_0) | g'(x_0))$. On a un résultat analogue pour le produit scalaire hermitien dans $\mathbf{C}^n$, ce dernier espace étant considéré comme espace vectoriel sur $\mathbf{R}$.

Considérons en particulier le cas où la norme euclidienne $\|f(x)\|$ est constante, et par suite aussi $(f(x) | f(x)) = \|f(x)\|^2$; en écrivant que la dérivée de $(f(x) | f(x))$ est nulle au point $x_0$, il vient $(f(x_0) | f'(x_0)) = 0$, autrement dit, $f'(x_0)$ est un vecteur orthogonal à $f(x_0)$.

#### Exemple 4 {#fvr-i-s1-n3-exa-4 .statement}

Si $E$ est une algèbre topologique sur $\mathbf{R}$ (cf. Introduction), le produit $xy$ de deux éléments de $E$ est fonction bilinéaire continue de $(\mathbf{x}, \mathbf{y})$; si $f$ et $g$ prennent leurs valeurs dans $E$ et sont dérivables au point $x_0$, la fonction $x \mapsto f(x)g(x)$ admet au point $x_0$ une dérivée égale à $f'(x_0)g(x_0) + f(x_0)g'(x_0)$. En particulier, si $U(x) = (u_{ij}(x))$, $V(x) = (\beta_{ik}(x))$ sont deux matrices carrées d’ordre $n$, dérivables au point $x_0$, leur produit

UV admet en ce point une dérivée égale à la matrice $U'(x_0)V(x_0) + U(x_0)V'(x_0)$ (avec $U'(x) = (\alpha_{ij}'(x))$ et $V'(x) = (\beta_{ij}'(x))$).

#### Exemple 5 {#fvr-i-s1-n3-exa-5 .statement}

Le déterminant $\det(\mathbf{x}_1, \mathbf{x}_2, \ldots, \mathbf{x}_n)$ de $n$ vecteurs $\mathbf{x}_i = (x_{ij})_{1 \leq i \leq n}$ de l’espace $\mathbf{R}^n$ (A, III, p. 90) étant une fonction multilinéaire (continue) des $\mathbf{x}_i$, on voit que si les $n^2$ fonctions numériques $f_{ij}$ sont dérivables au point $x_0$, leur déterminant $g(x) = \det(f_{ij}(x))$ admet en ce point une dérivée égale à

$$
\sum_{i=1}^n [\mathbf{f}_1(x_0), \ldots, \mathbf{f}_{i-1}(x_0), \mathbf{f}_i'(x_0), \mathbf{f}_{i+1}(x_0), \ldots, \mathbf{f}_n(x_0)]
$$

où $\mathbf{f}_i(x) = (f_{ij}(x))_{1 \leq j \leq n}$; en d’autres termes, on obtient la dérivée d’un déterminant d’ordre $n$ en faisant la somme des $n$ déterminants qu’on obtient en remplaçant, pour chaque $i$, les termes de la colonne d’indice $i$ du déterminant donné par leurs dérivées.

#### Remarque {#fvr-i-s1-n3-rem-1 .statement}

Si $U(x)$ est une matrice carrée dérivable et inversible au point $x_0$, la dérivée de son déterminant $\Delta(x) = \det(U(x))$ s’exprime encore à l’aide de la dérivée de $U(x)$ par la formule

$$
\Delta'(x_0) = \Delta(x_0) \cdot \operatorname{Tr}(U'(x_0)U^{-1}(x_0)).
$$

En effet, posons $U(x_0 + h) = U(x_0) + hV; \ V$ tend par définition vers $U'(x_0)$ lorsque $h$ tend vers 0. On peut alors écrire

$$
\Delta(x_0 + h) = \Delta(x_0) \cdot \det(I + hVU^{-1}(x_0)).
$$

Or, $\det(I + hX) = 1 + h \operatorname{Tr}(X) + \sum_{k=2}^n \lambda_k h^k$, les $\lambda_k$ ($k \geq 2$) étant des polynômes par rapport aux éléments de la matrice $X$; comme les éléments de $VU^{-1}(x_0)$ ont une limite lorsque $h$ tend vers 0, on a bien la formule (3).

### 4. Dérivée de l’inverse d’une fonction

#### Proposition 4 {#fvr-i-s1-prop-4 .statement}

Soit $E$ une algèbre normée complète sur $\mathbf{R}$, ayant un élément unité et soit $\mathbf{f}$ une fonction définie dans un intervalle $I \subset \mathbf{R}$, prenant ses valeurs dans $E$, et dérivable au point $x_0 \in I$. Si $y_0 = \mathbf{f}(x_0)$ est inversible$^1$ dans $E$, la fonction $x \mapsto (\mathbf{f}(x))^{-1}$ est définie dans un voisinage de $x_0$ (par rapport à $I$) et admet au point $x_0$ une dérivée égale à $- (\mathbf{f}(x_0))^{-1}\mathbf{f}'(x_0)(\mathbf{f}(x_0))^{-1}$.

En effet, l’ensemble des éléments inversibles de $E$ est un ensemble ouvert où la fonction $y \mapsto y^{-1}$ est continue (TG, IX, p. 40); comme $\mathbf{f}$ est continue (par rapport à $I$) au point $x_0$, $(\mathbf{f}(x))^{-1}$ est définie dans un voisinage de $x_0$, et on a

$$
(\mathbf{f}(x))^{-1} - (\mathbf{f}(x_0))^{-1} = (\mathbf{f}(x))^{-1}(\mathbf{f}(x_0) - \mathbf{f}(x)) (\mathbf{f}(x_0))^{-1}.
$$

La proposition résulte donc de la continuité de $y^{-1}$ au voisinage de $y_0$, et de la continuité de $xy$ dans $E \times E$.

#### Exemple 1 {#fvr-i-s1-n4-exa-1 .statement}

Le cas particulier le plus important est celui où $E$ est l’un des corps $\mathbf{R}$ ou $\mathbf{C}$: si $f$ est une fonction à valeurs réelles ou complexes, dérivable au point $x_0$ et telle que $f(x_0) \neq 0$, $1/f$ admet au point $x_0$ une dérivée égale à $- f'(x_0)/(f(x_0))^2$.

1 On rappelle (A, I, p. 15) qu’un élément $z \in E$ est dit *inversible* s’il existe un élément de $E$, noté $z^{-1}$, tel que l’on ait $zz^{-1} = z^{-1}z = e$ (e élément unité de $E$).

#### Exemple 2 {#fvr-i-s1-n4-exa-2 .statement}

Si $U = (z_{ij}(x))$ est une matrice carrée d’ordre $n$, dérivable au point $x_0$ et inversible en ce point, $U^{-1}$ admet au point $x_0$ une dérivée égale à $-\ U^{-1}U'U^{-1}$.

### 5. Dérivée d’une fonction composée

#### Proposition 5 {#fvr-i-s1-prop-5 .statement}

Soient $f$ une fonction numérique définie dans un intervalle $I \subset \mathbf{R}$, et $g$ une fonction vectorielle définie dans un intervalle de $\mathbf{R}$ contenant $f(I)$. Si $f$ est dérivable au point $x_0$ et $g$ dérivable au point $f(x_0)$, la fonction composée $g \circ f$ admet au point $x_0$ une dérivée égale à $g'(f(x_0))f'(x_0)$.

En effet, posons $h = g \circ f$; on peut écrire, pour $x \neq x_0$,
$$
\frac{h(x) - h(x_0)}{x - x_0} = u(x) \frac{f(x) - f(x_0)}{x - x_0}
$$
où on pose $u(x) = \frac{g(f(x)) - g(f(x_0))}{f(x) - f(x_0)}$ si $f(x) \neq f(x_0)$, et $u(x) = g'(f(x_0))$ dans le cas contraire. Lorsque $x$ tend vers $x_0$, $f(x)$ a pour limite $f(x_0)$, donc $u(x)$ a pour limite $g'(f(x_0))$, d’où la proposition en vertu de la continuité de la fonction $yx$ dans $\mathbf{E} \times \mathbf{R}$.

### 6. Dérivée d’une fonction réciproque

#### Proposition 6 {#fvr-i-s1-prop-6 .statement}

Soit $f$ un homéomorphisme d’un intervalle $I \subset \mathbf{R}$ sur un intervalle $J = f(I) \subset \mathbf{R}$, et soit $g$ l’homéomorphisme réciproque.\footnote{Pour que $f$ soit un homéomorphisme de $I$ sur une partie de $\mathbf{R}$, on sait qu’il faut et il suffit que $f$ soit continue et strictement monotone dans $I$ (TG, IV, p. 9, th. 5).} Si $f$ est dérivable au point $x_0 \in I$, et si $f'(x_0) \neq 0$, $g$ admet au point $y_0 = f(x_0)$ une dérivée égale à $1/f'(x_0)$.

En effet, pour tout $y \in J$, on a $g(y) \in I$ et $u = f(g(y))$; on peut donc écrire, pour $y \neq y_0$,
$$
\frac{g(y) - g(y_0)}{y - y_0} = \frac{g(y) - x_0}{f(g(y)) - f(x_0)}
$$
et $\neq y_0$, $g(y)$ tend vers $x_0$ en restant dans $I$ et $\neq x_0$, et le second membre de la formule précédente a donc une limite égale à $1/f'(x_0)$, puisque par hypothèse $f'(x_0) \neq 0$.

#### Corollaire {#fvr-i-s1-n6-cor-1 .statement}

Si $f$ est dérivable dans $I$ et si $f'(x) \neq 0$ dans $I$, $g$ est dérivable dans $J$ et sa dérivée en tout point $y \in J$ est égale à $1/f'(g(y))$.

Par exemple, pour tout entier $n > 0$, la fonction $x^{1/n}$, homéomorphisme de $\mathbf{R}_+$ sur lui-même, réciproque de $x^n$, a pour dérivée en tout point $x > 0$, $\frac{1}{n} x^{\frac{1}{n}-1}$.

On en déduit aisément, d’après la prop. 5, que, pour tout nombre rationnel $r = p/q > 0$, la fonction $x^r = (x^{1/q})^p$ a pour dérivée $rx^{r-1}$ en tout point $x > 0$.

#### Remarque 1 {#fvr-i-s1-n6-rem-1 .statement}

Toutes les propositions qui précèdent, énoncées pour des fonctions dérivables en un point $x_0$, donnent aussitôt des propositions pour des fonctions dérivables à droite (resp. à gauche) en $x_0$, en considérant au lieu de ces fonctions, leurs restrictions à l’intersection de l’intervalle où sont définies ces fonctions et de l’intervalle $(x_0, +\infty]$ (resp.$]-\infty, x_0]$); nous laissons au lecteur le soin de les énoncer.

#### Remarque 2 {#fvr-i-s1-n6-rem-2 .statement}

Les définitions et propositions qui précèdent (à l’exception de ce qui concerne les dérivées à droite et dérivées à gauche) s’étendent aisément au cas où on remplace $\mathbf{R}$ par un corps topologique commutatif quelconque $K$, et les espaces vectoriels topologiques (resp. algèbres topologiques) sur $K$. Dans la déf. 1 et les prop. 1, 2 et 3, il suffit de remplacer $I$ par un voisinage de $x_0$ dans $K$; dans la prop. 4, il faut supposer de plus que l’application $y \mapsto y^{-1}$ est définie et continue dans un voisinage de $f(x_0)$ dans $E$. La prop. 5 se généralise de la façon suivante: soient $K'$ un sous-corps du corps topologique $K$, $E$ un espace vectoriel topologique sur $K$; soit $f$ une fonction définie dans un voisinage $V \subset K'$ de $x_0 \in K'$, à valeurs dans $K$ (considéré comme espace vectoriel topologique sur $K'$), dérivable au point $x_0$, et soit $g$ une fonction définie dans un voisinage de $f(x_0) \in K$, à valeurs dans $E$, et dérivable au point $f(x_0)$; alors l’application $g \circ f$ est dérivable au point $x_0$ et a une dérivée en ce point égale à $g'(f(x_0))f'(x_0)$ ($E$ étant alors considéré comme espace vectoriel topologique sur $K'$).

Avec les mêmes notations, soit $f$ une fonction définie dans un voisinage $V$ de $a \in K$, à valeurs dans $E$, et dérivable au point $a$; si $a \in K'$ et n’est pas point isolé dans $K'$, la restriction de $f$ à $V \cap K'$ est dérivable au point $a$, et a pour dérivée $f'(a)$ en ce point. Ces considérations s’appliqueront surtout, en pratique, au cas où $K = \mathbf{C}$ et $K' = \mathbf{R}$.

Enfin, la prop. 6 s’étend au cas où on remplace $I$ par un voisinage de $x_0 \in K$, et $f$ par un homéomorphisme de $I$ sur un voisinage $J = f(I)$ de $y_0 = f(x_0)$ dans $K$.

### 7. Dérivées des fonctions numériques

Les définitions et propositions qui précèdent se complètent sur quelques points lorsqu’il s’agit de fonctions numériques (finies) d’une variable réelle.

Tout d’abord, si $f$ est une telle fonction, définie dans un intervalle $I \subset \mathbf{R}$, et continue par rapport à $I$ en un point $x_0 \in I$, il peut se faire, lorsque $x$ tend vers $x_0$ en restant dans $I$ et $\neq x_0$, que $\frac{f(x) - f(x_0)}{x - x_0}$ ait une limite égale à $+\infty$ ou à $-\infty$; on dit alors encore que $f$ est dérivable au point $x_0$ et a pour dérivée en ce point $+\infty$ (resp. $-\infty$); si, en tout point $x$ de $I$, la fonction $f$ a une dérivée (finie ou infinie) $f'(x)$, la fonction $f'$ (à valeurs dans $\mathbf{R}$) est encore appelée la fonction dérivée (ou simplement la dérivée) de $f$. On généralise de même les définitions de la dérivée à droite et de la dérivée à gauche.

#### Exemple {#fvr-i-s1-n7-exa-1 .statement}

Au point $x = 0$, la fonction $x^{1/2}$ (fonction réciproque de $x^3$, homéomorphisme de $\mathbf{R}$ sur lui-même) admet une dérivée égale à $+\infty$; la fonction $|x|^{1/2}$ admet au point $x = 0$ une dérivée à droite égale à $+\infty$ et une dérivée à gauche égale à $-\infty$.

Les formules donnant la dérivée d’une somme, d’un produit de fonctions numériques dérivables, ou de l’inverse d’une fonction dérivable (prop. 1, 3 et 4) ainsi que la dérivée d’une fonction (numérique) composée (prop. 5) sont encore valables lorsque les dérivées qui y figurent sont infinies, pourvu que toutes les expressions intervenant dans ces formules aient un sens (TG, IV, p. 15–16). Enfin, dans la prop. 6, si on suppose que $f$ est strictement croissante (resp. strictement décroissante) et continue dans $I$, et si $f'(x_0) = 0$, la fonction réciproque $g$ admet au point $y_0 = f(x_0)$ une dérivée égale à $+\infty$ (resp. $-\infty$); si $f'(x_0) = +\infty$ (resp. $-\infty$), $g$ admet une dérivée égale à 0. On a des résultats analogues pour les dérivées à droite et dérivées à gauche, que nous laissons au lecteur le soin d’énoncer.

Soit $C$ le graphe ou courbe représentative d’une fonction numérique finie $f$, partie du plan $\mathbf{R}^2$ formée des points $(x, f(x))$ où $x$ parcourt l’ensemble où $f$ est définie. Si, en un point $x_0 \in I$, la fonction $f$ a une dérivée à droite finie, la demi-droite ayant comme origine le point $M_{x_0} = (x_0, f(x_0))$ de $C$, et pour paramètres directeurs $(1, f'_d(x_0))$ est appelée demi-tangente à droite à la courbe $C$ au point $M_{x_0}$; lorsque $f'_d(x_0) = +\infty$ (resp. $f'_d(x_0) = -\infty$), on appelle encore ainsi la demi-droite d’origine $M_{x_0}$ et de paramètres $(0, 1)$ (resp. $(0, -1)$). On définit de même la demi-tangente à gauche au point $M_{x_0}$, lorsque $f'_g(x_0)$ existe. Avec ces définitions, on vérifie aussitôt que l’angle que fait la demi-tangente à droite (resp. à gauche) avec l’axe des abscisses, est la limite de l’angle que fait avec cet axe la demi-droite d’origine $M_{x_0}$ passant par le point $M_x = (x, f(x))$ de $C$, lorsque $x$ tend vers $x_0$ en restant $> x_0$ (resp. $< x_0$).

On peut dire aussi que la demi-tangente à droite (resp. à gauche) est la limite de la demi-droite d’origine $M_{x_0}$ passant par $M_x$, en considérant sur l’ensemble des demi-droites de même origine, la topologie de l’espace quotient $\mathbf{C}^*/\mathbf{R}^*_+$ (TG, VIII, p. 9).

Si les deux demi-tangententes en un point $M_{x_0}$ de $C$ existent, elles ne sont opposées que lorsque $f$ a une dérivée (finie ou non) au point $x_0$ (supposé intérieur à $I$); elles ne sont identiques que lorsque $f'_d(x_0)$ et $f'_g(x_0)$ sont infinies et de signes contraires. Dans les deux cas, on dit que la droite qui contient les deux demi-tangententes est la tangente à $C$ au point $M_{x_0}$.

Lorsque la tangente en $M_{x_0}$ existe, elle est la limite de la droite passant par $M_{x_0}$ et $M_x$, lorsque $x$ tend vers $x_0$ en restant $\neq x_0$, la topologie sur l’ensemble des droites passant par un même point étant celle de l’espace quotient $\mathbf{C}^*/\mathbf{R}^*$ (TG, VIII, p. 15).

Les notions de tangente et de demi-tangente à une courbe représentative sont des cas particuliers de notions générales qui seront définies dans la partie de ce Traité consacrée aux variétés différentielles.

#### Définition 4 {#fvr-i-s1-def-4 .statement}

On dit qu’une fonction numérique finie $f$, définie dans une partie $A$ d’un espace topologique $E$, admet un maximum relatif (resp. maximum relatif strict, minimum relatif, minimum relatif strict) en un point $x_0 \in A$, par rapport à $A$, s’il existe un voisinage $V$ de $x_0$ dans $E$ tel qu’en tout point $x \in V \cap A$ différent de $x_0$, on ait $f(x) \leqslant f(x_0)$ (resp. $f(x) < f(x_0)$, $f(x) \geqslant f(x_0)$, $f(x) > f(x_0)$).

Il est clair que si $f$ atteint sa borne supérieure (resp. inférieure) dans $A$ en un point de $A$, elle a un maximum relatif (resp. minimum relatif) par rapport à $A$ en ce point; la réciproque est bien entendu inexacte.

On notera que si $B \subset A$, et si $f$ admet (par exemple) un maximum relatif en un point $x_0 \in B$, par rapport à $B$, $f$ n’admet pas nécessairement un maximum relatif par rapport à $A$ en ce point.

#### Proposition 7 {#fvr-i-s1-prop-7 .statement}

Soit $f$ une fonction numérique finie, définie dans un intervalle $I \subset \mathbf{R}$. Si, en un point $x_0$, intérieur à $I$, $f$ admet un maximum relatif (resp. un minimum relatif) et a en ce point une dérivée à droite et une dérivée à gauche, on a $f'_d(x_0) \leqslant 0$ et $f'_g(x_0) \geqslant 0$ (resp. $f'_d(x_0) \geqslant 0$ et $f'_g(x_0) \leqslant 0$) ; en particulier, si $f$ est dérivable au point $x_0$, on a $f'(x_0) = 0$.

La proposition résulte trivialement des définitions.

On peut dire encore que si en un point $x_0$ intérieur à $I$ la fonction $f$ est dérivable et admet un maximum ou minimum relatif, la tangente à sa courbe représentative est parallèle à l’axe des abscisses. La réciproque est inexacte, comme le montre l’exemple de la fonction $x^3$ qui a une dérivée nulle au point $x = 0$, mais n’a ni maximum ni minimum relatif en ce point.

## EXERCICES {#fvr-i-s1-exercises}

See the [exercises for § 1](exercises/s1/).
