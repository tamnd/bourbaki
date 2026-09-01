---
book: int
book_title: Integration
chapter: VII
chapter_title: Mesure de Haar
section: 3
section_title: Applications et exemples
lang: fr
source: int-vii-viii-fr
pdf_pages: 0069-0094, 0114-0118
extraction: ocr
subsections:
    - "no": 1
      title: Groupes compacts d’applications linéaires.
      page: 0
      pdf_page: 69
    - "no": 2
      title: Trivialité d’espaces fibrés et d’extensions de groupes.
      page: 0
      pdf_page: 71
    - "no": 3
      title: Exemples.
      page: 0
      pdf_page: 78
statements: 26
exercises: 6
content_sha256: 8e5a9d75c0385e0263d9a5248ee1146c952d531befa9e00f05d2bc085ff82735
---

## § 3. Applications et exemples.

### 1. Groupes compacts d’applications linéaires.

Soit $E$ un espace vectoriel de dimension finie sur $\mathbf{R}, \mathbf{C}$ ou $\mathbf{H}$. Alors $\mathrm{End}(E)$ est une algèbre de dimension finie sur $\mathbf{R}$, et la topologie canonique sur $\mathrm{End}(E)$ (§ 1, no 10) est la topologie de la convergence compacte. Le groupe $\mathrm{Aut}(E) = \mathbf{GL}(E)$ est une partie ouverte de $\mathrm{End}(E)$, donc est un groupe localement compact. Soit $(e_1, e_2, \ldots, e_n)$ une base de $E$, et pour tout endomorphisme $u$ de $E$, soit $M(u) = (\alpha_{ij}(u))$ la matrice de $u$ par rapport à cette base ; dire qu’une partie $S$ de $\mathrm{End}(E)$ est relativement compacte dans $\mathrm{End}(E)$ équivaut à dire que les fonctions $\alpha_{ij}(u)$ sont bornées dans $S$.

#### Proposition 1 {#int-vii-s3-prop-1 .statement}

Soit $G$ un sous-groupe de $\mathrm{Aut}(E)$. Les trois propriétés suivantes sont équivalentes :
(i) $G$ est relativement compact dans $\mathrm{End}(E)$ ;
(ii) $G$ est relativement compact dans $\mathrm{Aut}(E)$ ;

(iii) G laisse invariante une forme hermitienne positive non dégénérée sur E.

(iii) ⇒ (i) : supposons que G laisse invariante une forme hermitienne positive non dégénérée Ψ. Soit (e₁, ..., eₙ) une base orthonormale pour Ψ (Alg., chap. IX, § 6, no 1, cor. 1 du th. 1). Pour tout u ∈ G, soit (uᵢⱼ) sa matrice par rapport à (eᵢ). Quel que soit j, on a $\sum_{i=1}^{n} |u_{ij}|^2 = 1$, donc $|u_{ij}| \leq 1$ quels que soient i et j, ce qui prouve (i).

(i) ⇒ (ii) : ceci résulte de Top. Gén., chap. X, 2ᵉ éd., § 4, cor. du th. 4, compte tenu du fait que la topologie de End(E) est celle de la convergence compacte.

(ii) ⇒ (iii) : supposons que l’adhérence $\overline{G}$ de G dans Aut(E) soit compacte. Soit Φ une forme hermitienne positive non dégénérée sur E. Si le corps des scalaires est $\mathbf{R}$ ou $\mathbf{C}$, la donnée de Φ fait de E un espace hilbertien de dimension finie, et la condition (iii) résultera du lemme suivant :

#### Lemme 1 {#int-vii-s3-lem-1 .statement}

Soient F un espace hilbertien, K un groupe compact, et s → U(s) une représentation de K dans le groupe des éléments inversibles de $\mathcal{L}(F ; F)$, continue pour la topologie de la convergence simple. Il existe une forme hermitienne positive non dégénérée φ sur F telle que $\varphi(U(s)x, U(s)y) = \varphi(x, y)$ quels que soient s ∈ K, x ∈ F, y ∈ F, et telle que la structure d’espace vectoriel topologique de F définie par φ (Esp. vect. top., chap. V, § 1, no 3) soit identique à la structure initiale de F.

Soit α une mesure de Haar sur K. Quels que soient x, y dans F, l’application s → (U(s)x|U(s)y) est continue. Posons

$$
\varphi(x, y) = \int (U(s)x|U(s)y)d\alpha(s).
$$

Il est immédiat que $\varphi(x, y)$ est une forme sesquilinéaire sur F. Comme l’ensemble des endomorphismes U(s) est compact dans $\mathcal{L}_s(F ; F)$, il existe une constante M telle que $\|U(s)\| \leq M$ pour tout s ∈ K. Pour tout x ∈ F, on a donc

$$
M^{-1}\|x\| \leq \|U(s)x\| \leq M\|x\|,
$$

d'où les inégalités

$$
M^{-2\alpha}(K)\|x\|^2 \leq \varphi(x, x) \leq M^{2\alpha}(K)\|x\|^2,
$$

ce qui montre que $\varphi$ est positive non dégénérée et que la norme $\varphi(x, x)^{1/2}$ est équivalente à la norme $\|x\|$. Enfin, pour tout $t \in K$, on a

$$
\varphi(U(t)x, U(t)y) = \int (U(st)x | U(st)y)d\alpha(s)
$$
$$
= \int (U(s)x | U(s)y)d\alpha(s) = \varphi(x, y)
$$

Lorsque le corps des scalaires est $\mathbf{H}$, on raisonne exactement de même, en remplaçant partout la fonction $s \to (U(s)x | U(s)y)$ par la fonction $s \to \Phi(sx, y)$ définie dans $G$, à valeurs dans $\mathbf{H}$. Ce qui achève la démonstration du lemme.

#### Remarque {#int-vii-s3-n1-rem-1 .statement}

Soit $\Phi$ une forme hermitienne positive non dégénérée sur $E$. Le groupe unitaire $\mathbf{U}(\Phi)$ est fermé dans $\mathrm{Aut}(E)$, donc compact (prop. 1). La prop. 1 montre aussi que tout sous-groupe compact de $\mathrm{Aut}(E)$ est contenu dans un sous-groupe de la forme $\mathbf{U}(\Phi)$. Si maintenant $\mathbf{U}(\Phi)$ est contenu dans un sous-groupe compact $K$ de $\mathrm{Aut}(E)$, on voit qu’il existe une forme hermitienne positive non dégénérée $\Phi'$ sur $E$ telle que $\mathbf{U}(\Phi) \subset K \subset \mathbf{U}(\Phi')$ et il en résulte facilement (exerc. 1) que $\Phi$ et $\Phi'$ sont proportionnelles, d’où $\mathbf{U}(\Phi) = K$. Ainsi les sous-groupes compacts maximaux de $\mathrm{Aut}(E)$ sont les sous-groupes de la forme $\mathbf{U}(\Phi)$.

### 2. Trivialité d’espaces fibrés et d’extensions de groupes.

#### Proposition 2 {#int-vii-s3-prop-2 .statement}

Soit $X$ un espace localement compact dans lequel un groupe localement compact $H$ opère à droite, continûment et proprement, par $(x, \xi) \to x\xi$. Supposons $X/H$ paracompact. Soit $g$ une représentation continue de $H$ dans $\mathbf{R}^n$. Il existe alors une application continue $f$ de $X$ dans $\mathbf{R}^n$ telle que $f(x\xi) = f(x) + g(\xi)$ quels que soient $x \in X$ et $\xi \in H$.

On se ramène aussitôt au cas où $n = 1$. Comme le groupe additif $\mathbf{R}$ est isomorphe au groupe multiplicatif $\mathbf{R}_+^*$, la proposition est alors conséquence immédiate de la prop. 7 du § 2, no 4.

#### Corollaire {#int-vii-s3-n2-cor-1 .statement}

*Soit X un espace localement compact dans lequel un espace vectoriel réel V de dimension finie opère à droite, continûment et proprement, par $(x, v) \to xv$. Soit $\pi$ l’application canonique de X sur $B = X/V$. Supposons B paracompact.*

a) *Il existe une application continue $f$ de X dans V telle que $f(xv) = f(x) + v$ quels que soient $x \in X$ et $v \in V$.

b) *Si $f$ est une application vérifiant les conditions de a), l’application $x \to (\pi(x), f(x))$ est un homéomorphisme de X sur $B \times V$.

L’assertion a) résulte de la prop. 2 dans laquelle on prend pour $g$ l’application identique de V. Soit $f$ une application vérifiant les conditions de a). L’application $x \to x.(-f(x))$ de X dans X est continue et constante sur chaque orbite, donc de la forme $\varphi \circ \pi$, où $\varphi$ est une application continue de B dans X ; pour tout $b \in B$, on a $\pi(\varphi(b)) = b$. Les applications $x \to (\pi(x), f(x))$ de X dans $B \times V$ et $(b, v) \to \varphi(b).v$ de $B \times V$ dans X sont réciproques l’une de l’autre, car $\varphi(\pi(x)).f(x) = x.(-f(x)).(f(x)) = x,\ \pi(\varphi(b).v) = \pi(\varphi(b)) = b$, et, si $b = \pi(y), f(\varphi(\pi(y)).v) = f(y.(-f(y)).v) = f(y) - f(y) + v = v$. Comme ces applications sont continues, ce sont des homéomorphismes.

