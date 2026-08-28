---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Algèbres de Lie
section: 7
section_title: Le théorème d'Ado
lang: fr
source: lie-i-fr
pdf_pages: 0093-0098, 0133-0144
extraction: ocr
subsections:
    - "no": 1
      title: Coefficients d’une représentation
      page: 0
      pdf_page: 94
    - "no": 2
      title: Le théorème d’agrandissement
      page: 0
      pdf_page: 94
    - "no": 3
      title: Le théorème d’Ado
      page: 0
      pdf_page: 97
statements: 5
exercises: 3
content_sha256: 339de6daa991ab17374c3e2e3705963e7c21541c7af192be97426dda50db8b62
---

## § 7. Le théorème d’Ado

On rappelle que $K$ désigne un corps de caractéristique 0 et que toutes les algèbres de Lie sont supposées de dimension finie sur $K$.

### 1. Coefficients d’une représentation

Soient U une algèbre associative à élément unité sur K, U* le dual de l’espace vectoriel U, et ρ une représentation de U dans un espace vectoriel E. Pour $e \in E$ et $e' \in E^*$, soit $\theta(e, e') \in U^*$ le coefficient correspondant de $\rho$ (Alg., chap. VIII, § 13, n° 3). On rappelle que $\theta(e, e')(x) = \langle \rho(x)e, e' \rangle$, et que l’application $e \mapsto \theta(e, e')$ est, pour $e'$ fixé, un homomorphisme du U-module E dans le U-module U* de la représentation corégulière de U (loc. cit., prop. 1); par suite, le sous-espace vectoriel de U* engendré par les coefficients de $\rho$ (sous-espace que nous noterons C(ρ) dans ce paragraphe) est un sous-U-module de U*. Si $(e'_i)_{i \in I}$ est une famille d’éléments engendrant E* sur K, l’application $e \to (\theta(e, e'_i))$ est un U-homomorphisme injectif de E dans C(ρ)I, car $\theta(e, e'_i) = 0$ pour tout i entraîne $\langle e, e'_i \rangle = \langle \rho(1)e, e'_i \rangle = \theta(e, e'_i)(1) = 0$ pour tout i, donc $e = 0$.

En particulier, si U est l’algèbre enveloppante d’une algèbre de Lie g, et si $\rho$ est une représentation de g (identifiée à une représentation de U) dans un espace vectoriel E de dimension n, le g-module E est isomorphe à un sous-g-module de $(C(\rho))^n$.

### 2. Le théorème d’agrandissement

Soient $g = \mathfrak{h} + g'$ une algèbre de Lie somme directe d’un idéal $g'$ et d’une sous-algèbre $\mathfrak{h}$, U l’algèbre enveloppante de g, et $U' \subset U$ l’algèbre enveloppante de $g'$. Il existe une structure de g-module sur $U'$ et une seule telle que : α) pour $x \in g'$ et $u \in U'$, $x_{U'}u = -ux$; β) pour $x \in \mathfrak{h}$ et $u \in U'$, $x_{U'}u = xu - ux$ (ce dernier élément est bien dans $U'$, puisque la dérivation intérieure de U définie par x laisse stable $g'$, donc $U'$). En effet, les conditions α) et β) définissent de manière unique une application linéaire $x \to x_{U'}$ de g dans $\mathcal{L}_K(U')$. Il suffit donc de vérifier que $[x, y]_{U'} = [x_{U'}, y_{U'}]$; on peut se borner à envisager les cas suivants :

1) $x \in g', y \in g'$: alors,

