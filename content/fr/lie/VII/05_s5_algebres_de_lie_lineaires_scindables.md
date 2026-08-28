---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: Sous-algèbres de Cartan. Éléments réguliers
section: 5
section_title: Algèbres de Lie linéaires scindables
lang: fr
source: lie-vii-viii-fr
pdf_pages: 0034-0044, 0058-0061
extraction: ocr
subsections:
    - "no": 1
      title: Algèbres de Lie linéaires scindables
      page: 0
      pdf_page: 34
    - "no": 2
      title: Enveloppe scindable
      page: 0
      pdf_page: 36
    - "no": 3
      title: Décompositions des algèbres scindables
      page: 0
      pdf_page: 37
    - "no": 4
      title: Algèbres de Lie linéaires d’endomorphismes nilpotents
      page: 0
      pdf_page: 39
    - "no": 5
      title: Caractérisations des algèbres de Lie scindables
      page: 0
      pdf_page: 42
statements: 28
exercises: 11
content_sha256: a24d978da4af3d8ad9b83d93064b0453b1784b2438c3b5e6aedb1c71a8f69ecf
---

## § 5. Algèbres de Lie linéaires scindables

Dans ce paragraphe, on suppose $k$ de caractéristique 0. On désigne par $V$ un espace vectoriel de dimension finie.

### 1. Algèbres de Lie linéaires scindables

#### Définition 1 {#lie-vii-s5-def-1 .statement tag=00WG}

Soit $g$ une sous-algèbre de Lie de $\mathfrak{gl}(V)$. On dit que $g$ est scindable si $g$ contient les composantes semi-simple et nilpotente de chacun de ses éléments (A, VII, § 5, no 8).

#### Exemple 1 {#lie-vii-s5-n1-exa-1 .statement tag=00WH}

Soient $V'$ et $V''$ des sous-espaces vectoriels de $V$ tels que $V'' \supset V'$. L'ensemble des $x \in \mathfrak{gl}(V)$ tels que $x(V'') \subset V'$ est une sous-algèbre de Lie scindable de $\mathfrak{gl}(V)$; en effet, pour tout $x \in \mathfrak{gl}(V)$, les composantes semi-simple et nilpotente de $x$ sont de la forme $P(x)$ et $Q(x)$, où $P$ et $Q$ sont des polynômes sans terme constant.

#### Exemple 2 {#lie-vii-s5-n1-exa-2 .statement tag=00WI}

Supposons $V$ muni d'une structure d'algèbre. L'ensemble des dérivations de $V$ est une sous-algèbre de Lie scindable de $\mathfrak{gl}(V)$ ($§ 1$, no 1, prop. 4 (ii)).

#### Exemple 3 {#lie-vii-s5-n1-exa-3 .statement tag=01KQ}

*Plus généralement, on peut montrer que l'algèbre de Lie d'un sous-groupe algébrique de $\mathbf{GL}(V)$ est scindable.*

#### Proposition 1 {#lie-vii-s5-prop-1 .statement tag=00WJ}

Soient $g$ une sous-algèbre de Lie scindable de $\mathfrak{gl}(V)$, $x \in g$, $s$ et $n$ les composantes semi-simple et nilpotente de $x$.

(i) Les composantes semi-simple et nilpotente de $\mathrm{ad}_g x$ sont respectivement $\mathrm{ad}_g s$ et $\mathrm{ad}_g n$.

(ii) Pour que $x$ soit régulier dans $g$, il faut et il suffit que $s$ le soit.

(iii) Si $g'$ est une sous-algèbre de $\mathfrak{gl}(V)$ contenant $g$, tout automorphisme élémentaire de $g$ se prolonge en un automorphisme élémentaire de $g'$.

Posons $a = \mathfrak{gl}(V)$. D'après I, § 5, no 4, lemme 2, les composantes semi-simple et nilpotente de $\mathrm{ad}_a x$ sont $\mathrm{ad}_a s$ et $\mathrm{ad}_a n$; l'assertion (i) résulte de là. On en déduit que les polynômes caractéristiques de $\mathrm{ad}_g x$ et $\mathrm{ad}_g s$ sont les mêmes; d’où (ii). Si $\mathrm{ad}_g x$ est nilpotent, on a $\mathrm{ad}_g x = \mathrm{ad}_g n$, donc $\mathrm{ad}_{g'} n$ prolonge $\mathrm{ad}_g x$, et $n$ est un élément nilpotent de $g'$, d’où (iii).

Soit $g$ une sous-algèbre de Lie de $\mathfrak{gl}(V)$. On sait (I, § 6, no 5, th. 4) que les conditions suivantes sont équivalentes:
(i) la représentation identique de $g$ est semi-simple;
(ii) $g$ est réductive et tout élément du centre de $g$ est un endomorphisme semi-simple.
Ces conditions sont encore équivalentes à la suivante:
(iii) $g$ est une sous-algèbre réductive dans $\mathfrak{gl}(V)$.
En effet, (i) $\Rightarrow$ (iii) d’après I, § 6, no 5, cor. 3 du th. 4, et (iii) $\Rightarrow$ (i) d’après I, § 6, no 6, cor. 1 de la prop. 7. Nous allons voir que si $g$ vérifie ces conditions, $g$ est scindable. Plus généralement:

#### Proposition 2 {#lie-vii-s5-prop-2 .statement tag=00WK}

*Soient $g$ une sous-algèbre de Lie de $\mathfrak{gl}(V)$ réductive dans $\mathfrak{gl}(V)$, E un espace vectoriel de dimension finie et $\pi : g \to \mathfrak{gl}(E)$ une représentation linéaire semi-simple de $g$ dans $E$. Alors:*
(i) $g$ et $\pi(g)$ sont scindables.
(ii) *Les éléments semi-simples (resp. nilpotents) de $\pi(g)$ sont les images par $\pi$ des éléments semi-simples (resp. nilpotents) de $g$*.
(iii) *Si $\mathfrak{h}$ est une sous-algèbre scindable de $\mathfrak{gl}(V)$ contenue dans $g$, $\pi(\mathfrak{h})$ est une sous-algèbre scindable de $\mathfrak{gl}(E)$*.
(iv) *Si $\mathfrak{h}'$ est une sous-algèbre scindable de $\mathfrak{gl}(E)$, $\pi^{-1}(\mathfrak{h}')$ est une sous-algèbre scindable de $\mathfrak{gl}(V)$*.