#### Remarque {#int-vii-s3-n2-rem-1 .statement}

Soient E un espace affine réel de dimension finie, T un espace compact, $\mu$ une mesure *de masse totale* 1 sur T, $f$ une application continue de T dans E. Si on choisit une origine $a$ dans E, E se trouve muni d’une structure d’espace vectoriel, et l’intégrale $\int_T f(t)d\mu(t)$ a donc un sens ; elle représente le point $x$ de E tel que

$$
x - a = \int_T (f(t) - a)d\mu(t).
$$

Ce point est indépendant du choix de $a$. En effet, soient $a' \in \mathbf{E}$ et $x' \in \mathbf{E}$ tel que $x' - a' = \int_{\mathbf{T}} (f(t) - a') d\mu(t)$. On a

$$
x' - a = (x' - a') + (a' - a) = \int_{\mathbf{T}} (f(t) - a') d\mu(t)
$$
$$
+ \int_{\mathbf{T}} (a' - a) d\mu(t) = \int_{\mathbf{T}} (f(t) - a) d\mu(t) = x - a
$$

d'où $x' = x$. On pourra donc utiliser le symbole $\int_{\mathbf{T}} f(t) d\mu(t)$ sans préciser le choix de l'origine dans $\mathbf{E}$. Si $u$ est une application affine de $\mathbf{E}$ dans un autre espace affine $\mathbf{E}'$ de dimension finie, on a

$$
u \left( \int_{\mathbf{T}} f(t) d\mu(t) \right) = \int_{\mathbf{T}} u(f(t)) d\mu(t)
$$

En effet, on peut identifier $\mathbf{E}$ et $\mathbf{E}'$ à des espaces vectoriels de telle sorte que $u$ devienne une application linéaire, et la formule est alors connue (chap. III, § 4, no 2, prop. 4).

#### Lemme 2 {#int-vii-s3-lem-2 .statement}

Soient $G$ un groupe compact, $\mu$ la mesure de Haar normalisée de $G$, $\mathbf{E}$ un espace affine de dimension finie, $A$ le groupe affine de $\mathbf{E}$, $\varrho$ un homomorphisme de $G$ dans $A$. On suppose que, pour tout $x \in \mathbf{E}$, l'application $s \to \varrho(s)x$ de $G$ dans $\mathbf{E}$ est continue. Alors, pour tout $x \in \mathbf{E}$, le point

$$
x_0 = \int_G \varrho(s)x d\mu(s) \in \mathbf{E}
$$

est invariant par $G$.

En effet, pour tout $t \in G$, on a

$$
\varrho(t)x_0 = \int_G \varrho(t)\varrho(s)x d\mu(s) = \int_G \varrho(ts)x d\mu(s) = \int_G \varrho(s)x d\mu(s) = x_0.
$$

#### Proposition 3 {#int-vii-s3-prop-3 .statement}

Soit $G$ un groupe localement compact. Soit $H$ un sous-groupe distingué fermé de $G$, isomorphe à $\mathbf{R}^n$ et tel que $G/H$ soit compact.

a) Il existe un sous-groupe fermé L de G tel que G soit produit semi-direct topologique de L et de H.

b) Si M est un sous-groupe compact de G, il existe un élément $x \in H$ tel que $x^{-1}Mx \subset L$.

c) Tout sous-groupe compact de G est contenu dans un sous-groupe compact maximal.

d) Les sous-groupes compacts maximaux de G sont les sous-groupes transformés de L par les automorphismes intérieurs de G.

Soit $\pi$ l’homomorphisme canonique de G sur $K = G/H$. Par passage au quotient, l’application $(s, h) \to shs^{-1}$ de $G \times H$ dans H définit une application continue $(\sigma, h) \to \sigma.h$ de $K \times H$ dans H telle que $shs^{-1} = \pi(s).h$. Nous identifierons H à $\mathbf{R}^n$ (et emploierons donc, suivant le cas, la notation multiplicative ou additive pour la loi de groupe dans H). D’après le cor. de la prop. 2, il existe une application continue $f$ de G dans H telle que $f(xh) = f(x) + h$ pour $x \in G,\ h \in H$. Pour tout $x \in G$, soit $p(x) = x.(-f(x))$ qui ne dépend que de la classe de $x$ suivant H. Posons

$$
\text{(1)} \quad F(x, y) = p(xy)^{-1}p(x)p(y) = f(xy)y^{-1}x^{-1}x(-f(x))y(-f(y))
= f(xy)[y^{-1}(-f(x))y](-f(y))
= f(xy) - \pi(y)^{-1}f(x) - f(y).
$$

On voit que, si $F(x, y) = 0$ quels que soient $x,\ y$ dans G, $p(G) = L$ est un sous-groupe de G qui rencontre toute classe suivant H en un point et un seul. Comme $p$ est continu, G est alors produit semi-direct topologique de L et de H (Top. gén., chap. III, 3e éd., § 2, no 10).

Or, quels que soient $h,\ h' \in H$, on a

