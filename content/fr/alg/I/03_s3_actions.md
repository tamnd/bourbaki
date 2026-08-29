---
book: alg
book_title: Algebra
chapter: I
chapter_title: STRUCTURES ALGÉBRIQUES
section: 3
section_title: Actions
lang: fr
source: alg-i-iii-fr
book_pages: A I.23-A I.28, A I.122-A I.123
pdf_pages: 0033-0038, 0132-0133
extraction: ocr
subsections:
    - "no": 1
      title: Actions
      page: 23
      pdf_page: 33
    - "no": 2
      title: Parties stables pour une action. Action induite
      page: 25
      pdf_page: 35
    - "no": 3
      title: Action quotient
      page: 25
      pdf_page: 35
    - "no": 4
      title: Distributivité
      page: 26
      pdf_page: 36
    - "no": 5
      title: Distributivité d’une loi interne par rapport à une autre
      page: 28
      pdf_page: 38
statements: 23
exercises: 10
content_sha256: ee4b2e3ff8b24219c1460bf40c37c82b11b0657ccfb5d0937024d65174be79fe
---

## § 3. ACTIONS

### 1. Actions

#### Définition 1 {#alg-i-s3-def-1 .statement}

Soient $\Omega$ et $E$ deux ensembles. On appelle action de $\Omega$ sur $E$ une application de $\Omega$ dans l’ensemble $E^E$ des applications de $E$ dans lui-même.

Soit $\alpha \mapsto f_\alpha$ une action de $\Omega$ sur E. On dit que l’application $(\alpha, x) \mapsto f_\alpha(x)$ (resp. $(x, \alpha) \mapsto f_\alpha(x)$) est la loi d’action à gauche (resp. à droite) de $\Omega$ sur E associée à l’action donnée$^1$ de $\Omega$ sur E. Etant donnée une application g de $\Omega \times E$ (resp. $E \times \Omega$) dans E, il existe une action $\alpha \mapsto f_\alpha$ de $\Omega$ dans E et une seule telle que la loi d’action à gauche (resp. à droite) associée soit g (E, II, p. 31, prop. 3).

Dans ce chapitre, nous dirons pour abréger « loi d’action » au lieu de « loi d’action à gauche ». L’élément $f_\alpha(x)$ de E (pour $\alpha \in \Omega$ et $x \in E$), est parfois appelé le transformé de x par $\alpha$ ou le composé de $\alpha$ et de x. Pour le désigner, on emploie souvent la notation multiplicative à gauche $\alpha.x$ (resp. à droite $x.\alpha$), le point pouvant être omis; le composé de $\alpha$ et de $x$ s’appelle alors le produit de $\alpha$ et de $x$ (resp. de $x$ et de $\alpha$). On emploie aussi la notation exponentielle $x^\alpha$. Dans les raisonnements des paragraphes suivants, nous utiliserons ordinairement la notation $\alpha \perp x$. Les éléments de $\Omega$ sont souvent appelés opérateurs.

#### Exemple 1 {#alg-i-s3-n1-exa-1 .statement}

Soit E un magma associatif, noté multiplicativement. L’application qui, à un entier n strictement positif, fait correspondre l’application $x \mapsto x^n$ de E dans lui-même, est une action de $\mathbf{N}^*$ sur E. Si E est un groupe, l’application qui, à un entier rationnel a, fait correspondre l’application $x \mapsto x^a$ de E dans E, est une action de $\mathbf{Z}$ sur E.

#### Exemple 2 {#alg-i-s3-n1-exa-2 .statement}

Soit E un magma, de loi notée $\top$. L’application qui, à un élément $x \in E$, fait correspondre l’application $A \mapsto x \top A$ de l’ensemble des parties de E dans lui-même, est une action de E sur $\mathcal{P}(E)$.

#### Exemple 3 {#alg-i-s3-n1-exa-3 .statement}

Soit E un ensemble. L’application identique de $E^E$ est une action de $E^E$ sur E, dite action canonique. La loi d’action correspondante est l’application $(f, x) \mapsto f(x)$ de $E^E \times E$ dans E.

#### Exemple 4 {#alg-i-s3-n1-exa-4 .statement}

Soit $(\Omega_i)_{i \in I}$ une famille d’ensembles. Pour tout $i \in I$, soit $f_i : \Omega_i \to E^E$ une action de $\Omega_i$ sur E. Soit $\Omega$ la somme des $\Omega_i$ (E, II, p. 30). L’application f de $\Omega$ dans $E^E$ prolongeant les $f_i$ est une action de $\Omega$ sur E. Ceci permet de ramener la considération de familles d’actions à celle d’une seule action.