Soit $s = [g, g]$ et soit $c$ le centre de $g$. On a $g = s \times c$, et $\pi(g) = \pi(s) \times \pi(c)$ d’après I, § 6, no 4, cor. de la prop. 5. Soient $y \in s$, $z \in c$, $y_s$ et $y_n$ les composantes semi-simple et nilpotente de $y$. Alors $y_s, y_n \in s$ (I, § 6, no 3, prop. 3), $y_s + z$ est semi-simple (A, VII, § 5, no 7, cor. de la prop. 16), et $y_n$ commute à $y_s + z$. Donc les composantes semi-simple et nilpotente de $y + z$ sont $y_s + z$ et $y_n$. Ainsi, $g$ est scindable. Comme $\pi(g)$ est réductive dans $\mathfrak{gl}(E)$, le même argument s’applique à $\pi(g)$ et montre que $\pi(g)$ est scindable. En outre, les éléments nilpotents de $g$ (resp. $\pi(g)$) sont les éléments nilpotents de $s$ (resp. $\pi(s)$). Donc les éléments nilpotents de $\pi(g)$ sont les images par $\pi$ des éléments nilpotents de $g$ (I, § 6, no 3, prop. 4). Les éléments semi-simples de $g$ (resp. $\pi(g)$) sont les sommes d’éléments semi-simples de $s$ (resp. $\pi(s)$) et d’éléments de $c$ (resp. $\pi(c)$). Donc les éléments semi-simples de $\pi(g)$ sont les images par $\pi$ des éléments semi-simples de $g$ (I, loc. cit.). D’où (ii).

Les assertions (iii) et (iv) résultent immédiatement de (i) et (ii).

#### Remarque 1 {#lie-vii-s5-n1-rem-1 .statement tag=00WL}

L’hypothèse de semi-simplicité faite sur $\pi$ équivaut à dire que $\pi(x)$ est semi-simple pour tout $x \in c$. Cette hypothèse est notamment vérifiée lorsque $\pi$ se déduit de la représentation identique $g \to \mathfrak{gl}(V)$ par application successive des opérations suivantes : produit tensoriel, passage au dual, à une sous-représentation, à un quotient, à une somme directe.

#### Remarque 2 {#lie-vii-s5-n1-rem-2 .statement tag=00WM}

Soient $g \subset \mathfrak{gl}(V)$, $g' \subset \mathfrak{gl}(V')$ des algèbres de Lie scindables, $\varphi$ un isomorphisme de $g$ sur $g'$. On prendra garde que $\varphi$ ne transforme pas nécessairement les éléments semi-simples (resp. nilpotents) de $g$ en éléments semi-simples (resp. nilpotents) de $g'$ (exerc. 2). Il en est toutefois ainsi si $g$ est semi-simple (I, § 6, n° 3, th. 3).

#### Proposition 3 {#lie-vii-s5-prop-3 .statement tag=00WN}

*Soit $a$ une sous-algèbre de Lie scindable de $\mathfrak{gl}(V)$ et soient $b$ et $c$ des sous-espaces vectoriels de $\mathfrak{gl}(V)$ tels que $b \subset c$. Soit $a'$ l’ensemble des $x \in a$ tels que $[x, c] \subset b$. Alors $a'$ est scindable.*

Posons $g = \mathfrak{gl}(V)$; la sous-algèbre $h'$ de $\mathfrak{gl}(g)$ formée des $z \in \mathfrak{gl}(g)$ tels que $z(c) \subset b$ est scindable (Exemple 1). Soit $\pi : g \to \mathfrak{gl}(g)$ la représentation adjointe de $g$. La prop. 2 (iv), appliquée à $\pi$, montre que $\pi^{-1}(h')$ est scindable. Il en est donc de même de $a' = a \cap \pi^{-1}(h')$.

#### Corollaire 1 {#lie-vii-s5-prop-3-cor-1 .statement tag=00WO}

*Si $a$ est une sous-algèbre de Lie scindable de $\mathfrak{gl}(V)$, et $n$ une sous-algèbre de Lie de $a$, le normalisateur (resp. le centralisateur) de $n$ dans $a$ est scindable.*

Cela résulte de la prop. 3 en prenant $c = n$, $b = n$ (resp. $c = n$, $b = \{0\}$).

#### Corollaire 2 {#lie-vii-s5-prop-3-cor-2 .statement tag=00WP}

*Les sous-algèbres de Cartan d’une sous-algèbre de Lie scindable de $\mathfrak{gl}(V)$ sont scindables.*

Cela résulte du corollaire 1.

#### Remarque {#lie-vii-s5-n1-rem-3 .statement tag=00WQ}

Nous démontrerons plus loin (n° 5, th. 2) une réciproque au cor. 2.

### 2. Enveloppe scindable

L’intersection d’une famille de sous-algèbres de Lie scindables de $\mathfrak{gl}(V)$ est évidemment scindable. Par suite, si $g$ est une sous-algèbre de Lie de $\mathfrak{gl}(V)$, l’ensemble des sous-algèbres de Lie scindables de $\mathfrak{gl}(V)$ contenant $g$ possède un plus petit élément, appelé *l’enveloppe scindable* de $g$; dans ce paragraphe, cette enveloppe sera notée $e(g)$.

#### Proposition 4 {#lie-vii-s5-prop-4 .statement tag=00WR}

*Soient $g$ une sous-algèbre de Lie de $\mathfrak{gl}(V)$ et $n$ un idéal de $g$. Alors $n$ et $e(n)$ sont des idéaux de $e(g)$, et l’on a $[e(g), e(n)] = [g, n]$*.