$$
F(xh, yh') = f(xhyh') - \pi(y)^{-1}f(xh) - f(yh')
= f(xhy) + h' - \pi(y)^{-1}f(x) - \pi(y)^{-1}h - f(y) - h'
= f(xy(\pi(y)^{-1}h)) - \pi(y)^{-1}f(x) - f(y) - \pi(y)^{-1}h
= f(xy) - \pi(y)^{-1}f(x) - f(y) = F(x, y).
$$

Donc F définit par passage aux quotients une application continue $\varphi$ de $K \times K$ dans H.

D'autre part, quels que soient $x, y, z$ dans $G$, on a
$$
\begin{align*}
F(z, xy) + F(x, y) &= f(zxy) - \pi(xy)^{-1}f(z) - f(xy) + f(xy) \\
&\quad - \pi(y)^{-1}f(x) - f(y) \\
&= \pi(y)^{-1}f(zx) - \pi(xy)^{-1}f(z) - \pi(y)^{-1}f(x) + f(zxy) \\
&\quad - \pi(y)^{-1}f(zx) - f(y) \\
&= \pi(y)^{-1}F(z, x) + F(zx, y)
\end{align*}
$$
donc, quels que soient $x', y', z'$ dans $K$, on a
$$
-\varphi(x', y') = \varphi(z', x'y') - {y'}^{-1}\varphi(z', x') - \varphi(z'x', y').
$$
Intégrons par rapport à $z'$ au moyen de la mesure de Haar normalisée $\alpha$ de $K$. Si on pose $\psi(x') = \int \varphi(z', x') d\alpha(z')$, $\psi$ est une fonction continue sur $K$, et on obtient (en observant que les opérations de $K$ dans $\mathbf{R}^n$ respectent la structure d'espace vectoriel de $\mathbf{R}^n$ d'après *Top. gén.*, chap. VII, § 2, no 1, prop. 1)
$$
-\varphi(x', y') = \psi(x'y') - {y'}^{-1}\psi(x') - \psi(y').
$$
Autrement dit, en posant $k = \psi \circ \pi$, qui est une fonction continue dans $G$,
(2)
$$
-F(x, y) = k(xy) - \pi(y)^{-1}k(x) - k(y).
$$
Comparant (1) et (2), on voit que, si on remplace $f$ par la fonction continue $f + k$, (ce qui laisse vérifiée la propriété $f(xh) = f(x) + h$), on remplace $F$ par 0, et, comme on l’a vu plus haut, ceci achève la démonstration de a).

Pour tout $g \in G$, soit $l_g$ (resp. $h_g$) l’unique élément de $L$ (resp. $H$) tel que $g = h_g l_g$. Si $h_1 \in H$ et $g \in G$, on a
$$
gh_1 = h_g l_g h_1 = h_g (l_g h_1 l_g^{-1}) l_g
$$
donc $h_g = h_{g h_1} + l_g h_1 l_g^{-1}$. Pour tout $g \in G$, soit $\psi_g$ l’application de $H$ dans lui-même définie par
$$
\psi_g(h_1) = h_g + l_g h_1 l_g^{-1}.
$$
On voit que l’application $(g, h_1) \to \psi_g(h_1)$ de $G \times H$ dans $H$ est continue et fait de H un espace homogène pour G, dans lequel le stabilisateur de l’origine est L. Remarquons en outre que lorsqu’on identifie H à $\mathbf{R}^n$, $\psi_g$ est une application *affine* de H dans lui-même. Ceci posé, soit M un sous-groupe compact de G ; en vertu du lemme 2, il existe un $x \in H$ tel que $\psi_m(x) = x$ pour *tout* $m \in M$. Pour $y \in H$, $\psi_y$ est la translation de vecteur $y$; on en déduit que pour tout $m \in M$, $\psi_{x^{-1}} \circ \psi_m \circ \psi_x$ transforme l’origine de H en elle-même, donc $x^{-1}mx \in L$. Ceci prouve que $x^{-1}Mx \subset L$, d’où b).

Soit L’ un sous-groupe fermé de G contenant L. Alors L’ est produit semi-direct topologique de L et de $L' \cap H$. Si L’ est compact, $L' \cap H$ est compact, donc se réduit à un point (*Top. gén.*, chap. VII, § 1, no 2, cor. 1 du th. 2), donc $L' = L$. Ceci prouve que L est un sous-groupe compact maximal de G ; il en est donc de même des sous-groupes transformés de L par les automorphismes intérieurs de G. Les assertions c) et d) de la prop. 3 sont alors des conséquences immédiates de b).

#### Proposition 4 {#int-vii-s3-prop-4 .statement}

*Soient G un groupe localement compact et H un sous-groupe distingué fermé de G tel que K = G/H soit compact. Alors toute représentation continue u de H dans $\mathbf{R}$, telle que $u(s\xi s^{-1}) = u(\xi)$ quels que soient $\xi \in H$ et $s \in G$, peut être prolongée en une représentation continue de G dans $\mathbf{R}$.*

Soient $L = G \times \mathbf{R}$, et M l’ensemble des $(\xi, -u(\xi))$ où $\xi$ parcourt H. Il est clair que M est un sous-groupe distingué fermé de L. Soient $L' = L/M$ et $\pi$ l’application canonique de L sur L’. Le sous-groupe de L engendré par M et $\mathbf{R}$ est $H \times \mathbf{R}$, donc est fermé ; donc $\pi(\mathbf{R})$ est un sous-groupe fermé N de L’. La restriction $\rho$ de $\pi$ à $\mathbf{R}$ est une représentation continue bijective de $\mathbf{R}$ sur N. Le lemme 2 de l’Appendice 1 prouve que $\rho$ est bicontinue. Par ailleurs, $L'/N$ est isomorphe à

$$
L/(H \times \mathbf{R}) = G/H,
$$

donc est compact. D’après la prop. 3, et compte tenu du fait que N est dans le centre de L’, L’ est le produit de N et d’un autre sous-groupe. Il existe donc une représentation continue de L’ sur N qui se réduit sur N à l’application identique. Donc il existe une représentation continue $v$ de $L$ sur $\mathbf{R}$ qui est triviale sur $M$ et se réduit sur $\mathbf{R}$ à l’application identique. Pour $\xi \in H$, on a $v((\xi, 0)) = v((\xi, -u(\xi)(e, u(\xi)))) = u(\xi)$, ce qui achève la démonstration.

#### Lemme 3 {#int-vii-s3-lem-3 .statement}

*Soit G un groupe topologique engendré par un voisinage compact de e. Soit H un sous-groupe fermé de G tel que l’espace homogène G/H soit compact. Alors, H est engendré par un voisinage compact de e dans H.*

Soit C un ensemble compact tel que $G = CH$. En agrandissant C, on peut supposer que C engendre G et que $G = \dot{C}H$. Alors $C^2$ est compact et recouvert par les $\dot{C}s$ ($s \in H$) qui sont ouverts. Donc il existe $s_1, \ldots, s_n$ dans H tels que $C^2 \subset \dot{C}s_1 \cup \ldots \cup \dot{C}s_n$. Soit $\Gamma$ le sous-groupe de H engendré par les $s_i$. On a $C^2 \subset C\Gamma$. Par récurrence, on en déduit $C^n \subset C\Gamma$ pour tout $n$, donc $G = C\Gamma$. Tout élément de H se met sous la forme $ab$ avec $a \in C, b \in \Gamma$, d’où $a \in H$, d’où $a \in C \cap H$. Donc H est engendré par $C \cap H$ et les $s_i$, c’est-à-dire par un ensemble compact.

#### Lemme 4 {#int-vii-s3-lem-4 .statement}

*Soient G un groupe topologique connexe, D un sous-groupe totalement discontinu distingué de G. Alors D est contenu dans le centre de G.*

En effet, soit $d \in D$. L’image de G par l’application continue $x \to dx d^{-1}$ est un sous-ensemble connexe de D, donc se réduit à $\{d\}$, ce qui prouve que $xd = dx$ pour tout $x \in G$.

#### Proposition 5 {#int-vii-s3-prop-5 .statement}

*Soit G un groupe topologique connexe admettant un sous-groupe distingué discret D tel que K = G/D soit compact, et que le groupe des commutateurs de K soit dense dans K. Alors D est fini et G est compact.*

Le groupe G est localement isomorphe à K (*Top. Gén.*, chap. III, 3e éd., § 2, no 6, prop. 19) donc localement compact ; puisqu’il est connexe, il est engendré par un voisinage compact de e. D’après les lemmes 3 et 4, D est un groupe commutatif de type fini, donc isomorphe à un groupe $\mathbf{Z}^r \times D_1$ avec $D_1$ fini (*Alg.*, chap. VII, § 4, no 6, th. 3). Supposons $r > 0$. Il existe alors une représentation $f$ de $D$ sur $\mathbf{Z}$. D’après la prop. 4, $f$ se prolonge en une représentation continue $g$ de $G$ dans $\mathbf{R}$. Par passage aux quotients, $g$ définit une représentation continue $g'$ de $K$ dans $\mathbf{R}/\mathbf{Z}$; comme $\mathbf{R}/\mathbf{Z}$ est commutatif, le noyau de $g'$ contient le groupe des commutateurs de $K$, donc $g'$ est triviale ; autrement dit, $g(G) \subset \mathbf{Z}$. Comme $G$ est connexe, on en déduit $g(G) = \{0\}$, ce qui est absurde puisque $f(D) = \mathbf{Z}$. Donc $r = 0$ et $D$ est fini. Par suite $G$ est compact (*Top. Gén.*, chap. III, 3<sup>e</sup> éd., § 4, no 1, cor. 2 de la prop. 2).

### 3. Exemples.

Dans ce no (exception faite des exemples 7 et 8), $K$ désignera un corps commutatif localement compact non discret ; $dx$ désignera une mesure de Haar sur le groupe additif de $K$.

On rappelle que $\operatorname{mod} x = |x|$ si $K = \mathbf{R}$, $\operatorname{mod} x = |x|^2$ si $K = \mathbf{C}$, $\operatorname{mod} x = |x|_p$ si $K = \mathbf{Q}_p$.

**Exemple 1. — Groupe linéaire.**

Soit $A$ l’algèbre $\mathbf{M}_n(K)$. Le groupe $A^*$ des éléments inversibles de $A$ n’est autre que le groupe linéaire $\mathbf{GL}(n, K)$. Pour tout $X \in A$, la norme réduite $\mathrm{Nrd}_{A/K}(X)$ est $\det X$ ; par suite, $N_{A/K}(X) = (\det X)^n$ (*Alg.*, chap. VIII, § 12, no 3, prop. 8). Comme $X \to {}^t X$ est un isomorphisme de $A$ sur l’algèbre opposée, on a $N_{A^*/K}(X) = N_{A/K}({}^t X) = \det ({}^t X)^n = (\det X)^n$. Alors, la prop. 16 du § 1, no 11 prouve que

$$
\operatorname{mod} (\det X)^{-n} \cdot \bigotimes_{i,j} dx_{ij} \tag{3}
$$

$(X = (x_{ij}))$

est une mesure de Haar à gauche et à droite sur $\mathbf{GL}(n, K)$.

Pour déterminer toutes les mesures relativement invariantes sur $\mathbf{GL}(n, K)$, on s’appuiera sur le lemme suivant :

**Lemme 5. — Les représentations continues de $\mathbf{GL}(n, K)$ dans $\mathbf{C}^*$ sont les applications de la forme $X \to \chi(\det X)$, où $\chi$ est une représentation continue de $K^*$ dans $\mathbf{C}^*$.**

Une telle application est évidemment une représentation continue de $\mathbf{GL}(n, K)$ dans $\mathbf{C}^*$. Réciproquement, soit $\psi$ une représentation continue de $\mathbf{GL}(n, K)$ dans $\mathbf{C}^*$. Pour $x \in K^*$, posons

$$
\widetilde{x} = \begin{pmatrix}
x & & \\
& 1 & 0 \\
& 0 & 1 \\
& & \ddots \\
& & & 1
\end{pmatrix}
$$

et $\chi(x) = \psi(\widetilde{x})$. Alors, pour toute matrice $X \in \mathbf{GL}(n, K)$, on a $(\det X^{-1})^\sim . X \in \mathbf{SL}(n, K)$. Comme $\mathbf{SL}(n, K)$ est le groupe des commutateurs de $\mathbf{GL}(n, K)$ (*Alg.*, chap. III, 3e éd.), on a $\psi((\det X^{-1})^\sim . X) = 1$, d'où

$$
\psi(X) = \psi((\det X)^\sim) = \chi(\det X).
$$

Ceci posé, le cor. 1 de la prop. 10 du § 1, no 8, prouve que les mesures relativement invariantes sur $\mathbf{GL}(n, K)$ sont, à un facteur constant près, les mesures de la forme

$$
\chi(\det X) \cdot \bigotimes_{i,j} dx_{ij} \tag{4} \quad (X = (x_{ij}))
$$

où $\chi$ est une représentation continue de $K^*$ dans $\mathbf{C}^*$.

#### Exemple 2 {#int-vii-s3-n3-exa-2 .statement}

*Groupe affine.*
Pour tout $X \in \mathbf{GL}(n, K)$ et tout $x \in K^n$, soit $(X, x)$ l’application linéaire affine $\xi \to X\xi + x$ dans $K^n$. L’ensemble des $(X, x)$ est le groupe affine $G$ de $K^n$ (*Alg.*, chap. II, 3e éd., § 9, no 4). L’ensemble $T$ des translations est un sous-groupe distingué fermé de $G$, canoniquement isomorphe à $K^n$; d’autre part, $\mathbf{GL}(n, K)$ est un sous-groupe fermé de $G$, et $G$ est produit semi-direct de $\mathbf{GL}(n, K)$ et $T = K^n$. On munit $G$ de la topologie (localement compacte) pour laquelle $G$ est produit semi-direct topologique de $\mathbf{GL}(n, K)$ et de $T$ (*Top. gén.*, chap. III, § 2, no 10). On a

$$
(X, x) = (1, x) . (X, 0).
$$

D’autre part, si $X \in \mathbf{GL}(n, K)$ et $x \in T$, on a, pour tout $\xi \in K^n$,

$$
(X, 0)(1, x)(X, 0)^{-1}\xi = X(X^{-1}\xi + x) = \xi + Xx = (1, Xx)\xi
$$

donc l’automorphisme $(1, x) \to (X, 0)(1, x)(X, 0)^{-1}$ de $T$ a pour module $\operatorname{mod}(\det X)$ (§ 1, no 10, prop. 15). Compte tenu de l’exemple 1 et du § 2, no 9, *Remarque*,

(5) $$
\operatorname{mod}(\det X)^{-n-1}. (\bigotimes_{i,j} dx_{ij}) \otimes (\bigotimes_i dx_i) \quad (X = (x_{ij}),\ x = (x_i))
$$
est une mesure de Haar à gauche sur $G$. D’autre part, d’après la prop. 14 du § 2, no 9,
$$
\Delta_G((X, x)) = \Delta_{\mathbf{GL}(n, K)}(X)\Delta_{K^n}(x)(\operatorname{mod} \det X)^{-1}
$$
ou
(6)
$$
\Delta_G((X, x)) = \operatorname{mod}(\det X^{-1}).
$$
Donc une mesure de Haar à droite sur $G$ est
(7)
$$
(\operatorname{mod} \det X)^{-n}. (\bigotimes_{i,j} dx_{ij}) \otimes (\bigotimes_i dx_i).
$$

#### Exemple 3 {#int-vii-s3-n3-exa-3 .statement}

*Groupe trigonal strict*.

Soit $[1, n]$ l’ensemble des entiers $m$ tels que $1 \leq m \leq n$. Soit $J$ un sous-ensemble de $[1, n] \times [1, n]$ satisfaisant aux conditions suivantes :
1) si $(i, j) \in J$, on a $i < j$;
2) si $(i, j) \notin J$, alors, pour tout entier $k$ tel que $i < k < j$, l’un au moins des deux couples $(i, k)$ et $(k, j)$ n’appartient pas à $J$.

