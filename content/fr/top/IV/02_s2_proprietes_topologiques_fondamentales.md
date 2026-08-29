---
book: top
book_title: General Topology
chapter: IV
chapter_title: NOMBRES RÉELS
section: 2
section_title: Propriétés topologiques fondamentales de la droite numérique
lang: fr
source: top-i-iv-fr
book_pages: TG IV.6-TG IV.10, TG IV.47-TG IV.51
pdf_pages: 0277-0281, 0318-0322
extraction: ocr
subsections:
    - "no": 1
      title: L’axiome d’Archimède
      page: 6
      pdf_page: 277
    - "no": 2
      title: Parties compactes de $\mathbf{R}$
      page: 6
      pdf_page: 277
    - "no": 3
      title: Borne supérieure d’une partie de $\mathbf{R}$
      page: 7
      pdf_page: 278
    - "no": 4
      title: Caractérisation des intervalles
      page: 7
      pdf_page: 278
    - "no": 5
      title: Parties connexes de $\mathbf{R}$
      page: 8
      pdf_page: 279
    - "no": 6
      title: Homéomorphismes d’un intervalle sur un intervalle
      page: 9
      pdf_page: 280
statements: 13
exercises: 16
content_sha256: 842a87d576784909c12db349ec9b48782447457e381a492f4bfcc8417b49fe3b
---

## § 2. PROPRIÉTÉS TOPOLOGIQUES FONDAMENTALES DE LA DROITE NUMÉRIQUE

### 1. L’axiome d’Archimède

Les propriétés topologiques de la droite numérique, que nous allons exposer dans ce paragraphe, découlent du théorème suivant:

#### Théorème 1 {#top-iv-s2-thm-1 .statement}

*Quels que soient les nombres réels $x > 0$ et $y > 0$, il existe un entier $n > 0$ tel que $y < nx$.*

En effet, il existe deux nombres rationnels $p/q, r/s$ tels que $0 < p/q < x$ et $y < r/s$, puisque les intervalles ouverts $]0, x[$ et $]y, \to[$ ne sont pas vides (IV, p. 4, prop. 4); il suffit de prendre $n$ tel que $nps > qr$.

#### Remarque {#top-iv-s2-n1-rem-1 .statement}

On trouvera dans V, § 2 une construction axiomatique de la théorie des nombres réels dans laquelle l’énoncé ci-dessus figure en tant qu’axiome; pour plus de détails sur cet axiome, voir la Note historique du chap. IV.

### 2. Parties compactes de $\mathbf{R}$

**Théorème 2** (Borel–Lebesgue). — *Pour qu’une partie de la droite numérique $\mathbf{R}$ soit compacte, il faut et il suffit qu’elle soit fermée et bornée.*

1) La condition est *nécessaire*. Soit $A$ une partie compacte de $\mathbf{R}$, et $a$ un nombre réel $> 0$. L’ensemble $A$ est fermé (I, p. 62, prop. 4) et il existe un nombre fini de points $x_i$ ($1 \leq i \leq n$) de $\mathbf{R}$ tels que $A$ soit contenu dans la réunion des voisinages $[x_i - a, x_i + a]$ (I, p. 61). Soit $b$ le maximum des nombres $|x_i|$; on a $A \subset (-b - a, b + a)$.

2) La condition est *suffisante*. Il suffit de montrer que tout intervalle $(-a, a)$ ($a > 0$) est *compact*; comme cet intervalle est un ensemble fermé dans un espace uniforme complet, il suffira de voir que, pour tout $b > 0$, on peut recouvrir $(-a, +a)$ par un nombre *fini* d’intervalles de la forme $[x - b, x + b]$ (II, p. 30, corollaire). Or, soit $n$ un entier $> 0$ tel que $a < nb$; si $x \in (-a, +a)$ et si $m$ est le plus grand entier (positif ou négatif) tel que $mb \leq x$, on a $-n \leq m \leq n$ et $mb \leq x \leq (m+1)b$; donc les $2n+1$ intervalles $((k-1)b, (k+1)b)$ ($-n \leq k \leq n$) forment un recouvrement du type voulu.

#### Corollaire 1 {#top-iv-s2-thm-1-cor-1 .statement}

*Pour qu’une partie de la droite numérique $\mathbf{R}$ soit relativement compacte, il faut et il suffit qu’elle soit bornée.*

