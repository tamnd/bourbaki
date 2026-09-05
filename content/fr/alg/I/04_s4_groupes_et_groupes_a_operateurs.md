---
book: alg
book_title: Algebra
chapter: I
chapter_title: STRUCTURES ALGÉBRIQUES
section: 4
section_title: Groupes et groupes à opérateurs
lang: fr
source: alg-i-iii-fr
book_pages: A I.28-A I.49, A I.123-A I.129
pdf_pages: 0038-0059, 0133-0139
extraction: ocr
subsections:
    - "no": 1
      title: Groupes
      page: 28
      pdf_page: 38
    - "no": 2
      title: Groupes à opérateurs
      page: 0
      pdf_page: 39
    - "no": 3
      title: Sous-groupes
      page: 31
      pdf_page: 41
    - "no": 4
      title: Groupes quotients
      page: 33
      pdf_page: 43
    - "no": 5
      title: Décomposition d’un homomorphisme
      page: 36
      pdf_page: 46
    - "no": 6
      title: Sous-groupes d’un groupe quotient
      page: 37
      pdf_page: 47
    - "no": 7
      title: Le théorème de Jordan-Hölder
      page: 0
      pdf_page: 49
    - "no": 8
      title: Produits et produits fibrés
      page: 43
      pdf_page: 53
    - "no": 9
      title: Sommes restreintes
      page: 45
      pdf_page: 55
    - "no": 10
      title: Groupes monogènes
      page: 46
      pdf_page: 56
statements: 66
exercises: 26
content_sha256: a711b3ebd89b32c5ea3ea2e1f026589a09b73c0afb90ab9651e4a83e25fe9554
---

## § 4. GROUPES ET GROUPES A OPÉRATEURS

### 1. Groupes

Rappelons la définition suivante (I, p. 15, déf. 6):

#### Définition 1 {#alg-i-s4-def-1 .statement}

On appelle groupe un ensemble muni d’une loi de composition associative, possédant un élément neutre et pour laquelle tout élément est inversible.

Autrement dit, un groupe est un monoïde (I, p. 12, déf. 2) dans lequel tout élément est inversible. Une loi de composition sur un ensemble qui y détermine une structure de groupe est appelée une loi de groupe. Si G et H sont deux groupes, un homomorphisme de magmas de G dans H est encore appelé un homomorphisme de groupes. Un tel homomorphisme f transforme élément neutre en élément neutre; en effet, soit e (resp. e') l’élément neutre de G (resp. H); en notant multiplicativement les lois de groupe de G et H, on a $e.e = e$, d’où $f(e).f(e) = f(e)$ et, en multipliant par $f(e)^{-1}$, on obtient $f(e) = e'$. Par suite f est unifère. Il résulte alors de I, p. 15, que $f(x^{-1}) = f(x)^{-1}$ pour tout $x \in G$.

#### Exemple {#alg-i-s4-n1-exa-1 .statement}

Dans un monoïde quelconque E, l’ensemble des éléments inversibles, muni de la structure induite par celle de E, est un groupe. En particulier, l’ensemble des applications bijectives d’un ensemble F sur lui-même (ou ensemble des permutations de F) est un groupe pour la loi $(f, g) \mapsto f \circ g$, qu’on appelle groupe symétrique de l’ensemble F et qu’on note $\mathcal{S}_F$.

Dans ce paragraphe, sauf indication contraire, nous noterons toujours multiplicativement la loi de composition d’un groupe, et nous désignerons par e l’élément neutre d’une loi de groupe ainsi notée.

Un groupe G est dit fini si l’ensemble sous-jacent à G est fini; sinon il est dit infini; le cardinal d’un groupe est appelé l’ordre du groupe.

Si une loi de composition sur G détermine sur G une structure de groupe, il en est de même de la loi opposée. L’application d’un groupe G sur lui-même qui, à tout $x \in G$, fait correspondre l’inverse de x, est un isomorphisme de G sur le groupe opposé (I, p. 16, prop. 4).

Suivant nos conventions générales (E, II, p. 10), nous désignerons par $A^{-1}$ l’image d’une partie A de G par l’application $x \mapsto x^{-1}$. Mais il importe de noter que, malgré l’analogie des notations, $A^{-1}$ n’est pas en général élément inverse de A pour la loi de composition $(X, Y) \mapsto XY$ entre parties de G (rappelons que XY est l’ensemble des $xy$ pour $x \in X, y \in Y$); en effet, l’élément neutre pour cette loi est $\{e\}$, et les seuls éléments de $\mathfrak{P}(G)$, inversibles pour cette loi, sont les ensembles A réduits à un seul élément (un tel A, d’ailleurs, a bien pour inverse $A^{-1}$). On a l’identité $(AB)^{-1} = B^{-1}A^{-1}$ pour $A \subset G, B \subset G$. On dit que A est une partie symétrique de G si $A = A^{-1}$. Quel que soit $A \subset G$, les parties $A \cup A^{-1}, A \cap A^{-1}$ et $AA^{-1}$ sont symétriques.

### 2. Groupes à opérateurs

#### Définition 2 {#alg-i-s4-def-2 .statement}

Soit $\Omega$ un ensemble. On appelle groupe à opérateurs dans $\Omega$ un groupe G muni d’une action de $\Omega$ dans G distributive par rapport à la loi de groupe.

On notera dans la suite $x^\alpha$ le composé de $\alpha \in \Omega$ et $x \in G$. Là distributivité s’exprime alors par l’identité $(xy)^\alpha = x^\alpha y^\alpha$.

Dans un groupe à opérateurs G, chaque opérateur définit un endomorphisme de la structure de groupe sous-jacente; ces endomorphismes seront parfois appelés les homothéties du groupe à opérateurs G.

On dit qu’un groupe à opérateurs G est commutatif (ou abélien) si sa loi de groupe est commutative.

On identifie dans la suite un groupe G au groupe, à opérateurs dans $\varnothing$, obtenu en munissant G de l’unique action de $\varnothing$ dans G. Cela permet de considérer les groupes comme des cas particuliers de groupes à opérateurs, et de leur appliquer les définitions et résultats relatifs à ces derniers que nous allons énoncer.

#### Exemple {#alg-i-s4-n2-exa-1 .statement}

Dans un groupe commutatif G, noté multiplicativement, on a $(xy)^n = x^n y^n$ quel que soit $n \in \mathbf{Z}$ (I, p. 23); l’action $n \mapsto (x \mapsto x^n)$ de $\mathbf{Z}$ dans G définit par suite, avec la loi du groupe, une structure de groupe à opérateurs sur G.

#### Définition 3 {#alg-i-s4-def-3 .statement}

Soient G et G’ des groupes à opérateurs dans $\Omega$. On appelle homomorphisme de groupes à opérateurs de G dans G’, un homomorphisme du groupe G dans le groupe G’ tel que l’on ait

$$
f(x^\alpha) = (f(x))^\alpha
$$

pour tout $\alpha \in \Omega$ et tout $x \in G$.

Un endomorphisme du groupe à opérateurs G est un endomorphisme du groupe G permutable avec toutes les homothéties de G.

Comme deux homothéties d’un groupe à opérateurs G ne sont pas nécessairement permutables, une homothétie de G n’est pas en général un endomorphisme du groupe à opérateurs G.

L’application identique d’un groupe à opérateurs est un homomorphisme de groupes à opérateurs; le composé de deux homomorphismes de groupes à opérateurs en est un. Pour qu’une application soit un isomorphisme de groupes à opérateurs, il faut et il suffit que ce soit un homomorphisme bijectif de groupes à opérateurs, et l’application réciproque est alors un isomorphisme de groupes à opérateurs.

Plus généralement, soient G (resp. G’) un groupe à opérateurs dans $\Omega$ (resp. $\Omega'$). Soit $\varphi$ une application de $\Omega$ dans $\Omega'$. On appelle $\varphi$-homomorphisme de G dans G’ un homomorphisme du groupe G dans le groupe G’ tel que l’on ait

$$
f(x^{\alpha}) = (f(x))^{\varphi(\alpha)}
$$

pour tout $\alpha \in \Omega$ et tout $x \in G$.

Dans la suite de ce paragraphe, on se donne un ensemble $\Omega$. Sauf mention du contraire, les groupes à opérateurs considérés admettent $\Omega$ pour ensemble d’opérateurs.

### 3. Sous-groupes

#### Définition 4 {#alg-i-s4-def-4 .statement}

Soit G un groupe à opérateurs. On appelle sous-groupe stable de G une partie H de G possédant les propriétés suivantes :
(i) $e \in H$;
(ii) la relation « $x \in H$ et $y \in H$ » implique $x \in H$;
(iii) la relation $x \in H$ implique $x^{-1} \in H$;
(iv) la relation « $x \in H$ et $\alpha \in \Omega$ » implique $x^\alpha \in H$.

Si H est un sous-groupe stable de G, la structure induite sur H par la structure de groupe à opérateurs de G est une structure de groupe à opérateurs, et l’injection canonique de H dans G est un homomorphisme de groupes à opérateurs.

Soit G un groupe. Un sous-groupe stable de G muni de l’action de $\varnothing$ (I, p. 30), c’est-à-dire une partie de G possédant les propriétés (i), (ii), (iii) de la déf. 4, est appelé un sous-groupe de G. Lorsqu’on parlera d’un sous-groupe d’un groupe à opérateurs G, il s’agira d’un sous-groupe du groupe sous-jacent à G. Un sous-groupe d’un groupe à opérateurs G n’est pas nécessairement un sous-groupe stable de G.

Exemple 1). — Soient $\Sigma$ une espèce de structure (E, IV, p. 4) et S une structure d’espèce $\Sigma$ sur un ensemble E (loc. cit.). L’ensemble des automorphismes de S est un sous-groupe de $\mathfrak{S}_E$.

#### Proposition 1 {#alg-i-s4-prop-1 .statement}

Soient G un groupe à opérateurs et H une partie de G stable pour les homothéties de G. Les conditions suivantes sont équivalentes :
a) H est un sous-groupe stable de G.
b) H n’est pas vide et les relations $x \in H, y \in H$ entraînent $xy \in H$ et $x^{-1} \in H$.
c) H n’est pas vide et les relations $x \in H, y \in H$ entraînent $xy^{-1} \in H$.
d) H est stable pour la loi de G et la loi de composition induite sur H par la loi de composition de G est une loi de groupe.

Il est clair que a) entraîne b). Montrons que b) entraîne a). Il suffit de montrer que H contient l’élément neutre de G. La partie H n’étant pas vide, soit $x \in H$. Alors $x^{-1} \in H$ et $e = xx^{-1}$ appartient à H. Il est clair que b) entraîne c). Montrons que c) entraîne b). Tout d’abord, H n’étant pas vide possède un élément x. Par suite $xx^{-1} = e$ est un élément de H. Pour tout élément $x$ de H, $x^{-1} = ex^{-1}$ appartient à H; donc les relations $x \in H, y \in H$ entraînent $xy = x(y^{-1})^{-1} \in H$. Il est clair que a) entraîne d). Montrons que d) entraîne a) : l’injection canonique de H dans G est un homomorphisme de groupes; par suite $e \in H$ et la relation $x \in H$ implique $x^{-1} \in H$ (I, p. 29).

