---
book: int
book_title: Integration
chapter: IX
chapter_title: MESURES SUR LES ESPACES TOPOLOGIQUES SÉPARÉS
section: 1
section_title: Prémesures et mesures sur un espace topologique
lang: fr
source: int-ix-fr
pdf_pages: 0005-0024, 0098-0099
extraction: ocr
subsections:
    - "no": 1
      title: Encombrements
      page: 0
      pdf_page: 5
    - "no": 2
      title: Prémesures et mesures
      page: 0
      pdf_page: 6
    - "no": 3
      title: Exemples de mesures
      page: 0
      pdf_page: 9
    - "no": 4
      title: Ensembles et fonctions localement négligeables
      page: 0
      pdf_page: 11
    - "no": 5
      title: Ensembles et fonctions mesurables
      page: 0
      pdf_page: 12
    - "no": 6
      title: Familles filtrantes; support d’une mesure
      page: 0
      pdf_page: 13
    - "no": 7
      title: Enveloppes supérieures et sommes de mesures
      page: 0
      pdf_page: 15
    - "no": 8
      title: Concassages
      page: 0
      pdf_page: 16
    - "no": 9
      title: Intégrale supérieure
      page: 0
      pdf_page: 19
    - "no": 10
      title: Théorie de l’intégration
      page: 0
      pdf_page: 22
statements: 51
exercises: 10
content_sha256: cf41fb60f0d46e9f933e1b74399ab40bbc279a155d5448cc76ec34e6ae1f277a
---

## § 1. Prémesures et mesures sur un espace topologique

### 1. Encombrements

#### Définition 1 {#int-ix-s1-def-1 .statement}

Soit T un ensemble. On appelle encombrement sur T toute application p de $\mathcal{F}_+(T)$ dans $\overline{\mathbf{R}}_+$ qui possède les propriétés suivantes:

a) Si f et g sont deux éléments de $\mathcal{F}_+$ tels que $f \leqslant g$, on a $p(f) \leqslant p(g)$.
b) Si f est un élément de $\mathcal{F}_+$, et t un nombre $\geqslant 0$, on a $p(tf) = tp(f)$.
c) Si f et g sont deux éléments de $\mathcal{F}_+$, on a $p(f + g) \leqslant p(f) + p(g)$.
d) Si $(f_n)$ est une suite croissante d’éléments de $\mathcal{F}_+$, et si $f = \lim_{n \to \infty} f_n$, on a $p(f) = \lim_{n \to \infty} p(f_n)$.

Si A est une partie de T, on écrit $p(A)$ au lieu de $p(\varphi_A)$.

La condition b) entraîne $p(0) = 0$. D’autre part, soit $(f_n)$ une suite d’éléments de $\mathcal{F}_+$; les conditions c) et d) entraînent l’inégalité

$$
p \left( \sum_n f_n \right) \leqslant \sum_n p(f_n) \quad \text{(«inégalité de convexité dénombrable»)}.
$$

Par exemple, soient T un espace localement compact, $\mu$ une mesure positive sur T; alors $\mu^*$ et $\mu^*$ sont des encombrements sur T. Cela résulte des prop. 10, 11, 12 et du th. 3 du chap. IV, 2e éd., § 1, n° 3 pour $\mu^*$, et de la prop. 1 du chap. V, 2e éd., § 1, n° 1 pour $\mu^*$.

#### Proposition 1 {#int-ix-s1-prop-1 .statement}

*Soit* $(p_\alpha)_{\alpha \in A}$ *une famille d’encombrements sur* T. *La somme et l’enveloppe supérieure de la famille* $(p_\alpha)$ *(dans* $\mathcal{F}_+ (\mathcal{F}_+ (T))$) *sont alors des encombrements*.

La somme d’une famille finie d’encombrements étant évidemment un encombrement, il suffit de traiter le cas de l’enveloppe supérieure. Les propriétés $a), b), c)$ de la définition 1 étant évidemment satisfaites, il reste à établir d). Posons $p = \sup_\alpha p_\alpha$; on a, avec les notations de la définition 1, d)

$$
p(f) = \sup_\alpha p_\alpha(f) = \sup_\alpha \sup_n p_\alpha(f_n) = \sup_n \sup_\alpha p_\alpha(f_n) = \sup_n p(f_n).
$$

#### Définition 2 {#int-ix-s1-def-2 .statement}

*Soit* p *un encombrement sur un ensemble* T. *On dit que* p *est borné si* $p(T) < +\infty$. *Si* T *est un espace topologique, on dit que* p *est localement borné si tout* $x \in T$ *admet un voisinage* V *tel que* $p(V) < +\infty$.

Il résulte alors des propriétés a) et c) de la déf. 1 que $p(K) < +\infty$ pour toute partie compacte K de T. En particulier, si T est compact, tout encombrement localement borné sur T est borné.

Soient p un encombrement sur un ensemble T, et A une partie de T. Pour toute fonction $f \in \mathcal{F}_+(A)$, soit $f^0$ le prolongement par 0 de f à T; l’application $f \mapsto p(f^0)$ sur $\mathcal{F}_+(A)$ est alors un encombrement, qu’on appelle *l’encombrement induit par* p *sur* A, et qu’on note $p|A$ ou $p_A$.

Soient T et U deux ensembles, $\pi$ une application de T dans U et p un encombrement sur T. On appelle *encombrement image* de p par $\pi$ l’encombrement $\pi(p)$ sur U, dont la valeur pour $f \in \mathcal{F}_+(U)$ est donnée par

$$
(\pi(p))(f) = p(f \circ \pi).
$$

Soit p un encombrement sur un ensemble T; on dit que p est *concentré* sur une partie A de T si $p(T - A) = 0$.

#### Lemme 1 {#int-ix-s1-lem-1 .statement}

*Si l’encombrement* p *est concentré sur* A $\subset$ T, *on a* $p(f) = p(f \varphi_A)$ *pour tout* $f \in \mathcal{F}_+(T)$.

Posons en effet $T - A = B$, d’où $p(\varphi_B) = 0$; on a

$$
f \varphi_B \leq (+\infty) \cdot \varphi_B = \sup_{n \in \mathbf{N}} n \varphi_B,
$$

donc $p(f \varphi_B) = 0$ d’après les propriétés $a), b), d)$, de la déf. 1. Il en résulte que $p(f) \leq p(f \varphi_A) + p(f \varphi_B) = p(f \varphi_A)$ d’après c), et enfin $p(f) = p(f \varphi_A)$ d’après a).

### 2. Prémesures et mesures

Soit T un espace topologique, et soit $\mathfrak{A}$ l’ensemble des parties compactes de T, ordonné par inclusion. Pour tout $K \in \mathfrak{A}$, soit $\mathcal{M}(K; \mathbf{C})$ l’ensemble des mesures complexes sur K. Pour tout couple (K, L) d’éléments de $\mathfrak{A}$, tel que $K \subset L$, soit $t_{KL}$ l’application de $\mathcal{M}(L; \mathbf{C})$ dans $\mathcal{M}(K; \mathbf{C})$ qui associe à toute mesure $\mu$ sur L la mesure $\mu_K$ induite par $\mu$ sur K (chap. IV, 2e éd., § 5, n° 7, déf. 4). On a $t_{KM} = t_{KL} \circ t_{LM}$ lorsque K, L et M sont des parties compactes de T telles que $K \subset L \subset M$; ceci résulte de la transitivité des mesures induites (chap. V, 2e éd., § 7, n° 2, prop. 4). Les éléments de la limite projective de la famille $(\mathcal{M}(K; \mathbf{C}))_{K \in \mathfrak{A}}$ pour les applications $t_{KL}$ seront appelés prémesures sur T. Autrement dit:

#### Définition 3 {#int-ix-s1-def-3 .statement}

On appelle prémesure sur un espace topologique T toute application w qui associe, à toute partie compacte K de T, une mesure $w_K$ sur K, et qui possède la propriété suivante :

Si K et L sont deux parties compactes de T telles que $K \subset L$, la mesure $(w_L)_K$ induite par $w_L$ sur K est égale à $w_K$.
On dit que la prémesure w est réelle (resp. positive) si toutes les mesures $w_K$ sont réelles (resp. positives).

