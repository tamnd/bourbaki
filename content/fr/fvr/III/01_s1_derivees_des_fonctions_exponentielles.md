---
book: fvr
book_title: Functions of a Real Variable
chapter: III
chapter_title: FONCTIONS ÉLÉMENTAIRES
section: 1
section_title: Dérivées des fonctions exponentielles et circulaires
lang: fr
source: fvr-i-vii-fr
pdf_pages: 0091-0105, 0114-0122
extraction: ocr
subsections:
    - "no": 1
      title: Dérivées des fonctions exponentielles; nombre $e$
      page: 0
      pdf_page: 91
    - "no": 2
      title: Dérivée de $\log_a x$
      page: 3
      pdf_page: 93
    - "no": 3
      title: '*Dérivées des fonctions circulaires; nombre $\pi$*'
      page: 4
      pdf_page: 94
    - "no": 4
      title: Fonctions circulaires réciproques
      page: 5
      pdf_page: 95
    - "no": 5
      title: L’exponentielle complexe
      page: 7
      pdf_page: 97
    - "no": 6
      title: Propriétés de la fonction $e^z$
      page: 8
      pdf_page: 98
    - "no": 7
      title: Le logarithme complexe
      page: 10
      pdf_page: 100
    - "no": 8
      title: Primitives des fonctions rationnelles
      page: 11
      pdf_page: 101
    - "no": 9
      title: Fonctions circulaires complexes; fonctions hyperboliques
      page: 12
      pdf_page: 102
statements: 8
exercises: 39
content_sha256: cde00cf088adb1d7eca07f0a2802d72337590cbaacfcf3b7045c3411500b70b7
---

## § 1. DÉRIVÉES DES FONCTIONS EXPONENTIELLES ET CIRCULAIRES

### 1. Dérivées des fonctions exponentielles; nombre $e$

On sait que tout homomorphisme continu du groupe additif $\mathbf{R}$ dans le groupe multiplicatif $\mathbf{R}^*$ des nombres réels $\neq 0$ est une fonction de la forme $x \mapsto a^x$ (dite *fonction exponentielle*) où $a$ est un nombre $> 0$ (TG, V, p. 11); c’est un isomorphisme de $\mathbf{R}$ sur le groupe multiplicatif $\mathbf{R}_+^*$ des nombres $> 0$ si $a \neq 1$, et l’isomorphisme réciproque de $\mathbf{R}_+^*$ sur $\mathbf{R}$ se note $\log_a x$ et est appelé *logarithme de base* $a$.

