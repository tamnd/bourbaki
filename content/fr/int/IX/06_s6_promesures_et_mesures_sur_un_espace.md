---
book: int
book_title: Integration
chapter: IX
chapter_title: MESURES SUR LES ESPACES TOPOLOGIQUES SÉPARÉS
section: 6
section_title: Promesures et mesures sur un espace localement convexe
lang: fr
source: int-ix-fr
pdf_pages: 0068-0093, 0108-0108
extraction: ocr
subsections:
    - "no": 1
      title: Promesures sur un espace localement convexe
      page: 0
      pdf_page: 68
    - "no": 2
      title: Image d'une promesure
      page: 0
      pdf_page: 70
    - "no": 3
      title: Transformée de Fourier d'une promesure
      page: 0
      pdf_page: 70
    - "no": 4
      title: Calculs d’intégrales gaussiennes
      page: 0
      pdf_page: 72
    - "no": 5
      title: Promesures et mesures gaussiennes
      page: 0
      pdf_page: 74
    - "no": 6
      title: Exemples de promesures gaussiennes
      page: 0
      pdf_page: 77
    - "no": 7
      title: Mesure de Wiener
      page: 0
      pdf_page: 79
    - "no": 8
      title: Continuité de la transformée de Fourier
      page: 0
      pdf_page: 85
    - "no": 9
      title: Le lemme de Minlos
      page: 0
      pdf_page: 87
    - "no": 10
      title: Mesures sur le dual d’un espace nucléaire
      page: 0
      pdf_page: 89
    - "no": 11
      title: Mesures sur un espace de Hilbert
      page: 0
      pdf_page: 90
statements: 36
exercises: 1
content_sha256: 4427ce6e61509fb93e77e5267f3caa6025ae8004ae114e8fc45c6c7344706320
---

## § 6. Promesures et mesures sur un espace localement convexe

Dans tout ce paragraphe, on ne considère que des espaces vectoriels sur le corps des nombres réels. Par espace localement convexe, on entend un espace vectoriel topologique séparé et localement convexe sur $\mathbf{R}$. Le dual topologique d’un espace localement convexe $E$ sera noté $E'$; pour $x \in E$ et $x' \in E'$, on posera $\langle x, x' \rangle = x'(x)$.

### 1. Promesures sur un espace localement convexe

Soit $E$ un espace localement convexe. On note $\mathcal{F}(E)$ l’ensemble des sous-espaces vectoriels fermés de codimension finie de $E$, ordonné par la relation $\supset$. Pour tout $V \in \mathcal{F}(E)$, on note $p_V$ l’application canonique de $E$ sur $E/V$. Soient $V$ et $W$ deux éléments de $\mathcal{F}(E)$ tels que $V \supset W$; on note $p_{VW}$ l’application de $E/W$ dans $E/V$ déduite par passage aux quotients de l’application identique de $E$. La famille $\mathcal{Q}(E) = (E/V, p_{VW})$ est un système projectif d’espaces localement convexes, indexé par $\mathcal{F}(E)$. On l’appelle le *système projectif des quotients de dimension finie de* $E$.