Soient w et w' deux prémesures sur T, t un nombre complexe; on définit les prémesures $w + w'$ et $tw$ par les formules $(w + w')_K = w_K + w'_K, (tw)_K = tw_K$ pour toute partie compacte $K \subset T$. Les prémesures sur T forment évidemment un espace vectoriel, noté $\mathcal{P}(T; \mathbf{C})$; l’espace des prémesures réelles sera noté $\mathcal{P}(T; \mathbf{R})$ ou plus souvent $\mathcal{P}(T)$, et le cône convexe des prémesures positives sera désigné par la notation $\mathcal{P}_+(T)$. Soit w une prémesure; l’application $K \mapsto |w_K|$ est alors une prémesure sur T (chap. IV, 2e éd., § 5, n° 7, lemme 3) que l’on notera $|w|$. Si w est réelle, on posera $w^+ = \frac{1}{2}(|w| + w), w^- = \frac{1}{2}(|w| - w)$; ces deux prémesures étant positives, on voit que toute prémesure réelle est différence de deux prémesures positives. On a évidemment $(w^+)_K = (w_K)^+, (w^-)_K = (w_K)^-$ pour toute partie compacte K de T.

L’espace vectoriel $\mathcal{P}(T)$ est ordonné par le cône $\mathcal{P}_+(T)$. Il est clair qu’on a $w^+ = \sup (w, 0), w^- = \sup (-w, 0)$; par suite, $\mathcal{P}(T)$ est réticulé et $\sup (w, w') = w + (w' - w)^+$, $\inf (w, w') = w - (w' - w)^-$. De plus, on a évidemment
$$
(\sup (w, w'))_K = \sup (w_K, w'_K), \quad (\inf (w, w'))_K = \inf (w_K, w'_K),
$$
pour toute partie compacte K de T.

#### Définition 4 {#int-ix-s1-def-4 .statement}

Soit w une prémesure positive sur T. Nous poserons pour toute fonction $f \in \mathcal{F}_+(T)$
(1)
$$
w^*(f) = \sup_K (w_K)^*(f_K),
$$
K parcourant l’ensemble des parties compactes de T.

Pour chaque ensemble compact K, soit $p^K$ l’encombrement image de l’encombrement $(w_K)^*$ par l’injection canonique de K dans T; $w^*$ est l’enveloppe supérieure des encombrements $p^K$, c’est donc un encombrement (n° 1, prop. 1).

On dit que $w^\bullet$ est l'intégrale supérieure essentielle associée à la prémesure positive $w$. On écrit fréquemment $\int^\bullet f\,dw, \int^\bullet f(t)\,dw(t)$ au lieu de $w^\bullet(f)$.

Remarque 1). — Si $v$ et $w$ sont deux prémesures positives, on a $(v + w)^\bullet = v^\bullet + w^\bullet$ (chap. V, 2e éd., § 1, n° 1, prop. 3). Si $v$ et $w$ sont deux prémesures complexes, on a $|v + w|^\bullet \leq |v|^\bullet + |w|^\bullet$.

#### Proposition 2 {#int-ix-s1-prop-2 .statement}

a) Soit $w$ une prémesure positive. Pour toute partie compacte $K$ de $T$, l’encombrement $(w^\bullet)_K$ induit par $w^\bullet$ sur $K$ est égal à $(w_K)^\bullet$. Pour toute fonction $f \in \mathcal{F}_+(T)$, on a les relations $(w_K)^\bullet(f_K) = w^\bullet(f_{\varphi_K})$ et
$$
w^\bullet(f) = \sup_K w^\bullet(f_{\varphi_K}).
$$
(2)

b) Inversement, soit $p$ un encombrement sur $T$ satisfaisant aux conditions suivantes:
1) Pour toute partie compacte $K$ de $T$, il existe une mesure positive $w_K$ sur $K$ telle que $p_K = (w_K)^\bullet$.
2) Pour toute fonction $f \in \mathcal{F}_+(T)$, on a $p(f) = \sup_K p(f_{\varphi_K})$.

L’application $w : K \mapsto w_K$ est alors une prémesure positive sur $T$, et on a $p = w^\bullet$.

Démontrons a): soient $g \in \mathcal{F}_+(K)$ et $g^0$ le prolongement par zéro de $g$ à $T$; on a, d’après la définition des encombremens induits, $(w^\bullet)_K(g) = w^\bullet(g^0) = \sup_L (w_L)^\bullet(g^0|L)$, $L$ parcourant l’ensemble des parties compactes de $T$, ou seulement l’ensemble de celles qui contiennent $K$. Mais si $L$ contient $K$, on a $(w_L)^\bullet(g^0|L) = (w_K)^\bullet(g)$ du fait que $g^0|L$ est nulle hors de $K$ (chap. V, 2e éd., § 7, n° 1, prop. 1), ce qui prouve la première assertion. On a donc $(w_K)^\bullet(f_K) = (w^\bullet)_K(f_K) = w^\bullet((f_K)^0) = w^\bullet(f_{\varphi_K})$ pour tout $f \in \mathcal{F}_+(T)$, et (2) ne fait que traduire la formule (1).

Passons à b): la mesure $w_K$ considérée en 1) est unique (chap. V, 2e éd., § 1, n° 1). Montrons que l’application $K \mapsto w_K$ est une prémesure: soient $K$ et $L$ deux parties compactes telles que $K \subset L$, et soit $\lambda$ la mesure induite par $w_L$ sur $K$; tout revient à montrer que $\lambda^\bullet = (w_K)^\bullet$. Or on a $\lambda^\bullet = ((w_L)^\bullet)_K$ (chap. V, 2e éd., § 7, n° 1, prop. 1); comme $(w_L)^\bullet = p_L$, on a $\lambda^\bullet = (p_L)_K = p_K = (w_K)^\bullet$.

Notons $w$ la prémesure $K \mapsto w_K$; comme $p_K = (w_K)^\bullet = (w^\bullet)_K$, on a $p(f_{\varphi_K}) = p_K(f_K) = (w^\bullet)_K(f_K) = w^\bullet(f_{\varphi_K})$. Les deux encombremens $p$ et $w^\bullet$ sont alors égaux en vertu de la formule (2) et de l’hypothèse 2) sur $p$.

C.Q.F.D.

L’encombrement induit $(w^\bullet)_K$ étant égal à $(w_K)^\bullet$, il n’y a aucune ambiguïté à écrire simplement $w_K^\bullet$. Nous emploierons cette notation dans toute la suite.

#### Corollaire {#int-ix-s1-n2-cor-1 .statement}

Soient $v$ et $w$ deux prémesures positives sur $T$, telles que $v^\bullet(L) = w^\bullet(L)$ pour toute partie compacte $L$ de $T$; on a alors $v = w$. En particulier, la relation $v^\bullet = w^\bullet$ entraîne $v = w$.

En effet, soit $K$ un ensemble compact dans $T$; on a, pour tout ensemble compact $L \subset K$, la relation
$$
w_K(L) = w_K^\bullet(L) = w^\bullet(L) = v^\bullet(L) = v_K^\bullet(L) = v_K(L)
$$

d’après la prop. 2; on a donc $w_K = v_K$ (chap. IV, 2e éd., § 4, n° 10, cor. 3 de la prop. 19), et enfin $w = v$ par la définition des prémesures.

#### Définition 5 {#int-ix-s1-def-5 .statement}

Soit $w$ une prémesure sur un espace topologique $T$. On dit que $w$ est une mesure (resp. une mesure bornée) si l’encombrement $|w|^*$ est localement borné (resp. borné) (cf. n° 1, déf. 2).

L’ensemble des mesures complexes sur $T$ est évidemment un espace vectoriel (Remarque 1), qui sera noté $\mathcal{M}(T; \mathbf{C})$. L’espace des mesures réelles sera noté $\mathcal{M}(T; \mathbf{R})$ ou plus souvent $\mathcal{M}(T)$, et on désignera par $\mathcal{M}_+(T)$ le cône des mesures positives.

Si $w$ est une mesure complexe, sa partie réelle et sa partie imaginaire sont des mesures réelles. Si $w$ est une mesure réelle, $w^+$ et $w^-$ sont des mesures positives. Toute mesure complexe (resp. réelle) est donc combinaison linéaire (resp. différence) de mesures positives.

#### Remarque 2 {#int-ix-s1-n2-rem-2 .statement}

Si $T$ est localement compact, toute prémesure $w$ sur $T$ est une mesure. En effet, tout $x \in T$ admet un voisinage compact $K$, et on a $|w|^*(K) = \|w_K\| < +\infty$, de sorte que l’encombrement $|w|^*$ est localement borné.

#### Remarque 3 {#int-ix-s1-n2-rem-3 .statement}

Pour toute partie borélienne $A$ de $T$ (en particulier pour $A = T$), et toute mesure positive $\mu$ sur $T$, le nombre $\mu^*(A)$ est la borne supérieure des mesures $\mu^*(K)$ des parties compactes de $A$. En effet, pour toute partie compacte $K$ de $A$, on a $\mu^*(K) \leq \mu^*(A)$; d’autre part, si $\mathfrak{K}$ est l’ensemble des parties compactes de $T$, on a
$$
\mu^*(A) = \sup_{K \in \mathfrak{K}} \mu_K^*(A \cap K) = \sup_{K \in \mathfrak{K}} \sup_{L \in \mathfrak{K}, L \subseteq A \cap K} \mu_K^*(L) \leq \sup_{L \in \mathfrak{K}, L \subseteq A} \mu^*(L)
$$
d’après le cor. 1 du th. 4 du chap. IV, § 4, n° 6 (2e éd.).

### 3. Exemples de mesures

#### Exemple 1 {#int-ix-s1-n3-exa-1 .statement}

Mesures sur un espace localement compact

La proposition suivante montre que la théorie de ce chapitre contient celle du chap. IV. Dans l’énoncé, le mot « mesure » et la notation $\mathcal{M}(T; \mathbf{C})$ sont pris au sens des chapitres antérieurs.

#### Proposition 3 {#int-ix-s1-prop-3 .statement}

Soit $T$ un espace localement compact, et soit $\mu$ une mesure sur $T$. Désignons par $W(\mu)$ l’application qui à chaque partie compacte $K$ de $T$ associe la mesure induite $\mu_K$. Alors $W(\mu)$ est une prémesure sur $T$, on a $W(|\mu|) = |W(\mu)|$, et l’application linéaire $W : \mu \mapsto W(\mu)$ est une bijection de l’espace $\mathcal{M}(T; \mathbf{C})$ sur l’espace $\mathcal{P}(T; \mathbf{C})$ des prémesures sur $T$. En outre, si $\mu$ est positive, on a $\mu^* = (W(\mu))^*$.

Il est évident que $W(\mu)$ est une prémesure (chap. V, 2e éd., § 7, n° 2, prop. 4), et que l’application $W$ est linéaire. La relation $W(\mu) = 0$ signifie que $\mu$ induit la mesure 0 sur tout ensemble compact dans $T$; on a alors $\mu(f) = 0$ pour $f \in \mathcal{H}(T; \mathbf{C})$, donc $\mu = 0$, ce qui prouve que $W$ est injective. Reste à prouver que $W$ est surjective. Comme toute prémesure est combinaison linéaire de prémesures positives, il nous suffira de construire, pour toute prémesure positive $w$, une mesure positive $\mu$ telle que $w = W(\mu)$. Soit donnée une fonction $f \in \mathcal{K}(T)$, et soit $L$ un ensemble compact contenant le support de $f$; le nombre $w_L(f_L)$ ne dépend pas du choix de $L$, d’après la définition des mesures induites, et l’on peut donc poser $\mu(f) = w_L(f_L)$; alors $\mu$ est une forme linéaire positive sur $\mathcal{K}(T)$, c’est-à-dire une mesure positive. Vérifions que $w = W(\mu)$; tout d’abord, la relation $\mu^*(f) = w_L^*(f_L)$ s’étend au cas où $f$ est une fonction finie semi-continue supérieurement, positive, nulle hors de $L$. En effet, soient $M$ un voisinage compact de $L$, et $\mathcal{H}$ l’ensemble (filtrant décroissant) des fonctions continues sur $T$, à support contenu dans $M$, qui majorent $f$. On a (chap. IV, 2e éd., § 4, n° 4, cor. 2 de la prop. 5)