Nous allons voir que la fonction $f(x) = a^x$ a pour tout $x \in \mathbf{R}$ une dérivée de la forme $e \cdot a^x$ (où on a évidemment $e = f'(0)$). Cela résulte du théorème général suivant:

#### Théorème 1 {#fvr-iii-s1-thm-1 .statement}

*Soit E une algèbre normée complète sur le corps $\mathbf{R}$, ayant un élément unité $e$, et soit $\mathbf{f}$ un homomorphisme continu du groupe additif $\mathbf{R}$ dans le groupe multiplicatif $G$ des éléments inversibles de $E$. L’application $\mathbf{f}$ est dérivable en tout point $x \in \mathbf{R}$, et on a*

$$
\mathbf{f}'(x) = \mathbf{f}(x)\mathbf{f}'(0).
$$

Remarquons d’abord que, $E$ étant une algèbre complète, $G$ est *ouvert* dans $E$ (TG, IX, p. 40, prop. 14). Considérons la fonction $g(x) = \int_0^a \mathbf{f}(x + t) \, dt$, où $a > 0$ est un nombre que nous préciserons plus loin; comme $\mathbf{f}(x + t) = \mathbf{f}(x)\mathbf{f}(t)$ par hypothèse, on a $g(x) = \int_0^a \mathbf{f}(x)\mathbf{f}(t) \, dt = \mathbf{f}(x) \int_0^a \mathbf{f}(t) \, dt$ (I, p. 14, prop. 3). Soit $\alpha > 0$ tel que la boule $\|x - e\| \leq \alpha$ soit contenue dans $G$; comme $\mathbf{f}(0) = e$ et que $\mathbf{f}$ est continue par hypothèse, on peut supposer que $a$ est pris assez petit pour que $\|\mathbf{f}(t) - e\| \leq \alpha$ dans $(0, a)$; par suite (II, p. 12, formule (16)), on a

$$
\left\| \frac{1}{a} \int_0^a \mathbf{f}(t) \, dt - e \right\| \leq \alpha,
$$

et $\frac{1}{a} \int_0^a f(t) \, dt$ appartient à G, autrement dit est inversible; il en est de même de $b = \int_0^a f(t) \, dt$, et on peut écrire $f(x) = g(x)b^{-1}$; il suffit donc de prouver que $g(x)$ est dérivable; or, par le changement de variable $x + t = u$, on a $g(x) = \int_x^{x+a} f(u) \, du$; comme $f$ est continue, $g$ est dérivable pour tout $x \in \mathbf{R}$ (II, p. 6, prop. 3), et on a
$$
g'(x) = f(x + a) - f(x) = f(x)(f(a) - e).
$$
D’où $f'(x) = g'(x)b^{-1} = f(x)c$, où $c = (f(a) - e)b^{-1}$, et on a évidemment $f'(0) = c$.

Réciproquement, on peut démontrer, soit directement (III, p. 24, exerc. 1), soit à l’aide de la théorie des équations différentielles linéaires (IV, p. 29) que toute application dérivable $f$ de $\mathbf{R}$ dans une algèbre normée complète E, telle que $f'(x) = f(x)c$ et $f(0) = e$, est un homomorphisme du groupe additif $\mathbf{R}$ dans le groupe multiplicatif G.

#### Proposition 1 {#fvr-iii-s1-prop-1 .statement}

Pour tout nombre $a > 0$ et $\neq 1$, la fonction exponentielle $a^x$ admet en tout point $x \in \mathbf{R}$ une dérivée égale à $(\log_e a)a^x$ où $e$ est un nombre $> 1$ (indépendant de $a$).

L’application du th. 1 au cas où E est le corps $\mathbf{R}$ lui-même montre en effet que $a^x$ admet en tout point une dérivée égale à $\varphi(a).a^x$, où $\varphi(a)$ est un nombre réel $\neq 0$ ne dépendant que de $a$. Soit $b$ un second nombre $> 0$ et $\neq 1$; la fonction $b^x$ a une dérivée égale à $\varphi(b).b^x$ d’après ce qui précède; d’autre part, on a $b^x = a^{x.\log_a b}$ donc (I, p. 17, prop. 5), la dérivée de $b^x$ est égale à $\log_a b . \varphi(a)b^x$; par comparaison des deux expressions obtenues, il vient
$$
\varphi(b) = \varphi(a) . \log_a b.
$$
On en déduit qu’il existe un nombre $b$ et un seul tel que $\varphi(b) = 1$; en effet, cette relation équivaut, d’après (2), à $b = a^{1/\varphi(a)}$. Il est d’usage de désigner par $e$ le nombre réel ainsi déterminé; d’après (2), on a $\varphi(a) = \log_e a$, ce qui achève de démontrer la prop. 1.

On écrira souvent $\exp x$ au lieu de $e^x$.

La définition du nombre $e$ montre qu’on a
$$
\mathrm{D}(e^x) = e^x
$$
ce qui prouve que $e^x$ est strictement croissante, et par suite que $e > 1$.

Au § 2 (III, p. 15), nous verrons comment on peut calculer des valeurs aussi approchées qu’on veut du nombre $e$.

DéFINITION 1. — Les logarithmes de base $e$ sont appelés logarithmes népériens (ou logarithmes naturels).

On convient d’ordinaire d’omettre la base dans la notation d’un logarithme népérien. Sauf mention expresse du contraire, la notation $\log x$ ($x > 0$) désignera donc le logarithme népérien de x. Avec cette notation, la prop. 1 s’exprime par l’identité
(4) $D(a^x) = (\log a)a^x$
valable pour $a$ quelconque $> 0$ (puisque pour $a = 1, \log a = 0$).
Cette relation montre que $a^x$ a des dérivées de tout ordre, et qu’on a
(5) $D^n(a^x) = (\log a)^n a^x.$

En particulier, pour tout $a > 0$ et $\neq 1$, on a $D^2(a^x) > 0$ pour tout $x \in \mathbf{R}$, et par suite $a^x$ est strictement convexe dans $\mathbf{R}$ (I, p. 39, corollaire). On en déduit la proposition suivante:

**Proposition 2** (« inégalité de la moyenne géométrique »). — *Quels que soient les nombres* $z_i > 0$ ($1 \leq i \leq n$) *et les nombres* $p_i > 0$ *tels que* $\sum_{i=1}^n p_i = 1$, *on a*
(6) $z_1^{p_1}z_2^{p_2}\ldots z_n^{p_n} \leq p_1z_1 + p_2z_2 + \cdots + p_nz_n.$
*En outre les deux membres de* (6) *ne sont égaux que si tous les* $z_i$ *sont égaux*.

En effet, posons $z_i = e^{x_i}$; l’inégalité (6) s’écrit
(7) $\exp(p_1x_1 + p_2x_2 + \cdots + p_nx_n) \leq p_1e^{x_1} + p_2e^{x_2} + \cdots + p_ne^{x_n}.$
La proposition résulte alors de la prop. 1 de I, p. 34, appliquée à la fonction $e^x$, strictement convexe dans $\mathbf{R}$.

On dit que le premier membre (resp. le second membre) de (6) est la *moyenne géométrique pondérée* (resp. la *moyenne arithmétique pondérée*) des $n$ nombres $z_i$, relatives aux *poids* $p_i$ ($1 \leq i \leq n$). Si $p_i = 1/n$ pour $1 \leq i \leq n$, on dit que les moyennes arithmétique et géométrique correspondantes sont les moyennes arithmétique et géométrique *ordinaires* des $z_i$. L’inégalité (6) s’écrit alors
(8) $(z_1z_2\ldots z_n)^{1/n} \leq \frac{1}{n}(z_1 + z_2 + \cdots + z_n).$

### 2. Dérivée de $\log_a x$

Comme $a^x$ est strictement monotone dans $\mathbf{R}$ pour $a \neq 1$, l’application de la formule de dérivation des fonctions réciproques (I, p. 17, prop. 6) donne, pour tout $x > 0$
(9) $D(\log_a x) = \frac{1}{x \log a}$
et en particulier
(10) $D(\log x) = \frac{1}{x}$

Si $u$ est une fonction numérique admettant une dérivée au point $x_0$, et telle que $u(x_0) > 0$, la fonction $\log u$ admet au point $x_0$ une dérivée égale à $u'(x_0)/u(x_0)$. En particulier, on a $D(\log |x|) = 1/|x| = 1/x$ si $x > 0$, et

$$
D(\log |x|) = - \frac{1}{|x|} = \frac{1}{x}
$$

si $x < 0$; autrement dit, on a $D(\log |x|) = 1/x$ quel que soit $x \neq 0$. On en conclut que si, dans un intervalle $I$, la fonction numérique $u$ n’est pas nulle et admet une dérivée finie, $\log |u(x)|$ admet dans $I$ une dérivée égale à $u'/u$; cette dérivée est dite *dérivée logarithmique* de $u$. Il est clair que la dérivée logarithmique de $|u|^a$ est $au'/u$, et que la dérivée logarithmique d’un produit est égale à la somme des dérivées logarithmiques des facteurs; l’application de ces règles permet souvent de calculer plus rapidement la dérivée d’une fonction. Elles redonnent en particulier la formule

(II)
$$
D(x^\alpha) = \alpha x^{\alpha-1} \quad (\alpha \text{ réel quelconque, } x > 0)
$$
déjà démontrée par une autre voie (II, p. 19).

#### Exemple {#fvr-iii-s1-n2-exa-1 .statement}

Si $u$ est une fonction $\neq 0$ dans un intervalle $I$, $v$ une fonction numérique quelconque, on a $\log(|u|^v) = v \log |u|$, donc si $u$ et $v$ sont dérivables
$$
\frac{1}{|u|^v} D(|u|^v) = v' \log |u| + v \frac{u'}{u}.
$$