On peut montrer que la limite projective du système projectif $\mathcal{Q}(E)$ est canoniquement isomorphe au dual algébrique ${E'}^*$ de $E'$, muni de la topologie faible $\sigma({E'}^*, E')$.

#### Définition 1 {#int-ix-s6-def-1 .statement}

*Soit $E$ un espace localement convexe. On appelle promesure sur $E$ tout système projectif de mesures ($§ 4$, no 2, déf. 1) sur le système projectif des quotients de dimension finie de $E$.*

En d’autres termes, une promesure $\mu$ sur $E$ est une famille $(\mu_V)_{V \in \mathcal{F}(E)}$, où $\mu_V$ est une mesure (positive) bornée sur l’espace de dimension finie E/V, et où $\mu_V = p_{VW}(\mu_W)$ lorsque V ⊃ W. Toutes les mesures $\mu_V$ ont la même masse totale que l’on appelle la *masse totale* de la promesure $\mu$.

Pour qu’un sous-espace V de E appartienne à $\mathcal{F}(E)$, il faut et il suffit qu’il existe un nombre fini d’éléments $x'_1, \ldots, x'_n$ de E’ tels que V se compose des $x \in E$ satisfaisant à $\langle x, x'_i \rangle = 0$ pour $1 \leq i \leq n$ (*Esp. vect. top.*, chap. II, 2e éd., § 6, n° 3, cor. 2 du th. 1 et n° 5, cor. 2 de la prop. 7). De plus, il existe sur un espace vectoriel de dimension finie une seule topologie séparée d’espace vectoriel topologique (*loc. cit.*, chap. I, § 2, n° 3, th. 2). Par suite, la notion de promesure sur E ne dépend que du dual E’ de E.

Soit $\lambda$ une mesure bornée sur E. Pour tout $V \in \mathcal{F}(E)$, notons $\tilde{\lambda}_V$ l’image de $\lambda$ par l’application canonique $p_V$ de E sur E/V. On a $p_V = p_{VW} \circ p_W$ pour deux éléments V et W de $\mathcal{F}(E)$ tels que V ⊃ W; par suite, la famille $\tilde{\lambda} = (\tilde{\lambda}_V)_{V \in \mathcal{F}(E)}$ est une promesure sur E. Nous dirons que $\tilde{\lambda}$ est la promesure *associée* à la mesure $\lambda$. On voit immédiatement que $\lambda$ et $\tilde{\lambda}$ ont même masse totale.

#### Proposition 1 {#int-ix-s6-prop-1 .statement}

*Soit E un espace localement convexe. L’application $\lambda \mapsto \tilde{\lambda}$ est une bijection de l’ensemble des mesures bornées sur E sur l’ensemble des promesures $(\mu_V)_{V \in \mathcal{F}(E)}$ sur E satisfaisant à la condition suivante*:

*Pour tout $\varepsilon > 0$, il existe une partie compacte K de E telle que l’on ait $\mu_V(E/V - p_V(K)) \leq \varepsilon$ pour tout $V \in \mathcal{F}(E)$.*

On sait que l’intersection des noyaux des formes linéaires continues sur E est égale à 0 (*Esp. vect. top.*, chap. II, 2e éd., § 4, n° 2, cor. 1 de la prop. 2); on a par suite $\bigcap_{V \in \mathcal{F}(E)} V = \{0\}$ et la famille $(p_V)_{V \in \mathcal{F}(E)}$ est cohérente et séparante. La proposition résulte alors du th. 1 du § 4, n° 2.

En particulier, l’application $\lambda \mapsto \tilde{\lambda}$ est injective. Si $\mu$ est une promesure sur E, et s’il existe une mesure bornée $\lambda$ sur E telle que $\mu = \tilde{\lambda}$, nous dirons par abus de langage que $\mu$ est une mesure. Si E est de dimension finie, toute promesure $\mu = (\mu_V)_{V \in \mathcal{F}(E)}$ est une mesure: en effet, on a $\{0\} \in \mathcal{F}(E)$, $E/\{0\} = E$ et $p_{V,\{0\}} = p_V$, d’où $\mu_V = p_V(\mu_{\{0\}})$ pour tout $V \in \mathcal{F}(E)$; autrement dit, on a $\mu = \tilde{\lambda}$ avec $\lambda = \mu_{\{0\}}$.

#### Proposition 2 {#int-ix-s6-prop-2 .statement}

*Soient T un ensemble dénombrable, et E l’espace des fonctions réelles sur T, muni de la topologie de la convergence simple. Toute promesure sur E est une mesure.*

Pour tout $t \in T$, soit $\varepsilon_t$ la forme linéaire $f \mapsto f(t)$ sur E. On sait (*Esp. vect. top.*, chap. II, 2e éd., § 6, n° 6, cor. 2 de la prop. 8) que la famille $(\varepsilon_t)_{t \in T}$ est une base de l’espace vectoriel E’. On note par ailleurs $\Phi$ l’ensemble des parties finies de T, et pour tout $J \in \Phi$, on note $E_J$ l’ensemble des fonctions sur T nulles en tout point de J. Soit $F \in \mathcal{F}(E)$; comme l’orthogonal $F^0$ de F est un sous-espace de dimension finie de E’, il existe $J \in \Phi$ telle que $F^0$ soit contenu dans le sous-espace G de E’ engendré par les $\varepsilon_t$ pour $t \in J$. Comme $F^0 \subset G$, on a

$$
E_J = G^0 \subset F^{00} = F
$$

et la famille *dénombrable* $(E_J)_{J \in \Phi}$ est cofinale dans $\mathcal{F}(E)$. La prop. résulte alors du th. 2 du § 4, n° 3.

### 2. Image d'une promesure

Soient $E$ et $E_1$ deux espaces localement convexes, et $u$ une application linéaire continue de $E$ dans $E_1$. Pour tout $V_1 \in \mathcal{F}(E_1)$, le sous-espace $V = u^{-1}(V_1)$ de $E$ appartient à $\mathcal{F}(E)$, et $u$ définit par passage aux quotients une application linéaire $u_{V_1}$ de $E/V$ dans $E_1/V_1$. Soient $V_1$ et $W_1$ dans $\mathcal{F}(E_1)$ tels que $V_1 \supset W_1$; posons $V = u^{-1}(V_1)$ et $W = u^{-1}(W_1)$. On a $V \supset W$ et un diagramme commutatif

$$
\begin{array}{ccc}
E & \xrightarrow{p_W} & E/W \\
u \downarrow & & \downarrow u_{W_1} \\
E_1 & \xrightarrow{p_{W_1}} & E_1/W_1
\end{array}
$$
$$
\begin{array}{ccc}
E/W & \xrightarrow{p_{VW}} & E/V \\
\downarrow & & \downarrow u_{V_1} \\
E_1/W_1 & \xrightarrow{p_{V_1W_1}} & E_1/V_1.
\end{array}
$$

Soit alors $\mu = (\mu_V)_{V \in \mathcal{F}(E)}$ une promesure sur $E$. Pour tout $V_1 \in \mathcal{F}(E_1)$, posons
$$(1)$$
$$\nu_{V_1} = u_{V_1}(\mu_{u^{-1}(V_1)}).$$
La commutativité du diagramme précédent montre que la famille $\nu = (\nu_{V_1})_{V_1 \in \mathcal{F}(E_1)}$ est une promesure sur $E_1$. On dit que $\nu$ *est l'image de* $\mu$ *par* $u$, et on la note $u(\mu)$.

Soient $\lambda$ une mesure bornée sur $E$ et $u(\lambda)$ la mesure sur $E_1$ image de $\lambda$ par $u$. Si la promesure $\mu$ est associée à $\lambda$, la promesure $u(\mu)$ est associée à $u(\lambda)$. Cela résulte de la commutativité du diagramme précédent.

Soit $V \in \mathcal{F}(E)$. Il est immédiat que la promesure sur $E/V$ image de la promesure $\mu$ par l'application canonique $p_V : E \to E/V$ est associée à la mesure $\mu_V$.

Soit $u_1$ une application linéaire continue de $E_1$ dans un espace localement convexe $E_2$. On établit sans peine la relation $(u_1 \circ u)(\mu) = u_1(u(\mu))$ (« transitivité de l'image des promesures »).

### 3. Transformée de Fourier d'une promesure

Soient $E$ un espace localement convexe et $\mu = (\mu_V)_{V \in \mathcal{F}(E)}$ une promesure sur $E$. Pour toute forme linéaire continue $x'$ sur $E$, on note $\mu_{x'}$ la mesure sur $\mathbf{R}$ image par $x'$ de la promesure $\mu$ sur $E$. La transformée de Fourier de $\mu$ est la fonction $\mathcal{F}\mu$ sur $E'$ définie par
$$(2)$$
$$(\mathcal{F}\mu)(x') = \int_{\mathbf{R}} e^{it} d\mu_{x'}(t).$$

Soit $\lambda$ une mesure bornée sur E. La transformée de Fourier de $\lambda$ est la fonction sur $E'$ définie par

$$
(\mathcal{F}\lambda)(x') = \int_E e^{i\langle x, x' \rangle} d\lambda(x).
$$

Soit $\mu$ la promesure associée à $\lambda$. Pour tout $x' \in E'$, la mesure $\mu_{x'}$ sur $\mathbf{R}$ est l’image par $x': E \to \mathbf{R}$ de la mesure $\lambda$ sur E; des formules (2) et (3), on déduit aussitôt $\mathcal{F}\mu = \mathcal{F}\lambda$.

Soient $\mu$ une promesure quelconque sur E, $u$ une application linéaire continue de E dans un espace localement convexe $E_1$. Notons $^t u$ l’application linéaire de $E'_1$ dans $E'$ transposée de $u$ et $v$ la promesure $u(\mu)$ sur $E_1$. Pour tout $x'_1 \in E'_1$, on a $^t u(x'_1) = x'_1 \circ u$, d’où

$$
\nu_{x'_1} = x'_1(v) = x'_1(u(\mu)) = (x'_1 \circ u)(\mu) = \mu_{^t u(x'_1)}.
$$

On a par suite

$$
\mathcal{F}(u(\mu)) = (\mathcal{F}\mu) \circ ^t u.
$$

En particulier, prenons pour $u$ l’application canonique $p_V$ de E sur $E/V$ (pour $V \in \mathcal{F}(E)$). La promesure $p_V(\mu)$ sur $E/V$ est associée à la mesure $\mu_V$, et $^t p_V$ est un isomorphisme du dual de $E/V$ sur le sous-espace $V^0$ de $E'$ orthogonal à V. Si nous identifions $(E/V)'$ à $V^0$ par $^t p_V$, on a

$$
(\mathcal{F}\mu)(x') = \int_{E/V} e^{i\langle x, x' \rangle} d\mu_V(x)
$$

pour tout $x' \in V^0$. On a $E' = \bigcup_{V \in \mathcal{F}(E)} V^0$, de sorte que la formule précédente caractérise la fonction $\mathcal{F}\mu$ sur $E'$. Enfin, si l’on fait $x' = 0$ dans (5), on voit que la masse totale de $\mu$ est égale à $(\mathcal{F}\mu)(0)$.

#### Proposition 3 {#int-ix-s6-prop-3 .statement}

*Soit E un espace localement convexe. L’application $\mu \mapsto \mathcal{F}\mu$ de l’ensemble des promesures sur E dans l’ensemble des fonctions sur E’ est injective.*

La formule (5) permet de se ramener au cas où E est de dimension finie; comme tout espace de dimension finie est isomorphe à un espace $\mathbf{R}^n$, nous pouvons même supposer qu’il existe un entier $n \geqslant 0$ tel que $E = \mathbf{R}^n$. Nous avons donc à prouver que si $\mu$ est une mesure bornée (non nécessairement positive) sur $\mathbf{R}^n$ et si

$$
\int_{\mathbf{R}^n} e^{i\langle x, y \rangle} d\mu(x) = 0
$$

pour toute forme linéaire $y$ sur $\mathbf{R}^n$, on a $\mu = 0$.

Pour tout entier $m \geqslant 0$, soit $G_m$ le sous-groupe $m.\mathbf{Z}^n$ de $\mathbf{R}^n$. On note $\mathcal{C}_m$ l’espace vectoriel des fonctions continues $f$ sur $\mathbf{R}^n$ telles que $f(x + a) = f(x)$ pour $x \in \mathbf{R}^n$ et $a \in G_m$. D’après la prop. 8 de Top. gén., chap. X, 2e éd., § 4, n° 4, toute fonction de $\mathcal{C}_m$ est limite uniforme de combinaisons linéaires finies de fonctions du type $x \mapsto e^{2\pi i \langle x, q \rangle}$ avec $q \in m^{-1}.\mathbf{Z}^n$. On a donc $\mu(f) = 0$ pour toute fonction $f \in \mathcal{C}_m$.

Soit $f$ une fonction continue à support compact sur $\mathbf{R}^n$. Pour tout entier $m \geq 0$, posons $f_m(x) = \sum_{q \in G_m} f(x + q)$. Il est immédiat que pour tout $x \in \mathbf{R}^n$, la série précédente n’a qu’un nombre fini de termes, et que $f_m$ appartient à $\mathcal{C}_m$. De plus, on voit facilement que la suite $(f_m)$ tend uniformément vers $f$ sur tout compact, et qu’il existe une constante $C \geq 0$ telle que $|f_m| \leq C$ pour tout $m$. On a par suite $\mu(f) = \lim_{m \to \infty} \mu(f_m)$ d’après la prop. 12 du § 5, n° 6. Comme on a $f_m \in \mathcal{C}_m$, on a $\mu(f_m) = 0$, d’où finalement $\mu(f) = 0$. On a donc $\mu = 0$.

*Remarque. — Lorsque E est de dimension finie, tout caractère de E est de la forme $x \mapsto e^{i\langle x, x' \rangle}$ avec $x' \in E'$ (Théor. spect., chap. II, § 1, n° 9, cor. 3 de la prop. 12). La prop. 3 résulte dans ce cas du théorème d’unicité pour la transformation de Fourier (loc. cit., § 1, n° 6, cor. de la prop. 6).*

### 4. Calculs d’intégrales gaussiennes

#### Lemme 1 {#int-ix-s6-lem-1 .statement}

Pour tout entier $n \geq 0$, on a

(6)
$$
\int_{\mathbf{R}} |x|^n e^{-x^2/2} dx = 2^{\frac{n+1}{2}} \Gamma\left(\frac{n+1}{2}\right)
$$

(7)
$$
\int_{\mathbf{R}} x^{2n} e^{-x^2/2} dx = (2\pi)^{1/2} \frac{(2n)!}{2^n n!}
$$

(8)
$$
\int_{\mathbf{R}} x^{2n+1} e^{-x^2/2} dx = 0.
$$

Rappelons la formule

(9)
$$
\Gamma(s) = \int_0^\infty u^{s-1} e^{-u} du
$$
valable pour tout nombre réel $s > 0$ (Fonct. var. réelle, chap. VII, § 1, n° 3, prop. 3). En faisant le changement de variable $x = (2u)^{1/2}$, il vient d’après (9)

$$
\int_0^\infty x^n e^{-x^2/2} dx = \int_0^\infty (2u)^{n/2} e^{-u} \frac{1}{2} 2^{1/2} u^{-1/2} du = 2^{\frac{n-1}{2}} \Gamma\left(\frac{n+1}{2}\right),
$$
d’où la formule (6) puisque l’on a
$$
\int_{\mathbf{R}} |x|^n e^{-x^2/2} dx = 2 \int_0^\infty x^n e^{-x^2/2} dx.
$$
La formule (7) résulte de (6) et de la relation
$$
\Gamma\left(n + \frac{1}{2}\right) = \pi^{1/2} \frac{(2n)!}{2^{2n} n!}.
$$
Pour $n = 0$, cette relation se réduit à $\Gamma(\frac{1}{2}) = \pi^{1/2}$, c’est-à-dire à la formule (21)

de Fonct. var. réelle, chap. VII, § 1, n° 3. Le cas général s’en déduit par récurrence sur $n$ en tenant compte de la relation $\Gamma(x + 1) = x \cdot \Gamma(x)$ (loc. cit., § 1, n° 1).

Enfin, la formule (8) résulte de ce que la fonction $x \mapsto x^{2n+1} e^{-x^2/2}$ est impaire.

#### Lemme 2 {#int-ix-s6-lem-2 .statement}

Pour tout nombre complexe $y$, on a

$$
(2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} e^{ixy} dx = e^{-y^2/2}.
$$

En particulier, on a

$$
(2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} dx = 1.
$$

Le changement de variable $x \mapsto -x$ donne

$$
(2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} e^{ixy} dx = (2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} e^{-ixy} dx;
$$

comme on a $\cos u = \frac{e^{iu} + e^{-iu}}{2}$ pour tout nombre complexe $u$, on en déduit

$$
(2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} e^{ixy} dx = (2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} \cos xy dx.
$$

Pour tout entier $n \geqslant 0$, posons

$$
g_n(x) = (-1)^n (2\pi)^{-1/2} \frac{(xy)^{2n}}{(2n)!} e^{-x^2/2}.
$$

D’après (7), on a

$$
\int_{\mathbf{R}} |g_n(x)| dx = \frac{1}{n!} \left( \frac{|y|^2}{2} \right)^n
$$
$$
\int_{\mathbf{R}} g_n(x) dx = \frac{1}{n!} \left( -\frac{y^2}{2} \right)^n,
$$

d’où

$$
\sum_{n=0}^{\infty} \int_{\mathbf{R}} |g_n(x)| dx = e^{|y|^2/2} < +\infty.
$$

Comme on a par ailleurs

$$
(2\pi)^{-1/2} e^{-x^2/2} \cos xy = \sum_{n=0}^{\infty} g_n(x),
$$

on peut intégrer terme à terme cette égalité, d’où

$$
(2\pi)^{-1/2} \int_{\mathbf{R}} e^{-x^2/2} \cos xy dx = \sum_{n=0}^{\infty} \int_{\mathbf{R}} g_n(x) dx = e^{-y^2/2}
$$

d’après (14). La formule (11) résulte alors de (12).

### 5. Promesures et mesures gaussiennes

#### Proposition 4 {#int-ix-s6-prop-4 .statement}

Soit E un espace localement convexe. Pour toute forme quadratique positive Q sur E', il existe une promesure $\Gamma_Q$ sur E et une seule, telle que $\mathcal{F}\Gamma_Q = e^{-Q/2}$. La masse totale de $\Gamma_Q$ est égale à 1.

L’unicité de $\Gamma_Q$ résulte de la proposition 3 du n° 3. La masse totale de $\Gamma_Q$ est égale à $(\mathcal{F}\Gamma_Q)(0) = e^{-Q(0)/2} = 1$. Nous démontrons l’existence par étapes.

A) E est de dimension finie n et Q est non dégénérée.

D’après le lemme 2 du n° 4, la mesure $\gamma_1$ sur $\mathbf{R}$ admettant la densité $t \mapsto (2\pi)^{-1/2} e^{-t^2/2}$ est bornée, de masse totale 1. Posons $\gamma = \gamma_1 \otimes \cdots \otimes \gamma_1$ (n facteurs). Du lemme 2 du n° 4, on déduit

$$
\int_{\mathbf{R}^n} e^{i(a_1 t_1 + \cdots + a_n t_n)} d\gamma(t_1, \ldots, t_n) = \prod_{j=1}^n \int_{\mathbf{R}} e^{ia_j t} d\gamma_1(t)
$$
$$
= \prod_{j=1}^n (2\pi)^{-1/2} \int_{\mathbf{R}} e^{ia_j t} e^{-t^2/2} dt
$$
$$
= \prod_{j=1}^n e^{-a_j^2/2}
$$
$$
= \exp \left( -\frac{1}{2}(a_1^2 + \cdots + a_n^2) \right).
$$

Comme Q est positive et non dégénérée, il existe une base $(e'_1, \ldots, e'_n)$ de E' orthonormale pour Q (Alg., chap. IX, § 7, n° 1). Notons f l’isomorphisme $x \mapsto (e'_1(x), \ldots, e'_n(x))$ de E sur $\mathbf{R}^n$ et $\Gamma_Q$ la mesure $f^{-1}(\gamma)$ sur E. Soit $x' = a_1 e'_1 + \cdots + a_n e'_n$ dans E'; on a $x'(f^{-1}(t_1, \ldots, t_n)) = \sum_{j=1}^n t_j a_j$ pour $t_1, \ldots, t_n$ réels, d’où

$$
\int_E e^{i\langle x, x' \rangle} d\Gamma_Q(x) = \int_{\mathbf{R}^n} e^{i(a_1 t_1 + \cdots + a_n t_n)} d\gamma(t_1, \ldots, t_n)
$$
$$
= \exp \left( -\frac{1}{2}(a_1^2 + \cdots + a_n^2) \right) = \exp \left( -\frac{1}{2}Q(x') \right).
$$

Par suite, on a $\mathcal{F}\Gamma_Q = e^{-Q/2}$.

B) E est de dimension finie.

Soit N le sous-espace vectoriel de E' formé des $x'$ tels que $Q(x') = 0$. Notons M l’orthogonal de N dans E et j l’injection canonique de M dans E. L’application linéaire $t j : E' \to M'$ est surjective, de noyau N, et il existe donc sur M' une forme quadratique positive non dégénérée q telle que $Q = q \circ t j$. D’après ce qui précède, il existe sur M une mesure bornée $\Gamma$ telle que $\mathcal{F}\Gamma = e^{-q/2}$. Si l’on pose $\Gamma_Q = j(\Gamma)$, on a

$$
\mathcal{F}\Gamma_Q = (\mathcal{F}\Gamma) \circ t j = \exp \left( -q \circ t j / 2 \right) = e^{-Q/2}
$$

d’après la formule (4) du n° 3.

C) Cas général.

Soit $V \in \mathcal{F}(E)$. Notons $p_V$ l’application canonique de E sur E/V et $Q_V$ la forme quadratique positive $Q \circ t p_V$ sur $(E/V)'$; enfin, soit $\mu_V$ la mesure sur $E/V$ de transformée de Fourier $e^{-Q_V/2}$ (cf. B)). Si $W \in \mathcal{F}(E)$ est contenu dans $V$, on a $p_V = p_{VW} \circ p_W$, d'où $Q_V = Q_W \circ t p_{VW}$; d'après la formule (4) du n° 3, la mesure $p_{VW}(\mu_W)$ a pour transformée de Fourier la fonction $(e^{-Q_W/2}) \circ t p_{VW} = e^{-Q_V/2}$, donc est égale à $\mu_V$. La famille $(\mu_V)_{V \in \mathcal{F}(E)}$ est donc une promesure $\mu$ sur $E$. La formule (5) du n° 3 montre que $\mathcal{F} \mu$ est égale à $e^{-Q/2}$.

#### Définition 2 {#int-ix-s6-def-2 .statement}

Soit $E$ un espace localement convexe. Pour toute forme quadratique positive $Q$ sur $E'$, on appelle promesure gaussienne de variance $Q$ sur $E$, et l'on note $\Gamma_Q$, la promesure sur $E$ dont la transformée de Fourier est égale à $e^{-Q/2}$. On dit qu'une promesure $\mu$ sur $E$ est gaussienne s'il existe une forme quadratique positive $Q$ sur $E'$ telle que $\mu = \Gamma_Q$.

Par abus de langage, on dira qu'une mesure bornée $\mu$ sur $E$ est gaussienne de variance $Q$ si la promesure associée $\tilde{\mu}$ est égale à $\Gamma_Q$.

#### Remarque 1 {#int-ix-s6-n5-rem-1 .statement}

Soit $E$ un espace vectoriel de dimension finie, et soit $\mu$ une mesure positive de masse 1 sur $E$, telle que toute forme linéaire sur $E$ appartienne à $\mathcal{L}^2(E, \mu)$. On définit un élément $m$ de $E$ et une forme quadratique positive $V$ sur $E'$ par les formules
$$
\langle m, x' \rangle = \int_E \langle x, x' \rangle \, d\mu(x), \qquad V(x') = \int_E \langle x - m, x' \rangle^2 \, d\mu(x).
$$
Dans la terminologie traditionnelle du Calcul des Probabilités, $m$ s'appelle la moyenne et $V$ la variance de $\mu$; on dit que $\mu$ est centrée si $m = 0$.

Soient alors $a$ un élément de $E$ et $Q$ une forme quadratique positive sur $E'$. Notons $\Gamma_{a, Q}$ l'image de la mesure $\Gamma_Q$ par la translation $x \mapsto x + a$. On voit facilement que $\Gamma_{a, Q}$ est une mesure positive de masse 1 sur $E$, de transformée de Fourier $x' \mapsto e^{i \langle a, x' \rangle - \frac{1}{2} Q(x')}$ et de moyenne $a$. De plus, la prop. 6 entraîne que $Q$ est la variance de $\Gamma_{a, Q}$. Traditionnellement, on dit que $\Gamma_{a, Q}$ est la mesure gaussienne de moyenne $a$ et variance $Q$, et que $\Gamma_Q = \Gamma_{0, Q}$ est la mesure gaussienne centrée de variance $Q$. Comme nous n'aurons à considérer que des mesures gaussiennes centrées, nous omettons ce qualificatif.

#### Remarque 2 {#int-ix-s6-n5-rem-2 .statement}

Soit $Q$ une forme quadratique sur le dual $E'$ d'un espace localement convexe $E$. S'il existe une promesure sur $E$ de transformée de Fourier $e^{-Q/2}$, la forme quadratique $Q$ est nécessairement positive : la fonction $e^{-Q/2}$ est en effet bornée sur $E'$; donc, pour tout $x' \in E'$, la fonction $t \mapsto e^{-t^2 Q(x')/2} = e^{-Q(t x')/2}$ sur $\mathbf{R}$ est bornée, d'où $Q(x') \geqslant 0$.

#### Remarque 3 {#int-ix-s6-n5-rem-3 .statement}

Le dual de $\mathbf{R}$ est canoniquement isomorphe à $\mathbf{R}$ et les formes quadratiques positives sur $\mathbf{R}$ sont les fonctions de la forme $t \mapsto a t^2$ avec $a \geqslant 0$. Pour tout $a \geqslant 0$, il existe donc une mesure bornée $\gamma_a$ sur $\mathbf{R}$ et une seule dont la transformée de Fourier soit égale à la fonction $t \mapsto e^{-a t^2/2}$; on dit par abus de langage que $\gamma_a$ est la mesure gaussienne sur $\mathbf{R}$ de variance $a$.

La transformée de Fourier de $\gamma_0$ est la constante 1, d'où $\gamma_0 = \varepsilon_0$ (masse unité à l'origine de $\mathbf{R}$). Supposons $a > 0$ et notons $u_a$ l'application linéaire $x \mapsto a^{1/2} x$; on a $\mathcal{F} \gamma_a = \mathcal{F} \gamma_1 \circ t u_a$ d'où $\gamma_a = u_a(\gamma_1)$. Le lemme 2 montre que $\gamma_1$ est la mesure de densité $x \mapsto (2\pi)^{-1/2} e^{-x^2/2}$ par rapport à la mesure de Lebesgue; on en déduit facilement
$$
(15) \qquad d\gamma_a(x) = (2\pi a)^{-1/2} e^{-x^2/2a} \, dx.
$$

L'image d'une promesure gaussienne par une application linéaire continue est une promesure gaussienne. De manière précise, on a le résultat suivant:

#### Proposition 5 {#int-ix-s6-prop-5 .statement}

Soient E et E₁ deux espaces localement convexes et u une application linéaire continue de E dans E₁. Soient Q une forme quadratique positive sur E' et Q₁ la forme quadratique positive Q o t u sur E₁'. On a u(Γ_Q) = Γ_{Q₁}.
Posons μ = u(Γ_Q). D’après la formule (4) du n° 3, on a
$$
\mathcal{F}μ = (\mathcal{F}Γ_Q) o t u = e^{-Q/2} o t u = e^{-Q_1/2} = \mathcal{F}Γ_{Q_1}
$$
d’où μ = Γ_{Q₁} d’après la prop. 3 du n° 3.

#### Corollaire {#int-ix-s6-n5-cor-1 .statement}

Soient E un espace localement convexe et Q une forme quadratique positive sur E'. Pour tout x' ∈ E', l’image de Γ_Q par x' est la mesure gaussienne de variance Q(x') sur R.

#### Proposition 6 {#int-ix-s6-prop-6 .statement}

Soient E un espace localement convexe et μ une mesure gaussienne sur E, de variance Q. Pour tout entier n ≥ 0, et tout x' ∈ E', on a les relations
(16)
$$
\int_E |\langle x, x' \rangle|^n dμ(x) = π^{-1/2} 2^{n/2} \Gamma \left( \frac{n+1}{2} \right) Q(x')^{n/2}
$$
(17)
$$
\int_E \langle x, x' \rangle^{2n} dμ(x) = \frac{(2n)!}{2^n n!} Q(x')^n
$$
(18)
$$
\int_E \langle x, x' \rangle^{2n+1} dμ(x) = 0.
$$
En particulier, on a
(19)
$$
\int_E \langle x, x' \rangle^2 dμ(x) = Q(x') \quad (x' \in E').
$$

Si ces formules sont vraies pour un élément x' de E', elles sont vraies pour tous ses multiples t.x' (avec t réel). On peut donc se contenter de les établir lorsque Q(x') est égal à 0 ou 1.
a) Supposons Q(x') = 0. La mesure x'(μ) est égale à γ₀ = ε₀, donc x' est nulle μ-presque partout; les formules (16) à (19) sont alors évidentes.
b) Supposons Q(x') = 1, d’où x'(μ) = γ₁. On a
$$
\int_E |\langle x, x' \rangle|^n dμ(x) = \int_\mathbf{R} |t|^n dγ_1(t) = (2π)^{-1/2} \int_\mathbf{R} |t|^n e^{-t^2/2} dt
$$
et (16) résulte immédiatement de (6) (n° 4, lemme 1). De même, les formules (17) et (18) résultent de (7) et (8). Enfin, (19) s’obtient en faisant n = 1 dans (17).

Nous pouvons maintenant démontrer une réciproque du cor. de la prop. 5.

#### Proposition 7 {#int-ix-s6-prop-7 .statement}

Soient E un espace localement convexe et μ une promesure sur E. On suppose que x'(μ) est une mesure gaussienne sur R pour tout x' ∈ E'. Alors μ est une promesure gaussienne sur E.

Pour tout $x' \in E'$, soit $Q(x')$ la variance de la mesure gaussienne $x'(\mu)$ sur $\mathbf{R}$. On a $x'(\mu) = \gamma_{Q(x')}$, d'où

$$
(\mathcal{F}\mu)(x') = \int_{\mathbf{R}} e^{it.1} d\gamma_{Q(x')}(t) = e^{-Q(x').1^2/2}
$$

d’après la définition de $\mathcal{F}\mu$ (n° 3, formule (2)). Autrement dit, on a $\mathcal{F}\mu = e^{-Q/2}$, et il reste à prouver que $Q$ est une forme quadratique positive sur $E'$.

Pour tout sous-espace vectoriel fermé $V$ de $E$, de codimension finie, notons $p_V$ l’application canonique de $E$ sur $E/V$, $\mu_V$ la mesure $p_V(\mu)$ sur $E/V$ et posons $Q_V = Q \circ {}^t p_V$. Comme on a $E' = \bigcup_{V \in \mathcal{F}(E)} \operatorname{Im}({}^t p_V)$ et que ${}^t p_V$ est injectif, il suffit de prouver que $Q_V$ est une forme quadratique positive sur $(E/V)'$. Soient $u \in (E/V)'$ et $x' = {}^t p_V(u)$. On a

$$
u(\mu_V) = u(p_V(\mu)) = x'(\mu) = \gamma_{Q(x')};
$$

la prop. 6 entraîne alors

$$
Q_V(u) = Q(x') = \int_{\mathbf{R}} t^2 d\gamma_{Q(x')}(t) = \int_{E/V} u(x)^2 d\mu_V(x),
$$

donc $Q_V$ est une forme quadratique positive sur $(E/V)'$.

### 6. Exemples de promesures gaussiennes

1) Soit $E$ un espace hilbertien réel. L’application $x' \mapsto \|x'\|^2$ est une forme quadratique positive sur $E'$. La promesure gaussienne correspondante s’appelle la *promesure gaussienne canonique* sur $E$. On peut montrer que cette promesure n’est pas une mesure si $E$ est de dimension infinie.

Soit $A$ un opérateur linéaire continu dans $E$. L’application $x' \mapsto \|{}^t A.x'\|^2$ est une forme quadratique positive sur $E'$. La promesure correspondante $\mu_A$ sur $E$ est une mesure si et seulement si $A$ est un opérateur de Hilbert–Schmidt.

2) *Noyaux de type positif*. On note $T$ un ensemble et $E = \mathbf{R}^T$ l’espace vectoriel des fonctions réelles dans $T$, muni de la topologie de la convergence simple. Pour tout $t \in T$, on note $\varepsilon_t$ la forme linéaire $f \mapsto f(t)$ sur $E$. La famille $(\varepsilon_t)_{t \in T}$ est une base de $E'$ (*Esp. vec. top.*, chap. II, 2e éd., § 6, n° 6, cor. 2 de la prop. 8).

