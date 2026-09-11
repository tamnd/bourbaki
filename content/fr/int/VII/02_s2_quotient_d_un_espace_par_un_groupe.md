---
book: int
book_title: Integration
chapter: VII
chapter_title: Mesure de Haar
section: 2
section_title: Quotient d'un espace par un groupe ; espaces homogènes
lang: fr
source: int-vii-viii-fr
pdf_pages: 0038-0069, 0110-0113
extraction: ocr
subsections:
    - "no": 1
      title: Résultats généraux.
      page: 0
      pdf_page: 38
    - "no": 2
      title: '*Cas où $\chi = 1$*.'
      page: 0
      pdf_page: 41
    - "no": 3
      title: '*Autre interprétation de $\lambda^\#$*.'
      page: 0
      pdf_page: 44
    - "no": 4
      title: Cas où $X/H$ est paracompact.
      page: 0
      pdf_page: 49
    - "no": 5
      title: Mesures quasi-invariantes sur un espace homogène.
      page: 0
      pdf_page: 52
    - "no": 6
      title: Mesures relativement invariantes sur un espace homogène.
      page: 0
      pdf_page: 57
    - "no": 7
      title: Mesure de Haar sur un groupe quotient.
      page: 0
      pdf_page: 59
    - "no": 8
      title: Une propriété de transitivité.
      page: 0
      pdf_page: 60
    - "no": 9
      title: Construction de la mesure de Haar d’un groupe à partir des mesures de Haar de certains sous-groupes.
      page: 0
      pdf_page: 64
    - "no": 10
      title: Intégration dans un domaine fondamental.
      page: 0
      pdf_page: 66
statements: 52
exercises: 13
content_sha256: 58e83c46193f68820de944214b0a2cb526001f5aaea4db3c9735ea3b49fdb0c2
---

## § 2. Quotient d’un espace par un groupe ; espaces homogènes.

### 1. Résultats généraux.

Soit X un espace localement compact dans lequel un groupe localement compact H opère à droite, continûment et proprement, par $(x, \xi) \to x\xi$ ($x \in X, \xi \in H$). La relation d’équivalence définie par H dans X est ouverte (Top. Gén., chap. III, 3e éd., § 2, no 4, lemme 2) et X/H est séparé (loc. cit., § 4, no 2, prop. 3) donc localement compact (Top. Gén., chap. I, 3e éd., § 10, no 4, prop. 10). On notera $\pi$ l’application canonique de X sur X/H. Le saturé d’une partie Y de X est $YH = \pi^{-1}(\pi(Y))$. Si K est une partie compacte de X, $\pi(K)$ est compact, et le saturé $\pi^{-1}(\pi(K))$ est fermé dans X. Toute partie compacte de X/H est l’image par $\pi$ d’une partie compacte de X (Top. Gén., chap. I, 3e éd., § 10, no 4, prop. 10). On suppose donnée une fois pour toutes une mesure de Haar à gauche $\beta$ sur H.

Soit $\chi$ une représentation continue de H dans $\mathbf{R}_+^*$. Si une fonction $g$ sur X satisfait à $g(x\xi) = \chi(\xi)g(x)$ quels que soient $x \in X$ et $\xi \in H$, son support S est invariant par H et s’écrit donc $\pi^{-1}(\pi(S))$. On désignera par $\mathscr{K}^\chi(X)$ l’espace de Riesz formé des fonctions numériques continues $g$ sur X qui satisfont à $g(x\xi) = \chi(\xi)g(x)$ ($x \in X, \xi \in H$), et dont le support est le saturé d’une partie compacte de X ; on notera $\mathscr{K}_+^\chi(X)$ l’ensemble des éléments $\geq 0$ de $\mathscr{K}^\chi(X)$. En particulier, $\mathscr{K}^1(X)$ n’est autre que l’ensemble des fonctions continues sur X, constantes sur les orbites, et dont le support est le saturé d’une partie compacte.

#### Proposition 1 {#int-vii-s2-prop-1 .statement}

Soit f une fonction numérique continue sur X dont le support S ait une intersection compacte avec le saturé de toute partie compacte de X.

a) Pour tout $x \in X$, la fonction $\xi \to f(x\xi)$ sur H appartient à $\mathscr{K}(H)$; on pose

$$
f^\chi(x) = \int_H f(x\xi)\chi(\xi)^{-1}d\beta(\xi).
$$

b) La fonction $f^\chi$ est continue, est nulle hors de SH, et satisfait à $f^\chi(x\xi) = \chi(\xi)f^\chi(x)$.

c) Si $g$ est une fonction numérique continue sur $X$ et satisfait à $g(x\xi) = \chi(\xi)g(x)$, on a $(f g)^\chi = f^1 g$ ($f^1$ étant donné par la formule (1) où on remplace $\chi$ par la représentation $\xi \to 1$ de $H$ dans $\mathbf{R}_+^*$).

d) Si $\eta \in H$, on a $(\delta(\eta)f)^\chi = \chi(\eta)\Delta_H(\eta)^{-1}f^\chi$.

Soient $x_0 \in X$ et $V$ un voisinage compact de $x_0$ dans $X$. L’ensemble des $\xi \in H$ tels que $V\xi$ rencontre $S$ est aussi l’ensemble des $\xi \in H$ tels que $V\xi$ rencontre $S \cap VH$, donc est compact dans $H$ puisque $S \cap VH$ est compact et que $H$ opère proprement dans $X$ (Top. Gén., chap. III, 3e éd., § 4, no 5, th. 1); alors le lemme 1 du § 1, no 1 prouve a) et la continuité de $f^\chi$. Le reste de b) est évident. Enfin c) et d) résultent des calculs suivants :

$$
(fg)^\chi(x) = \int_H f(x\xi)g(x\xi)\chi(\xi)^{-1}d\beta(\xi) = \int_H f(x\xi)g(x)\chi(\xi)\chi(\xi)^{-1}d\beta(\xi)
$$
$$
= g(x) \int_H f(x\xi)d\beta(\xi) = g(x)f^1(x)
$$
$$
(\delta(\eta)f)^\chi(x) = \int_H f(x\xi\eta)\chi(\xi)^{-1}d\beta(\xi)
$$
$$
= \Delta_H(\eta)^{-1} \int_H f(x\xi)\chi(\xi\eta^{-1})^{-1}d\beta(\xi)
$$
$$
= \chi(\eta)\Delta_H(\eta)^{-1} \int_H f(x\xi)\chi(\xi)^{-1}d\beta(\xi).
$$

#### Proposition 2 {#int-vii-s2-prop-2 .statement}

L’application $f \to f^\chi$ de $\mathcal{K}(X)$ dans $\mathcal{K}^\chi(X)$ est linéaire, et l’image de $\mathcal{K}(X)$ (resp. $\mathcal{K}_+(X)$) est $\mathcal{K}^\chi(X)$ (resp. $\mathcal{K}_+^\chi(X)$).

La linéarité est immédiate. Il est clair que $f^\chi \geqslant 0$ pour $f \geqslant 0$. Il suffit alors d’appliquer le lemme suivant :

#### Lemme 1 {#int-vii-s2-lem-1 .statement}

Soient $K$ une partie compacte de $X$, $u$ une fonction de $\mathcal{K}_+(X)$, avec $u(x) > 0$ pour $x \in K$. Soit $g \in \mathcal{K}^\chi(X)$ telle que $\operatorname{Supp} g \subset KH$.

a) On a $\inf_{x \in KH} u^1(x) > 0$.

b) La fonction h égale à $g/u^1$ dans KH, à 0 dans $X - KH$, appartient à $\mathcal{K}^\times(X)$.

c) $g = (uh)^\times$.

On a $u^1(x) > 0$ pour $x \in K$, donc $\inf_{x \in KH} u^1(x) = \inf_{x \in K} u^1(x) > 0$.

L’assertion b) en résulte aussitôt. Enfin, d’après la prop. 1 c), on a $(uh)^\times = u^1h$, et il est clair que $u^1h = g$.

Soit I une forme linéaire relativement bornée (chap. II, § 2, n° 2) sur $\mathcal{K}^\times(X)$. Alors $f \to I(f^\times)$ est une forme linéaire relativement bornée sur $\mathcal{K}(X)$, c’est-à-dire une mesure $\mu_I$ sur X. L’application $I \to \mu_I$ est injective d’après la prop. 2. Les mesures $\mu_I$ ainsi obtenues sur X peuvent être caractérisées comme suit :

#### Proposition 3 {#int-vii-s2-prop-3 .statement}

Soit $\mu$ une mesure sur X. Les conditions suivantes sont équivalentes :

a) Il existe une forme linéaire relativement bornée I sur $\mathcal{K}^\times(X)$ telle que $I(f^\times) = \mu(f)$ pour toute $f \in \mathcal{K}(X)$.

b) $\delta(\xi)\mu = \chi(\xi)^{-1}\Delta_H(\xi)\mu$ pour tout $\xi \in H$.

c) Quelles que soient $f, g$ dans $\mathcal{K}(X)$, on a

$$
\mu(f \cdot g^1) = \mu(f^\times \cdot g).
$$

d) Si $f \in \mathcal{K}(X)$ est telle que $f^\times = 0$, alors $\mu(f) = 0$.

$a) \Rightarrow b)$ : si $\mu(f) = I(f^\times)$, on a, compte tenu de la prop. 1 d) :

$$
\langle \delta(\xi)\mu, f \rangle = \langle \mu, \delta(\xi^{-1})f \rangle = I((\delta(\xi^{-1})f)^\times) = I(\chi(\xi)^{-1}\Delta_H(\xi)f^\times)
= \chi(\xi)^{-1}\Delta_H(\xi)\langle \mu, f \rangle,
$$

donc $\delta(\xi)\mu = \chi(\xi)^{-1}\Delta_H(\xi)\mu$.

$b) \Rightarrow c)$ : supposons l’hypothèse b) satisfaite. Observons que les fonctions $(x, \xi) \to f(x)g(x\xi)$ et $(x, \xi) \to f(x\xi)g(x)$ sur $X \times H$ sont continues à support compact (parce que H opère proprement dans X) ; ceci posé, le th. 2 du chap. III, § 5, n° 1 permet d’écrire :

$$
\int_X f(x) d\mu(x) \int_H g(x\xi) d\beta(\xi) = \int_H d\beta(\xi) \int_X f(x) g(x\xi) d\mu(x)
$$
$$
= \int_H d\beta(\xi) \int_X f(x\xi^{-1}) g(x) \chi(\xi) \Delta_H(\xi)^{-1} d\mu(x)
$$
$$
= \int_X g(x) d\mu(x) \int_H f(x\xi^{-1}) \chi(\xi) \Delta_H(\xi)^{-1} d\beta(\xi)
$$
$$
= \int_X g(x) d\mu(x) \int_H f(x\xi) \chi(\xi)^{-1} d\beta(\xi)
$$

ce qui prouve c).

c) $\Rightarrow$ d) : si c) est vérifiée et si $f^\chi = 0$, on a $\mu(f \cdot g^1) = 0$ pour toute $g \in \mathcal{K}(X)$, donc $\mu(f) = 0$ en choisissant $g \in \mathcal{K}(X)$ telle que $g^1 = 1$ sur Supp $f$ (ce qui est possible d'après la prop. 2 appliquée avec $\chi = 1$).

d) $\Rightarrow$ a) : si la condition d) est satisfaite, il existe une forme linéaire I sur $\mathcal{K}^\chi(X)$ telle que $\mu(f) = I(f^\chi)$ pour $f \in \mathcal{K}(X)$, et cette forme est relativement bornée en vertu de la prop. 2.

### 2. *Cas où $\chi = 1$*.