#### Remarque 1 {#alg-i-s4-n3-rem-1 .statement}

On prouve de même que la condition b) de l’énoncé équivaut à la condition
c’) $H \neq \varnothing$ et les relations $x \in H$ et $y \in H$ entraînent $y^{-1}x \in H$.

#### Remarque 2 {#alg-i-s4-n3-rem-2 .statement}

Pour tout sous-groupe H de G, on a les relations
$$
H.H = H \quad \text{et} \quad H^{-1} = H.
$$
En effet, on a $H.H \subset H$ et $H^{-1} \subset H$ d’après b). Comme $e \in H$, on a $H.H \supset e.H = H$, et le passage à l’inverse transforme l’inclusion $H^{-1} \subset H$ en $H \subset H^{-1}$, d’où les formules (1).

Si $H$ est un sous-groupe stable de $G$, et $K$ un sous-groupe stable de $H$, il est clair que $K$ est un sous-groupe stable de $G$.

L’ensemble $\{e\}$ est le plus petit sous-groupe stable de $G$. L’intersection d’une famille de sous-groupes stables de $G$ est un sous-groupe stable. Il y a donc un plus petit sous-groupe stable $H$ de $G$ contenant une partie donnée $X$ de $G$; on l’appelle le *sous-groupe stable engendré par* $X$, et on dit que $X$ est un *système générateur* (ou *ensemble générateur*) de $H$.

#### Proposition 2 {#alg-i-s4-prop-2 .statement}

*Soient $X$ une partie non vide d’un groupe à opérateurs $G$ et $\hat{X}$ la partie stable pour l’action de $\Omega$ dans $G$ engendrée par $X$. Le sous-groupe stable engendré par $X$ est la partie stable pour la loi de $G$ engendrée par l’ensemble $Y = \hat{X} \cup \hat{X}^{-1}$.*

En effet, cette dernière partie $Z$ est l’ensemble des composés des suites finies dont tous les termes sont des éléments de $\hat{X}$ ou des inverses d’éléments de $\hat{X}$; l’inverse d’un tel composé est un composé de même forme (I, p. 17, cor. 1), et $Z$ est stable par l’action de $\Omega$, comme on le voit en appliquant I, p. 26, prop. 1 aux homothéties de $G$, donc (I, p. 31, prop. 1) $Z$ est un sous-groupe stable de $G$. Réciproquement, tout sous-groupe stable contenant $X$ contient évidemment $Y$, donc $Z$.

#### Corollaire 1 {#alg-i-s4-prop-2-cor-1 .statement}

*Soient $G$ un groupe à opérateurs et $X$ une partie de $G$ stable pour l’action de $\Omega$. Le sous-groupe engendré par $X$ et le sous-groupe stable engendré par $X$ coïncident.*

#### Corollaire 2 {#alg-i-s4-prop-2-cor-2 .statement}

*Soient $G$ un groupe et $X$ une partie de $G$ formée d’éléments deux à deux permutables. Le sous-groupe de $G$ engendré par $X$ est commutatif.*

L’ensemble $Y = X \cup X^{-1}$ est formé d’éléments deux à deux permutables (I, p. 16, prop. 5) et la loi induite sur la partie stable engendrée par $Y$ est commutative (I, p. 8, cor. 2).

Si $G$ est un groupe à opérateurs, le sous-groupe *stable* engendré par une partie de $G$ formée d’éléments deux à deux permutables n’est pas nécessairement commutatif.

#### Corollaire 3 {#alg-i-s4-prop-2-cor-3 .statement}

*Soient $f : G \to G'$ un homomorphisme de groupes à opérateurs et $X$ une partie de $G$. L’image par $f$ du sous-groupe stable de $G$ engendré par $X$ est le sous-groupe stable de $G'$ engendré par $f(X)$.*

Posons $X' = f(X)$. On a $\hat{X}' = f(\hat{X})$ et ${X'}^{-1} = f(X^{-1})$. Par suite $f(\hat{X} \cup \hat{X}^{-1}) = \hat{X}' \cup \hat{{X}'}^{-1}$. Le corollaire résulte donc de I, p. 6, prop. 1.

*Exemple 2).* — Soient $G$ un groupe et $x$ un élément de $G$. Le sous-groupe engendré par $\{x\}$ (qu’on appelle plus simplement le sous-groupe engendré par $x$) est l’ensemble des $x^n$ pour $n \in \mathbf{Z}$. La partie stable (pour la loi de $G$) engendrée par $\{x\}$ est l’ensemble des $x^n$ où $n \in \mathbf{N}^*$. Ces deux ensembles sont en général distincts.

Ainsi, dans le groupe additif $\mathbf{Z}$, le sous-groupe engendré par un élément $x$ est l’ensemble $x.\mathbf{Z}$ des $xn$, pour $n \in \mathbf{Z}$, et la partie stable engendrée par $x$ est l’ensemble des $xn$, pour $n \in \mathbf{N}^*$. Ces deux ensembles sont toujours distincts si $x \neq 0$.

La réunion d’une famille *filtrante croissante* de sous-groupes stables de $G$ est évidemment un sous-groupe stable. Il en résulte que, si $P$ est une partie de $G$ et $H$ un sous-groupe stable de G ne rencontrant pas P, l’ensemble des sous-groupes stables de G contenant H et ne rencontrant pas P, ordonné par inclusion, est inductif (E, III, p. 20). En appliquant le th. de Zorn (E, III, p. 20), on obtient le résultat suivant:
**Proposition 3.** — *Soient G un groupe à opérateurs, P une partie de G, H un sous-groupe stable de G ne rencontrant pas P. L’ensemble des sous-groupes stables de G contenant H et ne rencontrant pas P possède un élément maximal.*

### 4. Groupes quotients

#### Théorème 1 {#alg-i-s4-thm-1 .statement}

*Soit R une relation d’équivalence dans un groupe à opérateurs G; si R est compatible à gauche (resp. à droite) (I, p. 26) avec la loi de groupe de G, et compatible avec l’action de Ω, la classe d’équivalence de e est un sous-groupe stable H de G et la relation R est équivalente à $x^{-1}y \in H$ (resp. $yx^{-1} \in H$). Réciproquement, si H est un sous-groupe stable de G, la relation $x^{-1}y \in H$ (resp. $yx^{-1} \in H$) est une relation d’équivalence compatible à gauche (resp. à droite) avec la loi de groupe de G et compatible avec l’action de Ω, pour laquelle H est la classe d’équivalence de e.*

Bornons-nous à considérer le cas où la relation R est compatible à gauche avec la loi de G (le cas d’une relation compatible à droite s’en déduit en remplaçant la loi de G par la loi opposée). La relation $y \equiv x$ (mod. R) équivaut à $x^{-1}y \equiv e$ (mod. R), car $y \equiv x$ entraîne $x^{-1}y \equiv x^{-1}x = e$ et réciproquement $x^{-1}y \equiv e$ entraîne $y = x(x^{-1}y) \equiv x$. Si H désigne la classe d’équivalence de e, la relation R est donc équivalente à $x^{-1}y \in H$. Montrons que H est un sous-groupe stable de G. Pour tout opérateur α, la relation $x \equiv e$ entraîne $x^\alpha \equiv e^\alpha = e$, donc $H^\alpha \subset H$, et H est stable pour l’action de Ω. Il suffit d’établir (I, p. 31, prop. 1) que $x \in H$ et $y \in H$ entraînent $x^{-1}y \in H$, c’est-à-dire que $x \equiv e$ et $y \equiv e$ entraînent $x \equiv y$, ce qui est une conséquence de la transitivité de R.

Réciproquement, soit H un sous-groupe stable de G; la relation $x^{-1}y \in H$ est réflexive, puisque $x^{-1}x = e \in H$; elle est symétrique, puisque $x^{-1}y \in H$ entraîne $y^{-1}x = (x^{-1}y)^{-1} \in H$; elle est transitive, car $x^{-1}y \in H$ et $y^{-1}z \in H$ entraînent $x^{-1}z = (x^{-1}y)(y^{-1}z) \in H$; elle est compatible à gauche avec la loi de composition de G, car on peut écrire $x^{-1}y = (zx)^{-1}(zy)$ pour tout $z \in G$; enfin, pour tout opérateur α, la relation $y \in xH$ entraîne $y^\alpha \in x^\alpha H^\alpha \subset x^\alpha H$, donc la relation d’équivalence $x^{-1}y \in H$ est compatible avec l’action de Ω sur G. C. Q. F. D.

Soient G un groupe, H un sous-groupe de G; la relation $x^{-1}y \in H$ (resp. $yx^{-1} \in H$) s’écrit aussi sous la forme équivalente $y \in xH$ (resp. $y \in Hx$). Tout sous-groupe H de G définit ainsi deux relations d’équivalence dans G, à savoir $y \in xH$ et $y \in Hx$; les classes d’équivalence pour ces relations sont respectivement les ensembles $xH$, qu’on appelle *classes à gauche suivant H* (ou *modulo H*), et les ensembles $Hx$, qu’on appelle *classes à droite suivant H* (ou *modulo H*). En *saturant* une partie $A \subset G$ pour ces relations (E, II, p. 44), on obtient respectivement les ensembles AH et HA. L’application $x \mapsto x^{-1}$ transforme classes à gauche modulo H en classes à droite modulo H et réciproquement.

Le cardinal de l’ensemble des classes à gauche (modulo H) s’appelle l’indice du sous-groupe H par rapport à G, et on le désigne par la notation (G:H); il est aussi égal au cardinal de l’ensemble des classes à droite.

Si un sous-groupe K de G contient H, il est réunion de classes à gauche (ou à droite) suivant H. Puisqu’une classe à gauche suivant K se déduit de K par une translation à gauche, l’ensemble des classes à gauche suivant H contenues dans une classe à gauche suivant K a un cardinal indépendant de celle-ci. Par suite (E, III, p. 41, prop. 9):

#### Proposition 4 {#alg-i-s4-prop-4 .statement}

*Soient H et K deux sous-groupes d’un groupe G, tels que H ⊂ K. On a*
$$
(G:H) = (G:K)(K:H).
$$

#### Corollaire {#alg-i-s4-n4-cor-1 .statement}

*Si G est un groupe fini d’ordre g, H un sous-groupe de G d’ordre h, on a*
$$
h.(G:H) = g
$$
(en particulier, l’ordre et l’indice de H sont des *diviseurs* de l’ordre de G).

Le th. 1 permet de déterminer les relations d’équivalence compatibles avec les lois d’un groupe à opérateurs G: si R est une telle relation, elle est à la fois compatible à droite et à gauche avec la loi de groupe de G et avec l’action de Ω. Par suite, si H est la classe de e (mod. R), H est un sous-groupe stable tel que les relations $y \in xH$ et $y \in Hx$ soient équivalentes (puisque toutes deux sont équivalentes à R); on a donc $xH = Hx$ quel que soit $x \in G$. Réciproquement, s’il en est ainsi, l’une ou l’autre des relations équivalentes $y \in xH, y \in Hx$, est compatible avec la loi du groupe, puisqu’elle est à la fois compatible à gauche et à droite avec cette loi (I, p. 27), et est compatible avec l’action de Ω. L’égalité $xH = Hx$ étant équivalente à $xHx^{-1} = H$, on pose la définition suivante:

#### Définition 5 {#alg-i-s4-def-5 .statement}

*Soit G un groupe à opérateurs. Un sous-groupe stable H de G est appelé sous-groupe stable distingué (ou invariant ou normal) de G si l’on a $xHx^{-1} = H$ pour tout $x \in G$.*

Si $\Omega = \varnothing$, un sous-groupe stable distingué de G est appelé un *sous-groupe distingué* (ou *invariant*, ou *normal*) de G. Dans un groupe commutatif, tout sous-groupe est distingué.

Pour vérifier qu’un sous-groupe stable H est distingué, il suffit de montrer que $xHx^{-1} \subset H$ pour tout $x \in G$; en effet, s’il en est ainsi, on a aussi $x^{-1}Hx \subset H$ pour tout $x \in G$, c’est-à-dire $H \subset xHx^{-1}$, et, par suite $H = xHx^{-1}$.

Soient H un sous-groupe stable distingué de G, R la relation d’équivalence $y \in xH$ définie par H; sur l’ensemble quotient G/R, la loi interne, quotient par R de la loi du groupe G, est associative; la classe de e est l’élément neutre pour cette loi quotient; les classes de deux éléments inverses dans G sont inverses pour la loi quotient, et l’action de $\Omega$, quotient par $R$ de l’action de $\Omega$ sur $G$, est distributive par rapport à la loi interne de $G/R$ (I, p. 27). Donc, en résumant les résultats obtenus:

#### Théorème 2 {#alg-i-s4-thm-2 .statement}

*Soit $G$ un groupe à opérateurs. Pour qu’une relation d’équivalence $R$ sur $G$ soit compatible avec la loi de groupe et l’action de $\Omega$, il faut et il suffit qu’elle soit de la forme $x^{-1}y \in H$, où $H$ est un sous-groupe stable distingué de $G$ (la relation $x^{-1}y \in H$ étant d’ailleurs équivalente à $yx^{-1} \in H$ pour un tel sous-groupe). La loi de composition sur $G/R$ quotient de celle de $G$ et l’action de $\Omega$ sur $G/R$ quotient de celle de $\Omega$ sur $G$ par une telle relation $R$ munissent $G/R$ d’une structure de groupe à opérateurs, dite structure quotient, et l’application canonique de passage au quotient est un homomorphisme de groupes à opérateurs.*

#### Définition 6 {#alg-i-s4-def-6 .statement}

*Le quotient d’un groupe à opérateurs $G$ par la relation d’équivalence définie par un sous-groupe stable distingué $H$ de $G$, muni de la structure quotient, s’appelle le groupe à opérateurs quotient de $G$ par $H$ et se note $G/H$. L’application canonique $G \to G/H$ s’appelle homomorphisme canonique.*

Pour qu’une application de $G/H$ dans un groupe à opérateurs soit un homomorphisme de groupes à opérateurs, il faut et il suffit que son composé avec l’application canonique de $G$ sur $G/H$ en soit un; ceci justifie le nom de groupe quotient (E, IV, p. 21).

Soient $G$ un groupe et $H$ un sous-groupe distingué de $G$. Le quotient $G/H$, muni de sa structure de groupe, s’appelle *groupe quotient* de $G$ par $H$.

On note $x \equiv y$ (mod. $H$) ou $x \equiv y$ ($H$) la relation d’équivalence définie par un sous-groupe stable distingué de $G$.

#### Proposition 5 {#alg-i-s4-prop-5 .statement}

*Soient $f : G \to G'$ un homomorphisme de groupes à opérateurs, $H$ et $H'$ des sous-groupes stables distingués de $G$ et $G'$ respectivement tels que $f(H) \subset H'$. L’application $f$ est compatible avec les relations d’équivalence définies par $H$ et $H'$. Soient $\pi : G \to G/H$ et $\pi' : G' \to G'/H'$ les homomorphismes canoniques. L’application $\bar{f} : G/H \to G'/H'$ déduite de $f$ par passage aux quotients est un homomorphisme.

Si $x \equiv y$ (mod. $H$), on a $x^{-1}y \in H$, d’où $f(x)^{-1}f(y) = f(x^{-1})f(y) = f(x^{-1}y) \in f(H) \subset H'$, donc $f(x) \equiv f(y)$ (mod. $H'$). La deuxième assertion résulte de la propriété universelle des lois quotients (I, p. 11).