$$
\mu^*(f) = \inf_{h \in \mathcal{H}} \mu(h) = \inf_{h \in \mathcal{H}} w_M(h_M) = w_M^*(f_M)
$$

et d’autre part $w_M^*(f_M) = w_L^*(f_L)$ puisque $f_M$ est nulle dans $M - L$ (chap. V, 2e éd., § 7, n° 1, prop. 1). En particulier, si l’on prend pour $f$ le prolongement par 0 d’un élément de $\mathcal{K}_+(L)$, cette formule montre que $\mu_L = w_L$ d’après la définition des mesures induites, et on a donc bien $W(\mu) = w$.

Si $\mu$ est positive, on a

$$
\mu^*(f) = \sup_K \mu^*(f_{\varphi_K}) = \sup_K \mu_K^*(f_K) = (W(\mu))^*(f)
$$

pour tout $f \in \mathcal{F}_+(T)$ (chap. V, 2e éd., § 1, déf. 1 et § 7, prop. 1). La relation $|W(\mu)| = W(|\mu|)$ est évidente (chap. IV, 2e éd., § 5, n° 7, lemme 3).

C.Q.F.D.

Lorsque $T$ est *localement compact*, nous *identifierons* dans toute la suite les espaces $\mathcal{M}(T; \mathbf{C})$ et $\mathcal{P}(T; \mathbf{C})$ au moyen de la bijection $W$.

#### Exemple 2 {#int-ix-s1-n3-exa-2 .statement}

*Mesures à support compact sur un espace topologique.*

#### Lemme 2 {#int-ix-s1-lem-2 .statement}

*Soient* $T$ *un espace topologique, L une partie compacte de* $T$, $\lambda$ *une mesure positive sur* $L$. *Il existe une mesure positive unique* $\mu$ *sur* $T$, *telle que l’on ait, pour toute fonction* $f \in \mathcal{F}_+(T)$,

(3)
$$
\mu^*(f) = \lambda^*(f_L).
$$

Posons en effet $p(f) = \lambda^*(f_L)$ pour tout $f \in \mathcal{F}_+(T)$, et montrons que les conditions 1) et 2) de la prop. 2, *b*) sont vérifiées. La seconde est évidemment vérifiée: on a en fait $p(f) = p(f_{\varphi_K})$ si $K$ contient $L$. Si $K \subset T$ est compact, et si $h \in \mathcal{F}_+(K)$, on a

$$
p_K(h) = p(h^0) = \lambda^*(h^0|L).
$$

Mais $h^0|L$ est le prolongement par 0 de $h_{K \cap L}$ à $L$: la dernière expression est donc égale à $\mu_K(h)$, où $\mu_K$ est l’image de $\lambda|(K \cap L)$ par l’injection de $K \cap L$ dans $K$ (chap. V, 2e éd., § 6, n° 2, prop. 2 et § 7, n° 1, prop. 1) et l’on a $p_K = (\mu_K)^*$. La condition 1) de la prop. 2, *b*) est donc aussi vérifiée, et l’existence de $\mu$ en résulte aussitôt.

C.Q.F.D.

On dira que $\mu$ est la mesure sur $T$ définie par $\lambda$. En particulier, pour tout point $x$ de $T$, on peut définir la mesure $\varepsilon_x$; elle est caractérisée par $(\varepsilon_x)^*(f) = f(x)$ pour $f \in \mathcal{F}_+(T)$.

#### Remarque 1 {#int-ix-s1-n3-rem-1 .statement}

Lorsque $T$ est localement compact, $\mu$ est l’image de $\lambda$ par l’injection de $L$ dans $T$. Nous verrons au § 2, n° 3, Exemple 1, lorsque les mesures images auront été traitées, que cette interprétation vaut encore pour des espaces quelconques.
2) Nous verrons aussi que les mesures définies dans l’Exemple 2 sont les mesures positives à support compact dans $T$ (n° 6, Remarque 2)).

Nous ne considérerons plus désormais que des mesures positives, sauf mention expresse du contraire. Dans toute la suite de ce paragraphe, $T$ désignera un espace topologique et $\mu$ une mesure positive sur $T$.

De nombreux résultats des n°s suivants s’étendent aux prémesures positives. Cette extension est laissée au lecteur.

### 4. Ensembles et fonctions localement négligeables

#### Définition 6 {#int-ix-s1-def-6 .statement}

On dit qu’une fonction $f \in \mathcal{F}_+$ (resp. une partie $A$ de $T$) est localement négligeable pour la mesure $\mu$ si $\mu^*(f) = 0$ (resp. $\mu^*(A) = 0$). On dit que $\mu$ est concentrée sur une partie $A$ de $T$ si $T - A$ est localement $\mu$-négligeable.

#### Remarque 1 {#int-ix-s1-n4-rem-1 .statement}

Les notions ainsi définies coïncident, lorsque $T$ est localement compact, avec les notions usuelles.
2) Lorsque nous aurons défini les ensembles négligeables, nous verrons que les ensembles localement négligeables sont bien ceux dont le germe, en tout point de $T$, est un germe d’ensemble négligeable (n° 9, cor. 2 de la prop. 14).
3) Comme aux chap. IV et V, l’expression « localement presque partout » sera synonyme de « sauf sur un ensemble localement négligeable ».
4) Si $\theta$ est une mesure complexe, on dira qu’une fonction (resp. une partie de $T$) est localement négligeable pour $\theta$ si elle l’est pour la mesure positive $|\theta|$.
Exemple. — Soient $L$ une partie compacte de $T$, $\lambda$ une mesure sur $L$, et $\mu$ la mesure sur $T$ définie par $\lambda$ (n° 3, Exemple 2). La formule (3) entraîne aussitôt qu’une fonction $f \in \mathcal{F}_+(T)$ est localement $\mu$-négligeable si et seulement si $f_L$ est $\lambda$-négligeable.

Il résulte immédiatement de la formule (1) qu’une fonction $f \in \mathcal{F}_+(T)$ est localement $\mu$-négligeable si et seulement si $f_K$ est $\mu_K$-négligeable pour toute partie compacte $K$ de $T$. Les propriétés des ensembles localement négligeables se ramènent donc aussitôt à celles des ensembles négligeables dans les espaces compacts, traitées au chap. IV. Voici quelques résultats qui seront utilisés par la suite sans autre référence.

— Pour qu’une fonction $f \geqslant 0$ soit localement négligeable, il faut et il suffit que $f(t) = 0$ localement presque partout (chap. IV, 2e éd., § 2, n° 3, th. 1). Si $\mathbf{f}$ est une fonction à valeurs dans un espace de Banach, il est donc équivalent de dire que $\mathbf{f} = 0$ localement presque partout, ou que $\mu^*(|\mathbf{f}|) = 0$; nous dirons encore dans ce cas que $\mathbf{f}$ est localement négligeable.
— La somme et l’enveloppe supérieure d’une suite de fonctions $\geqslant 0$, localement négligeables, sont localement négligeables (loc. cit., n° 1, prop. 2).

— Si $f$ et $g$ sont deux fonctions $\geqslant 0$ égales localement presque partout, on a $\mu^*(f) = \mu^*(g)$ (*loc. cit.*, n° 3, prop. 6).

### 5. Ensembles et fonctions mesurables

#### Définition 7 {#int-ix-s1-def-7 .statement}

*On dit qu'une fonction* $f$ *définie dans* $T$, *à valeurs dans un espace topologique* $F$ *(séparé ou non)* *est mesurable pour la mesure* $\mu$ *(ou* $\mu$-*mesurable)* *si, pour toute partie compacte* $K$ *de* $T$, *la fonction* $f_K$ *est* $\mu_K$*-mesurable*.

Cela revient à dire qu'il existe, pour tout ensemble compact $K$, une partition de $K$ en un ensemble $\mu_K$-négligeable $N$ et une suite $(K_n)$ d'ensembles compacts, tels que la restriction de $f$ à chacun des $K_n$ soit continue. Comme il est équivalent de dire que $N$ est $\mu_K$-négligeable, ou localement $\mu$-négligeable (n° 4), on voit que $f$ est $\mu$-mesurable si et seulement si, pour tout ensemble compact $K$, il existe une partition de $K$ en un ensemble localement $\mu$-négligeable $N$ et une suite $(K_n)$ d'ensembles compacts telle que $f_{K_n}$ soit continue pour tout $n$. Cette définition est identique à la déf. 1 du chap. IV, 2e éd., § 5, n° 1, et on retrouve donc la notion habituelle de fonction mesurable lorsque $T$ est localement compact.

On dit qu'une partie $A$ de $T$ est mesurable si sa fonction caractéristique est mesurable. Si $A$ est $\mu$-mesurable, et si $\mu^*(A) < +\infty$, ce nombre est noté simplement $\mu(A)$ et appelé la *mesure* de $A$. On écrit de même $\mu(f)$ pour $\mu^*(f)$ si $f$ est $\mu$-mesurable $\geqslant 0$ et si $\mu^*(f) < +\infty$.

Si $\theta$ est une mesure complexe sur $T$, on dit qu'une fonction $f$ (resp. une partie de $T$) est $\theta$-mesurable si elle est mesurable pour la mesure positive $|\theta|$. Les résultats ci-dessous s'étendent aux mesures complexes.