Soit $g_1$ l’ensemble des $x \in \mathfrak{gl}(V)$ tels que $[x, n] \subset [g, n]$. C’est une sous-algèbre de Lie scindable de $\mathfrak{gl}(V)$, contenant $g$ donc $e(g)$, cf. n° 1, prop. 3 ; autrement dit, $[e(g), n] \subset [g, n]$. Soit $n_1$ l’ensemble des $y \in gl(V)$ tels que
$$
[e(g), y] \subset [g, n].
$$
C’est une sous-algèbre de Lie scindable de $gl(V)$ contenant $n$ d’après ce qui précède, donc contenant $e(n)$; autrement dit $[e(g), e(n)] \subset [g, n]$, d’où
$$
[e(g), e(n)] = [g, n].
$$
On en déduit $[e(g), n] \subset [e(g), e(n)] \subset n$, de sorte que $n$ et $e(n)$ sont des idéaux de $e(g)$.

#### Corollaire 1 {#lie-vii-s5-prop-4-cor-1 .statement tag=00WS}

(i) *On a* $D^i g = D^i e(g)$ *pour* $i \geq 1$, *et* $C^i g = C^i e(g)$ *pour* $i \geq 2$.
(ii) *Si* $g$ *est commutative* (resp. *nilpotente*, resp. *résoluble*), *alors* $e(g)$ *est commutative* (resp. *nilpotente*, resp. *résoluble*).
L’assertion (i) résulte de la prop. 4 par récurrence sur $i$ et (ii) résulte de (i).

#### Corollaire 2 {#lie-vii-s5-prop-4-cor-2 .statement tag=00WT}

*Soit* $r$ *le radical de* $g$. *Si* $g$ *est scindable*, $r$ *est scindable*.
En effet, $e(r)$ est un idéal résoluble de $g$ d’après la prop. 4 et le cor. 1, donc $e(r) = r$.

### 3. Décompositions des algèbres scindables

Si $g$ est une sous-algèbre de Lie de $gl(V)$ de radical $r$, l’ensemble des éléments nilpotents de $r$ est un idéal nilpotent de $g$, le plus grand idéal de nilpotence de la représentation identique de $g$ (I, § 5, no 3, cor. 6 du th. 1). Dans ce paragraphe, nous noterons $n_V(g)$ cet idéal. Il contient le radical nilpotent $[g, g] \cap r$ de $g$ (I, § 5, no 3, th. 1).

#### Proposition 5 {#lie-vii-s5-prop-5 .statement tag=00WU}

*Soit* $g$ *une sous-algèbre de Lie nilpotente scindable de* $gl(V)$. *Soit* $t$ *l’ensemble des éléments semi-simples de* $g$. *Alors* $t$ *est une sous-algèbre centrale de* $g$, *et* $g$ *est l’algèbre de Lie produit de* $t$ *et de* $n_V(g)$.
Si $x \in t$, $\operatorname{ad}_g x$ est semi-simple et nilpotent, donc nul, de sorte que $x$ est central dans $g$. Par suite, $t$ est un idéal de $g$, et $t \cap n_V(g) = 0$. Comme $g$ est scindable, on a $g = t + n_V(g)$, d’où la proposition.

#### Proposition 6 {#lie-vii-s5-prop-6 .statement tag=00WV}

*Soit* $g$ *une sous-algèbre de Lie scindable de* $gl(V)$. *Soient* $\mathcal{T}$ *l’ensemble des sous-algèbres commutatives de* $g$ *formées d’éléments semi-simples*, *et* $\mathcal{T}_1$ *l’ensemble des éléments maximaux de* $\mathcal{T}$. *Soit* $\mathcal{H}$ *l’ensemble des sous-algèbres de Cartan de* $g$.
(i) *Pour* $h \in \mathcal{H}$, *soit* $\varphi(h)$ *l’ensemble des éléments semi-simples de* $h$. *Alors* $\varphi(h) \in \mathcal{T}_1$.
(ii) *Pour* $t \in \mathcal{T}_1$, *soit* $\psi(t)$ *le commutant de* $t$ *dans* $g$. *Alors* $\psi(t) \in \mathcal{H}$.
(iii) *Les applications* $\varphi$ *et* $\psi$ *sont des bijections réciproques de* $\mathcal{H}$ *sur* $\mathcal{T}_1$ *et de* $\mathcal{T}_1$ *sur* $\mathcal{H}$.
(iv) *Si* $k$ *est algébriquement clos*, $\operatorname{Aut}_e(g)$ *opère transitivement dans* $\mathcal{T}_1$.
Soit $h \in \mathcal{H}$, et posons $t = \varphi(h)$. D’après la prop. 5 et le cor. 2 de la prop. 3, on a $t \in \mathcal{T}$ et $\mathfrak{h} = t \times n_V(\mathfrak{h})$. Pour toute sous-algèbre $u$ de $g$, notons encore $\psi(u)$ le commutant de $u$ dant $g$. Alors $\mathfrak{h} \subset \psi(t)$, et $\psi(t) \subset g^0(\mathfrak{h})$ puisque les éléments de $n_V(\mathfrak{h})$ sont nilpotents, donc $\mathfrak{h} = \psi(t)$. Si $t' \in \mathcal{T}$ et $t \subset t'$, on a $t' \subset \psi(t) = \mathfrak{h}$ d’où $t' = t$, de sorte que $t \in \mathcal{T}_1$.

Soit $t \in \mathcal{T}_1$, et posons $c = \psi(t)$. Soit $\mathfrak{h}$ une sous-algèbre de Cartan de $c$. D’après le § 2, no 3, prop. 10, on a $\mathfrak{h} \in \mathcal{H}$ et $t \subset \mathfrak{h}$. Posons $t_1 = \varphi(\mathfrak{h}) \in \mathcal{T}$. On a $t \subset t_1$ donc $t = t_1$, et $\mathfrak{h} = \psi(t_1) = \psi(t) = c$ d’après ce qui précède. Ainsi, $\psi(t) \in \mathcal{H}$, et $\varphi(\psi(t)) = t$.