#### Exemple 5 {#alg-i-s3-n1-exa-5 .statement}

Etant données une action de $\Omega$ sur E de loi notée $\perp$, une partie $\Xi$ de $\Omega$ et une partie X de E, on désigne par $\Xi \perp X$ l’ensemble des $\alpha \perp x$ pour $\alpha \in \Xi$ et $x \in X$; lorsque $\Xi$ est réduite à un élément $\alpha$, on écrit généralement $\alpha \perp X$ au lieu de $\{\alpha\} \perp X$. L’application qui, à $\alpha \in \Omega$, fait correspondre l’application $X \mapsto \alpha \perp X$ est une action de $\Omega$ sur $\mathcal{P}(E)$, dite déduite de l’action donnée par extension à l’ensemble des parties.

#### Exemple 6 {#alg-i-s3-n1-exa-6 .statement}

Soit $\alpha \mapsto f_\alpha$ une action de $\Omega$ sur E. Soit g une application de $\Omega'$ dans $\Omega$. Alors l’application $\beta \mapsto f_{g(\beta)}$ est une action de $\Omega'$ sur E.

#### Exemple 7 {#alg-i-s3-n1-exa-7 .statement}

Soit $f : E \times E \to E$ une loi de composition sur un ensemble E. L’application $\gamma : x \mapsto \gamma_x$ (resp. $\delta : x \mapsto \delta_x$) (I, p. 14) qui, à un élément $x \in E$ fait correspondre la translation à gauche (resp. à droite) par $x$, est une action de E sur lui-même; on l’appelle l’action à gauche (resp. à droite) de E sur lui-même déduite de la loi donnée. Lorsque $f$ est commutative, ces deux actions coïncident.

La loi d’action à gauche (resp. à droite) associée à $\gamma$ est $f$ (resp. la loi opposée à $f$). La loi d’action à droite (resp. à gauche) associée à $\delta$ est $f$ (resp. la loi opposée à $f$).

Soient $\Omega, E, F$ des ensembles, $\alpha \mapsto f_\alpha$ une action de $\Omega$ sur E, $\alpha \mapsto g_\alpha$ une action de $\Omega$ sur F. On appelle $\Omega$-morphismisme de E dans F, ou application de E dans F compatible avec les actions de $\Omega$, une application h de E dans F telle que
$$
g_\alpha(h(x)) = h(f_\alpha(x))
$$

1 Ou parfois la loi de composition externe sur E ayant $\Omega$ comme ensemble d’opérateurs.

quels que soient $\alpha \in \Omega$ et $x \in E$. Le composé de deux $\Omega$-morphismes est un $\Omega$-morphisme.

Soient $\Omega, \Xi, E, F$ des ensembles, $\alpha \mapsto f_\alpha$ une action de $\Omega$ dans $E$, $\beta \mapsto g_\beta$ une action de $\Xi$ dans $F$, $\varphi$ une application de $\Omega$ dans $\Omega'$. On appelle $\varphi$-morphism de $E$ dans $F$ une application $h$ de $E$ dans $F$ telle que

$$
g_{\varphi(\alpha)}(h(x)) = h(f_\alpha(x))
$$

quels que soient $\alpha \in \Omega$ et $x \in E$.

### 2. Parties stables pour une action. Action induite

#### Définition 2 {#alg-i-s3-def-2 .statement}

*Une partie A d’un ensemble E est dite stable pour une action $\alpha \mapsto f_\alpha$ de $\Omega$ sur E si l’on a $f_\alpha(A) \subset A$ pour tout $\alpha \in \Omega$. Un élément x de E est dit invariant par un élément $\alpha$ de $\Omega$ si $f_\alpha(x) = x$.*

L’intersection d’une famille de parties stables de E pour une action donnée est stable. Il existe donc une plus petite partie stable de E contenant une partie X donnée; elle est dite *engendrée* par X; elle se compose des éléments $(f_{\alpha_1} \circ f_{\alpha_2} \circ \cdots \circ f_{\alpha_n})(x)$, où $x \in X, n \geqslant 0, \alpha_i \in \Omega$ pour tout i.

#### Remarque {#alg-i-s3-n2-rem-1 .statement}

