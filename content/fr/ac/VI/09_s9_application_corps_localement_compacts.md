---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: Valuations
section: 9
section_title: 'Application : corps localement compacts'
lang: fr
source: ac-v-vii-fr
pdf_pages: 0151-0156, 0191-0193
extraction: ocr
subsections:
    - "no": 1
      title: Fonction module sur un corps localement compact.
      page: 0
      pdf_page: 151
    - "no": 2
      title: Existence de représentants.
      page: 0
      pdf_page: 153
    - "no": 3
      title: Structure des corps localement compacts.
      page: 0
      pdf_page: 154
statements: 10
exercises: 5
content_sha256: 61fb6b833d5460050c69f490fe5ccf382187a4e3b04c1d94954fce65913a3c43
---

## § 9. Application : corps localement compacts.

### 1. Fonction module sur un corps localement compact.

Soit K un corps localement compact (non nécessairement commutatif). Rappelons que l’on a défini (Intégr., chap. VII,

#### Proposition 1 {#ac-vi-s9-prop-1 .statement}

Si K est un corps localement compact, la fonction mod_K appartient à $\mathcal{V}(K)$ (§ 6, no 1). En outre :
(i) Si s > 0 est tel que $(\mathrm{mod}_K)^s = g$ soit une valeur absolue, alors g définit la topologie de K.
(ii) Si K est non discret et si mod_K est une valeur absolue ultramétrique, il existe une valuation discrète normée $\nu$ sur K, dont l’anneau est compact et le corps résiduel fini à q éléments, de sorte que $\mathrm{mod}_K = q^{-\nu}$. La topologie de K est définie par $\nu$.
Cela résulte du § 6, no 1, prop. 1, du § 5, no 1, prop. 2 et d’Intégr., chap. VII, § 1, no 10, prop. 12 et 13.

#### Proposition 2 {#ac-vi-s9-prop-2 .statement}

Soient K, K' deux corps localement compacts (non nécessairement commutatifs) tels que K soit un sous-corps topologique de K' et que K soit non discret. Alors :
(i) K' est un espace vectoriel à gauche (resp. à droite) de dimension finie sur K.
(ii) Si K est contenu dans le centre de K', on a, pour tout $x \in K'$
$$
\mathrm{mod}_{K'}(x) = \mathrm{mod}_K(\mathrm{N}_{K'/K}(x)).
$$
En effet, comme K est un corps valué complet non discret, l’assertion (i) résulte de Esp. vect. top., chap. I, § 2, no 4, th. 3; l’assertion (ii) n’est autre que Intégr., chap. VII, § 1, no 11, prop. 17.

#### Corollaire 1 {#ac-vi-s9-prop-2-cor-1 .statement}

Tout corps localement compact dont le centre est non discret est de rang fini sur son centre.
En effet, le centre Z d’un corps localement compact K est fermé dans K, donc localement compact.

#### Corollaire 2 {#ac-vi-s9-prop-2-cor-2 .statement}