### 3. *Dérivées des fonctions circulaires; nombre $\pi$*

On a défini, en Topologie générale (TG, VIII, p. 8) l’homomorphisme continu $x \mapsto \mathbf{e}(x)$ du groupe additif $\mathbf{R}$ sur le groupe multiplicatif $\mathbf{U}$ des nombres complexes de valeur absolue 1; c’est une fonction périodique de période principale 1, et on a $\mathbf{e}(\frac{1}{4}) = i$. On sait (*loc. cit.*) que tout homomorphisme continu de $\mathbf{R}$ sur $\mathbf{U}$ est de la forme $x \mapsto \mathbf{e}(x/a)$, et qu’on pose $\cos_a x = \Re(\mathbf{e}(x/a))$, $\sin_a x = \Im(\mathbf{e}(x/a))$ (*fonctions trigonométriques*, ou *fonctions circulaires*, de base $a$); ces dernières fonctions sont des applications continues de $\mathbf{R}$ dans $[-1, +1]$, admettant $a$ pour période principale. On a $\sin_a(x + a/4) = \cos_a x$, $\cos_a(x + a/4) = -\sin_a x$, et la fonction $\sin_a x$ est croissante dans l’intervalle $[-a/4, a/4]$.

#### Proposition 3 {#fvr-iii-s1-prop-3 .statement}

*La fonction $\mathbf{e}(x)$ admet en tout point de $\mathbf{R}$ une dérivée égale à $2\pi i \mathbf{e}(x)$, où $\pi$ est une constante $> 0$.*

En effet, le th. 1 de III, p. 1, appliqué au cas où $E$ est le corps $\mathbf{C}$ des nombres complexes, donne la relation $\mathbf{e}'(x) = \mathbf{e}'(0)\mathbf{e}(x)$; en outre, comme $\mathbf{e}(x)$ a une norme euclidienne constante, $\mathbf{e}'(x)$ est orthogonal à $\mathbf{e}(x)$ (I, p. 15, *Exemple 3*); on a donc $\mathbf{e}'(0) = \alpha i$, avec $\alpha$ réel. Comme $\sin_1 x$ est croissante dans $[-\frac{1}{4}, \frac{1}{4}]$, sa dérivée pour $x = 0$ est $\geqslant 0$, donc $\alpha \geqslant 0$, et comme $\mathbf{e}(x)$ n’est pas constante, $\alpha > 0$; il est d’usage de désigner le nombre $\alpha$ ainsi défini par la notation $2\pi$.

Nous montrerons au § 2 (III, p. 23) comment on peut calculer des valeurs aussi approchées qu’on veut du nombre $\pi$.

On a donc la formule

$$
\mathrm{D}\left(e^{\left(\frac{x}{a}\right)}\right) = \frac{2\pi i}{a} e^{\left(\frac{x}{a}\right)}.
$$

On voit que cette formule se simplifie lorsque $a = 2\pi$; c’est pourquoi on utilise exclusivement en Analyse les fonctions circulaires relatives à la base $2\pi$; on convient d’omettre la base dans la notation de ces fonctions; sauf mention expresse du contraire, les notations $\cos x$, $\sin x$ et $\tg x$ désigneront donc respectivement $\cos_{2\pi} x$, $\sin_{2\pi} x$ et $\tg_{2\pi} x$. Avec ces conventions, la formule (12), où on fait $a = 2\pi$, s’écrit

$$
\mathrm{D}(\cos x + i \sin x) = \cos \left(x + \frac{\pi}{2}\right) + i \sin \left(x + \frac{\pi}{2}\right),
$$

ce qui équivaut à

$$
\mathrm{D}(\cos x) = -\sin x, \quad \mathrm{D}(\sin x) = \cos x,
$$

d’où l’on tire

$$
\mathrm{D}(\tg x) = 1 + \tg^2 x = \frac{1}{\cos^2 x}.
$$

A côté des trois fonctions circulaires $\cos x$, $\sin x$ et $\tg x$, on emploie encore, dans la pratique du calcul numérique, les trois fonctions auxiliaires: cotangente, sécante et cosécante, définies par les formules

