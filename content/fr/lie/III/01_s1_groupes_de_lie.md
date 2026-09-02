---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: GROUPES DE LIE
section: 1
section_title: Groupes de Lie
lang: fr
source: lie-ii-iii-fr
pdf_pages: 0093-0117, 0255-0256
extraction: ocr
subsections:
    - "no": 1
      title: Définition d’un groupe de Lie
      page: 0
      pdf_page: 93
    - "no": 2
      title: Morphismes de groupes de Lie
      page: 0
      pdf_page: 97
    - "no": 3
      title: Sous-groupes de Lie
      page: 0
      pdf_page: 98
    - "no": 4
      title: Produits semi-directs de groupes de Lie
      page: 0
      pdf_page: 99
    - "no": 5
      title: Quotient d’une variété par un groupe de Lie
      page: 0
      pdf_page: 101
    - "no": 6
      title: Espaces homogènes et groupes quotients
      page: 0
      pdf_page: 103
    - "no": 7
      title: Orbites
      page: 0
      pdf_page: 106
    - "no": 8
      title: Fibrés vectoriels à opérateurs
      page: 0
      pdf_page: 107
    - "no": 9
      title: Définition locale d’un groupe de Lie
      page: 0
      pdf_page: 110
    - "no": 10
      title: Groupuscules
      page: 0
      pdf_page: 112
    - "no": 11
      title: Morceaux de lois d’opération
      page: 0
      pdf_page: 116
statements: 57
exercises: 10
content_sha256: daf1e810cb10a82fd11c52aa27ac0e8805be34f3f67a8d8ba89c110c532e71df
---

## § 1. Groupes de Lie

### 1. Définition d’un groupe de Lie

Soit G un ensemble. Une structure de groupe et une structure de K-variété analytique sur G sont dites compatibles si la condition suivante est vérifiée:

(GL) L’application $(g, h) \mapsto gh^{-1}$ de $G \times G$ dans G est analytique.

#### Définition 1 {#lie-iii-s1-def-1 .statement}

On appelle groupe de Lie sur K un ensemble G muni d’une structure de groupe et d’une structure de K-variété analytique, ces deux structures étant compatibles.

Un groupe de Lie sur R (resp. C, Q_p) est appelé groupe de Lie réel (resp. complexe, p-adique).

Soit G un groupe muni d’une structure de variété analytique. Pour g, h, g_0, h_0 dans G, on a

$$
gh^{-1} = (g_0 h_0^{-1}) h_0 ((g_0^{-1} g)(h_0^{-1} h)^{-1}) h_0^{-1}.
$$

Il en résulte que G est un groupe de Lie si et seulement si les trois conditions suivantes sont vérifiées:

(GL_1) pour tout g_0 \in G, l’application g \mapsto g_0 g de G dans G est analytique;
(GL_2) pour tout g_0 \in G, l’application g \mapsto g_0 g g_0^{-1} de G dans G est analytique dans un voisinage ouvert de e;
(GL_3) l’application (g, h) \mapsto gh^{-1} de G \times G dans G est analytique dans un voisinage ouvert de (e, e).

Soit G un groupe de Lie. Pour tout g \in G, \gamma(g) et \delta(g) sont des automorphismes de la variété sous-jacente à G. Il en résulte que cette variété est pure (VAR, R, 5.1.7). En particulier, la dimension de G en g est égale à dim G pour tout g \in G (rappelons que dim G est un entier \geqslant 0 ou +\infty).

Puisqu’une application analytique est continue, un groupe de Lie est un groupe topologique pour la topologie sous-jacente à sa structure de variété. Soit G un ensemble. Une structure de groupe topologique et une structure de K-variété analytique sur G sont dites compatibles si la structure de groupe et la structure de variété sont compatibles, et si la topologie de G est la topologie sous-jacente à la structure de variété.

#### Lemme 1 {#lie-iii-s1-lem-1 .statement}

Soient G un groupe de Lie, U un voisinage ouvert de e, E un espace normé complet, \varphi : U \to E une carte de la variété G. Il existe un voisinage W de e contenu dans U tel que \varphi | W soit un isomorphisme de W (muni de la structure uniforme droite) sur \varphi(W) (muni de la structure uniforme induite par celle de E).

On peut supposer que \varphi(e) = 0. Soit U' = \varphi(U). Soit \psi : U' \to U l’application réciproque de \varphi. Soit V un voisinage ouvert symétrique de e tel que V^2 \subset U, et posons V' = \varphi(V). Définissons des applications \theta_1, \theta_2 de V' \times V' dans V' \times U' de la manière suivante:

$$
\theta_1(x, y) = (x, \varphi(\psi(x)\psi(y)^{-1}))
$$
$$
\theta_2(x, y) = (x, \varphi(\psi(y)^{-1}\psi(x))).
$$

On vérifie aussitôt que \theta_2(\theta_1(x, y)) = \theta_1(\theta_2(x, y)) = (x, y) pour x, y assez voisins de 0. D’autre part, \theta_1 et \theta_2 sont analytiques, donc strictement dérivables en (0, 0).

Par suite (VAR, R, 1.2.2) il existe un voisinage W' de 0 dans V' et des constantes $a > 0,\ b > 0$ telles que
$$
a (\| x_1 - x_2 \| + \| \varphi(\psi(x_1)\psi(y_1)^{-1}) - \varphi(\psi(x_2)\psi(y_2)^{-1}) \|)
\leq \| x_1 - x_2 \| + \| y_1 - y_2 \|
\leq b (\| x_1 - x_2 \| + \| \varphi(\psi(x_1)\psi(y_1)^{-1}) - \varphi(\psi(x_2)\psi(y_2)^{-1}) \|)
$$
quels que soient $x_1, x_2, y_1, y_2$ dans W'. Faisant $x_1 = x_2 = y_2$, il vient
$$(2)\quad a \| \varphi(\psi(x_1)\psi(y_1)^{-1}) \| \leq \| x_1 - y_1 \| \leq b \| \varphi(\psi(x_1)\psi(y_1)^{-1}) \|.$$
Pour $\delta > 0$, soit $N_\delta$ l’ensemble des couples $(x, y) \in W' \times W'$ tels que $\| x - y \| \leq \delta$. Les $N_\delta$ forment un système fondamental d’entourages dans $W'$. Posons $W = \psi(W')$. Soit $M_\delta$ l’ensemble des couples $(u, v) \in W \times W$ tels que $\| \varphi(uv^{-1}) \| \leq \delta$. Les $M_\delta$ forment un système fondamental d’entourages dans W pour la structure uniforme droite. Or la relation (2) prouve que
$$
N_\delta \subset (\varphi \times \varphi)(M_{a^{-1}\delta}), \quad (\varphi \times \varphi)(M_\delta) \subset N_{b\delta}
$$
donc W possède la propriété du lemme.

#### Proposition 1 {#lie-iii-s1-prop-1 .statement}

*Un groupe de Lie est un groupe topologique métrisable et complet.*
Puisque e admet un voisinage ouvert homéomorphe à une boule ouverte d’un espace normé, e admet un système fondamental dénombrable de voisinages dont l’intersection est $\{e\}$. Donc G est métrisable (TG, III, § 1, cor. de la prop. 2, et IX, § 3, prop. 1). D’après le lemme 1, il existe un voisinage de e qui est complet pour la structure uniforme droite, donc G est complet (TG, III, § 3, prop. 4).

#### Proposition 2 {#lie-iii-s1-prop-2 .statement}

*Soit G un groupe de Lie.*
(i) *Si K = \mathbf{R} ou \mathbf{C}, G est localement connexe.*
(ii) *Si K est distinct de \mathbf{R} et \mathbf{C}, G est éparpillé* (TG, IX, § 6, déf. 5).
(iii) *Supposons K localement compact. Pour que G soit localement compact, il faut et il suffit que G soit de dimension finie.*
(iv) *Si G est engendré par un sous-espace dont la topologie admet une base dénombrable, alors la topologie de G admet une base dénombrable.*
Soit U un voisinage de e. Il existe un voisinage ouvert $U_1$ de e contenu dans U et homéomorphe à une boule ouverte d’un espace normé E sur K. Si K = \mathbf{R} ou \mathbf{C}, $U_1$ est connexe, ce qui prouve (i). Supposons K ultramétrique. Il existe un voisinage $U_2$ de e fermé dans G et tel que $U_2 \subset U_1$. Puis il existe un voisinage $U_3$ de e tel que $U_3 \subset U_2$ et tel que $U_3$ soit ouvert et fermé relativement à $U_1$. Alors $U_3$ est fermé relativement à $U_2$, donc à G, et ouvert relativement à $U_1$, donc à G. Ceci prouve (ii). Pour que G soit localement compact, il faut et il suffit que E soit localement compact; si K est localement compact, cela revient à dire que E est de dimension finie (EVT, I, § 2, th. 3), d’où (iii). Supposons G engendré par un sous-ensemble V, et posons $W = V \cup V^{-1}$; on a $G = W \cup W^2 \cup W^3 \cup \cdots$; s’il existe une suite dense dans V, on voit qu’il existe une suite dense dans G, et, comme G est métrisable (prop. 1), la topologie de G admet une base dénombrable.

#### Corollaire {#lie-iii-s1-n1-cor-1 .statement}

Si K = R ou C, et si G est connexe de dimension finie, alors G est localement connexe, localement compact, et sa topologie admet une base dénombrable.

#### Lemme 2 {#lie-iii-s1-lem-2 .statement}

Soient X une variété de classe Cr, e un point de X, U et V des voisinages ouverts de e, et m une application de classe Cr de U × U dans X, vérifiant les conditions suivantes :

a) $m(e, x) = m(x, e) = x$ pour tout $x \in U$;
b) On a $V \subset V, m(V \times V) \subset U$ et $m(m(x, y), z) = m(x, m(y, z))$ quels que soient $x, y, z$ dans V.

Alors il existe un voisinage ouvert W de e dans V et un automorphisme $\theta$ de la variété W, tels que $\theta(e) = e, \theta(\theta(x)) = x$ et $m(x, \theta(x)) = m(\theta(x), x) = e$ pour tout $x \in W$.

On a $m(e, y) = y$ pour tout $y \in U$, donc, d’après le théorème des fonctions implicites, il existe un voisinage ouvert $W_1$ de e dans V et une application $\theta_1$ de classe Cr de $W_1$ dans V tels que $\theta_1(e) = e, m(x, \theta_1(x)) = e$ pour tout $x \in W_1$. De même, il existe un voisinage ouvert $W_2$ de e dans V et une application $\theta_2$ de classe Cr de $W_2$ dans V tels que $\theta_2(e) = e, m(\theta_2(x), x) = e$ pour tout $x \in W_2$. Pour $x \in W_1 \cap W_2$, on a
$$
\begin{align*}
\theta_2(x) &= m(\theta_2(x), e) = m(\theta_2(x), m(x, \theta_1(x))) \\
&= m(m(\theta_2(x), x), \theta_1(x)) = m(e, \theta_1(x)) = \theta_1(x).
\end{align*}
$$
Soit $\theta(x)$ la valeur commune de $\theta_1(x)$ et $\theta_2(x)$ pour $x \in W_1 \cap W_2$. Soit W l’ensemble des $x \in W_1 \cap W_2$ tels que $\theta(x) \in W_1 \cap W_2$. L’ensemble W est ouvert. Pour $x \in W$, on a
$$
\theta(\theta(x)) = m(m(x, \theta(x)), \theta(\theta(x))) = m(x, m(\theta(x), \theta(\theta(x)))) = m(x, e) = x,
$$
donc $\theta(x) \in W$. On voit que $\theta | W$ définit un automorphisme de la variété W.