On appelle noyau de type positif (réel) sur $T$ toute fonction à valeurs réelles $K$ sur $T \times T$ satisfaisant aux relations

(20)
$$
K(t, t') = K(t', t) \quad \text{pour } t, t' \text{ dans } T,
$$

(21)
$$
\sum_{i,j=1}^p c_i c_j K(t_i, t_j) \geqslant 0
$$

quels que soient l’entier positif $p$, les éléments $t_1, \ldots, t_p$ de $T$ et les nombres réels $c_1, \ldots, c_p$. S’il en est ainsi, la formule

(22)
$$
q \left( \sum_{t \in T} c_t \varepsilon_t \right) = \sum_{t, t' \in T} c_t c_{t'} K(t, t')
$$

définit une forme quadratique positive sur E'. Inversement, si q est une forme quadratique positive sur E', la formule

$$
K(t, t') = \frac{1}{2}[q(\varepsilon_t + \varepsilon_{t'}) - q(\varepsilon_t) - q(\varepsilon_{t'})]
$$

définit un noyau de type positif K sur T. On obtient ainsi deux bijections réciproques entre l'ensemble des noyaux de type positif sur T, et celui des formes quadratiques positives sur E'.

Soient K un noyau de type positif sur T, et q la forme quadratique associée sur E'. La promesure gaussienne sur E de variance q s'appelle aussi la *promesure gaussienne sur E de covariance* K. Si T est dénombrable, la prop. 2 du n° 1 entraîne que cette promesure est une mesure.

3) Soit T un ensemble dénombrable. On définit un noyau de type positif δ sur T en posant

$$
\delta(t, t') = \begin{cases}
1 & \text{si } t = t' \\
0 & \text{si } t \neq t'.
\end{cases}
$$

La forme quadratique correspondante est donnée par $q \left( \sum_{t \in T} c_t \varepsilon_t \right) = \sum_{t \in T} c_t^2$. Pour tout $t \in T$, notons $\mu_t$ la mesure gaussienne de variance 1 sur $\mathbf{R}$; on montre facilement que la mesure gaussienne sur $\mathbf{R}^T$ de covariance δ est égale à $\bigotimes_{t \in T} \mu_t$.

4) Soit $n \geqslant 1$ un entier. Une matrice carrée $C = (c_{ij})$ d'ordre n est dite *symétrique positive* si elle est symétrique et si l'on a $\sum_{i,j=1}^n c_{ij} x_i x_j \geqslant 0$ quels que soient $x_1, \ldots, x_n$ réels; il revient au même de dire que l'application $(i, j) \mapsto c_{ij}$ est un noyau de type positif sur l'ensemble $\{1, 2, \ldots, n\}$. On parlera donc de la mesure gaussienne $\gamma_C$ sur $\mathbf{R}^n$, de covariance C; elle est caractérisée par la formule

$$
\int_{\mathbf{R}^n} e^{i(x_1 t_1 + \cdots + x_n t_n)} d\gamma_C(t_1, \ldots, t_n) = \exp \left( -\frac{1}{2} \sum_{j,k=1}^n c_{jk} x_j x_k \right),
$$

pour $x_1, \ldots, x_n$ réels. De la prop. 6 du n° 5 (formule (19)), on déduit

$$
\int_{\mathbf{R}^n} t_j t_k d\gamma_C(t_1, \ldots, t_n) = c_{jk} \quad (1 \leqslant j, k \leqslant n).
$$

De la prop. 5 du n° 5, on déduit la formule

$$
u(\gamma_C) = \gamma_{UC^t U},
$$

où u est une application linéaire de $\mathbf{R}^n$ dans $\mathbf{R}^m$ de matrice U. Par ailleurs, on voit facilement (cf. début de la démonstration de la prop. 4 du n° 5) que, si $I_n$ désigne la matrice unité d'ordre n, la mesure $\gamma_{I_n}$ admet la densité

$$
(2\pi)^{-n/2} \exp \left( -\frac{1}{2}(t_1^2 + \cdots + t_n^2) \right)
$$

par rapport à la mesure de Lebesgue $\lambda_n$ sur $\mathbf{R}^n$.

Nous allons montrer que si la matrice $C$ est inversible, d’inverse $D = (d_{jk})$, on a

$$
(28)\quad d\gamma_C(t_1, \ldots, t_n) = (2\pi)^{-n/2} (\det D)^{1/2} \left( \exp \left( -\frac{1}{2} \sum_{j,k=1}^n d_{jk} t_j t_k \right) \right) dt_1 \ldots dt_n.
$$

En effet, si $C$ est inversible, la forme quadratique $q$ sur $\mathbf{R}^n$ définie par

$$
q(x_1, \ldots, x_n) = \sum_{j,k=1}^n c_{jk} x_j x_k
$$

est non dégénérée. En utilisant l’existence d’une base de $\mathbf{R}^n$ orthonormale pour $q$, on démontre l’existence d’une matrice $U$ carrée d’ordre $n$ telle que $C = U \cdot {}^t U$, d’où $\gamma_C = u(\gamma_{I_n})$ d’après (27) (on note $u$ l’automorphisme de $\mathbf{R}^n$ de matrice $U$). Soit $Q$ la forme quadratique sur $\mathbf{R}^n$ définie par

$$
Q(t_1, \ldots, t_n) = t_1^2 + \cdots + t_n^2;
$$

on a

$$
\gamma_{I_n} = (2\pi)^{-n/2} e^{-Q/2} \cdot \lambda_n,
$$

d’où

$$
u(\gamma_{I_n}) = (2\pi)^{-n/2} e^{-(Q \circ u^{-1})/2} \cdot u(\lambda_n).
$$

Il est immédiat que la forme quadratique $Q \circ u^{-1}$ sur $\mathbf{R}^n$ prend la valeur $\sum_{j,k=1}^n d_{jk} t_j t_k$ au point $(t_1, \ldots, t_n)$, et la prop. 15 du chap. VII, § 1, n° 10 montre que l’on a

$$
u(\lambda_n) = (\det U)^{-1} \cdot \lambda_n = (\det D)^{1/2} \cdot \lambda_n.
$$

La formule (28) résulte alors de là.

### 7. Mesure de Wiener

Dans ce n°, nous notons $T$ l’intervalle $]0, 1]$ de $\mathbf{R}$ et $\mathcal{H}$ l’espace de Hilbert des fonctions réelles de carré intégrable par rapport à la mesure de Lebesgue sur $T$, où l’on note $(f|g)$ le produit scalaire. On note aussi $\mathcal{C}$ l’espace des fonctions continues réelles sur $T$, tendant vers 0 au point 0; on munit $\mathcal{C}$ de la norme $\|f\| = \sup_{t \in T} |f(t)|$. L’intervalle compact $[0, 1] = T \cup \{0\}$ est le compactifié d’Alexandroff de l’intervalle localement compact mais non compact $T$; par suite, l’ensemble des fonctions continues à support compact sur $T$ est dense dans $\mathcal{C}$ et le dual de $\mathcal{C}$ s’identifie à l’espace $\mathcal{M}^1$ des mesures bornées (non nécessairement positives) sur $T$ (chap. III, 2e éd., § 1, n° 8, déf. 3).