#### Exemple {#int-ix-s1-n5-exa-1 .statement}

Soient $L$ une partie compacte de $T$, $\lambda$ une mesure sur $L$ et $\mu$ la mesure sur $T$ définie par $\lambda$ (n° 3, *Exemple* 2). Une fonction $f$ définie dans $T$ est $\mu$-mesurable si et seulement si $f_L$ est $\lambda$-mesurable. En effet, cette condition est évidemment nécessaire. Inversement, si elle est vérifiée, il existe une partition de $L$ en un ensemble $\lambda$-négligeable $N$ et une suite $(L_n)$ d'ensembles compacts, tels que $f_{L_n}$ soit continue pour tout $n$. Si $K$ est une partie compacte de $T$, l'ensemble $K - \bigcup_n (K \cap L_n)$ a une intersection avec $L$ qui est $\lambda$-négligeable, donc cet ensemble est $\mu$-négligeable d'après la formule (3) du n° 3, et la restriction de $f$ à $K \cap L_n$ est continue pour tout $n$.

La déf. 7 permet d'étendre, sans nouvelle démonstration, nombre de résultats sur les fonctions mesurables au cas des espaces non localement compacts. En voici quelques-uns, que nous utiliserons par la suite sans autre référence : les ensembles ouverts, les ensembles fermés de $T$ sont $\mu$-mesurables ; les ensembles $\mu$-mesurables forment une tribu (chap. IV, 2e éd., § 5, n° 4, cor. 2 du th. 2), qui contient les ensembles boréliens de $T$ (*loc. cit.*, cor. 3), et les ensembles sousliniens (chap. IV, § 5, n° 1, cor. 2 de la prop. 3)(1). Les opérations algébriques usuelles sur les fonctions numériques préservent la mesurabilité (chap. IV, 2e éd., § 5, n° 3), ainsi que les opérations de passage à la limite dénombrable (*loc. cit.*, n° 4, th. 2 et cor. 1). La propriété suivante mérite une mention plus explicite :

1. La démonstration de ce corollaire est valable sans modification pour les ensembles sousliniens dans un espace localement compact non métrisable (*Top. gén.*, chap. IX, 3e éd., § 6, n° 9, th. 5).

#### Proposition 4 {#int-ix-s1-prop-4 .statement}

Soient f une fonction positive et $(g_n)_{n \geq 1}$ une suite de fonctions positives $\mu$-mesurables sur T. Si l’on pose $g = \sum_{n \geq 1} g_n$, on a
$$
\mu^\bullet(fg) = \sum_{n \geq 1} \mu^\bullet(fg_n).
$$
(4)
Posons $h_n = \sum_{i=1}^n g_i$ pour tout $n \geq 1$. Pour toute partie compacte K de T, on a
$$
\mu_K^\bullet((fh_n)_K) = \sum_{i=1}^n \mu_K^\bullet((f g_i)_K)
$$
d’après la prop. 2 du chap. V, 2e éd., § 1, n° 1 appliquée à l’espace compact K. Passant à la limite selon l’ensemble filtrant croissant des parties compactes de T, on obtient
$$
\mu^\bullet(fh_n) = \sum_{i=1}^n \mu^\bullet(f g_i).
$$
Or $fg$ est la limite de la suite croissante $(fh_n)_{n \geq 1}$, d’où $\mu^\bullet(fg) = \lim_{n \to \infty} \mu^\bullet(fh_n)$; la formule précédente entraîne alors immédiatement (4).

#### Corollaire {#int-ix-s1-n5-cor-1 .statement}

Soit $(A_n)$ une suite de parties mesurables deux à deux disjointes, de réunion A. Pour toute partie B de T, on a
$$
\mu^\bullet(A \cap B) = \sum_n \mu^\bullet(A_n \cap B)
$$
et en particulier
$$
\mu^\bullet(A) = \sum_n \mu^\bullet(A_n).
$$

Parmi les propriétés des fonctions ou ensembles mesurables qui s’étendent comme ci-dessus aux espaces séparés, citons aussi la prop. 12 du chap. IV, 2e éd., § 5, n° 8 (familles $\mu$-denses d’ensembles compacts). Ainsi, une fonction $f$ à valeurs dans un espace topologique (séparé ou non) est $\mu$-mesurable si et seulement si l’ensemble des parties compactes K de T, telles que $f_K$ soit continue, est $\mu$-dense (*loc. cit.*, n° 10, prop. 15).

### 6. Familles filtrantes; support d’une mesure

#### Proposition 5 {#int-ix-s1-prop-5 .statement}

a) Soit H un ensemble filtrant croissant de fonctions $\geq 0$, semi-continues inférieurement dans toute partie compacte de T. On a alors
$$
\mu^\bullet(\sup_{h \in H} h) = \sup_{h \in H} \mu^\bullet(h).
$$
(5)
b) Soit H un ensemble filtrant décroissant de fonctions $\geq 0$, semi-continues supérieurement dans tout compact de T. S’il existe dans H une fonction $h_0$ telle que $\mu^\bullet(h_0) < +\infty$, on a
$$
\mu^\bullet(\inf_{h \in H} h) = \inf_{h \in H} \mu^\bullet(h).
$$
(6)

Nous avons en effet, pour tout ensemble compact $K \subset T$

$$
\mu^*(\sup_{h \in H} h \varphi_K) = \mu_K^*(\sup_{h \in H} h_K) = \sup_{h \in H} \mu_K^*(h_K) = \sup_{h \in H} \mu^*(h \varphi_K)
$$

dans le cas a) et

$$
\mu^*(\inf_{h \in H} h \varphi_K) = \mu_K^*(\inf_{h \in H} h_K) = \inf_{h \in H} \mu_K^*(h_K) = \inf_{h \in H} \mu^*(h \varphi_K)
$$

dans le cas b) d’après la prop. 2 du n° 2, et la prop. 8 du chap. V, 2e éd., § 1, n° 2. Le cas a) s’en déduit aussitôt, par passage à la borne supérieure par rapport à $K$ (n° 2, prop. 2). Pour traiter le cas b), désignons par $\varepsilon$ un nombre $> 0$, et choisissons l’ensemble compact $K$ tel que l’on ait $\mu^*(h_0 \varphi_K) \geq \mu^*(h_0) - \varepsilon$. Nous avons alors (n° 5, prop. 4) $\mu^*(h_0 \varphi_K) \leq \varepsilon$; pour toute fonction $h \in H$ majorée par $h_0$, on a donc $\mu^*(h \varphi_K) \leq \varepsilon$, et finalement $\mu^*(h \varphi_K) \geq \mu^*(h) - \varepsilon$ d’après la prop. 4 du n° 5. Par conséquent, on a

$$
\mu^*(\inf_{h \in H} h) \geq \mu^*(\inf_{h \in H} h \varphi_K) = \inf_{\substack{h \in H \\ h \leq h_0}} \mu^*(h \varphi_K) \geq \inf_{\substack{h \in H \\ h \leq h_0}} \mu^*(h) - \varepsilon.
$$

Par conséquent, le premier membre de (6) majore le second; l’inégalité inverse étant évidente, la proposition est établie.

#### Corollaire {#int-ix-s1-n6-cor-1 .statement}

a) Soit $(\mathbf{U}_\alpha)_{\alpha \in I}$ une famille filtrante croissante de parties ouvertes de $T$, de réunion $U$. On a $\mu^*(U) = \sup_{\alpha \in I} \mu^*(\mathbf{U}_\alpha)$.

b) Soit $(\mathbf{F}_\alpha)_{\alpha \in I}$ une famille filtrante décroissante de parties fermées de $T$, d’intersection $F$. S’il existe $\alpha \in I$ tel que $\mu^*(\mathbf{F}_\alpha)$ soit fini, on a $\mu^*(F) = \inf_{\alpha \in I} \mu^*(\mathbf{F}_\alpha)$.

D’après le cor. précédent, il existe un plus grand ouvert localement négligeable; ceci justifie la définition suivante:

#### Définition 8 {#int-ix-s1-def-8 .statement}

On appelle support d’une mesure $\mu$ sur $T$ le complémentaire du plus grand ensemble ouvert localement $\mu$-négligeable de $T$.

Le support de $\mu$ est désigné par la notation $\operatorname{Supp}(\mu)$.

#### Remarque 1 {#int-ix-s1-n6-rem-1 .statement}

Si $\mu$ est une mesure complexe, on appelle support de $\mu$ le support de la mesure positive $|\mu|$; c’est encore le complémentaire du plus grand ensemble ouvert localement $\mu$-négligeable.

#### Remarque 2 {#int-ix-s1-n6-rem-2 .statement}

Montrons que les mesures introduites dans l’Exemple 2 du n° 3 sont les mesures à support compact dans $T$. Soit $\mu$ une mesure positive sur $T$ dont le support est un ensemble compact $K$, et soit $\nu$ la mesure définie par $\mu_K$ (au sens du n° 3). Soit $f \in \mathcal{F}_+(T)$; on a

$$
\nu^*(f) = \mu_K^*(f_K) \quad (\text{n° 3, formule (3)}).
$$

L’encombrement $\mu^*$ étant concentré sur $K$, on a aussi

$$
\mu^*(f) = \mu^*(f \varphi_K) = \mu^*((f_K)^0) = \mu_K^*(f_K)
$$

d’où $\mu^* = \nu^*$, et enfin $\mu = \nu$. Inversement, si $K$ est un ensemble compact dans $T$ et $\lambda$ une mesure sur $K$, et si $\mu$ est la mesure sur $T$ définie par $\lambda$, on a $\mu^*(\mathbf{c}K) = 0$ (n° 3, formule (3)); par suite, le support de $\mu$ est contenu dans $K$, donc est compact.

### 7. Enveloppes supérieures et sommes de mesures

#### Proposition 6 {#int-ix-s1-prop-6 .statement}