Soient K' un corps localement compact et K un sous-corps fermé de K' (non nécessairement commutatifs). Si K' est un espace vectoriel à gauche (resp. à droite) de dimension finie n sur K, on a
$$
\mathrm{mod}_{K'}(x) = (\mathrm{mod}_K(x))^n \text{ pour tout } x \in K.
$$
En effet, de façon générale, on sait que dans un espace vectoriel (à gauche ou à droite) de dimension finie $n$ sur $K$, l’homothétie de rapport $x \in K$ a un module égal à $(\mathrm{mod}_K(x))^n$; il suffit d’appliquer cela à $K'$.

### 2. Existence de représentants.

#### Proposition 3 {#ac-vi-s9-prop-3 .statement}

Soit $K$ un corps (non nécessairement commutatif) localement compact non discret dont la topologie soit définie par une valuation discrète $\nu$; soient $A$ l’anneau et $m$ l’idéal de $\nu$, et posons $\mathrm{Card}(A/m) = q = p^f$ (p premier). Alors, il existe un système de représentants $S$ de $A/m$ dans $A$ et une uniformisante $u$ pour $\nu$, tels que $0 \in S$, que $S^* = S \cap K^*$ soit un sous-groupe cyclique de $K^*$ et que $u^{-1}Su = S$. En outre, tout élément de $A$ s’écrit d’une seule manière sous la forme $\sum_{i=0}^\infty s_i u^i$, où $s_i \in S$.

Nous utiliserons le lemme suivant :

#### Lemme 1 {#ac-vi-s9-lem-1 .statement}

Soient $x, y$ deux éléments permutables de $A$ tels que $x - y \in m^j (j \geq 1)$; alors $x^{p^n} - y^{p^n} \in m^{j+n}$ pour tout entier $n \geq 0$.

Par récurrence sur $n$, on se ramène à prouver le lemme pour $n = 1$. Alors $x^p - y^p = (x - y)(x^{p-1} + x^{p-2}y + \cdots + y^{p-1})$; le second facteur est une somme de $p$ termes, deux à deux congrus mod. $m$, et comme $A/m$ est de caractéristique $p$, on a $p.1 \in m$ dans $A$, donc on a $x^{p-1} + x^{p-2}y + \cdots + y^{p-1} \in m$; d’où $x^p - y^p \in m^{j+1}$.

On sait que le groupe multiplicatif $(A/m)^*$ est un groupe cyclique ayant $q - 1$ éléments (Alg., chap. V, § 11, no 1, th. 1); soit $x$ un représentant dans $A$ d’un générateur de ce groupe; on a donc $x^q - x \in m$, d’où, en vertu du lemme 1, $x^{q^{n+1}} - x^{q^n} \in m^{1+jn}$, puisque $x^q$ et $x$ sont permutables. Cela prouve que $(x^{q^n})_{n \geq 0}$ est une suite de Cauchy dans $A$; comme $A$ est compact, donc complet, cette suite a une limite $s$ dans $A$, qui est évidemment telle que $s \equiv x$ (mod. $m$) et $s^q = s$. Comme $s \neq 0$, on a $s^{q-1} = 1$, plus précisément $s$ est une racine primitive $(q-1)$-ème de l’unité dans $A$. Il est clair que l’ensemble $S$, formé de $0$ et des puissances $s^j (0 \leq j \leq q-2)$ est un système de représentants des classes de $A$ mod. $m$, et est stable pour la multiplication dans $A$.

Soit maintenant $a$ une uniformisante pour $\nu$, et considérons l’automorphisme intérieur $y \to a^{-1}ya$ de $K$; il transforme $A$ en lui-même, $m$ en lui-même, donc, par passage aux quotients,

Posons
$$
u = \sum_{j=0}^{q-2} s^{-j} a s^{jp^r}.
$$

On a $u \equiv (q - 1)a \equiv -a \ (\mathrm{mod.}\ m^2)$ puisque $p.1 \in m$; on en conclut que $u$ est aussi une uniformisante pour $\varphi$; en outre on a
$$
s^{-1} u s^{p^r} = u
$$
d’où l’on déduit que $u^{-1} S u = S$.

Enfin, pour tout $x \in A$ il existe une suite $(s_i) \quad (i \in \mathbf{N})$ et une seule telle que $s_i \in S$ pour tout $i$ et $x \equiv \sum_{i=0}^n s_i u^i \ (\mathrm{mod.}\ m^{n+1})$ pour tout $n \geq 0$: c’est immédiat par récurrence sur $n$, tout élément $t$ de $m^{n+1}$ vérifiant une relation de la forme $t \equiv t' u^{n+1} \ (\mathrm{mod.}\ m^{n+2})$, où $t'$ est un élément de $S$ déterminé de façon unique. On a donc $x = \sum_{i=0}^\infty s_i u^i$ et la famille $(s_i)$ vérifiant cette relation et telle que $s_i \in S$ pour tout $i$ est déterminée de façon unique.

### 3. Structure des corps localement compacts.

Les complétés $\mathbf{R}$ et $\mathbf{Q}_p$ du corps $\mathbf{Q}$ pour les valeurs absolues non impropres sur $\mathbf{Q}$ ($p$ premier quelconque) sont localement compacts. D’autre part, pour toute puissance $q = p^f$ d’un nombre premier $p$, le corps $\mathbf{F}_q((T))$ des séries formelles sur le corps fini $\mathbf{F}_q$, muni de la valuation définie au § 3, n° 4, Exemple 3, est localement compact : en effet l’idéal maximal de l’anneau de valuation $\mathbf{F}_q[[T]]$ est engendré par $T$; on sait que cet anneau est complet pour la topologie (T)-adique (chap. III, § 2, n° 6, prop. 6) et comme le corps résiduel $\mathbf{F}_q$ est fini, la prop. 2 du § 5, n° 1, prouve notre assertion. Inversement :

#### Théorème 1 {#ac-vi-s9-thm-1 .statement}

Soit $K$ un corps (non nécessairement commutatif) localement compact non discret.

(i) Si K est de caractéristique 0 et si mod_K n’est pas une valeur absolue ultramétrique, alors K est isomorphe à l’un des corps R, C ou H.

(ii) Si K est de caractéristique 0 et si mod_K est une valeur absolue ultramétrique, K est une algèbre de rang fini sur un corps p-adique Q_p.

(iii) Si K est de caractéristique p ≠ 0, il est isomorphe à un corps ayant pour centre un corps de séries formelles F_q((T)) (où q est une puissance de p), et de rang fini sur son centre.

(i) Il résulte du th. d’Ostrowski (§ 6, no 4, th. 2) que K est un corps topologique isomorphe à un sous-corps partout dense de R, C ou H, et comme K est complet il est isomorphe à R, C ou H.

(ii) Soient A l’anneau de la valeur absolue mod_K, m son idéal maximal. On sait que A/m est un corps fini (§ 5, no 1, prop. 2), donc la valeur absolue induite par mod_K sur Q a un corps résiduel fini, ce qui n’est possible que si elle est équivalente à une valeur absolue p-adique (§ 6, no 3, prop. 4); l’adhérence de Q dans K est par suite isomorphe à Q_p et est contenue dans le centre de K puisque ce dernier est fermé dans K; on conclut par la prop. 2 du no 1.

(iii) La seconde assertion résulte de la première et du cor. de la prop. 2 du no 1. Pour démontrer la première assertion, notons que mod_K est nécessairement une valeur absolue ultramétrique (§ 6, no 2, cor. de la prop. 3); avec les notations de la démonstration de la prop. 3 du no 2, le centre Z de K est formé des éléments permutable à la fois à s et à u; mais en vertu de (3), on a u^{-1}s u = s^{p'} d’où

$$
u^{-j} s u^j = s^{{p'}^j} = s,
$$

de sorte que u^q \in Z, et l’on en conclut que Z n’est pas discret. Comme Z est localement compact, on voit qu’on est ramené au cas où K est commutatif. La sous-F_p-algèbre F_p[s] dans K est alors un corps fini puisque s^{q-1} = 1, et l’on a évidemment y^q = y pour tout élément de ce corps, qui est donc identique à S et isomorphe à F_q puisque S \subset F_p[s] a q éléments. La somme de deux éléments de S étant dans S, l’application qui, à toute série formelle

$$
\sum_{i=0}^{\infty} s_i T^i \in F_q[[T]],
$$

fait correspondre l’élément

$$
\sum_{i=0}^{\infty} s_i u^i,
$$

est un homomorphisme bijectif de l’anneau F_q[[T]] sur l’anneau A, d’où aussitôt la conclusion.

#### Corollaire 1 {#ac-vi-s9-thm-1-cor-1 .statement}

Tout corps localement compact non discret est de rang fini sur son centre.

#### Corollaire 2 {#ac-vi-s9-thm-1-cor-2 .statement}

Tout corps localement compact est connexe ou totalement discontinu; s’il est connexe, il est isomorphe à $\mathbf{R}, \mathbf{C}$ ou $\mathbf{H}$.

En effet, si la topologie d’un corps $K$ est définie par une valeur absolue ultramétrique, $K$ est totalement discontinu pour cette topologie.

#### Remarque {#ac-vi-s9-n3-rem-1 .statement}

Soit $s$ un entier $> 0$; le sous-corps $F_q((T^s)) = L$ de $K = F_q((T))$ est fermé dans $K$ et l’on a $e(K/L) = s$ et $f(K/L) = 1$. On voit donc qu’il y a des sous-corps fermés non discrets $L$ de $K$ tels que $e(K/L)$ (et $a fortiori$ le degré $[K : L]$) soit arbitrairement grand (contrairement à ce qui se passe pour les corps localement compacts de caractéristique 0, où tout sous-corps localement compact $L$ d’un tel corps $K$ contient nécessairement $\mathbf{R}$ ou $\mathbf{Q}_p$ et où par suite $[K : L]$ est borné).

## EXERCICES {#ac-vi-s9-exercises}

See the [exercises for § 9](exercises/s9/).