Pour toute fonction $f \in \mathcal{H}$, on définit une fonction $Pf$ sur $T$ par

$$
(Pf)(t) = \int_0^t f(x) \, dx = (f|I_t),
$$

où $I_t$ est la fonction caractéristique de l’intervalle $]0, t]$. L’inégalité de Cauchy–Schwarz entraîne les inégalités

$$
|(Pf)(t)| \leq \|f\|_2 \cdot t^{1/2}
$$
$$
|(Pf)(t) - (Pf)(t')| \leq \|f\|_2 \cdot |t - t'|^{1/2};
$$

par suite, $Pf$ appartient à $\mathcal{C}$, et l’application linéaire $P$ de $\mathcal{H}$ dans $\mathcal{C}$ est continue de norme $\leq 1$.

Identifions l’espace de Hilbert $\mathcal{H}$ à son dual ($Esp.\ vect.\ top.$, chap. V, § 1, n° 6, th. 3), et notons $\Pi : \mathcal{M}^1 \to \mathcal{H}$ la transposée de $P : \mathcal{H} \to \mathcal{C}$. Pour toute mesure $\mu \in \mathcal{M}^1$ et toute fonction $f \in \mathcal{H}$, on a

$$
(\Pi \mu | f) = \mu(Pf) = \int_T d\mu(t) \int_T I_t(x) f(x) \, dx
$$
$$
= \int_T f(x) \, dx \int_T I_t(x) \, d\mu(t)
$$

d’après le théorème de Lebesgue–Fubini. Or on a

$$
I_t(x) = \begin{cases} 1 & \text{si } 0 < x \leq t \leq 1 \\ 0 & \text{sinon,} \end{cases}
$$

d’où finalement

$$
(\Pi \mu)(x) = \mu([x, 1]) \quad \text{pour } x \in T.
$$

Soient $\mu, \nu$ dans $\mathcal{M}^1$. On a

$$
(\Pi \mu | \Pi \nu) = \int_T \Pi \mu(x) \, \Pi \nu(x) \, dx = \int_T dx \int_T I_t(x) \, d\mu(t) \int_T I_{t'}(x) \, d\nu(t')
$$
$$
= \int_T \int_T d\mu(t) \, d\nu(t') \int_T I_t(x) I_{t'}(x) \, dx.
$$

Or $I_t . I_{t'}$ est la fonction caractéristique de l’intervalle $]0, t] \cap ]0, t']$, d’où immédiatement

$$
\int_T I_t(x) I_{t'}(x) \, dx = \inf (t, t').
$$

On en conclut

$$
(\Pi \mu | \Pi \nu) = \int_T \int_T \inf (t, t') \, d\mu(t) \, d\nu(t').
$$

D’après le résultat précédent, on définit une forme quadratique positive $W$ sur $\mathcal{M}^1$ par la formule

$$
W(\mu) = \int_T \int_T \inf (t, t') \, d\mu(t) \, d\mu(t') = \| \Pi \mu \|_2^2.
$$

En particulier, si $t_1, \ldots, t_n$ sont des éléments de $T$, et $c_1, \ldots, c_n$ des nombres réels, on a
$$
W \left( \sum_{j=1}^n c_j \varepsilon_{t_j} \right) = \sum_{j,k=1}^n c_j c_k \inf (t_j, t_k)
$$
et comme $W$ est positive, la fonction $(t, t') \mapsto \inf (t, t')$ est un noyau de type positif sur $T$.

#### Théorème 1 (Wiener) {#int-ix-s6-thm-1 .statement}

Soit $w$ l’image par $P : \mathcal{H} \to \mathcal{C}$ de la promesure gaussienne canonique sur l’espace de Hilbert $\mathcal{H}$. Alors $w$ est une mesure gaussienne de variance $W$ sur $\mathcal{C}$.

Par construction, on a $W(\mu) = \| tP(\mu) \|_2^2$; la prop. 5 du n° 5 montre que $w$ est une promesure gaussienne de variance $W$. Il reste à prouver que $w$ est une mesure sur $\mathcal{C}$.

A) Construction d’un espace mesuré auxiliaire $(\Omega, m)$:
Pour tout entier $n \geq 0$, on note $D_n$ l’ensemble des nombres de la forme $k/2^n$ avec $k = 1, 2, 3, \ldots, 2^n$. On pose $D = \bigcup_{n \geq 0} D_n$ (ensemble des nombres dyadiques contenus dans $T$) et $\Omega = \mathbf{R}^D$. Pour tout $t \in D$, on note $X(t)$ la forme linéaire $f \mapsto f(t)$ sur $\Omega$.