On a donc prouvé (i), (ii), (iii). Supposons $k$ algébriquement clos. Comme $\mathrm{Aut}_e(g)$ opère transitivement sur $\mathcal{H}$ ($§ 3$, no 2, th. 1), $\mathrm{Aut}_e(g)$ opère transitivement sur $\mathcal{T}_1$.

#### Corollaire 1 {#lie-vii-s5-prop-6-cor-1 .statement tag=00WW}

*Les sous-algèbres de Cartan de $g$ sont les centralisateurs des éléments réguliers semi-simples de $g$*.

Si $x \in g$ est régulier, $g^0(x)$ est une sous-algèbre de Cartan de $g$ ($§ 2$, no 3, th. 1 (i)); si en outre $x$ est semi-simple, $g^0(x)$ est le centralisateur de $x$ dans $g$. Réciproquement, soit $\mathfrak{h}$ une sous-algèbre de Cartan de $g$. Il existe $t \in \mathcal{T}_1$, tel que $\mathfrak{h} = \psi(t)$. D’après le $§ 1$, no 2, prop. 7, il existe $x \in t$ tel que $\mathfrak{h} = g^0(x)$; puisque $x \in t$, on a $g^0(x) = g_0(x)$. Alors $x$ est régulier ($§ 3$, no 3, th. 2 (ii)).

#### Corollaire 2 {#lie-vii-s5-prop-6-cor-2 .statement tag=00WX}

*Supposons en outre que $g$ soit résoluble. Alors*:

(i) *Le sous-groupe de $\mathrm{Aut}(g)$ formé des $e^{\mathrm{ad}\,x}$, $x \in \mathcal{C}^\infty g$ (cf. $§ 3$, no 4), opère transitive-ment dans $\mathcal{T}_1$.

(ii) *Si $t \in \mathcal{T}_1$, $g$ est produit semi-direct de $t$ et de $n_V(g)$*.

L’assertion (i) résulte de ce que le groupe des $e^{\mathrm{ad}\,x}$, $x \in \mathcal{C}^\infty g$, opère transitive-ment dans $\mathcal{H}$ ($§ 3$, no 4, th. 3).

Prouvons (ii). Soit $t \in \mathcal{T}_1$, et soit $\mathfrak{h} = \psi(t)$ la sous-algèbre de Cartan correspondante de $g$. Vu la prop. 5, on a $\mathfrak{h} = t + n_V(\mathfrak{h}) \subset t + n_V(g)$. On a d’autre part $g = \mathfrak{h} + [\mathfrak{g}, \mathfrak{g}]$ ($§ 2$, no 1, cor. 3 de la prop. 4) et $[\mathfrak{g}, \mathfrak{g}] \subset n_V(g)$, d’où $g = t + n_V(g)$. D’autre part, il est clair que $t \cap n_V(g) = \{0\}$. L’algèbre $g$ est donc bien produit semi-direct de $t$ par l’idéal $n_V(g)$.

#### Proposition 7 {#lie-vii-s5-prop-7 .statement tag=00WY}

*Soit $g$ une sous-algèbre de Lie scindable de $\mathrm{gl}(V)$*.

(i) *Il existe une sous-algèbre de Lie $m$ de $g$, réductive dans $\mathrm{gl}(V)$, telle que $g$ soit produit semi-direct de $m$ et de $n_V(g)$*.

(ii) *Deux sous-algèbres de Lie de $g$ ayant les propriétés de (i) sont conjuguées par $\mathrm{Aut}_e(g)$*.

Le radical $r$ de $g$ est scindable (no 2, cor. 2 de la prop. 4). D’après le cor. 2 à la prop. 6, il existe une sous-algèbre commutative $t$ de $r$, formée d’éléments semi-simples, telle que $r = t \oplus n_V(r)$. Comme $\mathrm{ad}_g t$ est formée d’éléments semi-simples, $g$ est somme directe de $[t, g]$ et du centralisateur $\mathfrak{s}$ de $t$ (I, $§ 3$, no 5, prop. 6). Comme $[t, g] \subset r$, on a $g = \mathfrak{s} + r$. Par suite, si $s$ est une sous-algèbre de Levi de $\mathfrak{z}$ (I, § 6, n° 8), on a $g = s + r$, de sorte que $s$ est une sous-algèbre de Levi de $g$. Posons $m = s \oplus t$. Comme $[s, t] = \{0\}$, $m$ est une sous-algèbre de Lie de $g$, réductive dans $\mathrm{gl}(V)$ d’après I, § 6, n° 5, th. 4. En outre,

$$
g = s \oplus r = s \oplus t \oplus n_V(r) = s \oplus t \oplus n_V(g) = m \oplus n_V(g)
$$

puisque $n_V(g) = n_V(r)$. D’où (i).

Soit maintenant $m'$ une sous-algèbre de Lie de $g$ supplémentaire de $n_V(g)$ et réductive dans $\mathrm{gl}(V)$. Montrons que $m'$ est conjuguée de $m$ par $\mathrm{Aut}_e(g)$. On a $m' = s' \oplus t'$ où $s' = [m', m']$ est semi-simple, et où le centre $t'$ de $m'$ est formé d’éléments semi-simples. Alors $r = t \oplus n_V(g) = t' \oplus n_V(g)$. Compte tenu du cor. 2 à la prop. 6, on est ramené au cas où $t = t'$. Alors $s' \subset \mathfrak{z}$; comme $\dim s' = \dim s$, $s'$ est une sous-algèbre de Levi de $\mathfrak{z}$. D’après I, § 6, n° 8, th. 5, il existe $x \in n_V(\mathfrak{z})$ tel que $e^{\mathrm{ad}\, x}(s) = s'$; comme $x$ commute à $t$, on a en même temps $e^{\mathrm{ad}\, x}(t) = t$.