Si $f$ est une fonction sur $X/H$, $f \circ \pi$ est une fonction sur $X$ constante sur les orbites, continue si et seulement si $f$ est continue. L’application $f \to f \circ \pi$ définit en particulier une *bijection* de $\mathcal{K}(X/H)$ sur $\mathcal{K}^1(X)$.

Nous pouvons alors, dans le cas où $\chi = 1$, reformuler de la manière suivante certains résultats du no 1 :

Soit $f$ une fonction numérique continue dans $X$ dont le support ait une intersection compacte avec le saturé de toute partie compacte de $X$. La formule

(3)
$$
f^b(\pi(x)) = \int_H f(x\xi) d\beta(\xi)
$$

définit une fonction continue $f^b$ sur $X/H$. Si $g$ est une fonction continue sur $X/H$, on a

(4)
$$
(f \cdot g \circ \pi)^b = f^b \cdot g.
$$

Si $\eta \in H$, on a

(5) $$
(\delta(\eta)f)^b = \Delta_H(\eta)^{-1}f^b.
$$

On n’oubliera pas que la définition de $f^b$ dépend du choix de $\beta$. Si $H$ est compact et $\beta$ normalisée, la fonction $f^b$ s’appelle parfois moyenne orbitale de $f$.

Si $f \in \mathcal{K}(X)$, on a $f^b \in \mathcal{K}(X/H)$. L’application $f \to f^b$ de $\mathcal{K}(X)$ dans $\mathcal{K}(X/H)$ est linéaire, et l’image de $\mathcal{K}(X)$ (resp. $\mathcal{K}_+(X)$) est $\mathcal{K}(X/H)$ (resp. $\mathcal{K}_+(X/H)$).

#### Remarque 1 {#int-vii-s2-n2-rem-1 .statement}

On va montrer que l’application $f \to f^b$ est un morphisme strict (Top. gén., chap. III, 3e éd., § 2, n° 8) de $\mathcal{K}(X)$ sur $\mathcal{K}(X/H)$.

a) Cette application est continue : il suffit de prouver que, pour toute partie compacte $K$ de $X$, la restriction à $\mathcal{K}(X, K)$ de $f \to f^b$ est une application continue de $\mathcal{K}(X, K)$ dans $\mathcal{K}(X/H, \pi(K))$ (Esp. vect. top., chap. II, § 2, n° 2, cor. de la prop. 1) ; comme $H$ opère proprement dans $X$, l’ensemble $P$ des $\xi \in H$ tels que $K\xi$ rencontre $K$ est compact ; on conclut de (3) que $\sup_{x \in K} |f^b(\pi(x))| \leq \beta(P) \sup_{x \in K} |f(x)|$, et ceci prouve notre assertion.

b) Soit $K'$ une partie compacte de $X/H$. Choisissons une partie compacte $K$ de $X$ telle que $\pi(K) = K'$, et montrons que la restriction de $f \to f^b$ à $\mathcal{K}(X, K)$ est un morphisme strict de $\mathcal{K}(X, K)$ sur $\mathcal{K}(X/H, K')$. Il suffit de construire pour cette restriction un inverse à droite (Esp. vect. top., chap. I, § 1, n° 8, prop. 13). Or, d’après le lemme 1 du n° 1 (dont nous adoptons les notations), on obtient un tel inverse en composant les applications suivantes :

α) l’application $f' \to f' \circ \pi$ de $\mathcal{K}(X/H, K')$ dans l’ensemble $E$ des fonctions de $\mathcal{K}^1(X)$ dont le support est contenu dans $KH$ ;
β) l’application de $E$ dans $E$ qui, à toute $g \in E$, fait correspondre la fonction égale à $g/u^1$ dans $KH$, à 0 dans $X - KH$ ;
γ) l’application de $E$ dans $\mathcal{K}(X)$ qui, à toute fonction $h \in E$, fait correspondre $uh$.

c) Ceci posé, si $V$ est un voisinage convexe de 0 dans $\mathcal{K}(X)$, $V \cap \mathcal{K}(X, K)$ est un voisinage convexe de 0 dans $\mathcal{K}(X, K)$, donc $V^b \cap \mathcal{K}(X/H, K')$ est un voisinage convexe de 0 dans $\mathcal{K}(X/H, K')$ d’après b), donc $V^b$ est un voisinage de 0 dans $\mathcal{K}(X/H)$ (Esp. vect. top., chap. II, § 2, n° 4). Ceci achève la démonstration.

#### Proposition 4 {#int-vii-s2-prop-4 .statement}

a) Soit $\lambda$ une mesure sur $X/H$. Il existe une mesure $\lambda^\#$ et une seule sur $X$ telle que

(6) $$
\int_{X/H} f^b d\lambda = \int_X f d\lambda^\#
$$

quelle que soit $f \in \mathcal{K}(X)$. On a $\delta(\xi)\lambda^\# = \Delta_H(\xi)\lambda^\#$ pour tout $\xi \in H$.

b) Réciproquement, soit $\mu$ une mesure sur $X$ telle que $\delta(\xi)\mu = \Delta_H(\xi)\mu$ pour tout $\xi \in H$. Il existe une mesure $\lambda$ et une seule sur $X/H$ telle que $\mu = \lambda^\#$.

C'est un cas particulier du no 1.

#### Définition 1 {#int-vii-s2-def-1 .statement}

Les hypothèses et les notations étant celles de la prop. 4, $\lambda$ s'appelle le quotient de $\mu$ par $\beta$ et se note $\frac{\mu}{\beta}$ ou $\mu/\beta$.

L'application $\lambda \to \lambda^\#$ de $\mathcal{M}(X/H)$ dans $\mathcal{M}(X)$ n'est autre que la transposée de l'application $f \to f^b$ de $\mathcal{K}(X)$ dans $\mathcal{K}(X/H)$. Soit $\mathfrak{F}$ un filtre sur $\mathcal{M}(X/H)$; dire que $\lim_{\lambda,\mathfrak{F}} \lambda^\#(f) = 0$ pour toute $f \in \mathcal{K}(X)$ équivaut à dire que $\lim_{\lambda,\mathfrak{F}} \lambda(f') = 0$ pour toute $f' \in \mathcal{K}(X/H)$; l'application $\lambda \to \lambda^\#$ est donc, pour les topologies vagues, un isomorphisme de $\mathcal{M}(X/H)$ sur un sous-espace vectoriel de $\mathcal{M}(X)$. Ce sous-espace est vaguement fermé, puisqu'il est l'ensemble des $\mu \in \mathcal{M}(X)$ telles que $\delta(\xi)\mu = \Delta_H(\xi)\mu$ pour tout $\xi \in H$. Il est clair que les conditions $\lambda \geqslant 0$ et $\lambda^\# \geqslant 0$ sont équivalentes.

La formule (6) s'écrit, par analogie avec la notation usuelle pour les intégrales doubles

$$
\int_X f(x)d\lambda^\#(x) = \int_{X/H} d\lambda(\dot{x}) \int_H f(x\xi)d\beta(\xi) \quad (\dot{x} = \pi(x)).
$$

Il s'agit d'un abus de notations, l'intégrale $\int_H f(x\xi)d\beta(\xi)$ étant considérée comme fonction de $\dot{x}$ et non de $x$; cette manière d'écrire s'emploiera souvent par la suite quand elle ne pourra prêter à confusion.

#### Remarque 2 {#int-vii-s2-n2-rem-2 .statement}

Soit $E$ un espace vectoriel localement convexe et soit $m$ une mesure vectorielle sur $X/H$, à valeurs dans $E$. L'application $f \to m(f^b)$ de $\mathcal{K}(X)$ dans $E$ est alors une mesure vectorielle sur $X$, à valeurs dans $E$, que nous noterons encore $m^\#$. L'application $m \to m^\#$ est encore un isomorphisme de $\mathcal{L}(\mathcal{K}(X/H); E)$ sur un sous-espace vectoriel $A$ de $\mathcal{L}(\mathcal{K}(X); E)$ (si on munit ces espaces de la topologie de la convergence simple). De plus, comme l'application $f \to f^b$ est un morphisme strict surjectif, le sous-espace $A$ se compose exactement des mesures vectorielles $n$ sur $X$ qui sont nulles sur le noyau $N$ de l’application $f \to f^\flat$. Pour que $n \in A$, il est donc nécessaire et suffisant que les mesures scalaires $z' \circ n$ soient nulles sur $N$ pour tout $z' \in E'$. On déduit alors de la prop. 3 que $n \in A$ si et seulement si l’on a
$$
\delta(\xi)n = \Delta_H(\xi)n
$$
pour tout $\xi \in H$.

### 3. *Autre interprétation de $\lambda^\#$*.

Pour tout $x \in X$, l’application $\xi \to x\xi$ de $H$ dans $X$ est propre (*Top. Gén.*, chap. III, 3e éd., § 4, no 2, prop. 4), donc $\beta$ admet une mesure image dans $X$ par cette application, image qui est concentrée sur l’orbite $xH$ (chap. V, § 6, no 2, cor. 3 de la prop. 2); comme $\beta$ est invariante à gauche, cette mesure image ne dépend que de la classe $u = \pi(x)$ de $x$ dans $X/H$, et sera notée $\beta_u$. Par définition, pour $f \in \mathcal{K}(X)$, on a
$$
\int_X f(y)d\beta_u(y) = \int_H f(x\xi)d\beta(\xi) = f^\flat(u).
$$
On voit donc que
$$
(\varepsilon_u)^\# = \beta_u.
$$

#### Lemme 2 {#int-vii-s2-lem-2 .statement}

*Soit $f$ une fonction sur $X$, à valeurs dans un espace topologique.*
a) *Si $f$ est une fonction numérique $\geq 0$, on a, pour $x \in X$*
$$
\int_X^* f(y)d\beta_{\dot{x}}(y) = \int_H^* f(x\xi)d\beta(\xi) \quad (\dot{x} = \pi(x)).
$$
b) *Pour que $f$ soit $\beta_{\dot{x}}$-mesurable, il faut et il suffit que la fonction $\xi \to f(x\xi)$ sur $H$ soit $\beta$-mesurable.*
c) *Supposons que $\mathbf{f}$ soit une fonction sur $X$, à valeurs dans un espace de Banach ou dans $\mathbf{R}$; alors, pour que $\mathbf{f}$ soit $\beta_{\dot{x}}$-intégrable (resp. essentiellement $\beta_{\dot{x}}$-intégrable), il faut et il suffit que la fonction $\xi \to \mathbf{f}(x\xi)$ sur $H$ soit $\beta$-intégrable (resp. essentiellement $\beta$-intégrable), et on a alors*
$$
\int_X \mathbf{f}(y)d\beta_{\dot{x}}(y) = \int_H \mathbf{f}(x\xi)d\beta(\xi).
$$
Cela résulte du chap. V, § 4, prop. 2, prop. 3 et th. 2.

Puisque $f^b \in \mathcal{K}(X/H)$ pour $f \in \mathcal{K}(X)$, la formule (8) prouve que l’application $u \to \beta_u$ de $X/H$ dans $\mathcal{M}(X)$ est vaguement continue, que la famille $(\beta_u)$ est $\lambda$-adéquate quelle que soit la mesure positive $\lambda$ sur $X/H$, et que

$$
\lambda^* = \int_{X/H} \beta_u d\lambda(u)
$$

ce qui fournit une nouvelle interprétation de $\lambda^*$.

#### Proposition 5 {#int-vii-s2-prop-5 .statement}

*Soit $\lambda$ une mesure positive sur $X/H$.*