Pour $t, t'$ dans $D$, posons $M(t, t') = \inf (t, t')$; on a vu que $M$ est un noyau de type positif sur $D$. Comme l’ensemble $D$ est dénombrable, on peut définir la mesure gaussienne $m$ sur $\Omega$ de covariance $M$ (n° 6, Exemple 2).

#### Lemme 3 {#int-ix-s6-lem-3 .statement}

Quels que soient $t, t'$ dans $D$, on a
$$
\int_\Omega \left| X \left( \frac{t + t'}{2} \right) - \frac{X(t) + X(t')}{2} \right|^3 dm = \frac{1}{(8\pi)^{1/2}} |t - t'|^{3/2}.
$$

On notera que $\frac{t + t'}{2}$ appartient à $D$. On sait (n° 6, Exemple 2) que la famille $(X(t))_{t \in D}$ est une base du dual topologique $\Omega'$ de $\Omega$; il existe donc une forme bilinéaire symétrique $\hat{M}$ sur $\Omega' \times \Omega'$ caractérisée par $\hat{M}(X(t), X(t')) = \inf (t, t')$. Par construction, la variance de la mesure gaussienne $m$ sur $\Omega$ est la forme quadratique $\xi \mapsto \hat{M}(\xi, \xi)$ sur $\Omega'$. Posons en particulier
$$
\xi = X \left( \frac{t + t'}{2} \right) - \frac{X(t) + X(t')}{2};
$$
un calcul facile donne
$$
\hat{M}(\xi, \xi) = \frac{|t - t'|}{4}.
$$
D’après la prop. 6 du n° 5 (formule (16)), on a
$$
\int_\Omega |\xi|^3 dm = \pi^{-1/2} 2^{3/2} \Gamma(2) \hat{M}(\xi, \xi)^{3/2};
$$
le lemme résulte immédiatement des formules (40) et (41).

B) Construction d'une application u de $\Omega$ dans $\mathcal{C}$:
Pour tout entier $n \geqslant 0$, on note $E_n$ le sous-espace de $\mathcal{C}$ formé des fonctions qui sont affines dans chacun des intervalles $\left[ \frac{k-1}{2^n}, \frac{k}{2^n} \right]$ pour $1 \leqslant k \leqslant 2^n$. Une fonction affine dans un intervalle compact I de $\mathbf{R}$ atteint ses bornes aux extrémités de I; par suite, on a

$$
\| f \| = \sup_{1 \leqslant k \leqslant 2^n} \left| f \left( \frac{k}{2^n} \right) \right|
$$

pour $f \in E_n$.

Pour toute fonction $g \in \Omega$ et tout entier $n \geqslant 0$, il existe une fonction $u_n(g)$ et une seule qui appartienne à $E_n$ et coïncide avec $g$ en tout point de $D_n$; on posera $T_n g = u_{n+1}(g) - u_n(g)$. Comme $D_n$ est fini, l'application $T_n$ de $\Omega$ dans $\mathcal{C}$ est continue, donc $m$-mesurable.

#### Lemme 4 {#int-ix-s6-lem-4 .statement}

Pour tout entier $n \geqslant 0$, on a

$$
\int_\Omega \| T_n g \|^3 \, dm(g) \leqslant \frac{1}{(8\pi)^{1/2}} 2^{-n/2}.
$$

Soient $g \in \Omega$ et $n \in \mathbf{N}$. On a $E_n \subset E_{n+1}$; par suite, la fonction $T_n g$ appartient à $E_{n+1}$ et s'annule en tout point de $D_n$; d'après (42), on a donc

$$
\| T_n g \|^3 = \sup_{1 \leqslant k \leqslant 2^n} \left| T_n g \left( \frac{2k-1}{2^{n+1}} \right) \right|^3 \leqslant \sum_{k=1}^{2^n} \left| T_n g \left( \frac{2k-1}{2^{n+1}} \right) \right|^3.
$$

Faisons la convention $g(0) = 0$. La construction de $u_n(g)$ par interpolation linéaire de $g$ entraîne les relations

![Figure 1](https://example.com/figure1.png)

Figure 1

(45) $T_n g\left(\frac{2k-1}{2^{n+1}}\right) = g\left(\frac{2k-1}{2^{n+1}}\right) - \frac{1}{2}\left(g\left(\frac{k-1}{2^n}\right) + g\left(\frac{k}{2^n}\right)\right)$

pour $1 \leq k \leq 2^n$. On en déduit par intégration

$$ \int_\Omega \left| T_n g\left(\frac{2k-1}{2^{n+1}}\right) \right|^3 dm(g) = \int_\Omega \left| X\left(\frac{2k-1}{2^{n+1}}\right) - \frac{1}{2}\left(X\left(\frac{k-1}{2^n}\right) + X\left(\frac{k}{2^n}\right)\right) \right|^3 dm; $$

on peut alors appliquer le lemme 3 avec $t = \frac{k-1}{2^n}, t' = \frac{k}{2^n}$, d'où

(46) $\int_\Omega \left| T_n g\left(\frac{2k-1}{2^{n+1}}\right) \right|^3 dm(g) = \frac{1}{(8\pi)^{1/2}} 2^{-\frac{3n}{2}}.$

D'après (44), on a alors

$$ \int_\Omega \|T_n g\|^3 dm(g) \leq \sum_{k=1}^{2^n} \int_\Omega \left| T_n g\left(\frac{2k-1}{2^{n+1}}\right) \right|^3 dm(g) = \frac{1}{(8\pi)^{1/2}} 2^n \cdot 2^{-\frac{3n}{2}}, $$

d'où le lemme.

D'après le lemme 4, l'application $T_n$ de $\Omega$ dans l'espace de Banach $\mathcal{C}$ appartient à $L_3^3(\Omega, m)$ et l'on a $N_3(T_n) \leq \frac{1}{(8\pi)^{1/6}} (2^{-1/6})^n$, d'où $\sum_{n=0}^\infty N_3(T_n) < +\infty$.

D'après la prop. 6 du chap. IV, 2e éd., § 3, n° 3, il existe un ensemble $\Omega_0 \subset \Omega$ tel que $\Omega - \Omega_0$ soit $m$-négligeable et que la série $\sum_{n=0}^\infty T_n(g)$ converge absolument dans $\mathcal{C}$ pour tout $g \in \Omega_0$. On définit alors une application $m$-mesurable $u$ de $\Omega$ dans $\mathcal{C}$ par

(47)
$$
u(g) = \begin{cases}
\sum_{n=0}^\infty T_n g = \lim_{n \to \infty} u_n(g) & \text{pour } g \in \Omega_0 \\
0 & \text{pour } g \in \Omega - \Omega_0.
\end{cases}
$$

Comme $u_n(g)$ et $g$ coïncident sur $D_m \subset D_n$ pour $0 \leq m \leq n$, il est immédiat que la restriction de $u(g)$ à $D$ est égale à $g$ pour tout $g \in \Omega_0$.

C) Construction d'une mesure gaussienne sur $\mathcal{C}$:

Soit $w'$ la mesure bornée sur $\mathcal{C}$, image de $m$ par l'application $m$-mesurable $u : \Omega \to \mathcal{C}$. Nous allons montrer que $w'$ est une mesure gaussienne sur $\mathcal{C}$, de variance $W$, d'où $w = w'$. On notera $\mathcal{D}$ le sous-espace vectoriel de $\mathcal{M}^1$ engendré par les mesures $\varepsilon_t$ pour $t$ parcourant $D$.

#### Lemme 5 {#int-ix-s6-lem-5 .statement}

Pour toute mesure $\mu \in \mathcal{D}$, on a

(48)
$$
\int_\mathcal{C} e^{i\langle f, \mu \rangle} dw'(f) = e^{-W(\mu)/2}.
$$

Posons $\mu = c_1 \varepsilon_{t_1} + c_2 \varepsilon_{t_2} + \cdots + c_n \varepsilon_{t_n}$ avec $t_1, \ldots, t_n$ dans $D$ et $c_1, \ldots, c_n$ dans $\mathbf{R}$. Pour tout $g \in \Omega_0$, la fonction $u(g)$ coïncide avec $g$ sur $D$; on a donc

$$
\langle u(g), \mu \rangle = \sum_{j=1}^n c_j g(t_j) \quad (g \in \Omega_0).
$$

On a aussi

$$
W(\mu) = \sum_{j,k=1}^n c_j c_k \inf (t_j, t_k),
$$

et, comme $m$ est la mesure gaussienne sur $\Omega$ de covariance $M$, et que $\Omega - \Omega_0$ est $m$-négligeable, on a

$$
\int_{\Omega_0} e^{i \sum_{j=1}^n c_j g(t_j)} dm(g) = \exp \left( -\frac{1}{2} \sum_{j,k=1}^n c_j c_k \inf (t_j, t_k) \right).
$$

Or, $\Omega - \Omega_0$ est $m$-négligeable et l’on a $w' = u(m)$; on en déduit

$$
\int_{\mathcal{C}} e^{i \langle f, \mu \rangle} d\omega'(f) = \int_{\Omega_0} e^{i \langle u(g), \mu \rangle} dm(g).
$$

La formule (48) résulte immédiatement des formules (49) à (52).

#### Lemme 6 {#int-ix-s6-lem-6 .statement}

*Soit $\mu \in \mathcal{M}^1$. Il existe une suite de mesures $\mu_n \in \mathcal{D}$ telles que $\mu(f) = \lim_{n \to \infty} \mu_n(f)$ pour tout $f \in \mathcal{C}$ et $W(\mu) = \lim_{n \to \infty} W(\mu_n)$.*

Soit $I = (0, 1]$. L’espace $\mathcal{M}^1$ des mesures bornées sur $T = ]0, 1]$ sera identifié au sous-espace de $\mathcal{M}(I)$ formé des mesures qui ne chargent pas 0. On munit $\mathcal{M}(I)$ de la topologie vague. L’application $t \mapsto \varepsilon_t$ de $I$ dans $\mathcal{M}(I)$ est continue (chap. III, 2e éd., § 1, n° 9, prop. 13); comme $D$ est dense dans $I$, l’adhérence $\overline{\mathcal{D}}$ de $\mathcal{D}$ contient toutes les mesures ponctuelles. Soit $A$ l’ensemble des mesures $v \in \mathcal{D}$ telles que $\|v\| \leq \|u\|$; la mesure $\mu$ est adhérente à $A$ (chap. III, 2e éd., § 2, n° 4, cor. 1 du th. 1). L’ensemble $A$ est relativement compact dans $\mathcal{M}(I)$ (chap. III, 2e éd., § 1, n° 9, prop. 15) et les parties compactes de $\mathcal{M}(I)$ sont métrisables (*Esp. vect. top.*, chap. IV, § 5, n° 1, prop. 2, et *Top. gén.*, chap. X, 2e éd, § 3, n° 3, th. 1). Il existe donc une suite de mesures $\mu_n \in A$ convergeant vers $\mu$ dans $\mathcal{M}(I)$. Comme $\mathcal{C}$ est identifié au sous-espace des fonctions continues sur $I$ nulles à l’origine, on a $\mu(f) = \lim_{n \to \infty} \mu_n(f)$ pour tout $f \in \mathcal{C}$. Par ailleurs, comme $\mathcal{C}(I) \otimes \mathcal{C}(I)$ est dense dans l’espace normé $\mathcal{C}(I \times I)$ (chap. III, 2e éd., § 4, n° 1, lemme 1), les relations $\lim_{n \to \infty} \mu_n = \mu$ et $\|\mu_n\| \leq \|\mu\|$ entraînent $\lim_{n \to \infty} (\mu_n \otimes \mu_n) = \mu \otimes \mu$ (chap. III, 2e éd., § 1, n° 10, prop. 17); comme les mesures $\mu_n$ et $\mu$ ne chargent pas 0, on a

$$
W(\mu_n) = \int_I \int_I \inf (t, t') \, d\mu_n(t) \, d\mu_n(t')
$$

$$
W(\mu) = \int_I \int_I \inf (t, t') \, d\mu(t) \, d\mu(t'),
$$

d'où $\lim_{n \to \infty} W(\mu_n) = W(\mu)$.

Il reste à prouver que la transformée de Fourier de $w'$ est égale à $e^{-W/2}$. Soit $\mu \in \mathcal{M}^1$; choisissons les mesures $\mu_n \in \mathcal{D}$ comme dans le lemme 6. La mesure $w'$ est bornée et l'on a $|e^{i\langle f, \mu_n \rangle}| = 1$ pour tout $n$; le lemme 5 et le théorème de convergence de Lebesgue (chap. IV, 2e éd., § 4, n° 3, th. 2) entraînent alors

$$
\int_\mathcal{C} e^{i\langle f, \mu \rangle} \, dw'(f) = \lim_{n \to \infty} \int_\mathcal{C} e^{i\langle f, \mu_n \rangle} \, dw'(f)
$$
$$
= \lim_{n \to \infty} e^{-W(\mu_n)/2} = e^{-W(\mu)/2}.
$$

C.Q.F.D.

La mesure $w$ sur $\mathcal{C}$, dont la transformée de Fourier est égale à $e^{-W/2}$ s'appelle la mesure de Wiener sur $\mathcal{C}$.

#### Remarque {#int-ix-s6-n7-rem-1 .statement}

Pour tout intervalle semi-ouvert $J = ]a, b]$ contenu dans $T$, posons $l(J) = b - a$ (longueur de $J$) et notons $A_J$ la forme linéaire $f \mapsto f(b) - f(a)$ sur $\mathcal{C}$. On peut montrer que la mesure de Wiener est caractérisée par la propriété suivante:
Soient $J_1, \ldots, J_n$ des intervalles semi-ouverts contenus dans $T$ et deux à deux disjoints. L'image de la mesure $w$ par l'application linéaire $f \mapsto (A_{J_1}(f), \ldots, A_{J_n}(f))$ de $\mathcal{C}$ dans $\mathbf{R}^n$ est égale à $\gamma_{a_1} \otimes \cdots \otimes \gamma_{a_n}$ avec $a_i = l(J_i)^{1/2}$ pour $1 \leq i \leq n$.

