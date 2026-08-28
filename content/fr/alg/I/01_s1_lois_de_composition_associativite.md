---
book: alg
book_title: Algebra
chapter: I
chapter_title: STRUCTURES ALGÉBRIQUES
section: 1
section_title: Lois de composition ; associativité ; commutativité
lang: fr
source: alg-i-iii-fr
pdf_pages: 0011-0022, 0128-0129
extraction: ocr
subsections:
    - "no": 1
      title: Lois de composition
      page: 0
      pdf_page: 11
    - "no": 2
      title: Composé d’une séquence d’éléments
      page: 3
      pdf_page: 13
    - "no": 3
      title: Lois associatives
      page: 4
      pdf_page: 14
    - "no": 4
      title: Parties stables. Lois induites
      page: 6
      pdf_page: 16
    - "no": 5
      title: Eléments permutables. Lois commutatives
      page: 7
      pdf_page: 17
    - "no": 6
      title: Lois quotients
      page: 10
      pdf_page: 20
statements: 31
exercises: 16
content_sha256: 9bf5da9f5a0e6717b3426434925ad79cb690c3a40d6527c17d75cd18b28d0942
---

## § 1. LOIS DE COMPOSITION; ASSOCIATIVITÉ; COMMUTATIVITÉ

### 1. Lois de composition

#### Définition 1 {#alg-i-s1-def-1 .statement}

Soit E un ensemble. On appelle loi de composition sur E une application f de E × E dans E. La valeur f(x, y) de f pour un couple (x, y) ∈ E × E s’appelle le composé de x et de y pour cette loi. Un ensemble muni d’une loi de composition est appelé un magma.

Le composé de x et de y se note le plus souvent en écrivant x et y dans un ordre déterminé et en les séparant par un signe caractéristique de la loi envisagée (signe qu’on pourra convenir d’omettre). Parmi les signes dont l’emploi est le plus fréquent, citons + et . , étant convenu en général que ce dernier peut s’omettre à volonté; avec ces signes, le composé de x et y s’écrira respectivement x + y, et x.y ou xy. Une loi notée par le signe + s’appelle le plus souvent addition (le composé x + y s’appelant alors la somme de x et de y) et on dit qu’elle est notée additivement; une loi notée par le signe . s’appelle le plus souvent multiplication (le composé x.y = xy s’appelant alors produit de x et de y), et on dit qu’elle est notée multiplicativement. Dans les raisonnements généraux des paragraphes 1 à 3 du présent chapitre, on se servira ordinairement des signes ⊔ et ⊓ pour noter des lois de composition quelconques.

On dit parfois, par abus de langage, qu’une application d’une partie de E × E dans E est une loi de composition non partout définie dans E.

#### Exemple 1 {#alg-i-s1-n1-exa-1 .statement}

Les applications (X, Y) ↦ X ∪ Y et (X, Y) ↦ X ∩ Y sont des lois de composition sur l’ensemble des parties d’un ensemble E.
2) Dans l’ensemble N des entiers naturels, l’addition, la multiplication, l’exponentiation sont des lois de composition (les composés de x ∈ N et de y ∈ N pour ces lois se notant respectivement x + y, xy ou x.y, et x^y) (E, III, p. 27–28).

3) Soit E un ensemble ; l’application (X, Y) ↦ X ○ Y est une loi de composition sur l’ensemble des parties de E × E (E, II, p. 11, déf. 6) ; l’application (f, g) ↦ f ○ g est une loi de composition sur l’ensemble des applications de E dans E (E, II, p. 31).

4) Soit E un ensemble ordonné réticulé (E, III, p. 13) ; si on désigne par sup(x, y) la borne supérieure de l’ensemble {x, y}, l’application (x, y) ↦ sup(x, y) est une loi de composition sur E. De même pour la borne inférieure inf(x, y). L’exemple 1 ci-dessus est un cas particulier de celui-ci, en considérant $\mathfrak{P}(E)$ comme ordonné par inclusion.

5) Soit $(E_i)_{i \in I}$ une famille de magmas. Notons $\tau_i$ la loi de composition sur $E_i$. L’application
$$
((x_i), (y_i)) \mapsto ((x_i \tau_i y_i))
$$
est une loi de composition sur le produit $E = \prod_{i \in I} E_i$, appelée *produit* des lois $\tau_i$. L’ensemble E, muni de cette loi, s’appelle le *magma produit* des magmas $E_i$. En particulier, si tous les magmas $E_i$ sont égaux à un même magma M, on obtient le *magma des applications de I dans M*.

Soit $(x, y) \mapsto x \top y$ une loi de composition sur un ensemble E. Etant données deux parties quelconques X, Y de E, on désignera par $X \top Y$ (pourvu que cette notation ne prête pas à confusion¹) l’ensemble des éléments $x \top y$ de E, tels que $x \in X, y \in Y$ (autrement dit, l’image de $X \times Y$ par l’application $(x, y) \mapsto x \top y$).

Si $a \in E$, on écrit généralement $a \top Y$ au lieu de $\{a\} \top Y$, et $X \top a$ au lieu de $X \top \{a\}$. L’application $(X, Y) \mapsto X \top Y$ est une loi de composition sur l’ensemble des parties de E.