#### Remarque 1 {#alg-i-s4-n4-rem-1 .statement}

Si $A$ est une partie quelconque d’un groupe $G$, et $H$ un sous-groupe distingué de $G$, on a $AH = HA$; cet ensemble est obtenu en saturant $A$ pour la relation $x \equiv y$ (mod. $H$).

#### Remarque 2 {#alg-i-s4-n4-rem-2 .statement}

Si $H$ est un sous-groupe distingué d’indice fini de $G$, le groupe quotient $G/H$ est un groupe fini d’ordre ($G : H$).

On notera que si $H$ est un sous-groupe distingué d’un groupe $G$ et si $K$ est un sous-groupe distingué de $H$, $K$ n’est pas nécessairement un sous-groupe distingué de $G$ (I, p. 130, exerc. 10).

Soit $G$ un groupe à opérateurs. L’intersection de toute famille de sous-groupes stables distingués de $G$ est un sous-groupe stable distingué. Par suite, pour toute partie X de G, il existe un plus petit sous-groupe stable distingué contenant X, appelé sous-groupe stable distingué engendré par X.

Dans un groupe à opérateurs G, les sous-groupes stables G et {e} sont distingués.

#### Définition 7 {#alg-i-s4-def-7 .statement}

Un groupe à opérateurs G est dit simple si G ≠ {e} et s’il n’existe aucun sous-groupe stable distingué de G autre que G et {e}.

### 5. Décomposition d’un homomorphisme

#### Proposition 6 {#alg-i-s4-prop-6 .statement}

Soient G un groupe à opérateurs, et G’ un magma muni d’une action de Ω, notée exponentiellement. Soit f : G → G’ un homomorphisme du magma G dans le magma G’ tel que, pour tout α ∈ Ω et tout x ∈ G, on ait f(xα) = f(x)α. Alors f(G) est une partie stable de G’ pour la loi de G’ et l’action de Ω ; l’ensemble f(G) muni des lois induites est un groupe à opérateurs, et l’application x ↦ f(x) de G dans f(G) est un homomorphisme de groupes à opérateurs.

En vertu de I, p. 6, prop. 1, f(G) est une partie stable de G’ pour la loi interne de G’. Pour tout élément x ∈ G et pour tout opérateur α, on a f(x)α = f(xα) ∈ f(G) et par suite f(G) est stable pour l’action de Ω sur G’. La loi interne de G’ étant notée multiplicativement, on a

$$
(f(x)f(y))f(z) = f(xy)f(z) = f((xy)z)
= f(x(yz)) = f(x)f(yz) = f(x)(f(y)f(z))
$$

quels que soient les éléments x, y, z de G ; par suite la loi induite sur f(G) est associative. Soit e l’élément neutre de G. Son image f(e) est élément neutre de f(G) (I, p. 13). Tout élément de f(G) est inversible dans f(G) (I, p. 15). Par suite la loi induite sur f(G) par la loi interne de G’ est une loi de groupe. Quels que soient les éléments x et y de G et l’opérateur α, on a

$$
(f(x)f(y))α = (f(xy))α = f((xy)α) = f(xαyα)
= f(xα)f(yα) = (f(x))α(f(y))α
$$

ce qui montre que l’action de Ω est distributive par rapport à la loi de groupe de f(G). Par suite f(G) muni des lois induites est un groupe à opérateurs et il est clair que l’application x ↦ f(x) est un homomorphisme de groupes à opérateurs.

#### Définition 8 {#alg-i-s4-def-8 .statement}

Soit f : G → G’ un homomorphisme de groupes à opérateurs. L’image réciproque de l’élément neutre de G’ est appelée le noyau de f.

Le noyau de f se note souvent Ker(f) et l’image f(G) de f se note parfois Im(f).

#### Théorème 3 {#alg-i-s4-thm-3 .statement}

Soit f : G → G’ un homomorphisme de groupes à opérateurs.
a) Ker(f) est un sous-groupe stable distingué de G ;
b) Im(f) est un sous-groupe stable de G’ ;
c) l’application f est compatible avec la relation d’équivalence définie sur G par Ker(f) ;

d) l’application $\tilde{f} : G / \mathrm{Ker}(f) \to \mathrm{Im}(f)$ déduite de $f$ par passage au quotient est un isomorphisme de groupes à opérateurs;
e) on a $f = \iota \circ \tilde{f} \circ \pi$, où $\iota$ est l’injection canonique de $\mathrm{Im}(f)$ dans $G'$ et $\pi$ l’homomorphisme canonique de $G$ sur $G / \mathrm{Ker}(f)$.

L’assertion b) résulte de la prop. 6. La relation d’équivalence $f(x) = f(y)$ sur $G$ est compatible avec la structure de groupe à opérateurs de $G$. D’après le th. 2 (I, p. 35), elle est donc de la forme $y \in xH$, où $H$ est un sous-groupe stable distingué de $G$, et $H$ est la classe de l’élément neutre, d’où $H = \mathrm{Ker}(f)$. Les assertions a), c) et d) en résultent. L’assertion e) est évidente (E, II, p. 44).

### 6. Sous-groupes d’un groupe quotient

#### Proposition 7 {#alg-i-s4-prop-7 .statement}

Soient $G$ et $H$ deux groupes à opérateurs, $f$ un homomorphisme de $G$ dans $H$ et $N$ le noyau de $f$.

a) Soit $H'$ un sous-groupe stable de $H$. L’image réciproque $G' = f^{-1}(H')$ est un sous-groupe stable de $G$, et $G'$ est distingué dans $G$ si $H'$ est distingué dans $H$. De plus, $N$ est un sous-groupe distingué de $G'$. Si $f$ est surjectif, on a $H' = f(G')$ et $f$ définit un isomorphisme de $G'/N$ sur $H'$ par passage au quotient.

b) Soit $G'$ un sous-groupe stable de $G$. L’image $H' = f(G')$ est un sous-groupe stable de $H$ et l’on a $f^{-1}(H') = G'N = NG'$. En particulier, on a $f^{-1}(H') = G'$ si et seulement si $N \subset G'$. Si $f$ est surjectif et si $G'$ est distingué dans $G$, alors $H'$ est distingué dans $H$.

a) Soient $x$ et $y$ dans $G'$ et $\alpha \in \Omega$; on a $f(x) \in H', f(y) \in H',$ d’où $f(xy^{-1}) = f(x)f(y)^{-1} \in H',$ c’est-à-dire $xy^{-1} \in G'$; donc $G'$ est un sous-groupe de $G$. On a $f(x^\alpha) = f(x)^\alpha \in H',$ d’où $x^\alpha \in G',$ et par suite $G'$ est stable. Supposons $H'$ distingué dans $H$ et soient $x \in G', y \in G$; on a $f(x) \in H'$ et