a) *Soit $f$ une fonction $\lambda^*$-mesurable sur $X$, à valeurs dans un espace topologique, constante hors d’une réunion dénombrable d’ensembles $\lambda^*$-intégrables. Alors, l’ensemble des $\dot{x} \in X/H$ tels que la fonction $\xi \to f(x\xi)$ ne soit pas $\beta$-mesurable est localement $\lambda$-négligeable.*

b) *Soit $f$ une fonction $\lambda^*$-mesurable $\geq 0$ sur $X$, nulle hors d’une réunion dénombrable d’ensembles $\lambda^*$-intégrables. Alors la fonction $\dot{x} \to \int^* f(x\xi)d\beta(\xi)$ sur $X/H$ est $\lambda$-mesurable, et l’on a*

$$
\int_X^* f(x)d\lambda^*(x) = \int_{X/H}^* d\lambda(\dot{x}) \int_H^* f(x\xi)d\beta(\xi) \qquad (\dot{x} = \pi(x)).
$$

c) *Soit $\mathbf{f}$ une fonction $\lambda^*$-intégrable sur $X$, à valeurs dans un espace de Banach ou dans $\mathbf{R}$. Alors l’ensemble des $\dot{x} \in X/H$ tels que $\xi \to \mathbf{f}(x\xi)$ ne soit pas $\beta$-intégrable est $\lambda$-négligeable ; la fonction $\mathbf{f}^b$ sur $X/H$ définie presque partout par la formule*

$$
\mathbf{f}^b(\dot{x}) = \int_H \mathbf{f}(x\xi)d\beta(\xi) \qquad (\dot{x} = \pi(x))
$$

est $\lambda$-intégrable, et l’on a

$$
\int_{X/H} |\mathbf{f}^b|d\lambda = \int_X |\mathbf{f}|d\lambda^*
$$

et

$$
\int_{X/H} |\mathbf{f}^b|d\lambda \leq \int_X |\mathbf{f}|d\lambda^*.
$$

d) Soit $f$ une fonction $\lambda^{\#}$-mesurable sur $X$, à valeurs dans un espace de Banach ou dans $\overline{\mathbf{R}}$, et nulle hors d'une réunion dénombrable d'ensembles $\lambda^{\#}$-intégrables. Alors, pour que $f$ soit $\lambda^{\#}$-intégrable, il faut et il suffit que

$$
\int_{X/H}^{*} d\lambda(\dot{x}) \int_{H}^{*} |f(x\xi)|\ d\beta(\xi) < +\infty \quad (\dot{x} = \pi(x)).
$$

Compte tenu du lemme 2, a), b), c) résultent du chap. V, § 3, prop. 3, prop. 4 et th. 1 (à l’exception de (13) qui résulte de (12), car il est clair que $|f^{\flat}| \leq |f|^{\flat}$) ; d) résulte de b).

#### Proposition 6 {#int-vii-s2-prop-6 .statement}

Soit $\lambda$ une mesure positive sur $X/H$.
a) Soit $N$ une partie de $X/H$. Pour que $N$ soit localement $\lambda$-négligeable, il faut et il suffit que $\pi^{-1}(N)$ soit localement $\lambda^{\#}$-négligeable.
b) Soit $g$ une fonction sur $X/H$, à valeurs dans un espace topologique. Pour que $g$ soit $\lambda$-mesurable, il faut et il suffit que $g \circ \pi$ soit $\lambda^{\#}$-mesurable.
c) Soit $h$ une fonction sur $X/H$ à valeurs dans un espace de Banach ou dans $\overline{\mathbf{R}}$. Pour que $h$ soit localement $\lambda$-intégrable, il faut et il suffit que $h \circ \pi$ soit localement $\lambda^{\#}$-intégrable, et l’on a alors $(h.\lambda)^{\#} = (h \circ \pi).\lambda^{\#}$.
Supposons $h \circ \pi$ localement $\lambda^{\#}$-intégrable. Pour toute $f \in \mathcal{K}(X)$, $f.(h \circ \pi)$ est $\lambda^{\#}$-intégrable, donc (prop. 5) la fonction $(f.(h \circ \pi))^{\flat} = f^{\flat}.h$ est $\lambda$-intégrable et l’on a

$$
\int_{X/H} f^{\flat}.h d\lambda = \int_{X} f.(h \circ \pi) d\lambda^{\#}.
$$

Comme $f \to f^{\flat}$ est une application surjective de $\mathcal{K}(X)$ sur $\mathcal{K}(X/H)$, cela montre que $h$ est localement $\lambda$-intégrable et que

$$
(h.\lambda)^{\#} = (h \circ \pi).\lambda^{\#}.
$$

En particulier, si $\pi^{-1}(N)$ est localement $\lambda^{\#}$-négligeable, $\varphi_N \circ \pi$ est localement $\lambda^{\#}$-négligeable, donc $(\varphi_N.\lambda)^{\#} = (\varphi_N \circ \pi).\lambda^{\#} = 0$, et par suite $\varphi_N.\lambda = 0$ et $N$ est localement $\lambda$-négligeable. Maintenant, supposons que $g \circ \pi$ soit $\lambda^{\#}$-mesurable. Soit $K'$ une partie compacte de X/H. Soit $f \in \mathcal{K}_+(X)$, telle que $f^\flat = 1$ dans $K'$ (no 1, prop. 2), et soit $K = \mathrm{Supp}\, f$; on a $\pi(K) \supset K'$. Il existe une partition de K formée d’un ensemble $\lambda^*$-négligeable M et d’une suite $(K_n)$ d’ensembles compacts tels que $(g \circ \pi)|K_n$ soit continue pour tout n. Alors $g|\pi(K_n)$ est continue. Soit P l’ensemble des points de K n’appartenant pas à $\pi(K_1) \cup \pi(K_2) \cup \ldots$; alors $\pi^{-1}(P) \cap K$ est contenu dans M, donc est $\lambda^*$-négligeable ; donc $f \cdot \varphi_{\pi^{-1}(P)}$ est $\lambda^*$-négligeable ; on en déduit (prop. 5)

$$
0 = \int_X f \cdot \varphi_{\pi^{-1}(P)} d\lambda^* = \int_{X/H} f^\flat \cdot \varphi_P d\lambda \geq \int_{X/H}^* \varphi_P d\lambda
$$

donc P est $\lambda$-négligeable, et g est $\lambda$-mesurable.

Si N est localement $\lambda$-négligeable, $\pi^{-1}(N)$ est localement $\lambda^*$-négligeable (App. 2). Si g est $\lambda$-mesurable, $g \circ \pi$ est $\lambda^*$-mesurable (ibid.). Enfin, supposons h localement $\lambda$-intégrable. Alors on sait déjà que $h \circ \pi$ est $\lambda^*$-mesurable. Pour toute $f \in \mathcal{K}_+(X)$, on a, d’après la prop. 5,

$$
\int_X^* f(x)|h|(\pi(x)) d\lambda^*(x) = \int_{X/H}^* |h|(u)f^\flat(u) d\lambda(u) < + \infty
$$

donc $h \circ \pi$ est localement $\lambda^*$-intégrable.

#### Corollaire 1 {#int-vii-s2-prop-6-cor-1 .statement}

Soient $\lambda, \lambda'$ deux mesures positives sur X/H. Pour que $\lambda'$ soit de base $\lambda$, il faut et il suffit que ${\lambda'}^*$ soit de base $\lambda^*$. Pour que $\lambda$ et $\lambda'$ soient équivalentes, il faut et il suffit que $\lambda^*$ et ${\lambda'}^*$ soient équivalentes.

La première assertion résulte de la prop. 6, a) et c). La deuxième résulte de la première.

#### Corollaire 2 {#int-vii-s2-prop-6-cor-2 .statement}

Soient $\lambda$ une mesure positive sur X/H, et f une fonction numérique $\lambda^*$-mesurable sur X. On suppose que, pour tout $\xi \in H$, on ait $\delta(\xi)f = f$ localement $\lambda^*$-presque partout. Alors il existe une fonction $\lambda$-mesurable g sur X/H telle que $f = g \circ \pi$ localement $\lambda^*$-presque partout.

En remplaçant f par $f/(1 + |f|)$, on se ramène au cas où f est bornée, donc localement $\lambda^*$-intégrable. Soit $\mu = f \cdot \lambda^*$. L’hypothèse sur f entraîne que $\delta(\xi)\mu = f \cdot \delta(\xi)\lambda^* = \Delta_H(\xi)\mu$ pour tout $\xi \in H$. Il existe alors (prop. 4) une mesure $\lambda'$ sur $X/H$ telle que $\mu = {\lambda'}^\#$. D’après le cor. 1, il existe une fonction localement $\lambda$-intégrable $g$ sur $X/H$ telle que $\lambda' = g.\lambda$. D’après la prop. 6, on a $f.\lambda^\# = {\lambda'}^\# = (g \circ \pi).\lambda^\#$, d’où $f = g \circ \pi$ localement $\lambda^\#$-presque partout.

#### Corollaire 3 {#int-vii-s2-prop-6-cor-3 .statement}

a) *Soit* $(\lambda_i)_{i \in I}$ *une famille de mesures réelles sur* $X/H$. *Pour que la famille* $(\lambda_i)$ *soit majorée dans* $\mathcal{M}(X/H)$, *il faut et il suffit que la famille* $(\lambda_i^\#)$ *soit majorée dans* $\mathcal{M}(X)$, *et on a alors*

$$
\sup(\lambda_i^\#) = (\sup \lambda_i)^\#.
$$

b) *Soit* $\lambda$ *une mesure réelle sur* $X/H$. *On a* $(\lambda^+)^{\#} = (\lambda^\#)^+$
*et* $(\lambda^-)^{\#} = (\lambda^\#)^-$.

c) *Soit* $\lambda$ *une mesure complexe sur* $X/H$. *On a* $|\lambda|^\# = |\lambda^\#|$.
Supposons la famille $(\lambda_i)$ majorée et posons $\mu = \sup \lambda_i$. Puisque $\lambda \geq 0$ entraîne $\lambda^\# \geq 0$, on a $\mu^\# \geq \lambda_i^\#$ pour tout $i$ ce qui montre que la famille $(\lambda_i^\#)$ est majorée et que

$$
(\sup \lambda_i)^\# \geq \sup(\lambda_i^\#).
$$

Réciproquement, supposons la famille $(\lambda_i^\#)$ majorée et soit $v = \sup (\lambda_i^\#)$. Puisque $\delta(\xi)\lambda_i^\# = \Delta_H(\xi)\lambda_i^\#$ pour tout $\xi \in H$, on a évidemment $\delta(\xi)v = \Delta_H(\xi)v$, donc il existe une mesure $\mu' \in \mathcal{M}(X/H)$ telle que $v = {\mu'}^\#$. Comme $\lambda^\# \geq 0$ entraîne $\lambda \geq 0$, on a $\mu' \geq \lambda_i$ pour tout $i$, ce qui montre que la famille $(\lambda_i)$ est majorée et que $v = {\mu'}^\# \geq (\sup \lambda_i)^\#$, d’où

$$
\sup (\lambda_i^\#) \geq (\sup \lambda_i)^\#
$$

ce qui achève la démonstration de a). L’assertion b) en résulte aussitôt, puisque $\lambda^+$ par exemple n’est autre que $\sup(\lambda, 0)$. Pour démontrer c), il suffit de remarquer que $|\lambda| = \sup \Re(\alpha \lambda)$ pour $\alpha$ nombre complexe de module 1, et d’autre part que $\Re(\mu^\#) = (\Re \mu)^\#$ pour toute $\mu \in \mathcal{M}(X/H)$.

#### Remarque 1 {#int-vii-s2-n3-rem-1 .statement}

La prop. 6 a) peut s’exprimer en disant que $\lambda$ est une mesure *pseudo-image* de $\lambda^\#$ par $\pi$ (chap. VI, § 3, no 2, déf. 1).

#### Remarque 2 {#int-vii-s2-n3-rem-2 .statement}

Supposons $H$ compact et $\beta$ normalisée. Le saturé de toute partie compacte de $X$ est compact. Donc, si $f \in \mathcal{K}(X/H)$, on a $f \circ \pi \in \mathcal{K}(X)$; et, pour toute mesure positive $\lambda$ sur $X/H$, la prop. 5c) donne

$$
\int_X (f \circ \pi)(x)d\lambda^*(x) = \int_{X/H} f(u)d\lambda(u).
$$

Autrement dit, $\lambda$ est l’image de $\lambda^*$ par $\pi$.

#### Remarque 3 {#int-vii-s2-n3-rem-3 .statement}

Le cor. 3 c) de la prop. 6 montre aussitôt que les résultats de ce n° restent valables dans le cas des mesures complexes (sauf ceux qui font intervenir l’intégrale supérieure).

#### Remarque 4 {#int-vii-s2-n3-rem-4 .statement}

Soit $m$ une mesure vectorielle sur $X/H$ à valeurs dans $E$ et soit $q$ une semi-norme semi-continue inférieurement sur $E$. Pour que $m$ soit $q$-majorable (chap. VI, § 2, n° 3, déf. 3), il faut et il suffit que $m^*$ le soit, et on a alors $q(m^*) = q(m)^*$. Ceci résulte aussitôt des définitions et du cor. 3 a).

Soit d’autre part $\mu$ une mesure positive sur $X/H$. Pour que $m$ soit scalairement de base $\mu$, il faut et il suffit que $m^*$ soit scalairement de base $\mu^*$ : cela résulte du cor. 1.

Enfin, si $m$ est de base $\mu$, de densité $f$ par rapport à $\mu$ (chap. VI, § 2, n° 4, déf. 4), alors $m^*$ est de base $\mu^*$, de densité $f \circ \pi$ : cela résulte de la prop. 6 c).