### 8. Continuité de la transformée de Fourier

#### Proposition 8 {#int-ix-s6-prop-8 .statement}

Soient $E$ un espace localement convexe, $\mu$ une promesure sur $E$ et $\Phi$ la transformée de Fourier de $\mu$. On a les inégalités

(53) $$ |\Phi(x')| \leq \Phi(0) $$
(54) $$ |\Phi(x') - \Phi(y')|^2 \leq 2\Phi(0)(\Phi(0) - \Re \Phi(x' - y')) $$

pour $x', y'$ dans $E'$.

La formule (5) du n° 3 permet de se ramener au cas où $E$ est de dimension finie et où $\mu$ est une mesure. On a

$$ |\Phi(x')| = \left| \int_E e^{i\langle x, x' \rangle} \, d\mu(x) \right| \leq \int_E |e^{i\langle x, x' \rangle}| \, d\mu(x) = \int_E d\mu(x) = \Phi(0), $$

d'où (53). De plus, si $a$ et $b$ sont des nombres réels, on a

$$ |e^{ia} - e^{ib}|^2 = |e^{ib}|^2 |e^{i(a-b)} - 1|^2 = (e^{i(a-b)} - 1)(e^{-i(a-b)} - 1) = 2 - 2 \cos (a - b); $$

d’après l’inégalité de Cauchy–Schwarz, on a alors

$$
|\Phi(x') - \Phi(y')|^2 = \left| \int_E (e^{i\langle x, x' \rangle} - e^{i\langle x, y' \rangle})\, d\mu(x) \right|^2
$$
$$
\leq \int_E |e^{i\langle x, x' \rangle} - e^{i\langle x, y' \rangle}|^2\, d\mu(x) \int_E 1^2\, d\mu(x)
$$
$$
= \int_E (2 - 2 \cos \langle x, x' - y' \rangle)\, d\mu(x) \cdot \Phi(0)
$$
$$
= 2 \Phi(0)(\Phi(0) - \Re \Phi(x' - y')),
$$
d’où (54).

#### Corollaire {#int-ix-s6-n8-cor-1 .statement}

Munissons E’ d’une topologie compatible avec sa structure d’espace vectoriel. Pour que $\Phi$ soit continue, il faut et il suffit que sa partie réelle $\Re \Phi$ soit continue à l’origine, et alors $\Phi$ est uniformément continue.
Cela résulte de l’inégalité (54).

Soit F un espace localement convexe. On munit le dual F’ de F d’une topologie compatible avec la dualité entre F et F’ et l’on identifie F au dual de F’. Par suite, la transformée de Fourier d’une mesure bornée $\mu$ sur F’ est la fonction $\mathcal{F} \mu$ sur F définie par

$$
(\mathcal{F} \mu)(x) = \int_{F'} e^{i\langle x, x' \rangle}\, d\mu(x').
$$

#### Proposition 9 {#int-ix-s6-prop-9 .statement}

Si F est tonnelé, la transformée de Fourier de toute mesure bornée sur F’ est une fonction uniformément continue sur F.
Soient $\mu$ une mesure bornée sur F’ et $\Phi$ sa transformée de Fourier. Soit $\varepsilon > 0$. Il existe une partie compacte K de F’ tel que $\mu(F' - K) \leq \varepsilon$. Or K est compact pour la topologie faible $\sigma(F', F)$, donc équicontinu car F est tonnelé (Esp. vect. top., chap. IV, § 2, n° 2, th. 1). Il existe donc un voisinage symétrique U de 0 dans F dont le polaire $U^0$ contient K. Soit $x$ dans $\varepsilon U$; on a

$$
\Phi(0) - \Re \Phi(x) = \int_{F'} (1 - \cos \langle x, x' \rangle)\, d\mu(x').
$$

Or on a $0 \leq 1 - \cos \langle x, x' \rangle \leq 2$ pour tout $x' \in F' - K$ et

$$
1 - \cos \langle x, x' \rangle \leq \frac{1}{2} \langle x, x' \rangle^2 \leq \frac{\varepsilon^2}{2}
$$

pour $x' \in K \subset U^0$; on en déduit

$$
0 \leq \Phi(0) - \Re \Phi(x) \leq 2 \mu(F' - K) + \frac{\varepsilon^2}{2} \mu(K) \leq 2 \varepsilon + \frac{\varepsilon^2}{2} \mu(F').
$$

Le second membre de cette inégalité tend vers 0 avec $\varepsilon$; donc $\Re \Phi$ est continue en 0 et la prop. résulte du cor. de la prop. 8.

### 9. Le lemme de Minlos

Soient T un espace vectoriel de dimension finie et $\mu$ une mesure bornée sur $T'$; nous identifions T au dual de $T'$ de sorte que la transformée de Fourier $\Phi$ de $\mu$ est une fonction sur T. On suppose données deux formes quadratiques positives h et q sur T et un nombre $\varepsilon > 0$. Pour tout nombre réel $r > 0$, on note $C_r$ l’ensemble des $x' \in T'$ tels que l’on ait $\langle x, x' \rangle^2 \leq r^2 h(x)$ pour tout $x \in T$.

#### Proposition 10 {#int-ix-s6-prop-10 .statement}

Sous l’hypothèse $\Phi(0) - \mathcal{R}\Phi \leq \varepsilon + q$, on a
$$
\mu(T' - C_r) \leq 3(\varepsilon + r^{-2} \operatorname{Tr}(q/h))
$$
pour tout $r > 0$.

On a noté $\operatorname{Tr}(q/h)$ la trace de q par rapport à h (cf. Annexe, n° 1). La formule (55) est triviale lorsque $\operatorname{Tr}(q/h)$ est infini. Nous supposons désormais $\operatorname{Tr}(q/h)$ fini, donc que $h(x) = 0$ entraîne $q(x) = 0$ pour tout $x \in T$.

Soient $a_1, \ldots, a_n$ des éléments de T, et D l’ensemble des $x' \in T'$ tels que
$$
\sum_{j=1}^n \langle a_j, x' \rangle^2 > 1.
$$
Pour tout $t$ réel $\geq 0$, on a $3(1 - e^{-t/2}) \geq 0$ et l’on a même
$$
3(1 - e^{-t/2}) \geq 3(1 - e^{-1/2}) \geq 3(1 - (\frac{9}{4})^{-1/2}) = 1
$$
pour $t > 1$, car $e > \frac{9}{4}$. Appliquant ces inégalités à $t = \sum_{j=1}^n \langle a_j, x' \rangle^2$, on obtient
$$
\mu(D) \leq 3 \int_{T'} \left( 1 - \exp \left( -\frac{1}{2} \sum_{j=1}^n \langle a_j, x' \rangle^2 \right) \right) d\mu(x').
$$

Soit $\gamma$ la mesure sur $\mathbf{R}$, de densité $t \mapsto (2\pi)^{-1/2} e^{-t^2/2}$ par rapport à la mesure de Lebesgue. D’après le lemme 2 du n° 4, on a
$$
\int_{\mathbf{R}} e^{iut} d\gamma(t) = e^{-u^2/2}
$$
pour tout $u$ réel. Par suite, on a
$$
1 - \exp \left( -\frac{1}{2} \sum_{j=1}^n \langle a_j, x' \rangle^2 \right) = \int \ldots \int \left( 1 - e^{i \sum_{j=1}^n \langle a_j, x' \rangle t_j} \right) d\gamma(t_1) \ldots d\gamma(t_n)
$$
pour tout $x' \in T'$. La fonction de $x', t_1, \ldots, t_n$ à intégrer au second membre est continue et majorée en module par 2, et les mesures $\mu$ et $\gamma$ sont bornées; on peut donc intégrer les deux membres de (57) par rapport à $d\mu(x')$ et interchanger les intégrations par rapport à $\mu$ et $\gamma$; on obtient
$$
\int_{T'} \left( 1 - \exp \left( -\frac{1}{2} \sum_{j=1}^n \langle a_j, x' \rangle^2 \right) \right) d\mu(x')
$$
$$
= \int \ldots \int \left( \Phi(0) - \Phi \left( \sum_{j=1}^n t_j a_j \right) \right) d\gamma(t_1) \ldots d\gamma(t_n).
$$

Comme $q$ est une forme quadratique sur $T$, il existe des nombres réels $q_{jk}$ tels que

$$
q \left( \sum_{j=1}^n t_j a_j \right) = \sum_{j,k} q_{jk} t_j t_k
$$

pour $t_1, \ldots, t_n$ réels; on a en particulier $q_{jj} = q(a_j)$ pour $1 \leq j \leq n$. Par ailleurs, l’intégrale $\int_{\mathbf{R}} t^n d\gamma(t)$ vaut respectivement 1, 0, 1 pour $n = 0, 1, 2$ (n° 4, lemme 1). On en déduit immédiatement

$$
\int \cdots \int \left( \varepsilon + q \left( \sum_{j=1}^n t_j a_j \right) \right) d\gamma(t_1) \ldots d\gamma(t_n) = \varepsilon + \sum_{j=1}^n q(a_j).
$$

Or, le premier membre de (58) et $\Phi(0)$ sont des nombres réels; on peut donc remplacer $\Phi$ par $\Re \Phi$ au second membre de (58). L’inégalité $\Phi(0) - \Re \Phi \leq \varepsilon + q$ et les formules (56), (58) et (59) entraînent alors

$$
\mu(D) \leq 3 \left( \varepsilon + \sum_{j=1}^n q(a_j) \right).
$$

Fixons le nombre $r > 0$. Comme la forme quadratique $h$ est positive, il existe une base $(e_1, \ldots, e_n)$ de $T$ et un entier $m$ compris entre 0 et $n$ tels que

$$
h \left( \sum_{j=1}^n t_j e_j \right) = \sum_{j=1}^m t_j^2,
$$

pour $t_1, \ldots, t_n$ réels (Annexe, n° 1, prop. 2). Il est alors immédiat que $C_r$ se compose des $x' \in T'$ tels que

$$
\sum_{j=1}^m \langle e_j, x' \rangle^2 \leq r^2, \qquad \sum_{j=m+1}^n \langle e_j, x' \rangle^2 = 0.
$$

Pour tout entier $l \geq 1$, soit $D_l$ l’ensemble des $x' \in T'$ satisfaisant à l’inégalité

$$
\sum_{j=1}^m \langle r^{-1} e_j, x' \rangle^2 + \sum_{j=m+1}^n \langle l e_j, x' \rangle^2 > 1.
$$

On voit facilement que la suite $(D_l)_{l \geq 1}$ est croissante de réunion $T' - C_r$, d’où

$$
\mu(T' - C_r) = \lim_{l \to \infty} \mu(D_l).
$$

Mais d’après (60), on a

$$
\mu(D_l) \leq 3 \left( \varepsilon + \sum_{j=1}^m r^{-2} q(e_j) + \sum_{j=m+1}^n l^2 q(e_j) \right);
$$

pour $j = m+1, \ldots, n$, on a $h(e_j) = 0$, donc $q(e_j) = 0$. De plus, on a $\mathrm{Tr}(q/h) = \sum_{j=1}^m q(e_j)$ (Annexe, n° 1, prop. 2). La relation (55) résulte alors de (61) et (62).

C.Q.F.D

### 10. Mesures sur le dual d’un espace nucléaire

Soit F un espace localement convexe. Soit $\mathcal{T}_s$ la topologie faible $\sigma(F', F)$ sur $F'$ et $\mathcal{T}_c$ la topologie de la convergence uniforme sur les parties compactes convexes de F. D’après le théorème de Mackey, (*Esp. vect. top.*, chap. IV, § 2, n° 3, th. 2) les topologies $\mathcal{T}_s$ et $\mathcal{T}_c$ sur $F'$ sont compatibles avec la dualité entre F et $F'$; il en est donc de même de toute topologie localement convexe $\mathcal{T}$ sur $F'$ intermédiaire entre $\mathcal{T}_s$ et $\mathcal{T}_c$. Si $\mathcal{T}$ est une telle topologie, et si $F'_\mathcal{T}$ désigne l’espace $F'$ muni de $\mathcal{T}$, on identifiera F au dual de $F'_\mathcal{T}$. Les promesures sur $F'$ sont donc les mêmes pour toutes les topologies $\mathcal{T}$ du type précédent, et si $\mu$ est une telle promesure, sa transformée de Fourier est une fonction sur F.

On appelle *topologie de Sazonov* sur F la topologie localement convexe $\mathcal{S}$ définie par les semi-normes continues N satisfaisant à la condition suivante: $N^2$ *est une forme quadratique positive sur F et il existe une forme quadratique positive continue H sur F telle que* $\mathrm{Tr}(N^2/H) < +\infty$. La topologie $\mathcal{S}$ est moins fine que la topologie donnée sur F; on dit que F est *nucléaire* si ces topologies sont identiques. Cette classe d’espaces sera étudiée plus tard en détail.

**Théorème 2** (Minlos). — *Soient F un espace localement convexe, $\mathcal{T}$ une topologie localement convexe sur $F'$ intermédiaire entre $\mathcal{T}_s$ et $\mathcal{T}_c$ et $\mu$ une promesure sur $F'_\mathcal{T}$. On suppose que transformée de Fourier $\Phi$ de $\mu$ est continue sur F pour la topologie de Sazonov. Alors $\mu$ est une mesure sur $F'_\mathcal{T}$*.

Soit $\varepsilon > 0$. Comme $\Phi$ est continue pour la topologie de Sazonov de F, il existe deux formes quadratiques positives continues Q et H sur F, telles que $\mathrm{Tr}(Q/H) < +\infty$ et que l’on ait
$$
\Phi(0) - \Re \Phi(x) \leq \varepsilon/6
$$
pour tout $x \in F$ tel que $Q(x) \leq 1$. D’après la prop. 8 du n° 8, on a $|\Re \Phi(x)| \leq \Phi(0)$ pour tout $x \in F$, d’où
$$
\Phi(0) - \Re \Phi(x) \leq \varepsilon/6 + 2\Phi(0)Q(x)
$$
pour tout $x \in F$.

Posons $r = (12\Phi(0)\ \mathrm{Tr}(Q/H)\varepsilon^{-1})^{1/2}$ et notons K l’ensemble des $x' \in F'_\mathcal{T}$ tels que $\langle x, x' \rangle^2 \leq r^2H(x)$ pour tout $x \in F$. Comme $H^{1/2}$ est une semi-norme continue sur F, l’ensemble K est équicontinu et fermé dans $F'_\mathcal{T}$; il est donc compact dans $F'_\mathcal{T}$ d’après le théorème d’Ascoli (*Top. gén.*, chap. X, 2e éd., § 2, n° 5, cor. 1 du th. 2).

Soit V un sous-espace vectoriel fermé de codimension finie de $F'_\mathcal{T}$; alors, V est l’orthogonal d’un sous-espace vectoriel T de dimension finie de F. Soit $\mu_V$ la mesure sur T’ image de la promesure $\mu$ sur $F'_\mathcal{T}$ par l’application $p_V$ transposée de l’injection canonique de T dans F; sa transformée de Fourier est la restriction de $\Phi$ à T. Enfin, d’après le théorème de Hahn–Banach (*Esp. vect. top.*, chap. II, 2e éd., § 3, n° 2, cor. 1 du th. 1), $p_V(K)$ est égal à l’ensemble $C_r$ des $x' \in T'$ tels que $\langle x, x' \rangle^2 \leq r^2 H(x)$ pour tout $x \in T$. D’après l’inégalité (63), on peut appliquer la prop. 10 du n° 9 à la mesure $\mu_v$ sur $T'$, en prenant pour $q$ la restriction de $2\Phi(0)Q$ à $T$ et pour $h$ celle de $H$. On a $\mathrm{Tr}(q/h) \leq 2\Phi(0)\mathrm{Tr}(Q/H)$, d’où

$$
\mu_v(T' - C_r) \leq 3 \left( \frac{\varepsilon}{6} + 2\Phi(0)\mathrm{Tr}(Q/H)r^{-2} \right) = \varepsilon.
$$

Comme $p_v$ définit par passage au quotient un isomorphisme de $F_{\mathcal{T}}'/V$ sur $T'$, la prop. 1 du n° 1 montre alors que $\mu$ est une mesure sur $F_{\mathcal{T}}'$.

C.Q.F.D.

#### Corollaire {#int-ix-s6-n10-cor-1 .statement}

Soient $F$ un espace nucléaire tonnelé, $\mathcal{T}$ une topologie localement convexe intermédiaire entre $\mathcal{T}_s$ et $\mathcal{T}_c$ sur $F'$, $\mu$ une promesure sur $F_{\mathcal{T}}'$ et $\Phi$ la transformée de Fourier de $\mu$. Pour que $\mu$ soit une mesure, il faut et il suffit que $\Phi$ soit continue sur $F$.

La nécessité résulte de la prop. 9 du n° 8 et la suffisance du th. 2.

#### Remarque {#int-ix-s6-n10-rem-1 .statement}

Soient $F$ un espace tonnelé et $\mathcal{T}$ une topologie localement convexe sur $F'$ intermédiaire entre $\mathcal{T}_s$ et $\mathcal{T}_c$. Toute partie de $F'$ compacte pour $\mathcal{T}$ est compacte pour la topologie moins fine $\mathcal{T}_s$. Réciproquement, soit $K$ une partie de $F'$ compacte pour $\mathcal{T}_s$. Comme $F$ est tonnelé, $K$ est équicontinue ($Esp.\ vect.\ top.$, chap. IV, § 2, n° 2, th. 1); mais d’après le théorème d’Ascoli, toute partie équicontinue de $F'$ est relativement compacte pour $\mathcal{T}_c$ et $a fortiori$ pour $\mathcal{T}$, donc $K$ est contenu dans une partie de $F'$ compacte pour $\mathcal{T}$. Il n’est pas difficile d’en conclure que l’application identique de $F_{\mathcal{T}}'$ sur $F_{\mathcal{T}_s}'$ définit une bijection entre les ensembles de mesures de ces deux espaces.

### 11. Mesures sur un espace de Hilbert

Soit $E$ un espace hilbertien réel, dans lequel le produit scalaire est noté $(x|y)$. Il existe un isomorphisme $j$ de $E$ sur son dual $E'$, caractérisé par la formule $\langle x, j(y) \rangle = (x|y)$ pour $x, y$ dans $E$ ($Esp.\ vect.\ top.$, chap. V, § 1, n° 6, th. 3). Nous identifierons $E$ et $E'$ au moyen de $j$. La transformée de Fourier d’une promesure $\mu$ sur $E$ est donc une fonction $\mathcal{F}\mu$ sur $E$; lorsque $\mu$ est une mesure, on a

$$
(\mathcal{F}\mu)(x) = \int_E e^{i(x|y)}\,d\mu(y) \qquad (x \in E).
$$

#### Théorème 3 (Prokhorov–Sazonov) {#int-ix-s6-thm-3 .statement}

Soient $E$ un espace hilbertien et $E_s$ l’espace $E$ muni de la topologie affaiblie. Soient $\mu$ une promesure sur $E$ et $\Phi$ sa transformée de Fourier. Les conditions suivantes sont équivalentes:

a) La fonction $\Phi$ est continue sur $E$ pour la topologie de Sazonov.
b) Pour tout $\varepsilon > 0$, il existe une forme quadratique positive nucléaire $Q$ sur $E$ telle que $\Phi(0) - \Re \Phi \leq \varepsilon + Q$.
c) La promesure $\mu$ est une mesure sur $E_s$.
b) $\Rightarrow a)$: cela résulte de la prop. 8 du n° 8 (cf. inégalité (54)).
a) $\Rightarrow c)$: cela résulte du théorème 2 du n° 10.