$$
\cotg x = \frac{1}{\tg x}, \quad \sec x = \frac{1}{\cos x}, \quad \cosec x = \frac{1}{\sin x}.
$$

Rappelons (TG, VIII, p. 10) que l’unité d’angle correspondant à la base $2\pi$ est appelée radian.

### 4. Fonctions circulaires réciproques

La restriction de la fonction $\sin x$ à l’intervalle $(-\pi/2, +\pi/2)$ est strictement croissante; on désigne par $\mathrm{Arc} \sin x$ sa fonction réciproque, qui est donc une application strictement croissante et continue de l’intervalle $(-1, +1)$ sur $(-\pi/2, +\pi/2)$ (fig. 6). La formule de dérivation des fonctions réciproques (I, p. 17, prop. 6) donne la dérivée de cette fonction

$$
\mathrm{D}(\mathrm{Arc} \sin x) = \frac{1}{\cos (\mathrm{Arc} \sin x)}.
$$

Comme $-\pi/2 \leq \mathrm{Arc} \sin x \leq \pi/2$, on a $\cos (\mathrm{Arc} \sin x) \geq 0$, et comme

$$
\sin (\mathrm{Arc} \sin x) = x,
$$

on a cos (Arc sin x) = $\sqrt{1 - x^2}$, d’où

(16) $$
\mathrm{D}(\mathrm{Arc}\,\sin\,x) = \frac{1}{\sqrt{1 - x^2}}.
$$

De même, la restriction de cos $x$ à l’intervalle $[0, \pi]$ est strictement décroissante; on désigne par Arc cos $x$ sa fonction réciproque, qui est une application strictement décroissante de $(-1, +-)$ sur $[0, \pi]$ (fig. 6). On a d’ailleurs

$$
\sin \left( \frac{\pi}{2} - \mathrm{Arc}\,\cos\,x \right) = \cos (\mathrm{Arc}\,\cos\,x) = x
$$