### 4. Cas où $X/H$ est paracompact.

Si $X/H$ est paracompact, on va voir d’abord que les espaces vectoriels $\mathcal{K}^\chi(X)$, pour $\chi$ variable, sont tous isomorphes entre eux, et en particulier isomorphes à $\mathcal{K}^1(X)$.

#### Proposition 7 {#int-vii-s2-prop-7 .statement}

Supposons $X/H$ paracompact. Soit $\chi$ une représentation continue de $H$ dans $\mathbf{R}_+^*$.

a) Il existe sur $X$ une fonction continue $r$, à valeurs $> 0$, telle que $r(x\xi) = \chi(\xi)r(x)$ quels que soient $x \in X$ et $\xi \in H$.

b) L’application $g \to g/r$ est un isomorphisme de l’espace vectoriel $\mathcal{K}^\chi(X)$ sur l’espace vectoriel $\mathcal{K}^1(X)$.

Appliquons la prop. 1 du n° 1 en prenant pour $f$ une fonction $\geqslant 0$ non identiquement nulle sur chaque orbite (c’est possible d’après le lemme 1 de l’Appendice 1) ; alors $r = f^\chi$ vérifie les propriétés de $a$. L’assertion $b$ est évidente.

#### Proposition 8 {#int-vii-s2-prop-8 .statement}

Supposons $X/H$ paracompact. Il existe une fonction $h \geq 0$ continue dans $X$, dont le support a une intersection compacte avec le saturé de toute partie compacte de $X$, et telle que $h^b = 1$. Pour une telle fonction, on a $g = (h . (g \circ \pi))^b$ quelle que soit la fonction $g$ continue dans $X/H$.

Appliquons la prop. 1 du n° 1, avec $\chi = 1$, en prenant pour $f$ une fonction $\geq 0$ non identiquement nulle sur chaque orbite. On a $f^1(x) > 0$ en tout point $x$ de $X$. Posons $h = f/f^1$. Alors $h^1 = f^1/f^1 = 1$, donc $h^b = 1$. Si $g$ est une fonction continue sur $X/H$, on a donc $(h . (g \circ \pi))^b = h^b . g = g$.

#### Remarque 1 {#int-vii-s2-n4-rem-1 .statement}

En particulier, soit $X$ un espace localement compact sur lequel opère à droite, continûment et proprement, un groupe discret $D$; supposons $X/D$ paracompact. Alors il existe sur $X$ une fonction continue $h \geq 0$, dont le support a une intersection compacte avec le saturé de toute partie compacte de $X$, et telle que $\sum_{d \in D} h(xd) = 1$ pour tout $x \in X$ (tous les termes de la somme étant nuls sauf un nombre fini d'entre eux).

#### Remarque 2 {#int-vii-s2-n4-rem-2 .statement}

Conservons les hypothèses et les notations de la prop. 8. L’application $g \to h . (g \circ \pi)$ est une application continue de $\mathcal{K}(X/H)$ dans $\mathcal{K}(X)$ qui est inverse à droite de l’application $f \to f^b$. Par suite, toute partie bornée (resp. compacte) de $\mathcal{K}(X/H)$ est l’image d’une partie bornée (resp. compacte) de $\mathcal{K}(X)$. On en déduit aussitôt que l’application $\lambda \to \lambda^\#$ est encore un isomorphisme de $\mathcal{M}(X/H)$ sur un sous-espace vectoriel fermé de $\mathcal{M}(X)$ quand on munit ces espaces de la topologie de la convergence bornée (resp. compacte).

#### Proposition 9 {#int-vii-s2-prop-9 .statement}

On conserve les hypothèses et les notations de la prop. 8. Soit $\lambda$ une mesure positive sur $X/H$.

a) Le couple $(\pi, h)$ est $\lambda^\#$-adapté, et $\int_X h(x) \varepsilon_{\pi(x)} d\lambda^\#(x) = \lambda$.

b) L’application $\pi$ est propre pour la mesure $h . \lambda^\#$, et $\pi(h . \lambda^\#) = \lambda$.

c) Soit $k$ une fonction sur $X/H$, à valeurs dans un espace de Banach ou dans $\overline{\mathbf{R}}$. Pour que $\mathbf{k}$ soit mesurable (resp. localement intégrable, essentiellement intégrable, intégrable) pour $\lambda$, il faut et il suffit que $h . (\mathbf{k} \circ \pi)$ le soit pour $\lambda^*$; et, si $\mathbf{k}$ est essentiellement intégrable pour $\lambda$, on a

$$
\int_{X/H} \mathbf{k} d\lambda = \int_X h . (\mathbf{k} \circ \pi) d\lambda^*.
$$

Soit $f \in \mathcal{K}(X/H)$. Alors $h . (f \circ \pi) \in \mathcal{K}(X)$ et l’on a

$$
\int_X h(x)f(\pi(x)) d\lambda^*(x) = \int_{X/H} f(\dot{x}) d\lambda(\dot{x}) \int_H h(x\xi) d\beta(\xi) = \int_{X/H} f(\dot{x}) d\lambda(\dot{x})
$$

d’où a). L’assertion b) se démontre de même. Les assertions de c) concernant la mesurabilité, l’intégrabilité essentielle et la formule (14) s’obtiennent alors en appliquant les résultats du chap. V (§ 4, prop. 3, § 5, prop. 4, § 4, th. 2). Si $\mathbf{k}$ est $\lambda$-intégrable, $h . (\mathbf{k} \circ \pi)$ est $\lambda^*$-intégrable (chap. V, § 3, n° 4, th. 1). Si $h . (\mathbf{k} \circ \pi)$ est $\lambda^*$-intégrable, la prop. 5 prouve que $(h . (\mathbf{k} \circ \pi))^b = h^b . \mathbf{k} = \mathbf{k}$ est $\lambda$-intégrable. Si $\mathbf{k}$ est localement $\lambda$-intégrable, $h . (\mathbf{k} \circ \pi)$ est localement $\lambda^*$-intégrable (prop. 6). Enfin, supposons $h . (\mathbf{k} \circ \pi)$ localement $\lambda^*$-intégrable; pour toute $f \in \mathcal{K}(X/H)$, $h . (\mathbf{k} \circ \pi) . (f \circ \pi)$ est à support compact, et

$$
|h . (\mathbf{k} \circ \pi) . (f \circ \pi)| \leq M |h . (\mathbf{k} \circ \pi)|
$$

en posant $M = \sup |f|$; donc $h . ((\mathbf{k}f) \circ \pi)$ est $\lambda^*$-intégrable, et par suite $\mathbf{k}f$ est $\lambda$-intégrable d’après ce qu’on a déjà démontré; ceci prouve bien que $\mathbf{k}$ est localement $\lambda$-intégrable.

#### Corollaire {#int-vii-s2-n4-cor-1 .statement}

*L’application linéaire continue* $f \to f^b$ de $L^1(X, \lambda^*)$ *dans* $L^1(X/H, \lambda)$ *définie par la prop. 5 est surjective*.

Supposons d’abord $X/H$ paracompact et soit $h$ une fonction sur $X$ satisfaisant aux conditions de la prop. 8. Si $k$ est une fonction numérique essentiellement $\lambda$-intégrable, $h . (k \circ \pi)$ est essentiellement $\lambda^*$-intégrable, et évidemment $(h . (k \circ \pi))^b = k$.