#### Définition 2 {#alg-i-s1-def-2 .statement}

*Soit E un magma. Notons $\tau$ sa loi de composition. La loi de composition $(x, y) \mapsto y \top x$ sur E est dite opposée à la précédente. L’ensemble E, muni de cette loi, est appelé magma opposé de E.*

Soient E et E′ deux magmas; nous noterons leurs lois par le même signe $\tau$. Conformément aux définitions générales (E, IV, p. 6), on appelle *isomorphisme de E sur E′* une application bijective $f$ de E sur E′, telle que
$$
f(x \top y) = f(x) \top f(y)
$$
pour tout couple $(x, y) \in E \times E$. On dit que E et E′ sont *isomorphes* s’il existe un isomorphisme de E sur E′.

Plus généralement:

#### Définition 3 {#alg-i-s1-def-3 .statement}

*On appelle homomorphisme, ou morphisme, de E dans E′ une application f de E dans E′ telle que la relation (1) soit vérifiée pour tout couple $(x, y) \in E \times E$; lorsque $E = E'$, on dit que f est un endomorphisme de E.*

L’application identique d’un magma E est un homomorphisme, le composé de deux homomorphismes est un homomorphisme.

Pour qu’une application $f$ de E dans E′ soit un isomorphisme, il faut et il

¹ Voici un exemple où ce principe de notation prêterait à confusion et ne devra donc pas s’appliquer. Supposons qu’il s’agisse de la loi de composition $(A, B) \mapsto A \cup B$ entre parties d’un ensemble E ; on en déduit une loi de composition $(\mathcal{A}, \mathcal{B}) \mapsto F(\mathcal{A}, \mathcal{B})$, entre parties de $\mathfrak{P}(E)$, $F(\mathcal{A}, \mathcal{B})$ étant l’ensemble des $A \cup B$ pour $A \in \mathcal{A}, B \in \mathcal{B}$ ; mais $F(\mathcal{A}, \mathcal{B})$ ne devra pas se noter $\mathcal{A} \cup \mathcal{B}$, cette notation ayant déjà un sens différent (réunion de $\mathcal{A}$ et $\mathcal{B}$ considérées comme parties de $\mathfrak{P}(E)$).

suffit que ce soit un homomorphisme bijectif, et $f^{-1}$ est alors un isomorphisme de $E'$ sur $E$.

### 2. Composé d’une séquence d’éléments

Rappelons qu’une famille d’éléments d’un ensemble $E$ est une application $i \mapsto x_i$ d’un ensemble $I$ (dit ensemble d’indices) dans $E$; on dit qu’une famille $(x_i)_{i \in I}$ est finie si l’ensemble d’indices est fini.

On appelle séquence d’éléments de $E$ une famille finie $(x_i)_{i \in I}$ d’éléments de $E$ dont l’ensemble d’indices $I$ est totalement ordonné.

En particulier, toute suite finie $(x_i)_{i \in H}$, où $H$ est une partie finie de l’ensemble $\mathbf{N}$ des entiers naturels, peut être considérée comme une séquence, en munissant $H$ de la relation d’ordre induite par la relation $m \leq n$ entre entiers naturels.

On dit que deux séquences $(x_i)_{i \in I}$ et $(y_k)_{k \in K}$ sont semblables s’il existe un isomorphisme $\varphi$ d’ensembles ordonnés de $I$ sur $K$ tel que $y_{\varphi(i)} = x_i$ pour tout $i \in I$.

Toute séquence $(x_\alpha)_{\alpha \in A}$ est semblable à une suite finie convenable. En effet, il existe une bijection croissante de $A$ sur un intervalle $[0, n]$ de $\mathbf{N}$.

#### Définition 4 {#alg-i-s1-def-4 .statement}

Soit $(x_\alpha)_{\alpha \in A}$ une séquence d’éléments d’un magma $E$ dont l’ensemble d’indices $A$ est non vide. On appelle composé (pour la loi $\top$) de la séquence $(x_\alpha)_{\alpha \in A}$, et on note $\prod_{\alpha \in A} x_\alpha$, l’élément de $E$ défini par récurrence sur le nombre d’éléments de $A$, de la façon suivante:

1° si $A = \{\beta\}$, alors $\prod_{\alpha \in A} x_\alpha = x_\beta$;
2° si $A$ a $p > 1$ éléments, si $\beta$ est le plus petit élément de $A$, et si $A' = A - \{\beta\}$, alors $\prod_{\alpha \in A} x_\alpha = x_\beta \top (\prod_{\alpha \in A'} x_\alpha)$.

Il est immédiat (par récurrence sur le nombre d’éléments des ensembles d’indices) que les composés de deux séquences semblables sont égaux; en particulier, le composé d’une séquence quelconque est égal au composé d’une suite finie.

Si $A = \{\lambda, \mu, \nu\}$ a trois éléments ($\lambda < \mu < \nu$) le composé $\prod_{\alpha \in A} x_\alpha$ est $x_\lambda \top (x_\mu \top x_\nu)$.