$$
f(yxy^{-1}) = f(y)f(x)f(y)^{-1} \in H'
$$

d’où $yxy^{-1} \in G'$; donc $G'$ est distingué dans $G$. Pour tout $n \in N$, on a $f(n) = e \in H',$ d’où $N \subset G'$; comme $N$ est distingué dans $G$, il l’est dans $G'$. Enfin, si $f$ est surjectif, on a $f(f^{-1}(A)) = A$ pour toute partie $A$ de $H$, d’où $H' = f(G')$; la restriction de $f$ à $G'$ est un homomorphisme $f'$ de $G'$ sur $H'$, de noyau $N$, donc $f'$ définit par passage au quotient un isomorphisme de $G'/N$ sur $H'$.

b) Soient $a$ et $b$ dans $H'$ et $\alpha \in \Omega$; il existe $x, y$ dans $G'$ tels que $a = f(x)$ et $b = f(y)$, d’où $ab^{-1} = f(xy^{-1}) \in H'$; donc $H'$ est un sous-groupe de $H$, qui est stable car $a^\alpha = f(x^\alpha) \in H'$. Soit $x \in G$; on a $x \in f^{-1}(H')$ si et seulement si $f(x) \in H' = f(G')$, c’est-à-dire si et seulement s’il existe $y$ dans $G'$ avec $f(x) = f(y)$; la relation $f(x) = f(y)$ équivaut à l’existence de $n \in N$ avec $x = yn$; finalement, $x \in f^{-1}(H')$ équivaut à $x \in G'N = NG'$. Il est clair que la relation $G' = G'N$ équivaut à $G' \supset N$. Supposons enfin $f$ surjectif et $G'$ distingué dans

G; soient $a \in H'$ et $b \in H$; il existe $x \in G'$ et $y \in G$ tels que $a = f(x)$ et $b = f(y)$, d’où $bab^{-1} = f(yxy^{-1}) \in f(G') = H'$. Donc $H'$ est distingué dans $H$.

#### Corollaire 1 {#alg-i-s4-prop-7-cor-1 .statement}

*On suppose f surjectif. Soient $\mathfrak{S}$ (resp. $\mathfrak{S}'$) l’ensemble des sous-groupes stables (resp. stables distingués) de $G$ contenant $N$ et $\mathfrak{H}$ (resp. $\mathfrak{H}'$) l’ensemble des sous-groupes stables (resp. stables distingués) de $H$, ces ensembles étant ordonnés par inclusion. L’application $G' \mapsto f(G')$ est un isomorphisme d’ensembles ordonnés $\Phi : \mathfrak{S} \to \mathfrak{H}$; l’isomorphisme réciproque $\Psi : \mathfrak{H} \to \mathfrak{S}$ est l’application $H' \mapsto f^{-1}(H')$. De plus $\Phi$ et $\Psi$ induisent des isomorphismes $\Phi' : \mathfrak{S}' \to \mathfrak{H}'$ et $\Psi' : \mathfrak{H}' \to \mathfrak{S}'$.

#### Corollaire 2 {#alg-i-s4-prop-7-cor-2 .statement}

*Soient $f : G \to H$ un homomorphisme des groupes à opérateurs, $N$ le noyau de $f$, $G'$ un sous-groupe stable de $G$ et $L$ un sous-groupe stable distingué de $G'$. Alors $LN, L.(G' \cap N)$ et $f(L)$ sont des sous-groupes stables distingués de $G'N, G'$ et $f(G')$ respectivement, et les trois groupes à opérateurs quotients $G'N/LN, G'/(L.(G' \cap N))$ et $f(G')/f(L)$ sont isomorphes.

Posons $H' = f(G')$ et notons $f'$ l’homomorphisme de $G'$ sur $H'$ qui coïncide avec $f$ sur $G'$; le noyau de $f'$ est $G' \cap N$ et l’on a $f'(L) = f(L)$; d’après la prop. 7 (I, p. 37), $f'(L)$ est un sous-groupe stable distingué de $H'$ et ${f'}^{-1}(f'(L)) = L.(G' \cap N)$ est un sous-groupe stable distingué de $G'$. Soit $\lambda$ l’homomorphisme canonique de $H'$ sur $H'/f'(L) = f(G')/f(L)$; comme $\lambda \circ f'$ est surjectif de noyau ${f'}^{-1}(f'(L)) = L.(G' \cap N)$, il définit un isomorphisme de $G'/(L.(G' \cap N))$ sur $f(G')/f(L)$. D’après la prop. 7, b) (I, p. 37), on a $f^{-1}(H') = G'N$; si $f''$ est l’homomorphisme de $G'N$ sur $H'$ qui coïncide avec $f$ sur $G'N$, l’homomorphisme $\lambda \circ f''$ de $G'N$ sur $f(G')/f(L)$ est surjectif, de noyau $f^{-1}(f(L)) = LN$; ceci prouve que $LN$ est un sous-groupe stable distingué de $G'N$ et que $\lambda \circ f''$ définit un isomorphisme de $G'N/LN$ sur $f(G')/f(L)$.

#### Corollaire 3 {#alg-i-s4-prop-7-cor-3 .statement}

*Soient $f : G \to H$ un homomorphisme de groupes à opérateurs, $N$ son noyau, $X$ une partie de $G$ telle que $f(X)$ engendre $H$, et $Y$ une partie de $N$ qui engendre $N$. Alors $X \cup Y$ engendre $G$.

Soit $G'$ le sous-groupe stable de $G$ engendré par $X \cup Y$. Comme $Y \subset G'$, on a $N \subset G'$. Comme $f(X) \subset f(G')$ on a $f(G') = H$, d’où $G' = f^{-1}(H) = G$.

#### Remarque {#alg-i-s4-n6-rem-1 .statement}

Avec les notations de la prop. 7 (I, p. 37), le fait que l’image réciproque d’un sous-groupe de $H$ est un sous-groupe de $G$ résulte du fait suivant:

*Si A et B sont des parties de H, et si f est surjectif, on a*

$$
f^{-1}(A.B) = f^{-1}(A) . f^{-1}(B), \quad f^{-1}(A^{-1}) = f^{-1}(A)^{-1}.
$$

On a évidemment $f^{-1}(A) . f^{-1}(B) \subset f^{-1}(A.B)$; d’autre part, si $z \in f^{-1}(A.B)$, il existe $a \in A$ et $b \in B$ tels que $f(z) = ab$; comme $f$ est surjectif, il existe $x \in G$ tel que $f(x) = a$; si l’on pose $y = x^{-1}z$, on a $f(y) = a^{-1}f(z) = b$, et $z = xy$, d’où $z \in f^{-1}(A) . f^{-1}(B)$. La relation $x \in f^{-1}(A^{-1})$ équivaut à $f(x) \in A^{-1}$, donc à $f(x^{-1}) \in A$, c’est-à-dire à $x^{-1} \in f^{-1}(A)$ et finalement à $x \in f^{-1}(A)^{-1}$.

#### Proposition 8 {#alg-i-s4-prop-8 .statement}

*Soient G un groupe à opérateurs, A et B deux sous-groupes stables de G.*

On suppose que les relations $a \in A$ et $b \in B$ impliquent $aba^{-1} \in B$ *(autrement dit, A normalise B)*. Alors on a $AB = BA$, et $AB$ est un sous-groupe stable de $G$, $A \cap B$ est un sous-groupe stable distingué de $A$, et $B$ est un sous-groupe stable distingué de $AB$. L’injection canonique de $A$ dans $AB$ définit par passage au quotient un isomorphisme de $A/(A \cap B)$ sur $AB/B$.

Les formules
$$
(ab)(a'b') = aa'({a'}^{-1}ba'.b')
$$
$$
(ab)^{-1} = a^{-1}(ab^{-1}a^{-1})
$$
$$
(ab)^{\alpha} = a^{\alpha}b^{\alpha}
$$

quels que soient $a, a'$ dans $A$, $b, b'$ dans $B$ et l’opérateur $\alpha$ de $G$, montrent que $AB$ est un sous-groupe stable de $G$. Soient $a \in A$ et $x \in A \cap B$; on a $axa^{-1} \in B$ d’après les hypothèses faites sur $A$ et $B$, et il est clair que $axa^{-1}$ appartient à $A$, donc $A \cap B$ est distingué dans $A$. Soient $a \in A$ et $b, b'$ dans $B$; la formule $(ab)b'(ab)^{-1} = a(bb'b^{-1})a^{-1}$ montre que $B$ est distingué dans $AB$. Soit $\varphi$ la restriction à $A$ de l’homomorphisme canonique de $AB$ sur $AB/B$; on a $\varphi(a) = aB$, donc le noyau de $\varphi$ est égal à $A \cap B$. Il est clair que $\varphi$ est surjectif, donc définit un isomorphisme de $A/(A \cap B)$ sur $AB/B$.

#### Théorème 4 {#alg-i-s4-thm-4 .statement}

Soient $G$ un groupe à opérateurs et $N$ un sous-groupe stable distingué de $G$.

a) *L’application* $G' \mapsto G'/N$ *est une bijection de l’ensemble des sous-groupes stables de* $G$ *contenant* $N$ *sur l’ensemble des sous-groupes stables de* $G/N$.

b) *Soit* $G'$ *un sous-groupe stable de* $G$ *contenant* $N$. *Pour que* $G'/N$ *soit distingué dans* $G/N$, *il faut et il suffit que* $G'$ *soit distingué dans* $G$, *et les groupes à opérateurs* $G/G'$ *et* $(G/N)/(G'/N)$ *sont alors isomorphes*.

c) *Soit* $G'$ *un sous-groupe stable de* $G$. *Alors* $G'N$ *est un sous-groupe stable de* $G$, *et* $N$ *est distingué dans* $G'N$. *De plus* $G' \cap N$ *est distingué dans* $G'$ *et les groupes à opérateurs* $G'/(G' \cap N)$ *et* $G'N/N$ *sont isomorphes*.

Notons $f$ l’homomorphisme canonique de $G$ sur $G/N$. Pour tout $x \in G$, on a $f(x) = xN$; par suite, on a $f(G') = G'/N$ pour tout sous-groupe $G'$ de $G$ contenant $N$. Comme $f$ est surjectif, l’assertion a) résulte de I, p. 38, cor. 1 ; il est de même de l’équivalence « $G'$ distingué » $\Leftrightarrow$ « $G'/N$ distingué ». Supposons que $G'$ soit un sous-groupe stable distingué de $G$, contenant $N$. D’après I, p. 35, prop. 5, appliquée à $\mathrm{Id}_G$, il existe un homomorphisme $u$ de $G/N$ dans $G/G'$ défini par $u(xN) = xG'$ pour tout $x \in G$. Il est immédiat que $u$ est surjectif, de noyau $G'/N$, d’où l’isomorphisme cherché de $(G/N)/(G'/N)$ sur $G/G'$. Enfin, c) résulte immédiatement de I, p. 38, prop. 8.

### 7. Le théorème de Jordan-Hölder

#### Définition 9 {#alg-i-s4-def-9 .statement}

On appelle suite de composition d’un groupe à opérateurs $G$ une suite finie $(G_i)_{0 \leq i \leq n}$ de sous-groupes stables de $G$, avec $G_0 = G$, $G_n = \{ e \}$ et telle que $G_{i+1}$ soit un sous-groupe distingué de $G_i$ pour $0 \leq i \leq n-1$. Les quotients $G_i/G_{i+1}$ s’appellent les quotients de la suite. Une suite de composition $\Sigma'$ est dite plus fine qu'une suite de composition $\Sigma$ si $\Sigma$ est une suite extraite de $\Sigma'$.

Si $(G_i)_{0 \leq i \leq n}$ et $(H_j)_{0 \leq j \leq m}$ sont respectivement des suites de composition de deux groupes à opérateurs $G$ et $H$, on dit qu’elles sont équivalentes si $m = n$ et s’il existe une permutation $\varphi$ de l’intervalle $[0, n - 1]$ de $\mathbf{N}$, telle que les groupes à opérateurs $G_i / G_{i+1}$ et $H_{\varphi(i)}/H_{\varphi(i)+1}$ soient isomorphes quel que soit $i$.

On notera qu’en général une suite extraite d’une suite de composition $(G_i)$ n’est pas une suite de composition, car pour $j > i + 1$, $G_j$ n’est pas en général un sous-groupe distingué de $G_i$.

#### Théorème 5 (Schreier) {#alg-i-s4-thm-5 .statement}

*Etant données deux suites de composition $\Sigma_1, \Sigma_2$ d’un groupe à opérateurs $G$, il existe deux suites de composition équivalentes $\Sigma'_1, \Sigma'_2$, plus fines respectivement que $\Sigma_1$ et $\Sigma_2$*.

Soient $\Sigma_1 = (H_i)_{0 \leq i \leq n}$ et $\Sigma_2 = (K_j)_{0 \leq j \leq p}$ les deux suites de composition données ayant respectivement $n + 1$ et $p + 1$ termes; nous allons voir qu’on peut former la suite de composition $\Sigma'_1$ en intercalant $p - 1$ sous-groupes $H'_{i,j}$ ($1 \leq j \leq p - 1$) entre $H_i$ et $H_{i+1}$ pour $0 \leq i \leq n - 1$, et la suite $\Sigma'_2$ en intercalant $n - 1$ sous-groupes $K'_{j,i}$ ($1 \leq i \leq n - 1$) entre $K_j$ et $K_{j+1}$ pour $0 \leq j \leq p - 1$; on obtiendra ainsi deux suites de $pn + 1$ sous-groupes stables de $G$; en choisissant convenablement les sous-groupes stables intercalés, nous allons montrer que ces suites sont des suites de composition équivalentes.

Remarquons pour cela que $H_i \cap K_j$ est un sous-groupe stable de $H_i$ et de $K_j$, donc (I, p. 39, th. 4) $H_{i+1}.(H_i \cap K_j)$ est un sous-groupe stable de $H_i$ contenant $H_{i+1}$ et $K_{j+1}.(H_i \cap K_j)$ est un sous-groupe stable de $K_j$ contenant $K_{j+1}$. Si on pose $H'_{i,j} = H_{i+1}.(H_i \cap K_j)$ et $K'_{j,i} = K_{j+1}.(H_i \cap K_j)$, $H'_{i,j+1}$ est un sous-groupe stable de $H'_{i,j}$ ($0 \leq j \leq p - 1$) et $K'_{j,i+1}$ est un sous-groupe stable de $K'_{j,i}$ ($0 \leq i \leq n - 1$). On a d’ailleurs $H'_{i,0} = H_i$, $H'_{i,p} = H_{i+1}$, $K'_{j,0} = K_j$, et $K'_{j,n} = K_{j+1}$. Pour démontrer le théorème, il suffit de montrer que $H'_{i,j+1}$ (resp. $K'_{j,i+1}$) est un sous-groupe stable distingué de $H'_{i,j}$ (resp. $K'_{j,i}$), et que les groupes quotients $H'_{i,j}/H'_{i,j+1}$ et $K'_{j,i}/K'_{j,i+1}$ sont isomorphes ($0 \leq i \leq n - 1$, $0 \leq j \leq p - 1$). Ceci résulte du lemme suivant en prenant $H = H_i$, $H' = H_{i+1}$, $K = K_j$, $K' = K_{j+1}$.