Soit $T_J$ l’ensemble des matrices $Z = (z_{ij})_{1 \leq i \leq n,\ 1 \leq j \leq n}$ à éléments dans $K$, telles que $z_{ii} = 1$, et $z_{ij} = 0$ pour $i \neq j$ et $(i, j) \notin J$. C’est un sous-ensemble fermé de $\mathbf{GL}(n, K)$. L’application $Z \to (z_{ij})_{(i, j) \in J}$ est un homéomorphisme de $T_J$ sur $K^s$ (où $s$ désigne le nombre d’éléments de $J$). Si $Z' = (z'_{ij}) \in T_J$, on a $Z'Z = (z''_{ij})$ avec
$$
z''_{ij} = z_{ij} + z'_{ij} + \sum_{i < h < j} z'_{ih}z_{hj} \text{ pour } i < j
$$
$$
z''_{ij} = 0 \text{ pour } i > j,\ z''_{ii} = 1
$$
d’où $Z'Z \in T_J$. Si on identifie $T_J$ à $K^s$, l’application $Z \to Z'Z$ (pour $Z'$ fixé) s’identifie à une application affine, et son déterminant est 1, comme on le voit en ordonnant lexicographiquement les couples $(i, j) \in J$ et en appliquant le lemme suivant :

#### Lemme 6 {#int-vii-s3-lem-6 .statement}

*Soit L un ensemble fini totalement ordonné. Pour tout $\lambda \in L$, soit $V_\lambda$ un module libre de dimension finie sur un anneau commutatif $k$; pour $\lambda, \mu$ dans $L$ tels que $\lambda \leq \mu$, soit $f_{\lambda \mu} \in \mathrm{Hom}_k(V_\mu, V_\lambda)$. Alors l’application linéaire*

$$
(v_\lambda)_{\lambda \in L} \mapsto \left( \sum_{\mu \geq \lambda} f_{\lambda \mu}(v_\mu) \right)_{\lambda \in L},
$$

*de $\prod_{\lambda \in L} V_\lambda$ dans $\prod_{\lambda \in L} V_\lambda$, a pour déterminant $\prod_{\lambda \in L} \det f_{\lambda \lambda}$.

On se ramène aussitôt au cas où L est un intervalle d’entiers et le lemme résulte alors d’*Alg.*, chap. III.

Si $Z \in T_J$, on voit alors qu’il existe $Z' \in T_J$ tel que $Z'Z = I_n$, d’où $Z' = Z^{-1}$. Ainsi, $T_J$ est un sous-groupe fermé de $\mathbf{GL}(n, K)$. D’autre part, la prop. 15 du § 1, n° 10, montre que la mesure

$$
\bigotimes_{(i, j) \in J} dz_{ij}
$$

est une mesure de Haar à gauche sur $T_J$. En calculant $ZZ'$, on voit de la même façon que cette mesure est une mesure de Haar à droite sur $T_J$.

On a un résultat analogue si on échange, dans la définition de $T_J$, le rôle des lignes et des colonnes.

Lorsque $J$ est l’ensemble des couples $(i, j)$ tels que $i < j$, le groupe $T_J$ s’appelle *groupe trigonal strict supérieur* d’ordre $n$ sur $K$ et se note $T_1(n, K)$. Son transposé s’appelle *groupe trigonal strict inférieur*.

#### Exemple 4 {#int-vii-s3-n3-exa-4 .statement}

*Groupe trigonal large.*

Soient $n_1, \ldots, n_r$ des entiers $\geq 1$. Posons $p_k = n_1 + \ldots + n_{k-1}$ et $n = p_{r+1} = n_1 + \ldots + n_r$. Soient $I_k$ l’ensemble des entiers $j$ tels que $p_k < j \leq p_{k+1}$ et $J$ la réunion des $I_k \times I_l$ pour $k < l$. Soit G le sous-groupe fermé de $\mathbf{GL}(n, K)$ dont les éléments sont les matrices $(Z_{kl})_{1 \leq k \leq r,\ 1 \leq l \leq r}$ telles que :

1) chaque $Z_{kl}$ est une matrice $(z_{ij})_{i \in I_k, j \in I_l}$ à éléments dans $K$, à $n_k$ lignes et à $n_l$ colonnes ;
2) $Z_{kl} = 0$ pour $k > l$;
3) $Z_{kk} \in \mathbf{GL}(n_k, K)$ pour $1 \leq k \leq r$.
La formule de produits par blocs

$$
\begin{pmatrix}
Z_{11} & 0 & \ldots & 0 \\
0 & Z_{22} & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}
\begin{pmatrix}
1 & Z_{12} & \ldots & Z_{1r} \\
0 & 1 & \ldots & Z_{2r} \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & 1
\end{pmatrix}
$$

$$
= \begin{pmatrix}
Z_{11} & Z_{11}Z_{12} & \ldots & Z_{11}Z_{1r} \\
0 & Z_{22} & \ldots & Z_{22}Z_{2r} \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}
$$

montre que $G$ est produit semi-direct topologique du sous-groupe $D$ des éléments $(Z_{kl}) \in G$ tels que $Z_{kl} = 0$ pour $k \neq l$ et du sous-groupe $T_J$ de l’exemple 3. De plus $D$ est isomorphe au produit direct des groupes $\mathbf{GL}(n_k, K)$ pour $1 \leq k \leq r$.

Soit $J'$ l’ensemble des couples $(j, i)$ pour $(i, j) \in J$ et soit $H$ l’ensemble des couples $(i, j) \in \{1, n\} \times \{1, n\}$ n’appartenant pas à $J'$. Soit $Z' = (z_{ij})_{1 \leq i \leq n, 1 \leq j \leq n}$ un élément de $G$. D’après la prop. 14 du § 2, no 9 et les exemples 1 et 3 ci-dessus, on obtient une mesure de Haar à gauche sur $G$ en prenant l’image de la mesure