Soit $(\lambda_\alpha)_{\alpha \in A}$ une famille filtrante croissante de mesures sur $T$, et soit $p = \sup_\alpha \lambda_\alpha^\bullet$. Pour que la famille $(\lambda_\alpha)$ soit majorée dans $\mathcal{M}(T)$, il faut et il suffit que l’encombrement $p$ soit localement borné. La famille $(\lambda_\alpha)$ admet alors une borne supérieure $\lambda$ dans $\mathcal{M}(T)$, et on a $\lambda^\bullet = p$. Pour tout ensemble compact $K$, la mesure $\lambda_K$ est la borne supérieure des mesures $(\lambda_\alpha)_K$ dans $\mathcal{M}(K)$.

Si la famille $(\lambda_\alpha)$ est majorée dans $\mathcal{M}(T)$, $p$ est évidemment localement borné. Inversement, supposons $p$ localement borné, et montrons qu’il satisfait aux conditions 1) et 2) de la prop. 2, b) du n° 2. Pour 2), cela résulte des égalités suivantes:

$$
p(f) = \sup_\alpha \lambda_\alpha^\bullet(f) = \sup_\alpha \sup_K \lambda_\alpha^\bullet(f \varphi_K) = \sup_K \sup_\alpha \lambda_\alpha^\bullet(f \varphi_K) = \sup_K p(f \varphi_K).
$$

D’autre part, soit $K$ un ensemble compact; l’encombrement $p_K$ est égal à l’enveloppe supérieure des encombremens $(\lambda_\alpha^\bullet)_K$, et il est borné puisque $p$ est localement borné. Les mesures $(\lambda_\alpha)_K$ admettent donc une borne supérieure $\lambda_K$ dans $\mathcal{M}(K)$, et on a $\lambda_K^\bullet = p_K$ (chap. V, 2e éd., § 1, n° 4, prop. 11). La condition 1) de la prop. 2, b) du n° 2 est donc satisfaite, et il existe donc une mesure $\lambda$ sur $T$ telle que $\lambda^\bullet = p$; il est clair que $\lambda$ est la borne supérieure des mesures $\lambda_\alpha$.

#### Définition 9 {#int-ix-s1-def-9 .statement}

Soit $(\mu_i)_{i \in I}$ une famille de mesures sur $T$. Soit $A$ l’ensemble des parties finies de $I$; pour tout $\alpha \in A$, soit $\lambda_\alpha = \sum_{i \in \alpha} \mu_i$. Si la famille $(\lambda_\alpha)$ admet dans $\mathcal{M}(T)$ une borne supérieure $\mu$, on dit que la famille $(\mu_i)$ est sommable, que $\mu$ est la somme de la famille $(\mu_i)$, et on écrit $\mu = \sum_{i \in I} \mu_i$.

Cette définition étend la déf. du chap. V, 2e éd., § 2, n° 1.

#### Proposition 7 {#int-ix-s1-prop-7 .statement}

Pour que la famille $(\mu_i)_{i \in I}$ soit sommable, il faut et il suffit que l’encombrement $p = \sum_{i \in I} \mu_i^\bullet$ soit localement borné, et l’on a dans ce cas $p = \mu^\bullet$. Pour toute partie compacte $K$ de $T$, la famille $((\mu_i)_K)_{i \in I}$ est alors sommable dans $\mathcal{M}(K)$, et l’on a $\mu_K = \sum_{i \in I} (\mu_i)_K$.

Les notations étant celles de la déf. 9, on a $\lambda_\alpha^\bullet = \sum_{i \in \alpha} \mu_i^\bullet$ pour toute partie finie $\alpha$ de $A$ (n° 2, Remarque 1). L’énoncé est alors une conséquence immédiate de la prop. 6.

La relation $\mu_K = \sum_{i \in I} (\mu_i)_K$ et la prop. 2 du chap. V, 2e éd., § 2, n° 2 nous donnent le résultat suivant:
Proposition 8. — Soit $\mu$ la somme d’une famille sommable $(\mu_i)_{i \in I}$ de mesures sur $T$. Pour qu’une application $f$ de $T$ dans un espace topologique $F$ (séparé ou non) soit $\mu$-mesurable, il faut et il suffit que $f$ soit $\mu_i$-mesurable pour tout $i \in I$.

### 8. Concassages

#### Définition 10 {#int-ix-s1-def-10 .statement}

On appelle concassage de T pour μ, ou μ-concassage, une famille localement dénombrable $(K_\alpha)_{\alpha \in A}$ de parties compactes de T deux à deux disjointes, telles que l’ensemble $N = T - \bigcup_{\alpha \in A} K_\alpha$ soit localement μ-négligeable.

#### Proposition 9 {#int-ix-s1-prop-9 .statement}

a) Il existe un concassage $(K_\alpha)_{\alpha \in A}$ de T pour μ.
b) Soit $(K_\alpha)_{\alpha \in A}$ un concassage de T pour μ. Si $\mu_\alpha$ est la mesure sur T définie par $\mu_{K_\alpha}$ (n° 3, Exemple 2), la famille $(\mu_\alpha)_{\alpha \in A}$ est sommable, sa somme est égale à μ, et on a pour toute fonction $f \in \mathcal{F}_+(T)$ la relation
$$
\mu^\bullet(f) = \sum_{\alpha \in A} \mu_\alpha^\bullet(f) = \sum_{\alpha \in A} \mu_{K_\alpha}^\bullet(f_{K_\alpha}). \tag{1}
$$
Pour qu’une application g de T dans un espace topologique G (séparé ou non) soit μ-mesurable, il faut et il suffit que $g_{K_\alpha}$ soit $\mu_{K_\alpha}$-mesurable pour tout $\alpha \in A$.

A) Existence d’un concassage:
La démonstration répète celle de la prop. 14 du chap. IV, 2e éd., § 5, n° 9, à de légères modification près. Soit $A$ l’ensemble des parties compactes K de T telles que $\operatorname{Supp}(\mu_K) = K$, et soit $H$ l’ensemble (ordonné par inclusion) des parties $L$ de $A$ formées d’ensembles deux à deux disjoints. Montrons d’abord que tout élément $L$ de $H$ est localement dénombrable. Soient $x$ un point de T, et V un voisinage ouvert de $x$ tel que $\mu^\bullet(V) < \infty$; soit $L_V$ l’ensemble des $K \in L$ qui rencontrent V. Si $(K_i)_{1 \leq i \leq n}$ est une suite finie d’éléments distincts de $L_V$, on a d’après le cor. de la prop. 4
$$
\sum_{i=1}^n \mu^\bullet(K_i \cap V) = \mu^\bullet(V \cap (\bigcup_{i=1}^n K_i)) \leq \mu^\bullet(V),
$$
puisque les $K_i$ sont deux à deux disjoints. On a donc
$$
\sum_{K \in L_V} \mu^\bullet(K \cap V) < +\infty.
$$
Or on a $\mu^\bullet(K \cap V) = \mu_K^\bullet(K \cap V) > 0$ pour tout $K \in L_V$, car $K \cap V$ est non vide, ouvert dans K, et le support de $\mu_K$ est K tout entier; $L_V$ est donc dénombrable, et $A$ est bien localement dénombrable. Il est immédiat que $H$ est inductif, et non vide (on a $\varnothing \in H$). Soit donc $S$ un élément maximal de $H$. Nous allons montrer que l’ensemble $N = T - \bigcup_{K \in S} K$ est localement négligeable. D’après la prop. 2, il suffit de vérifier que $\mu^\bullet(N \cap L) = 0$ pour tout ensemble compact L, ou encore que $\mu_L^\bullet(N \cap L) = 0$. Nous raisonnons par l’absurde. Supposons donc $\mu_L^\bullet(N \cap L) > 0$. L’ensemble des $K \in S$ qui rencontrent L étant dénombrable, $N \cap L$ est $\mu_L$-mesurable; il existe donc un ensemble compact J contenu dans $N \cap L$, tel que $\mu_L^\bullet(J) > 0$. Soit S le support de la mesure non nulle $(\mu_L)_J = \mu_J$; il est contenu dans N, la mesure $\mu_S$ n’est pas nulle, et on a $\operatorname{Supp}(\mu_S) = S$

(1) Nous verrons plus loin (§ 2, n° 2) que $\mu_\alpha$ est la mesure $\varphi_{K_\alpha} \cdot \mu$.

(chap. IV, 2e éd., § 5, n° 7, lemme 2). L’ensemble $\mathfrak{S} \cup \{ S \}$ appartient donc à $\mathcal{H}$, en contradiction avec le caractère maximal de $\mathfrak{S}$. Ceci prouve l’existence d’un concassage.

B) Démonstration de (7):

Pour tout $\alpha \in A$, on a $\mu_\alpha^\bullet(f) = \mu_{K_\alpha}^\bullet(f_{K_\alpha}) = \mu^\bullet(f_{\varphi_{K_\alpha}})$ d’après la formule (3) du n° 3 et la prop. 2, a) du n° 2; ces formules montrent que l’encombrement $\sum_{\alpha \in A} \mu_\alpha^\bullet$ est majoré par $\mu^\bullet$, donc que la famille $(\mu_\alpha)_{\alpha \in A}$ est sommable (n° 7, prop. 7).

Il suffit donc de montrer que l’on a $\mu = \sum_{\alpha \in A} \mu_\alpha$, c’est-à-dire d’établir la formule

$$
\mu_K^\bullet = \sum_{\alpha \in A} (\mu_\alpha)_K^\bullet
$$

pour toute partie compacte K de T. Or, K étant fixée, l’ensemble A’ des $\alpha \in A$ tels que $K_\alpha$ rencontre K est dénombrable. Soit $g \in \mathcal{F}_+(K)$; on a $g^0 = g^0 \varphi_N + \sum_{\alpha \in A} g^0 \varphi_{K_\alpha}$, et $g^0 \varphi_{K_\alpha} = 0$ pour $\alpha \in A - A'$; d’après la prop. 4 du n° 5, on a donc $\mu^\bullet(g^0) = \sum_{\alpha \in A} \mu^\bullet(g^0 \varphi_{K_\alpha})$, d’où