#### Lemme 1 (Zassenhaus) {#alg-i-s4-lem-1 .statement}

*Soient $H$ et $K$ deux sous-groupes stables d’un groupe à opérateurs $G$, $H'$ et $K'$ des sous-groupes stables distingués de $H$ et $K$ respectivement; alors $H'.(H \cap K')$ est un sous-groupe stable distingué de $H'.(H \cap K)$, $K'.(K \cap H')$ est un sous-groupe stable distingué de $K'.(K \cap H)$, et les groupes à opérateurs quotients $(H'.(H \cap K))/(H'.(H \cap K'))$ et $(K'.(K \cap H))/(K'.(K \cap H'))$ sont isomorphes*.

D’après I, p. 39, th. 4, $H' \cap K = H' \cap (H \cap K)$ est sous-groupe stable distingué de $H \cap K$; de même $K' \cap H$ est sous-groupe stable distingué de $K \cap H$; donc (I, p. 38, cor. 2) $(H' \cap K)(K' \cap H)$ est sous-groupe stable distingué de $H \cap K$. D’après le th. 4 (I, p. 39) appliqué au groupe $H$, $H'.(H' \cap K).(K' \cap H) =$

H'.(H ∩ K') est sous-groupe stable distingué de H'.(H ∩ K), et le groupe quotient (H'.(H ∩ K))/(H'.(H ∩ K')) est isomorphe à
$$(H ∩ K)/((H' ∩ K).(K' ∩ H)).$$
Dans ce dernier quotient, H et H' d’une part, K et K' de l’autre, figurent symétriquement; en les permutant, on obtient le résultat annoncé. C. Q.F.D.

#### Définition 10 {#alg-i-s4-def-10 .statement}

On appelle suite de Jordan-Hölder d’un groupe à opérateurs G une suite de composition Σ strictement décroissante, telle qu’il n’existe aucune suite de composition strictement décroissante, distincte de Σ et plus fine que Σ.

#### Proposition 9 {#alg-i-s4-prop-9 .statement}

Pour qu’une suite de composition G soit une suite de Jordan-Hölder de G, il faut et il suffit que tous les quotients de la suite soient simples.

Une suite de composition est strictement décroissante si et seulement si aucun de ses quotients successifs n’est réduit à l’élément neutre. Si une suite de composition strictement décroissante Σ n’est pas une suite de Jordan-Hölder, il existe une suite de composition strictement décroissante Σ' plus fine que Σ et distincte de Σ. Il y a donc deux termes consécutifs G_i, G_{i+1} de Σ qui ne sont pas consécutifs dans Σ'; soit H le premier terme qui suit G_i dans Σ'; H est un sous-groupe stable distingué de G_i, contenant G_{i+1} et distinct de ce dernier; donc H/G_{i+1} est un sous-groupe stable distingué de G_i/G_{i+1}, distinct de celui-ci et de l’élément neutre; par suite G_i/G_{i+1} n’est pas simple. Réciproquement, si Σ est une suite de composition strictement décroissante dont un des quotients G_i/G_{i+1} n’est pas simple, ce quotient contient un sous-groupe stable distingué autre que lui-même et {e}, dont l’image réciproque dans G_i est un sous-groupe stable distingué H de G_i, distinct de G_i et de G_{i+1} (I, p. 39, th. 4); il suffit d’insérer H entre G_i et G_{i+1} pour avoir une suite de composition strictement décroissante, distincte de Σ et plus fine que Σ.

#### Théorème 6 (Jordan-Hölder) {#alg-i-s4-thm-6 .statement}

Deux suites de Jordan-Hölder d’un groupe à opérateurs sont équivalentes.

Soient Σ_1, Σ_2 deux suites de Jordan-Hölder d’un groupe à opérateurs G; en appliquant le th. 5 (I, p. 40), on en déduit deux suites de composition équivalentes Σ'_1, Σ'_2, respectivement plus fines que Σ_1 et Σ_2; ces dernières étant des suites de Jordan-Hölder, Σ'_1 est identique à Σ_1 ou s’en déduit en répétant certains termes; la suite des quotients de Σ'_1 se déduit de celle de Σ_1 en insérant un certain nombre de termes isomorphes au groupe {e}; Σ_1 étant strictement décroissante, la suite des quotients de Σ_1 se déduit de celle de Σ'_1 en supprimant dans cette dernière tous les termes isomorphes à {e}. De même pour Σ_2 et Σ'_2. Comme les suites des quotients de Σ'_1 et Σ'_2 ne diffèrent (à des isomorphies près) que par l’ordre des termes, il en est de même de celles de Σ_1 et Σ_2; le théorème est démontré.

#### Corollaire {#alg-i-s4-n7-cor-1 .statement}

Soit G un groupe à opérateurs dans lequel il existe une suite de Jordan-Hölder. Si Σ est une suite de composition strictement décroissante quelconque de G, il existe une suite de Jordan-Hölder plus fine que Σ.

En effet, soit $\Sigma_0$ une suite de Jordan-Hölder de $G$; d’après le th. 5 (I, p. 40), il existe deux suites de composition équivalentes, $\Sigma'$ et $\Sigma'_0$, plus fines respectivement que $\Sigma$ et $\Sigma_0$; le raisonnement du th. 6 (I, p. 41) montre qu’en supprimant de $\Sigma'$ les répétitions, on obtient une suite $\Sigma''$ équivalente à $\Sigma_0$, donc une suite de Jordan-Hölder, puisque tous ses quotients sont simples (I, p. 41, prop. 9). Comme $\Sigma$ est strictement décroissante, $\Sigma''$ est plus fine que $\Sigma$, d’où le corollaire.

#### Remarque {#alg-i-s4-n7-rem-1 .statement}

Un groupe à opérateurs ne possède pas toujours de suite de Jordan-Hölder; un exemple est fourni par le groupe additif $\mathbf{Z}$ des entiers rationnels : la suite $(2^n . \mathbf{Z})_{n \geqslant 0}$ est une suite infinie strictement décroissante de sous-groupes (distingués) de $\mathbf{Z}$; quel que soit $p$, les $p$ premiers termes de cette suite forment, avec le groupe $\{0\}$, une suite de composition strictement décroissante; s’il existait une suite de Jordan-Hölder pour $\mathbf{Z}$, elle aurait au moins $p + 1$ termes, d’après le corollaire du th. 6; conclusion absurde, puisque $p$ est arbitraire.