$$
[x, y]_{U'}u = -u(xy - yx) = (x_{U'}y_{U'} - y_{U'}x_{U'})u;
$$

2) $x \in \mathfrak{h}, y \in g'$: alors,
$$
[x, y]_{U'} u = -u(xy - yx)
= x(-uy) - (-uy)x + (xu - ux)y = (x_{U'}y_{U'} - y_{U'}x_{U'})u;
$$

3) $x \in \mathfrak{h}, y \in \mathfrak{h}$: alors, $[x, y]_{U'}$ et $[x_{U'}, y_{U'}]$ sont deux dérivations de $U'$ dont les restrictions à $g'$ coïncident avec celles de $\operatorname{ad}_g [x, y]$ et $[\operatorname{ad}_g x, \operatorname{ad}_g y]$; donc ces dérivations sont égales.

Nous considérerons aussi la représentation duale $x \mapsto -{}^t x_{U'}$ de $g$ dans $U'^*$. Pour $x \in g'$, $-{}^t x_{U'}$ est la transposée de la multiplication à droite par $x$ dans $U'$; la représentation correspondante de $U'$ est donc la représentation corégulière de $U'$.

#### Définition 1 {#lie-i-s7-def-1 .statement}

Soient $g$ une algèbre de Lie, $g'$ une sous-algèbre de $g$, et $\rho'$ une représentation de $g'$ dans $V'$. Une représentation $\varphi$ de $g$ dans $V$ est appelée un agrandissement de $\rho'$ à $g$ s’il existe un homomorphisme injectif du $g'$-module $V'$ dans le $g'$-module $V$. On dit aussi que le $g$-module $V$ est un agrandissement du $g'$-module $V'$.

Si $\rho'$ est de dimension finie, et si $g'$ est un idéal résoluble de $g$, il est nécessaire, pour l’existence d’un agrandissement de dimension finie, que $[g, g']$ soit contenu dans le plus grand idéal de nilpotence de $\rho'$ (\S 5, no 3, th. 1).

#### Théorème 1 (Zassenhaus) {#lie-i-s7-thm-1 .statement}

Soient $g = g' + \mathfrak{h}$ une algèbre de Lie somme directe d’un idéal $g'$ et d’une sous-algèbre $\mathfrak{h}$, et $\rho'$ une représentation de dimension finie de $g'$, dont le plus grand idéal de nilpotence contient $[\mathfrak{h}, g']$.

a) Il existe un agrandissement de dimension finie $\varphi$ de $\rho'$ à $g$ dont le plus grand idéal de nilpotence contient celui de $\rho'$.

b) Si, pour tout $x \in \mathfrak{h}$, la restriction à $g'$ de $\operatorname{ad}_g x$ est nilpotente, on peut choisir $\varphi$ de façon qu’en outre le plus grand idéal de nilpotence de $\varphi$ contienne $\mathfrak{h}$.

Soit $U'$ l’algèbre enveloppante de $g'$. On supposera $U'$ et $U'^*$ munis des structures de $g$-modules définies au début de ce no.

U'*
Soit $I \subset U'$ le noyau de $\rho'$ (identifiée à une représentation de $U'$). C’est un idéal bilatère de codimension finie de $U'$. Le sous-espace $C(\rho')$ de $U'^*$ (cf. no 1) est orthogonal à $I$. Soit $S$ le sous-g-module de $U'^*$ engendré par $C(\rho')$.

Nous allons montrer que $S$ est de dimension finie sur $K$. Soient $V'$ l’espace où opère $\rho'$, et $V' = V'_0 \supset V'_1 \supset \cdots \supset V'_d = \{0\}$ une suite de Jordan-Hölder du $g'$-module $V'$. Soit $\rho'_i$ la représentation de $g'$ dans $V'_{i-1}/V'_i$ déduite de $\rho'$ ($1 \leq i \leq d$). Soit $I' \subset U'$ l’intersection des noyaux des $\rho'_i$ (identifiées à des représentations de $U'$). On a

$$
I'^d \subset I \subset I'
$$

et $I' \cap g'$ est le plus grand idéal de nilpotence de $\rho'$. D’après le § 2, no 6, cor. de la prop. 6, $I'^d$ est de codimension finie dans $U'$. Si $x \in \mathfrak{h}$, la dérivation $u \to xu - ux$ de $U'$ applique $g'$ dans $[\mathfrak{h}, g'] \subset I'$, donc $U'$ dans $I'$, donc $I'^d$ dans $I'^d$. Par ailleurs, il est clair que $I'^d$ est un sous-$g'$-module de $U'$. Donc $I'^d$ est un sous-g-module de $U'$. L’orthogonal de $I'^d$ dans $U'^*$ est un sous-g-module de dimension finie qui contient $C(\rho')$, donc $S$. Ceci montre bien que $S$ est de dimension finie sur $K$. Pour $x \in I' \cap g'$, $x^d$ est évidemment contenu dans l’annulateur du $g$-module $U'/I'^d$, donc aussi dans l’annulateur du $g$-module $S$.

On a vu au no 1 que le $g'$-module $V'$ est isomorphe à un sous-$g'$-module d’un produit $(C(\rho'))^n$. Donc le $g$-module $S^n$ fournit un agrandissement de dimension finie $\rho$ de $\rho'$ à $g$. En outre, $\rho(x)$ est nilpotent pour $x \in I' \cap g'$; comme $I' \cap g'$ est un idéal de $g$ (car il contient $[\mathfrak{h}, g']$ par hypothèse), on voit que $I' \cap g'$ est contenu dans le plus grand idéal de nilpotence de $\rho$. On a ainsi prouvé a).