Soit E un magma, de loi notée $\tau$. On prendra garde qu’une partie A de E stable pour l’action à gauche de E sur lui-même n’est pas nécessairement stable pour l’action à droite de E sur lui-même; une partie A de E stable pour l’action à gauche (resp. à droite) de E sur lui-même, est stable pour la loi de E, mais la réciproque est en général inexacte. Plus précisément, A est stable pour la loi de E si et seulement si l’on a $A \tau A \subset A$, alors que A est stable pour l’action à gauche (resp. à droite) de E sur lui-même si et seulement si l’on a $E \tau A \subset A$ (resp. $A \tau E \subset A$).

#### Exemple {#alg-i-s3-n2-exa-1 .statement}

Prenons pour magma E l’ensemble $\mathbf{N}$ muni de la multiplication. L’ensemble $\{1\}$ est stable pour la loi interne de $\mathbf{N}$, mais la partie stable pour l’action de $\mathbf{N}$ sur lui-même engendrée par $\{1\}$ est $\mathbf{N}$ tout entier.

#### Définition 3 {#alg-i-s3-def-3 .statement}

*Soient $\alpha \mapsto f_\alpha$ une action de $\Omega$ sur E, A une partie stable de E. L’application qui, à un élément $\alpha \in \Omega$, fait correspondre la restriction de $f_\alpha$ à A (considérée comme application de A dans lui-même), est une action de $\Omega$ sur A dite induite par l’action donnée.*

### 3. Action quotient

#### Définition 4 {#alg-i-s3-def-4 .statement}

*Soit $\alpha \mapsto f_\alpha$ une action d’un ensemble $\Omega$ sur un ensemble E. On dit qu’une relation d’équivalence R dans E est compatible avec l’action donnée si, quels que soient les éléments x et y de E tels que $x \equiv y \pmod{R}$ et quel que soit $\alpha \in \Omega$, on a $f_\alpha(x) \equiv f_\alpha(y) \pmod{R}$. L’application qui, à un élément $\alpha \in \Omega$, associe l’application de $E/R$ dans lui-même déduite de $f_\alpha$ par passage aux quotients, est une action de $\Omega$ sur $E/R$, appelée quotient de l’action de $\Omega$ sur E.*

Soit E un magma et soit R une relation d’équivalence sur E. On dit que R est compatible à gauche (resp. à droite) avec la loi de E si elle est compatible avec l’action à gauche (resp. à droite) de E sur lui-même déduite de la loi de E. Pour que R soit compatible avec la loi de E, il faut et il suffit qu’elle soit compatible à gauche et à droite avec la loi de E.

Nous laissons au lecteur le soin d’énoncer et de démontrer les analogues des prop. 6, 7 et 8 de I, p. 11.

### 4. Distributivité

#### Définition 5 {#alg-i-s3-def-5 .statement}

Soient $E_1, \ldots, E_n$ et F des ensembles et u une application de $E_1 \times \ldots \times E_n$ dans F. Soit $i \in \{1, n\}$. Supposons $E_i$ et F munis de structures de magmas. On dit que u est distributive relativement à la variable d’indice i si l’application partielle

$$
x_i \mapsto u(a_1, \ldots, a_{i-1}, x_i, a_{i+1}, \ldots, a_n)
$$

est un homomorphisme de $E_i$ dans F quels que soient les $a_j$ fixés dans $E_j$ pour $j \neq i$.

Si l’on note $\top$ les lois internes dans $E_i$ et F, la distributivité de u se traduit par les formules