Par contre, il existe une suite de Jordan-Hölder dans tout groupe à opérateurs fini $G$: en effet, si $G \neq \{e\}$, parmi les sous-groupes stables distingués de $G$, distincts de $G$, soit $H_1$ un sous-groupe maximal; lorsque $H_n \neq \{e\}$, définissons de même par récurrence $H_{n+1}$ comme un élément maximal de l’ensemble des sous-groupes stables distingués de $H_n$, distincts de $H_n$; la suite des ordres des $H_n$ est strictement décroissante, donc il existe $n$ tel que $H_n = \{e\}$, et la suite formée de $G$ et des $H_i$ ($1 \leqslant i \leqslant n$) est, d’après sa formation, une suite de Jordan-Hölder.

#### Définition 11 {#alg-i-s4-def-11 .statement}

Soit $G$ un groupe à opérateurs; on appelle longueur de $G$ la borne supérieure des entiers $n$ tels qu’il existe une suite de composition de $G$ strictement décroissante $(G_i)_{0 \leqslant i \leqslant n}$.

Si $G$ admet une suite de Jordan-Hölder, la longueur de $G$ est le nombre des quotients successifs de cette suite comme il résulte du cor. du th. 6 (I, p. 41). Si $G$ n’admet pas de suite de Jordan-Hölder, sa longueur est infinie; en effet d’après I, p. 41, prop. 9, pour toute suite de composition strictement décroissante de $G$, il existe une suite de composition strictement décroissante strictement plus fine. Le groupe réduit à l’élément neutre est le seul groupe à opérateurs de longueur zéro. Un groupe à opérateurs est simple si et seulement s’il est de longueur 1.

Soient $G$ un groupe à opérateurs, $H$ un sous-groupe stable distingué de $G$, $K$ le quotient $G/H$ et $\pi : G \to K$ l’homomorphisme canonique. Soient $\Sigma' = (H_i)_{0 \leqslant i \leqslant n}$ une suite de composition de $H$ et $\Sigma'' = (K_j)_{0 \leqslant j \leqslant p}$ une suite de composition de $K$. En posant $G_i = \pi^{-1}(K_i)$ pour $0 \leqslant i \leqslant p$ et $G_i = H_{i-p}$ pour $p \leqslant i \leqslant n+p$, on obtient une suite de composition $\Sigma = (G_i)_{0 \leqslant i \leqslant n+p}$ de $G$. La suite des quotients de $\Sigma$ s’obtient en juxtaposant la suite des quotients de $\Sigma''$ et la suite des quotients de $\Sigma'$. Si $\Sigma'$ et $\Sigma''$ sont des suites de Jordan-Hölder, $\Sigma$ est une suite de Jordan-Hölder de $G$ d’après la prop. 9 (I, p. 41). Si $H$ ou $K$ admet des suites de composition de longueur arbitrairement grande, il en est de même de $G$. Nous avons démontré:

#### Proposition 10 {#alg-i-s4-prop-10 .statement}

Soient $G$ un groupe à opérateurs, $H$ un sous-groupe stable distingué de $G$. La longueur de $G$ est la somme des longueurs de $H$ et de $G/H$.

#### Corollaire {#alg-i-s4-n7-cor-2 .statement}

Soient $G$ un groupe à opérateurs et $(G_i)_{0 \leq i \leq n}$ une suite de composition de $G$. La longueur de $G$ est la somme des longueurs des $G_i / G_{i+1}$ pour $0 \leq i \leq n - 1$.

Si $G$ et $G'$ sont des groupes à opérateurs isomorphes, et si $G$ admet une suite de Jordan-Hölder, il en est de même de $G'$ et les suites de Jordan-Hölder de $G$ et $G'$ sont équivalentes. Cependant, des groupes non isomorphes peuvent avoir des suites de Jordan-Hölder équivalentes ; il en est ainsi pour $\mathbf{Z}/4\mathbf{Z}$ et $(\mathbf{Z}/2\mathbf{Z}) \times (\mathbf{Z}/2\mathbf{Z})$, cf. I, p. 48.

### 8. Produits et produits fibrés

Soit $(G_i)_{i \in I}$ une famille de groupes à opérateurs. Soit $G$ le monoïde produit des $G_i$. Considérons l’action de $\Omega$ sur $G$ définie par

$$
((x_i)_{i \in I})^\alpha = (x_i^\alpha)_{i \in I} \quad (\alpha \in \Omega, x_i \in G_i).
$$

Muni de cette structure, $G$ est un groupe à opérateurs. Pour tout $i \in I$, l’application de projection $\mathrm{pr}_i : G \to G_i$ est un homomorphisme de groupes à opérateurs.

#### Définition 12 {#alg-i-s4-def-12 .statement}

Le groupe à opérateurs $G = \prod_{i \in I} G_i$ défini ci-dessus est appelé groupe à opérateurs produit des $G_i$. Les applications $\mathrm{pr}_i : G \to G_i$ sont appelées les homomorphismes de projection.

Un cas particulier de produit de groupes à opérateurs est le groupe $G^E$ formé par les applications d’un ensemble $E$ dans un groupe à opérateurs $G$, les lois étant définies par:

$$
(fg)(x) = f(x)g(x) \quad (f, g \text{ dans } G^E, x \in E)
$$
$$
f^\alpha(x) = f(x)^\alpha \quad (f \in G^E, \alpha \in \Omega, x \in E).
$$

Soit $(\varphi_i : H \to G_i)_{i \in I}$ une famille d’homomorphismes de groupes à opérateurs. L’application $h \mapsto (\varphi_i(h))_{i \in I}$ de $H$ dans $\prod_{i \in I} G_i$ est un homomorphisme de groupes à opérateurs. C’est le seul homomorphisme $\Phi : H \to \prod_{i \in I} G_i$ vérifiant $\mathrm{pr}_i \circ \Phi = \varphi_i$ pour tout $i$. Ceci justifie le nom de groupe à opérateurs produit (E, IV, p. 16).

Soit $(\varphi_i : H_i \to G_i)_{i \in I}$ une famille d’homomorphismes de groupes à opérateurs. L’application $\prod_{i \in I} \varphi_i : (h_i)_{i \in I} \mapsto (\varphi_i(h_i))_{i \in I}$ de $\prod_{i \in I} H_i$ dans $\prod_{i \in I} G_i$ est un homomorphisme de groupes à opérateurs.

#### Proposition 11 {#alg-i-s4-prop-11 .statement}

Soit $(\varphi_i : H_i \to G_i)_{i \in I}$ une famille d’homomorphismes de groupes à opérateurs et posons $\Phi = \prod_{i \in I} \varphi_i$.

a) On a $\mathrm{Ker}(\Phi) = \prod_{i \in I} \mathrm{Ker}(\varphi_i)$; en particulier, si tous les $\varphi_i$ sont injectifs, $\Phi$ est injectif.

b) On a $\operatorname{Im}(\Phi) = \prod_{i \in I} \operatorname{Im}(\varphi_i)$; en particulier, si tous les $\varphi_i$ sont surjectifs, $\Phi$ est surjectif.
C’est immédiat.

En particulier, soit $(G_i)_{i \in I}$ une famille de groupes à opérateurs et, pour tout $i$, soit $H_i$ un sous-groupe stable (resp. stable distingué) de $G_i$. Le produit $\prod_{i \in I} H_i$ est un sous-groupe stable (resp. stable distingué) de $\prod_{i \in I} G_i$ et l’application canonique de $\prod_{i \in I} G_i$ sur $\prod_{i \in I} (G_i/H_i)$ définit par passage au quotient un isomorphisme de $(\prod_{i \in I} G_i)/(\prod_{i \in I} H_i)$ sur $\prod_{i \in I} (G_i/H_i)$. Par exemple, soit $J$ une partie de $I$. Le sous-ensemble $G_J$ de $\prod_{i \in I} G_i$ formé des $(x_i)_{i \in I}$ tels que $x_i = e_i$ pour $i \notin J$ est un sous-groupe stable distingué. L’application $\iota_J$ qui à $x = (x_j)_{j \in J}$ associe l’élément $y = (y_i)_{i \in I}$ tel que $y_i = e_i$ pour $i \notin J$ et $y_i = x_i$ pour $i \in J$, est un isomorphisme de $\prod_{j \in J} G_j$ sur $G_J$. L’application $\mathrm{pr}_{I-J}$ définit par passage au quotient un isomorphisme $\theta_J$ du groupe quotient $G/G_J$ sur $\prod_{i \in I-J} G_i$. Le composé $\mathrm{pr}_J \circ \iota_J$ est l’application identique de $\prod_{j \in J} G_j$. On identifie souvent $G/G_J$ à $\prod_{i \in I-J} G_i$ grâce à $\theta_J$, et $\prod_{i \in J} G_i$ à $G_J$ grâce à $\iota_J$.

Si $J_1$ et $J_2$ sont des parties disjointes de $I$, il résulte des définitions que tout élément de $G_{J_1}$ commute à tout élément de $G_{J_2}$.

#### Définition 13 {#alg-i-s4-def-13 .statement}

Soient $G$ un groupe à opérateurs et $(H_i)_{i \in I}$ une famille de sous-groupes stables distingués de $G$. Soit $p_i : G \to G/H_i$ l’homomorphisme canonique. On dit que $G$ est produit interne (ou produit) de la famille des groupes quotients $(G/H_i)$ si l’homomorphisme $g \mapsto (p_i(g))_{i \in I}$ est un isomorphisme de $G$ sur $\prod_{i \in I} G/H_i$.

Soient $G$ et $H$ des groupes à opérateurs, et soient $\varphi$ et $\psi$ deux homomorphismes de $G$ dans $H$. L’ensemble des éléments $x$ de $G$ tels que $\varphi(x) = \psi(x)$ est un sous-groupe stable de $G$, appelé groupe de coïncidence de $\varphi$ et $\psi$. En particulier, soient $\varphi_1 : G_1 \to H$ et $\varphi_2 : G_2 \to H$ des homomorphismes de groupes à opérateurs; le groupe de coïncidence des homomorphismes $\varphi_1 \circ \mathrm{pr}_1$ et $\varphi_2 \circ \mathrm{pr}_2$ de $G_1 \times G_2$ dans $H$ est appelé produit fibré de $G_1$ et $G_2$ sur $H$ relativement à $\varphi_1$ et $\varphi_2$. Il se note $G_1 \times_H G_2$ quand il n’y a pas d’ambiguïté sur $\varphi_1$ et $\varphi_2$, et les restrictions $p_1$ et $p_2$ de $\mathrm{pr}_1$ et $\mathrm{pr}_2$ à $G_1 \times_H G_2$ s’appellent encore homomorphismes de projection. On a $\varphi_1 \circ p_1 = \varphi_2 \circ p_2$. Les éléments de $G_1 \times_H G_2$ sont les couples $(x_1, x_2) \in G_1 \times G_2$ tels que $\varphi_1(x_1) = \varphi_2(x_2)$. Si $f_i$ est un homomorphisme d’un groupe à opérateurs $K$ dans $G_i$ ($i = 1, 2$) et si $\varphi_1 \circ f_1 = \varphi_2 \circ f_2$, il existe un homomorphisme $f$ et un seul de $K$ dans $G_1 \times_H G_2$ tel que $f_i = p_i \circ f$ pour $i = 1, 2$.

### 9. Sommes restreintes