![Graph showing y = Arc cos x and y = Arc sin x](https://i.imgur.com/3Q5z5QG.png)

Fig. 6

et comme $-\pi/2 \leq \pi/2 - \mathrm{Arc}\,\cos\,x \leq \pi/2$, on a

(17) $$
\mathrm{Arc}\,\cos\,x = \frac{\pi}{2} - \mathrm{Arc}\,\sin\,x
$$

d’où résulte en particulier que

(18) $$
\mathrm{D}(\mathrm{Arc}\,\cos\,x) = -\frac{1}{\sqrt{1 - x^2}}.
$$

Enfin, la restriction de tg $x$ à l’intervalle $]-\pi/2, +\pi/2[$ est strictement croissante; on désigne par Arc tg x sa fonction réciproque, qui est une application strictement croissante de $\mathbf{R}$ sur ]$-\pi/2,\ +\pi/2[$ (fig. 7); on a

$$
\lim_{x \to -\infty} \operatorname{Arc}\tg x = -\frac{\pi}{2}, \quad \lim_{x \to +\infty} \operatorname{Arc}\tg x = \frac{\pi}{2}
$$

![Graph of y = Arc tg x](https://i.imgur.com/3Q5z5QG.png)

Fig. 7

et par application de la formule de dérivation des fonctions réciproques et de la formule (15) de III, p. 5, on a

(19)
$$
D(\operatorname{Arc}\tg x) = \frac{1}{1 + x^2}.
$$

### 5. L’exponentielle complexe

On a déterminé (TG, VIII, p. 8) tous les homomorphismes continus du groupe topologique (additif) $\mathbf{C}$ des nombres complexes sur le groupe topologique (multiplicatif) $\mathbf{C}^*$ des nombres complexes $\neq 0$; ce sont les applications

(20)
$$
x + iy \mapsto e^{\alpha x + \beta y} e^{(\gamma x + \delta y)}
$$
où $\alpha, \beta, \gamma, \delta$ sont quatre nombres réels assujettis à la seule condition $\alpha \delta - \beta \gamma \neq 0$. Proposons-nous de déterminer ceux de ces homomorphismes $z \mapsto f(z)$ qui sont *dérivables* dans $\mathbf{C}$. Remarquons d’abord qu’il suffit que $f$ soit dérivable au point $z = 0$; en effet pour tout point $z \in \mathbf{C}$, on a
$$
\frac{f(z + h) - f(z)}{h} = f(z) \frac{f(h) - 1}{h};
$$
si $f'(0)$ existe, il en est donc de même de $f'(z)$, et on a $f'(z) = af(z)$, avec $a = f'(0)$. D’autre part, si $g$ est un second homomorphisme dérivable, tel que $g'(z) = bg(z)$, on a $g(az/b) = f(z)$, car on constate aussitôt que le quotient $g(az/b)/f(z)$ admet partout une dérivée nulle et est égal à 1 pour $z = 0$; tous les homomorphismes dérivables sont donc de la forme $z \mapsto f(\lambda z)$, où $f$ est l’un d’entre eux (supposé exister), et $\lambda$ une constante (complexe) quelconque.

Cela étant, si $f$ est dérivable au point $z = 0$, chacune des applications $x \mapsto f(x)$, $y \mapsto f(iy)$ de $\mathbf{R}$ dans $\mathbf{C}$ est nécessairement dérivable au point $0$, la première ayant comme dérivée $f'(0)$, la seconde $if'(0)$. Or les dérivées des applications $x \mapsto e^{ax}e(\gamma x)$, $y \mapsto e^{by}e(\delta y)$ au point $0$ sont respectivement égales à $\alpha + 2\pi i \gamma$ et $\beta + 2\pi i \delta$, d’où les conditions $\beta = -2\pi \gamma$ et $\alpha = 2\pi \delta$; ces conditions sont en particulier remplies par l’homomorphisme $x + iy \mapsto e^x e(y/2\pi)$, que nous désignerons provisoirement par $f_0$. Nous allons maintenant montrer qu’effectivement $f_0$ est dérivable au point $z = 0$.

En effet, il est clair que $x \mapsto f_0(x)$ et $y \mapsto f_0(iy)$ ont des dérivées de tout ordre; en particulier, la formule de Taylor d’ordre 1 appliquée à ces fonctions montre que, pour tout $\varepsilon > 0$, il existe $r > 0$ tel que, si on pose
$$
f_0(x) = 1 + x + \varphi(x)x, \quad f_0(iy) = 1 + iy + \psi(y)y,
$$
les conditions $|x| \leq r, |y| \leq r$ entraînent $|\varphi(x)| \leq \varepsilon$ et $|\psi(y)| \leq \varepsilon$; cela étant, on a $f_0(x + iy) = f_0(x)f_0(iy) = 1 + (x + iy) + \theta(x, y)$, avec
$$
\theta(x, y) = (i + \varphi(x)\psi(y))xy + (1 + x)y\psi(y) + (1 + iy)x\varphi(x);
$$
pour $|z| \leq r$, on a $|x| \leq r$ et $|y| \leq r$, d’où
$$
|\theta(x, y)| \leq (1 + \varepsilon^2)|z|^2 + 2\varepsilon|z|(1 + |z|)
$$
ce qui prouve que le quotient $\frac{f_0(z) - 1 - z}{z}$ tend vers 0 avec $z$, c’est-à-dire que $f_0$ admet au point $z = 0$ une dérivée égale à 1. Alors, ce qui précède prouve que, pour tout $z \in \mathbf{C}$, on a
$$
\mathrm{D}(f_0(z)) = f_0(z).
$$
Cette propriété rapproche encore $f_0$ de la fonction $e^x$, qui est d’ailleurs la restriction de $f_0$ à l’axe réel; pour cette raison, on pose la définition suivante:

#### Définition 2 {#fvr-iii-s1-def-2 .statement}

On appelle exponentielle complexe l’homomorphisme $x + iy \mapsto e^x e(y/2\pi)$ de $\mathbf{C}$ sur $\mathbf{C}^*$; sa valeur pour un nombre complexe quelconque $z$ se note $e^z$ ou $\exp z$.

### 6. Propriétés de la fonction $e^z$

Le fait que $z \mapsto e^z$ est un homomorphisme de $\mathbf{C}$ dans $\mathbf{C}^*$ se traduit par les identités
$$
e^{z+z'} = e^z e^{z'}, \quad e^0 = 1, \quad e^{-z} = 1/e^z.
$$
On a par définition, pour tout $z = x + iy$
$$
e^{x+iy} = e^x (\cos y + i \sin y)
$$

et comme $e^x > 0$, on voit que $e^z$ a pour valeur absolue $e^x$, pour amplitude $y$ (modulo $2\pi$).

La déf. 2 (III, p. 8) donne en particulier
$$
e(x) = e^{2\pi i x}
$$
ce qui permet d’écrire les formules qui définissent $\cos x$ et $\sin x$ sous la forme
$$
\cos x = \frac{1}{2} (e^{ix} + e^{-ix}), \quad \sin x = \frac{1}{2i} (e^{ix} - e^{-ix})
$$
(formules d’Euler).

Comme $2\pi$ est période principale de $e(y/2\pi)$, $2\pi i$ est période principale de $e^z$; autrement dit, le groupe des périodes de $e^z$ est l’ensemble des nombres $2n\pi i$, où $n$ parcourt $\mathbf{Z}$.

Enfin, la formule (21) de III, p. 8 s’écrit
$$
D(e^z) = e^z
$$
d’où, pour tout nombre complexe $a$
$$
D(e^{az}) = ae^{az}.
$$

#### Remarque {#fvr-iii-s1-n6-rem-1 .statement}

Si, dans la formule (27), on restreint la fonction $e^{ax}$ (a complexe) à l’axe réel, on obtient encore, pour $x$ réel
$$
D(e^{ax}) = ae^{ax}.
$$

Cette formule permet de calculer une primitive de chacune des fonctions $e^{ax} \cos \beta x, e^{ax} \sin \beta x$ ($\alpha$ et $\beta$ réels); en effet, on a $e^{(\alpha + i\beta)x} = e^{ax} \cos \beta x + i e^{ax} \sin \beta x$, donc, d’après (28)
$$
D\left( \Re \left( \frac{1}{\alpha + i\beta} e^{(\alpha + i\beta)x} \right) \right) = e^{ax} \cos \beta x,
$$
$$
D\left( \Im \left( \frac{1}{\alpha + i\beta} e^{(\alpha + i\beta)x} \right) \right) = e^{ax} \sin \beta x.
$$

De la même manière, on ramène le calcul d’une primitive de $x^n e^{ax} \cos \beta x$, ou de $x^n e^{ax} \sin \beta x$ ($n$ entier $> 0$) à celui d’une primitive de $x^n e^{(\alpha + i\beta)x}$; or, la formule d’intégration par parties d’ordre $n + 1$ (II, p. 10, formule (11)) montre qu’une primitive de cette dernière fonction est
$$
e^{(\alpha + i\beta)x} \left[ \frac{x^n}{\alpha + i\beta} - \frac{n x^{n-1}}{(\alpha + i\beta)^2} + \frac{n(n-1)x^{n-2}}{(\alpha + i\beta)^3} + \ldots + (-1)^n \frac{n!}{(\alpha + i\beta)^{n+1}} \right].
$$

En vertu des formules d’Euler, on peut d’autre part exprimer toute puissance entière positive de $\cos x$ ou de $\sin x$ comme combinaison linéaire d’exponentielles $e^{px}$ ($p$ entier positif ou négatif). D’après la formule (28), on pourra donc exprimer par une combinaison linéaire de fonctions de la forme $x^n e^{ax} \cos \lambda x$ et $x^n e^{ax} \sin \mu x$, une primitive d’une fonction de la forme $x^n e^{ax} (\cos \beta x)^r (\sin \gamma x)^s$ ($n, p, r, s$ entiers, $\alpha, \beta, \gamma, \lambda, \mu$ réels).

#### Exemple {#fvr-iii-s1-n6-exa-1 .statement}

On a
$$
\sin^{2n} x = \frac{(-1)^n}{2^{2n}} (e^{ix} - e^{-ix})^{2n} = \frac{(-1)^n}{2^{2n}} \left( e^{2nix} - \binom{2n}{1} e^{(2n-2)ix} + \ldots + e^{-2nix} \right)
$$

d’où
$$
\int_0^x \sin^{2n} t \, dt = \frac{(-1)^n}{2^{2n}} \left( \frac{1}{n} \sin 2nx - \binom{2n}{1} \frac{1}{n-1} \sin (2n-2)x + \ldots \right.
$$
$$
\left. + (-1)^{n-1} \binom{2n}{n-1} \sin 2x + (-1)^n \binom{2n}{n} x \right)
$$
et en particulier
$$
\int_0^{\pi/2} \sin^{2n} t \, dt = \binom{2n}{n} \frac{1}{2^{2n}} \frac{\pi}{2} = \frac{1.3.5\ldots(2n-1)}{2.4.6\ldots2n} \frac{\pi}{2}.
$$

### 7. Le logarithme complexe

Soit B la « bande » formée des points $z = x + iy$ tels que $-\pi \leq y < \pi$; la fonction $e^z$ prend chacune de ses valeurs une fois et une seule dans B; autrement dit, $z \mapsto e^z$ est une application bijective et continue de B sur $\mathbf{C}^*$; l’image par cette application du segment (semi-ouvert) $x = x_0, -\pi \leq y < \pi$ est le cercle $|z| = e^{x_0}$; l’image de la droite $y = y_0$ est la demi-droite (ouverte) définie par $\mathrm{Am}(z) = y_0$ (mod. $2\pi$). L’image par $z \mapsto e^z$ de l’intérieur $\dot{B}$ de B, c’est-à-dire de l’ensemble des $z \in \mathbf{C}$ tels que $|\mathcal{I}(z)| < \pi$, est le complémentaire F du demi-axe réel négatif (fermé) dans $\mathbf{C}$; si on convient de désigner par $\mathrm{Am}(z)$ la mesure de l’amplitude de z qui appartient à $]-\pi, +\pi[$, l’ensemble F peut encore être défini par les relations $-\pi < \mathrm{Am}(z) < \pi$. Comme $z \mapsto e^z$ est un homomorphisme strict de $\mathbf{C}$ sur $\mathbf{C}^*$, l’image par cette application de tout ensemble ouvert dans $\dot{B}$ (donc dans $\mathbf{C}$) est un ensemble ouvert dans $\mathbf{C}^*$ (donc dans F); autrement dit, la restriction de $z \mapsto e^z$ à $\dot{B}$ est un homéomorphisme de $\dot{B}$ sur F. On désigne par $z \mapsto \log z$ l’homéomorphisme de F sur $\dot{B}$, réciproque du précédent; pour un nombre complexe $z \in F$, $\log z$ est appelé la détermination principale du logarithme de z. Si $z = x + iy$ et $\log z = u + iv$, on a $x + iy = e^{u+iv}$, d’où $e^u = |z|$, et comme $-\pi < v < \pi$, $v = \mathrm{Am}(z)$. D’ailleurs, on a $\operatorname{tg}\left(v + \pi/2\right) = -x/y$ si $y \neq 0$; on peut donc écrire
$$
\begin{cases}
u = \log |z| = \frac{1}{2} \log (x^2 + y^2) \\
v = \frac{\pi}{2} - \operatorname{Arc tg} \frac{x}{y} & \text{si } y > 0 \\
v = 0 & \text{si } y = 0 \\
v = -\frac{\pi}{2} - \operatorname{Arc tg} \frac{x}{y} & \text{si } y < 0.
\end{cases}
$$
Il est clair que $\log z$ est un prolongement à F de la fonction $\log x$ définie sur le demi-axe réel positif ouvert $\mathbf{R}_+^*$. Si $z, z'$ sont deux points de F tels que $zz'$ ne soit pas réel négatif, on a $\log (zz') = \log z + \log z' + 2\varepsilon \pi i$, où $\varepsilon = +1, -1$ ou 0 suivant les valeurs de $\mathrm{Am}(z)$ et $\mathrm{Am}(z')$.

On notera qu’aux points du demi-axe réel négatif, la fonction $\log z$ n’a pas de limité; de façon précise, si x tend vers $x_0 < 0$ et si y tend vers 0 en restant >0 (resp. <0), log z tend vers $\log |x_0| + \pi i$ (resp. $\log |x_0| - \pi i$); lorsque z tend vers 0, $|\log z|$ croît indéfiniment.

Nous verrons plus tard comment la théorie des fonctions analytiques permet de prolonger la fonction log z, et de définir le logarithme complexe dans toute sa généralité.

Comme log z est un homéomorphisme réciproque de $e^z$, la formule de dérivation des fonctions réciproques (I, p. 17, prop. 6) montre qu’en tout point $z \in \mathbf{F}$, log z est dérivable, et qu’on a

$$
\text{D}(\log z) = \frac{1}{e^{\log z}} = \frac{1}{z}
$$

formule qui généralise la formule (10) de III, p. 3.

### 8. Primitives des fonctions rationnelles

La formule (31) permet de calculer une primitive d’une fonction rationnelle quelconque $r(x)$ d’une variable réelle x, à coefficients réels ou complexes. En effet, on sait (A, VII, §2, No 2) qu’une telle fonction peut s’écrire (d’une seule manière) comme somme d’un nombre fini de termes, qui sont:

a) soit de la forme $ax^p$ ($p$ entier $\geqslant 0$, a nombre complexe);
b) soit de la forme $a/(x-b)^m$ ($m$ entier $> 0$, a et b nombres complexes).

Or, il est facile d’obtenir une primitive de chacun de ces termes:
a) une primitive de $ax^p$ est $a \frac{x^{p+1}}{p+1}$;
b) si $m > 1$, une primitive de $a/(x-b)^m$ est $\frac{a}{(1-m)(x-b)^{m-1}}$;
c) enfin, d’après les formules (10) (III, p. 3) et (31) (III, p. 11), une primitive de $\frac{a}{x-b}$ est $a \log |x-b|$ si b est réel, $a \log (x-b)$ si b est complexe. Dans ce dernier cas, si $b = p + iq$, on a d’ailleurs (III, p. 10, formules (30))