#### Proposition 3 {#lie-iii-s1-prop-3 .statement}

Soient X une variété analytique, et m une loi de composition associative analytique sur X, admettant un élément neutre. L’ensemble G des éléments inversibles de X est ouvert dans X, et G est un groupe de Lie pour $m | (G \times G)$ et pour la structure de variété induite par celle de X.

D’après le lemme 2, G est un voisinage de l’élément neutre. Pour tout $g \in G$, l’application $x \mapsto m(g, x)$ est un automorphisme de la variété X. Donc l’image de G par cette application est un voisinage de g, évidemment contenu dans G. Par suite, G est ouvert dans X. Il est clair que les conditions (GL₁) et (GL₂) sont vérifiées. La condition (GL₃) est vérifiée d’après le lemme 2.

Exemples de groupes de Lie.

1. Soit E un espace normable complet sur K. L’application $(x, y) \mapsto x - y$ de $E \times E$ dans E est linéaire continue, donc analytique. Donc E, muni de ses structures de groupe additif et de variété analytique, est un groupe de Lie.
En particulier, K est un groupe de Lie.

Par exemple, soit E un espace normable complet sur K, et prenons $A = \mathcal{L}(E)$ (TG, IX, § 3, prop. 5). Alors $A^*$ est le groupe $\mathbf{GL}(E)$ des automorphismes de E. *Ce groupe est donc muni canoniquement d’une structure de groupe de Lie sur K.* Plus particulièrement, $\mathbf{GL}(n, K)$, muni de la structure de variété induite par celle de $\mathbf{M}_n(K)$, est un groupe de Lie. Pour $n = 1$, on voit que le groupe multiplicatif $K^*$ est un groupe de Lie pour la structure de variété induite par celle de K.

3. Soit G un groupe de Lie sur K. Soient $K' = \mathbf{R}$ ou $\mathbf{C}$ ou un corps ultramétrique complet non discret, et $\sigma$ un isomorphisme du corps valué $K'$ sur un sous-corps valué de K. Alors le groupe G, muni de la structure de $K'$-variété obtenue par restriction des scalaires, est un groupe de Lie sur $K'$, qui est dit *déduit du groupe de Lie G par restriction des scalaires* (de K à $K'$ au moyen de $\sigma$). Par exemple, tout groupe de Lie complexe est canoniquement muni d’une structure de groupe de Lie réel. Par exemple encore, à tout groupe de Lie complexe G est associé un groupe de Lie complexe appelé le *conjugué* de G, déduit de G au moyen de l’automorphisme $z \mapsto \bar{z}$ de $\mathbf{C}$.

### 2. Morphismes de groupes de Lie

#### Définition 2 {#lie-iii-s1-def-2 .statement}

*Soient G et H des groupes de Lie. On appelle morphisme de groupes de Lie de G dans H (ou simplement morphisme de G dans H si aucune confusion n’est à craindre) une application de G dans H qui est un homomorphisme de groupes et qui est analytique. Le groupe des automorphismes de G se note Aut(G).*

L’application identique de G est un morphisme. Le composé de deux morphismes est un morphisme. Si $f : G \to H$ et $f' : H \to G$ sont deux morphismes réciproques, $f$ et $f'$ sont des isomorphismes de groupes de Lie.

#### Exemple 1 {#lie-iii-s1-n2-exa-1 .statement}

Soit G un groupe de Lie. Pour tout $x \in G$, Int$(x)$ est un automorphisme du groupe de Lie G.

#### Exemple 2 {#lie-iii-s1-n2-exa-2 .statement}

Soit G un groupe de Lie. On note $G^\vee$ le groupe opposé à G, muni de la même structure de variété que G. Il est immédiat que $G^\vee$ est un groupe de Lie (dit groupe de Lie *opposé* à G), et que l’application $g \mapsto g^{-1}$ est un isomorphisme du groupe de Lie G sur le groupe de Lie $G^\vee$.

#### Exemple 3 {#lie-iii-s1-n2-exa-3 .statement}

Soient G un groupe de Lie, E un espace normable complet. On appelle *représentation linéaire analytique* de G dans E (ou simplement représentation linéaire de G dans E si aucune confusion n’est à craindre) un morphisme du groupe de Lie G dans le groupe de Lie $\mathbf{GL}(E)$, autrement dit une application analytique $\pi$ de G dans $\mathbf{GL}(E)$ telle que $\pi(gg') = \pi(g)\pi(g')$ pour $g, g'$ dans G. Supposons que E admette une base finie $(e_1, e_2, \ldots, e_n)$ sur $K$; soit $(e_1^*, e_2^*, \ldots, e_n^*)$ la base duale; soit $\rho$ un homomorphisme du groupe $G$ dans le groupe $\mathbf{GL}(E)$; alors les conditions suivantes sont équivalentes:

(i) $\rho$ est une représentation linéaire analytique;
(ii) quels que soient $x \in E$ et $x' \in E'$, la fonction $g \mapsto \langle \rho(g)x, x' \rangle$ sur $G$ est analytique;
(iii) quels que soient $i$ et $j$, la fonction $g \mapsto \langle \rho(g)e_i, e_j^* \rangle$ sur $G$ est analytique.
En effet, les implications (i) $\Rightarrow$ (ii) $\Rightarrow$ (iii) sont claires. D’autre part, les fonctions $u \mapsto \langle ue_i, e_j^* \rangle$ forment un système de coordonnées sur $\mathcal{L}(E)$; donc leurs restrictions à $\mathbf{GL}(E)$ forment un système de coordonnées sur $\mathbf{GL}(E)$, d’où l’implication (iii) $\Rightarrow$ (i).

Soient $G$ un groupe de Lie réel, $E$ un espace normable complet réel, $\rho$ un homomorphisme du groupe $G$ dans le groupe $\mathbf{GL}(E)$. On verra au § 8, th. 1, que, si $\rho$ est continu (lorsque $\mathbf{GL}(E)$ est muni de la topologie déduite de la norme de $\mathcal{L}(E)$), alors $\rho$ est analytique. Mais on prendra garde que cette notion de continuité est différente de celle considérée en INT, VIII, § 2, déf. 1 (ii) (exerc. 1).

#### Exemple 4 {#lie-iii-s1-n2-exa-4 .statement}

Soient $G$ un groupe de Lie réel, $E$ un espace normable complet *complexe*. Une *représentation linéaire analytique de G dans E* est un morphisme de $G$ dans le groupe de Lie réel sous-jacent à $\mathbf{GL}(E)$.

#### Proposition 4 {#lie-iii-s1-prop-4 .statement}

*Soient G et H des groupes de Lie, f un homomorphisme du groupe G dans le groupe H. Pour que f soit analytique, il faut et il suffit qu’il existe une partie ouverte non vide U de G telle que $f|U$ soit analytique.*

La condition est évidemment nécessaire. Supposons-la vérifiée. Pour tout $x_0 \in G$, on a $f(x_0x) = f(x_0)f(x)$ quel que soit $x \in U$, donc $f|x_0U$ est analytique. Or les ensembles $x_0U$, pour $x_0 \in G$, forment un recouvrement ouvert de $G$.

#### Remarque {#lie-iii-s1-n2-rem-1 .statement}

Si $f$ est une immersion en $e$ (resp. une submersion en $e$), il est clair que $f$ est une immersion (resp. une submersion).

### 3. Sous-groupes de Lie

Soient $G$ un groupe de Lie, $H$ un sous-groupe de $G$ qui est en même temps une sous-variété de $G$. Alors l’application $(x, y) \mapsto xy^{-1}$ de $H \times H$ dans $G$ est analytique, donc l’application $(x, y) \mapsto xy^{-1}$ de $H \times H$ dans $H$ est analytique (VAR, R, 5.8.5). Ainsi $H$, muni des structures de groupe et de variété induites par celles de $G$, est un groupe de Lie.

#### Définition 3 {#lie-iii-s1-def-3 .statement}

*Soit G un groupe de Lie. On dit qu’un sous-ensemble H de G est un sous-groupe de Lie si H est un sous-groupe et une sous-variété de G.*

Un sous-groupe ouvert de $G$ est un sous-groupe de Lie de $G$. En particulier, si $G$ est un groupe de Lie réel ou complexe, sa composante neutre est un sous-groupe de Lie de $G$.

#### Proposition 5 {#lie-iii-s1-prop-5 .statement}

Soient G un groupe de Lie, H un sous-groupe de Lie de G.
    (i) H est fermé dans G.
    (ii) L’injection canonique de H dans G est un morphisme de groupes de Lie.
    (iii) Soient L un groupe de Lie et f une application de L dans G telle que f(L) ⊂ H.
Pour que f soit un morphisme de L dans H, il faut et il suffit que f soit un morphisme de L dans G.
D’après VAR, R, 5.8.3, H est localement fermé. Donc H est fermé (TG, III, § 2, prop. 4). L’assertion (ii) est évidente. L’assertion (iii) résulte de VAR, R, 5.8.5.

#### Proposition 6 {#lie-iii-s1-prop-6 .statement}

Soient G un groupe de Lie, H un sous-groupe de G. Pour que H soit un sous-groupe de Lie de G, il faut et il suffit qu’il existe un point h ∈ H et un voisinage ouvert U de h dans G tels que H ∩ U soit une sous-variété de G.
La condition est évidemment nécessaire. Supposons-la vérifiée. Pour tout h' ∈ H, la translation γ(h'h^{-1}) est un automorphisme de la variété G et transforme la sous-variété H ∩ U de U en la sous-variété (h'h^{-1}H) ∩ (h'h^{-1}U) de h'h^{-1}U. Comme h'h^{-1}H = H et que h'h^{-1}U est un voisinage ouvert de h' dans G, on voit que tout point de H possède un voisinage ouvert V tel que V ∩ H soit une sous-variété de G. Donc H est une sous-variété de G.
C.Q.F.D.

Soient G un groupe de Lie, H un sous-groupe de Lie de G. Si L est un sous-groupe de Lie de H, L est un sous-groupe de Lie de G d’après VAR, R, 5.8.6. Soit M un sous-groupe de Lie de G tel que M ⊂ H. Alors M est un sous-groupe de Lie de H, car l’injection canonique de M dans H est évidemment une immersion.
Soit k un sous-corps fermé non discret de K. On appelle k-sous-groupe de Lie de G un sous-groupe de Lie du k-groupe de Lie sous-jacent à G.

#### Remarque {#lie-iii-s1-n3-rem-1 .statement}

Si on remplace « sous-variété » par « quasi-sous-variété » dans la déf. 3, on obtient la définition des quasi-sous-groupes de Lie de G. (Pour G de dimension finie, les quasi-sous-groupes de Lie ne sont autres que les sous-groupes de Lie.) Supposons K de caractéristique 0. La prop. 5 reste valable, avec la même démonstration, pour les quasi-sous-groupes de Lie. La prop. 6 reste valable, avec la même démonstration, en remplaçant « sous-groupe de Lie » par « quasi-sous-groupe de Lie », et « sous-variété » par « quasi-sous-variété ».