Soit $(G_i)_{i \in I}$ une famille de groupes à opérateurs et, pour tout $i \in I$, soit $H_i$ un sous-groupe stable de $G_i$. Le sous-ensemble de $\prod_{i \in I} G_i$ formé des $(x_i)_{i \in I}$ tels que l’ensemble des $i \in I$ pour lesquels $x_i \notin H_i$ soit fini, est un sous-groupe stable de $\prod_{i \in I} G_i$ égal à $\prod_{i \in I} G_i$ si $I$ est fini. On l’appelle la somme restreinte des $G_i$ par rapport aux $H_i$. Lorsque, pour tous les $i$ sauf un nombre fini d’entre eux, $H_i$ est un sous-groupe stable distingué de $G_i$, la somme restreinte est un sous-groupe stable distingué du produit. Lorsque, pour tout $i$, le sous-groupe $H_i$ est réduit à l’élément neutre de $G_i$, la somme restreinte des $G_i$ par rapport aux $H_i$ s’appelle simplement somme restreinte des $G_i$ et se note parfois $\prod_{i \in I} G_i$. Pour tout $i_0 \in I$, l’application $\iota_{i_0}: G_{i_0} \to \prod_{i \in I} G_i$ définie par $\iota_{i_0}(x) = (x_i)_{i \in I}$, où $x_{i_0} = x$ et $x_i = e_i$ si $i \neq i_0$, est un homomorphisme injectif de groupes à opérateurs appelé injection canonique. On identifie $G_i$ au sous-groupe stable $\operatorname{Im}(\iota_i)$. Les sous-groupes $G_i$ sont distingués. Pour $i \neq j$, les éléments de $G_i$ et $G_j$ commutent et $G_i \cap G_j = \{e\}$. Le groupe $\prod_{i \in I} G_i$ est engendré par l’ensemble $\bigcup_{i \in I} G_i$.

#### Proposition 12 {#alg-i-s4-prop-12 .statement}

Soit $(\varphi_i: G_i \to K)_{i \in I}$ une famille d’homomorphismes de groupes à opérateurs telle que, quels que soient $i \in I$ et $j \in I$ avec $i \neq j$, $x \in G_i$, $y \in G_j$, les éléments $\varphi_i(x)$ et $\varphi_j(y)$ de $K$ commutent; il existe un homomorphisme de groupes à opérateurs $\Phi$ de $\prod_{i \in I} G_i$ dans $K$ et un seul tel que l’on ait $\varphi_i = \Phi \circ \iota_i$ pour tout $i \in I$. Pour tout élément $x = (x_i)_{i \in I}$ de $\prod_{i \in I} G_i$, on a $\Phi(x) = \prod_{i \in I} \varphi_i(x_i)$.

Si $\Phi$ et $\Psi$ répondent à la question, ils coïncident dans $\bigcup_{i \in I} G_i$, donc dans $\prod_{i \in I} G_i$, d’où l’unicité de $\Phi$. Démontrons l’existence de $\Phi$: pour tout élément $x = (x_i)_{i \in I}$ de $\prod_{i \in I} G_i$, posons $\Phi(x) = \prod_{i \in I} \varphi_i(x_i)$ (I, p. 9). Il est clair que $\Phi \circ \iota_i = \varphi_i$ pour tout $i$ et que $\Phi$ commute aux homothéties; la formule $\Phi(xy) = \Phi(x)\Phi(y)$ résulte de I, p. 10, formule (9).

#### Définition 14 {#alg-i-s4-def-14 .statement}

Soient $G$ un groupe à opérateurs et $(H_i)_{i \in I}$ une famille de sous-groupes stables de $G$. On dit que $G$ est somme restreinte interne (ou somme restreinte) de la famille de sous-groupes $(H_i)$ si tout élément de $H_i$ est permutable avec tout élément de $H_j$ pour $j \neq i$ et si l’unique homomorphisme de $\prod_{i \in I} H_i$ dans $G$ dont la restriction à chaque $H_i$ est l’injection canonique est un isomorphisme.

Lorsque $I$ est fini, on dit aussi, par abus de langage, produit direct interne (ou produit direct, ou produit) au lieu de somme restreinte interne. Tout sous-groupe stable $H$ de $G$ pour lequel il existe un sous-groupe stable $H'$ de $G$ tel que $G$ soit produit direct de $H$ et $H'$ est appelé facteur direct de $G$.

#### Proposition 13 {#alg-i-s4-prop-13 .statement}

*Soient G un groupe à opérateurs et $(H_i)_{i \in I}$ une famille de sous-groupes stables de G telle que tout élément de $H_i$ soit permutable avec tout élément de $H_j$ pour $j \neq i$. Pour que G soit somme restreinte de la famille de sous-groupes $(H_i)_{i \in I}$, il faut et il suffit que tout élément x de G se mette, de façon unique, sous la forme $\prod_{i \in I} y_i$, où $(y_i)_{i \in I}$ est une famille à support fini d’éléments de G telle que $y_i \in H_i$ pour tout i.*

C’est évident.

#### Proposition 14 {#alg-i-s4-prop-14 .statement}

*Soient G un groupe à opérateurs et $(H_i)_{i \in I}$ une famille finie de sous-groupes stables de G. Pour que G soit somme restreinte de la famille de sous groupes $(H_i)$, il faut et il suffit que chaque $H_i$ soit distingué et que G soit produit des groupes quotients $G/H^i$, où $H^i$ est le sous-groupe engendré par les $H_j$ pour $j \neq i$.

La condition est évidemment nécessaire. Réciproquement, supposons G produit des $K_i = G/H^i$, et identifions G au produit des $K_i$. Alors $H_i$ s’identifie à un sous-groupe de $K_i$, de sorte que, pour $i \neq j$, tout élément de $H_i$ est permutable à tout élément de $H_j$; d’autre part, $H^i$ s’identifie au produit des $K_j$ pour $j \neq i$, donc $H_i = K_i$ pour tout $i$ et G est produit direct des $H_i$.

#### Proposition 15 {#alg-i-s4-prop-15 .statement}

*Soient G un groupe à opérateurs et $(H_i)_{1 \leq i \leq n}$ une suite de sous-groupes stables distingués de G telle que*

$$(H_1 H_2 \ldots H_i) \cap H_{i+1} = \{e\} \quad \text{pour } 1 \leq i \leq n - 1.$$

*L’ensemble $H_1 H_2 \ldots H_n$ est un sous-groupe stable distingué de G, somme restreinte des $H_i$*