$$
\bigotimes_{k=1}^r ((\operatorname{mod} \det Z_{kk})^{-n_k} \cdot \bigotimes_{i, j \in I_k} dz_{ij}) \otimes (\bigotimes_{(i, j) \in J} dz_{ij})
$$

par l’application

$$
((Z_{kk}), (Z_{kl})) \to \begin{pmatrix}
Z_{11} & Z_{11}Z_{12} & \ldots & Z_{11}Z_{1r} \\
0 & Z_{22} & \ldots & Z_{22}Z_{2r} \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}
$$

Or, considérons, pour $k < l$, l’espace vectoriel des matrices $Z_{kl} = (z_{ij})_{i \in I_k, j \in I_l}$. Il est somme directe des $n_l$ sous-espaces $M_j$ ($j \in I_l$) formé des matrices telles que $z_{ih} = 0$ pour $h \neq j$. Chacun de ces sous-espaces $M_j$ est stable par l’application

Z_{kl} \to Z_{kk}Z_{kl}, et la restriction à M_j de cette application admet pour matrice $Z_{kk}$. Par suite (§ 1, no 10, prop. 15) l’image de la mesure $\bigotimes_{i \in I_k, j \in I_l} dz_{ij}$ par l’application $Z_{kl} \to Z_{kk}Z_{kl}$ est
$$
(\text{mod det } Z_{kk})^{-n_l} \cdot \bigotimes_{i \in I_k, j \in I_l} dz_{ij}.
$$
Une mesure de Haar à gauche sur G est donc
$$
(9) \quad \prod_{k=1}^r (\text{mod det } Z_{kk})^{-q_k} \cdot \bigotimes_{(i, j) \in H} dz_{ij}
$$
avec $q_k = \sum_{k \leq l \leq r} n_l = n - p_k$.

Calculons le module de G en utilisant encore la prop. 14 du § 2. Les groupes D et T_J sont unimodulaires ; d’autre part :
$$
\begin{pmatrix}
Z_{11} & 0 & \ldots & 0 \\
0 & Z_{22} & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}
\begin{pmatrix}
1 & Z_{12} & \ldots & Z_{1r} \\
0 & 1 & \ldots & Z_{2r} \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & 1
\end{pmatrix}
\begin{pmatrix}
Z_{11} & 0 & \ldots & 0 \\
0 & Z_{22} & \ldots & 0 \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}^{-1}
$$
$$
= \begin{pmatrix}
1 & Z'_{12} & \ldots & Z'_{1r} \\
0 & 1 & \ldots & Z'_{2r} \\
\ldots & \ldots & \ldots & \ldots \\
0 & 0 & \ldots & 1
\end{pmatrix}
$$
avec $Z'_{kl} = Z_{kk}Z_{kl}Z_{ll}^{-1}$. Compte tenu de l’exemple 3 et de la prop. 15 du § 1, no 10, on voit en raisonnant comme ci-dessus que si $X = \operatorname{diag}(Z_{11}, \ldots, Z_{rr}) \in D$, le module de l’automorphisme $Z \to X^{-1}ZX$ de T_J est
$$
\prod_{k < l} (\text{mod det } Z_{kk})^{-n_l} (\text{mod det } Z_{ll})^{n_k}
$$
donc
$$
(10) \quad \Delta_G(Z) = \prod_{k=1}^r (\text{mod det } Z_{kk})^{n + n_k - 2q_k}
$$
Le groupe G’ transposé de G s’étudie de la même manière. On trouve comme mesure de Haar à gauche
$$
\prod_{k=1}^r (\text{mod det } Z_{kk})^{-p_{k+1}} \cdot \bigotimes_{(j, i) \in H} dz_{ij}
$$

et comme module de $G'$

$$
\prod_{k=1}^{r} (\text{mod det } Z_{kk})^{n+n_k-2p_{k+1}}
$$

Si en particulier on prend $n_1 = \ldots = n_r = 1$, on trouve pour groupe $G$ le groupe $T(n, K)^*$ des éléments inversibles de la sous-algèbre de $\mathbf{M}_n(K)$ formée des matrices $X = (x_{ij})$ telles que $x_{ij} = 0$ pour $i > j$. Cette algèbre, que nous noterons $T(n, K)$, est appelée *algèbre trigonale supérieure*, et le groupe $T(n, K)^*$ est appelé *groupe trigonal large supérieur* d’ordre $n$ sur $K$. Les formules précédentes prennent alors la forme que voici : une mesure de Haar à gauche sur $T(n, K)^*$ est

(9 bis)
$$
\prod_{i=1}^{n} (\text{mod } z_{ii})^{i-n-1} \cdot \bigotimes_{i \leq j} dz_{ij} \qquad (Z = (z_{ij}))
$$
et le module de $T(n, K)^*$ est

(10 bis)
$$
\Delta_{T(n, K)^*}(Z) = \prod_{i=1}^{n} (\text{mod } z_{ii})^{2i-n-1} \qquad (Z = (z_{ij}))
$$
Pour le transposé de $T(n, K)^*$, ou *groupe trigonal large inférieur*, on trouve comme mesure de Haar à gauche

$$
\prod_{i=1}^{n} (\text{mod } z_{ii})^{-i} \cdot \bigotimes_{i \geq j} dz_{ij}
$$
et comme module

$$
\prod_{i=1}^{n} (\text{mod } z_{ii})^{n+1-2i}
$$

#### Remarque {#int-vii-s3-n3-rem-1 .statement}

Le groupe $T(n, K)^*$ est un sous-groupe fermé de $\mathbf{GL}(n, K)$, et $\Delta_{T(n, K)^*}((z_{ij})) = \prod_{i=1}^{n} (\text{mod } z_{ii})^{2i-n-1}$. On a vu dans l’exemple 1 que $\Delta_{\mathbf{GL}(n, K)} = 1$. Si $n > 1$, la fonction

$$
\Delta_{\mathbf{GL}(n, K)}/\Delta_{T(n, K)^*}
$$

sur $T(n, K)^*$ ne peut se prolonger en une représentation continue de $G$ dans $\mathbf{C}^*$ (car une telle représentation est égale à 1 sur $\mathbf{SL}(n, K)$ d’après le lemme 5, alors que $\operatorname{mod}(z_{11})^{1-n} \neq 1$ pour $z_{11}$ bien choisi). Il en résulte que l’espace homogène $\mathbf{GL}(n, K)/T(n, K)^*$ n’admet aucune mesure relativement invariante si $n > 1$ ($\S$ 2, no 6, th. 3).

Cet espace homogène s’identifie, pour $n = 2$, à la droite projective sur $K$. En effet, soit $(e_1, e_2)$ la base canonique de $K^2$. Le groupe $\mathbf{GL}(2, K)$ opère transitivement sur l’ensemble des droites de $K^2$ privées de 0, et le stabilisateur de $Ke_1 - \{0\}$ est $T(2, K)^*$.

**Exemple 5. — Groupe trigonal spécial.**

Reprenons les notations du début de l’exemple 4, et considérons le sous-groupe $G_1 = G \cap \mathbf{SL}(n, K)$. Il est produit semi-direct topologique du groupe $D_1 = D \cap \mathbf{SL}(n, K)$ et de $T_J$. Le groupe $D_1$ admet un sous-groupe distingué $A$ isomorphe à $\mathbf{SL}(n_r, K)$, à savoir le sous-groupe composé des éléments $\operatorname{diag}(Z_{kk})$ avec $Z_{kk} = 1$ pour $k < r$. L’homomorphisme

$$
\varphi : \operatorname{diag}(Z_{11}, \ldots, Z_{rr}) \to (Z_{11}, \ldots, Z_{r-1, r-1})
$$

de $D_1$ dans $\mathbf{GL}(n_1, K) \times \ldots \times \mathbf{GL}(n_{r-1}, K)$ est surjectif et de noyau $A$. D’autre part, $\varphi$ est continu. Compte tenu du lemme 2 de l’Appendice I, $D_1/A$ peut s’identifier à

$$
\mathbf{GL}(n_1, K) \times \ldots \times \mathbf{GL}(n_{r-1}, K).
$$

Nous désignerons par $\mu$ la mesure de Haar sur $A$ (cf. *Exemple 6*) et par

$$
\alpha = \bigotimes_{k=1}^{r-1} ((\operatorname{mod} \det Z_{kk})^{-n_k} \cdot \bigotimes_{i, j \in I_k} dz_{ij}) \otimes' (d\mu(Z_{rr}))
$$

la mesure de Haar sur $D_1$ telle que

$$
\alpha/\mu = \bigotimes_{k=1}^{r-1} ((\operatorname{mod} \det Z_{kk})^{-n_k} \cdot \bigotimes_{i, j \in I_k} dz_{ij})
$$

($\S$ 2, no 7, prop. 10). On montre alors comme dans l’*Exemple 4* qu’une mesure de Haar à gauche sur $G_1$ est