### 4. Produits semi-directs de groupes de Lie

Soient I un ensemble fini, (L_i)_{i \in I} une famille de groupes de Lie. Les structures de groupe et de variété sur L = \prod_{i \in I} L_i sont compatibles, et L est ainsi muni d’une structure de groupe de Lie. On dit que L est le groupe de Lie produit de la famille de groupes de Lie (L_i)_{i \in I}.

Soient $L$ et $M$ des groupes de Lie, $\sigma$ un homomorphisme de $L$ dans le groupe des automorphismes du groupe $M$. Soit $S$ le produit semi-direct externe de $L$ par $M$ relatif à $\sigma$ (A, I, p. 64, déf. 2).

#### Proposition 7 {#lie-iii-s1-prop-7 .statement}

*Si l’application* $(m, l) \mapsto \sigma(l)m$ *de* $M \times L$ *dans* $M$ *est analytique, le groupe* $S$, *muni de la structure de variété produit de* $M$ *et* $L$, *est un groupe de Lie*.

En effet, on a, pour $l, l'$ dans $L$ et $m, m'$ dans $M$,
$$
(m, l)(m', l')^{-1} = ml{l'}^{-1}{m'}^{-1} = m(\sigma(l{l'}^{-1}){m'}^{-1})l{l'}^{-1}
= (m(\sigma(l{l'}^{-1}){m'}^{-1}), l{l'}^{-1})
$$
d’où la proposition.

Si les conditions de la prop. 7 sont vérifiées, on dit que le groupe de Lie $S$ est le *groupe de Lie produit semi-direct (externe) de* $L$ *par* $M$ *relatif à* $\sigma$.

Il est clair que l’injection canonique de $L$ (resp. $M$) dans $S$ est un isomorphisme de $L$ (resp. $M$) sur un sous-groupe de Lie de $S$, que l’on identifie à $L$ (resp. $M$). L’application canonique de $S$ sur $L$ est un morphisme de groupes de Lie.

Réciproquement, soient $G$ un groupe de Lie, et $L, M$ deux sous-groupes de Lie tels que le groupe $G$ soit (algébriquement) produit semi-direct de $L$ par $M$ (A, I, p. 65). Posons $\sigma(l)m = lml^{-1}$ pour $l \in L$ et $m \in M$. Alors $\sigma$ vérifie la condition de la prop. 7. On peut donc former le groupe de Lie $S$ produit semi-direct de $L$ par $M$ relatif à $\sigma$. L’application $j : (m, l) \mapsto ml$ de $S$ sur $G$ est un isomorphisme de groupes, et est analytique. Si $j$ est un isomorphisme de groupes de Lie, on dit que *le groupe de Lie G est produit semi-direct (interne) de* $L$ *par* $M$, et l’on identifie $S$ et $G$. Pour tout $g \in G$, écrivons $g = p(g)q(g)$, où $p(g) \in M$ et $q(g) \in L$. Pour que le groupe de Lie $G$ soit produit semi-direct de $L$ par $M$, il faut et il suffit que l’une des applications $p : G \to M$ et $q : G \to L$ soit analytique, auquel cas toutes deux sont analytiques; ou encore, il faut et il suffit que $T_e(G)$ soit somme directe topologique de $T_e(M)$ et $T_e(L)$ (car, si cette condition est vérifiée, $j$ est étale en $e_S$).

#### Exemple {#lie-iii-s1-n4-exa-1 .statement}

Soient $E$ un espace normable, $G = \mathbf{GL}(E)$, $T$ le groupe des translations de $E$, $A$ le groupe de permutations de $E$ engendré par $G$ et $T$. Le groupe $A$ est algébriquement produit semi-direct de $G$ par $T$. (Si $E$ est de dimension finie, $A$ est le groupe affine de $E$, cf. A, II, p. 131.) Soient $\sigma$ la représentation linéaire identique de $G$ dans $E$, et $S$ le produit semi-direct externe de $G$ par $E$ relatif à $\sigma$. Pour tout $x \in E$, soit $t_x$ la translation de $E$ définie par $x$. L’application $(x, u) \mapsto t_x \circ u$ est un isomorphisme $\Phi$ du groupe $S$ sur le groupe $A$. L’application $(x, u) \mapsto \sigma(u)x = u(x)$ de $E \times \mathcal{L}(E)$ dans $E$ est bilinéaire continue, donc analytique; sa restriction à $E \times G$ est par suite analytique. Ainsi, le groupe $S$, muni de la structure de variété produit de $E$ et $G$, est un groupe de Lie. Transportons cette structure à $A$ grâce à $\Phi$. Alors $A$ devient un groupe de Lie, produit semi-direct interne de $G$ par $T$ en tant que groupe de Lie.

#### Proposition 8 {#lie-iii-s1-prop-8 .statement}

Soient G et H des groupes de Lie, $p : G \to H$ et $s : H \to G$ des morphismes de groupes de Lie tels que $p \circ s = \mathrm{id}_H$, et $N = \mathrm{Ker}\, p$. Alors N est un sous-groupe de Lie de G, s est un isomorphisme de H sur un sous-groupe de Lie de G, et le groupe de Lie G est produit semi-direct interne de $s(H)$ par N.

On a $T_e(p) \circ T_e(s) = \mathrm{id}_{T_e(H)}$, donc $p$ (resp. $s$) est une submersion (resp. une immersion). D’après VAR, R, 5.10.5, N est un sous-groupe de Lie de G. D’autre part, s est un homéomorphisme de H sur $s(H)$, donc s est un isomorphisme de H sur un sous-groupe de Lie de G (VAR, R, 5.8.3). Enfin, pour tout $g \in G$, on a $g = (s \circ p)(g) . n$ avec un $n \in N$; comme $s \circ p$ est analytique, le groupe de Lie G est produit semi-direct de $s(H)$ par N.

### 5. Quotient d’une variété par un groupe de Lie

Soient G un groupe de Lie, X une variété de classe $C^r$, et $(g, x) \mapsto gx$ une loi d’opération à gauche (A, I, p. 49) de classe $C^r$ de G dans X. Pour tout $g \in G$, notons $\tau(g)$ l’automorphisme $x \mapsto gx$ de X défini par g. Pour tout $x \in X$, notons $\rho(x)$ l’application orbitale $g \mapsto gx$ de G dans X définie par x. On a

$$
\rho(x) = \rho(gx) \circ \delta(g) \qquad \rho(x) = \tau(g) \circ \rho(x) \circ \gamma(g^{-1})
$$

quels que soient $g \in G$ et $x \in X$. Donc

$$
T_g(\rho(x)) = T_e(\rho(gx)) \circ T_g(\delta(g))
$$
$$
T_g(\rho(x)) = T_x(\tau(g)) \circ T_e(\rho(x)) \circ T_g(\gamma(g^{-1})).
$$

#### Proposition 9 {#lie-iii-s1-prop-9 .statement}

Soient $x \in X$ et $g_0 \in G$.

(i) Si $\rho(x)$ est une immersion (resp. une submersion, une subimmersion) en $g_0$, alors, pour tout $g \in G$, $\rho(gx)$ est une immersion (resp. une submersion, une subimmersion).

(ii) Si $\rho(x)$ est de rang k en $g_0$, alors, pour tout $g \in G$, $\rho(gx)$ est de rang constant égal à k.

Cela résulte aussitôt des formules (4) et (5) puisque $T_g(\delta(g))$, $T_x(\tau(g))$, $T_g(\gamma(g^{-1}))$ sont des isomorphismes.

#### Corollaire {#lie-iii-s1-n5-cor-1 .statement}

Soit $x \in X$. Si K est de caractéristique 0 et X de dimension finie, $\rho(x)$ est une subimmersion. Si de plus $\rho(x)$ est injective, $\rho(x)$ est une immersion.

Cela résulte de la prop. 9 et de VAR, R, 5.10.6.

Observons que, si $\eta$ désigne l’application $(g, x) \mapsto gx$ de $G \times X$ dans X, on a, pour $g \in G$, $x \in X$, $u \in T_g(G)$, $v \in T_x(X)$,

$$
T_{(g,x)}(\eta)(u, v) = T_{(g,x)}(\eta)(u, 0) + T_{(g,x)}(\eta)(0, v)
$$

c’est-à-dire

$$
T_{(g,x)}(\eta)(u, v) = T_g(\rho(x))u + T_x(\tau(g))v.
$$

#### Proposition 10 {#lie-iii-s1-prop-10 .statement}

Soient G un groupe de Lie, X une variété de classe C^r munie d’une loi d’opération à gauche de classe C^r de G dans X. Supposons que:
a) le groupe G opère proprement et librement dans X;
b) pour tout x ∈ X, ρ(x) est une immersion (ce qui est une conséquence de a) si K est de caractéristique 0 et X de dimension finie).

Alors la relation d’équivalence définie par G dans X est régulière (VAR, R, 5.9.5). Il existe sur l’ensemble quotient X/G une structure de variété et une seule telle que l’application canonique π : X → X/G soit une submersion. La topologie sous-jacente à cette structure de variété est la topologie quotient de celle de X; elle est séparée. Enfin, (X, G, X/G, π) est une fibration principale à gauche.¹

Soit θ l’application (g, x) ↦ (x, gx) de G × X dans X × X. Cette application est de classe C^r. Montrons que c’est une immersion. Pour u ∈ T_g(G) et v ∈ T_x(X), on a, d’après (6),

$$
T_{(g,x)}(\theta)(u, v) = (v, T_g(\rho(x))u + T_x(\tau(g))v).
$$

Mais T_g(ρ(x)) est injective d’après l’hypothèse b), donc T_{(g,x)}(θ) est injective. Son image est somme directe topologique du sous-espace H_{g,x} formé par les vecteurs (v, T_x(τ(g))v) pour v ∈ T_x(X), et du sous-espace I_{g,x} = {0} × T_g(ρ(x))(T_g(G)). D’après l’hypothèse b), T_g(ρ(x))(T_g(G)) admet un supplémentaire topologique J_{g,x} dans T_{gx}(X). Donc l’image de T_{(g,x)}(θ) admet le supplémentaire topologique {0} × J_{g,x}. On a donc bien prouvé que θ est une immersion de G × X dans X × X.

Comme G opère librement dans X, θ est injective. Soit C le graphe de la relation d’équivalence R définie par G dans X. Comme G opère proprement, θ est un homéomorphisme de G × X sur C (TG, I, § 10, prop. 2). D’après VAR, R, 5.8.3, C’est une sous-variété de X × X, et θ est un isomorphisme de la variété G × X sur la variété C. L’espace tangent T_{(x,gx)}(C) s’identifie à

$$
T_{(g,x)}(\theta)(T_{(g,x)}(G \times X)) = H_{g,x} \oplus I_{g,x} \subset T_{(x,gx)}(X \times X).
$$

Soient pr_1 et pr_2 les projections canoniques de X × X sur les deux facteurs. Il est immédiat que T_{(x,gx)}(pr_1) applique H_{g,x} sur T_x(X), et que le noyau de T_{(x,gx)}(pr_1) | T_{(x,gx)}(C) est I_{g,x}. Ainsi, pr_1 | C est une submersion de C sur X. D’après VAR, R, 5.9.5, R est régulière. Par définition, il existe donc sur l’ensemble quotient X/G une structure de variété et une seule telle que π soit une submersion. La topologie sous-jacente de X/G est la topologie quotient de celle de X (VAR, R, 5.9.4). Cette topologie est séparée (TG, III, § 4, prop. 3).