Par récurrence sur $n$, on se ramène aussitôt à démontrer la proposition pour $n = 2$. Montrons d’abord que, si $x \in H_1$, $y \in H_2$, $x$ et $y$ sont *permutables*; en effet, on a $xyx^{-1}y^{-1} = (xyx^{-1})y^{-1} = x(yx^{-1}y^{-1})$ donc ($H_1$ et $H_2$ étant distingués) $xyx^{-1}y^{-1} \in H_1 \cap H_2$, c’est-à-dire $xyx^{-1}y^{-1} = e$, d’après l’hypothèse. Par ailleurs $H_1 H_2$ est une partie de G stable par les homothéties de G. Il en résulte (I, p. 31, prop. 1) que $H_1 H_2$ est un sous-groupe stable de G, et on vérifie immédiatement que ce sous-groupe est distingué. Supposons enfin qu’on ait $xy = x'y'$, avec $x \in H_1$, $x' \in H_1$, $y \in H_2$, $y' \in H_2$; on en tire ${x'}^{-1}x = y'y^{-1}$, donc ${x'}^{-1}x \in H_1 \cap H_2 = \{e\}$, $x' = x$, et de même $y' = y$; $H_1 H_2$ est bien produit direct de $H_1$ et $H_2$.

Lorsque les groupes considérés sont commutatifs, on emploie le terme de *somme directe* au lieu de somme restreinte.

### 10. Groupes monogènes

Soit $a \in \mathbf{Z}$; puisque $a\mathbf{Z}$ est un sous-groupe de $\mathbf{Z}$, la relation entre éléments $x, y$ de $\mathbf{Z}$ qui s’énonce « il existe $z \in \mathbf{Z}$ tel que $x - y = az$ » est une relation d’équivalence, que l’on convient, une fois pour toutes, d’écrire $x \equiv y$ (mod. $a$) ou plus brièvement $x \equiv y$ (*a*), et qui s’appelle une *congruence modulo* $a$. En remplaçant $a$ par $-a$, on obtient une relation équivalente, donc on pourra supposer $a \geq 0$; pour $a = 0$, $x \equiv y$ (0) signifie $x = y$, donc on n’aura de relation distincte de l’égalité que si $a \neq 0$: aussi supposerons-nous par la suite que $a > 0$ sauf indication formelle du contraire.

Pour $a > 0$, le quotient de $\mathbf{Z}$ par la congruence $x \equiv y \ (a)$, c’est-à-dire le groupe $\mathbf{Z}/a\mathbf{Z}$, s’appelle le *groupe des entiers rationnels modulo* $a$.

#### Proposition 16 {#alg-i-s4-prop-16 .statement}

*Soit* $a$ *un entier* $> 0$. *Les entiers* $r$ *tels que* $0 \leq r < a$ *forment un système de représentants de la relation d’équivalence* $x \equiv y \ (\text{mod. } a)$ *dans* $\mathbf{Z}$.

Si $x$ est un entier $\geq 0$, il existe (E, III, p. 39) des entiers $q$ et $r$ tels que $x = aq + r$ et $0 \leq r < a$, et on a $x \equiv r \ (\text{mod. } a)$. Si $x$ est un entier $\leq 0$, l’entier $-x$ est $\geq 0$, et d’après ce qui précède, il existe un entier $r$ tel que $0 \leq r < a$ et $-x \equiv r \ (\text{mod. } a)$. Posons $r' = 0$ si $r = 0$ et $r' = a - r$ si $r > 0$; on a

$$
x \equiv -r \equiv r' \ (\text{mod. } a)
$$

et $0 \leq r' < a$. Montrons maintenant que si $0 \leq r < r' < a$, on a $r \not\equiv r' \ (\text{mod. } a)$. On a $r' - r < na$ pour $n \geq 1$ et $r' - r > na$ pour $n \leq 0$, d’où $-r \notin a\mathbf{Z}$.

#### Corollaire {#alg-i-s4-n10-cor-1 .statement}

*Soit* $a$ *un entier* $> 0$. *Le groupe* $\mathbf{Z}/a\mathbf{Z}$ *des entiers rationnels modulo* $a$ *est un groupe d’ordre* $a$.

#### Proposition 17 {#alg-i-s4-prop-17 .statement}

*Soit* $\mathbf{H}$ *un sous-groupe de* $\mathbf{Z}$. *Il existe un entier* $a \geq 0$ *et un seul tel que* $\mathbf{H} = a\mathbf{Z}$.

Si $\mathbf{H} = \{0\}$, on a $\mathbf{H} = 0\mathbf{Z}$. Supposons $\mathbf{H} \neq \{0\}$. Le sous-groupe $\mathbf{H}$ possède un élément $x \neq 0$. On a $x > 0$ ou $-x > 0$, et par suite $\mathbf{H}$ possède des éléments $> 0$. Soit $a$ le plus petit élément $> 0$ de $\mathbf{H}$. Le sous-groupe $a\mathbf{Z}$ engendré par $a$ est contenu dans $\mathbf{H}$; montrons que $\mathbf{H} \subset a\mathbf{Z}$. Soit $y \in \mathbf{H}$. D’après la prop. 16, il existe un entier $r$ tel que $y \equiv r \ (\text{mod. } a)$ et $0 \leq r < a$. *A fortiori*, $y \equiv r \ (\text{mod. } \mathbf{H})$, d’où $r \in \mathbf{H}$. Mais ceci n’est possible que si $r = 0$, et par suite $y \in a\mathbf{Z}$. L’entier $a$ est unique : si $\mathbf{H} = \{0\}$, on a nécessairement $a = 0$, et si $\mathbf{H} \neq \{0\}$, l’entier $a$ est l’ordre de $\mathbf{Z}/\mathbf{H}$.

#### Définition 15 {#alg-i-s4-def-15 .statement}

*On dit qu’un groupe est monogène s’il admet un système générateur réduit à un élément*. *Un groupe monogène fini est dit cyclique*.

Tout groupe monogène est commutatif (I, p. 32, cor. 2). Tout groupe quotient d’un groupe monogène est monogène (I, p. 32, cor. 3).

Le groupe additif $\mathbf{Z}$ est monogène : il est engendré par $\{1\}$. Pour tout entier positif $a$, le groupe $\mathbf{Z}/a\mathbf{Z}$ est monogène, car c’est un quotient de $\mathbf{Z}$.

#### Proposition 18 {#alg-i-s4-prop-18 .statement}

*Un groupe monogène fini d’ordre* $a$ *est isomorphe à* $\mathbf{Z}/a\mathbf{Z}$. *Un groupe monogène infini est isomorphe à* $\mathbf{Z}$.

Soient $G$ un groupe monogène (noté multiplicativement) et $x$ un générateur de $G$. L’identité $x^m x^n = x^{m+n}$ (I, p. 6, formule (4)) montre que l’application $n \mapsto x^n$ est un homomorphisme de $\mathbf{Z}$ dans $G$. Son image est un sous-groupe de $G$ contenant $x$, donc c’est $G$. D’après I, p. 36, th. 3, le groupe $G$ est isomorphe au quotient de $\mathbf{Z}$ par un sous-groupe, qui est nécessairement de la forme $a\mathbf{Z}$ (prop. 17). Si $a > 0$, le groupe $G$ est fini d’ordre $a$, et si $a = 0$, le groupe $G$ est isomorphe à $\mathbf{Z}$.

#### Proposition 19 {#alg-i-s4-prop-19 .statement}

Soit $a$ un entier $> 0$. Soient $H$ un sous-groupe de $\mathbf{Z}/a\mathbf{Z}$, $b$ l’ordre de $H$ et $c$ son indice dans $\mathbf{Z}/a\mathbf{Z}$. On a $a = bc$, $H = c\mathbf{Z}/a\mathbf{Z}$, et $H$ est isomorphe à $\mathbf{Z}/b\mathbf{Z}$.

Réciproquement, soient $b$ et $c$ deux entiers $> 0$ tels que $a = bc$. On a $a\mathbf{Z} \subset c\mathbf{Z}$, et $c\mathbf{Z}/a\mathbf{Z}$ est un sous-groupe de $\mathbf{Z}/a\mathbf{Z}$, d’ordre $b$ et d’indice $c$.

On a $a = bc$ (I, p. 34, corollaire). D’après I, p. 39, $H$ est de la forme $H'/a\mathbf{Z}$, où $H'$ est un sous-groupe de $\mathbf{Z}$, et $\mathbf{Z}/H'$ est isomorphe à $(\mathbf{Z}/a\mathbf{Z})/H$, donc d’ordre $c$. D’après la prop. 17 et le cor. de la prop. 16 (I, p. 47), on a $H' = c\mathbf{Z}$, donc $H$ est monogène. Enfin $H$ est isomorphe à $\mathbf{Z}/b\mathbf{Z}$ d’après la prop. 18. Réciproquement, si $a = bc$, on a $a\mathbf{Z} \subset c\mathbf{Z}$ car $a \in c\mathbf{Z}$; le groupe quotient $(\mathbf{Z}/a\mathbf{Z})/(c\mathbf{Z}/a\mathbf{Z})$ est isomorphe à $\mathbf{Z}/c\mathbf{Z}$ (I, p. 39, th. 4), donc d’ordre $c$ (I, p. 34, corollaire), et d’indice $b$ (I, p. 34, corollaire).

#### Corollaire {#alg-i-s4-n10-cor-2 .statement}

Tout sous-groupe d’un groupe monogène est monogène.

Soient $a$ et $b$ deux entiers $\neq 0$. La relation $b \in a\mathbf{Z}$ s’écrit aussi : $b$ est un multiple de $a$, ou encore $a$ divise $b$ ou bien encore $a$ est un diviseur de $b$.

#### Définition 16 {#alg-i-s4-def-16 .statement}

On dit qu’un entier $p > 0$ est premier si $p \neq 1$ et s’il n’admet pas de diviseur $> 1$ autre que $p$.

#### Proposition 20 {#alg-i-s4-prop-20 .statement}

Un entier $p > 0$ est premier si et seulement si le groupe $\mathbf{Z}/p\mathbf{Z}$ est un groupe simple.

Cela résulte de la prop. 19.

#### Corollaire {#alg-i-s4-n10-cor-3 .statement}

Tout groupe simple commutatif est cyclique d’ordre premier.

Soit $G$ un tel groupe. On a $G \neq \{e\}$; soit $a \neq e$ un élément de $G$. Le sous-groupe engendré par $a$ est distingué car $G$ est commutatif, non réduit à $\{e\}$, donc égal à $G$. Par suite $G$ est monogène, donc isomorphe à un groupe de la forme $\mathbf{Z}/p\mathbf{Z}$, avec $p > 0$, car $\mathbf{Z}$ n’est pas simple, et $p$ est nécessairement premier.

#### Remarque {#alg-i-s4-n10-rem-1 .statement}

Un groupe fini $G$ d’ordre premier est nécessairement cyclique. En effet, $G$ n’admet pas d’autre sous-groupe que $G$ et $\{e\}$, donc il est engendré par tout élément $\neq e$.

#### Lemme 2 {#alg-i-s4-lem-2 .statement}

Soit $a$ un entier $> 0$. En associant à toute suite de composition $(H_i)_{0 \leq i \leq n}$ du groupe $\mathbf{Z}/a\mathbf{Z}$ la suite $(s_i)_{1 \leq i \leq n}$, où $s_i$ est l’ordre de $H_{i-1}/H_i$, on obtient une application bijective de l’ensemble des suites de composition de $\mathbf{Z}/a\mathbf{Z}$ sur l’ensemble des suites finies $(s_i)$ d’entiers $> 0$ telles que $a = s_1 \ldots s_n$. La suite de composition $(H_i)_{0 \leq i \leq n}$ est une suite de Jordan-Hölder si et seulement si les $s_i$ sont premiers.

Si $(H_i)_{0 \leq i \leq n}$ est une suite de composition de $\mathbf{Z}/a\mathbf{Z}$, il résulte, par récurrence sur $n$, de I, p. 34, prop. 4, que $a = \prod_{i=1}^n (H_{i-1}: H_i)$.

Réciproquement, soit $(s_i)_{1 \leq i \leq n}$ une suite d’entiers $> 0$ telle que $a = s_1 \ldots s_n$. Si $(H_i)_{0 \leq i \leq n}$ est une suite de composition de $\mathbf{Z}/a\mathbf{Z}$ telle que $(H_{i-1}: H_i) = s_i$ pour $1 \leq i \leq n$, on a nécessairement $((\mathbf{Z}/a\mathbf{Z}): H_i) = \prod_{1 \leq j \leq i} s_j$ comme on le voit par récurrence sur $i$, d’où $H_i = (\prod_{j=1}^i s_j)\mathbf{Z}/a\mathbf{Z}$ (I, p. 47, prop. 19), ce qui montre l’injectivité de l’application considérée. Montrons sa surjectivité: en posant $H_i = (\prod_{j=1}^i s_j) \mathbf{Z}/a\mathbf{Z}$ pour $0 \leq i \leq n$, on obtient une suite de composition de $\mathbf{Z}/a\mathbf{Z}$ telle que $(H_{i-1}: H_i) = s_i$ (I, p. 47, prop. 19). La deuxième assertion du lemme résulte de I, p. 48, prop. 20 et I, p. 41, prop. 9.

Notons $\mathfrak{P}$ l’ensemble des entiers premiers.

**Théorème 7** (décomposition en facteurs premiers). — *Soit a un entier strictement positif. Il existe une famille $(v_p(a))_{p \in \mathfrak{P}}$ d’entiers $\geq 0$ et une seule telle que l’ensemble des $p \in \mathfrak{P}$ pour lesquels $v_p(a) \neq 0$ soit fini et que l’on ait*

$$
a = \prod_{p \in \mathfrak{P}} p^{v_p(a)}.
$$

Comme le groupe $\mathbf{Z}/a\mathbf{Z}$ est fini, il admet une suite de Jordan-Hölder. Le lemme 2 (I, p. 48) entraîne alors que $a$ est produit d’entiers premiers, d’où l’existence de la famille $(v_p(a))$; de plus, pour toute famille $(v_p(a))_{p \in \mathfrak{P}}$ satisfaisant aux conditions du th. 7, l’entier $v_p(a)$ est, pour tout $p \in \mathfrak{P}$, égal au nombre de facteurs d’une suite de Jordan-Hölder de $\mathbf{Z}/a\mathbf{Z}$ isomorphes à $\mathbf{Z}/p\mathbf{Z}$ (lemme 2). L’unicité de la famille $(v_p(a))$ résulte donc du théorème de Jordan-Hölder (I, p. 41, th. 6).

#### Corollaire {#alg-i-s4-n10-cor-4 .statement}

*Soient a et b deux entiers $> 0$. On a $v_p(ab) = v_p(a) + v_p(b)$. Pour que a divise b il faut et il suffit que $v_p(a) \leq v_p(b)$ pour tout nombre premier p.*

Dans un groupe quelconque G, si le sous-groupe (monogène) engendré par un élément $x \in G$ est d’ordre fini d, on dit que $x$ est un élément d’ordre d; le nombre d est donc le plus petit entier $> 0$ tel que $x^d = e$; si le sous-groupe engendré par $x$ est infini, on dit que $x$ est d’ordre infini. Ces définitions, et la prop. 4 (I, p. 34), entraînent en particulier que, dans un groupe fini G, l’ordre de tout élément de G est un *diviseur* de l’ordre de G.

#### Proposition 21 {#alg-i-s4-prop-21 .statement}

*Dans un groupe fini G d’ordre n, on a $x^n = e$ pour tout $x \in G$.*
En effet, si $p$ est l’ordre de $x$, on a $n = pq$, avec q entier, donc $x^n = (x^p)^q = e$.

## EXERCICES {#alg-i-s4-exercises}

See the [exercises for § 4](exercises/s4/).