#### Remarque {#alg-i-s1-n2-rem-1 .statement}

On notera qu’il y a un certain arbitraire dans la définition du composé d’une séquence; la récurrence que nous avons introduite procède « de droite à gauche ». Si on procédait « de gauche à droite », le composé de la séquence $(x_\lambda, x_\mu, x_\nu)$ ci-dessus serait $(x_\lambda \top x_\mu) \top x_\nu$.

Quand on utilise d’autres notations, le composé d’une séquence $(x_\alpha)_{\alpha \in A}$ s’écrit $\prod_{\alpha \in A} x_\alpha$ pour une loi notée $\perp$; pour une loi notée additivement, il est d’usage de le désigner par $\sum_{\alpha \in A} x_\alpha$, et de l’appeler la somme de la séquence $(x_\alpha)_{\alpha \in A}$ (les $x_\alpha$ étant appelés les termes de la somme); pour une loi notée multiplicativement, on le désigne le plus souvent par la notation $\prod_{\alpha \in A} x_\alpha$, et on l’appelle le *produit* de la séquence $(x_\alpha)$ (les $x_\alpha$ étant appelés les *facteurs* du produit)¹.

Lorsqu’il n’y a pas de confusion possible sur l’ensemble d’indices (ni sur sa structure d’ordre) on se dispense souvent de l’écrire dans la notation du composé d’une séquence et on écrit donc, par exemple pour une loi notée additivement, $\sum_\alpha x_\alpha$ au lieu de $\sum_{\alpha \in A} x_\alpha$; de même pour les autres notations.

Pour une loi notée $\tau$, le composé d’une *suite* $(x_i)$, ayant pour ensemble d’indices un intervalle $[p, q]$ non vide de $\mathbf{N}$, se note $\prod_{p \leq i \leq q} x_i$, ou $\prod_{i=p}^{q} x_i$; de même pour les lois notées par d’autres signes.

Soient E et F deux magmas, dont les lois sont notées $\tau$, et $f$ un homomorphisme de E dans F. Pour toute séquence $(x_\alpha)_{\alpha \in A}$ d’éléments de E, on a

(2)
$$
f\left( \prod_{\alpha \in A} x_\alpha \right) = \prod_{\alpha \in A} f(x_\alpha).
$$

### 3. Lois associatives

#### Définition 5 {#alg-i-s1-def-5 .statement}

*Une loi de composition* $(x, y) \mapsto x \tau y$ *sur un ensemble* E *est dite associative si, quels que soient les éléments* $x, y, z$ *de* E, *on a*
$$
(x \tau y) \tau z = x \tau (y \tau z).
$$
*Un magma dont la loi est associative est appelé magma associatif.*

La loi opposée à une loi associative est associative.

#### Exemple 1 {#alg-i-s1-n3-exa-1 .statement}

L’addition et la multiplication des entiers naturels sont des lois de composition associatives sur $\mathbf{N}$ (E, III, p. 27, corollaire).

#### Exemple 2 {#alg-i-s1-n3-exa-2 .statement}

Les lois citées aux exemples 1), 3) et 4) de I, p. 1–2 sont associatives.

**Théorème 1** (Théorème d’associativité). — *Soit* E *un magma associatif dont la loi est notée* $\tau$. *Soit* A *un ensemble fini non vide, totalement ordonné, réunion d’une séquence de parties non vides* $(B_i)_{i \in I}$ *telles que les relations* $\alpha \in B_i, \beta \in B_j, i < j$ *entraînent* $\alpha < \beta$; *soit* $(x_\alpha)_{\alpha \in A}$ *une séquence d’éléments de* E, *ayant* A *pour ensemble d’indices*. *On a*

(3)
$$
\prod_{\alpha \in A} x_\alpha = \prod_{i \in I} \left( \prod_{\alpha \in B_i} x_\alpha \right).
$$

¹ L’emploi de ce terme et de la notation $\prod_{\alpha \in A} x_\alpha$ devra être évité lorsqu’il risque de créer des confusions avec le produit des ensembles $x_\alpha$ défini en théorie des ensembles (E, II, p. 32). Cependant, lorsque les $x_\alpha$ sont des cardinaux, et que l’addition (resp. la multiplication) est la somme cardinale (resp. le produit cardinal), le cardinal désigné par $\sum_{\alpha \in A} x_\alpha$ (resp. $\prod_{\alpha \in A} x_\alpha$) avec la notation ci-dessus est la somme cardinale (resp. le produit cardinal) de la famille $(x_\alpha)_{\alpha \in A}$ (E, III, p. 25–26).

Démontrons le théorème par récurrence sur le cardinal $n$ de $A$. Soient $p$ le cardinal de $I$ et $h$ son plus petit élément; posons $J = I - \{h\}$. Si $n = 1$, on a nécessairement $p = 1$, puisque les $B_i$ ne sont pas vides, et le théorème est évident. Sinon, le théorème étant supposé vrai pour un ensemble d’indices ayant au plus $n - 1$ éléments, distinguons deux cas:

a) $B_h$ a un seul élément $\beta$. Posons $C = \bigcup_{i \in J} B_i$. Le premier membre de (3) est égal, par définition, à $x_\beta \top (\prod_{\alpha \in C} x_\alpha)$; le second membre est égal, par définition, à
$$
x_\beta \top (\prod_{i \in J} (\prod_{\alpha \in B_i} x_\alpha));
$$
l’égalité résulte de ce que le théorème est supposé vrai pour $C$ et $(B_i)_{i \in J}$.

b) Sinon, soit $\beta$ le plus petit élément de $A$ (donc de $B_h$); soit $A' = A - \{\beta\}$, et soit $B'_i = A' \cap B_i$ pour $i \in I$; on a $B'_i = B_i$ pour $i \in J$. L’ensemble $A'$ a $n - 1$ éléments, et les conditions du théorème sont satisfaites par $A'$ et ses parties $B'_i$; on a donc par hypothèse:
$$
\prod_{\alpha \in A'} x_\alpha = (\prod_{\alpha \in B'_h} x_\alpha) \top (\prod_{i \in J} (\prod_{\alpha \in B_i} x_\alpha)).
$$
Formons le composé de $x_\beta$ et de chacun des deux membres: au premier membre, on obtient par définition $\prod_{\alpha \in A} x_\alpha$; au second, on obtient, en utilisant l’associativité,
$$
(x_\beta \top (\prod_{\alpha \in B'_h} x_\alpha)) \top (\prod_{i \in J} (\prod_{\alpha \in B_i} x_\alpha))
$$
ce qui est égal, d’après la définition 3, au second membre de la formule (3).

Pour une loi associative notée $\top$, le composé $\prod_{p \leq i \leq q} x_i$ d’une suite $(x_i)_{i \in [p, q]}$ se note encore (lorsqu’aucune confusion n’est possible)
$$
x_p \top \cdots \top x_q.
$$
Un cas particulier du th. 1 est la formule
$$
x_0 \top x_1 \top \cdots \top x_n = (x_0 \top x_1 \top \cdots \top x_{n-1}) \top x_n.
$$
Considérons une séquence de $n$ termes dont tous les termes sont égaux à un même élément $x \in E$. Le composé de cette séquence se note $\prod^n x$ pour une loi notée $\top$, $\perp x$ pour une loi notée $\perp$. Pour une loi notée multiplicativement, le composé se note $x^n$ et s’appelle *puissance n-ème* de $x$. Pour une loi notée additive-ment, le composé se note le plus souvent $nx$ et s’appelle *n-uple* de $x$. Le théorème d’associativité, appliqué à une séquence dont tous les termes sont égaux, donne la formule
$$
\prod^{n_1 + n_2 + \cdots + n_p} x = (\prod^{n_1} x) \top (\prod^{n_2} x) \top \cdots \top (\prod^{n_p} x).
$$

En particulier, si $p = 2$,

$$
\text{(4)} \quad \tau^{m+n} x = (\tau^m x) \tau (\tau^n x)
$$

et, si $n_1 = n_2 = \cdots = n_p = m$,

$$
\text{(5)} \quad \tau^{pm} x = \tau^p (\tau^m x).
$$

Si $X$ est une partie de $E$, on désigne parfois, conformément aux notations ci-dessus, par $\tau^p X$ l’ensemble $X_1 \tau X_2 \tau \cdots \tau X_p$ où

$$
X_1 = X_2 = \cdots = X_p = X;
$$

c’est donc l’ensemble de tous les composés $x_1 \tau x_2 \tau \cdots \tau x_p$, pour $x_1 \in X$, $x_2 \in X, \ldots, x_p \in X$.

Il importe de ne pas confondre cet ensemble avec l’ensemble des $\tau^p x$, où $x$ parcourt $X$.

### 4. Parties stables. Lois induites

#### Définition 6 {#alg-i-s1-def-6 .statement}

Une partie $A$ d’un ensemble $E$ est dite stable pour une loi de composition $\tau$ sur $E$ si le composé de deux éléments de $A$ appartient à $A$. L’application $(x, y) \mapsto x \tau y$ de $A \times A$ dans $A$ s’appelle alors la loi induite sur $A$ par la loi $\tau$. L’ensemble $A$, muni de la loi induite par $\tau$, s’appelle un sous-magma de $E$.

Autrement dit, pour que $A$ soit stable pour une loi $\tau$, il faut et il suffit que $A \tau A \subset A$. On identifie souvent une partie stable de $E$ et le sous-magma correspondant.

L’intersection d’une famille de parties stables de $E$ est stable; en particulier il existe une plus petite partie stable $A$ de $E$ contenant une partie $X$ donnée; elle est dite engendrée par $X$ et $X$ est appelé un système générateur de $A$, ou ensemble générateur de $A$. On dit aussi que le sous-magma $A$ est engendré par $X$.

#### Proposition 1 {#alg-i-s1-prop-1 .statement}

Soient $E$ et $F$ deux magmas, et $f$ un homomorphisme de $E$ dans $F$.

(i) L’image par $f$ d’une partie stable de $E$ est une partie stable de $F$.
(ii) L’image réciproque par $f$ d’une partie stable de $F$ est une partie stable de $E$.
(iii) Soit $X$ une partie de $E$. L’image par $f$ de la partie stable de $E$ engendrée par $X$ est la partie stable de $F$ engendrée par $f(X)$.
(iv) Si $g$ est un second homomorphisme de $E$ dans $F$, l’ensemble des éléments $x$ de $E$ tels que $f(x) = g(x)$ est une partie stable de $E$.

Les assertions (i), (ii) et (iv) sont évidentes; démontrons (iii). Soient $\overline{X}$ la partie stable de $E$ engendrée par $X$ et $\overline{f(X)}$ la partie stable de $F$ engendrée par $f(X)$. D’après (i), on a $\overline{f(X)} \subset f(\overline{X})$, et d’après (ii), on a $\overline{X} \subset f^{-1}(\overline{f(X)})$, d’où $f(\overline{X}) \subset \overline{f(X)}$.

#### Proposition 2 {#alg-i-s1-prop-2 .statement}

Soient E un magma associatif et X une partie de E. Soit X' l’ensemble des $x_1 \top x_2 \top \cdots \top x_n$, où $n \geqslant 1$ et où $x_i \in X$ pour $1 \leqslant i \leqslant n$. La partie stable engendrée par X est égale à X'.

Il est immédiat, par récurrence sur n, que le composé d’une séquence de n termes appartenant à X appartient à la partie stable engendrée par X ; il suffit donc de voir que X' est stable. Or, si u et v sont deux éléments de X', ils sont de la forme $u = x_0 \top x_1 \top \cdots \top x_{n-1}$, $v = x_n \top x_{n+1} \top \cdots \top x_{n+p}$ avec $x_i \in X$ pour $0 \leqslant i \leqslant n + p$; donc (I, p. 4, th. 1) $u \top v = x_0 \top x_1 \top \cdots \top x_{n+p}$ appartient à X'.

#### Exemple 1 {#alg-i-s1-n4-exa-1 .statement}

Dans l’ensemble N des entiers naturels, la partie stable pour l’addition engendrée par {1} est l’ensemble des entiers $\geqslant 1$; pour la multiplication, l’ensemble {1} est stable.
2) Etant donnée une loi $\top$ sur un ensemble E, pour qu’une partie $\{h\}$ réduite à un seul élément soit stable pour la loi $\top$, il faut et il suffit que $h \top h = h$; on dit alors que h est idempotent. Par exemple, tout élément d’un ensemble ordonné réticulé est idempotent pour chacune des lois sup et inf.
3) Pour une loi associative $\top$ sur un ensemble E, la partie stable engendrée par un ensemble $\{a\}$ réduit à un seul élément est l’ensemble des éléments $\top^n a$, où n parcourt l’ensemble des entiers $> 0$.

### 5. Eléments permutables. Lois commutatives

#### Définition 7 {#alg-i-s1-def-7 .statement}

Soit E un magma dont la loi est notée $\top$. On dit que deux éléments x et y de E commutent (ou sont permutables) si $y \top x = x \top y$.

#### Définition 8 {#alg-i-s1-def-8 .statement}

Une loi de composition sur un ensemble E est dite commutative si deux éléments quelconques de E commutent pour cette loi. Un magma dont la loi de composition est commutative est appelé magma commutatif.

Une loi commutative est égale à son opposée.

#### Exemple 1 {#alg-i-s1-n5-exa-1 .statement}

L’addition et la multiplication des entiers naturels sont des lois commutatives sur N (E, III, p. 27, corollaire).
2) Dans un ensemble ordonné réticulé, les lois sup et inf sont commutatives; il en est ainsi, en particulier, des lois $\cup$ et $\cap$ entre parties d’un ensemble E.
3) Soit E un ensemble, de cardinal $> 1$. La loi $(f, g) \mapsto f \circ g$ entre applications de E dans E n’est pas commutative, comme on le voit en prenant pour f et g des applications constantes distinctes, mais l’application identique est permutable avec toute application.
4) Soit $(x, y) \mapsto x \top y$ une loi commutative sur E; la loi $(X, Y) \mapsto X \top Y$ entre parties de E est commutative.