Dans le cas général, soit $u \in L^1(X/H, \lambda)$. Il existe une fonction $f \in \mathcal{L}^1(X/H, \lambda)$, de classe $u$ et nulle en dehors d’une réunion dénombrable d’ensembles compacts $K_n$. Définissons par récurrence une suite d’ensembles ouverts relativement compacts $U_n$ de $X/H$, tels que $U_{n+1} \supset K_n \cup \overline{U}_n$, et soit $V$ la réunion des $U_n$. Alors $V$ est une partie ouverte de $X/H$, réunion dénombrable de parties compactes $\overline{U}_n$, donc paracompacte (*Top. gén.*, chap. I, 3e éd., § 9, no 10, th. 5). Posons $Y = \pi^{-1}(V)$ et soit $\lambda_V$ (resp. $\lambda_Y^\#$) la mesure induite par $\lambda$ (resp. $\lambda^\#$) sur $V$ (resp. $Y$). Il est clair que $Y/H$ s’identifie à $V$ (*Top. gén.*, chap. I, 3e éd., § 3, prop. 10) et que $\lambda_Y^\#$ s’identifie à $(\lambda_V)^\#$. De plus, $f$ est nulle en dehors de $V$ et appartient à $\mathcal{L}^1(V, \lambda_V)$. Il existe donc $g \in \mathcal{L}^1(Y, \lambda_Y^\#)$ telle que $g^b = f$ presque partout sur $V$. En prolongeant $g$ par 0 sur $X - Y$, on obtient une fonction $g_1 \in \mathcal{L}^1(X, \lambda^\#)$ et il est clair que la classe de $g_1^b$ dans $L^1(X/H, \lambda)$ n’est autre que $u$.

#### Remarque 3 {#int-vii-s2-n4-rem-3 .statement}

Supposons $X/H$ paracompact et gardons les notations de la proposition 9. L’application $k \to h(k \circ \pi)$ de $L^1(X/H, \lambda)$ dans $L^1(X, \lambda^\#)$ est alors *isométrique* d’après (14) et est *inverse à droite* de l’application $f \to f^b$ de $L^1(X, \lambda^\#)$ sur $L^1(X/H, \lambda)$.

### 5. Mesures quasi-invariantes sur un espace homogène.

#### Lemme 3 {#int-vii-s2-lem-3 .statement}

Soient $G$ un groupe *localement compact*, $\mu$ une mesure de Haar à gauche sur $G$, $\nu$ et $\nu'$ deux mesures non nulles *quasi-invariantes* sur $G$. Si, pour tout $s \in G$, les densités de $\gamma(s)\nu$ par rapport à $\nu$ et de $\gamma(s)\nu'$ par rapport à $\nu'$ sont égales localement $\mu$-presque partout, $\nu$ et $\nu'$ sont *proportionnelles*.

Ecrivons $\nu = \rho . \mu$, $\nu' = \rho' . \mu$ où $\rho, \rho'$ sont des fonctions localement $\mu$-intégrables sur $G$ et partout non nulles ($§ 1$, no 9, prop. 11). Pour tout $s \in G$, on a

$$
\gamma(s)\nu = (\gamma(s)\rho) . \mu, \qquad \gamma(s)\nu' = (\gamma(s)\rho') . \mu,
$$

et l’hypothèse entraîne que $\rho^{-1} . \gamma(s)\rho = {\rho'}^{-1} . \gamma(s)\rho'$ localement $\mu$-presque partout. Posons $\sigma = \rho'/\rho$, qui est une fonction $\mu$-mesurable sur $G$. Pour tout $s \in G$, on a $\gamma(s)\sigma = \sigma$ localement $\mu$-presque partout. Donc $\sigma$ est égale à une constante localement μ-presque partout, d’après le cor. 2 de la prop. 6 appliqué avec X = H = G.

Soient G un groupe localement compact, H un sous-groupe fermé de G. Considérons l’espace homogène G/H des classes à gauche suivant H, sur lequel G opère continûment à gauche. Nous allons montrer qu’il existe une classe et une seule de mesures quasi-invariantes non nulles sur G/H.

Remarquons que H opère sur G continûment et proprement par translations à droite ; et l’espace quotient, qui n’est autre que G/H, est paracompact (Top. Gén., chap. III, 3e éd., § 4, no 6, prop. 13). On peut ainsi appliquer les résultats des nos 1 à 4, avec X = G. On a donc des applications $f \to f^b$ de $\mathcal{K}(G)$ sur $\mathcal{K}(G/H)$, et $\lambda \to \lambda^\#$ de $\mathcal{M}(G/H)$ dans $\mathcal{M}(G)$ (une fois fixée une mesure de Haar à gauche $\beta$ dans H). Le fait que G opère à gauche dans G/H donne lieu à une propriété supplémentaire :

$$
(15)\quad \gamma_{G/H}(s) \cdot f^b = (\gamma_G(s) \cdot f)^b \quad (s \in G,\ f \in \mathcal{K}(G))
$$
$$
(16)\quad (\gamma_{G/H}(s) \cdot \lambda)^\# = \gamma_G(s) \cdot \lambda^\# \quad (s \in G,\ \lambda \in \mathcal{M}(G/H)).
$$

En effet, pour tout $x \in G$, on a
$$
(\gamma_{G/H}(s) \cdot f^b)(\pi(x)) = f^b(s^{-1}\pi(x)) = f^b(\pi(s^{-1}x))
$$
$$
= \int_H f(s^{-1}x\xi)d\beta(\xi) = \int_H (\gamma_G(s)f)(x\xi)d\beta(\xi) = (\gamma_G(s)f)^b(\pi(x))
$$
d’où la formule (15), qui entraîne la formule (16).

#### Lemme 4 {#int-vii-s2-lem-4 .statement}

*Soient $\lambda$ une mesure $\neq 0$ sur $G/H$ et $\mu$ une mesure de Haar à gauche sur $G$. Les propriétés suivantes sont équivalentes :*

a) $\lambda$ est quasi-invariante par $G$ ;
b) pour qu’une partie $A$ de $G/H$ soit localement $\lambda$-négligeable, il faut et il suffit que $\pi^{-1}(A)$ soit localement $\mu$-négligeable ;
c) la mesure $\lambda^\#$ est équivalente à $\mu$.

Supposons qu’il en soit ainsi, et soit $\lambda^\# = \rho \cdot \mu$, $\rho$ étant une fonction localement $\mu$-intégrable partout non nulle. Alors, pour tout $s \in G$, la densité $\theta_s$ de $\gamma_{G/H}(s)\lambda$ par rapport à $\lambda$ est telle que

$$
\theta_s(\pi(x)) = \frac{\rho(s^{-1}x)}{\rho(x)}
$$

localement $\mu$-presque partout sur $G$.

c) $\Rightarrow$ b) : cela résulte aussitôt de la prop. 6 a).

b) $\Rightarrow$ a) : si la propriété b) est vérifiée, l’ensemble des parties de $G/H$ localement $\lambda$-négligeables est invariant par $G$, donc $\lambda$ est quasi-invariante par $G$.

a) $\Rightarrow$ c) : supposons $\lambda$ quasi-invariante par $G$; pour tout $s \in G$, $\lambda$ et $\gamma_{G/H}(s)\lambda$ sont équivalentes, donc $\lambda^\#$ et

$$
\gamma_G(s) \cdot \lambda^\# = (\gamma_{G/H}(s) \cdot \lambda)^\#
$$

sont équivalentes (cor. 1 de la prop. 6) ; comme $\lambda^\# \neq 0$, $\lambda^\#$ est équivalente à $\mu$ (§ 1, no 9, prop. 11).

En outre, pour tout $s \in G$, on a

$$
(\theta_s \circ \pi) \cdot \lambda^\# = (\theta_s \cdot \lambda)^\# = (\gamma_{G/H}(s)\lambda)^\# = \gamma_G(s)\lambda^\#
$$
$$
= (\gamma_G(s)\rho) \cdot \mu = \frac{\gamma_G(s)\rho}{\rho} \cdot \lambda^\#
$$

d’où (17).

L’équivalence de a) et b) entraîne d’abord le résultat d’unicité déjà annoncé, et même un résultat plus précis :

#### Théorème 1 {#int-vii-s2-thm-1 .statement}

Soient $G$ un groupe localement compact, $H$ un sous-groupe fermé de $G$.

a) Deux mesures quasi-invariantes non nulles sur $G/H$ sont équivalentes ; les parties de $G/H$ localement négligeables pour ces mesures sont celles dont l’image réciproque dans $G$ sont localement négligeables pour une mesure de Haar.

b) Soient $\lambda, \lambda'$ deux mesures quasi-invariantes non nulles sur $G/H$. Si, pour tout $s \in G$, les densités de $\gamma_{G/H}(s)\lambda$ par rapport à $\lambda$ et de $\gamma_{G/H}(s)\lambda'$ par rapport à $\lambda'$ sont égales localement presque partout pour $\lambda$ (ou $\lambda'$), $\lambda$ et $\lambda'$ sont proportionnelles.

a) résulte aussitôt du lemme 4. Soient $\lambda$ et $\lambda'$ deux mesures quasi-invariantes non nulles vérifiant la condition de b). Alors, pour tout $s \in G$, les densités de $\gamma_G(s)\lambda^\#$ par rapport à $\lambda^\#$ et de $\gamma_G(s)\lambda'^\#$ par rapport à $\lambda'^\#$ sont égales localement μ-presque partout, donc (lemme 3) $\lambda^\#$ et $\lambda'^\#$ sont proportionnelles, donc λ et λ' sont proportionnelles.

D'autre part, le lemme 4 ramène la recherche des mesures quasi-invariantes non nulles sur G/H à celle des mesures sur G équivalentes à la mesure de Haar et de la forme $\lambda^\#$. On a à ce sujet le lemme suivant :

#### Lemme 5 {#int-vii-s2-lem-5 .statement}

Soient μ une mesure de Haar à gauche sur G, et ρ une fonction localement μ-intégrable. Pour que ρ.μ soit de la forme $\lambda^\#$, il faut et il suffit que, pour tout ξ ∈ H, on ait

$$
\rho(x\xi) = \frac{\Delta_H(\xi)}{\Delta_G(\xi)} \rho(x)
$$

localement μ-presque partout sur G.

Dire que ρ.μ est de la forme $\lambda^\#$ revient à dire que, pour tout ξ ∈ H, on a δ(ξ)(ρ.μ) = Δ_H(ξ)ρ.μ (prop. 4). Or

$$
δ(ξ)(ρ.μ) = (δ(ξ)ρ) . (δ(ξ)μ) = Δ_G(ξ)(δ(ξ)ρ) . μ,
$$

d'où le lemme.

Nous pouvons maintenant établir le résultat d'existence annoncé, et même un résultat plus précis :

#### Théorème 2 {#int-vii-s2-thm-2 .statement}

Soient G un groupe localement compact, H un sous-groupe fermé de G, μ une mesure de Haar à gauche sur G, β une mesure de Haar à gauche sur H.

a) Il existe des fonctions ρ continues > 0 sur G telles que

$$
ρ(x\xi) = \frac{\Delta_H(\xi)}{\Delta_G(\xi)} ρ(x) \text{ quels que soient } x ∈ G \text{ et } ξ ∈ H.
$$

b) Etant donnée une telle fonction ρ, on peut former la mesure λ = (ρ.μ)/β sur G/H, et λ est une mesure positive non nulle quasi-invariante par G.

c) Pour s, x dans G, ρ(sx)/ρ(x) ne dépend que de s et π(x), donc définit une fonction χ continue > 0 sur G × (G/H) telle que

$$
χ(s, π(x)) = \frac{ρ(sx)}{ρ(x)}.
$$

Alors on a

(20) $\gamma_{G/H}(s)\lambda = \chi(s^{-1}, .) \cdot \lambda$ pour tout $s \in G$.

a) résulte de la prop. 7.
b) résulte des lemmes 5 et 4.
c) résulte de (17).

#### Remarque 1 {#int-vii-s2-n5-rem-1 .statement}

On déduit de la remarque 1 du n° 3 que les mesures quasi-invariantes non nulles sur $G/H$ ne sont autres que les mesures pseudo-images par $\pi$ d'une mesure de Haar sur $G$.

#### Remarque 2 {#int-vii-s2-n5-rem-2 .statement}

Si $G$ est un groupe de Lie, nous verrons plus tard qu'on peut choisir la fonction $\rho$ du th. 2 indéfiniment différentiable.*

Dans les conditions du th. 2, certains résultats des n°s 3 et 4 se spécialisent ainsi (compte tenu du chap. V, § 4, th. 2 et prop. 2 pour passer des propriétés relatives à $\mu$ aux propriétés relatives à $\rho \cdot \mu$):

a) Soit $f$ une fonction $\mu$-mesurable sur $G$, à valeurs dans un espace topologique, constante hors d'une réunion dénombrable d'ensembles $\mu$-intégrables ; alors l'ensemble des $\dot{x} \in G/H$ tels que la fonction $\xi \to f(x\xi)$ ne soit pas $\beta$-mesurable est localement $\lambda$-négligeable.

b) Soit $f$ une fonction $\mu$-mesurable $\geqslant 0$ sur $G$, nulle hors d'une réunion dénombrable d'ensembles $\mu$-intégrables. Alors la fonction $\dot{x} \to \int_H^* f(x\xi)d\beta(\xi)$ sur $G/H$ est $\lambda$-mesurable et on a
$$
\int_G^* f(x)\rho(x)d\mu(x) = \int_{G/H}^* d\lambda(\dot{x}) \int_H^* f(x\xi)d\beta(\xi) \quad (\dot{x} = \pi(x)).
$$

c) Soit $\mathbf{f}$ une fonction $\mu$-intégrable sur $G$, à valeurs dans un espace de Banach ou dans $\overline{\mathbf{R}}$. Alors l'ensemble des $\dot{x} \in G/H$ tels que $\xi \to \mathbf{f}(x\xi)$ ne soit pas $\beta$-intégrable est $\lambda$-négligeable ; la fonction $\dot{x} \to \int_H \mathbf{f}(x\xi)d\beta(\xi)$ est $\lambda$-intégrable, et
$$
\int_G \mathbf{f}(x)\rho(x)d\mu(x) = \int_{G/H} d\lambda(\dot{x}) \int_H \mathbf{f}(x)\xi d\beta(\xi).
$$