Supposons enfin que, pour tout $x \in \mathfrak{h}$, la restriction à $g'$ de $\mathrm{ad}_g x$ soit nilpotente. Comme les éléments de $\mathfrak{h}$ opèrent dans $U'$ par des dérivations, il existe, pour tout $u \in U'$ et tout $x \in \mathfrak{h}$, un entier $e$ tel que $(x_{v'})^e \cdot u = 0$; les endomorphismes déduits de $x_{v'}$ dans $U'/I'^d$ et dans $S$ (qui sont des espaces de dimension finie) sont donc nilpotents. Ainsi, $\rho(x)$ est nilpotent pour tout $x \in \mathfrak{h}$. On a vu plus haut qu’il en est de même pour $x \in I' \cap g'$. Comme $I' \cap g'$ est un idéal de $g'$ contenant $[h, g']$, la somme $h + (I' \cap g')$ est aussi un idéal de $g$. L’assertion b) du th. 1 résulte donc du lemme suivant :

#### Lemme 1 {#lie-i-s7-lem-1 .statement}

Soit $g = g' + h$ une algèbre de Lie somme d’un idéal $g'$ et d’une sous-algèbre $h$. Soit $\sigma$ une représentation de dimension finie de $g$. On suppose que $\sigma(x)$ est nilpotent pour tout $x \in g'$ et tout $x \in h$. Alors, $\sigma(x)$ est nilpotent pour tout $x \in g$.

Passant au quotient par le noyau de $\sigma$, on peut supposer $\sigma$ fidèle. Alors, $g'$ et $h$ sont nilpotentes, donc $g$, qui est une extension d’un quotient de $h$ par $g'$, est résoluble. Alors, $h$ et $g'$ sont contenus dans le plus grand idéal de nilpotence de $\sigma$ ($\S 5$, no 3, cor. 6 du th. 1).

Pour une amélioration du th. 1, cf. exerc. 4.

### 3. Le théorème d’Ado

#### Proposition 1 {#lie-i-s7-prop-1 .statement}

Soient $g$ une algèbre de Lie, $n$ son plus grand idéal nilpotent, $a$ un idéal nilpotent de $g$, et $\rho$ une représentation de dimension finie de $a$ telle que tout élément de $\rho(a)$ soit nilpotent. Alors, $\rho$ admet un agrandissement de dimension finie $\sigma$ à $g$, tel que tout élément de $\sigma(n)$ soit nilpotent.

Soit $a = n_0 \subset n_1 \subset \cdots \subset n_p = n$ une suite de sous-algèbres de $n$, telles que $n_{i-1}$ soit un idéal de codimension 1 de $n_i$ pour $1 \leq i \leq p$ ($\S 4$, no 1, prop. 1 e)). L’algèbre $n_i$ est donc somme directe de $n_{i-1}$ et d’une sous-algèbre de dimension 1. Comme $\mathrm{ad}_n x$ est nilpotent pour tout $x \in n$, on peut (th. 1) trouver de proche en proche des agrandissements de dimension finie $\rho_1, \rho_2, \ldots, \rho_p = \rho'$ de $\rho$ à $n_1, n_2, \ldots, n_p = n$, tels que tout élément de $\rho'(n)$ soit nilpotent.

Soit $r$ le radical de $g$, et soit $n = r_0 \subset r_1 \subset \cdots \subset r_q = r$ une suite de sous-algèbres de $r$, telle que $r_{i-1}$ soit un idéal de codimension 1 de $r_i$, pour $1 \leq i \leq q$ ($\S 5$, no 1, prop. 2d)). L’algèbre $r_i$ est donc somme directe de $r_{i-1}$ et d’une sous-algèbre de dimension 1. Comme $[r, r] \subset n$, on peut (th. 1) trouver de proche en proche des agrandissements de dimension finie $\rho'_1, \rho'_2, \ldots, \rho'_q = \rho''$ de $\rho'$ à $r_1, r_2, \ldots, r_q = r$, tels que tout élément de $\rho''(n)$ soit nilpotent.

Enfin, $g$ est somme directe de $r$ et d’une sous-algèbre $s$ ($\S 6$, n° 8, th. 5). Comme $[s, r] \subset n$, on peut (th. 1) trouver un agrandissement de dimension finie $\sigma$ de $\rho''$ à $g$ tel que tout élément de $\sigma(n)$ soit nilpotent.

#### Théorème 2 {#lie-i-s7-thm-2 .statement}

*Toute algèbre de Lie possède une représentation linéaire fidèle de dimension finie.*

De façon plus précise :

**Théorème 3** (Ado). — *Soient $g$ une algèbre de Lie et $n$ son plus grand idéal nilpotent. Il existe une représentation fidèle $\rho$ de dimension finie de $g$ telle que tout élément de $\rho(n)$ soit nilpotent.*

L’algèbre de Lie $K$ de dimension 1 admet des représentations fidèles $\tau$ de dimension finie telles que tout élément de $\tau(K)$ soit nilpotent, par exemple la représentation

$$
\lambda \mapsto \begin{pmatrix} 0 & 0 \\ \lambda & 0 \end{pmatrix}.
$$

On en déduit aisément que le centre $c$ de $g$, qui est produit d’algèbres de dimension 1, admet une représentation fidèle $\sigma$ de dimension finie telle que tout élément de $\sigma(c)$ soit nilpotent. Soit $\sigma_1$ un agrandissement de dimension finie de $\sigma$ à $g$ tel que tout élément de $\sigma_1(n)$ soit nilpotent (prop. 1); si $f$ désigne le noyau de $\sigma_1$, on a $f \cap c = \{0\}$. Par ailleurs, soit $\sigma_2$ la représentation adjointe de $g$, dont le noyau est $c$; tout élément de $\sigma_2(n)$ est nilpotent. La somme directe $\rho$ de $\sigma_1$ et $\sigma_2$ est de dimension finie; tout élément de $\rho(n)$ est nilpotent; et le noyau de $\rho$, contenu dans $f$ et dans $c$, est nul, de sorte que $\rho$ est fidèle.

## EXERCICES {#lie-i-s7-exercises}

Les conventions du § 7 restent valables, sauf mention du contraire.

See the [exercises for § 7](exercises/s7/).