(1)
$$
u(a_1, \ldots, a_{i-1}, x_i \top x'_i, a_{i+1}, \ldots, a_n)
= u(a_1, \ldots, a_{i-1}, x_i, a_{i+1}, \ldots, a_n) \top u(a_1, \ldots, a_{i-1}, x'_i, a_{i+1}, \ldots, a_n)
$$
pour $a_1 \in E_1, \ldots, a_{i-1} \in E_{i-1}, x_i \in E_i, x'_i \in E_i, a_{i+1} \in E_{i+1}, \ldots, a_n \in E_n$.

#### Exemple {#alg-i-s3-n4-exa-1 .statement}

Soient E un monoïde (resp. un groupe), noté multiplicativement. L’application $(n, x) \mapsto x^n$ de $\mathbf{N} \times E$ (resp. $\mathbf{Z} \times E$) dans E est distributive par rapport à la première variable d’après la formule $x^{m+n} = x^m x^n$ (on munit $\mathbf{N}$ de l’addition). Si E est commutatif, cette application est distributive par rapport à la deuxième variable d’après la formule $(xy)^n = x^n y^n$.

#### Proposition 1 {#alg-i-s3-prop-1 .statement}

Soient $E_1, E_2, \ldots, E_n$ et F des monoïdes commutatifs notés additivement et soit u une application de $E_1 \times \ldots \times E_n$ dans F, distributive par rapport à toutes les variables. Pour chaque $i \in \{1, n\}$, soient $L_i$ un ensemble fini non vide et $(x_{i,\lambda})_{\lambda \in L_i}$ une famille d’éléments de $E_i$. On pose $y_i = \sum_{\lambda \in L_i} x_{i,\lambda}$ pour $i \in \{1, n\}$. On a

(2)
$$
u(y_1, \ldots, y_n) = \sum_{\alpha} u(x_{1,\alpha_1}, \ldots, x_{n,\alpha_n})
$$
la somme étant étendue aux suites $\alpha = (\alpha_1, \ldots, \alpha_n)$ appartenant à $L_1 \times \cdots \times L_n$.

On raisonne par récurrence sur n, le cas $n = 1$ résultant de la formule (2) de I, p. 4. D’après la même référence, on a

(3)
$$
u(y_1, \ldots, y_{n-1}, y_n) = \sum_{\alpha_n \in L_n} u(y_1, \ldots, y_{n-1}, x_{n,\alpha_n})
$$
car $y_n = \sum_{\alpha_n \in L_n} x_{n,\alpha_n}$ et l’application $z \mapsto u(y_1, \ldots, y_{n-1}, z)$ de $E_n$ dans F est un homomorphisme de magmas. Par l’hypothèse de récurrence utilisée pour les applications distributives $(z_1, \ldots, z_{n-1}) \mapsto u(z_1, \ldots, z_{n-1}, x_n, \alpha_n)$ de $E_1 \times \cdots \times E_{n-1}$ dans $F$, on a

(4)
$$
u(y_1, \ldots, y_{n-1}, x_n, \alpha_n) = \sum_{\alpha_1, \ldots, \alpha_{n-1}} u(x_1, \alpha_1, \ldots, x_{n-1}, \alpha_{n-1}, x_n, \alpha_n),
$$
la somme étant étendue aux suites $(\alpha_1, \ldots, \alpha_{n-1})$ appartenant à $M = L_1 \times \cdots \times L_{n-1}$. Or on a $L_1 \times \cdots \times L_n = M \times L_n$; posant $t_{\alpha_1, \ldots, \alpha_n} = u(x_1, \alpha_1, \ldots, x_n, \alpha_n)$, on a

(5)
$$
\sum_{\alpha_1, \ldots, \alpha_n} t_{\alpha_1, \ldots, \alpha_n} = \sum_{\alpha_n} \left( \sum_{\alpha_1, \ldots, \alpha_{n-1}} t_{\alpha_1, \ldots, \alpha_{n-1}, \alpha_n} \right)
$$
d’après la formule (7) de I, p. 9. On déduit immédiatement (2) de (3), (4) et (5).

#### Remarque {#alg-i-s3-n4-rem-1 .statement}

Si l’on a $u(a_1, \ldots, a_{i-1}, 0, a_{i+1}, \ldots, a_n) = 0$ pour $i \in \{1, n\}$ et $a_j \in E_j$ ($j \neq i$), alors la formule (2) reste valable pour des familles $(x_i, \lambda)_{\lambda \in L_i}$ à support fini.

Un cas particulier de la déf. 5 est celui où $u$ est la loi d’action associée à une action d’un ensemble $\Omega$ sur un magma $E$. Si $u$ est distributive par rapport à la seconde variable, on dit encore que l’action de $\Omega$ sur le magma $E$ est distributive. En d’autres termes:

#### Définition 6 {#alg-i-s3-def-6 .statement}

*On dit qu’une action* $\alpha \mapsto f_\alpha$ *d’un ensemble* $\Omega$ *sur un magma* $E$ *est distributive si, pour tout* $\alpha \in \Omega$, *l’application* $f_\alpha$ *est un endomorphisme du magma* $E$.

Si l’on note $\top$ la loi du magma $E$ et $\perp$ la loi d’action associée à l’action de $\Omega$ sur $E$, la distributivité de celle-ci se traduit donc par la formule

(6)
$$
\alpha \perp (x \top y) = (\alpha \perp x) \top (\alpha \perp y) \quad \text{(pour } \alpha \in \Omega \text{ et } x, y \text{ dans } E\text{)}.
$$

Par abus de langage, on dit encore que loi $\perp$ est distributive (ou distributive à droite) par rapport à la loi $\top$.

La formule (2) de I, p. 4 montre que l’on a alors, pour toute séquence $(x_\lambda)_{\lambda \in L}$ d’éléments de $E$ et tout $\alpha \in \Omega$

(7)
$$
\alpha \perp \left( \bigwedge_{\lambda \in L} x_\lambda \right) = \bigwedge_{\lambda \in L} (\alpha \perp x_\lambda).
$$

Si une action $\alpha \mapsto f_\alpha$ est distributive et si une relation d’équivalence $R$ dans $E$ est compatible avec la loi de composition de $E$ et l’action $\alpha \mapsto f_\alpha$, l’action quotient sur $E/R$ est distributive.

Lorsque la loi de $E$ est écrite multiplicativement, on emploie fréquemment la notation exponentielle $x^\alpha$ pour une loi d’action distributive par rapport à cette multiplication, de sorte que la distributivité s’exprime par l’identité $(xy)^\alpha = x^\alpha y^\alpha$. Si la loi de $E$ est notée additivement, on emploie fréquemment la notation multiplicative à gauche $\alpha . x$ (resp. à droite $x . \alpha$) pour une loi d’action distributive par rapport à cette addition, la distributivité s’exprimant par l’identité
$$
\alpha(x + y) = \alpha x + \alpha y \quad \text{(resp. } (x + y)\alpha = x\alpha + y\alpha\text{)}.
$$

On peut aussi considérer le cas où $\Omega$ est muni d’une loi interne, notée $\top$, et où la loi d’action est distributive par rapport à la première variable, ce qui signifie que

$$(8)$$
$$(\alpha \top \beta) \perp x = (\alpha \perp x) \top (\beta \perp x)$$

quels que soient $\alpha, \beta$ dans $\Omega$ et $x \in E$. On a alors, d’après la formule (2) de I, p. 4

$$(9)$$
$$\left( \prod_{\lambda \in L} \alpha_\lambda \right) \perp x = \prod_{\lambda \in L} (\alpha_\lambda \perp x)$$

pour toute séquence $(\alpha_\lambda)_{\lambda \in L}$ d’éléments de $\Omega$ et tout $x \in E$.

### 5. Distributivité d’une loi interne par rapport à une autre

#### Définition 7 {#alg-i-s3-def-7 .statement}

Soient $\top$ et $\perp$ deux lois internes sur un ensemble $E$. On dit que la loi $\perp$ est distributive par rapport à la loi $\top$ si l’on a

$$(10)$$
$$x \perp (y \top z) = (x \perp y) \top (x \perp z)$$

$$(11)$$
$$(x \top y) \perp z = (x \perp z) \top (y \perp z)$$

pour $x, y, z$ dans $E$.

On remarquera que (10) et (11) sont équivalentes si la loi $\perp$ est commutative. En général, on notera l’une des lois additivement et l’autre multiplicativement; lorsque la multiplication est distributive par rapport à l’addition, on a:

$$(12)$$
$$x . (y + z) = x . y + x . z$$

$$(13)$$
$$(x + y) . z = x . z + y . z$$

#### Exemple 1 {#alg-i-s3-n5-exa-1 .statement}

Dans l’ensemble $\mathcal{P}(E)$ des parties d’un ensemble $E$, chacune des lois internes $\cap$ et $\cup$ est distributive par rapport à elle-même et à l’autre. Cela résulte des formules du type
$$
\begin{align*}
A \cap (B \cup C) &= (A \cap B) \cup (A \cap C) \\
A \cup (B \cap C) &= (A \cup B) \cap (A \cup C).
\end{align*}
$$

#### Exemple 2 {#alg-i-s3-n5-exa-2 .statement}

Dans $\mathbf{Z}$ (et plus généralement, dans tout ensemble totalement ordonné) chacune des lois sup et inf est distributive par rapport à l’autre et par rapport à elle-même.

#### Exemple 3 {#alg-i-s3-n5-exa-3 .statement}

Dans $\mathbf{Z}$ (* et plus généralement dans tout anneau *) la multiplication est distributive par rapport à l’addition.

#### Exemple 4 {#alg-i-s3-n5-exa-4 .statement}

Dans $\mathbf{N}$, l’addition et la multiplication sont distributives par rapport aux lois sup et inf.

## EXERCICES {#alg-i-s3-exercises}

See the [exercises for § 3](exercises/s3/).