#### Définition 9 {#alg-i-s1-def-9 .statement}

Soient E un magma et X une partie de E. On appelle commutant de X dans E l’ensemble des éléments de E qui commutent avec chacun des éléments de X.

Soient X et Y deux parties de E, X' et Y' leurs commutants respectifs. Si $X \subset Y$, on a $Y' \subset X'$.
Soit $(X_i)_{i \in I}$ une famille de parties de E, et pour tout $i \in I$ soit $X'_i$ le commutant de $X_i$. Le commutant de $\bigcup_{i \in I} X_i$ est $\bigcap_{i \in I} X'_i$.

Soient X une partie de E, et X' le commutant de X. Le commutant X'' de X' est appelé le bicommuntant de X. On a X ⊂ X''. Le commutant X'' de X'' est égal à X'. En effet, X' est contenu dans son bicommuntant X'', et la relation X ⊂ X'' entraîne X'' ⊂ X'.

#### Proposition 3 {#alg-i-s1-prop-3 .statement}

*Soit E un magma associatif dont la loi est notée $\top$. Si un élément x de E commute avec chacun des éléments y et z de E, il commute avec y $\top$ z.*

En effet, on a
$$
x \top (y \top z) = (x \top y) \top z = (y \top x) \top z = y \top (x \top z) = y \top (z \top x) = (y \top z) \top x.
$$