### 4. Algèbres de Lie linéaires d’endomorphismes nilpotents

#### Lemme 1 {#lie-vii-s5-lem-1 .statement tag=00WZ}

Soient $n$ une sous-algèbre de Lie de $\mathrm{gl}(V)$ formée d’endomorphismes nilpotents, et $N$ le sous-groupe $\exp n$ de $\mathbf{GL}(V)$ (§ 3, n° 1, lemme 1).

(i) Soient $\rho$ une représentation linéaire de dimension finie de $n$ dans $W$, telle que les éléments de $\rho(n)$ soient nilpotents, $W'$ un sous-espace vectoriel de $W$ stable pour $\rho, \rho_1$ et $\rho_2$ la sous-représentation et la représentation quotient de $\rho$ définies par $W'$, $\pi, \pi_1, \pi_2$ les représentations de $N$ compatibles avec $\rho, \rho_1, \rho_2$ (§ 3, n° 1). Alors $\pi_1, \pi_2$ sont la sous-représentation et la représentation quotient de $\pi$ définies par $W'$.

(ii) Soient $\rho_1, \rho_2$ des représentations linéaires de dimension finie de $n$ telles que les éléments de $\rho_1(n)$ et de $\rho_2(n)$ soient nilpotents, et $\pi_1, \pi_2$ les représentations de $N$ compatibles avec $\rho_1, \rho_2$. Alors $\pi_1 \otimes \pi_2$ est la représentation de $N$ compatible avec $\rho_1 \otimes \rho_2$.

(iii) Soient $\rho_1, \rho_2$ des représentations linéaires de dimension finie de $n$ dans des espaces vectoriels $V_1, V_2$, telles que les éléments de $\rho_1(n)$ et de $\rho_2(n)$ soient nilpotents, $\rho$ la représentation de $n$ dans $\mathrm{Hom}(V_1, V_2)$ déduite de $\rho_1, \rho_2$. Soient $\pi_1, \pi_2$ les représentations de $N$ compatibles avec $\rho_1, \rho_2$, et $\pi$ la représentation de $N$ dans $\mathrm{Hom}(V_1, V_2)$ déduite de $\pi_1, \pi_2$. Alors $\pi$ est la représentation de $N$ compatible avec $\rho$.

L’assertion (i) est évidente. Soient $\rho_1, \rho_2, \pi_1, \pi_2$ comme dans (ii). Si $x \in n$, on a, puisque $\rho_1(x) \otimes 1$ et $1 \otimes \rho_2(x)$ commutent,

$$
\exp(\rho_1(x) \otimes 1 + 1 \otimes \rho_2(x)) = \exp(\rho_1(x) \otimes 1) \cdot \exp(1 \otimes \rho_2(x))
= (\exp \rho_1(x)) \otimes 1 \cdot 1 \otimes (\exp \rho_2(x))
= (\exp \rho_1(x)) \otimes (\exp \rho_2(x))
= \pi_1(\exp x) \otimes \pi_2(\exp x)
= (\pi_1 \otimes \pi_2)(\exp x)
$$

d’où (ii). Soient $\rho_1, \rho_2, \rho, \pi_1, \pi_2, \pi, V_1, V_2$ comme dans (iii). Si $v_1 \in \mathrm{End}\, V_1$ et v_2 \in \mathrm{End}\ V_2$, notons $ R_{v_1}, L_{v_2} $ les applications $ u \mapsto uv_1, u \mapsto v_2u $ de $ \mathrm{Hom}(V_1, V_2) $ dans lui-même; ces applications commutent et $ \rho(x)u = (L_{\rho_2(x)} - R_{\rho_1(x)})u $, donc
$$
\exp \rho(x) \cdot u = \exp L_{\rho_2(x)} \cdot \exp R_{-\rho_1(x)} \cdot u \\
= L_{\exp \rho_2(x)} \cdot R_{\exp(-\rho_1(x))} \cdot u \\
= L_{\pi_2(\exp x)} \cdot R_{\pi_1(\exp(-x))} \cdot u \\
= \pi(\exp x) \cdot u
$$
d'où (iii).

**Lemme 2.1.** — (i) *Soient W un sous-espace vectoriel de V de dimension d*, D la droite $ \wedge^d W \subset \wedge^d V $, $ \theta $ la représentation canonique de $ \mathfrak{gl}(V) $ dans $ \wedge V $ (**III**, App.). *Soit* $ x \in \mathfrak{gl}(V) $. *Alors* $ x(W) \subset W $ *si et seulement si* $ \theta(x)(D) \subset D $.

(ii) *Soient* $ (e_1, \ldots, e_n) $ *la base canonique de* $ k^n $, $ \theta $ *la représentation canonique de* $ \mathfrak{gl}(n, k) $ *dans* $ \wedge(k^n) $, *et* $ x \in \mathfrak{gl}(n, k) $. *Alors* $ x \in \mathfrak{n}(n, k) $ *si et seulement si*
$$
\theta(x)(e_{n-d+1} \wedge \cdots \wedge e_n) = 0
$$
*pour* $ 1 \leq d \leq n $.

(i) Si $ x(W) \subset W $, il est clair que $ \theta(x)D \subset D $. Inversement, supposons que $ \theta(x)D \subset D $. Soit $ u $ un élément non nul de $ D $ et soit $ y \in W $. On a $ y \wedge u = 0 $. Puisque $ \theta(x) $ est une dérivation de $ \wedge V $, ceci entraîne
$$
\theta(x)y \wedge u + y \wedge \theta(x)u = 0.
$$
Or $ \theta(x)u \in ku $, d'où $ y \wedge \theta(x)u = 0 $ et par suite $ \theta(x)y \wedge u = 0 $. D'après A, III, p. 89, prop. 13, cela entraîne $ \theta(x)y \in W $, i.e. $ x(y) \in W $, ce qui prouve bien que $ x(W) \subset W $.