#### Corollaire 2 {#top-iv-s2-thm-1-cor-2 .statement}

*La droite numérique est un espace localement compact et non compact.*

    *Remarque.* — Le th. 2 est souvent cité sous le nom de « théorème de Heine–Borel »; voir les Notes historiques des chap. II et IV.

### 3. Borne supérieure d’une partie de $\mathbf{R}$

Rappelons (E, III, p. 10) que la *borne supérieure* (resp. *inférieure*) d’une partie $A$ d’un ensemble ordonné $E$ est (lorsqu’elle existe) *le plus petit majorant* (resp. *le plus grand minorant*) de $A$.

#### Théorème 3 {#top-iv-s2-thm-3 .statement}

*Toute partie majorée* (resp. *minorée*) *et non vide de la droite numérique a une borne supérieure* (resp. *inférieure*).

En effet, soit $A$ une partie majorée et non vide de $\mathbf{R}$; soit $b$ un majorant de $A$; on a donc $A \subset ]\leftarrow, b]$. Pour chaque $x \in A$, considérons l’ensemble $A_x$ des majorants de $x$ appartenant à $A$; les ensembles $A_x$ forment une *base de filtre* $\mathcal{B}$ sur $\mathbf{R}$, car $A_y \subset A_x$ si $y \geq x$. Soit $a$ un point de $A$; pour tout $x \geq a$, appartenant à $A$, $A_x$ est contenu dans l’intervalle *compact* $[a, b]$, donc la base de filtre $\mathcal{B}$ a un point adhérent $c$. Les intervalles $[x, \rightarrow[$ étant fermés, $c$ appartient à leur intersection, donc $c$ est un *majorant* de $A$; d’autre part, tout autre majorant $z$ de $A$ est $\geq c$, car, dans le cas contraire, le voisinage $]z, \rightarrow[$ de $c$ ne contiendrait aucun point de $A$; $c$ est donc bien la *borne supérieure* de $A$.

On peut raisonner de même pour un ensemble minoré non vide $B$, ou remarquer simplement que $-B$ est majoré et non vide, et que, si $c$ est la borne supérieure de $-B$, $-c$ est la borne inférieure de $B$.

La borne supérieure $c$ de $A$ peut être caractérisée par les deux propriétés suivantes:
1° Quel que soit $x \in A$, $x \leq c$.
2° Quel que soit $a < c$, il existe $x \in A$ tel que $a < x \leq c$.

La borne supérieure d’un ensemble *fermé* (majoré et non vide) appartient à cet ensemble et en constitue *le plus grand élément*; la borne supérieure d’une partie $A$ quelconque, majorée et non vide, de $\mathbf{R}$, peut donc être définie comme *le plus grand nombre réel adhérent* à $A$.

### 4. Caractérisation des intervalles

#### Proposition 1 {#top-iv-s2-prop-1 .statement}

*Pour qu’une partie non vide $A$ de $\mathbf{R}$ soit un intervalle, il faut et il suffit que, quels que soient les points $a, b$ de $A$ tels que $a < b$, l’intervalle fermé $[a, b]$ soit contenu dans $A$.*

La condition est évidemment nécessaire. Réciproquement, supposons-la vérifiée. Si A n’est ni majoré ni minoré, il est identique à $\mathbf{R}$, car, pour tout $x \in \mathbf{R}$, il existe alors deux points $a, b$ de A tels que $a < x < b$. Si A est majoré et non minoré, soit $k$ sa borne supérieure ; quel que soit $x < k$, il existe $a$ et $b$ dans A tels que $a < x < b \leq k$, donc $x \in A$; A ne peut donc être que l’un des deux intervalles $]\leftarrow, k]$, $]\leftarrow, k[$. On raisonne de même dans les autres cas.

### 5. Parties connexes de $\mathbf{R}$

#### Théorème 4 {#top-iv-s2-thm-4 .statement}

Pour qu’une partie A de $\mathbf{R}$ soit connexe, il faut et il suffit que A soit un intervalle.

1° La condition est nécessaire. Supposons A connexe ; s’il est réduit à un point, c’est un intervalle. Sinon, soient $a$ et $b$ deux points de A tels que $a < b$; il suffit, d’après la prop. 1 de IV, p. 7, de montrer que tout $x$ tel que $a < x < b$ appartient à A. Or, si on avait $x \notin A$, on aurait $A \subset \mathcal{G}\{x\}$; mais $\mathcal{G}\{x\}$ est la réunion de deux ensembles ouverts $]\leftarrow, x[$ et $x, \rightarrow[$ qui sont sans point commun et dont chacun rencontre A; A ne serait donc pas connexe, contrairement à l’hypothèse.

2° La condition est suffisante. Montrons d’abord que tout intervalle compact $[a, b]$ est connexe. Pour tout entier $n > 0$ soit $V_{1/n}$ l’entourage formé des couples $(x, y)$ tels que $|x - y| \leq 1/n$; d’après II, p. 32, prop. 6, il suffit de voir que deux points quelconques $x, y$ de $[a, b]$ tels que $x < y$ peuvent être joints par une $V_{1/n}$-chaîne. Soit $p$ le plus grand entier tel que $p/n \leq x$, $q$ le plus grand entier tel que $q/n \leq y$ (ces entiers existent d’après le th. 1 de IV, p. 6); on a $p \leq q$. Si $q = p$, $y - x < 1/n$, les points $x$ et $y$ forment déjà une $V_{1/n}$-chaîne. Si $q < p$, posons $x_i = (p + i)/n$ ($i = 1, 2, \ldots, q - p$); on a $x_1 - x \leq 1/n$, $y - x_{q-p} \leq 1/n$ et $x_{i+1} - x_i = 1/n$, donc les points $x, x_1, x_2, \ldots, x_{q-p}, y$ forment une $V_{1/n}$-chaîne joignant $x$ et $y$.

Si maintenant I est un intervalle quelconque non réduit à un point, et $a$ et $b$ deux points de I tels que $a < b$, l’intervalle $(a, b)$ est contenu dans I et est connexe, donc I est connexe.

#### Corollaire 1 {#top-iv-s2-thm-4-cor-1 .statement}

La droite numérique est un espace connexe et localement connexe.

#### Corollaire 2 {#top-iv-s2-thm-4-cor-2 .statement}

Les seules parties compactes et connexes de $\mathbf{R}$ sont les intervalles fermés bornés.

D’après le th. 4, une partie de $\mathbf{R}$ ne contenant aucun intervalle non réduit à un point est totalement discontinue; il en est ainsi, en particulier, de l’ensemble $\mathbf{Q}$ des nombres rationnels, puisque l’ensemble $\mathbf{C}\mathbf{Q}$ des nombres irrationnels est partout dense.

#### Proposition 2 {#top-iv-s2-prop-2 .statement}

Tout ensemble ouvert non vide dans $\mathbf{R}$ est la réunion d’une famille dénombrable d’intervalles ouverts, sans point commun deux à deux.

Soit A un ensemble ouvert non vide dans $\mathbf{R}$; comme $\mathbf{R}$ est localement connexe, toute composante connexe de A est un ensemble ouvert connexe (I, p. 85, prop. 11) donc un intervalle ouvert d’après le th. 4. Deux quelconques de ces intervalles sont toujours sans point commun; d’autre part, chacun d’eux contient un nombre rationnel, donc l’ensemble de ces intervalles a une puissance inférieure à celle de $\mathbf{Q}$, c’est-à-dire est dénombrable.

Tout ensemble fermé dans $\mathbf{R}$ est donc le complémentaire de la réunion d’une suite (finie ou infinie) $(I_n)$ d’intervalles ouverts sans point commun deux à deux; ces intervalles sont dits intervalles contigus à l’ensemble fermé considéré. Réciproquement, si on se donne une telle suite d’intervalles, le complémentaire de leur réunion est un ensemble fermé auquel ces intervalles sont contigus.

#### Exemple {#top-iv-s2-n5-exa-1 .statement}

Définissons par récurrence, une famille dénombrable $(I_{n,p})$ d’intervalles ouverts, deux à deux sans point commun, de la manière suivante:

L’entier $n$ prend toutes les valeurs $\geqslant 0$; pour chaque valeur de $n, p$ prend les valeurs $1, 2, 3, \ldots, 2^n$. Tous les intervalles $I_{n,p}$ sont contenus dans $A = [0, 1]$, et on prend $I_{0,1} = ]\frac{1}{3}, \frac{2}{3}[$ (« tiers médian » de ]$0, 1[$). Supposons ensuite les $2^{m+1} - 1$ intervalles $I_{n,p}$ définis pour $0 \leqslant n \leqslant m$, de sorte que, si $J_m$ est leur réunion, l’ensemble $A \cap \complement J_m$ soit la réunion de $2^{m+1}$ intervalles fermés $K_{m,p}$ ($1 \leqslant p \leqslant 2^{m+1}$) deux à deux sans point commun, et ayant tous pour longueur $\frac{1}{3^{m+1}}$. Si $K_{m,p} = [a, b]$, on prend alors pour $I_{m+1,p}$ l’intervalle ouvert $\left] a + \frac{b-a}{3}, b - \frac{b-a}{3} \right[$ (« tiers médian » de l’intervalle $]a, b[$); on vérifie immédiatement que $K_{m,p} \cap \complement I_{m+1,p}$ est réunion de deux intervalles disjoints de longueur $\frac{1}{3^{m+2}}$, donc $A \cap \complement J_{m+1}$ est réunion de $2^{m+2}$ intervalles fermés disjoints de longeur $\frac{1}{3^{m+2}}$ (fig. 1).

![Figure 1](https://i.imgur.com/3Q5z5QG.png)

Figure 1

Si $K'$ est le complémentaire de la réunion des $I_{n,p}$ l’ensemble fermé $K = A \cap K'$ est appelé l’ensemble triadique de Cantor; il est évidemment compact (IV, p. 6, th. 2); en outre, il est totalement discontinu. En effet, s’il contenait un intervalle $I$ de longueur $> 0$, $I$ serait nécessairement contenu dans un intervalle $K_{m,p}$, donc sa longueur serait $\leqslant 1/3^{m+1}$ quel que soit $m$, ce qui est absurde.

### 6. Homéomorphismes d’un intervalle sur un intervalle

#### Théorème 5 {#top-iv-s2-thm-5 .statement}

Soit $I$ un intervalle de $\mathbf{R}$; pour qu’une application $f$ de $I$ dans $\mathbf{R}$ soit un homéomorphisme de $I$ sur $f(I)$, il faut et il suffit que $f$ soit strictement monotone et continue dans $I$; $f(I)$ est alors un intervalle de $\mathbf{R}$.

1° La condition est nécessaire. En effet, soient $a$ et $b$ deux points de $I$ tels que $a < b$ et supposons par exemple $f(a) < f(b)$. Montrons que $f$ est strictement croissante dans $I$. Tout d’abord, si $a < c < b$, on a nécessairement $f(a) < f(c) < f(b)$; en effet, si on avait par exemple $f(a) < f(b) < f(c)$, l’image par $f$ de l’intervalle $[a, c]$ serait un ensemble connexe (I, p. 82, prop. 4) et contiendrait donc l’intervalle $\{f(a), f(c)\}$; il existerait par suite $x \in [a, c]$ tel que $f(x) = f(b)$, contrairement à l’hypothèse que $f$ est injective.

On en déduit que, si $x$ et $y$ sont deux points de I tels que $x < y$, on a $f(x) < f(y)$; en effet, on a $f(a) < f(x) < f(b)$ pour $a < x < b$, $f(a) < f(b) < f(x)$ pour $b < x, f(x) < f(a) < f(b)$ pour $x < a$; en répétant le raisonnement pour $a, x$ et $y$ au lieu de $a, b$ et $x$, on voit que $f(x) < f(y)$.

$2^\circ$ La condition est *suffisante*. Supposons $f$ continue et strictement monotone (par exemple, strictement croissante) dans I; $f(I)$ est connexe, donc est un intervalle, et comme $f$ est strictement croissante, $f$ est une application bijective de I sur $f(I)$. En outre, l’image par $f$ d’un intervalle ouvert *dans* I est un intervalle ouvert *dans* $f(I)$; donc (IV, p. 5, prop. 5), $f$ est un homéomorphisme de I sur $f(I)$.

#### Remarque {#top-iv-s2-n6-rem-1 .statement}

La première partie de la démonstration précédente établit en fait qu’une application *continue* et *injective* de I dans $\mathbf{R}$ est *strictement monotone*; d’après la seconde partie, on voit que *toute application injective et continue* $f$ *d’un intervalle* I *dans* $\mathbf{R}$ *est un homéomorphisme de* I *sur* $f(I)$.

## EXERCICES {#top-iv-s2-exercises}

See the [exercises for § 2](exercises/s2/).