c) $\Rightarrow b)$: supposons que $\mu$ soit une mesure sur $E_s$. Soit $\varepsilon > 0$. Pour tout entier $n \geqslant 1$, l’ensemble $B_n$ des $x \in E$ de norme $\leqslant n$ est une partie fermée de $E_s$ et l’on a $E = \bigcup_{n \geqslant 1} B_n$. Il existe donc un entier $n \geqslant 1$ tel que $\mu(E - B_n) < \frac{\varepsilon}{2}$. La formule
$$
(65) \quad Q(x) = \frac{1}{2} \int_{B_n} (x|y)^2 \, d\mu(y)
$$
définit une forme quadratique positive $Q$ sur $E$. Posons $C = \frac{n^2}{2} \mu(B_n)$. Si $(e_1, \ldots, e_p)$ est une suite orthonormale finie dans $E$, on a
$$
\sum_{j=1}^p (e_j|y)^2 \leq \|y\|^2 \leq n^2
$$
pour tout $y \in B_n$ d’après l’inégalité de Bessel. Par intégration, on en déduit
$$
\sum_{j=1}^p Q(e_j) = \frac{1}{2} \int_{B_n} \sum_{j=1}^p (e_j|y)^2 \, d\mu(y) \leq \frac{n^2}{2} \mu(B_n) = C,
$$
donc $Q$ est nucléaire.