$$
\mu_K^\bullet(g) = \mu^\bullet(g^0) = \sum_{\alpha \in A} \mu^\bullet(g^0 \varphi_{K_\alpha}) = \sum_{\alpha \in A} \mu_\alpha^\bullet(g^0) = \sum_{\alpha \in A} (\mu_\alpha)_K^\bullet(g);
$$

on a ainsi établi (8).

C) Mesurabilité:

Pour qu’une fonction g définie dans T soit $\mu$-mesurable, il faut et il suffit qu’elle soit $\mu_\alpha$-mesurable pour tout $\alpha \in A$ (n° 7, prop. 8); mais cela revient à dire que $g_{K_\alpha}$ est $\mu_{K_\alpha}$-mesurable pour tout $\alpha \in A$ (n° 5, Exemple). C.Q.F.D.

Comme dans la prop. 14 du chap. IV, 2e éd., § 5, n° 9, on peut assujettir les compacts $K_\alpha$ à appartenir à un ensemble $\mu$-dense de parties compactes de T, donné à l’avance. Nous aurons seulement besoin du résultat suivant, que nous établirons directement.

#### Proposition 10 {#int-ix-s1-prop-10 .statement}

Si g est une application $\mu$-mesurable à valeurs dans un espace topologique G (séparé ou non), il existe un $\mu$-concassage $(L_\beta)_{\beta \in B}$ de T tel que les restrictions $g_{L_\beta}$ soient continues pour tout $\beta \in B$.

Considérons un concassage $(K_\alpha)_{\alpha \in A}$ de T pour $\mu$. L’application g étant mesurable, il existe pour chaque $\alpha \in A$ une partition de $K_\alpha$ en une suite $(K_{\alpha n})$ d’ensembles compacts et un ensemble localement négligeable $N_\alpha$, tels que la restriction de g à chacun des ensembles $K_{\alpha n}$ soit continue. La famille $(K_{\alpha n})_{(\alpha, n) \in A \times \mathbf{N}}$ est alors le concassage cherché. Elle est en effet localement dénombrable, et l’ensemble $N' = N \cup (\bigcup_{\alpha} N_\alpha)$ est localement négligeable, car un ensemble compact rencontre au plus une infinité dénombrable d’ensembles $N_\alpha$.

#### Scholie {#int-ix-s1-n8-sch-1 .statement}

Soit $(K_\alpha)_{\alpha \in A}$ un concassage de $T$, et soit $N = T - \bigcup_{\alpha} K_\alpha$. Nous désignerons par $T'$ l’espace localement compact obtenu en munissant $T$ de la topologie somme des topologies des sous-espaces $K_\alpha$, et d’une topologie localement compacte quelconque sur $N$ (sauf mention du contraire, nous munirons toujours $N$ de la topologie discrète). Pour chaque $\alpha \in A$, soit $i_\alpha$ l’injection canonique de $K_\alpha$ dans $T'$, et soit $\mu'_\alpha$ la mesure sur $T'$, image de $\mu_{K_\alpha}$ par $i_\alpha$. La famille $(\mu'_\alpha)$ est sommable: en effet, si $f$ est une fonction continue à support compact dans $T'$, $\operatorname{Supp}(f)$ ne rencontre $K_\alpha$ que pour un nombre fini d’indices $\alpha$. Nous poserons $\mu' = \sum_{\alpha \in A} \mu'_\alpha$. L’ensemble $N$ étant localement négligeable pour $\mu'$, puisqu’il l’est pour chaque $\mu'_\alpha$ (prop. 9), la famille $(K_\alpha)_{\alpha \in A}$ est un $\mu'$-concassage de $T'$; or la mesure induite par $\mu'$ sur $K_\alpha$ est évidemment $\mu_{K_\alpha}$ et la formule (7), appliquée à $\mu$ et à $\mu'$, montre que $\mu^* = {\mu'}^*$. De même, la dernière assertion de l’énoncé, appliquée à $\mu$ et à $\mu'$, montre que les applications mesurables sont les mêmes pour les deux mesures $\mu$ et $\mu'$.

Ces deux propriétés permettent de ramener presque toute la théorie de l’intégration par rapport à $\mu$ à la théorie faite sur les espaces localement compacts. Ces considérations seront développées au n° 10.

Voici une autre application de la notion de concassage:

#### Proposition 11 {#int-ix-s1-prop-11 .statement}

Soit $X$ une partie $\mu$-mesurable de $T$. Il existe une famille localement dénombrable $(L_\alpha)_{\alpha \in A}$ de parties compactes de $X$, deux à deux disjointes, telle que $X - \bigcup_{\alpha \in A} L_\alpha$ soit localement $\mu$-négligeable. Si, de plus, $X$ est réunion d’une suite $(X_n)$ d’ensembles mesurables tels que $\mu^*(X_n) < +\infty$, l’ensemble $B$ des $\alpha \in A$ tels que $\mu^*(L_\alpha) \neq 0$ est dénombrable, et $X - \bigcup_{\beta \in B} L_\beta$ est localement $\mu$-négligeable.

Soit $f$ la fonction caractéristique de $X$, et soit $(K_\alpha)_{\alpha \in A}$ un concassage de $T$ tel que la restriction de $f$ à chacun des $K_\alpha$ soit continue (prop. 10). L’ensemble $L_\alpha = K_\alpha \cap X$ est alors compact pour tout $\alpha \in A$, et $(L_\alpha)_{\alpha \in A}$ est la famille cherchée. Passons à la seconde assertion; les ensembles mesurables $X_n$ peuvent évidemment être supposés disjoints, et il suffit d’établir l’énoncé pour chacun d’eux. Autrement dit, quitte à changer de notation, nous pouvons supposer $\mu^*(X) < +\infty$. L’ensemble $B$ des $\alpha \in A$ tels que $\mu^*(L_\alpha) > 0$ est alors dénombrable, et il nous reste seulement à prouver que l’ensemble $N = \bigcup_{\alpha \in A - B} L_\alpha$ est localement négligeable.

Mais soit $K$ un ensemble compact; la famille $(L_\alpha)_{\alpha \in A}$ étant localement dénombrable, l’ensemble $K \cap N$ est réunion d’une sous-famille dénombrable de la famille $(K \cap L_\alpha)_{\alpha \in A - B}$, et cet ensemble est donc localement négligeable. Il en est alors de même de $N$ (n° 2, prop. 2) et la proposition est établie.

### 9. Intégrale supérieure

#### Définition 11 {#int-ix-s1-def-11 .statement}

Pour toute fonction $f \in \mathcal{F}_+(\mathrm{T})$, on appelle intégrale supérieure de $f$ (par rapport à la mesure $\mu$) le nombre positif fini ou infini

$$
\mu^*(f) = \inf_g \mu^*(g)
$$

où $g$ parcourt l’ensemble des fonctions semi-continues inférieurement qui majorent $f$.

On utilise aussi les notations $\int^* f(t)\ d\mu(t)$ et $\int^* f\ d\mu$. Lorsque $\mathrm{T}$ est localement compact, cette définition coïncide avec la définition usuelle (chap. V, 2e éd., § 1, no 1, prop. 4). On a évidemment $\mu^*(f) \leq \mu^*(f)$, avec égalité si $f$ est semi-continue inférieurement. Si $A$ est une partie de $\mathrm{T}$, on écrit $\mu^*(A)$ au lieu de $\mu^*(\varphi_A)$, et ce nombre est appelé la mesure extérieure de $A$. Les ensembles mesurables de mesure extérieure finie sont appelés ensembles intégrables, comme dans le cas des espaces localement compacts.

Une fonction $\mathbf{f}$ à valeurs dans un espace de Banach ou dans $\overline{\mathbf{R}}$ telle que $\mu^*(|\mathbf{f}|) = 0$ est dite négligeable; un ensemble $A \subset \mathrm{T}$ est dit négligeable si $\varphi_A$ est négligeable, c’est-à-dire si l’on a $\mu^*(A) = 0$. On introduit l’expression presque partout comme au chap. IV, 2e éd., § 2, no 3.

#### Proposition 12 {#int-ix-s1-prop-12 .statement}

La fonction $\mu^*$ est un encombrement sur $\mathrm{T}$.

Les propriétés $a), b), c)$ de la déf. 1 du no 1 sont évidentes. La démonstration de la propriété d) est identique à celle du th. 3 du chap. IV, 2e éd., § 1, no 3, compte tenu des prop. 4 et 5, a).

#### Corollaire {#int-ix-s1-n9-cor-1 .statement}

Une fonction $\mathbf{f}$, à valeurs dans un espace de Banach ou dans $\overline{\mathbf{R}}$, est négligeable si et seulement si $\mathbf{f}(t) = 0$ presque partout.

On se ramène immédiatement au cas d’une fonction positive. La démonstration est alors identique à celle du th. 1 du chap. IV, 2e éd., § 2, no 3.

#### Proposition 13 {#int-ix-s1-prop-13 .statement}

Pour toute partie $A$ de $\mathrm{T}$, $\mu^*(A)$ est la borne inférieure des mesures extérieures des ensembles ouverts contenant $A$.

La démonstration est identique à celle de la prop. 19 du chap. IV, 2e éd., § 1, no 4.

#### Définition 12 {#int-ix-s1-def-12 .statement}

Soit $\mathbf{f}$ une fonction définie dans $\mathrm{T}$, à valeurs dans un espace de Banach ou dans $\overline{\mathbf{R}}$. On dit que $\mathbf{f}$ est modérée pour la mesure $\mu$, ou $\mu$-modérée, si $\mathbf{f}$ est nulle dans le complémentaire d’une réunion dénombrable d’ouverts intégrables. On dit qu’une partie $A$ de $\mathrm{T}$ est modérée si la fonction $\varphi_A$ est modérée. On dit que la mesure $\mu$ est modérée si la fonction $1$ est $\mu$-modérée.