Pour tout b ∈ X/G, il existe un voisinage ouvert W de b et un morphisme σ : W → X tel que π ∘ σ = id_W (VAR, R, 5.9.1). Soit φ la bijection (g, w) ↦ gσ(w) de G × W sur π^{-1}(W). Elle est de classe C^r. On a π(gσ(w)) = w, et

¹ Les fibrations principales définies en VAR, R, 6.2.1, sont des fibrations principales à droite. La définition des fibrations principales à gauche s’en déduit de manière évidente.

θ⁻¹(σ(w), gσ(w)) = (g, σ(w)), donc la bijection réciproque de φ est de classe C⁰. Il est clair que φ(gg', w) = gφ(g', w) pour w ∈ W, g ∈ G, g' ∈ G. Donc (X, G, X/G, π) est une fibration principale à gauche.

C.Q.F.D.

#### Remarque {#lie-iii-s1-n5-rem-1 .statement}

Conservons les hypothèses précédentes. Soient de plus H une variété de classe C⁰ et (x, h) ↦ m(x, h) une application de classe C⁰ de X × H dans X telle que m(gx, h) = gm(x, h) pour x ∈ X, g ∈ G, h ∈ H. Soit n l’application de (X/G) × H dans X/G déduite de m par passage aux quotients. Montrons que n est de classe C⁰. Considérons le diagramme

$$
\begin{array}{ccc}
X \times H & \xrightarrow{m} & X \\
\pi \times 1 \downarrow & & \downarrow \pi \\
(X/G) \times H & \xrightarrow{n} & X/G.
\end{array}
$$

Il est commutatif, π ∘ m est de classe C⁰, et π × 1 est une submersion surjective; il suffit alors d’appliquer VAR, R, 5.9.5.

Soient G un groupe de Lie, X une variété de classe C⁰, et (g, x) ↦ xg une loi d’opération à droite de classe C⁰ de G dans X. Posons τ(g)x = ρ(x)g = xg pour g ∈ G, x ∈ X. On a cette fois

(3') $\rho(x) = \rho(xg) \circ \gamma(g^{-1}), \quad \rho(x) = \tau(g) \circ \rho(x) \circ \delta(g),$

donc

(4') $T_g(\rho(x)) = T_e(\rho(xg)) \circ T_g(\gamma(g^{-1}))$

(5') $T_g(\rho(x)) = T_x(\tau(g)) \circ T_e(\rho(x)) \circ T_g(\delta(g)).$

D’autre part, si η désigne l’application (g, x) ↦ xg de G × X dans X, la formule (6) reste valable. La prop. 9, son corollaire, et la prop. 10 restent également valables (à condition de remplacer, dans cette dernière, « fibration principale à gauche » par « fibration principale à droite »).

### 6. Espaces homogènes et groupes quotients

#### Proposition 11 {#lie-iii-s1-prop-11 .statement}

Soient X un groupe de Lie, G un sous-groupe de Lie de X.

(i) Il existe sur l’ensemble homogène X/G une structure de variété analytique et une seule telle que la projection canonique π de X sur X/G soit une submersion. La loi d’opération de X dans X/G est analytique. Pour tout x ∈ X, le noyau de Tₓ(π) se déduit de Tₑ(G) par Tₑ(γ(x)).

(ii) Si G est distingué dans X, X/G est un groupe de Lie pour sa structure de groupe et sa structure de variété définie en (i). L’application π est un morphisme de groupes de Lie.

$$
\pi^{-1}(\pi(x)) = xG = \gamma(x)(G),
$$

donc se déduit de T_e(G) par T_e(\gamma(x)).

Supposons G distingué. Soit m l’application (x, y) \mapsto xy^{-1} de (X/G) × (X/G) dans X/G. On a (m \circ (\pi \times \pi))(x, y) = \pi(xy^{-1}) quels que soient x, y dans X. Donc m \circ (\pi \times \pi) est analytique. Comme \pi \times \pi est une submersion surjective, m est analytique (VAR, R, 5.9.5), d’où (ii).

On dit que l’ensemble homogène X/G, muni de la structure de variété définie en (i), est l’espace homogène de Lie (à gauche) quotient de X par G. On définit de façon analogue l’espace homogène de Lie (à droite) G\setminus X. Quand G est distingué, le groupe de Lie X/G défini en (ii) s’appelle le groupe de Lie quotient de X par G.

#### Proposition 12 {#lie-iii-s1-prop-12 .statement}

Soient X un groupe de Lie, Y une variété analytique non vide munie d’une loi d’opération à gauche analytique de X dans Y. Pour tout y \in Y, soient \rho(y) l’application orbitale définie par y, et X_y le stabilisateur de y dans X. Les conditions suivantes sont équivalentes:

(i) il existe y \in Y tel que \rho(y) soit une submersion surjective;
(i') pour tout y \in Y, \rho(y) est une submersion surjective;
(ii) il existe y \in Y tel que X_y soit un sous-groupe de Lie de X et que l’application canonique de X/X_y dans Y soit un isomorphisme de variétés;
(ii') pour tout y \in Y, X_y est un sous-groupe de Lie de X, et l’application canonique de X/X_y dans Y est un isomorphisme de variétés;
(iii) l’application (x, y) \mapsto (y, xy) de X \times Y dans Y \times Y est une submersion surjective.

Comme l’application canonique de X sur X/X_y est une submersion, les équivalences (i) \Leftrightarrow (ii), (i') \Leftrightarrow (ii') sont immédiates. On a (i) \Leftrightarrow (i') d’après la prop. 9 du n° 5. L’équivalence (i') \Leftrightarrow (iii) résulte de la formule (7) du n° 5.

Sous les conditions de la prop. 12, on dit que Y est un espace homogène de Lie (à gauche) pour X. On définit de manière analogue un espace homogène de Lie à droite pour X.

#### Exemple {#lie-iii-s1-n6-exa-1 .statement}

Soit G un groupe de Lie. Faisons opérer G \times G à gauche dans G par (g_1, g_2)x = g_1xg_2^{-1}. Soit \rho l’application orbitale de e. Alors les restrictions de T_{(e,e)}(\rho) à T_{(e,e)}(G \times \{e\}) = T_e(G) \times \{0\} et à T_{(e,e)}(\{e\} \times G) = \{0\} \times T_e(G) sont des isomorphismes de ces espaces sur T_e(G). Donc T_{(e,e)}(\rho) est surjective, et Ker T_{(e,e)}(\rho) admet par exemple le supplémentaire topologique T_e(G) \times \{0\} dans T_{(e,e)}(G \times G). Ainsi, \rho est une submersion en (e, e). Donc G est un espace homogène de Lie à gauche pour G \times G.

#### Proposition 13 {#lie-iii-s1-prop-13 .statement}

Soient G un groupe de Lie, H un sous-groupe de Lie distingué de G, X une variété de classe C^r, et (g, x) ↦ gx une loi d’opération à gauche de classe C^r de G dans X. On suppose que les conditions a) et b) de la prop. 10 sont vérifiées.

(i) La loi d’opération à gauche (h, x) ↦ hx de H dans X vérifie les conditions a) et b) de la prop. 10 (de sorte qu’on peut considérer les variétés quotients X/G et X/H).

(ii) La loi d’opération à gauche de G dans X définit par passage aux quotients une loi d’opération à gauche de classe C^r de G/H dans X/H; cette loi vérifie les conditions a) et b) de la prop. 10 (de sorte qu’on peut considérer la variété quotient (X/H)/(G/H)).

(iii) L’application canonique de X sur X/H définit par passage aux quotients une bijection de X/G sur (X/H)/(G/H). Cette bijection est un isomorphisme de variétés de classe C^r.

Il est clair que H opère librement dans X; il opère proprement d’après TG, III, § 4, n° 1, Exemple 1. Les applications orbitales de H dans X sont des immersions puisque l’injection canonique de H dans G est une immersion. Cela prouve (i).

La loi d’opération de G dans X définit évidemment, par passage aux quotients, une loi d’opération à gauche de G/H dans X/H. Cette loi est de classe C^r d’après VAR, R, 5.9.6. Soient g ∈ G et x ∈ X tels que (Hg)(Hx) = Hx; alors H(gx) = Hx, donc gx ∈ Hx et g ∈ H; cela prouve que G/H opère librement dans X/H. L’application θ : (g, x) ↦ (x, gx) de G × X dans X × X est fermée; d’autre part, on a θ(Hg × Hx) = Hx × H(gx); il en résulte aussitôt que l’application

$$(Hg, Hx) ↦ (Hx, H(gx))$$

de (G/H) × (X/H) dans (X/H) × (X/H) est fermée; comme en outre G/H opère librement dans X/H, le th. 1 c) de TG, I, § 10, n° 2 prouve que G/H opère proprement dans X/H.

Soient π l’application canonique de X sur X/H, σ l’application canonique de G sur G/H, x un élément de X et y = π(x).

$$
\begin{array}{ccc}
G & \xrightarrow{\rho(x)} & X \\
\sigma \downarrow & & \pi \downarrow \\
G/H & \xrightarrow{\rho(y)} & X/H
\end{array}
$$

Alors, π ∘ ρ(x) = ρ(y) ∘ σ, donc

$$T_x(\pi) \circ T_e(\rho(x)) = T_e(\rho(y)) \circ T_e(\sigma).$$

Soit u ∈ T_e(G/H) tel que T_e(ρ(y))u = 0. Il existe v ∈ T_e(G) tel que u = T_e(σ)v. Alors (T_x(π)(T_e(ρ(x))v)) = 0, donc T_e(ρ(x))v est tangent à Hx (VAR, R, 5.10.5) et par suite de la forme T_e(ρ(x)|H)v' pour un v' ∈ T_e(H). Comme T_e(ρ(x)) est injective, on en déduit que v = v', d’où v ∈ T_e(H) et par suite u = 0. Ainsi, T_e(ρ(y)) est injective. L’image de T_e(ρ(y)) est égale à celle de T_x(π) ∘ T_e(ρ(x));

or l’image de $T_e(\rho(x))$ admet un supplémentaire topologique dans $T_x(X)$, et contient le noyau de $T_x(\pi)$. On voit donc que $\rho(y)$ est une immersion, ce qui achève de prouver (ii).

L’assertion (iii) résulte de ce qui précède, et de VAR, R, 5.9.7.

#### Corollaire {#lie-iii-s1-n6-cor-1 .statement}

Soient G un groupe de Lie, H et L des sous-groupes de Lie distingués de G, avec $L \subset H$. Alors $H/L$ est un sous-groupe de Lie distingué de $G/L$, et la bijection canonique de $G/H$ sur $(G/L)/(H/L)$ est un isomorphisme de groupes de Lie.

### 7. Orbites

#### Proposition 14 {#lie-iii-s1-prop-14 .statement}

Soient G un groupe de Lie, X une variété analytique, et $(g, x) \mapsto gx$ une loi d’opération à gauche analytique de G dans X. Soit $x \in X$. Supposons que l’application orbitale correspondante $\rho(x)$ soit une subimmersion (ce qui est toujours le cas si K est de caractéristique 0 et X de dimension finie (cor. de la prop. 9)). Soit $G_x$ le stabilisateur de x dans G.