$$
\operatorname{mod} \left( \prod_{k=1}^{r-1} (\det Z_{kk})^{n_k - a_k} \right)
$$
$$
\cdot \left[ \bigotimes_{k=1}^{r-1} ((\operatorname{mod} \det Z_{kk})^{-n_k} \bigotimes_{i,j \in I_k} dz_{ij}) \otimes' d\mu(Z_{rr}) \right] \otimes \bigotimes_{(i,j) \in J} dz_{ij}
$$

Comme $G_1$ est distingué dans $G$, le module de $G_1$ est la restriction de celui de $G$ (§ 2, no 7, prop. 10 b).

Si $n_r = 1$, le sous-groupe $A$ est réduit à l’élément neutre et une mesure de Haar à gauche sur $G$ est

$$
\operatorname{mod} \left( \prod_{k=1}^{r-1} (\det Z_{kk})^{-a_k} \right) \cdot \bigotimes_{k=1}^{r-1} \left( \bigotimes_{i,j \in I_k} dz_{ij} \right) \otimes \bigotimes_{(i,j) \in J} dz_{ij}
$$

Si l’on prend $n_1 = n_2 = \ldots = n_r = 1$, le groupe $G_1$ obtenu s’appelle groupe trigonal spécial supérieur et son transposé $G'_1$ s’appelle groupe trigonal spécial inférieur. Une mesure de Haar à gauche sur $G_1$ est

$$(11)$$
$$
\operatorname{mod} \left( \prod_{i=1}^{n-1} z_{ii}^{i-n-1} \right) \cdot \left( \bigotimes_{i=1}^{n-1} dz_{ii} \right) \otimes \left( \bigotimes_{1 \leq i < j \leq n} dz_{ij} \right)
$$

et le module de $G_1$ est

$$(12)$$
$$
\operatorname{mod} \left( \prod_{i=1}^{n-1} z_{ii}^{2i-2n} \right)
$$

On trouve de même pour mesure de Haar à gauche sur $G'_1$

$$
\operatorname{mod} \left( \prod_{i=1}^{n-1} z_{ii}^{n-i-1} \right) \cdot \left( \bigotimes_{i=1}^{n-1} dz_{ii} \right) \otimes \left( \bigotimes_{1 \leq j < i \leq n} dz_{ij} \right)
$$

et pour module

$$
\operatorname{mod} \left( \prod_{i=1}^{n-1} z_{ii}^{2n-2i} \right).
$$

#### Exemple 6 {#int-vii-s3-n3-exa-6 .statement}

*Groupe linéaire spécial.*

Les sous-groupes fermés $T_1(n, K)$ et $t(T(n, K)^*)$ de $\mathbf{GL}(n, K)$ ont pour intersection $\{e\}$. Donc l’application $(M, N) \to M . N$ est une bijection continue $\varphi$ de $T_1(n, K) \times {}^t(T(n, K)^*)$ sur une partie $\Omega$ de $\mathbf{GL}(n, K)$.

#### Lemme 7 {#int-vii-s3-lem-7 .statement}

a) *Soit $U = (u_{ij}) \in \mathbf{GL}(n, K)$. Pour que $U \in \Omega$, il faut et il suffit que $\det(u_{ij})_{k \leq i, j \leq n} \neq 0$ pour $k = 2, 3, \ldots, n$.
    b) $\Omega$ est une partie ouverte de $\mathbf{GL}(n, K)$.
    c) *L’application $\varphi$ est un homéomorphisme de*
        $$
        T_1(n, K) \times {}^t(T(n, K)^*)
        $$
    *sur* $\Omega$.

Pour que $U \in \Omega$, il faut et il suffit qu’il existe un
$$
Z = (z_{ij}) \in T_1(n, K)
$$
tel que $ZU \in {}^t(T(n, K))$ (on aura alors nécessairement $ZU \in {}^t(T(n, K)^*)$ puisque $U$ et $Z$ sont inversibles). D’après ce qu’on a vu plus haut, si $Z$ existe, il est unique. Donc, pour que $U \in \Omega$, il faut et il suffit que le système linéaire
$$
\sum_{k=1}^n z_{ik} u_{kj} = 0 \qquad (1 \leq i < j \leq n)
$$
(où $(z_{ij}) \in T_1(n, K)$) admette une solution unique. Or ce système peut s’écrire
$$
\sum_{k=i+1}^n z_{ik} u_{kj} = -u_{ij} \qquad (1 \leq i < j \leq n).
$$
Pour $i$ fixé, on a un système de $n - i$ équations par rapport aux inconnues $z_{i,i+1}, z_{i,i+2}, \ldots, z_{i,n}$; pour que ces systèmes admettent des solutions uniques, il faut et il suffit que
$$
\det(u_{kj})_{i+1 \leq k \leq n, i+1 \leq j \leq n} \neq 0
$$
pour $i = 1, 2, \ldots, n - 1$. Ceci prouve a). Il en résulte que $\Omega$ est ouvert dans $\mathbf{GL}(n, K)$. D’autre part, en résolvant le système (13) par les formules de Cramer, on obtient les $z_{ij}$ comme fonctions rationnelles des $u_{ij}$ à dénominateurs non nuls dans $\Omega$, donc $Z$ dépend continûment de $U$ dans $\Omega$, ce qui prouve c).

Soit maintenant $G'_1 \subset {}^t(T(n, K)^*)$ le groupe trigonal spécial inférieur. L’application $(M, N) \to M.N$ est une bijection continue $\psi$ de $T_1(n, K) \times G'_1$ sur une partie $\Omega'$ de $\mathbf{SL}(n, K)$.

#### Lemme 8 {#int-vii-s3-lem-8 .statement}

a) *Soit $U = (u_{ij}) \in \mathbf{SL}(n, K)$. Pour que $U \in \Omega'$, il faut et il suffit que $\det(u_{ij})_{k \leq i,j \leq n} \neq 0$ pour $k = 2, 3, \ldots, n$.*
b) *$\Omega'$ est une partie ouverte de $\mathbf{SL}(n, K)$.*
c) *L’application $\psi$ est un homéomorphisme de $T_1(n, K) \times G'_1$ sur $\Omega'$.*

En effet, soient $M \in T_1(n, K)$ et $N \in {}^t(T(n, K)^*)$. Pour que $M.N \in \mathbf{SL}(n, K)$, il faut et il suffit que $N \in G'_1$. Donc

$$
\Omega' = \mathbf{SL}(n, K) \cap \Omega
$$

et le lemme 8 résulte aussitôt du lemme 7.

#### Proposition 6 {#int-vii-s3-prop-6 .statement}

a) *Le groupe $\mathbf{SL}(n, K)$ est unimodulaire.*
b) *Soient $\mu_1, \mu_2$ des mesures de Haar à gauche sur le groupe trigonal strict supérieur $T_1(n, K)$ et sur le groupe trigonal spécial inférieur $G'_1$. L’image de $\mu_1 \otimes \mu_2$ par l’homéomorphisme
$$
(M, N) \to M.N^{-1}
$$
de $T_1(n, K) \times G'_1$ sur $\Omega'$ est la restriction à $\Omega$ d’une mesure de Haar de $\mathbf{SL}(n, K)$.
c) *Le complémentaire de $\Omega'$ dans $\mathbf{SL}(n, K)$ est négligeable pour la mesure de Haar de $\mathbf{SL}(n, K)$.*

Le groupe $\mathbf{GL}(n, K)$ est unimodulaire (exemple 1), et $\mathbf{SL}(n, K)$ est un sous-groupe distingué de $\mathbf{GL}(n, K)$, donc est unimodulaire ($§ 2$, no 7, prop. 10, b)). L’assertion b) résulte de a), du lemme 8, et de la prop. 13 du $§ 2$, no 9. Prouvons c). D’après le lemme 8 a), il suffit de prouver ceci : si $p((u_{ij})_{1 \leq i,j \leq n})$ est un polynôme, non identiquement nul sur $\mathbf{SL}(n, K)$, l’ensemble E des $U \in \mathbf{SL}(n, K)$ tels que $p(U) = 0$ est négligeable pour la mesure de Haar. Compte tenu du $§ 1$, no 10, cor. de la prop. 13, la topologie de $\mathbf{SL}(n, K)$ est à base dénombrable. Il suffit donc de prouver que, pour tout $U_0 \in E$, il existe un voisinage de $U_0$ dans $\mathbf{SL}(n, K)$ dont l’intersection avec E est négligeable ; ou encore qu’il existe un voisinage W de I dans $\mathbf{SL}(n, K)$ tel que $U_0^{-1}E \cap W$ soit négligeable. Prenons $W = \Omega$. Compte tenu de b), tout revient à voir que l’ensemble des couples $(M, N) \in T_1(n, K) \times G'_1$ tels que $p(U_0MN) = 0$ est négligeable pour $\mu_1 \otimes \mu_2$. D’après les expressions de $\mu_1$ et $\mu_2$ (calculées aux exemples 3 et 5), ceci résultera du lemme suivant :

#### Lemme 9 {#int-vii-s3-lem-9 .statement}

*Soit $\psi$ un polynôme $\neq 0$ de $K[X_1, \ldots, X_r]$. Dans l’espace $K^r$, l’ensemble $N$ défini par $\psi(x_1, \ldots, x_r) = 0$ est négligeable pour la mesure de Haar.*

Raisonnons par récurrence sur $r$. Le lemme est évident pour $r = 1$, car alors $N$ est un ensemble fini. En changeant au besoin la numérotation des variables, on peut supposer que $\psi \notin K[X_1, \ldots, X_{r-1}]$; soit