d) Il existe sur $G$ une fonction continue $h \geqslant 0$, dont le support a une intersection compacte avec le saturé KH de toute partie compacte K de G, et telle que $\int_{\mathbf{H}} h(x\xi)d\beta(\xi) = 1$ pour tout $x \in G$. Pour qu'une fonction $g$ sur $G/H$ soit mesurable (resp. localement intégrable, essentiellement intégrable, intégrable) pour $\lambda$, il faut et il suffit que $h . (g \circ \pi)$ le soit pour $\mu$; et, quand $g$ est essentiellement intégrable pour $\lambda$, on a

$$
\int_{G/H} g(u)d\lambda(u) = \int_G h(x)g(\pi(x))\rho(x)d\mu(x).
$$

### 6. Mesures relativement invariantes sur un espace homogène.

Soient toujours G un groupe localement compact, H un sous-groupe fermé, $\beta$ une mesure de Haar à gauche sur H.

#### Lemme 6 {#int-vii-s2-lem-6 .statement}

Soient $\lambda$ une mesure sur $G/H$, $\chi$ une représentation continue de G dans $\mathbf{C}^*$. Les propriétés suivantes sont équivalentes :

a) $\lambda$ est relativement invariante sur $G/H$ de multiplicateur $\chi$;
b) $\lambda^*$ est relativement invariante sur G de multiplicateur à gauche $\chi$;
c) $\lambda^*$ est de la forme $a\chi.\mu$ ($a \in \mathbf{C}$).

La condition a) signifie que, pour tout $s \in G$, on a

$$
\gamma_{G/H}(s)\lambda = \chi(s)^{-1}\lambda ;
$$

ceci équivaut à $(\gamma_{G/H}(s)\lambda)^* = \chi(s)^{-1}\lambda^*$, c'est-à-dire à

$$
\gamma_G(s)\lambda^* = \chi(s)^{-1}\lambda^* .
$$

D'où l'équivalence de a) et b). L'équivalence de b) et c) résulte du § 1, no 8, cor. 1 de la prop. 10.

#### Théorème 3 {#int-vii-s2-thm-3 .statement}

Soient G un groupe localement compact, H un sous-groupe fermé de G, $\mu$ (resp. $\beta$) une mesure de Haar à gauche sur G (resp. H), $\chi$ une représentation continue de G dans $\mathbf{C}^*$.

a) Pour qu'il existe sur $G/H$ une mesure non nulle relativement invariante par G et de multiplicateur $\chi$, il faut et il suffit que $\chi(\xi) = \Delta_H(\xi)/\Delta_G(\xi)$ pour tout $\xi \in H$.

b) Cette mesure est alors unique à un facteur constant près ; plus précisément, elle est proportionnelle à $(\chi \cdot \mu)/\beta$.

Pour qu’il existe sur $G/H$ une mesure non nulle relativement invariante par $G$ de multiplicateur $\chi$, il faut et il suffit (lemme 6) que $\chi \cdot \mu$ soit de la forme $\lambda^*$, donc (n° 2, prop. 4) que $\delta(\xi)(\chi \cdot \mu) = \Delta_H(\xi)(\chi \cdot \mu)$ pour tout $\xi \in H$. Cette condition s’écrit aussi $\chi(\xi)\chi \cdot \Delta_G(\xi)\mu = \Delta_H(\xi)\chi \cdot \mu$, c’est-à-dire

$$
\chi(\xi) = \Delta_H(\xi)/\Delta_G(\xi),
$$

pour tout $\xi \in H$. D’où a). L’assertion b) résulte aussitôt du lemme 6 et du fait que l’application $\lambda \to \lambda^*$ est injective.

On verra au § 3 (n° 3, exemple 4) des exemples très simples où la représentation $\xi \to \Delta_H(\xi)/\Delta_G(\xi)$ ne se prolonge pas en une représentation continue de $G$ dans $\mathbf{C}^*$. Dans ce cas, il n’existe donc aucune mesure complexe non nulle sur $G/H$ relativement invariante par $G$.

#### Corollaire 1 {#int-vii-s2-thm-3-cor-1 .statement}

Pour qu’il existe sur $G/H$ une mesure positive non nulle relativement invariante par $G$, il faut et il suffit qu’il existe une représentation continue de $G$ dans $\mathbf{R}_+^*$ prolongeant la représentation $\xi \to \Delta_H(\xi)/\Delta_G(\xi)$.

On notera que cette condition est remplie lorsque $H$ est unimodulaire.

#### Corollaire 2 {#int-vii-s2-thm-3-cor-2 .statement}

Pour qu’il existe sur $G/H$ une mesure positive non nulle invariante par $G$, il faut et il suffit que $\Delta_G$ coïncide avec $\Delta_H$ sur $H$.

#### Corollaire 3 {#int-vii-s2-thm-3-cor-3 .statement}

On suppose que $H$ est unimodulaire et qu’il existe sur $G/H$ une mesure positive bornée non nulle $\nu$ relativement invariante par $G$. Alors $\nu$ est invariante, et $G$ est unimodulaire.

Soit $\chi$ le multiplicateur de $\nu$. Pour tout $s \in G$, $\nu$ et $\gamma(s)\nu$ ont même masse totale finie (§ 1, n° 1, formule (6)) ; comme $\gamma(s)\nu = \chi(s)^{-1}\nu$, on a $\chi(s) = 1$. Donc $\nu$ est invariante. D’après le cor. 2, $\Delta_G(s) = 1$ pour tout $s \in H$. Soit $G'$ l’ensemble des $t \in G$ tels que $\Delta_G(t) = 1$. C’est un sous-groupe fermé distingué de $G$ contenant $H$. Soit $\pi$ l’application canonique de $G/H$ sur

G/G'. Alors $\pi(v)$ est une mesure positive bornée non nulle invariante par G. Donc la mesure de Haar à gauche du groupe G/G, est bornée, de sorte que G/G' est compact ($§ 1, \mathrm{n}^{\circ} 2, \mathrm{prop.}\ 2$). Par suite l'image de G par $\Delta_G$ est un sous-groupe compact de $\mathbf{R}_+^*$; ce sous-groupe est réduit à $\{1\}$, donc $\Delta_G = 1$ sur tout G.

### 7. Mesure de Haar sur un groupe quotient.

#### Proposition 10 {#int-vii-s2-prop-10 .statement}

Soient G un groupe localement compact, G' un sous-groupe distingué fermé, G'' le groupe G/G', $\pi$ l'application canonique de G sur G/G', $\alpha, \alpha', \alpha''$ des mesures de Haar à gauche sur G, G', G''.

a) En multipliant au besoin $\alpha$ par un facteur constant, on a $\alpha'' = \alpha / \alpha'$. En particulier, si $f \in \mathcal{K}(G)$,

$$
\int_G f(x)d\alpha(x) = \int_{G''} d\alpha''(\dot{x}) \int_{G'} f(x\xi)d\alpha'(\xi) \qquad (\dot{x} = \pi(x)).
$$

b) On a $\Delta_G(\xi) = \Delta_{G'}(\xi)$ pour tout $\xi \in G'$; en particulier, si G est unimodulaire, G' l'est aussi.

c) Le noyau de la représentation $\Delta_G$ de G dans $\mathbf{R}_+^*$ est le plus grand sous-groupe distingué fermé unimodulaire de G.

En appliquant le th. 3 du n° 6 avec $\chi = 1$ (et sachant qu'ici il existe une mesure sur G/G' invariante par G, à savoir $\alpha''$), on obtient a) et b); c) résulte aussitôt de b).

#### Proposition 11 {#int-vii-s2-prop-11 .statement}