Par exemple, l’encombrement $\mu^*$ étant localement borné, toute partie compacte $K$ de $\mathrm{T}$ est contenue dans un ensemble ouvert $V$ tel que $\mu^*(V) < +\infty$; une fonction nulle hors d’un ensemble compact est donc modérée. Une fonction négligeable est modérée. Les remarques qui suivent la déf. 2 du chap. V, 2e éd., § 1, no 2 s’étendent aussitôt à la présente situation. En particulier, la somme d'une suite de fonctions positives modérées est modérée.

#### Remarque 1 {#int-ix-s1-n9-rem-1 .statement}

Sur un espace de Lindelöf T (Top. Gén., chap. IX, 3e édit., Appendice I, déf. 1), et en particulier sur un espace souslinien, toute mesure est modérée. Les ouverts de mesure finie forment en effet un recouvrement de T, dont on peut extraire un recouvrement dénombrable de T.

#### Remarque 2 {#int-ix-s1-n9-rem-2 .statement}

On prendra garde que l’existence d’une suite d’ensembles boréliens de mesure finie pour $\mu$, de réunion T, n’entraîne pas nécessairement l’existence d’une suite d’ensembles ouverts de mesure finie, de réunion T (autrement dit, n’entraîne pas que $\mu$ est modérée). Voir l’exerc. 8.

#### Proposition 14 {#int-ix-s1-prop-14 .statement}

Soit $f \in \mathcal{F}_+(T)$. Si $f$ est $\mu$-modérée, on a $\mu^*(f) = \mu^*(f)$; si $f$ n’est pas $\mu$-modérée, on a $\mu^*(f) = +\infty$.

Si $\mu^*(f) < +\infty$, il existe une fonction semi-continue inférieurement $g \geq f$ telle que $\mu^*(g) < +\infty$. Pour tout $n \in \mathbf{N}$, soit $G_n$ l’ensemble des $t \in T$ tels que $g(t) > 1/n$; l’ensemble $G_n$ est ouvert, on a $\mu^*(G_n) \leq n \mu^*(g) < +\infty$, et $f$ est nulle hors de la réunion des $G_n$: la fonction $f$ est donc modérée.

Montrons ensuite que $\mu^*$ et $\mu^*$ ont même valeur pour les fonctions modérées. Comme $\mu^*$ et $\mu^*$ sont des encombrements, il suffit d’établir la relation $\mu^*(f) = \mu^*(f)$ lorsque $f$ est une fonction positive, majorée par une constante M, et nulle hors d’un ensemble ouvert G de mesure finie, ce que nous allons faire à présent.

La mesure $\mu$ est la borne supérieure, dans $\mathcal{M}(T)$, d’une famille filtrante croissante $(\mu_i)_{i \in I}$ de mesures à support compact: cela résulte aussitôt de la prop. 9 du n° 8. Soit $g$ une fonction semi-continue inférieurement dans T, comprise entre $f$ et la fonction semi-continue inférieurement $M_{\varphi_G}$. Posons $v_i = \mu - \mu_i$; on a $\mu^* = \mu_i^* + v_i^*$ (n° 2, Remarque 1) et par conséquent

$$
\mu^*(g) - \mu^*(f) = (\mu_i^*(g) - \mu_i^*(f)) + (v_i^*(g) - v_i^*(f))
$$
$$
\leq (\mu_i^*(g) - \mu_i^*(f)) + v_i^*(M_{\varphi_G}).
$$

On a $v_i^*(M_{\varphi_G}) = \mu^*(M_{\varphi_G}) - \mu_i^*(M_{\varphi_G})$ et $\mu^*(M_{\varphi_G}) = \sup \mu_i^*(M_{\varphi_G})$ (n° 7, prop. 6); le nombre $v_i^*(M_{\varphi_G})$ peut donc être rendu arbitrairement petit par un choix convenable de $i$. Tout revient donc à montrer qu’on peut trouver, quels que soient le nombre $c > 0$ et l’indice $i \in I$, une fonction semi-continue inférieurement $g$ comprise entre $f$ et $M_{\varphi_G}$, telle que $\mu_i^*(g) - \mu_i^*(f) \leq c$. Or soit L le support compact de la mesure $\mu_i$, et soit $\lambda$ la mesure $(\mu_i)_L$; puisque $\mu_i$ est concentrée sur L, on a $\mu_i^*(h) = \mu_i^*(h_{\varphi_L}) = \lambda^*(h_L)$ pour toute fonction $h \in \mathcal{F}_+(T)$ (n° 1, lemme 1 et n° 2, prop. 2); on a donc

$$
\mu_i^*(g) - \mu_i^*(f) = \lambda^*(g_L) - \lambda^*(f_L).
$$

Mais L est compact; on a donc $\lambda^* = \lambda^*$, et il existe par conséquent une fonction semi-continue inférieurement $h$ définie dans L, majorant $f_L$ et telle que $\lambda^*(h) \leq \lambda^*(f_L) + c$. L’ensemble L étant fermé dans T, la fonction k égale à $h$ dans L, et à $+\infty$ dans $T - L$, est semi-continue inférieurement dans T et majore f, et on a $\lambda^*(k_L) = \lambda^*(h) \leq \lambda^*(f_L) + c$. Il ne reste plus qu’à poser $g = \inf (k, M_{\varphi_G})$: $g$ est semi-continue inférieurement, majore $f$, et on a

$$
\mu_i^*(g) \leq \mu_i^*(k) = \lambda^*(k_L) \leq \lambda^*(f_L) + c = \mu_i^*(f) + c.
$$

#### Corollaire 1 {#int-ix-s1-prop-14-cor-1 .statement}

Pour qu’une fonction soit négligeable, il faut et il suffit qu’elle soit localement négligeable et modérée.

#### Corollaire 2 {#int-ix-s1-prop-14-cor-2 .statement}

Pour qu’une fonction $f$ soit localement négligeable, il faut et il suffit que tout $x \in T$ possède un voisinage $V$ tel que $f_{\varphi_V}$ soit négligeable.

En effet, si cette propriété est satisfaite, $f_{\varphi_K}$ est négligeable pour tout ensemble compact $K$, et $f$ est donc localement négligeable (n° 2, prop. 2). Inversement, supposons que $f$ soit localement négligeable, et soit $x$ un point de $T$; il admet un voisinage ouvert $V$ de mesure finie. La fonction $f_{\varphi_V}$ est alors localement négligeable et modérée, donc négligeable.

#### Corollaire 3 {#int-ix-s1-prop-14-cor-3 .statement}

Soit $f$ une fonction modérée définie dans $T$. Il existe une suite $(K_n)$ de parties compactes deux à deux disjointes, et un ensemble négligeable $H$, tels que $f = f_{\varphi_H} + \sum_n f_{\varphi_{K_n}}$.

En effet, soit $G$ un ensemble, réunion dénombrable d’ouverts intégrables tels que $f$ soit nulle hors de $G$; alors $G$ est réunion d’une suite $(K_n)$ d’ensembles compacts disjoints deux à deux, et d’un ensemble localement négligeable $H$ (n° 8, prop. 11); mais $H$ est modéré, donc négligeable.

#### Corollaire 4 {#int-ix-s1-prop-14-cor-4 .statement}

Soient $\mu$ et $\nu$ deux mesures sur $T$ telles que $\mu^* = \nu^*$, on a alors $\mu = \nu$.

En effet, l’égalité $\mu^* = \nu^*$ entraîne $\mu^*(f) = \nu^*(f)$ pour toute fonction positive $f$, modérée pour $\mu$ et $\nu$, donc pour toute fonction positive à support compact. On en déduit $\mu^* = \nu^*$ (n° 2, prop. 2), puis $\mu = \nu$ (n° 2, cor. de la prop. 2).

#### Corollaire 5 {#int-ix-s1-prop-14-cor-5 .statement}

Si $\mu$ est une mesure modérée sur $T$, il existe une suite $(\mu_n)_{n \in \mathbf{N}}$ de mesures à support compact telle que $\mu = \sum_{n \in \mathbf{N}} \mu_n$.

Par hypothèse, la fonction constante 1 est $\mu$-modérée. Appliquons le cor. 3 au cas $f = 1$; il existe donc une suite $(K_n)_{n \in \mathbf{N}}$ de parties compactes de $T$ deux à deux disjointes telle que $1 = \sum_{n \in \mathbf{N}} \varphi_{K_n}$ $\mu$-presque partout. Soit $\mu_n$ la mesure définie par la mesure $\mu_{K_n}$ sur $K_n$ (n° 3, Exemple 2). On sait (n° 6, Remarque 2) que $\mu_n$ est à support compact, et que l’on a $\mu_n^*(f) = \mu^*(f_{\varphi_{K_n}})$ pour $f \in \mathcal{F}_+(T)$. Or $f$ est égale à $\sum_{n \in \mathbf{N}} f_{\varphi_{K_n}}$ $\mu$-presque partout, d’où $\mu^*(f) = \sum_{n \in \mathbf{N}} \mu^*(f_{\varphi_{K_n}}) = \sum_{n \in \mathbf{N}} \mu_n^*(f)$. On en déduit $\mu = \sum_{n \in \mathbf{N}} \mu_n$ (n° 7, prop. 7).

### 10. Théorie de l’intégration

#### Définition 13 {#int-ix-s1-def-13 .statement}