(ii) La condition énoncée en (ii) est évidemment nécessaire pour que $ x \in \mathfrak{n}(n, k) $. Supposons qu'elle soit vérifiée. D'après (i), $ x $ laisse stable
$$
ke_{n-d+1} + \cdots + ke_n,
$$
et cela pour $ d = 1, \ldots, n $, donc $ x $ est triangulaire inférieure. Posons
$$
x = (x_{ij})_{1 \leq i, j \leq n}.
$$
On a $ 0 = x(e_n) = x_{nn}e_n $, donc $ x_{nn} = 0 $. Soit $ i < n $, et supposons prouvé que $ x_{jj} = 0 $ pour $ j > i $. Alors
$$
0 = \theta(x)(e_i \wedge e_{i+1} \wedge \cdots \wedge e_n) = x_{ii}(e_i \wedge e_{i+1} \wedge \cdots \wedge e_n),
$$
donc $ x_{ii} = 0 $. On voit ainsi que $ x \in \mathfrak{n}(n, k) $.

#### Proposition 8 {#lie-vii-s5-prop-8 .statement tag=00X0}

*Soient n une sous-algèbre de Lie de* $ \mathfrak{gl}(V) $ *formée d’éléments nilpotents, q le normalisateur de n dans* $ \mathfrak{gl}(V) $. *Il existe un espace vectoriel E de dimension finie, une représentation* $ \rho $ *de* $ \mathfrak{gl}(V) $ *dans* E, *et un sous-espace vectoriel F de* E, *vérifiant les conditions suivantes*:
(i) *l’image par* $ \rho $ *d’une homothétie de* V *est diagonalisable*;

1 Dans ce lemme, k peut être un corps commutatif quelconque.

(ii) F est stable par $\rho(q)$;
(iii) n est l’ensemble des $x \in \mathfrak{gl}(V)$ tels que $\rho(x)(F) = 0$.

Soit $n = \dim V$. D’après le th. d’Engel, on peut identifier V à $k^n$ de telle sorte que $n \subset n(n, k)$. Soit P l’algèbre des fonctions polynomiales sur $\mathfrak{gl}(n, k)$. Pour $i = 0, 1, \ldots$, soit $P_i$ l’ensemble des éléments de P homogènes de degré $i$. Soit N = exp n, qui est un sous-groupe du groupe trigonal strict inférieur T. Soit J l’ensemble des éléments de P qui sont nuls sur N ; c’est un idéal de P. Soit $N_J$ l’ensemble des $x \in \mathfrak{gl}(n, k)$ tels que $p(x) = 0$ pour tout $p \in J$. On a $N \subset N_J$. Inversement, soit $x \in N_J$. Notons $p_{ij}$ les fonctions polynomiales donnant les composantes d’un élément de $\mathfrak{gl}(n, k)$. L’idéal J contient les $p_{ij}$ (pour $i < j$) et les $p_{ii} - 1$; on a donc $x \in T$. D’autre part, si $u$ est une forme linéaire sur $\mathfrak{gl}(n, k)$ nulle sur n, il existe $p_u \in P$ tel que $p_u(z) = u(\log z)$ pour tout $z \in T$ (§ 3, no 1, lemme 1 (i)); on a $p_u \in J$, d’où $u(\log x) = 0$. On en déduit que $\log x$ appartient à n, d’où $x \in N$, ce qui prouve que $N = N_J$.

Pour tout $p \in P$ et $g \in \mathbf{GL}_n(k)$, soit $\lambda(g)p$ la fonction $x \mapsto p(g^{-1}x)$ sur $\mathfrak{gl}(n, k)$; on a $\lambda(g)p \in P$, $\lambda(g)$ est un automorphisme de l’algèbre P, et $\lambda$ est une représentation de $\mathbf{GL}_n(k)$ dans P qui laisse stable chaque $P_i$. Montrons que

(1)
$$
N = \{ x \in \mathbf{GL}_n(k) \mid \lambda(x)J = J \}.
$$

Si $x \in N$, $p \in J$, $y \in N$, on a $(\lambda(x)p)(y) = p(x^{-1}y) = 0$ puisque $x^{-1}y \in N$; donc $\lambda(x)p \in J$, de sorte que $\lambda(x)J = J$. Soit $x \in \mathbf{GL}_n(k)$ tel que $\lambda(x)J = J$; soit $p \in J$; on a $p(x^{-1}) = (\lambda(x)p)(e) = 0$, donc $x^{-1} \in N_J = N$ et $x \in N$. Cela prouve (1).