(i) $G_x$ est un sous-groupe de Lie, et $T_e(G_x) = \mathrm{Ker}\ T_e(\rho(x))$.

(ii) L’application canonique $i_x$ de l’espace homogène $G/G_x$ dans X est une immersion d’image $Gx$.

(iii) Si de plus l’orbite $Gx$ est localement fermée et si la topologie de G admet une base dénombrable, alors $Gx$ est une sous-variété de X, $i_x$ est un isomorphisme de la variété $G/G_x$ sur la variété $Gx$, et $T_x(Gx) = \mathrm{Im}\ T_e(\rho(x))$.

L’image réciproque de x par $\rho(x)$ est $G_x$. Comme $\rho(x)$ est une subimmersion, $G_x$ est une sous-variété, et, pour tout $g \in G$, l’espace tangent J à $gG_x = \rho(x)^{-1}(gx)$ en $g$ est $\mathrm{Ker}\ T_g(\rho(x))$ (VAR, R, 5.10.5), d’où (i). Soit $\pi : G \to G/G_x$ l’application canonique. On a $i_x \circ \pi = \rho(x)$. Comme $G/G_x$ est variété quotient de G, cette égalité prouve que $i_x$ est analytique. De plus, les noyaux de $T_g(\rho(x))$ et de $T_g(\pi)$ sont tous deux égaux à J. Donc $T_{\pi(g)}(i_x)$ est injective. L’image de $T_{\pi(g)}(i_x)$ est égale à l’image de $T_g(\rho(x))$, donc admet un supplémentaire topologique. Ceci prouve (ii).

Supposons $Gx$ localement fermée. Tout point de $Gx$ possède alors un voisinage dans $Gx$ qui est homéomorphe à un sous-espace fermé d’un espace métrique complet, donc qui est un espace de Baire. Donc $Gx$ est un espace de Baire (TG, IX, § 5, prop. 4). Si G est à base dénombrable, $i_x$ est donc un homéomorphisme de $G/G_x$ sur $Gx$ (TG, IX, § 5). Alors, d’après (ii) et VAR, R, 5.8.3, $i_x$ est un isomorphisme de la variété $G/G_x$ sur la variété $Gx$, et

$$
T_x(Gx) = \mathrm{Im}\ T_{\pi(e)}(i_x) = \mathrm{Im}\ T_e(\rho(x)).
$$

#### Remarque {#lie-iii-s1-n7-rem-1 .statement}

Soient G un groupe de Lie de dimension finie, X une variété de classe $C^r$, et $(g, x) \mapsto gx$ une loi d’opération à gauche de classe $C^r$ de G dans X. Alors la prop. 14 reste valable. Le seul point qui nécessite une démonstration différente est le fait que $G_x$ est un sous-groupe de Lie. Mais si $r \neq \omega$, on a $K = \mathbf{R}$; comme il est clair que $G_x$ est fermé, $G_x$ est un sous-groupe de Lie d’après le § 8, th. 2.

#### Corollaire {#lie-iii-s1-n7-cor-1 .statement}

Soient G un groupe de Lie dont la topologie admet une base dénombrable, X une variété analytique non vide de dimension finie, munie d’une loi d’opération à gauche analytique de G dans X. On suppose que G opère transitivement dans X, et que K est de caractéristique 0. Alors X est un espace homogène de Lie pour G.

Soit x ∈ X. L’orbite de x, égale à X, est fermée, et on peut donc appliquer la prop. 14 (iii).

### 8. Fibrés vectoriels à opérateurs

Soient G un groupe de Lie, X une variété de classe C^r, et (g, x) ↦ gx une loi d’opération à gauche de classe C^r de G dans X. Soit E un fibré vectoriel de classe C^r, de base X, et π : E → X la projection de E sur X. Pour tout x ∈ X, soit E_x la fibre de E en x. Soit (g, u) ↦ gu une loi d’opération à gauche de G dans E telle que π soit compatible avec les opérations de G dans X et dans E. Pour tout g ∈ G et tout x ∈ X, la restriction à E_x de l’application u ↦ gu est une bijection ψ_{g,x} de E_x sur E_{gx}. Nous supposerons que, pour tout g ∈ G et tout x ∈ X, ψ_{g,x} est linéaire continue, donc est un isomorphisme de l’espace normable E_x sur l’espace normable E_{gx}.

Soit φ l’automorphisme (g, x) ↦ (g, gx) de la variété G × X. Soient p la projection canonique de G × X sur X, et E' l’image réciproque de E relativement à p. Soit ψ : E' → E' l’application somme des ψ_{g,x} : E'_{(g, x)} → E'_{(g, gx)}.

#### Définition 4 {#lie-iii-s1-def-4 .statement}

Si ψ est un φ-morphisme de fibrés vectoriels de classe C^r, on dit que E est un G-fibré vectoriel de classe C^r.

Autrement dit, E est un G-fibré vectoriel de classe C^r si, quel que soit (g_0, x_0) ∈ G × X, la condition suivante est vérifiée: il existe un voisinage ouvert U de (g_0, x_0) dans G × X tel que, si l’on identifie E' |U (resp. E' | φ(U)) à un fibré vectoriel trivial de fibre M (resp. N) grâce à une carte vectorielle, l’application (g, x) ↦ ψ_{g,x} de U dans 𝒫(M, N) soit de classe C^r.

L’application ψ est évidemment bijective, et il résulte du critère local ci-dessus que ψ^{-1} est un φ^{-1}-morphismes de fibrés vectoriels, de sorte que ψ est un φ-isomorphisme de fibrés vectoriels.

On appelle G-fibré vectoriel trivial de base X un fibré vectoriel X × F (où F est un espace normable complet), muni de la loi d’opération (g, (x, f)) ↦ (gx, f) de G dans X × F.

Reprenons les hypothèses et notations précédant la déf. 4, et soit de plus τ un foncteur vectoriel de classe C^r pour les isomorphismes (VAR, R, 7.6.6). Alors τE est un fibré vectoriel de base X. Pour tout x ∈ X, sa fibre (τE)_x est égale à τ(E_x). Quels que soient les espaces normables N_1, N_2, notons Isom(N_1, N_2) l’ensemble des isomorphismes de N_1 sur N_2. Si g ∈ G, on a

$$
\tau(\psi_{g,x}) \in \mathrm{Isom}((\tau E)_x, (\tau E)_{gx}).
$$

Les $\tau(\psi_{g,x})$ définissent une loi d’opération à gauche $(g,u) \mapsto gu$ de $G$ dans $\tau E$, et la projection canonique de $\tau E$ sur $X$ est compatible avec les opérations de $G$ dans $X$ et $\tau E$.

#### Proposition 15 {#lie-iii-s1-prop-15 .statement}

*Si $E$ est un $G$-fibré vectoriel de classe $C^r$, $\tau E$ est un $G$-fibré vectoriel de classe $C^r$.*

Soient $g_0, x_0, U, M, N$ comme dans l’alinéa suivant la déf. 4. Alors l’application $(g, x) \mapsto \tau(\psi_{g,x})$ de $U$ dans $\mathcal{L}(\tau M, \tau N)$ est composée de l’application $(g, x) \mapsto \psi_{g,x}$ de $U$ dans $\mathcal{L}(M, N)$, et de l’application $f \mapsto \tau(f)$ de Isom$(M, N)$ dans Isom$(\tau M, \tau N)$; ces deux applications sont de classe $C^r$, donc il en est de même de leur composée, d’où la proposition.

#### Proposition 16 {#lie-iii-s1-prop-16 .statement}

*Soient $G$ un groupe de Lie, $X$ une variété de classe $C^r$ ($r \geq 2$), et $(g, x) \mapsto gx$ une loi d’opération à gauche de classe $C^r$ de $G$ dans $X$, d’où, par transport de structure, une loi d’opération à gauche de $G$ dans $TX$. Pour cette loi, $TX$ est un $G$-fibré vectoriel de classe $C^{r-1}$.*

Soit $\mathrm{pr}_1$ (resp. $\mathrm{pr}_2$) la projection canonique de $G \times X$ sur $G$ (resp. $X$), et soit $E_1$ (resp. $E_2$) l’image réciproque de $TG$ (resp. $TX$) relativement à $\mathrm{pr}_1$ (resp. $\mathrm{pr}_2$). Alors le fibré vectoriel $T(G \times X)$ est somme directe de $E_1$ et $E_2$. Soient $i : E_2 \to T(G \times X)$ et $q : T(G \times X) \to E_2$ les morphismes canoniques de fibrés vectoriels définis par cette décomposition en somme directe. Soit $\varphi$ l’application $(g, x) \mapsto (g, gx)$ de $G \times X$ dans $G \times X$. Alors l’application notée $\psi$ dans la déf. 4 (où l’on fait $E = TX$) n’est autre que $q \circ T(\varphi) \circ i$. Or $T(\varphi)$ est un $\varphi$-morphisme de fibrés vectoriels de classe $C^{r-1}$ (VAR, R, 8.1.2).

#### Corollaire {#lie-iii-s1-n8-cor-1 .statement}

*Si $\tau$ est un foncteur vectoriel de classe $C^r$ pour les isomorphismes, $\tau(TX)$ est un $G$-fibré vectoriel de classe $C^{r-1}$.*

Cela résulte des prop. 15 et 16.

#### Remarque 1 {#lie-iii-s1-n8-rem-1 .statement}

Si $\tau$ est un foncteur vectoriel de classe $C^r$ pour les isomorphismes *en dimension finie*, et si $E$ est de rang fini, $\tau E$ se définit de la même manière, et la prop. 15 reste valable; le cor. de la prop. 16 reste valable pourvu que $X$ soit de dimension finie.

#### Exemple {#lie-iii-s1-n8-exa-1 .statement}

Reprenons les hypothèses et notations de la prop. 16, et soit $F$ un espace normable complet. Alors $\mathcal{L}((TX)^p ; F)$ est un $G$-fibré vectoriel de classe $C^{r-1}$; il en est de même de $\mathrm{Alt}^p(TX ; F)$ si $K$ est de caractéristique zéro, ou si $X$ est de dimension finie (cf. VAR, R, 7.7, 7.8). Si $X$ est de dimension finie, $\bigotimes^p(TX) \otimes \bigotimes^q(TX)^*$ est un $G$-fibré vectoriel de classe $C^{r-1}$.

#### Proposition 17 {#lie-iii-s1-prop-17 .statement}

*Soient $G$ un groupe de Lie, $X$ un espace homogène de Lie à gauche pour $G$, $x_0$ un point de $X$, $G_0$ le stabilisateur de $x_0$ dans $G$, $E$ et $E'$ des $G$-fibrés vectoriels à gauche de classe $C^r$ et de base $X$, $E_0$ (resp. $E'_0$) la fibre en $x_0$ de $E$ (resp. $E'$), $f$ un élément de $\mathcal{L}(E_0, E'_0)$ tel que $f(gu) = gf(u)$ quels que soient $u \in E_0$ et $g \in G_0$. Alors il existe un morphisme et un seul de $E$ dans $E'$, compatible avec les opérations de $G$, et prolongeant $f$.