#### Corollaire {#alg-i-s1-n5-cor-1 .statement}

*Soit E un magma associatif. Le commutant d’une partie quelconque de E est une partie stable de E.*

#### Définition 10 {#alg-i-s1-def-10 .statement}

*On appelle centre d’un magma E le commutant de E. Un élément du centre de E est appelé élément central de E.*

Si E est un magma associatif, son centre est une partie stable d’après le cor. de la prop. 3, et la loi induite sur ce centre est commutative.

#### Proposition 4 {#alg-i-s1-prop-4 .statement}

*Soient E un magma associatif, X et Y deux parties de E. Si tout élément de X commute avec tout élément de Y, tout élément de la partie stable engendrée par X commute avec tout élément de la partie stable engendrée par Y.*

Soient X' et X'' le commutant et le bicommuntant de X. Ce sont des parties stables de E. On a X ⊂ X'' et Y ⊂ X', donc X'' (resp. X') contient la partie stable de E engendrée par X (resp. Y). Comme tout élément de X'' commute avec tout élément de X', la proposition en résulte.

#### Corollaire 1 {#alg-i-s1-prop-4-cor-1 .statement}

*Si x et y sont permutables pour la loi associative $\top$, il en est de même de $\top^m x$ et $\top^n y$, quels que soient les entiers m > 0 et n > 0; en particulier, $\top^m x$ et $\top^n x$ sont permutables quels que soient x et les entiers m > 0, n > 0.*

#### Corollaire 2 {#alg-i-s1-prop-4-cor-2 .statement}

*Si tous les couples d’éléments d’une partie X sont permutables pour une loi associative $\top$, la loi induite par $\top$ sur la partie stable engendrée par X est associative et commutative.*

**Théorème 2** (théorème de commutativité). — *Soit $\top$ une loi de composition associative sur E; soit $(x_\alpha)_{\alpha \in A}$ une famille finie non vide d’éléments de E, deux à deux permutables; soient B et C deux ensembles totalement ordonnés ayant A pour ensemble sous-jacent. Alors $\prod_{\alpha \in B} x_\alpha = \prod_{\alpha \in C} x_\alpha$*

Le théorème étant vrai si A a un seul élément β, raisonnons par récurrence sur le nombre p d’éléments de A. Soit p un entier > 1, supposons le théorème vrai lorsque Card A < p et démontrons-le pour Card A = p. On peut supposer que A est l’intervalle $\{0, p - 1\}$ de $\mathbf{N}$; le composé de la séquence $(x_\alpha)_{\alpha \in A}$ définie par a relation d’ordre naturelle sur A est $\prod_{i=0}^{p-1} x_i$.

Ordonnons totalement $A$ d’une autre manière, et soient $h$ le plus petit élément de $A$ pour cet ordre, $A'$ l’ensemble des autres éléments de $A$ (totalement ordonné par l’ordre induit). Supposons d’abord $0 < h < p - 1$, et posons $P = \{0, 1, \ldots, h-1\}$, et $Q = \{h+1, \ldots, p-1\}$; le théorème étant supposé vrai pour $A'$, on a, en appliquant de plus le théorème d’associativité (puisque $A' = P \cup Q$)

$$
\prod_{\alpha \in A'} x_\alpha = \left( \prod_{i=0}^{h-1} x_i \right) \top \left( \prod_{i=h+1}^{p-1} x_i \right)
$$

d’où, en composant $x_h$ avec les deux membres, et par application répétée de la commutativité et de l’associativité de $\top$:

$$
\prod_{\alpha \in A} x_\alpha = x_h \top \left( \prod_{\alpha \in A'} x_\alpha \right) = x_h \top \left( \prod_{i=0}^{h-1} x_i \right) \top \left( \prod_{i=h+1}^{p-1} x_i \right)
$$
$$
= \left( \prod_{i=0}^{h-1} x_i \right) \top x_h \top \left( \prod_{i=h+1}^{p-1} x_i \right) = \prod_{i=0}^{p-1} x_i,
$$

ce qui démontre le théorème dans ce cas. Si $h = 0$ ou $h = p - 1$, on trouve le même résultat mais d’une manière plus simple, les termes relatifs à $P$ ou bien les termes relatifs à $Q$ n’apparaissant pas dans les formules.

Pour une loi associative et commutative sur un ensemble $E$, le composé d’une famille finie $(x_\alpha)_{\alpha \in A}$ d’éléments de $E$ est par définition la valeur commune des composés de toutes les séquences obtenues en ordonnant totalement $A$ de toutes les manières possibles. Ce composé se note encore $\prod_{\alpha \in A} x_\alpha$ pour une loi notée $\top$; de même pour les autres notations.

#### Théorème 3 {#alg-i-s1-thm-3 .statement}

*Soient $\top$ une loi associative sur $E$, $(x_\alpha)_{\alpha \in A}$ une famille finie non vide d’éléments de $E$ deux à deux permutables. Si $A$ est réunion d’une famille de parties non vides $(B_i)_{i \in I}$, deux à deux disjointes, on a*

$$(6)$$
$$
\prod_{\alpha \in A} x_\alpha = \prod_{i \in I} \left( \prod_{\alpha \in B_i} x_\alpha \right).
$$

En effet, cela résulte du th. 2 (I, p. 8) en ordonnant totalement $A$ et $I$ de façon que les $B_i$ vérifient les conditions du th. 1 (I, p. 4).

Signalons deux cas particuliers importants de ce théorème:

1) Si $(x_{\alpha \beta})_{(\alpha, \beta) \in A \times B}$ est une famille finie d’éléments permutables d’un magma associatif dont l’ensemble d’indices est le produit de deux ensembles finis non vides $A, B$ (« famille double »), on a

$$(7)$$
$$
\prod_{(\alpha, \beta) \in A \times B} x_{\alpha \beta} = \prod_{\alpha \in A} \left( \prod_{\beta \in B} x_{\alpha \beta} \right) = \prod_{\beta \in B} \left( \prod_{\alpha \in A} x_{\alpha \beta} \right)
$$

comme il résulte du th. 3 en considérant $A \times B$ comme réunion des ensembles $\{\alpha\} \times B$ d’une part, des ensembles $A \times \{\beta\}$ de l’autre.

Par exemple, si B a n éléments, et si, pour chaque $\alpha \in A$, tous les $x_{\alpha \beta}$ ont une même valeur $x_\alpha$, on a

(8)
$$
\prod_{\alpha \in A} (\prod^n x_\alpha) = \prod^n (\prod_{\alpha \in A} x_\alpha).
$$

Si B a deux éléments, on obtient le résultat suivant: soient $(x_\alpha)_{\alpha \in A}$, $(y_\alpha)_{\alpha \in A}$ deux familles non vides d’éléments de E. Si les $x_\alpha$ et les $y_\beta$ sont deux à deux permutables, on a

(9)
$$
\prod_{\alpha \in A} (x_\alpha \prod y_\alpha) = (\prod_{\alpha \in A} x_\alpha) \prod (\prod_{\alpha \in A} y_\alpha).
$$

En raison de la formule (7), le composé d’une suite double $(x_{ij})$, dont l’ensemble d’indices est le produit de deux intervalles $[p, q]$ et $[r, s]$ de $\mathbf{N}$, se note souvent, pour une loi associative et commutative écrite additivement
$$
\sum_{i=p}^q \sum_{j=r}^s x_{ij} \quad \text{ou} \quad \sum_{j=r}^s \sum_{i=p}^q x_{ij}
$$
et de même pour les lois notées par d’autres signes.

#### Exemple 2 {#alg-i-s1-n5-exa-2 .statement}

Soit $n$ un entier $> 0$ et soit A l’ensemble des couples d’entiers $(i, j)$ tels que $0 \leq i \leq n, 0 \leq j \leq n$ et $i < j$; le composé d’une famille $(x_{ij})_{(i, j) \in A}$ (pour une loi associative et commutative), se notera encore $\prod_{0 \leq i < j \leq n} x_{ij}$ (ou simplement $\prod_{i < j} x_{ij}$ si aucune confusion n’en résulte); le th. 3 donne ici les formules

(10)
$$
\prod_{0 \leq i < j \leq n} x_{ij} = \prod_{i=0}^{n-1} (\prod_{j=i+1}^n x_{ij}) = \prod_{j=1}^n (\prod_{i=0}^{j-1} x_{ij}).
$$

On a des formules analogues à (7) pour une famille dont l’ensemble d’indices est le produit de plus de deux ensembles, des formules analogues à (10) pour une famille dont l’ensemble d’indices est l’ensemble $S_p$ des suites strictement croissantes $(i_k)_{1 \leq k \leq p}$ de $p$ entiers tels que $0 \leq i_k \leq n$ ($p \leq n + 1$): dans ce dernier cas, le composé de la famille $(x_{i_1 i_2 \ldots i_p})_{(i_1, \ldots, i_p) \in S_p}$ se note
$$
\prod_{0 \leq i_1 < i_2 < \ldots < i_p \leq n} x_{i_1 i_2 \ldots i_p}, \quad \text{ou simplement} \quad \prod_{i_1 < i_2 < \ldots < i_p} x_{i_1 i_2 \ldots i_p}.
$$

#### Proposition 5 {#alg-i-s1-prop-5 .statement}

*Soient E et F des magmas dont les lois sont notées $\top$, et soient f et g des homomorphismes de E dans F. Soit $f \top g$ l’application $x \mapsto f(x) \top g(x)$ de E dans F. Si F est associatif et commutatif, $f \top g$ est un homomorphisme.*

En effet, quels que soient les éléments $x$ et $y$ de E, on a:
$$
(f \top g)(x \top y) = f(x \top y) \top g(x \top y) = f(x) \top f(y) \top g(x) \top g(y)
= f(x) \top g(x) \top f(y) \top g(y) = ((f \top g)(x)) \top ((f \top g)(y)).
$$

### 6. Lois quotients

#### Définition 11 {#alg-i-s1-def-11 .statement}

*Soit E un ensemble. On dit qu’une loi de composition $\top$ et une relation d’équivalence R dans E sont compatibles si les relations x ≡ x' (mod R) et y ≡ y' (mod R) (pour x, x', y, y' dans E) entraînent x ⊔ y ≡ x' ⊔ y' (mod R); la loi de composition sur l’ensemble quotient E/R qui, aux classes d’équivalence de x et de y, fait correspondre la classe d’équivalence de x ⊔ y, s’appelle la loi quotient de la loi ⊔ par R. L’ensemble E/R, muni de la loi quotient, s’appelle le magma quotient de E par R.

Dire qu’une relation d’équivalence R dans E est compatible avec la loi de composition f : E × E → E, signifie que l’application f est compatible (au sens de E, II, p. 44) avec les relations d’équivalence produit R × R dans E × E (E, II, p. 46) et R dans E. Cela signifie aussi que le graphe de R est un sous-magma de E × E.

Si la loi ⊔ est associative (resp. commutative), il en est de même de la loi quotient (on dit pour abréger que l’associativité, ou la commutativité, se conserve par passage au quotient).

L’application canonique du magma E dans le magma E/R est un homomorphisme.

Pour qu’une application g de E/R dans un magma F soit un homomorphisme, il faut et il suffit que le composé de g et de l’application canonique de E sur E/R soit un homomorphisme.

Les deux propositions suivantes se déduisent immédiatement des définitions:

#### Proposition 6 {#alg-i-s1-prop-6 .statement}

Soient E et F deux magmas et f un homomorphisme de E dans F. Notons R x, y la relation f(x) = f(y) entre éléments x, y de E. Alors R est une relation d’équivalence dans E compatible avec la loi de E et l’application de E/R sur f(E) déduite de f par passage au quotient est un isomorphisme du magma quotient E/R sur le sous-magma f(E) de F.

#### Proposition 7 {#alg-i-s1-prop-7 .statement}

Soient E un magma et R une relation d’équivalence dans E compatible avec la loi de E. Pour qu’une relation d’équivalence S dans E/R soit compatible avec la loi quotient, il faut et il suffit que S soit de la forme T/R, où T est une relation d’équivalence dans E, entraînée par R et compatible avec la loi de E. L’application canonique de E/T sur (E/R)/(T/R) (E, II, p. 46) est alors un isomorphisme de magmas.

#### Proposition 8 {#alg-i-s1-prop-8 .statement}

Soient E un magma, A une partie stable de E et R une relation d’équivalence dans E, compatible avec la loi de E. Le saturé B de A pour R (E, II, p. 44) est une partie stable. Les relations d’équivalence R_A et R_B induites par R dans A et B respectivement sont compatibles avec les lois induites et l’application déduite de l’injection canonique de A dans B par passage aux quotients est un isomorphisme de magmas de A/R_A sur B/R_B.

Notons ⊔ la loi de E. Si x et y sont deux éléments de B, il existe deux éléments x' et y' de A tels que x ≡ x' (mod R) et y ≡ y' (mod R); on a alors x ⊔ y ≡ x' ⊔ y' (mod R) et x' ⊔ y' ∈ A, d’où x ⊔ y ∈ B. Ainsi B est une partie stable de E, et les autres assertions sont évidentes.

Soient $M$ un magma, et $((u_\alpha, v_\alpha))_{\alpha \in I}$ une famille d’éléments de $M \times M$. Considérons toutes les relations d’équivalence $S$ dans $M$ qui sont compatibles avec la loi de $M$, et telles que $u_\alpha \equiv v_\alpha$ (mod. $S$) pour tout $\alpha \in I$. L’intersection des graphes de ces relations est le graphe d’une relation d’équivalence $R$, qui est compatible avec la loi de $M$, et telle que $u_\alpha \equiv v_\alpha$ (mod $R$). Donc $R$ est *la plus fine* (E, III, p. 4 et p. 8) des relations d’équivalence possédant ces deux propriétés. On l’appelle la relation d’équivalence compatible avec la loi de $M$ *engendrée* par les $(u_\alpha, v_\alpha)$.

#### Proposition 9 {#alg-i-s1-prop-9 .statement}

*On conserve les notations précédentes. Soit $f$ un homomorphisme de $M$ dans un magma tel que $f(u_\alpha) = f(v_\alpha)$ pour tout $\alpha \in I$. Alors $f$ est compatible avec $R$.*

Soit $T$ la relation d’équivalence associée à $f$. On a $u_\alpha \equiv v_\alpha$ (mod $T$) pour tout $\alpha \in I$, et $T$ est compatible avec la loi de $M$, donc $T$ est moins fine que $R$; cela prouve la proposition.

## EXERCICES {#alg-i-s1-exercises}

See the [exercises for § 1](exercises/s1/).