L’idéal J est de type fini (AC, III, § 2, no 10, cor. 2 du th. 2). Il existe donc un entier q tel que, si $W = P_0 + P_1 + \cdots + P_q$, alors $J \cap W$ engendre J comme idéal. Notons $\lambda_j$ (resp. $\lambda'$) la sous-représentation de $\lambda$ définie par $P_j$ (resp. par W). D’après (1), on a:

(2)
$$
N = \{ x \in \mathbf{GL}_n(k) \mid \lambda'(x)(J \cap W) = J \cap W \}.
$$

Montrons que, pour tout $j$, il existe une représentation $\sigma_j$ de l’algèbre de Lie $\mathfrak{gl}(n, k)$ dans $P_j$, telle que:

(3)
$$
\sigma_j|_{n(n, k)} \text{ est compatible } (§ 3, \text{no } 1) \text{ avec } \lambda_j|T.
$$
(4)
Pour tout $x \in k.l_n$, $\sigma_j(x)$ est une homothétie.

Comme $\lambda_j$ est la puissance symétrique $j$-ième de $\lambda_1$, il suffit de montrer l’existence de $\sigma_1$, cf. lemme 1. Or $\lambda_1$ est la représentation contragrédiente de la représentation $\gamma$ de $\mathbf{GL}_n(k)$ dans $\mathfrak{gl}(n, k)$ donnée par
$$
\gamma(x)y = xy, \quad x \in \mathbf{GL}_n(k), \quad y \in \mathfrak{gl}(n, k).
$$
Soit c la représentation de l’algèbre de Lie $\mathfrak{gl}(n, k)$ dans $\mathfrak{gl}(n, k)$ donnée par
$$
c(x)y = xy, \quad x, y \in \mathfrak{gl}(n, k).
$$
On vérifie aussitôt que $c|_{n(n, k)}$ et $\gamma|T$ sont compatibles, et que $c(x)$ est une homothétie pour tout $x \in k . 1_n$. Il suffit alors de prendre pour $\sigma_1$ la représentation duale de $c$ (I, § 3, n° 3).

Soit maintenant $\sigma'$ la représentation de $\mathfrak{gl}(n, k)$ dans $W$ somme directe des $\sigma_j, 0 \leq j \leq q$. Vu (2), et les relations
$$
\lambda'(\exp(x)) = \exp(\sigma'(x)) \quad \text{et} \quad \sigma'(\log(y)) = \log(\lambda'(y)), \quad x \in n(n, k), \quad y \in T,
$$
on a
$$
n = \{ x \in n(n, k) \mid \sigma'(x)(J \cap W) \subset J \cap W \}.
$$
(5)
Soit $d = \dim(J \cap W)$, et soit $\tau = \wedge^d \sigma'$. Soit $D = \wedge^d(J \cap W)$. D’après (5) et le lemme 2 (i), on a
$$
n = \{ x \in n(n, k) \mid \tau(x)(D) \subset D \}.
$$
(6)
Mais $\tau(n(n, k))$ est formé d’endomorphismes nilpotents, donc (6) peut aussi s’écrire
$$
n = \{ x \in n(n, k) \mid \tau(x)(D) = 0 \}.
$$
(7)
Soit alors $E = \wedge^d W \oplus \wedge^1 V \oplus \wedge^2 V \oplus \cdots \oplus \wedge^n V$; soit $\rho$ la somme directe de $\tau$ et des représentations canoniques de $\mathfrak{gl}(n, k)$ dans $\wedge^1 V, \ldots, \wedge^n V$. Soit $E_0 \subset E$ la somme de $D = \wedge^d(J \cap W)$ et des droites engendrées par $e_{n-j+1} \wedge \cdots \wedge e_n$ pour $j = 1, \ldots, n$. D’après (7) et le lemme 2 (ii), on a
$$
n = \{ x \in \mathfrak{gl}(V) \mid \rho(x)(E_0) = 0 \}.
$$
(8)
Il est immédiat que, si $x \in k . 1$, $\rho(x)$ est diagonalisable. Enfin, si $F$ est l’ensemble des éléments de $E$ annulés par $\rho(n)$, $F$ est stable par $\rho(q)$ (I, § 3, n° 5, prop. 5), et l’on a, d’après (8),
$$
n = \{ x \in \mathfrak{gl}(V) \mid \rho(x)(F) = 0 \}.
$$
(9)

### 5. Caractérisations des algèbres de Lie scindables

Toute algèbre de Lie scindable est engendrée comme espace vectoriel (et $a$ fortiori comme algèbre de Lie) par l’ensemble de ses éléments qui sont, soit semi-simples, soit nilpotents. Inversement:

#### Théorème 1 {#lie-vii-s5-thm-1 .statement tag=00X1}

Soit $g$ une sous-algèbre de Lie de $\mathfrak{gl}(V)$ et soit $X$ une partie de $g$ engendrant $g$ comme $k$-algèbre de Lie. Si tout élément de $X$ est, soit semi-simple, soit nilpotent, $g$ est scindable.

a) $g$ est commutative.
Les éléments semi-simples (resp. nilpotents) de $g$ forment un sous-espace vectoriel $g_s$ (resp. $g_n$). L’hypothèse équivaut à $g = g_s \oplus g_n$, d’où le fait que $g$ est scindable.

b) $g$ est réductive.

Alors $g = g' \times c$ avec $g'$ semi-simple et $c$ commutative. D’après la prop. 2, $g'$ est scindable. Soit $x = a + b \in g$ avec $a \in g',\ b \in c$. Soient $a_s,\ a_n,\ b_s,\ b_n$ les composantes semi-simples et nilpotentes de $a,\ b$. Comme $a_s,\ a_n,\ b_s,\ b_n$ commutent deux à deux, les composantes semi-simple et nilpotente de $x$ sont $a_s + b_s,\ a_n + b_n$. Or $a_s,\ a_n \in g'$. Si $x$ est semi-simple, on a $x = a_s + b_s$; comme $a_s$ appartient à $g'$, on a $b_s \in g$, d’où $b_s \in c$ puisque $b_s$ commute à $g$; par suite, $a = a_s$ et $b = b_s$. De même, si $x$ est nilpotent, on a $a = a_n$ et $b = b_n$. Il en résulte que les projections sur $c$ des éléments de $X$ sont, soit semi-simples, soit nilpotentes; d’après a), cela entraîne que $c$ est scindable. Reprenant les notations précédentes, mais sans hypothèse sur $x$, on a maintenant $b_s,\ b_n \in c$, donc $a_s + b_s,\ a_n + b_n \in g$, ce qui prouve le théorème dans ce cas.

c) Cas général.

Supposons le théorème démontré pour les algèbres de Lie de dimension < dim $g$ et démontrons-le pour $g$.

Soit $n$ le plus grand idéal de nilpotence de la représentation identique de $g$. Si $n = 0$, $g$ admet une représentation semi-simple injective, donc est réductive. Supposons $n \neq 0$. Soit $p$ le normalisateur de $n$ dans $gl(V)$. Il existe $E,\ \rho,\ F$ vérifiant les conditions de la prop. 8. Puisque $g \subset p,\ \rho(g)$ laisse $F$ stable; soit $\rho_0$ la représentation $u \mapsto \rho(u)|F$ de $g$ dans $F$; on a $n = \mathrm{Ker}\ \rho_0$. Tout élément semi-simple (resp. nilpotent) de $gl(V)$ a pour image par $\rho$ un élément semi-simple (resp. nilpotent) (prop. 2). L’algèbre $\rho_0(g)$ est donc engendrée par des éléments qui sont soit semi-simples, soit nilpotents. D’après l’hypothèse de récurrence, $\rho_0(g)$ est scindable.