L’unicité de ce morphisme est évidente. Prouvons son existence. Soient $g$, $g'$ dans $G$ et $u \in E_0$ tels que $gu = g'u$. On a ${g'}^{-1}g \in G_0$ et ${g'}^{-1}gu = u$, donc ${g'}^{-1}gf(u) = f(u)$, c’est-à-dire $gf(u) = g'f(u)$. On définit donc une application $\varphi$ de $E$ dans $E'$ en posant $\varphi(gu) = gf(u)$. Il est clair que cette application prolonge $f$, et qu’elle est compatible avec les opérations de $G$. Montrons que $\varphi$ est un morphisme de fibrés vectoriels de classe $C^r$. Soit $x_1 \in X$. Il existe un voisinage ouvert $V$ de $x_1$ dans $X$ et une sous-variété $W$ de $G$, tels que l’application $g \mapsto gx_0$ soit un isomorphisme $\theta$ de classe $C^r$ de $W$ sur $V$. En diminuant $V$ et $W$, on peut supposer que:

1) $E \mid V$ (resp. $E' \mid V$) s’identifie à un fibré vectoriel trivial de fibre $M$ (resp. $M'$);
2) si l’on note $\psi_g$ (resp. $\psi'_g$) l’application $u \mapsto gu$ de $E_0$ (resp. $E'_0$) dans $E_{gx_0}$ (resp. $E'_{gx_0}$), alors les applications $g \mapsto \psi_g$ et $g \mapsto \psi_g^{-1}$ (resp. $g \mapsto \psi'_g$ et $g \mapsto {\psi'_g}^{-1}$) de $W$ dans $\mathcal{L}(E_0, M)$ et $\mathcal{L}(M, E_0)$ (resp. $\mathcal{L}(E'_0, M')$ et $\mathcal{L}(M', E'_0)$) sont de classe $C^r$.

Pour $x \in V$, soit $\varphi_x : M \to N$ la restriction de $\varphi$ à $E_x = M$. Alors $\varphi_x$ s’obtient en composant les applications suivantes:
1) l’application $(\psi_{\theta^{-1}x})^{-1}$ de $M$ dans $E_0$;
2) l’application $f$ de $E_0$ dans $E_0$;
3) l’application $\psi'_{\theta^{-1}x}$ de $E_0$ dans $M'$.

On voit donc que l’application $x \mapsto \varphi_x$ de $V$ dans $\mathcal{L}(M, M')$ est de classe $C^r$.

#### Corollaire 1 {#lie-iii-s1-prop-17-cor-1 .statement}

Soit $E_0^{G_0}$ l’ensemble des éléments de $E_0$ invariants par $G_0$. Pour tout $u \in E_0^{G_0}$, soit $\sigma_u$ l’application de $X$ dans $E$ définie par $\sigma_u(gx_0) = gu$ pour tout $g \in G$.
(i) Les sections¹ $G$-invariantes de $E$ sont de classe $C^r$.
(ii) $u \mapsto \sigma_u$ est une bijection de $E_0^{G_0}$ sur l’ensemble des sections $G$-invariantes de $E$.

L’assertion (ii) est évidente. Pour prouver (i), il suffit de prouver que chaque section $\sigma_u$ est de classe $C^r$. Soit $E'$ le $G$-fibré trivial de base $X$ et de fibre $E_0^{G_0}$. Soit $f$ l’injection canonique de $E_0^{G_0}$ dans $E_0$. D’après la prop. 17, il existe un morphisme $\varphi$ de $E'$ dans $E$ compatible avec les opérations de $G$ et prolongeant $f$. Si $u \in E_0^{G_0}$ et $g \in G$, on a
$$
\sigma_u(gx_0) = gu = gf(u) = \varphi(gu) = \varphi((u, gx_0))
$$
donc $\sigma_u(x) = \varphi((u, x))$ pour tout $x \in X$, ce qui prouve notre assertion.

*Par exemple, soient $G$ un groupe de Lie réel de dimension finie, $G_0$ un sous-groupe de Lie compact de $G$, et $X$ l’espace homogène $G/G_0$. Notons $x_0$ l’image canonique de $e$ dans $X$. Il existe une forme bilinéaire symétrique positive non dégénérée sur $T_{x_0}(X)$

¹ Nous appelons ici section de $E$ une application $\sigma$ (non nécessairement de classe $C^r$) de $X$ dans $E$ telle que $p \circ \sigma = \mathrm{Id}_X$, où $p$ désigne la projection de $E$ sur $X$.

#### Corollaire 2 {#lie-iii-s1-prop-17-cor-2 .statement}

*On suppose que $G_0$ opère trivialement dans $E_0$. Soit $E'$ le $G$-fibré trivial de base $X$ et de fibre $E_0$. Il existe un isomorphisme et un seul de $E$ sur $E'$ compatible avec les opérations de $G$ et prolongeant $\mathrm{Id}_{E_0}$.

Cela résulte aussitôt de la prop. 17.

#### Remarque 2 {#lie-iii-s1-n8-rem-2 .statement}

Dans ce n°, on peut remplacer partout les lois d’opération à gauche par des lois d’opération à droite.

### 9. Définition locale d’un groupe de Lie

#### Proposition 18 {#lie-iii-s1-prop-18 .statement}

*Soient $G$ un groupe, $U$ et $V$ deux sous-ensembles de $G$ contenant $e$. Supposons $U$ muni d’une structure de variété analytique vérifiant les conditions suivantes*:
(i) $V = V^{-1}, V^2 \subset U, V$ est ouvert dans $U$;
(ii) l’application $(x, y) \mapsto xy^{-1}$ de $V \times V$ dans $U$ est analytique;
(iii) pour tout $g \in G$, il existe un voisinage ouvert $V'$ de $e$ dans $V$ tel que $gV'g^{-1} \subset U$ et tel que l’application $x \mapsto gxg^{-1}$ de $V'$ dans $U$ soit analytique.

Il existe alors sur $G$ une structure de variété analytique et une seule possédant les propriétés suivantes:
α) $G$, muni de cette structure, est un groupe de Lie;
β) $V$ est ouvert dans $G$;
γ) les structures de variété de $G$ et $U$ induisent la même structure sur $V$.

a) Soient $A$ une partie ouverte de $V$ et $v_0$ un élément de $V$ tels que $v_0A \subset V$. Alors $v_0A$ est l’ensemble des $v \in V$ tels que $v_0^{-1}v \in A$, donc est une partie ouverte de $V$ (compte tenu de (ii)). En outre, (ii) entraîne que les applications $v \mapsto v_0v$ de $A$ sur $v_0A$ et $v \mapsto v_0^{-1}v$ de $v_0A$ sur $A$ sont des bijections réciproques et analytiques, donc des isomorphismes analytiques.

b) Choisissons un voisinage ouvert $W$ de $e$ dans $V$ tel que $W = W^{-1}, W^3 \subset V$, et tel qu’il existe une carte $(W, \varphi, E)$ de la variété $U$, de domaine $W$. Pour tout $g \in G$, soit $\varphi_g$ l’application $h \mapsto \varphi(g^{-1}h)$ de $gW$ dans $E$. Montrons que les cartes $\varphi_g$ de $G$ sont analytiquement compatibles. Soient $g_1, g_2$ dans $G$ tels que $g_1W \cap g_2W \neq \varnothing$, de sorte que $g_2^{-1}g_1$ et $g_1^{-1}g_2$ appartiennent à $W^2$. D’après a), $W \cap g_1^{-1}g_2W$ est une partie ouverte de $W$, donc

$$
\varphi_{g_1}(g_1W \cap g_2W) = \varphi(W \cap g_1^{-1}g_2W)
$$

est une partie ouverte $D$ de $E$. Pour $d \in D$, on a,

$$
(\varphi_{g_2} \circ \varphi_{g_1}^{-1})(d) = \varphi(g_2^{-1}g_1\varphi^{-1}(d));
$$

d’après a), on voit que $\varphi_{g_2} \circ \varphi_{g_1}^{-1}$ est analytique.

c) D’après b), il existe sur G une structure de variété analytique telle que $(\varphi_g)_{g \in G}$ soit un atlas de G. Pour tout $g_0 \in G$, l’application $g \mapsto g_0 g$ ($g \in G$) laisse cet atlas invariant, donc est un automorphisme de G pour cette structure de variété. En particulier la condition $(GL_1)$ est vérifiée.

d) Soit $v_0 \in V$. D’après (ii), il existe un voisinage ouvert A de e dans W tel que $v_0 A \subset V$. Cela prouve d’abord que V est ouvert dans G. D’après a), l’application $v \mapsto v_0 v$ de A sur $v_0 A$ est un isomorphisme analytique pour les structures induites par U. Compte tenu de c), on voit que les structures de variété de G et U induisent la même structure sur $v_0 A$, donc finalement sur V.

e) Compte tenu de d), (ii) et (iii), on voit que les conditions $(GL_2)$ et $(GL_3)$ sont vérifiées. Donc G est un groupe de Lie.

f) Si une structure de variété sur G est compatible avec la structure de groupe de G et telle que V soit une sous-variété ouverte de G, alors $(\varphi_g)_{g \in G}$ est un atlas de G. D’où l’assertion d’unicité dans la proposition.

#### Proposition 19 {#lie-iii-s1-prop-19 .statement}

Soient G un groupe topologique, H un groupe de Lie, f un homomorphisme du groupe G dans le groupe H. On suppose qu’il existe un voisinage ouvert U de $e_G$ dans G, une carte (V, $\varphi$, E) de la variété H en $e_H$, et un sous-espace vectoriel fermé F de E admettant un supplémentaire topologique, tels que $f(U) \subset V$ et que $(\varphi \circ f)|U$ soit un homéomorphisme de U sur $\varphi(V) \cap F$. Alors, il existe sur G une structure unique de variété telle que f soit une immersion; cette structure est l’image inverse par f de la structure de variété de H. Pour cette structure, G est un groupe de Lie.

Comme les translations de G (resp. H) sont des homéomorphismes (resp. des isomorphismes analytiques), f vérifie la condition (R) de VAR, R, 5.8.1. Les deux premières assertions de la proposition résultent alors de VAR, R, loc. cit. Considérons le diagramme commutatif

$$
\begin{array}{ccc}
G \times G & \xrightarrow{m} & G \\
| & & | \\
H \times H & \xrightarrow{n} & H
\end{array}
$$

où $m(x, y) = xy^{-1}$ (resp. $n(x, y) = xy^{-1}$) pour $x, y$ dans G (resp. H). Alors $n \circ (f \times f)$ est analytique, donc $f \circ m$ est analytique, donc $m$ est analytique puisque $f$ est une immersion. Par suite, G est un groupe de Lie.

On dit que la structure de groupe de Lie de G est l’image inverse de la structure de groupe de Lie de H par f.

#### Corollaire {#lie-iii-s1-n9-cor-1 .statement}

Soient G un groupe topologique, N un sous-groupe distingué discret de G, $\pi$ l’application canonique de G sur $G/N$. Supposons donnée une structure de variété analytique sur $G/N$, compatible avec la structure de groupe topologique de $G/N$. Alors il existe sur G une structure unique de variété telle que $\pi$ soit une immersion; cette structure est l’image inverse par $\pi$ de la structure de variété de $G/N$. Pour cette structure, $\pi$ est étale, $G$ est un groupe de Lie, et $G/N$ est le groupe de Lie quotient de $G$ par $N$.