Soit $p \in (1, +\infty[ ;$ on désigne par $\overline{\mathcal{L}}^p(T, \mu)$ (resp. $\overline{\mathcal{L}}_F^p(T, \mu)$ si F est un espace de Banach) l’ensemble des applications $f$ de T dans $\overline{\mathbf{R}}$ (resp. dans F), $\mu$-mesurables et telles que $\mu^*(|f|^p) < +\infty$. On désigne par $\mathcal{L}^p(T, \mu)$ (resp. $\mathcal{L}_F^p(T, \mu)$) l’ensemble des éléments $\mu$-modérés de $\overline{\mathcal{L}}^p(T, \mu)$ (resp. $\overline{\mathcal{L}}_F^p(T, \mu)$).

On posera $\overline{N}_p(f) = (\mu^*(|f|^p))^{1/p}$, $N_p(f) = (\mu^*(|f|^p))^{1/p}$. On désigne par $\overline{N}_\infty(f)$ la borne inférieure des nombres $k \geq 0$ tels que $|f| \leq k$ localement $\mu$-presque partout; si $\overline{N}_\infty(f) < +\infty$, on dit que $f$ est essentiellement bornée. L’ensemble des applications mesurables et essentiellement bornées de T dans $\overline{\mathbf{R}}$ (resp. dans F) est désigné par $\overline{\mathcal{L}}^\infty(T, \mu)$ (resp $\overline{\mathcal{L}}_F^\infty(T, \mu)$). Les éléments de $\overline{\mathcal{L}}_F^1(T, \mu)$ (resp. $\mathcal{L}_F^1(T, \mu)$) sont appelés fonctions essentiellement intégrables (resp. fonctions intégrables) à valeurs dans F.

Si $\mu$ est une mesure complexe, on posera
$$
\overline{\mathcal{L}}_F^p(T, \mu) = \overline{\mathcal{L}}_F^p(T, |\mu|) \quad \text{et} \quad \mathcal{L}_F^p(T, \mu) = \mathcal{L}_F^p(T, |\mu|).
$$
Les notations ci-dessus sont fréquemment abrégées en $\overline{\mathcal{L}}_F^p(\mu)$, $\overline{\mathcal{L}}_F^p$ ou $\mathcal{L}^p(\mu)$, $\mathcal{L}^p$, si cela ne prête pas à confusion.

Nous avons vu au n° 8 (Scholie) que l’on peut construire un espace localement compact $T'$, ayant même ensemble sous-jacent que T et une topologie plus fine que celle de T, et munir $T'$ d’une mesure $\mu'$, telle que les fonctions $\mu$-mesurables et les fonctions $\mu'$-mesurables soient les mêmes et que les intégrales supérieures essentielles des fonctions positives pour $\mu$ et $\mu'$ soient égales. Il en résulte que les ensembles $\overline{\mathcal{L}}_F^p(\mu)$ et $\overline{\mathcal{L}}_F^p(\mu')$ sont identiques pour $1 \leq p \leq +\infty$. Cela entraîne aussi sans nouvelle démonstration que $\overline{\mathcal{L}}_F^p$ est un espace vectoriel, et que la fonction $\overline{N}_p$ est une semi-norme sur $\overline{\mathcal{L}}_F^p(\mu)$, pour laquelle cet espace est complet.

Soit $f$ un élément de $\overline{\mathcal{L}}_F^p (1 \leq p < \infty)$; comme on a $\mu^*(|f|^p) = {\mu'}^*(|f|^p) < +\infty$, la prop. 7 du chap. V, 2e éd., § 1, n° 2 entraîne que $f$ est nulle hors de la réunion d’une suite de parties compactes de $T'$ et d’un ensemble localement $\mu'$-négligeable; ce dernier ensemble étant localement $\mu$-négligeable, et tout ensemble compact de $T'$ étant compact dans T, on en déduit que $f$ est égale localement $\mu$-presque partout à une fonction $\mu$-modérée. Désignons par $\overline{\mathcal{N}}_F$ (resp. $\mathcal{N}_F$) l’espace des fonctions localement $\mu$-négligeables (resp. $\mu$-négligeables); nous avons donc $\overline{\mathcal{L}}_F^p = \mathcal{L}_F^p + \overline{\mathcal{N}}_F$, et $\mathcal{N}_F = \mathcal{L}_F^p \cap \overline{\mathcal{N}}_F$ (n° 9, cor. 1 de la prop. 14). L’espace $\overline{\mathcal{L}}_F^p / \overline{\mathcal{N}}_F$ s’identifie donc canoniquement à $\mathcal{L}_F^p / \mathcal{N}_F$, et on vérifie immédiatement que cette identification préserve la norme; cet espace quotient est noté $L_F^p(\mu)$. On peut l’interpréter comme l’espace normé associé à chacun des espaces semi-normés $\overline{\mathcal{L}}_F^p(\mu)$ ou $\mathcal{L}_F^p(\mu)$; $\overline{\mathcal{L}}_F^p$ étant complet, il en est de même de $L_F^p$ et de $\mathcal{L}_F^p$.

1. On notera que l’espace $\mathcal{L}_F^p(\mu)$ est contenu dans $\mathcal{L}_F^p(\mu')$, mais qu’il en est distinct en général.

L’ensemble des fonctions $\mathbf{f}$ à valeurs dans $F$, continues à support compact sur $T'$, est dense dans $\overline{\mathcal{L}}_F^p(\mu') = \overline{\mathcal{L}}_F^p(\mu)$ (chap. IV, 2e édit., § 3, n° 4, déf. 2). Reprenons les notations du Scholie du n° 8. Une partie compacte de $T'$ ne rencontrant qu’un nombre fini d’ensembles compacts $K_\alpha$, toute fonction $\mathbf{f}$ continue à support compact sur $T'$ s’écrit comme une somme

$$
\mathbf{f} = \sum_{\alpha \in A} \mathbf{f}_\alpha + \mathbf{g}
$$

où $\mathbf{f}_\alpha$ est, pour tout $\alpha$, le prolongement par 0 d’une fonction continue sur $K_\alpha$, où $\mathbf{f}_\alpha = 0$ sauf pour un nombre fini d’indices, et où $\mathbf{g}$ est localement $\mu$-négligeable. Nous avons donc le résultat suivant:

#### Proposition 15 {#int-ix-s1-prop-15 .statement}

*L’ensemble des fonctions $\mathbf{f}$ à valeurs dans $F$, telles que $\mathrm{Supp}(\mathbf{f})$ soit compact, et que la restriction de $\mathbf{f}$ à $\mathrm{Supp}(\mathbf{f})$ soit continue, est dense dans $\overline{\mathcal{L}}_F^p(\mu)$ et dans $\mathcal{L}_F^p(\mu)$, pour $1 \leq p < +\infty$.*

On notera que ces fonctions *ne sont pas* des fonctions continues *dans* $T$ à support compact.

Passons à la définition de l’intégrale.

#### Proposition 16 {#int-ix-s1-prop-16 .statement}

*Il existe une application linéaire continue et une seule $\mathbf{f} \mapsto \int \mathbf{f} \, d\mu$, de l’espace $\overline{\mathcal{L}}_F^1(\mu)$ dans $F$, qui possède la propriété suivante:
Si $\mathbf{f}$ est de la forme $t \mapsto g(t)\mathbf{a}$, avec $\mathbf{a} \in F$, et où $g$ est une fonction positive, finie, $\mu$-mesurable et telle que $\mu^*(g) < +\infty$, on a $\int \mathbf{f} \, d\mu = \mu^*(g) \cdot \mathbf{a}$.

En effet, les espaces semi-normés $\overline{\mathcal{L}}_F^1(\mu)$ et $\overline{\mathcal{L}}_F^1(\mu')$ sont identiques. Comme $\mu^* = {\mu'}^*$, l’application $\mathbf{f} \mapsto \int \mathbf{f} \, d\mu'$ satisfait à l’énoncé. D’autre part, l’ensemble des fonctions de la forme $\mathbf{f} = g \cdot \mathbf{a}$ considérées dans l’énoncé est *total* dans $\overline{\mathcal{L}}_F^1(\mu')$ (chap. IV, 2e éd., § 3, n° 5, prop. 10), d’où l’unicité.

*On dit que* $\int \mathbf{f} \, d\mu$ *est l’intégrale de* $\mathbf{f}$ *par rapport à* $\mu$ *et on note aussi ce vecteur* $\mu(\mathbf{f})$ *ou* $\int \mathbf{f}(t) d\mu(t)$.

Comme $\int \mathbf{f} \, d\mu = \int \mathbf{f} \, d\mu'$ pour toute fonction essentiellement intégrable $\mathbf{f}$ à valeurs dans $F$, toute la théorie de l’intégrale essentielle s’étend aux mesures sur les espaces séparés sans nouvelle démonstration; on en déduit les résultats relatifs à l’intégrale ordinaire en se restreignant aux fonctions modérées. Citons en particulier les résultats suivants:

— le th. 3 du chap. IV, 2e éd., § 3, n° 4, son extension à $\overline{\mathcal{L}}_F^p$, et ses deux corollaires.
— Le th. 4 du chap. IV, 2e éd., § 3, n° 5 (composition avec une application linéaire continue) et ses corollaires; les prop. 9, 11 et 12 de ce même numéro.

— Tous les résultats du chap. IV, 2e éd., § 3, n° 6, relatifs à la structure d’espace vectoriel ordonné de $L^p$.
— Tous les résultats du chap. IV, 2e éd., § 3, n° 7 et en particulier le théorème de Lebesgue.
— Tous les résultats du chap. IV, 2e éd., § 3, n° 8, sur les relations entre les espaces $L_F^p$.
— Le théorème 2 du chap. IV, 2e éd., § 4, n° 3 (énoncé du théorème de Lebesgue propre à $L_F^1$).
— L’inégalité de Hölder (chap. IV, 2e éd., § 6, n° 4, th. 2) et ses corollaires.
— Les relations entre les espaces $L_F^p$ établies au chap. IV, 2e éd., § 6, n° 5.
— Les résultats sur la dualité des espaces $L^p$ établis au chap. V, 2e éd., § 5, n° 8.
— Le théorème de Dunford-Pettis (chap. VI, § 2, n° 5, th. 1), ses corollaires 1 et 2, et la prop. 10 du chap. VI, § 2, n° 6 (dual de $L_F^1$).

## EXERCICES {#int-ix-s1-exercises}

See the [exercises for § 1](exercises/s1/).