On conserve les notations de la prop. 10. Soit u un automorphisme de G tel que $u(G') = G'$. Soient $u'$ la restriction de u à G', et $u''$ l'automorphisme de G'' déduit de u par passage aux quotients. Alors

$$
\operatorname{mod}_G(u) = \operatorname{mod}_{G'}(u') \operatorname{mod}_{G''}(u'').
$$

En effet, si $\alpha'' = \alpha / \alpha'$, on a $u''(\alpha'') = u(\alpha) / u'(\alpha')$, c'est-à-dire

$$
\operatorname{mod}_{G''}(u'')^{-1} \alpha'' = \operatorname{mod}_G(u)^{-1} \alpha / \operatorname{mod}_{G'}(u')^{-1} \alpha' = \frac{\operatorname{mod}_{G'}(u')}{\operatorname{mod}_G(u)} (\alpha / \alpha')
$$
$$
= \frac{\operatorname{mod}_{G'}(u')}{\operatorname{mod}_G(u)} \alpha'',
$$
d'où la proposition.

#### Corollaire {#int-vii-s2-n7-cor-1 .statement}

Pour tout $x \in G$, on a

$$
\Delta_G(x) = \Delta_{G/G'}(\dot{x}) \operatorname{mod}(i_x)
$$

en désignant par $\dot{x}$ l’image canonique de $x$ dans $G/G'$ et par $i_x$ l’automorphisme $s \to x^{-1}sx$ de $G'$.

Ceci résulte de la prop. 11, et de la formule (33) du § 1, no 4.

### 8. Une propriété de transitivité.

Soit $X$ un espace localement compact dans lequel un groupe localement compact $H$ opère à droite, continûment et proprement, par $(x, \xi) \to x\xi$ ($x \in X, \xi \in H$). Soit $H'$ un sous-groupe fermé de $H$; alors $H'$ opère à droite, continûment et proprement, dans $X$. Nous noterons $\pi, \pi', p$ les applications canoniques de $X$ sur $X/H$, de $X$ sur $X/H'$, et de $H$ sur $H/H'$.

Soient $\beta, \beta'$ des mesures de Haar à gauche sur $H, H'$; on suppose que $\Delta_H$ et $\Delta_{H'}$ coïncident sur $H'$; on peut donc former la mesure $\beta/\beta'$ sur $H/H'$, invariante à gauche par $H$ (no 6, th. 3). Soit d’autre part $\mu$ une mesure positive sur $X$ telle que

$$
\delta(\xi)\mu = \Delta_H(\xi)\mu
$$

pour $\xi \in H$; on peut donc former les mesures $\mu/\beta$ sur $X/H$ et $\mu/\beta'$ sur $X/H'$ (no 2, prop. 4). Nous allons écrire $\mu/\beta'$ comme l’intégrale, par rapport à $\mu/\beta$, d’une famille de mesures sur $X/H'$ indexées par les points de $X/H$. Lorsque $H' = \{e\}$, on retrouvera la situation du no 3.

L’application $(x, \xi) \to \pi'(x\xi)$ de $X \times H$ dans $X/H'$ est continue; comme $\pi'(x\xi) = \pi'(x\xi\xi')$ pour tout $\xi' \in H'$, cette application définit par passage au quotient une application continue de $X \times (H/H')$ dans $X/H'$; d’où, pour chaque $x$ fixé dans $X$, une application partielle $\omega_x$ de $H/H'$ dans $X/H'$, déduite par passage au quotient de l’application $\psi_x : \xi \to x\xi$ de $H$ dans $X$. Notons que $\psi_{x\xi} = \psi_x \circ \gamma_H(\xi)$, donc que $\omega_{x\xi} = \omega_x \circ \gamma_{H/H'}(\xi)$ pour tout $\xi \in H$.

#### Lemme 7 {#int-vii-s2-lem-7 .statement}

*Soient K une partie compacte de $X/H'$, et L une partie compacte de $X$. Alors* $\bigcup_{x \in L} \omega_x^{-1}(K)$ *est relativement compact dans $H/H'$.*

Soit $K_1$ une partie compacte de $X$ telle que $\pi'(K_1) = K$. Soit $K_2$ l’ensemble des $\xi \in H$ tels que $L\xi$ rencontre $K_1$. Alors $K_2$ est compact (*Top. Gén.*, chap. III, 3e éd., § 4, no 5, th. 1).

Soit $\xi \in H$ tel que $p(\xi) \in \bigcup_{x \in L} \omega_x^{-1}(K)$. Il existe donc un $x \in L$ tel que $\omega_x(p(\xi)) \in K$, autrement dit tel que $\pi'(x\xi) \in K$. Puisque $\pi'(K_1) = K$, il existe $\xi' \in H'$ tel que $x\xi\xi' \in K_1$. Alors $\xi\xi' \in K_2$, donc $p(\xi) = p(\xi\xi') \in p(K_2)$. On a ainsi montré que $\bigcup_{x \in L} \omega_x^{-1}(K) \subset p(K_2)$.

Ce lemme montre d’abord que l’application $\omega_x$ est *propre*. On peut donc former la mesure $\omega_x(\beta/\beta')$ sur $X/H'$, qui est concentrée sur $\omega_x(H/H') = \pi'(\psi_x(H)) = \pi'(xH)$. Si $f \in \mathcal{K}(X/H')$, le lemme 7, et le § 1, no 1, lemme 1 montrent que la fonction $x \to \langle f, \omega_x(\beta/\beta') \rangle$ est continue dans $X$; en outre, $\langle f, \omega_x(\beta/\beta') \rangle$ est nul quand Supp $f$ ne rencontre pas $\pi'(xH)$, autrement dit quand $\pi(x)$ n’appartient pas à l’image canonique de Supp $f$ dans $X/H$.

Par ailleurs, si $\xi \in H$, on a

$$
\omega_{x\xi}(\beta/\beta') = \omega_x(\gamma_{H/H'}(\xi)(\beta/\beta')) = \omega_x(\beta/\beta').
$$

L’application $x \to \omega_x(\beta/\beta')$ de $X$ dans $\mathcal{M}(X/H')$ définit donc par passage au quotient une application $u \to (\beta/\beta')_u$ de $X/H$ dans $\mathcal{M}(X/H')$. Ce qui précède montre que, pour toute $f \in \mathcal{K}(X/H')$, l’application $u \to \langle f, (\beta/\beta')_u \rangle$ est continue à support compact. Par suite, l’application $u \to (\beta/\beta')_u$ *est une famille vaguement continue et* $(\mu/\beta)$*-adéquate de mesures sur* $X/H'$, *l’ensemble d’indices étant* $X/H$.

Soient $x \in X$, et $u = \pi(x) \in X/H$. Soit $f$ une fonction sur $X/H'$, à valeurs dans un espace de Banach ou dans $\overline{\mathbf{R}}$. D’après le chap. V, § 4, th. 2, pour que $f$ soit $(\beta/\beta')_u$-intégrable, il faut et il suffit que la fonction $p(\xi) \to f(\omega_x(p(\xi))) = f(\pi'(x\xi))$ sur $H/H'$ soit $(\beta/\beta')$-intégrable, et l’on a alors

$$
(21)\quad \int_{X/H'} f(u') d(\beta/\beta')_u(u') = \int_{H/H'} f(\pi'(x\xi)) d(\beta/\beta')(\dot{\xi}) \quad (\dot{\xi} = p(\xi)).
$$

On a des propriétés analogues pour la mesurabilité, l’intégrale supérieure et l’intégrale essentielle.

**Proposition 12. — On a**

$$
(22)\quad \int_{X/H} (\beta/\beta')_u d(\mu/\beta)(u) = \mu/\beta'.
$$

Soit $f \in \mathcal{K}(X)$, et soit $f^b \in \mathcal{K}(X/H')$, définie par

$$
f^b(\pi'(x)) = \int_{H'} f(x\xi') d\beta'(\xi').
$$

Il suffit de prouver (cf. n° 2) que $f^b$ a même intégrale par rapport aux deux membres de (22). Or, $\langle \mu/\beta', f^b \rangle = \langle \mu, f \rangle$. D’autre part,

$$
\left\langle \int_{X/H} (\beta/\beta')_u d(\mu/\beta)(u), f^b \right\rangle = \int_{X/H} \langle (\beta/\beta')_u, f^b \rangle d(\mu/\beta)(u).
$$

Or, soient $x \in X$ et $u = \pi(x)$. On a

$$
\langle (\beta/\beta')_u, f^b \rangle = \langle \omega_x(\beta/\beta'), f^b \rangle = \int_{H/H'} f^b(\omega_x(\dot{\xi})) d(\beta/\beta')(\dot{\xi})
$$
$$
= \int_{H/H'} f^b(\pi'(x\xi)) d(\beta/\beta')(\dot{\xi})
$$
$$
= \int_{H/H'} d(\beta/\beta')(\dot{\xi}) \int_{H'} f(x\xi\xi') d\beta'(\xi')
$$
$$
= \int_H f(x\xi) d\beta(\xi).
$$

Donc

$$
\left\langle \int_{X/H} (\beta/\beta')_u d(\mu/\beta)(u), f^\flat \right\rangle = \int_{X/H} d(\mu/\beta)(u) \int_H f(x\xi) d\beta(\xi) = \langle \mu, f \rangle
$$

ce qui prouve la proposition.

#### Corollaire 1 {#int-vii-s2-lem-7-cor-1 .statement}

a) Soit $\mathbf{f}$ une fonction sur $X/H'$, à valeurs dans un espace de Banach ou dans $\overline{\mathbf{R}}$, intégrable pour $\mu/\beta'$. Il existe une partie $(\mu/\beta)$-négligeable $N$ de $X/H$ ayant la propriété suivante : si $x \in X$ est tel que $\pi(x) \notin N$, la fonction $\mathbf{f} \circ \omega_x$ sur $H/H'$, c'est-à-dire la fonction $\dot{\xi} \to \mathbf{f}(\pi'(x\xi))$, est intégrable pour $\beta/\beta'$; l'intégrale $\int_{H/H'} \mathbf{f}(\pi'(x\xi)) d(\beta/\beta')(\dot{\xi})$ ne dépend que de $\dot{x} = \pi(x)$, et est une fonction $(\mu/\beta)$-intégrable de $\dot{x}$; et l'on a

$$
\int_{X/H'} \mathbf{f} d(\mu/\beta') = \int_{X/H} d(\mu/\beta)(\dot{x}) \int_{H/H'} \mathbf{f}(\pi'(x\xi)) d(\beta/\beta')(\dot{\xi}).
$$

b) Soit $f$ une fonction $\geqslant 0$ sur $X/H'$, mesurable pour $\mu/\beta'$ et nulle hors d'une réunion dénombrable d'ensembles $(\mu/\beta')$-intégrables. Alors $\pi(x) \to \int_{H/H'}^* f(\pi'(x\xi)) d(\beta/\beta')(\dot{\xi})$ est $(\mu/\beta)$-mesurable, et l'on a

$$
\int_{X/H'}^* f d(\mu/\beta') = \int_{X/H}^* d(\mu/\beta)(\dot{x}) \int_{H/H'}^* f(\pi'(x\xi)) d(\beta/\beta')(\dot{\xi}).
$$

c) Soit $\mathbf{f}$ une fonction sur $X/H'$ à valeurs dans un espace de Banach ou dans $\overline{\mathbf{R}}$, mesurable pour $\mu/\beta'$ et nulle hors d'une réunion dénombrable d'ensembles $(\mu/\beta')$-intégrables. Alors, pour que $\mathbf{f}$ soit $(\mu/\beta')$-intégrable, il suffit que

$$
\int_{X/H}^* d(\mu/\beta)(\dot{x}) \int_{H/H'}^* |\mathbf{f}(\pi'(x\xi))| d(\beta/\beta')(\dot{\xi}) < +\infty.
$$

#### Corollaire 2 {#int-vii-s2-lem-7-cor-2 .statement}

Soient $G$ un groupe localement compact, $A$ et $B$ des sous-groupes fermés de $G$ tels que $A \supset B$. On suppose qu'il existe, sur l'espace homogène $G/B$ des classes à gauche suivant $B$, une mesure positive non nulle $\alpha$ invariante par $G$ et bornée.

a) L’image canonique de $\alpha$ dans $G/A$ est une mesure positive non nulle, invariante par $G$, et bornée.

b) $\Delta_G$ coïncide avec $\Delta_A$ sur $A$ et avec $\Delta_B$ sur $B$.

c) Il existe, sur l’espace homogène $A/B$ des classes à gauche de $A$ suivant $B$, une mesure positive non nulle invariante par $A$ et bornée.

L’assertion a) est immédiate. L’assertion b) résulte de a) et du no 6, cor. 2 du th. 3. D’après b), $\Delta_A$ coïncide avec $\Delta_B$ sur $B$, et on peut donc appliquer les résultats du présent numéro en y faisant $X = G, H = A, H' = B$. La fonction 1 sur $G/B$ est $\alpha$-intégrable. D’après le a) du cor. 1, la fonction 1 sur $A/B$ est intégrable pour $\beta/\beta', \beta$ et $\beta'$ désignant des mesures de Haar à gauche de $A$ et $B$; donc $\beta/\beta'$ est bornée.

### 9. Construction de la mesure de Haar d’un groupe à partir des mesures de Haar de certains sous-groupes.

Soient $G$ un groupe localement compact, $X$ et $Y$ deux sous-groupes fermés de $G$ tels que $\Omega = XY$ contienne un voisinage $U$ de $e$. Alors $\Omega$ est ouvert dans $G$; car, quels que soient $x_0 \in X$ et $y_0 \in Y$, on a $XY = (x_0X)(Yy_0) \supset x_0Uy_0$, et $x_0Uy_0$ est un voisinage de $x_0y_0$; donc $\Omega$ est un voisinage de chacun de ses points.

*Lorsque $G$ est un groupe de Lie d’algèbre de Lie $g$, la condition imposée à $X$ et $Y$ est satisfaite si les sous-algèbres correspondant à $X$ et $Y$ ont pour somme $g$.*

Le groupe $X \times Y$ opère continûment à gauche dans $G$ par la loi $(x, y).s = xsy^{-1}$ ($x \in X, y \in Y, s \in G$). Soit $Z = X \cap Y$. Le stabilisateur de $e$ dans $X \times Y$ est le sous-groupe $Z_0$ de $X \times Y$ formé des couples $(z, z)$, où $z \in Z$, sous-groupe qui est canoniquement isomorphe à $Z$. Donc l’ensemble $\Omega$ s’identifie à l’espace homogène des classes à gauche $(X \times Y)/Z_0$; plus précisément, l’application $(x, y) \to xy^{-1}$ de $X \times Y$ sur $\Omega$ définit par passage au quotient une bijection continue de $(X \times Y)/Z_0$ sur $\Omega$. Nous supposerons que cette application est un homéo-morphisme. (Il en est ainsi notamment si G est dénombrable à l'infini : cf. App. 1).

#### Proposition 13 {#int-vii-s2-prop-13 .statement}

Supposons en outre Z compact. Soient $\mu_G, \mu_X, \mu_Y$ des mesures de Haar à gauche sur G, X, Y, et $\Lambda$ la restriction de $\Delta_G$ à Y. Alors la restriction $\mu$ de $\mu_G$ à $\Omega$ est, à un facteur constant près, l'image de $\mu_X \otimes (\Lambda^{-1} \cdot \mu_Y)$ par l'application $(x, y) \to xy^{-1}$ de $X \times Y$ sur $\Omega$ (application qui est propre).
Pour $x \in X, \ y \in Y$, on a
$$
\gamma((x, y))\mu = \delta(y)\gamma(x)\mu = \Delta_G(y)\mu.
$$
Identifiant $\Omega$ à l'espace homogène $(X \times Y)/Z_0$ et choisissant une mesure de Haar convenable sur $Z_0$, on voit que $\mu^\#$ est le produit de la mesure de Haar à gauche de $X \times Y$, à savoir $\mu_X \otimes \mu_Y$, par la fonction $(x, y) \to \Delta_G(y)^{-1}$ (n° 6, lemme 6). D'autre part, $\mu$ est, à un facteur constant près, l'image de $\mu^\#$ par l'application canonique de $X \times Y$ sur $\Omega$ (n° 3, Remarque 2).

#### Corollaire {#int-vii-s2-n9-cor-1 .statement}

Soit $f$ une fonction définie dans $\Omega$, à valeurs dans un espace de Banach ou dans $\overline{\mathbf{R}}$. Pour que $f$ soit $\mu$-intégrable, il faut et il suffit que la fonction $(x, y) \to f(xy)\Delta_G(y)\Delta_Y(y)^{-1}$ soit $(\mu_X \otimes \mu_Y)$-intégrable ; on a alors
$$
(23) \quad \int_{\Omega} f(\omega)d\mu(\omega) = a \iint_{X \times Y} f(xy)\Delta_G(y)\Delta_Y(y)^{-1}d\mu_X(x)d\mu_Y(y),
$$
où $a$ est une constante $> 0$ indépendante de $f$.
D'après la prop. 13, et le chap. V, § 4, n° 4, th. 2, pour que $f$ soit $\mu$-intégrable, il faut et il suffit que la fonction $(x, y) \to f(xy^{-1})$ soit intégrable pour $\mu_X \otimes (\Lambda^{-1} \cdot \mu_Y)$, ou encore que la fonction $(x, y) \to f(xy^{-1})\Delta_G(y)^{-1}$ soit intégrable pour $\mu_X \otimes \mu_Y$, ou encore que la fonction $(x, y) \to f(xy)\Delta_G(y)\Delta_Y(y)^{-1}$ soit intégrable pour $\mu_X \otimes \mu_Y$. La formule (23) résulte d'un raisonnement analogue.

#### Proposition 14 {#int-vii-s2-prop-14 .statement}

Supposons que les conditions de la prop. 13 soient remplies et en outre que Y soit distingué.
a) La restriction de $\mu_G$ à $\Omega$ est, à un facteur constant près, l'image de $\mu_X \otimes \mu_Y$ par l'application $(x, y) \to xy$ de $X \times Y$ sur $\Omega$.

b) On a, pour $x \in X$ et $y \in Y$,

$$
\Delta_G(xy) = \Delta_X(x)\Delta_Y(y)\mathrm{mod}\,(i_x)
$$

en désignant par $i_x$ l’automorphisme $v \to x^{-1}vx$ de $Y$.

On a $\Delta_G = \Delta_Y$ sur $Y$ (prop. 10 b)), donc a) résulte de (23). Soient $x_0 \in X,\ y_0 \in Y$. Notons $p$ l’application $(x, y) \to xy$ de $X \times Y$ sur $\Omega$. Comme

$$
xy(x_0y_0)^{-1} = xx_0^{-1}(x_0yy_0^{-1}x_0^{-1}) = xx_0^{-1}i_{x_0^{-1}}(yy_0^{-1}),
$$

on a

$$
\Delta_G(x_0y_0)p(\mu_X \otimes \mu_Y) = \delta(x_0y_0)p(\mu_X \otimes \mu_Y)
$$
$$
= p(\delta(x_0)\mu_X \otimes i_{x_0^{-1}}\delta(y_0)\mu_Y) = p(\Delta_X(x_0)\mu_X \otimes \Delta_Y(y_0)(\mathrm{mod}\, i_{x_0})\mu_Y)
$$
$$
= \Delta_X(x_0)\Delta_Y(y_0)(\mathrm{mod}\, i_{x_0})p(\mu_X \otimes \mu_Y)
$$

d’où b).

#### Remarque {#int-vii-s2-n9-rem-1 .statement}

La prop. 14 s’applique en particulier quand G est produit semi-direct topologique de X par Y (Top. Gén., chap. III, 3e éd., § 2, n° 10). Dans ce cas, $Z = \{e\}$ et $\Omega = G$. Comme $yx = xi_x(y)$ pour $x \in X,\ y \in Y$, $\mu_G$ est aussi, à un facteur constant près, l’image de $(\mathrm{mod}\, i_x)\mu_X \otimes \mu_Y$ par l’application $(x, y) \to yx$ de $X \times Y$ dans G.

### 10. Intégration dans un domaine fondamental.

Soient X un espace localement compact, H un groupe discret opérant à droite continûment et proprement dans X. Soit $\pi$ l’application canonique de X sur X/H. Pour tout $x \in X$, on notera $H_x$ le stabilisateur de $x$ dans H ; c’est un sous-groupe fini de H (Top. gén., chap. III, 3e éd., § 4, n° 2, prop. 4) ; on notera $n(x)$ son ordre. Pour tout $s \in H$, on a $H_{xs} = s^{-1}H_x s$, donc $n(xs) = n(x)$. Il existe un voisinage ouvert U de $x$ tel que $U \cap Us = \varnothing$ pour $s \notin H_x$ (loc. cit., n° 4, démonstration de la prop. 8) ; pour $y \in U$, on a $H_y \subset H_x$ ; donc la fonction $n$ sur X est semi-continue supérieurement. Lorsque X est dénombrable à l’infini, H est dénombrable ; en effet, soit $(K_1, K_2, \ldots)$ un recouvrement de X par une suite de parties compactes, et soit x_0 \in X ; l'ensemble des s \in H tels que sx_0 \in K_i est fini (loc. cit., n° 5, th. 1), d'où notre assertion.

#### Définition 2 {#int-vii-s2-def-2 .statement}

Soit F \subset X. On dit que F est un domaine fondamental (pour H) si la restriction de \pi à F est une bijection de F sur X/H (autrement dit si F est un système de représentants pour la relation d'équivalence définie par H).

#### Lemme 8 {#int-vii-s2-lem-8 .statement}

Soit F un domaine fondamental. Pour tout x \in X, on a

$$
\sum_{s \in H} \varphi_{F_s}(x) = n(x).
$$

Comme \varphi_{F_s}(xt) = \varphi_{F_{st^{-1}}}(x) quels que soient s et t dans H, les deux membres de (24) restent invariants quand on remplace x par xt. On peut donc supposer que x \in F. Alors on a les équivalences

$$
\varphi_{F_s}(x) = 1 \Leftrightarrow x \in Fs \Leftrightarrow xs^{-1} \in F \Leftrightarrow xs^{-1} = x \Leftrightarrow s \in H_x
$$

d'où (24).

#### Proposition 15 {#int-vii-s2-prop-15 .statement}

On suppose X dénombrable à l'infini. Soit \mu une mesure \geqslant 0 sur X. Soit F un domaine fondamental tel que Fs soit \mu-mesurable pour tout s \in H. Soit f une fonction \mu-intégrable sur X, à valeurs dans un espace de Banach ou dans \mathbf{R}. Alors la famille des \int_{Fs} n(x)^{-1}f(x)d\mu(x) (s \in H) est sommable, et l'on a

$$
\int_X f(x)d\mu(x) = \sum_{s \in H} \int_{Fs} n(x)^{-1}f(x)d\mu(x).
$$

Si A est une partie finie de H, on a

$$
\left| \sum_{s \in A} n^{-1}f \varphi_{F_s} \right| \leq n^{-1} |f| \sum_{s \in A} \varphi_{F_s} \leq |f|
$$

d'après le lemme 8. Le lemme 8 prouve aussi que \sum_{s \in A} n^{-1}f \varphi_{F_s} converge simplement vers f suivant l'ensemble filtrant croissant

#### Théorème 4 {#int-vii-s2-thm-4 .statement}

Soient X un espace localement compact dénombrable à l'infini, H un groupe discret opérant à droite continûment et proprement dans X, π l'application canonique de X sur X/H, μ une mesure positive sur X invariante par H, β la mesure de Haar normalisée de H, et λ = μ/β. Soit F un domaine fondamental μ-mesurable.

a) Le couple (π, n^{-1}φ_F) est μ-adapté, et

$$
\int_X n(x)^{-1} φ_F(x) ε_{π(x)} dμ(x) = λ.
$$

b) L'application π est propre pour n^{-1}φ_F · μ, et π(n^{-1}φ_F · μ) = λ.