#### Remarque {#lie-iii-s1-n9-rem-1 .statement}

Soient $H$ un groupe de Lie réel ou complexe connexe, $\hat{H}$ son revêtement universel¹, $\pi$ l’application canonique de $\hat{H}$ sur $H$. Quand on parlera de $\hat{H}$ comme d’un groupe de Lie, il s’agira toujours de la structure image inverse de celle de $H$ par $\pi$.

### 10. Groupuscules

#### Définition 5 {#lie-iii-s1-def-5 .statement}

On appelle groupuscule de Lie sur $K$ un système $(G, e, \theta, m)$ vérifiant les conditions suivantes:

(i) $G$ est une variété analytique sur $K$;
(ii) $e \in G$;
(iii) $\theta$ est une application analytique de $G$ dans $G$;
(iv) $m$ est une application analytique d’une partie ouverte $\Omega$ de $G \times G$ dans $G$;
(v) pour tout $g \in G$, on a $(e, g) \in \Omega, (g, e) \in \Omega, m(e, g) = m(g, e) = g$;
(vi) pour tout $g \in G$, on a $(g, \theta(g)) \in \Omega, (\theta(g), g) \in \Omega, m(g, \theta(g)) = m(\theta(g), g) = e$;
(vii) si $g, h, k$ sont des éléments de $G$ tels que $(g, h) \in \Omega, (h, k) \in \Omega, (m(g, h), k) \in \Omega, (g, m(h, k)) \in \Omega$, alors $m(m(g, h), k) = m(g, m(h, k))$.

On dit que $e$ est l’élément neutre du groupuscule. On écrit souvent $gh$ au lieu de $m(g, h)$, et (par abus de notation) $g^{-1}$ au lieu de $\theta(g)$.

Un groupe de Lie $G$ est un groupuscule de Lie pour le choix évident de $e, \theta, m$.

Soit $G$ un groupuscule de Lie. On a $ee^{-1} = e$, c’est-à-dire

$$
e^{-1} = e.
$$

Pour tout $g \in G$, on a

$$
g = eg = ((g^{-1})^{-1}g^{-1})g = (g^{-1})^{-1}(g^{-1}g) = (g^{-1})^{-1}e,
$$

c’est-à-dire

$$
(g^{-1})^{-1} = g.
$$

Un sous-ensemble de $G$ invariant par l’application $g \mapsto g^{-1}$ est dit symétrique.

La variété $G$, munie du point $e$, de l’application $g \mapsto g^{-1}$, et de l’application $(g, h) \mapsto hg$, est un groupuscule de Lie $G^\vee$ dit opposé à $G$.

Le groupuscule de Lie $G$ est dit commutatif si, pour tout $(g, h) \in G \times G$ tel que $gh$ soit défini, $hg$ est défini et égal à $gh$.

¹ Cf. TG, XI ; en attendant la parution de ce chapitre, voir par exemple L. S. PONTRJAGIN, Topological groups, 2nd edition translated from Russian, Gordon and Breach, 1966 ; ou G. HOCHSCHILD, The structure of Lie groups, Holden-Day, 1965.

Soit G un groupuscule de Lie. L’ensemble des $(g, h) \in G \times G$ tels que $gh$ soit défini est un voisinage de $(e, e)$. D’autre part, les applications $(g, h) \mapsto gh$ et $g \mapsto g^{-1}$ sont continues. Donc $(gh)k = g(hk)$ pour $g, h, k$ assez voisins de $e$. De même, $(h^{-1}g^{-1})(gh) = h^{-1}(eh) = h^{-1}h = e$ pour $g, h$ assez voisins de $e$, d’où, en multipliant à droite par $(gh)^{-1}$,

$$(10)$$
$$(gh)^{-1} = h^{-1}g^{-1}$$ pour $g, h$ assez voisins de $e$.

#### Proposition 20 {#lie-iii-s1-prop-20 .statement}

*Soient G un groupuscule de Lie et $g \in G$. Il existe un voisinage ouvert U de e et un voisinage ouvert V de g possédant les propriétés suivantes:*
    *a)* $ug$ est défini pour tout $u \in U$;
    *b)* $vg^{-1}$ est défini pour tout $v \in V$;
    *c)* les applications $u \mapsto ug,\ v \mapsto vg^{-1}$ sont des isomorphismes analytiques réciproques l’un de l’autre de U sur V et de V sur U.

Comme l’ensemble de définition du produit est ouvert dans $G \times G$, il existe un voisinage ouvert U de $e$ et un voisinage ouvert V de $g$ avec les propriétés *a)* et *b)*. Posons $\eta(u) = ug$ pour $u \in U$, $\eta'(v) = vg^{-1}$ pour $v \in V$. En diminuant U et V, on peut supposer que $(ug)g^{-1} = u$ et $(vg^{-1})g = v$ pour $u \in U$ et $v \in V$. Alors $\eta$ et $\eta'$ sont des injections. En diminuant encore U, on peut supposer $\eta(U) \subset V$. Alors $\eta'(V) \supset U$, et $\eta(U)$ est l’image réciproque de U par $\eta'$, donc est un voisinage ouvert de $g$ dans V. Remplaçant V par $\eta(U)$, on se ramène finalement au cas où $\eta$ et $\eta'$ sont des bijections réciproques et analytiques.

C.Q.F.D.

Soient $G_1$, $G_2$ deux groupuscules de Lie, d’éléments neutres $e_1$, $e_2$. On dit qu’une application $f$ de $G_1$ dans $G_2$ est un *morphisme* si $f$ vérifie les conditions suivantes:
    (i) $f$ est analytique;
    (ii) $f(e_1) = e_2$;
    (iii) si $g, h$ dans $G_1$ sont tels que $gh$ soit défini, alors $f(g)f(h)$ est défini et égal à $f(gh)$.

Soit $g \in G_1$. Comme $gg^{-1}$ est défini et égal à $e_1$, $f(g)f(g^{-1})$ est défini et égal à $e_2$, donc

$$f(g)^{-1} = f(g)^{-1}(f(g)f(g^{-1})) = (f(g)^{-1}f(g))f(g^{-1})$$

c’est-à-dire

$$(11)$$
$$f(g)^{-1} = f(g^{-1}).$$

Le composé de deux morphismes est un morphisme.

Si $f : G_1 \to G_2$ et $f' : G_2 \to G_1$ sont des morphismes réciproques l’un de l’autre, ce sont des isomorphismes (compte tenu notamment de la formule (11)).

Soient $G_1, G_2$ deux groupuscules de Lie, $f$ une application de $G_1$ dans $G_2$ vérifiant les conditions (ii) et (iii) ci-dessus, et analytique dans un voisinage ouvert de $e_1$. Compte tenu de la prop. 20, on démontre, comme pour la prop. 4, que $f$ est un morphisme.

Soient $(G, e, \theta, m)$ un groupuscule de Lie, $\Omega$ l’ensemble de définition de $m$. Soit $H$ une sous-variété de $G$ contenant $e$ et stable par $\theta$. Supposons que l’ensemble $\Omega_1$ des $(x, y) \in \Omega \cap (H \times H)$ tels que $m(x, y) \in H$ soit ouvert dans $H \times H$. Alors $(H, e, \theta|H, m|\Omega_1)$ est un groupuscule de Lie. Un tel groupuscule de Lie s’appelle un *sous-groupuscule de Lie de G*. L’injection canonique de $H$ dans $G$ est un morphisme. Si $f : L \to G$ est un morphisme de groupuscules de Lie tel que $f(L) \subset H$, alors $f : L \to H$ est un morphisme de groupuscules de Lie.

Supposons $K$ de caractéristique 0. Remplaçons l’hypothèse que $H$ est une sous-variété de $G$ par l’hypothèse que $H$ est une quasi-sous-variété de $G$. Ce qu’on a énoncé dans l’alinéa précédent reste valable (cf. VAR, R, 5.8.5). On dit alors que $H$ est un quasi-sous-groupuscule de Lie de $G$.

Si $G$ est un groupuscule de Lie d’élément neutre $e$, tout voisinage ouvert symétrique de $e$ dans $G$ est un sous-groupuscule de Lie de $G$. (Ceci s’applique en particulier lorsque $G$ est un groupe de Lie.) Soit $H$ un sous-groupuscule de Lie de $G$; si $H$ est un voisinage de $e$ dans $G$, alors $H$ est ouvert dans $G$ d’après la prop. 20.

On définit de manière évidente le groupuscule de Lie *produit* d’un nombre fini de groupuscules de Lie.

#### Proposition 21 {#lie-iii-s1-prop-21 .statement}

*Soient $G, H$ deux groupuscules de Lie, $\varphi$ un morphisme de $G$ dans $H$. Les conditions suivantes sont équivalentes*:

(i) $\varphi$ est étale en $e$;
(ii) *il existe des sous-groupuscules de Lie ouverts $G', H'$ de $G, H$ tels que $\varphi|G'$ soit un isomorphisme de $G'$ sur $H'$*.

L’implication (ii) $\Rightarrow$ (i) est évidente. Supposons $\varphi$ étale en $e$. Il existe un sous-groupuscule de Lie ouvert $G_1$ de $G$ tel que $\varphi(G_1)$ soit ouvert dans $H$ et que $\varphi | G_1$ soit un isomorphisme de la variété $G_1$ sur la variété $\varphi(G_1)$. Puis il existe un sous-groupuscule de Lie ouvert $G'$ de $G_1$ tel que le produit dans $G$ de deux éléments de $G'$ soit toujours défini et appartienne à $G_1$. Si $g, g'$ dans $G'$ sont tels que $gg' \in G'$, on a $\varphi(g)\varphi(g') = \varphi(gg') \in \varphi(G')$; si $g, g'$ dans $G'$ sont tels que $gg' \in G_1 - G'$, on a $\varphi(g)\varphi(g') = \varphi(gg') \in \varphi(G_1) - \varphi(G')$. Donc $\varphi|G'$ est un isomorphisme du groupuscule de Lie $G'$ sur le sous-groupuscule de Lie ouvert $\varphi(G')$ de $H$.

Si les conditions de la prop. 21 sont vérifiées, on dit que $G$ et $H$ sont *localement isomorphes*.

#### Proposition 22 {#lie-iii-s1-prop-22 .statement}

*Soient $H$ un groupe de Lie, $U$ un sous-groupuscule de Lie de $H$, $N$ l’ensemble des $g \in H$ tels que $U$ et $gUg^{-1}$ aient même germe en $e$* (TG, I, § 6, n° 10).

Alors $N$ est un sous-groupe de $H$ contenant $U$. Il existe sur $N$ une structure de variété analytique et une seule possédant les propriétés suivantes:

(i) $N$, muni de cette structure, est un groupe de Lie;
(ii) $U$ est une sous-variété ouverte de $N$;
(iii) l’injection canonique de $N$ dans $H$ est une immersion.

Il est clair que $N$ est un sous-groupe de $H$. Si $g \in U$, on a $ge \in U$ et $geg^{-1} \in U$, donc $gu \in U$ et $gug^{-1} \in U$ pour $u$ assez voisin de $e$ dans $U$, donc le germe de $gUg^{-1}$ en $e$ est contenu dans celui de $U$; changeant $g$ en $g^{-1}$, on voit que les germes de $gUg^{-1}$ et de $U$ en $e$ sont égaux. Donc $U \subset N$.

Soit $V$ un voisinage ouvert de $e$ dans $U$ tel que $V = V^{-1},\ V^2 \subset U$. Les conditions (i), (ii), (iii) de la prop. 18 du n° 9 (où l’on remplace $G$ par $N$) sont vérifiées. Donc il existe une structure de variété analytique sur $N$ ayant les propriétés suivantes: $\alpha)$ $N$, muni de cette structure, est un groupe de Lie; $\beta)$ $V$ est ouvert dans $N$; $\gamma)$ les structures de variété de $N$ et $U$ induisent la même structure sur $V$. Puisque $V$ est une sous-variété de $H$, l’injection canonique de $N$ dans $H$ est une immersion en $e$, donc en tout point de $N$. Soit $u \in U$. Il existe un voisinage ouvert $V'$ de $e$ dans $V$ tel que l’application $v \mapsto uv$ soit un isomorphisme analytique de $V'$ sur un voisinage ouvert de $u$ dans $U$ (prop. 20), et en même temps sur un voisinage ouvert de $u$ dans $N$. Donc $U$ est ouvert dans $N$ et l’application identique de $U$ est un isomorphisme pour la structure de variété donnée sur $U$ et la structure de sous-variété ouverte de $N$; autrement dit, $U$ est une sous-variété ouverte de $N$.