Soient $x \in g$, et $x_s,\ x_n$ ses composantes semi-simple et nilpotente. D’après la prop. 2, les composantes semi-simple et nilpotente de $\rho(x)$ sont $\rho(x_s),\ \rho(x_n)$. Comme $\rho_0(g)$ est scindable, il existe $y,\ z \in g$ tels que

$$
\rho_0(y) = \rho(x_s)|F \qquad \rho_0(z) = \rho(x_n)|F.
$$

Alors $x_s \in y + n,\ x_n \in z + n$, donc $x_s,\ x_n \in g$.

C.Q.F.D.

#### Corollaire 1 {#lie-vii-s5-thm-1-cor-1 .statement tag=00X2}

Toute sous-algèbre de $gl(V)$ engendrée par des sous-algèbres scindables est scindable.

C’est clair.

#### Corollaire 2 {#lie-vii-s5-thm-1-cor-2 .statement tag=00X3}

Soit $g$ une sous-algèbre de Lie de $gl(V)$. Alors $[g,\ g]$ est scindable.

Soient $r$ le radical de $g,\ s$ une sous-algèbre de Levi de $g$ (I, § 6, no 8). On a

$$
[g,\ g] = [s,\ s] + [s,\ r] + [r,\ r] = s + [g,\ r].
$$

L’algèbre $[g,\ r]$ est scindable puisque tous ses éléments sont nilpotents (I, § 5, no 3). D’autre part, $s$ est scindable (prop. 2). Il en résulte que $[g,\ g]$ est scindable (cor. 1).

#### Corollaire 3 {#lie-vii-s5-thm-1-cor-3 .statement tag=00X4}

Soit $g$ une sous-algèbre de Lie de $\mathrm{gl}(V)$, et soit $X$ une partie de $g$ engendrant $g$ (comme k-algèbre de Lie).

(i) L’enveloppe scindable $e(g)$ de $g$ est engendrée par les composantes semi-simples et nilpotentes des éléments de $X$.

(ii) Si $k'$ est une extension de $k$, on a $e(g \otimes_k k') = e(g) \otimes_k k'$; pour que $g$ soit scindable, il faut et il suffit que $g \otimes_k k'$ le soit.

Soit $\tilde{g}$ la sous-algèbre de $\mathrm{gl}(V)$ engendrée par les composantes semi-simples et nilpotentes des éléments de $X$. On a $g \subset \tilde{g} \subset e(g)$; d’après le th. 1, $\tilde{g}$ est scindable, d’où $\tilde{g} = e(g)$, ce qui démontre (i). L’assertion (ii) en résulte, compte tenu de ce que $X$ engendre la $k'$-algèbre $g \otimes_k k'$.

#### Corollaire 4 {#lie-vii-s5-thm-1-cor-4 .statement tag=00X5}

Soit $g$ une sous-algèbre de Lie scindable de $\mathrm{gl}(V)$. Soit $\mathcal{T}$ l’ensemble des sous-algèbres commutatives de $g$ formées d’éléments semi-simples (cf. prop. 6). Les éléments maximaux de $\mathcal{T}$ ont tous même dimension.

Soient $k'$ une extension algébriquement close de $k$ et $V' = V \otimes_k k'$, $g' = g \otimes_k k'$. Soient $t_1, t_2$ des éléments maximaux de $\mathcal{T}$, $t_i' = t_i \otimes_k k'$, $h_i$ le commutant de $t_i$ dans $g$, $h_i' = h_i \otimes_k k'$. Alors $h_i'$ est une sous-algèbre de Cartan de $g'$ (prop. 6) donc $h_i'$ est une sous-algèbre de Cartan de $g'$. On a $h_i = t_i \times n_V(h_i)$, donc $h_i' = t_i' \times n_{V'}(h_i')$, de sorte que $t_i'$ est l’ensemble des éléments semi-simples de $h_i'$. Comme $g'$ est scindable (cor. 3), $t_1'$ et $t_2'$ sont conjugués par $\mathrm{Aut}_e(g')$ (prop. 6), de sorte que $\dim t_1 = \dim t_2$.

#### Théorème 2 {#lie-vii-s5-thm-2 .statement tag=00X6}

Soit $g$ une sous-algèbre de Lie de $\mathrm{gl}(V)$. Les conditions suivantes sont équivalentes:

(i) $g$ est scindable;
(ii) toute sous-algèbre de Cartan de $g$ est scindable;
(iii) $g$ possède une sous-algèbre de Cartan scindable;
(iv) le radical de $g$ est scindable.

(i) $\Rightarrow$ (ii): Cela résulte du cor. 2 à la prop. 3.
(ii) $\Rightarrow$ (i): Cela résulte du cor. 1 au th. 1, puisque $g$ est engendrée par ses sous-algèbres de Cartan (§ 2, no 3, cor. 3 au th. 1).
(ii) $\Rightarrow$ (iii): C’est évident.
(iii) $\Rightarrow$ (ii): D’après le cor. 3 au th. 1, on peut supposer $k$ algébriquement clos. Les sous-algèbres de Cartan de $g$ sont alors conjuguées par les automorphismes élémentaires de $g$ (§ 3, no 2, th. 1); vu la remarque 1 du § 3, no 1, il en résulte que, si l’une d’elles est scindable, toutes le sont.
(i) $\Rightarrow$ (iv): Cela résulte du cor. 2 de la prop. 4.
(iv) $\Rightarrow$ (i): Supposons que le radical $r$ de $g$ soit scindable. Soit $s$ une sous-algèbre de Levi de $g$; elle est scindable (prop. 2). Donc $g = s + r$ est scindable (cor. 1 du th. 1).

## EXERCICES {#lie-vii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