$$
\log (x-b) = \log \sqrt{(x-p)^2 + q^2} + i \operatorname{Arc tg} \frac{x-p}{q} \pm i \frac{\pi}{2}.
$$

Nous renvoyons à la partie de cet ouvrage consacrée au Calcul numérique, l’examen des méthodes les plus pratiques pour la détermination explicite d’une primitive d’une fonction rationnelle donnée explicitement.

On peut ramener au calcul d’une primitive d’une fonction rationnelle:
1° le calcul d’une primitive d’une fonction de la forme $r(e^{ax})$, r étant une fonction rationnelle, a un nombre réel; en effet, par le changement de variable $u = e^{ax}$, on est ramené à trouver une primitive de $r(u)/u$;

2° le calcul d’une primitive d’une fonction de la forme $f(\sin ax, \cos ax)$, où $f$ est une fonction rationnelle de deux variables et $a$ un nombre réel; par le changement de variable $u = \tg ax/2$, on est ramené à trouver une primitive de

$$
\frac{2}{1 + u^2} f \left( \frac{2u}{1 + u^2}, \frac{1 - u^2}{1 + u^2} \right).
$$

### 9. Fonctions circulaires complexes; fonctions hyperboliques

Les formules d’Euler (25) (III, p. 9) et la définition de $e^z$ pour tout $z$ complexe, permettent de prolonger à $\mathbf{C}$ les fonctions $\cos x$ et $\sin x$ définies dans $\mathbf{R}$, en posant, pour tout $z \in \mathbf{C}$