Enfin, considérons sur $N$ une structure de variété analytique ayant les propriétés (i) et (ii) de la proposition, et soit $N^*$ le groupe de Lie ainsi obtenu. Alors l’application identique de $N$ dans $N^*$ est étale en $e$, donc est un isomorphisme de groupes de Lie. Cela prouve l’assertion d’unicité de la proposition.

Soient $H$ un groupe de Lie, $U$ un quasi-sous-groupuscule de Lie de $H$, $N$ l’ensemble des $g \in H$ tels que $U$ et $gUg^{-1}$ aient même germe en $e$. Si $K$ est de caractéristique 0, il existe sur $G$ une structure de variété et une seule avec les propriétés (i) et (ii) de la prop. 22. La démonstration est la même que pour la prop. 22.

#### Corollaire {#lie-iii-s1-n10-cor-1 .statement}

Conservons les notations de la prop. 22. Soit $G$ le sous-groupe de $H$ engendré par $U$. Alors $G$ est un sous-groupe ouvert de $N$. Il existe sur $G$ une structure de groupe de Lie et une seule telle que $U$ soit une sous-variété ouverte de $G$ et que l’injection canonique de $G$ dans $H$ soit une immersion.

#### Remarque {#lie-iii-s1-n10-rem-1 .statement}

Conservons les notations de la prop. 22 et de son corollaire. Supposons que $K$ soit de caractéristique 0, que $H$ soit de dimension finie, et que la topologie de $U$ admette une base dénombrable. Même avec toutes ces hypothèses, il se peut que $G$ ne soit pas fermé dans $H$ (exerc. 3). Mais, si $G$ est fermé, $G$ est un sous-groupe de Lie de $H$. En effet, l’application $(g, h) \mapsto gh$ est une loi d’opération à gauche analytique de $G$ dans $H$. L’orbite de $e$ est $G$. Notre assertion résulte alors des prop. 2 (iv) et 14 (iii).

### 11. Morceaux de lois d’opération

Soient (G, e, θ, m) un groupuscule de Lie, X une variété de classe C^r.

#### Définition 6 {#lie-iii-s1-def-6 .statement}

On appelle morceau de loi d’opération à gauche de classe C^r de G dans X une application ψ, définie dans une partie ouverte Ω de G × X contenant {e} × X, à valeurs dans X, et possédant les propriétés suivantes:
(i) ψ est de classe C^r;
(ii) pour tout x ∈ X, on a ψ(e, x) = x;
(iii) il existe un voisinage Ω_1 de {e} × {e} × X dans G × G × X tel que, pour (g, g', x) ∈ Ω_1, les éléments m(g, g'), ψ(g', x), ψ(m(g, g'), x), ψ(g, ψ(g', x)) soient définis et ψ(g, ψ(g', x)) = ψ(m(g, g'), x).

On définit de manière analogue les morceaux de lois d’opération à droite de classe C^r.

On écrit souvent gx au lieu de ψ(g, x).

Soient G' un sous-groupuscule de Lie de G et X' un sous-variété de X. Supposons que l’ensemble Ω' des (g, x) ∈ Ω ∩ (G' × X') tels que ψ(g, x) ∈ X' soit ouvert dans G' × X' (condition toujours remplie si X' est ouvert dans X). Alors ψ|Ω' est un morceau de loi d’opération à gauche de classe C^r de G' dans X', qui est dit déduit de ψ par restriction à G' et X'.

#### Proposition 23 {#lie-iii-s1-prop-23 .statement}

Soient (G, e, θ, m) un groupuscule de Lie, X une variété de classe C^r, x_0 un point de X, Ω un voisinage ouvert de (e, x_0) dans G × X, ψ une application de Ω dans X ayant les propriétés suivantes:
(i) ψ est de classe C^r;
(ii) ψ(e, x) est égal à x pour x assez voisin de x_0;
(iii) ψ(m(g, g'), x) = ψ(g, ψ(g', x)) pour (g, g', x) assez voisin de (e, e, x_0).
Il existe alors un voisinage ouvert X' de x_0 dans X, et une partie ouverte Ω' de Ω ∩ (G × X'), tels que ψ|Ω' soit un morceau de loi d’opération à gauche de classe C^r de G dans X'.

Il existe un voisinage ouvert X' de x_0 dans X et un voisinage ouvert G' de e dans G tels que ψ(e, x) = x pour tout x ∈ X' et que ψ(g, ψ(g', x)) = ψ(m(g, g'), x) pour (g, g', x) ∈ G' × G' × X'. Soit Ω' l’ensemble des (g, x) ∈ Ω ∩ (G' × X') tels que ψ(g, x) ∈ X'. Alors Ω' est ouvert dans G × X', et X', Ω' ont les propriétés de la proposition.

#### Lemme 3 {#lie-iii-s1-lem-3 .statement}

Soient X un espace normal, (X_i)_{i \in I} un recouvrement ouvert localement fini de X. Pour tout (i, j) ∈ I × I et tout x ∈ X_i ∩ X_j, soit V_{ij}(x) un voisinage de x contenu dans X_i ∩ X_j. Alors on peut associer, à tout x ∈ X, un voisinage V(x) de x de telle sorte que les conditions suivantes soient vérifiées:

a) la relation $x \in X_i \cap X_j$ implique $V(x) \subset V_{ij}(x)$;
b) si $V(x)$ et $V(y)$ se rencontrent, il existe un $i \in I$ tel que $V(x) \cup V(y) \subset X_i$.

Il existe un recouvrement ouvert $(X'_i)_{i \in I}$ de $X$ tel que $\overline{X'_i} \subset X_i$ pour tout $i \in I$ (TG, IX, § 4, th. 3). Soit $x \in X$. Soit $V_1(x)$ l’intersection des $V_{ij}(x)$ et des $X'_k$ qui contiennent $x$; c’est un voisinage ouvert de $x$. Soit $V_2(x)$ un voisinage de $x$ contenu dans $V_1(x)$ et ne rencontrant qu’un nombre fini de $X_i$. Alors $V_2(x)$ ne rencontre qu’un nombre fini de $\overline{X'_i}$, donc l’ensemble

$$
V(x) = V_2(x) \cap \bigcap_{i \in I, x \notin \overline{X'_i}} (X - \overline{X'_i})
$$

est un voisinage de $x$. Si $x \in X_i \cap X_j$, on a $V_1(x) \subset X_i \cap X_j$, donc $V(x) \subset X_i \cap X_j$. Soient $x, y$ dans $X$ et supposons que $V(x)$ et $V(y)$ se rencontrent. Il existe un $i \in I$ tel que $x \in X'_i$. Alors $V_1(x) \subset X'_i$, donc $V(x) \subset X'_i$, donc $V(y) \cap \overline{X'_i} \neq \varnothing$. Alors $y \in \overline{X'_i}$ par définition de $V(y)$, d’où $y \in X_i$ et $V(y) \subset X_i$. Ainsi, $X_i$ contient $V(x)$ et $V(y)$.

#### Proposition 24 {#lie-iii-s1-prop-24 .statement}

Soient $G$ un groupuscule de Lie, $X$ une variété de classe $C^r$, $(X_i)_{i \in I}$ un recouvrement ouvert localement fini de $X$. Pour tout $i \in I$, soit $\psi_i$ un morceau de loi d’opération à gauche de classe $C^r$ de $G$ dans $X_i$. On suppose que l’espace topologique sous-jacent à $X$ est normal et que, pour tout $(i, j) \in I \times I$ et tout $x \in X_i \cap X_j$, $\psi_i$ et $\psi_j$ coïncident dans un voisinage de $(e, x)$. Il existe un morceau de loi d’opération à gauche de classe $C^r$ de $G$ dans $X$ tel que, pour tout $i \in I$ et tout $x \in X_i$, $\psi_i$ et $\psi$ coïncident dans un voisinage de $(e, x)$.

Pour tout $(i, j) \in I \times I$ et tout $x \in X_i \cap X_j$, choisissons un voisinage ouvert $V_{ij}(x)$ de $x$ dans $X_i \cap X_j$ tel que $\psi_i$ et $\psi_j$ soient définies et égales sur un voisinage de $\{e\} \times V_{ij}(x)$ dans $G \times X$. Pour tout $x \in X$, choisissons un voisinage ouvert $V(x)$ de $x$ dans $X$ de telle sorte que les conditions a) et b) du lemme 3 soient vérifiées. Soit $I_x$ l’ensemble des $i \in I$ tels que $x \in X_i$. C’est un ensemble fini. Soit $U_x$ l’ensemble des $(g, y) \in G \times V(x)$ tels que les $\psi_i$, pour $i \in I_x$, soient définies et coïncident dans un voisinage de $(g, y)$. Alors $U_x$ est ouvert et $(e, x) \in U_x$. Les $\psi_i$, pour $i \in I_x$, ont toutes même restriction à $U_x$. Soient $x, y$ dans $X$. Si $U_x$ et $U_y$ se rencontrent, $V(x)$ et $V(y)$ se rencontrent, donc il existe $i \in I$ tel que

$$
V(x) \cup V(y) \subset X_i.
$$

Alors $i \in I_x, i \in I_y, \psi_i|U_x = \psi_x, \psi_i|U_y = \psi_y$, donc $\psi_x|(U_x \cap U_y) = \psi_y|(U_x \cap U_y)$. Les $\psi_x$ définissent donc une application $\psi$ de $U = \bigcup_{x \in X} U_x$ dans $X$, et $U$ est un voisinage ouvert de $\{e\} \times X$ dans $G \times X$. Il est clair que $\psi$ est de classe $C^r$ et que $\psi(e, x) = x$ pour tout $x \in X$. Pour tout $i \in I$ et tout $x \in X_i$, $\psi$ coïncide avec $\psi_x$, donc avec $\psi_i$, dans un voisinage de $(e, x)$, donc $\psi$ vérifie la condition (iii) de la déf. 6.

## EXERCICES {#lie-iii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