c) Soit k une fonction sur X/H. Pour que k soit λ-mesurable (resp. λ-intégrable), il faut et il suffit que n^{-1}φ_F(k ∘ π) soit μ-mesurable (resp. μ-intégrable); et, si k est λ-intégrable, on a

$$
\int_{X/H} k dλ = \int_F n^{-1}(k ∘ π) dμ.
$$

On a μ = λ#. Soit f ∈ 𝒦_+(X/H). Alors n^{-1}φ_F(f ∘ π) est μ-mesurable ≥ 0, et l'on a d'après la prop. 5 b) du no 3

$$
\int_X^* n(x)^{-1} φ_F(x)f(π(x)) dμ(x) = \int_{X/H}^* f(\dot{x}) dλ(\dot{x}) \int_H^* n(xξ)^{-1} φ_F(xξ) dβ(ξ)
$$

et $\int_H^* n(xξ)^{-1} φ_F(xξ) dβ(ξ) = n(x)^{-1} \sum_{ξ ∈ H} φ_F(xξ) = 1$ d'après le lemme 8. Donc $n^{-1}φ_F.(f ∘ π)$ est μ-intégrable et

$$
\int_X n(x)^{-1} φ_F(x)f(π(x)) dμ(x) = \int_{X/H} f(\dot{x}) dλ(\dot{x})
$$

Ceci prouve a). L'assertion b) se démontre de même. L'assertion c) se déduit de b) et du chap. V, § 4, prop. 3 et th. 2.

#### Corollaire {#int-vii-s2-n10-cor-1 .statement}

On conserve les hypothèses et les notations du th. 4. Soit F' un second domaine fondamental μ-mesurable.

Soit $u$ une fonction sur $X$, à valeurs dans un espace de Banach ou dans $\overline{\mathbf{R}}$, invariante par $H$. On suppose que $u$ est $\mu$-intégrable dans $F$. Alors, $u$ est $\mu$-intégrable dans $F'$, et

$$
\int_F u(x)d\mu(x) = \int_{F'} u(x)d\mu(x).
$$

Comme $u$ et $n$ sont invariantes par $H$, il existe une fonction $v$ sur $X/H$ telle que $v \circ \pi$ coïncide avec $nu$ sur $F$ et sur $F'$. Alors $n^{-1}\varphi_F(v \circ \pi) = \varphi_F u$, $n^{-1}\varphi_{F'}(v \circ \pi) = \varphi_{F'} u$. D’après l’hypothèse $n^{-1}\varphi_F(v \circ \pi)$ est $\mu$-intégrable. D’après le th. 4, $v$ est $\lambda$-intégrable, $\varphi_{F'} u$ est $\mu$-intégrable, et l’on a

$$
\int_F u d\mu = \int_{X/H} v d\lambda = \int_{F'} u d\mu.
$$

Pour l’existence de domaines fondamentaux $\mu$-mesurables, cf. exerc. 13.

## EXERCICES {#int-vii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