$$
\psi(X_1, \ldots, X_r) = X_r^m \psi_0(X_1, \ldots, X_{r-1}) + \ldots + \psi_m(X_1, \ldots, X_{r-1})
$$

avec $m > 0$ et $\psi_0 \neq 0$. Dans l’espace $K^{r-1}$, soit $N_0$ l’ensemble défini par $\psi_0(x_1, \ldots, x_{r-1}) = 0$, qui est négligeable d’après l’hypothèse de récurrence. Pour tout $(x_1, \ldots, x_{r-1}) \notin N_0$, l’ensemble des $x_r \in K$ tels que $(x_1, \ldots, x_{r-1}, x_r) \in N$ est fini, donc négligeable. Comme $K^r$ est dénombrable à l’infini ($§ 1$, no 10, cor. de la prop. 13), $N \cap [(K^{r-1} - N_0) \times K]$ est négligeable dans $K^r$ (chap. V, $§ 8$, no 2, cor. 8 de la prop. 5). Donc $N$ est négligeable.

#### Exemple 7 {#int-vii-s3-n3-exa-7 .statement}

*Décomposition d’Iwasawa de $\mathbf{GL}(n, K)$.*

Dans cet exemple, $K$ désigne l’un des corps $\mathbf{R}, \mathbf{C}, \mathbf{H}$. Si $\lambda \in K$, on définit $\bar{\lambda}$ comme égal à $\lambda$ si $K = \mathbf{R}$, comme égal au conjugué de $\lambda$ si $K = \mathbf{C}$ ou $\mathbf{H}$. Soit $E$ un $K$-espace vectoriel à droite de dimension $n$, et soit $\Phi$ une forme hermitienne positive non dégénérée sur $E$.

#### Lemme 10 {#int-vii-s3-lem-10 .statement}

*Soit $(f_1, f_2, \ldots, f_n)$ une base de $E$.
a) Il existe une base orthonormale $(e_1, e_2, \ldots, e_n)$ et une seule de $E$ telle qu’on ait $f_i = e_1 \alpha_{i1} + e_2 \alpha_{i2} + \ldots + e_n \alpha_{in}$ ($i = 1, 2, \ldots, n$) avec $\alpha_{ii} > 0$ pour tout $i$.
b) Pour $\Phi$ fixée, les $e_i$ et les $\alpha_{ij}$ dépendent continûment de $(f_1, \ldots, f_n) \in E^n$.*

Soit $E_i = f_1 K + f_2 K + \ldots + f_i K$, qui est de dimension $i$. Soit $g_i$ un élément non nul de $E_i$ orthogonal à $E_{i-1}$ et tel que $\Phi(g_i, g_i) = 1$. Par récurrence sur $i$, on voit que $(g_1, \ldots, g_i)$ est une base orthonormale de $E_i$. En particulier, $(g_1, \ldots, g_n)$ est une base orthonormale de $E$. Soit $\lambda_i = \Phi(g_i, f_i)$. Comme $f_i \notin E_{i-1}$, on a $\lambda_i \neq 0$. Posons $e_i = g_i |\lambda_i| \lambda_i^{-1}$. On a
$$
\Phi(e_i, e_i) = |\lambda_i|^2 \overline{\lambda_i}^{-1} \Phi(g_i, g_i) \lambda_i^{-1} = 1,
$$
donc $(e_1, \ldots, e_i)$ est encore une base orthonormale de $E_i$; en outre, $\Phi(e_i, f_i) = |\lambda_i| \overline{\lambda_i}^{-1} \Phi(g_i, f_i) = |\lambda_i| > 0$, donc les $e_i$ possèdent les propriétés de a). Soient $(e'_1, \ldots, e'_n)$ une autre base orthonormale de $E$ avec ces mêmes propriétés. On voit par récurrence sur $i$ que $(e'_1, \ldots, e'_i)$ doit être une base de $E_i$, donc $e'_i = e_i \mu_i$ avec un $\mu_i \in K$. On a
$$
1 = \Phi(e'_i, e'_i) = \overline{\mu_i} \Phi(e_i, e_i) \mu_i = \overline{\mu_i} \mu_i,
$$
et $0 < \Phi(e'_i, f_i) = \overline{\mu_i} \Phi(e_i, f_i)$, donc $\mu_i > 0$ et $\mu_i^2 = 1$, donc $\mu_i = 1$, d'où a). Supposons prouvé que les $e_i$ et les $\alpha_{ij}$ dépendent continûment de $(f_1, \ldots, f_n)$ pour $i < i_0$, et prouvons que $e_{i_0}$ et les $\alpha_{i_0 j}$ dépendent continûment de $(f_1, \ldots, f_n)$. Pour $j < i_0$, $\overline{\alpha_{i_0 j}} = \Phi(f_{i_0}, e_j)$ dépend continûment de $(f_1, \ldots, f_n)$ d'après l'hypothèse de récurrence. D'autre part,
$$
\Phi(f_{i_0}, f_{i_0}) = |\alpha_{i_0 1}|^2 + |\alpha_{i_0 2}|^2 + \ldots + |\alpha_{i_0, i_0-1}|^2 + \alpha_{i_0, i_0}^2,
$$
donc $\alpha_{i_0, i_0}$ dépend continûment de $(f_1, \ldots, f_n)$. Donc
$$
e_{i_0} = (f_{i_0} - e_1 \alpha_{i_0 1} - \ldots - e_{i_0-1} \alpha_{i_0, i_0-1}) \alpha_{i_0 i_0}^{-1}
$$
dépend continûment de $(f_1, \ldots, f_n)$.

Soit désormais $E = K^n$ et prenons pour $\Phi$ la forme $\overline{x}_1 y_1 + \ldots + \overline{x}_n y_n$. Rappelons qu'on note $\mathbf{U}(n, K)$ le groupe unitaire correspondant. Même si $K$ est non commutatif, nous noterons encore $T_1(n, K)$ le groupe des matrices triangulaires supérieures de $\mathbf{M}_n(K)$ dont la diagonale est formée de 1.

#### Proposition 7 {#int-vii-s3-prop-7 .statement}

*Soit $D_*^+$ le groupe des matrices diagonales à éléments $> 0$. L’application $(U, D, T) \to UDT$ est un* homéomorphisme de $\mathbf{U}(n, K) \times D^*_+ \times T_1(n, K)$ sur $\mathbf{GL}(n, K)$.

Soit $(\varepsilon_1, \ldots, \varepsilon_n)$ la base canonique de $K^n$. Soit $X \in \mathbf{GL}(n, K)$. Alors les $X . \varepsilon_i = f_i$ constituent une base de E. On peut, à cette base $(f_i)$, associer une base $(e_i)$ grâce au lemme 10. Soit $U$ la matrice de l’automorphisme unitaire de E qui transforme $\varepsilon_i$ en $e_i$. Alors $U^{-1}.f_i = \varepsilon_1 \alpha_{i1} + \varepsilon_2 \alpha_{i2} + \ldots + \varepsilon_i \alpha_{ii}$ avec $\alpha_{ii} > 0$ pour $i = 1, 2, \ldots, n$. Donc $X = UC$, où $C$ est la matrice

$$
\begin{pmatrix}
\alpha_{11} & \alpha_{21} & \cdots & \alpha_{n1} \\
0 & \alpha_{22} & \cdots & \alpha_{n2} \\
\cdots & \cdots & \cdots & \cdots \\
0 & 0 & \cdots & \alpha_{nn}
\end{pmatrix}
$$

En outre, $U$ et $C$ dépendent continûment de $X$ d’après le lemme 10. D’autre part, la formule (8) montre que $C$ se met sous la forme $DT$ avec $D \in D^*_+$, $T \in T_1(n, K)$, $D$ et $T$ dépendant continûment de $C$. L’unicité de la décomposition $X = UDT$ résulte de la propriété d’unicité du lemme 10.

L’homéomorphisme de la prop. 7 s’appelle « décomposition d’Iwasawa » de $\mathbf{GL}(n, K)$.

Le groupe $G = D^*_+ . T_1(n, K)$ est l’ensemble des matrices triangulaires supérieures sur $K$ dont les éléments diagonaux sont $> 0$. Identifions l’élément $(z_{ij})$ de ce groupe à l’élément

$$
((z_{ii})_{1 \leqslant i \leqslant n}, (z_{ij})_{1 \leqslant i < j \leqslant n}) \in (\mathbf{R}_+^*)^n \times K^{n(n-1)/2}.
$$

Raisonnant exactement comme dans l’exemple 4, on trouve comme mesure de Haar à droite sur ce groupe

$$
\left( \prod_{i=1}^n z_{ii}^{-i} \right) \cdot \left( \bigotimes_{i=1}^n dz_{ii} \right) \otimes \left( \bigotimes_{i<j} dz_{ij} \right).
$$

Appliquant alors la prop. 13 du § 2, no 9, on voit que, si on identifie $\mathbf{GL}(n, K)$ à $\mathbf{U}(n, K) \times G$ par l’application $(U, S) \to US$, une mesure de Haar sur $\mathbf{GL}(n, K)$ est