$$
\cos z = \frac{1}{2}(e^{iz} + e^{-iz}), \qquad \sin z = \frac{1}{2i}(e^{iz} - e^{-iz})
$$

(cf. III, p. 28, exerc. 19).

Ces fonctions sont périodiques de période principale $2\pi$; on a $\cos (z + \pi/2) = -\sin z, \sin (z + \pi/2) = \cos z$; on vérifie également les identités

$$
\begin{align*}
&\cos^2 z + \sin^2 z = 1 \\
&\cos (z + z') = \cos z \cos z' - \sin z \sin z' \\
&\sin (z + z') = \sin z \cos z' + \cos z \sin z'.
\end{align*}
$$

Plus généralement, toute identité algébrique entre fonctions circulaires de variables réelles est encore vraie lorsqu’on donne à ces variables des valeurs complexes quelconques (III, p. 27, exerc. 18).

On pose $\tg z = \sin z/\cos z$ si $z \neq (2k + 1)\pi/2$ et $\cotg z = \cos z/\sin z$ si $x \neq k\pi$; ce sont des fonctions périodiques de période principale $\pi$.

La formule (27) (III, p. 9) montre que $\cos z$ et $\sin z$ sont dérivables dans $\mathbf{C}$, et que l’on a

$$
D(\cos z) = -\sin z, \qquad D(\sin z) = \cos z.
$$

Pour $z = ix$ ($x$ réel), les formules (32) donnent

$$
\cos ix = \frac{1}{2}(e^x + e^{-x}), \qquad \sin ix = \frac{i}{2}(e^x - e^{-x}).
$$

Il est commode de désigner par une notation particulière les fonctions réelles qui s’introduisent ainsi; on pose

$$
\begin{cases}
\ch x = \frac{1}{2}(e^x + e^{-x}) & \text{(cosinus hyperbolique de } x \text{)} \\
\sh x = \frac{1}{2}(e^x - e^{-x}) & \text{(sinus hyperbolique de } x \text{)} \\
\th x = \frac{\sh x}{\ch x} = \frac{e^x - e^{-x}}{e^x + e^{-x}} & \text{(tangente hyperbolique de } x \text{).}
\end{cases}
$$

On a donc, pour tout $x$ réel
$$(34)$$
$$ \cos ix = \operatorname{ch} x, \quad \sin ix = i \operatorname{sh} x. $$

De toute identité entre fonctions circulaires d’un certain nombre de variables complexes $z_k$ ($1 \leq k \leq n$) on déduit une identité entre fonctions hyperboliques, en remplaçant partout $z_k$ par $ix_k$ ($x_k$ réel, $1 \leq k \leq n$) et utilisant les formules (34); par exemple on a
$$
\begin{align*}
&\operatorname{ch}^2 x - \operatorname{sh}^2 x = 1 \\
&\operatorname{ch}(x + x') = \operatorname{ch} x \operatorname{ch} x' + \operatorname{sh} x \operatorname{sh} x' \\
&\operatorname{sh}(x + x') = \operatorname{sh} x \operatorname{ch} x' + \operatorname{ch} x \operatorname{sh} x'.
\end{align*}
$$

Les fonctions hyperboliques permettent d’exprimer les parties réelles et imaginaires de $\cos z$ et $\sin z$ pour $z = x + iy$, car
$$
\begin{align*}
\cos(x + iy) &= \cos x \cos iy - \sin x \sin iy = \cos x \operatorname{ch} y - i \sin x \operatorname{sh} y \\
\sin(x + iy) &= \sin x \cos iy + \cos x \sin iy = \sin x \operatorname{ch} y + i \cos x \operatorname{sh} y.
\end{align*}
$$

Enfin, on a
$$
\operatorname{D}(\operatorname{ch} x) = \operatorname{sh} x, \quad \operatorname{D}(\operatorname{sh} x) = \operatorname{ch} x, \quad \operatorname{D}(\operatorname{th} x) = 1 - \operatorname{th}^2 x = \frac{1}{\operatorname{ch}^2 x}.
$$

Comme $\operatorname{ch} x > 0$ pour tout $x$, on déduit de là que $\operatorname{sh} x$ est strictement croissant dans $\mathbf{R}$; comme $\operatorname{sh} 0 = 0$, $\operatorname{sh} x$ a donc le signe de $x$. Par suite, $\operatorname{ch} x$ est strictement décroissante pour $x \leq 0$, strictement croissante pour $x \geq 0$; enfin $\operatorname{th} x$ est strictement croissante dans $\mathbf{R}$. On a en outre
$$
\lim_{x \to -\infty} \operatorname{sh} x = -\infty, \quad \lim_{x \to +\infty} \operatorname{sh} x = +\infty
$$
$$
\lim_{x \to -\infty} \operatorname{ch} x = \lim_{x \to +\infty} \operatorname{ch} x = +\infty
$$
$$
\lim_{x \to -\infty} \operatorname{th} x = -1, \quad \lim_{x \to +\infty} \operatorname{th} x = +1 \tag{fig. 8 et 9}.
$$

On désigne parfois par $\operatorname{Arg} \operatorname{sh} x$ la fonction réciproque de $\operatorname{sh} x$, qui est une application strictement croissante de $\mathbf{R}$ sur $\mathbf{R}$; cette fonction s’exprime d’ailleurs à l’aide du logarithme, car de la relation $x = \operatorname{sh} y = \frac{1}{2}(e^y - e^{-y})$, on tire $e^{2y} - 2xe^y - 1 = 0$, et comme $e^y > 0$, $e^y = x + \sqrt{x^2 + 1}$, c’est-à-dire
$$
\operatorname{Arg} \operatorname{sh} x = \log (x + \sqrt{x^2 + 1}).
$$

De même, on désigne parfois par $\operatorname{Arg} \operatorname{ch} x$ la fonction réciproque de la restriction de $\operatorname{ch} x$ à $(0, +\infty)$; c’est une application strictement croissante de $(1, +\infty)$ sur $(0, +\infty)$; on montre comme ci-dessus que
$$
\operatorname{Arg} \operatorname{ch} x = \log (x + \sqrt{x^2 - 1}).
$$

Fig. 8

Les courbes $y = \operatorname{ch} x$ et $y = \operatorname{sh} x$ tracées sur les mêmes axes. La branche de $y = \operatorname{ch} x$ a son minimum au point $(0, 1)$ ; celle de $y = \operatorname{sh} x$ passe par l'origine et les deux courbes se rapprochent l'une de l'autre quand $x$ croît.

Fig. 9

La courbe $y = \operatorname{th} x$, croissante, passant par l'origine, entre les deux asymptotes $y = 1$ et $y = -1$.

Enfin, on désigne par Arg th $x$ la fonction réciproque de th $x$, qui est une application strictement croissante de $] - 1,\ +1[$ sur $\mathbf{R}$; on a d’ailleurs

$$
\operatorname{Arg}\operatorname{th}x = \frac{1}{2} \log \frac{1 + x}{1 - x}.
$$

#### Remarque {#fvr-iii-s1-n9-rem-1 .statement}

Pour $z$ complexe, on écrit aussi parfois
$$
\operatorname{ch}z = \frac{1}{2}(e^z + e^{-z}) = \cos iz \\
\operatorname{sh}z = \frac{1}{2}(e^z - e^{-z}) = -i \sin iz.
$$

Ces fonctions prolongent donc à $\mathbf{C}$ les fonctions hyperboliques définies dans $\mathbf{R}$.

## EXERCICES {#fvr-iii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