Par ailleurs, on a $1 - \cos t \leq \inf \left(2, \frac{t^2}{2}\right)$ pour tout nombre réel $t$, d’où
$$
\Phi(0) - \mathcal{R}\Phi(x) = \int_E (1 - \cos (x|y)) \, d\mu(y)
$$
$$
\leq \int_{B_n} \frac{1}{2} (x|y)^2 \, d\mu(y) + \int_{E - B_n} 2 \, d\mu(y)
$$
$$
= Q(x) + \varepsilon
$$
pour tout $x \in E$. Donc b) est vérifiée.

C.Q.F.D.

#### Corollaire 1 {#int-ix-s6-thm-3-cor-1 .statement}

Soient $E_1$ et $E_2$ deux espaces de Hilbert, $u$ une application de Hilbert–Schmidt de $E_1$ dans $E_2$ et $\mu$ une promesure sur $E_1$. On suppose que la transformée de Fourier $\Phi$ de $\mu$ est continue sur $E_1$. Alors la promesure $\nu = u(\mu)$ est une mesure sur $E_2$ muni de la topologie faible.

Avec les identifications de $E_1$ et $E_2$ à leurs duals introduites dans ce n°, la transformée de Fourier de $\nu$ est égale à $\Phi \circ u^*$ où $u^*$ est l’adjointe de $u$. Or $u^*$ est une application de Hilbert–Schmidt de $E_2$ dans $E_1$ (Annexe, n° 2), et la forme quadratique $y \mapsto \|u^*(y)\|^2$ sur $E_2$ est donc nucléaire. Si $(E_2)_\mathscr{S}$ désigne $E_2$ muni de la topologie de Sazonov, $u^*$ est donc une application linéaire continue de $(E_2)_\mathscr{S}$ dans $E_1$ et $\mathcal{F}_\nu = \Phi \circ u^*$ est continue sur $(E_2)_\mathscr{S}$; le théorème 3 montre alors que $\nu$ est une mesure sur l’espace $E_2$ muni de la topologie faible.

#### Corollaire 2 {#int-ix-s6-thm-3-cor-2 .statement}

Soit Q une forme quadratique positive nucléaire sur l’espace hilbertien E. La promesure gaussienne $\Gamma_Q$ de variance Q sur E est une mesure sur $E_s$.

La transformée de Fourier $\Phi$ de $\Gamma_Q$ est égale à $e^{-Q/2}$. Or on a $e^t \geq 1 + t$ pour tout nombre réel $t$, d’où $\Phi(0) - \Re \Phi \leq Q/2$. La condition b) du théorème 3 est donc vérifiée et $\Gamma_Q$ est une mesure sur $E_s$.

#### Remarque 1 {#int-ix-s6-n11-rem-1 .statement}

Soient E un espace hilbertien, $E_s$ l’espace E muni de la topologie faible et $j$ l’application identique de E dans $E_s$. On sait que $j$ définit une bijection de l’ensemble des promesures sur E sur l’ensemble correspondant pour $E_s$. Par ailleurs, si E est de type dénombrable, c’est un espace polonais et $j$ définit une bijection de l’ensemble des mesures bornées sur E sur l’ensemble des mesures bornées sur $E_s$ (§ 3, n° 3, Remarque); on peut montrer (théorème de Phillips) que ce théorème subsiste si E n’est pas de type dénombrable. Par suite, le théorème 3 fournit des critères pour qu’une promesure sur E soit une mesure.

#### Remarque 2 {#int-ix-s6-n11-rem-2 .statement}

On peut montrer (Annexe, exerc. 7b) que la topologie de Sazonov sur un espace hilbertien E est définie par les semi-normes du type $Q^{1/2}$ où Q est une forme quadratique positive nucléaire sur E.

*12. Relations avec les fonctions de type positif

#### Définition 3 {#int-ix-s6-def-3 .statement}

Soit G un groupe. On dit qu’une fonction $\Phi$ sur G à valeurs complexes est de type positif si l’on a les inégalités

$$
\sum_{j,k=1}^p c_j \overline{c_k} \Phi(x_j x_k^{-1}) \geq 0
$$

quels que soient $x_1, \ldots, x_p$ dans G et les nombres complexes $c_1, \ldots, c_p$.

Cette notion sera étudiée en détail plus tard.

#### Proposition 11 {#int-ix-s6-prop-11 .statement}

Soient E un espace vectoriel de dimension finie, $\mu$ une mesure (positive) bornée sur E et $\Phi$ la transformée de Fourier de $\mu$. La fonction $\Phi$ est continue et de type positif sur $E'$.

La continuité de $\Phi$ résulte de la prop. 9 du n° 8.

Montrons que $\Phi$ est de type positif. Soient $x'_1, \ldots, x'_p$ dans $E'$ et $c_1, \ldots, c_p$ des nombres complexes. On a

$$
\sum_{j,k} c_j \overline{c_k} \Phi(x'_j - x'_k) = \int_E \sum_{j,k} c_j \overline{c_k} e^{i \langle x, x'_j - x'_k \rangle} d\mu(x)
$$
$$
= \int_E \left| \sum_{j=1}^p c_j e^{i \langle x, x'_j \rangle} \right|^2 d\mu(x) \geq 0.
$$

C.Q.F.D.

On peut démontrer une réciproque connue sous le nom de théorème de Bochner: toute fonction continue de type positif sur $E'$ est la transformée de Fourier d’une mesure (positive) bornée (1). Nous admettrons ce résultat dans la suite du n° 12.

(1) Cette question sera étudiée dans un chapitre à paraître du Livre de Théories Spectrales. Le lecteur pourra se reporter à ce sujet à LOOMIS, Abstract Harmonic Analysis, van Nostrand, New-York, 1953.

#### Théorème 4 {#int-ix-s6-thm-4 .statement}

Soit E un espace localement convexe. La transformation de Fourier est une bijection de l’ensemble des promesures sur E sur l’ensemble des fonctions de type positif sur E’ dont la restriction à tout sous-espace de dimension finie est continue.

On sait (n° 3, prop. 3) que la transformation de Fourier est injective. Soient $\mu = (\mu_V)_{V \in \mathcal{F}(E)}$ une promesure sur E et $\Phi$ sa transformée de Fourier. Soit T un sous-espace de dimension finie de E’ et soit V l’orthogonal de T dans E. On peut identifier T au dual de E/V ; la restriction $\Phi_T$ de $\Phi$ à T est la transformée de Fourier de la mesure bornée $\mu_V$ sur E/V. D’après la prop. 11, $\Phi_T$ est continue et de type positif sur T. Vu l’arbitraire de T, il est clair que $\Phi$ est de type positif sur E’.

Réciproquement, soit $\Phi$ une fonction de type positif sur E’ dont la restriction à tout sous-espace de dimension finie de E soit continue. Pour tout $V \in \mathcal{F}(E)$, on identifie le dual de E/V à l’orthogonal $V^0$ de V dans E’ ; la restriction $\Phi_V$ de $\Phi$ à $V^0$ est continue et de type positif, et d’après le théorème de Bochner, il existe donc une mesure (positive) bornée $\mu_V$ sur E/V dont la transformée de Fourier soit $\Phi_V$. Soient V et W dans $\mathcal{F}(E)$ avec $W \subset V$, et soit $p_{VW}$ l’application canonique de E/W sur E/V ; avec les identifications faites, $t p_{VW}$ est l’injection de $V^0$ dans $W^0$. D’après la formule (4) du n° 3, on a alors

$$
\mathcal{F}(p_{VW}(\mu_W)) = (\mathcal{F}\mu_W) \circ t p_{VW} = \Phi_W \circ t p_{VW} = \Phi_V = \mathcal{F}\mu_V
$$

d’où $p_{VW}(\mu_W) = \mu_V$ d’après la prop. 3 du n° 3. Par suite, la famille $\mu = (\mu_V)_{V \in \mathcal{F}(E)}$ est une promesure sur E ; il est clair que $\Phi$ est la transformée de Fourier de $\mu$.

#### Corollaire {#int-ix-s6-n11-cor-1 .statement}

Soit F un espace nucléaire tonnelé ; on munit F’ d’une topologie localement convexe $\mathcal{T}$ intermédiaire entre la topologie faible $\sigma(F', F)$ et la topologie de la convergence uniforme sur les parties compactes et convexes de F. La transformation de Fourier est une bijection de l’ensemble des mesures (positives) bornées sur F’ sur l’ensemble des fonctions continues de type positif sur F.

Cela résulte immédiatement du th. 4 et du cor. du th. 2 du n° 10.*

## EXERCICES {#int-ix-s6-exercises}

See the [exercises for § 6](exercises/s6/).