$$
\left( \prod_{i=1}^n z_{ii}^{-i} \right) . \alpha \otimes \left( \bigotimes_{i=1}^n dz_{ii} \right) \otimes \left( \bigotimes_{i<j} dz_{ij} \right)
$$

$\alpha$ désignant une mesure de Haar sur $\mathbf{U}(n, K)$.

#### Exemple 8 {#int-vii-s3-n3-exa-8 .statement}

Espaces de formes hermitiennes.

Dans cet exemple, K désigne toujours l’un des corps $\mathbf{R}, \mathbf{C}, \mathbf{H}$. On posera $\delta = \dim_{\mathbf{R}} K$ (donc $\delta = 1, 2$ ou $4$). Une forme hermitienne sur l’espace vectoriel à droite $K^n$ s’écrit

$$
\Phi(x, y) = \Phi(x_1, \ldots, x_n, y_1, \ldots, y_n) = \sum_{i,j=1}^n \bar{x}_i h_{ij} y_j
$$

avec $h_{ij} = \overline{h_{ji}}$ quels que soient $i$ et $j$. Notons $\mathfrak{H}$ l’espace vectoriel sur $\mathbf{R}$ formé des matrices hermitiennes de $\mathbf{M}_n(K)$. L’application $(h_{ij}) \to \Phi$ est un isomorphisme de $\mathfrak{H}$ sur l’espace vectoriel des formes hermitiennes sur $K^n$, par lequel nous identifions ces deux espaces. Soit $\mathfrak{H}_+^* \subset \mathfrak{H}$ l’ensemble des formes hermitiennes positives non dégénérées sur $K^n$. L’ensemble $\mathfrak{H}_+^*$ est *convexe* dans $\mathfrak{H}$; en effet, si $\Phi_1, \Phi_2$ sont dans $\mathfrak{H}_+^*$ et si $\lambda, \mu$ sont deux nombres $> 0$ tels que $\lambda + \mu = 1$, il est clair que $\lambda \Phi_1 + \mu \Phi_2$ est une forme hermitienne positive ; d’autre part, si $(\lambda \Phi_1 + \mu \Phi_2)(x, x) = 0$, on a $\Phi_1(x, x) = \Phi_2(x, x) = 0$, donc $x = 0$, de sorte que $\lambda \Phi_1 + \mu \Phi_2$ est non dégénérée. Montrons maintenant que $\mathfrak{H}_+^*$ est une partie *ouverte* de $\mathfrak{H}$. Soit S l’ensemble des $x = (x_1, \ldots, x_n) \in K^n$ tels que $x_1 \bar{x}_1 + \ldots + x_n \bar{x}_n = 1$ ; c’est une partie compacte de $K^n$ ; si $\Phi \in \mathfrak{H}_+^*$, la fonction $x \to \Phi(x, x)$ est continue et $> 0$ sur S, et par suite sa borne inférieure est $> 0$ ; si $\Phi' \in \mathfrak{H}$ est suffisamment voisine de $\Phi$, on a donc $\Phi'(x, x) > 0$ pour tout $x \in S$, de sorte que $\Phi'$ est positive non dégénérée.

Le groupe linéaire $\mathbf{GL}(n, K)$ opère continûment à droite dans $\mathfrak{H}$ par $(X, \Phi) \to \Phi \circ X$, c’est-à-dire par $(X, H) \to {}^t \overline{X}.H.X$ si on note $H$ la matrice hermitienne correspondant à $\Phi$. Il est clair que $\mathfrak{H}_+^*$ est stable pour $\mathbf{GL}(n, K)$. Plus précisément, d’après *Alg.*, chap. IX, § 6, no 1, cor. 1 du th. 1, $\mathfrak{H}_+^*$ est l’orbite pour $\mathbf{GL}(n, K)$ de la forme $\sum_{i=1}^n \bar{x}_i y_i$ correspondant à la matrice unité $I_n$. Le stabilisateur de celle-ci est $\mathbf{U}(n, K)$. D’après le lemme de l’app. 2, $\mathfrak{H}_+^*$ s’identifie, comme espace homogène topologique, à $\mathbf{GL}(n, K)/\mathbf{U}(n, K)$.

Pour tout $X \in \mathbf{GL}(n, K)$, soit $\tilde{X}$ l’automorphisme

$$
H \to {}^t \overline{X}.H.X
$$

de l’espace vectoriel réel $\mathfrak{H}$. Si $\mu$ désigne la mesure de Haar du groupe additif $\mathfrak{H}$, on a $\widetilde{X}^{-1}(\mu) = |\det \widetilde{X}| \cdot \mu$ ($§ 1$, no 10, prop. 15). Montrons que

$$(15)$$
$$|\det \widetilde{X}| = |N(X)|^\lambda$$

où N désigne la norme dans $\mathbf{M}_n(K)$ considérée comme $\mathbf{R}$-algèbre, et où $\lambda = 1 - \frac{\delta - 2}{\delta n}$. Il suffit de vérifier (15) pour X parcourant un système de générateurs de $\mathbf{GL}(n, K)$, donc (Alg., chap. II, 3e éd., § 10, no 13) pour des X des types suivants :

a) X est la matrice d’une application de la forme

$$(x_1, \ldots, x_n) \to (x_{\sigma(1)}, \ldots, x_{\sigma(n)})$$

où $\sigma \in \mathcal{S}_n$. Dans ce cas, une puissance de X est égale à 1, donc $|\det \widetilde{X}| = |N(X)| = 1$.

b) X est la matrice d’une application de la forme

$$(x_1, x_2, \ldots, x_n) \to (ax_1, x_2, \ldots, x_n).$$

Alors, si $(h_{ij}) \in \mathfrak{H}$, on a $\widetilde{X}((h_{ij})) = (h'_{ij})$ avec $h'_{11} = \overline{a} h_{11} a$
$= |a|^2 h_{11}$, $h'_{1i} = \overline{a} h_{1i}$ pour $i > 1$, $h'_{ij} = h_{ij}$ pour $i > 1, j > 1$; donc

$$|\det \widetilde{X}| = |a|^2 |a|^{\delta(n-1)} = |a|^{2 + \delta(n-1)}.$$

D’autre part, si $Y = (y_{ij}) \in \mathbf{M}_n(K)$, on a $XY = (y'_{ij})$ avec $y'_{1j} = ay_{1j}$ et $y'_{ij} = y_{ij}$ pour $i > 1$; donc $|N(X)| = |a|^{\delta n}$. La formule (15) est encore vérifiée.

c) X est la matrice d’une application de la forme

$$(x_1, x_2, \ldots, x_n) \to (x_1 + bx_2, x_2, \ldots, x_n).$$

On a $\widetilde{X}((h_{ij})) = (h'_{ij})$ avec $h'_{11} = h_{11}$, $h'_{12} = h_{12} + h_{11} b$,
$h'_{1i} = h_{1i}$ pour $i > 2$, $h'_{22} = h_{22} + \overline{b} h_{12} + \overline{h}_{12} b + \overline{b} h_{11} b$,
$h'_{2i} = h_{2i} + \overline{b} h_{1i}$ pour $i > 2$, $h'_{ij} = h_{ij}$ pour $i > 2, j > 2$.
Compte tenu du lemme 6, on voit que $|\det \widetilde{X}| = 1$. On vérifie de même que $|N(\widetilde{X})| = 1$, ce qui achève de prouver la formule (15).

Ceci posé, la mesure $|\mathrm{N}(H)|^{-\lambda/2} d\mu(H)$ sur $\mathfrak{H}$ est invariante par $\mathbf{GL}(n, K)$, car

$$
\tilde{X}^{-1}(|\mathrm{N}(H)|^{-\lambda/2} d\mu(H)) = |\mathrm{N}(\tilde{X}(H))|^{-\lambda/2}.|\det \tilde{X}| d\mu(H)
$$
$$
= |\mathrm{N}(H)|^{-\lambda/2}|\mathrm{N}(X)|^{-\lambda}|\det \tilde{X}| d\mu(H) = |\mathrm{N}(H)|^{-\lambda/2} d\mu(H).
$$

Si $H \in \mathfrak{H}_+^*$, on a $H = \tilde{X}(I_n) = {}^t\overline{\tilde{X}} X$ pour un $X \in \mathbf{GL}(n, K)$, donc $\mathrm{N}(H) = \overline{\mathrm{N}(X)} \mathrm{N}(X) > 0$. Par suite, sur $\mathfrak{H}_+^*$, l’unique mesure invariante par $\mathbf{GL}(n, K)$ à un facteur constant près (cf. § 2, n° 6, th. 3) est la mesure

$$
d\gamma(H) = \mathrm{N}(H)^{-\lambda/2} d\mu(H).
$$

En particulier

$$
d\gamma(H) = (\det H)^{-(n+1)/2} d\mu(H) \quad \text{pour } K = \mathbf{R}
$$
$$
d\gamma(H) = (\det H)^{-n} d\mu(H) \quad \text{pour } K = \mathbf{C}.
$$

## EXERCICES {#int-vii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
