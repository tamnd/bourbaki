---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: GROUPES DE LIE
section: 6
section_title: Groupes de Lie réels ou complexes
lang: fr
source: lie-ii-iii-fr
pdf_pages: 0190-0212, 0264-0270
extraction: ocr
subsections:
    - "no": 1
      title: Passage des morphismes d’algèbres de Lie aux morphismes de groupes de Lie
      page: 0
      pdf_page: 190
    - "no": 2
      title: Sous-groupes intégraux
      page: 0
      pdf_page: 191
    - "no": 3
      title: Passage des algèbres de Lie aux groupes de Lie
      page: 0
      pdf_page: 196
    - "no": 4
      title: Application exponentielle
      page: 0
      pdf_page: 197
    - "no": 5
      title: Application aux représentations linéaires
      page: 0
      pdf_page: 201
    - "no": 6
      title: Sous-groupes intégraux distingués
      page: 0
      pdf_page: 202
    - "no": 7
      title: Primitives des formes différentielles à valeurs dans une algèbre de Lie
      page: 0
      pdf_page: 204
    - "no": 8
      title: Passage des lois d’opérations infinitésimales aux lois d’opérations
      page: 0
      pdf_page: 204
    - "no": 9
      title: Application exponentielle dans le groupe linéaire
      page: 0
      pdf_page: 206
    - "no": 10
      title: Complexification d’un groupe de Lie réel de dimension finie
      page: 0
      pdf_page: 208
statements: 76
exercises: 30
content_sha256: fe38d0e07965528001fa474c2453af125868ae27bc80af5a2f745d9e63d29fe6
---

## § 6. Groupes de Lie réels ou complexes

Dans ce paragraphe, on suppose que K est égal à $\mathbf{R}$ ou à $\mathbf{C}$.

### 1. Passage des morphismes d’algèbres de Lie aux morphismes de groupes de Lie

#### Lemme 1 {#lie-iii-s6-lem-1 .statement}

Soient $G$ un groupe topologique simplement connexe,$^1$ $W$ un voisinage ouvert connexe symétrique de $e$, $H$ un groupe, $f$ une application de $W^3$ dans $H$ telle que
$$
f(xyz) = f(x)f(y)f(z)
$$
pour $x, y, z$ dans $W$. Il existe un morphisme $f'$ de $G$ dans $H$ tel que $f'|W = f|W$.

Pour $(g, h) \in G \times H$ et $U$ voisinage ouvert de $e$ dans $W$, soit $A(g, h, U)$ l’ensemble des $(gu, hf(u)) \in G \times H$ pour $u \in U$. On a $(g, h) \in A(g, h, U)$, et $A(g, h, U_1) \cap A(g, h, U_2) = A(g, h, U_1 \cap U_2)$. Soit $(s, t) \in A(g, h, U)$; on a $s = gu$ et $t = hf(u)$ pour un $u \in U$; il existe un voisinage ouvert $U'$ de $e$ dans $W$ tel que $uU' \subset U$; alors, pour $u' \in U'$, on a
$$
(su', tf(u')) = (guu', hf(uu')) \in A(g, h, U)
$$
donc $A(s, t, U') \subset A(g, h, U)$. Il résulte de là que les $A(g, h, U)$ forment la base d’une topologie sur $G \times H$. Nous noterons $Y$ l’ensemble $G \times H$ muni de cette topologie, et désignerons par $p$ la projection canonique de $Y$ sur $G$, qui est ouverte. La restriction de $p$ à $A(g, h, U)$ est un homéomorphisme de $A(g, h, U)$ sur $gU$. Donc $(Y, p)$ est un revêtement de $G$. Soit $Y_0$ le sous-groupe de $Y$ engendré par $A(e, e, W)$, et soit $\mathcal{B}$ l’ensemble des $A(e, e, U)$. Il est clair que $\mathcal{B}$ vérifie les conditions $(GV'_I)$ et $(GV'_{II})$ de TG, III, § 1, n° 2. L’ensemble $Y'_0$ des $y \in Y_0$ tels que les applications $z \mapsto yzy^{-1}$ et $z \mapsto y^{-1}zy$ de $Y_0$ dans $Y_0$ soient continues en $(e, e)$ est un sous-groupe de $Y_0$. Soit $w \in W$. L’application $w' \mapsto ww'w^{-1}$ de $W$ dans $G$ est continue, donc l’application $(w', f(w')) \mapsto (ww'w^{-1}, f(ww'w^{-1}))$ de $A(e, e, W)$ dans $Y$ est continue en $(e, e)$. Or $f(ww'w^{-1}) = f(w)f(w')f(w^{-1})$, et par suite
$$
(ww'w^{-1}, f(ww'w^{-1})) = (w, f(w))(w', f(w'))(w, f(w))^{-1}.
$$
Comme $w^{-1} \in W$, on voit que $(w, f(w)) \in Y'_0$. Ainsi, $A(e, e, W) \subset Y'_0$, de sorte que $Y'_0 = Y_0$. Le groupe $Y_0$, muni de la base de filtre $\mathcal{B}$, vérifie donc la condition $(GV'_{III})$ de TG, III, § 1, n° 2. Comme $(g, h) . A(e, e, U) = A(g, h, U)$, $Y_0$ est un groupe topologique, connexe puisque $A(e, e, W)$ est connexe. Alors $p(Y_0)$ est un sous-groupe ouvert de $G$, d’où $p(Y_0) = G$ puisque $G$ est connexe. Le noyau de $p|Y_0$ est discret. Comme $G$ est simplement connexe, $p|Y_0$ est un homéomorphisme de $Y_0$ sur $G$. Par suite, $Y_0$ est le graphe d’un morphisme $f'$ de $G$ dans $H$. Pour $g \in W$, on a $(g, f(g)) \in A(e, e, W) \subset Y_0$, d’où $f(g) = f'(g)$.

$^1$ Cf. le chap. XI de TG (à paraître). Il est prouvé dans ce chapitre que si $G_1, G_2$ sont des groupes topologiques connexes, si $\varphi$ est un homomorphisme continu ouvert de $G_1$ sur $G_2$ à noyau discret, et si $G_2$ est simplement connexe, alors $\varphi$ est un homéomorphisme. Rappelons d’autre part qu’un espace simplement connexe est connexe.

#### Théorème 1 {#lie-iii-s6-thm-1 .statement}

Soient G et H des groupes de Lie, h un morphisme continu de L(G) dans L(H). On suppose G simplement connexe. Alors il existe un morphisme φ de groupes de Lie de G dans H, et un seul, tel que h = L(φ).

L’existence de φ résulte du lemme 1, et du § 4, n° 1, th. 1 (i). L’unicité de φ résulte du § 4, n° 1, th. 1(ii) et du fait que G est connexe.

#### Corollaire {#lie-iii-s6-n1-cor-1 .statement}

Soit G un groupe de Lie simplement connexe de dimension finie. Il existe une représentation linéaire analytique de dimension finie de G dont le noyau est discret.

Il existe (chap. I, § 7, th. 2) un espace vectoriel E de dimension finie, et un morphisme injectif h de L(G) dans l’algèbre de Lie End(E). D’après le th. 1, il existe un morphisme φ de G dans GL(E) tel que L(φ) = h. Donc φ est une immersion, et par suite son noyau est discret.

#### Remarque 1 {#lie-iii-s6-n1-rem-1 .statement}

Il existe des groupes de Lie simplement connexes de dimension finie qui ne possèdent aucune représentation linéaire analytique injective de dimension finie (exerc. 2).

#### Remarque 2 {#lie-iii-s6-n1-rem-2 .statement}

Il existe des groupes de Lie connexes G de dimension finie tels que toute représentation linéaire analytique de dimension finie de G ait un noyau non discret (exerc. 3 et 4).

### 2. Sous-groupes intégraux

#### Définition 1 {#lie-iii-s6-def-1 .statement}

Soit G un groupe de Lie. On appelle sous-groupe intégral de G un sous-groupe H muni d’une structure de groupe de Lie connexe telle que l’injection canonique de H dans G soit une immersion.

On appelle sous-groupe à un paramètre de G un sous-groupe intégral de dimension 1.

Soient H un sous-groupe intégral de G, i l’injection canonique de H dans G. Alors L(i) définit un isomorphisme de L(H) sur une sous-algèbre de Lie de L(G) admettant un supplémentaire topologique. On identifie L(H) à son image par L(i).

#### Exemple 1 {#lie-iii-s6-n2-exa-1 .statement}

Un sous-groupe de Lie connexe de G est un sous-groupe intégral de G.

#### Exemple 2 {#lie-iii-s6-n2-exa-2 .statement}

Supposons G de dimension finie. Soit H un sous-groupe de G; munissons-le de la structure induite par la structure de groupe de Lie de G (§ 4, n° 5, déf. 3). Alors sa composante neutre H_0 est un sous-groupe intégral de G, et la sous-algèbre tangente en e à H est L(H_0) (§ 4, n° 5, prop. 9 (ii)).

#### Exemple 3 {#lie-iii-s6-n2-exa-3 .statement}

Soient G un groupe de Lie complexe, H un sous-groupe intégral de G, G_1 (resp. H_1) le groupe de Lie réel sous-jacent à G (resp. H). Alors H_1 est un sous-groupe intégral de G_1, et L(H_1) est l’algèbre de Lie réelle sous-jacente à L(H).

#### Théorème 2 {#lie-iii-s6-thm-2 .statement}

Soit G un groupe de Lie.

(i) L’application $H \mapsto L(H)$ est un bijection de l’ensemble des sous-groupes intégraux de G sur l’ensemble des sous-algèbres de Lie de $L(G)$ admettant un supplémentaire topologique.

(ii) Soit H un sous-groupe intégral de G. Tout sous-groupuscule de Lie connexe de G d’algèbre de Lie $L(H)$ est une sous-variété ouverte de H qui engendre H.

a) Soit $\mathfrak{h}$ une sous-algèbre de Lie de $L(G)$ admettant un supplémentaire topologique. Soit $H_1$ un sous-groupuscule de Lie de G tel que $L(H_1) = \mathfrak{h}$ (\S 4, th. 3). On peut choisir $H_1$ de telle sorte qu’il soit connexe. Soit H le sous-groupe de G engendré par $H_1$. Il existe (\S 1, cor. de la prop. 22) une structure de groupe de Lie sur H telle que $H_1$ soit une sous-variété ouverte de H et que l’injection canonique de H dans G soit une immersion. Comme $H_1$ est connexe, H est connexe, donc est un sous-groupe intégral de G. On a $L(H) = L(H_1) = \mathfrak{h}$. Cela prouve que l’application considérée en (i) est surjective.

b) Soient H un sous-groupe intégral de G, et $N_1$ un sous-groupuscule de Lie connexe de G d’algèbre de Lie $L(H)$. Comme l’injection canonique de H dans G est une immersion, il existe un sous-groupuscule ouvert $H_1$ de H qui est en même temps sous-variété de G, donc un sous-groupuscule de Lie de G d’algèbre de Lie $L(H)$. D’autre part, soit N le sous-groupe de G engendré par $N_1$; d’après la partie a) de la démonstration, il est muni d’une structure de sous-groupe intégral de G tel que $N_1$ soit une sous-variété ouverte de N. D’après le \S 4, th. 3, $H_1 \cap N_1$ est ouvert dans $H_1$ et $N_1$. Donc le sous-groupe de G engendré par $H_1 \cap N_1$ est égal d’une part à H, d’autre part à N. Par suite les groupes de Lie H et N sont égaux. Cela prouve (ii), et prouve aussi que l’application considérée en (i) est injective.

#### Remarque 1 {#lie-iii-s6-n2-rem-1 .statement}

Soit H un sous-groupe intégral de G. Soit Y le feuilletage gauche de G associée à $L(H)$. Si $g \in G$, munissons $gH$ de la structure de variété déduite de celle de H par $\gamma(g)$. D’après VAR, R, 9.3.2, l’injection canonique de $gH$ dans Y est un morphisme. Ce morphisme est étale. Donc les feuilles connexes maximales de Y sont les classes à gauche suivant H.

#### Proposition 1 {#lie-iii-s6-prop-1 .statement}

Soient G et M des groupes de Lie, H un sous-groupe intégral de G, $\varphi$ un morphisme de M dans G tel que $L(\varphi)(L(M)) \subset L(H)$. On suppose M connexe. Alors $\varphi(M) \subset H$, et $\varphi$, considéré comme application de M dans H, est un morphisme de groupes de Lie.

En effet, avec les notations de la Remarque 1, $\varphi$ est un morphisme de M dans Y (VAR, R, 9.3.2), donc $\varphi(M) \subset H$ puisque M est connexe.

#### Corollaire 1 {#lie-iii-s6-prop-1-cor-1 .statement}

Soient G et H des groupes de Lie, $\varphi$ un morphisme de groupes de Lie de G dans H, N le noyau de $\varphi$, et $h = L(\varphi)$. Supposons G connexe et H de dimension finie.

(i) N est un sous-groupe de Lie de G, et $L(N) = \mathrm{Ker}\ h$.

(ii) Soit $H'$ le sous-groupe intégral de $H$ d’algèbre de Lie $\mathrm{Im}\ h$. Alors $\varphi(G) = H'$.
(iii) L’application de $G/N$ dans $H'$ déduite de $\varphi$ par passage au quotient est un isomorphisme de groupes de Lie.
(i) a déjà été démontré ($\S 3$, no 8, prop. 28).
Soit $\psi$ le morphisme de groupes de Lie de $G/N$ dans $H$ déduit de $\varphi$ par passage au quotient; c’est une immersion ($\S 3$, no 8, prop. 28). D’après la prop. 1, $\psi$ est un morphisme de groupes de Lie de $G/N$ dans $H'$. Ce morphisme est étale, donc $\psi(G/N) = H'$ puisque $H'$ est connexe; cela prouve (ii). Alors $\psi : G/N \to H'$ est bijectif, et est un isomorphisme de groupes de Lie, ce qui prouve (iii).

#### Corollaire 2 {#lie-iii-s6-prop-1-cor-2 .statement}

Soient $G$ un groupe de Lie, $H_1$ et $H_2$ des sous-groupes intégraux de $G$. Si $L(H_2) \subset L(H_1)$, alors $H_2$ est un sous-groupe intégral de $H_1$.
Soient $i_1 : H_1 \to G$, $i_2 : H_2 \to G$ les injections canoniques. Alors
$$
L(i_2)(L(H_2)) = L(H_2) \subset L(H_1).
$$
D’après la prop. 1, $i_2$ est une application analytique de $H_2$ dans $H_1$, et même une immersion de $H_2$ dans $H_1$ puisque $L(i_2)$ est un isomorphisme de $L(H_2)$ sur une sous-algèbre de $L(H_1)$ admettant un supplémentaire topologique.

#### Corollaire 3 {#lie-iii-s6-prop-1-cor-3 .statement}

Soient $G$ un groupe de Lie de dimension finie, $(H_i)_{i \in I}$ une famille de sous-groupes de Lie de $G$. Alors $H = \bigcap_{i \in I} H_i$ est un sous-groupe de Lie de $G$, et
$$
L(H) = \bigcap_{i \in I} L(H_i).
$$
Il existe une partie finie $J$ de $I$ telle que $\bigcap_{i \in J} L(H_i)$ soit égal à l’intersection $M$ de tous les $L(H_i)$. On sait que $H^* = \bigcap_{i \in J} H_i$ est un sous-groupe de Lie tel que $L(H^*) = M$ ($\S 3$, no 8, cor. 2 de la prop. 29). Soit $H_0$ la composante neutre de $H^*$. C’est un sous-groupe de Lie de $G$, et $L(H_0) = M$. D’après le cor. 2, on a $H_0 \subset H_i$ pour tout $i$, donc $H_0 \subset H \subset H^*$, d’où le corollaire.

#### Corollaire 4 {#lie-iii-s6-prop-1-cor-4 .statement}

Soit $G$ un groupe de Lie connexe de dimension finie. Les conditions suivantes sont équivalentes:
(i) $G$ est unimodulaire (INT, VII, $\S 1$, no 3, déf. 3);
(ii) $\det \operatorname{Ad} g = 1$ pour tout $g \in G$;
(iii) $\operatorname{Tr} \operatorname{ad} a = 0$ pour tout $a \in L(G)$.
L’application $g \mapsto \det \operatorname{Ad} g$ est un morphisme $\varphi$ de $G$ dans $K^*$. D’après le $\S 3$, prop. 35 (no 10) et 44 (no 12), on a $L(\varphi)a = \operatorname{Tr} \operatorname{ad} a$ pour tout $a \in L(G)$. Il est clair que $\operatorname{Im} L(\varphi) = \{0\}$ ou $K$. Dans le premier (resp. deuxième) cas, on a

#### Proposition 2 {#lie-iii-s6-prop-2 .statement}

*Soient G un groupe de Lie de dimension finie, H un sous-groupe intégral de G.* Les conditions suivantes sont équivalentes:
(i) H est fermé;
(ii) la topologie de H est induite par celle de G;
(iii) H est un sous-groupe de Lie de G.
(i) $\Rightarrow$ (iii): cela résulte du § 1, prop. 2 (iv) (n° 1) et 14 (iii) (n° 7).
(iii) $\Rightarrow$ (ii): évident.
(ii) $\Rightarrow$ (i): si la topologie de H est induite par celle de G, H est fermé parce que H est complet (§ 1, n° 1, prop. 1).

#### Proposition 3 {#lie-iii-s6-prop-3 .statement}

*Soient G un groupe de Lie, H un sous-groupe intégral de G, M une variété analytique connexe non vide, f une application de M dans G et r $\in N_K$. Considérons les conditions suivantes:*
(i) $f$ est de classe $C^r$, et $f(M) \subset H$;
(ii) $f(M) \subset H$, et $f$, considérée comme application de M dans H, est de classe $C^r$;
(iii) $f$ est de classe $C^r$, $f(M)$ rencontre H, et l’image de $T_m(M)$ est contenue dans $f(m) . L(H)$ pour tout $m \in M$.
*On a (ii) $\Leftrightarrow$ (iii) $\Rightarrow$ (i).* Si la topologie de H admet une base dénombrable, les trois conditions sont équivalentes.
(ii) $\Rightarrow$ (i) et (ii) $\Rightarrow$ (iii): évident.
(iii) $\Rightarrow$ (ii): supposons vérifiée la condition (iii). D’après VAR, R, 9.2.8, $f$ est un morphisme de classe $C^r$ de M dans le feuilletage gauche associé à $L(H)$. Comme M est connexe, on a $f(M) \subset H$.
Si la topologie de H admet une base dénombrable, la condition (i) implique que $f$ est une application de classe $C^r$ de M dans H (VAR, R,9.2.8); donc (i) $\Rightarrow$ (ii).

#### Corollaire 1 {#lie-iii-s6-prop-3-cor-1 .statement}

*Soient G un groupe de Lie de dimension finie, H un sous-groupe intégral de G. Alors la sous-algèbre de Lie tangente en e à H ($\S 4$, n° 5, déf. 2 et 3) est $L(H)$, et la structure de groupe de Lie de H est la structure induite par celle de G.*
En effet, comme H est connexe de dimension finie, sa topologie admet une base dénombrable.

#### Corollaire 2 {#lie-iii-s6-prop-3-cor-2 .statement}

*Soient G un groupe de Lie, $H_1$ et $H_2$ des sous-groupes intégraux de G. On suppose que la topologie de $H_1$ admet une base dénombrable. Alors*
$$
H_2 \subset H_1 \iff L(H_2) \subset L(H_1),
$$
*et, si ces conditions sont vérifiées, $H_2$ est un sous-groupe intégral de $H_1$.*

La dernière assertion, et l’implication $L(H_2) \subset L(H_1) \Rightarrow H_2 \subset H_1$, résultent du cor. 2 de la prop. 1. L’implication inverse résulte de la prop. 3.

#### Corollaire 3 {#lie-iii-s6-prop-3-cor-3 .statement}

Soient $G$ un groupe de Lie, $H_1$ et $H_2$ des sous-groupes intégraux de $G$ dont la topologie admet une base dénombrable. Si $H_1$ et $H_2$ ont même ensemble sous-jacent, les structures de groupes de Lie de $H_1$ et $H_2$ sont égales.
Cela résulte du cor. 2.

#### Remarque 2 {#lie-iii-s6-n2-rem-2 .statement}

Soit $G$ un groupe de Lie de dimension finie. Soit $H$ un sous-groupe de $G$. Nous dirons, par abus de langage, que $H$ est un sous-groupe intégral de $G$ s’il existe une structure $S$ de groupe de Lie sur $H$ telle que $H$, muni de $S$, soit un sous-groupe intégral de $G$. D’après le cor. 3 de la prop. 3, si $S$ existe, $S$ est unique.

#### Remarque 3 {#lie-iii-s6-n2-rem-3 .statement}

Soit $V$ une variété de classe $C^r$. Soient $M$ une partie de $V$, $x$ et $y$ des éléments de $M$. Considérons la propriété suivante:
$P_{M,x,y}$: il existe $I, x_0, x_1, \ldots, x_n f_1, \ldots, f_n$ tels que: a) $I$ est une partie ouverte connexe de $K$; b) $x_0, \ldots, x_n$ sont dans $M$, $x_0 = x, x_n = y$; c) pour $1 \leq i \leq n$, $f_i$ est une application de classe $C^r$ de $I$ dans $V$ qui prend les valeurs $x_{i-1}$ et $x_i$, et $f_i(I) \subset M$.
Nous dirons que $M$ est une partie $C^r$-connexe de $V$ si, quels que soient les éléments $x, y$ de $M$, on a la propriété $P_{M,x,y}$.

#### Proposition 4 {#lie-iii-s6-prop-4 .statement}

Soient $G$ un groupe de Lie de dimension finie, $H$ un sous-groupe de $G$. Soit $r \in \mathbf{N}_K$. Les conditions suivantes sont équivalentes:
(i) $H$ est un sous-groupe intégral de $G$;
(ii) muni de la structure de groupe de Lie induite par celle de $G$, $H$ est connexe;
(iii) $H$ est $C^r$-connexe.
(ii) $\Rightarrow$ (i): évident.
(i) $\Rightarrow$ (iii): supposons $H$ muni d’une structure de groupe de Lie telle que $H$ soit un sous-groupe intégral de $G$. Utilisons les notations de la Remarque 3. L’ensemble des $y \in H$ tels que la propriété $P_{H,e,y}$ soit vraie est un sous-groupe ouvert de $H$. Comme $H$ est connexe, ce sous-groupe est égal à $H$, donc la condition (iii) est vérifiée.
(iii) $\Rightarrow$ (ii): supposons la condition (iii) vérifiée, et munissons $H$ de la structure induite par la structure de groupe de Lie de $G$. Soit $\mathfrak{h}$ la sous-algèbre tangente à $H$ en $e$. La composante neutre $H_0$ de $H$ est un sous-groupe intégral de $G$ tel que $L(H_0) = \mathfrak{h}$. Montrons que $H = H_0$. Il suffit de prouver ceci: soient $I$ une partie ouverte connexe de $K$, $f$ une application de classe $C^r$ de $I$ dans $G$ telle que $f(I) \subset H$, $\lambda$ et $\mu$ deux points de $I$; si $f(\lambda) \in H_0$, alors $f(\mu) \in H_0$. Or, pour tout $v \in I$, on a $(T_v f)(K) \subset f(v) \mathfrak{h}$ par définition de $\mathfrak{h}$, de sorte que notre assertion résulte de la prop. 3.

#### Remarque 4 {#lie-iii-s6-n2-rem-4 .statement}

Si $K = \mathbf{R}$, on peut aussi caractériser les sous-groupes intégraux de $G$ comme les sous-groupes qui, munis de la topologie induite par celle de $G$, sont connexes *par arcs* (\S 8, exerc. 4). Toutefois, il peut exister des sous-groupes *connexes* qui ne sont pas intégraux (AC, VI, \S 9, \S g, exerc. 9).

#### Corollaire {#lie-iii-s6-n2-cor-1 .statement}

*Soient $G$ un groupe de Lie de dimension finie, $H_1$ et $H_2$ deux sous-groupes intégraux de $G$. Le sous-groupe de $G$ engendré par $H_1$ et $H_2$, et le sous-groupe $(H_1, H_2)$ de $G$, sont des sous-groupes intégraux de $G$*.

Le sous-groupe $(G, G)$ de $G$ n’est pas toujours fermé (\S 9, exerc. 6).

Rappelons (\S 3, no 11, cor. 5 de la prop. 41) que si $a$ est une algèbre de dimension finie, $\mathrm{Aut}(a)$ est un sous-groupe de Lie de $\mathbf{GL}(a)$ et que $L(\mathrm{Aut}(a))$ est l’algèbre de Lie des dérivations de $a$.

#### Définition 2 {#lie-iii-s6-def-2 .statement}

*Soit $a$ une algèbre de Lie de dimension finie. On note $\mathrm{Ad}(a)$ ou $\mathrm{Int}(a)$, le sous-groupe intégral de $\mathrm{Aut}(a)$ d’algèbre de Lie $\mathrm{ad}(a)$. Les éléments de ce groupe s’appellent automorphismes intérieurs de $a$*.

Par transport de structure, $\mathrm{ad}(a)$ est invariant par $\mathrm{Aut}(a)$, donc $\mathrm{Int}(a)$ est distingué dans $\mathrm{Aut}(a)$. Compte tenu du \S 4, no 4, cor. 1 de la prop. 8, et du fait que $\mathrm{Int}(a)$ est connexe, les éléments de $\mathrm{Int}(a)$ sont les produits finis d’automorphismes de la forme $\exp \mathrm{ad}\, x$ où $x \in a$. En général, $\mathrm{Int}(a)$ n’est pas un sous-groupe de Lie de $\mathrm{Aut}(a)$ (exerc. 14).

### 3. Passage des algèbres de Lie aux groupes de Lie

#### Théorème 3 {#lie-iii-s6-thm-3 .statement}

(i) *Si $L$ est une algèbre de Lie de dimension finie, il existe un groupe de Lie $G$ simplement connexe tel que $L(G)$ soit isomorphe à $L$*.

(ii) *Soient $G_1$ et $G_2$ deux groupes de Lie connexes, avec $G_1$ simplement connexe. Soient $f$ un isomorphisme de $L(G_1)$ sur $L(G_2)$, $\varphi$ le morphisme de $G_1$ dans $G_2$ tel que $L(\varphi) = f$, et $N$ le noyau de $\varphi$. Alors $N$ est un sous-groupe discret du centre de $G_1$, et le morphisme de $G_1/N$ dans $G_2$ déduit de $\varphi$ est un isomorphisme de groupes de Lie. Si $G_2$ est simplement connexe, $\varphi$ est un isomorphisme*.

Soit $L$ une algèbre de Lie de dimension finie. Il existe un espace vectoriel $E$ de dimension finie tel qu’on puisse identifier $L$ à une sous-algèbre de Lie de $\mathrm{End}(E)$ (chap. I, \S 7, th. 2). Soit $H$ le sous-groupe intégral de $\mathbf{GL}(E)$ d’algèbre de Lie $L$. Soit $\hat{H}$ son revêtement universel (\S 1, no 9, Remarque). Alors $L(\hat{H})$ est isomorphe à $L$, d’où (i).

Soient $G_1, G_2, f, \varphi, N$ comme dans (ii). Alors $\varphi$ est étale, donc $\varphi(G_1)$ est un sous-groupe ouvert de $G_2$, donc $\varphi(G_1) = G_2$. D’autre part, $N$ est discret, donc contenu dans le centre de $G_1$ (INT, VII, \S 3, lemme 4). Il est clair que le morphisme de $G/N$ sur $G_2$ déduit de $\varphi$ est un isomorphisme de groupe de Lie. Si $G_2$ est simplement connexe, toute application étale de $G_1$ sur $G_2$ est injective, donc $N = \{e\}$.

#### Proposition 5 {#lie-iii-s6-prop-5 .statement}

Soit G un groupe de Lie réel connexe. Supposons donnée sur L(G) une structure d’algèbre de Lie normable complexe L’ compatible avec sa structure d’algèbre de Lie normable réelle. Il existe sur G une structure de groupe de Lie complexe et une seule compatible avec la structure de groupe de Lie réel et pour laquelle l’algèbre de Lie est L’.

D’après le § 4, n° 2, cor. 2 du th. 2, il suffit de prouver que la structure de L’ est invariante par Ad G. Soit φ une application exponentielle de G. D’après le § 4, n° 4, cor. 3 (i) de la prop. 8, il existe un voisinage V de 0 dans L(G) tel que la structure de L’ soit invariante par Ad φ(V). Or φ(V) engendre G parce que G est connexe.

La conclusion de la prop. 5 ne subsiste pas nécessairement si G n’est pas supposé connexe (exerc. 7).

#### Proposition 6 {#lie-iii-s6-prop-6 .statement}

Soit G un groupe de Lie complexe connexe. Si G est compact, G est commutatif.

L’application holomorphe g ↦ Ad g de G dans $\mathcal{L}(L(G))$ est constante (VAR, R, 3.3.7), donc ad $a = 0$ pour tout $a \in L(G)$ ($\S 3$, n° 12, prop. 44). Donc G est commutatif ($\S 4$, cor. 3 du th. 1).

### 4. Application exponentielle

#### Théorème 4 {#lie-iii-s6-thm-4 .statement}

Soit G un groupe de Lie. Il existe une application exponentielle de G et une seule définie dans L(G).

Il existe un voisinage ouvert convexe U de 0 dans L(G) et une application exponentielle φ de G définie sur U. On peut supposer, en choisissant U assez petit, que

$$
\varphi((\lambda + \lambda')a) = \varphi(\lambda a)\varphi(\lambda'a)
$$

pour $a \in L(G)$, $\lambda, \lambda'$ dans K, $\lambda a, \lambda'a, (\lambda + \lambda')a$ dans U.

Soit $a \in L(G)$. Il existe un entier $n > 0$ tel que $\frac{1}{n} a \in U$. Si m est un autre entier $> 0$ tel que $\frac{1}{m} a \in U$, on a $\frac{1}{nm} a \in U$, et la relation (1) entraîne

$$
\varphi\left(\frac{1}{n} a\right) = \left(\varphi\left(\frac{1}{nm} a\right)\right)^m, \quad \varphi\left(\frac{1}{m} a\right) = \left(\varphi\left(\frac{1}{nm} a\right)\right)^n;
$$

donc $\left(\varphi\left(\frac{1}{n} a\right)\right)^n = \left(\varphi\left(\frac{1}{m} a\right)\right)^m$. Il existe un prolongement $\psi : L(G) \to G$ de φ tel que $\psi(a) = \left(\varphi\left(\frac{1}{n} a\right)\right)^n$ pour $a \in L(G)$ et n entier $> 0$ tel que $\frac{1}{n} a \in U$. Il est clair que $\psi$ est analytique, et est une application exponentielle de G. Si $\psi' : L(G) \to G$ est une application exponentielle de G, $\psi$ et $\psi'$ coïncident dans un voisinage de 0, donc sont égales puisque $L(G)$ est connexe.

Quand on parlera désormais de l’application exponentielle de G, il s’agira de l’application considérée au th. 4. On la note exp_G ou exp s’il n’y a pas risque de confusion.

#### Exemple {#lie-iii-s6-n4-exa-1 .statement}

Soit A une algèbre associative unifière normée complète. Alors exp_A* est l’application exponentielle définie au chap. II, § 7, n° 3.

#### Proposition 7 {#lie-iii-s6-prop-7 .statement}

Soient G un groupe de Lie, a un élément de L(G). L’application $\lambda \mapsto \exp(\lambda a)$ de K dans G est l’unique morphisme $\varphi$ du groupe de Lie K dans G tel que $(\mathrm{T}_0 \varphi)1 = a$.

Les applications $(\lambda, \lambda') \mapsto \exp(\lambda a) \exp(\lambda' a)$ et $(\lambda, \lambda') \mapsto \exp(\lambda + \lambda') a$ de $K \times K$ dans G sont analytiques et coïncident dans un voisinage de $(0, 0)$. Comme $K \times K$ est connexe, ces applications sont égales. Donc $\varphi : \lambda \mapsto \exp(\lambda a)$ est un morphisme de groupes de Lie de K dans G. L’application tangente en 0 à $\lambda \mapsto \lambda a$ est l’application $\lambda \mapsto \lambda a$; et $T_e(\exp) = \mathrm{Id}_{L(G)}$; donc $(\mathrm{T}_0 \varphi)1 = a$. L’assertion d’unicité de la proposition résulte du th. 1.

#### Proposition 8 {#lie-iii-s6-prop-8 .statement}

Soit G un groupe de Lie. Quels que soient x, y dans L(G), on a, en notant n un entier,

$$
\exp(x + y) = \lim_{n \to + \infty} \left( \left( \exp \frac{1}{n} x \right) \left( \exp \frac{1}{n} y \right) \right)^n
$$

$$
\exp[x, y] = \lim_{n \to + \infty} \left( \left( \exp \frac{1}{n} x \right) \left( \exp \frac{1}{n} y \right) \left( \exp \frac{1}{n} x \right)^{-1} \left( \exp \frac{1}{n} y \right)^{-1} \right)^{n^2}.
$$

Compte tenu de la prop. 7, cela résulte de la prop. 4 du § 4, n° 3, en y prenant $\lambda = \frac{1}{n}$.

#### Proposition 9 {#lie-iii-s6-prop-9 .statement}

Soient G un groupe de Lie complexe, G’ le groupe de Lie réel sous-jacent. Alors $\exp_G = \exp_{G'}$.

Cela résulte de la prop. 5 du § 4, n° 3, et de l’analyticité de $\exp_G$ et $\exp_{G'}$.

#### Proposition 10 {#lie-iii-s6-prop-10 .statement}

Soient G et H des groupes de Lie, $\varphi$ un morphisme de G dans H.
(i) $\varphi \circ \exp_G = \exp_H \circ \mathrm{L}(\varphi)$.
(ii) Si G est un sous-groupe intégral de H, on a $\exp_G = \exp_H|L(G)$.

Les deux membres de l’égalité (i) sont des applications analytiques de L(G) dans H qui coïncident dans un voisinage de 0 (§ 4, prop. 8, n° 4), donc sont égales. L’assertion (ii) est un cas particulier de (i).

#### Corollaire 1 {#lie-iii-s6-prop-10-cor-1 .statement}

Soient G un groupe de Lie, G’ un sous-groupe de Lie de G, et $a \in L(G)$.
Les conditions suivantes sont équivalentes:
(i) $a \in L(G')$;

(ii) $\exp(\lambda a) \in G'$ pour $\lambda \in K$ et $|\lambda|$ assez petit;
(iii) $\exp(\lambda a) \in G'$ pour tout $\lambda \in K$.
On raisonne comme au § 4, n° 4, cor. 1 de la prop. 8.

#### Corollaire 2 {#lie-iii-s6-prop-10-cor-2 .statement}

Soient $G$ un groupe de Lie, $H$ un sous-groupe intégral de $G$, et $a \in L(G)$.
Considérons les conditions suivantes:
(i) $a \in L(H)$;
(ii) $\exp_G(\lambda a) \in H$ pour tout $\lambda \in K$.
On a (i) $\Rightarrow$ (ii). Si la topologie de $H$ admet une base dénombrable, on a (i) $\Leftrightarrow$ (ii).
Soit $i$ l’injection canonique de $H$ dans $G$. Si $a \in L(H)$, on a
$$
\exp_G(\lambda a) = (\exp_G \circ L(i))(\lambda a) = (i \circ \exp_H)(\lambda a) \in H.
$$
Donc (i) $\Rightarrow$ (ii). La réciproque pour $H$ à base dénombrable résulte de la prop. 3.

#### Corollaire 3 {#lie-iii-s6-prop-10-cor-3 .statement}

Soient $G$ un groupe de Lie, $\rho$ une représentation linéaire analytique de $G$, $x \in L(G)$ et $g \in G$.
(i) $\rho(\exp x) = \exp L(\rho)x$;
(ii) $\mathrm{Ad}(\exp x) = \exp \mathrm{ad}\, x$;
(iii) $g(\exp x)g^{-1} = \exp(\mathrm{Ad}\, g.x)$.
On raisonne comme au § 4, n° 4, cor. 2 et 3 de la prop. 8.

#### Corollaire 4 {#lie-iii-s6-prop-10-cor-4 .statement}

Soit $G$ un groupe de Lie connexe de dimension finie.
(i) On a $\mathrm{Int}(L(G)) = \mathrm{Ad}(G)$.
(ii) Soit $Z$ le centre de $G$. Alors $Z$ est un sous-groupe de Lie de $G$ dont l’algèbre de Lie est le centre de $L(G)$. L’application de $G/Z$ dans $\mathrm{Int}\, L(G)$ déduite de $g \mapsto \mathrm{Ad}\, g$ par passage au quotient est un isomorphisme de groupes de Lie.
L’assertion (i) résulte du cor. 3 (ii) et des remarques suivant la déf. 2. Soit $g \in G$. Pour que $\mathrm{Ad}\, g = \mathrm{Id}_{L(G)}$, il faut et il suffit que $\mathrm{Int}\, g$ coïncide avec $\mathrm{Id}_G$ dans un voisinage de $e$ (§ 4, n° 1, th. 1(ii)), donc dans $G$ tout entier; autrement dit, il faut et il suffit que $g \in Z$. Ceci posé, (ii) résulte du cor. 1 de la prop. 1.

#### Définition 3 {#lie-iii-s6-def-3 .statement}

Soit $G$ un groupe de Lie connexe de dimension finie. Le groupe de Lie $\mathrm{Int}(L(G)) = \mathrm{Ad}(G)$ s’appelle le groupe adjoint de $G$.

#### Proposition 11 {#lie-iii-s6-prop-11 .statement}

Soit $G$ un groupe de Lie commutatif connexe.
(i) $\exp$ est un morphisme étale du groupe de Lie additif $L(G)$ sur $G$.
(ii) Si $K = \mathbf{R}$, et si $G$ est de dimension finie, $G$ est isomorphe à un groupe de Lie de la forme $\mathbf{R}^p \times \mathbf{T}^q$ ($p, q$ entiers $\geqslant 0$).
D’après la formule de Hausdorff, on a $(\exp x)(\exp y) = \exp(x + y)$ pour $x, y$ assez voisins de 0, donc quels que soient x et y dans L(G) par prolongement analytique. Donc exp est un homomorphisme de groupes, et est étale puisque

$$
T_e(\exp) = \mathrm{Id}_{L(G)}.
$$

D’où (i). L’assertion (ii) résulte de (i) et de TG, VII, § 1, prop. 9.

#### Proposition 12 {#lie-iii-s6-prop-12 .statement}

*Soient G un groupe de Lie, et L = L(G). Pour tout x ∈ L, identifions T_x(L) à L, de sorte que la différentielle droite ω(x) de exp en x est une application linéaire de L dans L. Pour tout x ∈ L, on a*

$$
ω(x) = \sum_{n \geq 0} \frac{1}{(n + 1)!} (\mathrm{ad}\ x)^n.
$$

Les deux membres sont des fonctions analytiques de x, et sont égaux pour x assez voisin de 0 (§ 4, n° 3, prop. 6).

#### Remarque {#lie-iii-s6-n4-rem-1 .statement}

On a ω(x) . (ad x) = exp ad x − 1. On écrit, par abus de notation,

$$
ω(x) = \frac{\exp \mathrm{ad}\ x - 1}{\mathrm{ad}\ x}.
$$

#### Corollaire {#lie-iii-s6-n4-cor-1 .statement}

*Soient G un groupe de Lie complexe, et x ∈ L(G). L’application tangente en x à exp_G a pour noyau $\bigoplus_{n \in \mathbf{Z} - \{0\}} \mathrm{Ker}(\mathrm{ad}\ x - 2i\pi n)$.*

La fonction entière $z \mapsto \sum_{n \geq 0} \frac{1}{(n + 1)!} z^n$, égale à $\frac{e^z - 1}{z}$ pour $z \neq 0$, admet pour zéros les points de $2\pi i \mathbf{Z} - \{0\}$, qui sont tous des zéros simples. Le corollaire résulte alors de la prop. 12 et du lemme suivant:

#### Lemme 2 {#lie-iii-s6-lem-2 .statement}

*Soient E un espace de Banach complexe, u un élément de $\mathcal{L}(E)$, S le spectre de u dans $\mathcal{L}(E)$ (TS, I, § 1, n° 2), f une fonction complexe holomorphe dans un voisinage ouvert Ω de S. On suppose que f n’admet dans Ω qu’un nombre fini de zéros $z_1, \ldots, z_n$ deux à deux distincts, de multiplicités $h_1, \ldots, h_n$. Alors Kerf(u) est somme directe des Ker$(u - z_i)^{h_i}$ pour $1 \leq i \leq n$.

(Pour la définition de f(u), voir TS, I, § 4, n° 8.)

Il existe une fonction holomorphe g dans Ω, partout non nulle, telle que $f(z) = (z - z_1)^{h_1} \ldots (z - z_n)^{h_n} g(z)$. Alors $g(u) g^{-1}(u) = g^{-1}(u) g(u) = 1$, donc $\mathrm{Ker}\ f(u) = \mathrm{Ker}\prod_{i=1}^n (u - z_i)^{h_i}$. Considérons Kerf(u) comme un $\mathbf{C}[X]$-module grâce à la loi externe $(h, x) \mapsto h(u)x$ pour $h \in \mathbf{C}[X]$, $x \in \mathrm{Ker}\ f(u)$. On voit que Kerf(u) est somme directe des Ker$(u - z_i)^{h_i}$ en utilisant, A, VII, § 2, n° 1, prop. 1.

### 5. Application aux représentations linéaires

#### Proposition 13 {#lie-iii-s6-prop-13 .statement}

Soient G un groupe de Lie connexe, ρ une représentation linéaire analytique de G dans un espace normable complet E. Soient E₁, E₂ deux sous-espaces vectoriels fermés de E tels que E₂ ⊂ E₁. Les conditions suivantes sont équivalentes:
(i) ρ(g)x ≡ x (mod E₂) pour tout g ∈ G et tout x ∈ E₁;
(ii) L(ρ)(L(G)) applique E₁ dans E₂.
On a
$$
\begin{align*}
&\rho(g)x \equiv x \pmod{E_2} \quad \text{pour tout } g \in G \text{ et tout } x \in E_1 \\
\Leftrightarrow &\rho(\exp a)x \equiv x \pmod{E_2} \quad \text{pour tout } a \in L(G) \text{ et tout } x \in E_1 \\
\Leftrightarrow &(\exp L(\rho)a)x \equiv x \pmod{E_2} \quad \text{pour tout } a \in L(G) \text{ et tout } x \in E_1.
\end{align*}
$$
D’autre part, si u ∈ $\mathcal{L}(E)$, on a
$$
\begin{align*}
&\exp(\lambda u)x \equiv x \pmod{E_2} \quad \text{pour tout } \lambda \in K \text{ et tout } x \in E_1 \\
\Leftrightarrow &u(E_1) \subset E_2
\end{align*}
$$
d’où la proposition.

#### Corollaire 1 {#lie-iii-s6-prop-13-cor-1 .statement}

Pour que E₁ soit stable pour ρ, il faut et il suffit que E₁ soit stable pour L(ρ).
Il suffit de faire E₁ = E₂ dans la prop 13.

#### Corollaire 2 {#lie-iii-s6-prop-13-cor-2 .statement}

Supposons ρ de dimension finie. Pour que ρ soit simple (resp. semi-simple), il faut et il suffit que L(ρ) soit simple (resp. semi-simple).
Cela résulte du cor. 1.

#### Corollaire 3 {#lie-iii-s6-prop-13-cor-3 .statement}

Soit x ∈ E. Pour que x soit invariant par ρ(G), il faut et il suffit que x soit annulé par L(ρ)(L(G)) (c’est-à-dire que x soit invariant par L(ρ) au sens du chap. I, § 3, déf. 3).
Il suffit de faire E₁ = Kx, E₂ = 0 dans la prop. 13.

#### Corollaire 4 {#lie-iii-s6-prop-13-cor-4 .statement}

Soit ρ' une autre représentation linéaire analytique de G dans un espace normable complet E'. Soit T ∈ $\mathcal{L}(E, E')$. Les conditions suivantes sont équivalentes:
(i) Tρ(g) = ρ'(g)T pour tout g ∈ G;
(ii) TL(ρ)(a) = L(ρ')(a)T pour tout a ∈ L(G).
Soit σ la représentation linéaire de G dans $\mathcal{L}(E, E')$ déduite de ρ et ρ' (\S 3, n° 11, cor. 1 de la prop. 41). La condition (i) signifie que T est invariant par σ(G). La condition (ii) signifie que T est annulé par L(σ)(L(G)). Il suffit alors d’appliquer le cor. 3.

#### Corollaire 5 {#lie-iii-s6-prop-13-cor-5 .statement}

Supposons ρ et ρ' de dimension finie. Pour que ρ et ρ' soient équivalentes, il faut et il suffit que L(ρ) et L(ρ') soient équivalentes.
C’est un cas particulier du cor. 4.

#### Corollaire 6 {#lie-iii-s6-prop-13-cor-6 .statement}

Supposons G de dimension finie. Soit t ∈ U(G). Pour que L_t (resp. R_t) soit invariant à droite (resp. à gauche), il faut et il suffit que t appartienne au centre de U(G).

Pour que L_t (resp. R_t) soit invariant à droite (resp. à gauche), il faut et il suffit que ε_g \* t = t \* ε_g pour tout g ∈ G, c’est-à-dire que (Int g) \* t = t. Il existe un entier n tel que t ∈ U_n(G). D’après le cor. 3, et d’après la prop. 45 du § 3, n° 12, on a (Int g) \* t = t pour tout g ∈ G si et seulement si [a, t] = 0 pour tout a ∈ L(G), c’est-à-dire si et seulement si t commute à U(G).

### 6. Sous-groupes intégraux distingués

#### Lemme 3 {#lie-iii-s6-lem-3 .statement}

Soient G un groupe de Lie, H_1 et H_2 des sous-groupes intégraux dont la topologie admet une base dénombrable, et g ∈ G. Alors

$$
gH_1g^{-1} = H_2 \iff (\mathrm{Ad}\, g)(L(H_1)) = L(H_2).
$$

On a Ad g = T_e(Int g). Donc, par transport de structure, (Int g)(H_1) a pour algèbre de Lie (Ad g)(L(H_1)). Comme H_1 et H_2 sont à base dénombrable, dire que les ensembles H_2 et (Int g)(H_1) sont égaux revient à dire que les sous-groupes intégraux H_2 et (Int g)H_1 sont égaux (n° 2, cor. 3 de la prop. 3). Ceci posé, le lemme résulte du th. 2 (i).

#### Proposition 14 {#lie-iii-s6-prop-14 .statement}

Soient G un groupe de Lie, H un sous-groupe intégral dont la topologie admet une base dénombrable. Les conditions suivantes sont équivalentes:
(i) H est distingué dans G;
(ii) L(H) est invariant par Ad(G).
Si de plus G est connexe, ces conditions sont équivalentes à la suivante:
(iii) L(H) est un idéal de L(G).
Si de plus G est simplement connexe et L(H) de codimension finie dans L(G), ces conditions impliquent que H est un sous-groupe de Lie de G et que G/H est simplement connexe.

L’équivalence (i) ⇔ (ii) résulte du lemme 3. Si de plus G est connexe, la condition (ii) équivaut à dire que L(H) est stable pour ad L(G) (n° 5, cor. 1 de la prop. 13, et § 3, n° 12, prop. 44).

Supposons que G soit simplement connexe et que L(H) soit un idéal de codimension finie dans L(G). D’après le th. 3 du n° 3, il existe un groupe de Lie simplement connexe G' tel que L(G') soit isomorphe à L(G)/L(H). Il existe un morphisme continu f de L(G) sur L(G') de noyau L(H). D’après le th. 1 du n° 1, il existe un morphisme φ de G dans G' tel que L(φ) = f. Ce morphisme est une submersion, donc son noyau N est un sous-groupe de Lie de G tel que L(N) = Ker f = L(H). Donc H est la composante neutre de N et est par suite un sous-groupe de Lie de G. Soit ψ le morphisme de G/H dans G' déduit de φ par passage au quotient. Ce morphisme est étale; puisque G' est simplement connexe, ψ est un isomorphisme de G/H sur G'.

#### Corollaire 1 {#lie-iii-s6-prop-14-cor-1 .statement}

Soit $G$ un groupe de Lie simplement connexe de dimension finie. Soient $m, h$ des sous-algèbres de Lie de $L(G)$ telles que $L(G)$ soit produit semi-direct de $m$ par $h$. Soient $M, H$ les sous-groupes intégraux correspondants de $G$. Alors $M$ et $H$ sont des sous-groupes de Lie simplement connexes de $G$, et, en tant que groupe de Lie, $G$ est produit semi-direct de $M$ par $H$.

D’après la prop. 14, $H$ est un sous-groupe de Lie distingué de $G$ et le groupe de Lie $G/H$ est simplement connexe. Soit $\pi$ le morphisme canonique de $G$ sur $G/H$. Il existe un morphisme $\theta$ de $G/H$ dans $M$ tel que $L(\theta)$ soit l’isomorphisme canonique de $L(G)/L(H) = L(G)/h$ sur $L(M) = m$. Alors

$$
L(\pi \circ \theta) = L(\pi) \circ L(\theta) = \mathrm{Id}_{L(G/H)},
$$

donc $\pi \circ \theta = \mathrm{Id}_{G/H}$. D’après le n° 1, cor. 1 de la prop. 1, $\theta(G/H) = M$. D’après la prop. 8 du § 1, n° 4, $M$ est un sous-groupe de Lie de $G$, et le groupe de Lie $G$ est produit semi-direct de $M$ par $H$.

#### Corollaire 2 {#lie-iii-s6-prop-14-cor-2 .statement}

Soient $G$ un groupe de Lie simplement connexe de dimension finie, $H$ un sous-groupe de Lie connexe distingué de $G$, et $\pi$ le morphisme canonique de $G$ sur $G/H$.

(i) Il existe une application analytique $\rho$ de $G/H$ dans $G$ telle que $\pi \circ \rho = \mathrm{Id}_{G/H}$.

(ii) Pour toute application $\rho$ ayant les propriétés de (i), l’application $(h, m) \mapsto h\rho(m)$ de $H \times (G/H)$ dans $G$ est un isomorphisme de variétés analytiques.

(iii) $H$ et $G/H$ sont simplement connexes.

Soit $n = \dim G - \dim H$. Le corollaire est évident pour $n = 0$. Raisonnons par récurrence sur $n$.

Supposons qu’il existe un idéal de $L(G)$ contenant $L(H)$, distinct de $L(G)$ et $L(H)$. Soit $H'$ le sous-groupe de Lie connexe correspondant de $G$. Soient $\pi_1 : G \to G/H'$ et $\pi_2 : H' \to H'/H$ les morphismes canoniques. D’après l’hypothèse de récurrence, il existe des applications analytiques $\rho_1 : G/H' \to G$, $\rho_2 : H'/H \to H'$ telles que $\pi_1 \circ \rho_1 = \mathrm{Id}_{G/H'}$, $\pi_2 \circ \rho_2 = \mathrm{Id}_{H'/H}$. Soit $\pi_3 : G/H \to G/H'$ le morphisme canonique. Si $x \in G/H$, et si $y$ est un représentant de $x$ dans $G$, $y$ et $\rho_1(\pi_3(x))$ ont même image canonique modulo $H'$, donc $x^{-1}\pi(\rho_1(\pi_3(x))) \in H'/H$. Posons

$$
\rho(x) = \rho_1(\pi_3(x))\rho_2(\pi(\rho_1(\pi_3(x))))^{-1}x) \in G.
$$

Il est clair que $\rho$ est une application analytique de $G/H$ dans $G$. On a

$$
\begin{align*}
\pi(\rho(x)) &= \pi(\rho_1(\pi_3(x)))\pi_2(\rho_2(\pi(\rho_1(\pi_3(x))))^{-1}x)) \\
&= \pi(\rho_1(\pi_3(x)))\pi(\rho_1(\pi_3(x)))^{-1}x = x.
\end{align*}
$$

Si maintenant les seuls idéaux de $L(G)$ contenant $L(H)$ sont $L(G)$ et $L(H)$, l’algèbre de Lie $L(G)/L(H)$ est ou bien de dimension 1 ou bien simple. Dans les deux cas, $L(G)$ est produit semi-direct d’une sous-algèbre par $L(H)$; c’est évident dans le premier cas, et, dans le deuxième, cela résulte du chap. I, § 6, cor. 3 du th. 5. L’assertion (i) résulte alors du cor. 1.

L’assertion (ii) est évidente. L’assertion (iii) résulte de (i) et (ii).

Les conclusions du cor. 2 ne sont plus nécessairement vraies quand G est de dimension infinie, ou quand H n’est pas distingué (exerc. 8 et 15).

#### Corollaire 3 {#lie-iii-s6-prop-14-cor-3 .statement}

Soient G un groupe de Lie connexe de dimension finie, H un sous-groupe de Lie connexe distingué de G. Le morphisme canonique de $\pi_1(H)$ dans $\pi_1(G)$ est injectif.

Soient $G_1$ le revêtement universel de G, $\lambda$ l’application canonique de $G_1$ sur G. L’algèbre de Lie de $G_1$ s’identifie à $L(G)$. Le sous-groupe de Lie $\lambda^{-1}(H)$ de $G_1$ est distingué dans $G_1$, et son algèbre de Lie est $L(H)$. Soient $H_1$ la composante neutre de $\lambda^{-1}(H)$ et $\lambda_1 = \lambda|_{H_1}$. On a $L(H_1) = L(H)$, donc $\lambda_1$ est un morphisme étale de $H_1$ sur H. D’autre part, $H_1$ est simplement connexe (cor. 2), donc s’identifie au revêtement universel de H. Alors, d’après TG, XI, le morphisme canonique de $\pi_1(H)$ dans $\pi_1(G)$ s’identifie à l’injection canonique de Ker $\lambda_1$ dans Ker $\lambda$.

### 7. Primitives des formes différentielles à valeurs dans une algèbre de Lie

#### Proposition 15 {#lie-iii-s6-prop-15 .statement}

Soient G un groupe de Lie, M une variété de classe $C^r$ ($r \geqslant 2$), $\alpha$ une forme différentielle de classe $C^{r-1}$ et de degré 1 sur M à valeurs dans $L(G)$, telle que $d\alpha + [\alpha]^2 = 0$. On suppose M simplement connexe. Pour tout $x \in M$ et tout $s \in G$, il existe une application f de classe $C^{r-1}$ de M dans G et une seule telle que $f(x) = s$ et $f^{-1}.df = \alpha$.

L’unicité de f résulte du § 3, no 17, cor. 2 de la prop. 59, et du fait que M est connexe. Prouvons l’existence de f. Il existe un recouvrement ouvert $(U_i)_{i \in I}$ de M, et, pour tout $i \in I$, une application $g_i : U_i \to G$ de classe $C^{r-1}$ telle que $g_i^{-1}.dg_i = \alpha$ sur $U_i$ (§ 4, no 6, th. 5). D’après le § 3, no 17, cor. 2 de la prop. 59, $g_ig_j^{-1}$ est localement constante dans $U_i \cap U_j$. Posons $g_ig_j^{-1} = g_{ij}$. Soit $G_d$ le groupe G muni de la topologie discrète. Les $g_{ij} : U_i \cap U_j \to G_d$ sont continues, et $g_{ij}g_{jk} = g_{ik}$ dans $U_i \cap U_j \cap U_k$. Puisque M est simplement connexe, il existe des applications continues $\lambda_i : U_i \to G_d$ telles que $g_ig_i^{-1} = \lambda_i \lambda_j^{-1}$ dans $U_i \cap U_j$. Soit g l’application de M dans G ayant $\lambda_i^{-1}g_i$ pour restriction à $U_i$ quel que soit $i \in I$. Cette application est de classe $C^{r-1}$, et $g^{-1}.dg = \alpha$. L’application f de M dans G définie par $f = s(g(x))^{-1}g$ vérifie les conditions $f^{-1}.df = \alpha$ et $f(x) = s$.

### 8. Passage des lois d’opérations infinitésimales aux lois d’opérations

#### Lemme 4 {#lie-iii-s6-lem-4 .statement}

Soient G un groupe topologique connexe, X un espace topologique séparé, et $f_1, f_2$ des lois d’opérations à gauche (resp. à droite) de G dans X telles que, pour tout $x \in X$, les applications $s \mapsto f_1(s, x), s \mapsto f_2(s, x)$ de G dans X soient continues. On suppose qu’il existe un voisinage V de $\{e\} \times X$ dans $G \times X$ tel que $f_1$ et $f_2$ coïncident sur V. Alors $f_1 = f_2$.

Soient $x \in X$, et A l’ensemble des $g \in G$ tels que $f_1(g, x) = f_2(g, x)$. Alors A est fermé dans G. D’autre part, soit $g \in A$; posons $y = f_1(g, x) = f_2(g, x)$. Il existe un voisinage U de e dans G tel que $f_1(t, y) = f_2(t, y)$ pour $t \in U$, autrement dit tel que $f_1(t', x) = f_2(t', x)$ pour $t' \in Ug$ (resp. $gU$). Donc A est ouvert dans G, et par suite $A = G$.

#### Proposition 16 {#lie-iii-s6-prop-16 .statement}

*Soient G un groupe de Lie connexe, X une variété séparée de classe $C^r$, et $f_1, f_2$ des lois d’opérations à gauche (resp. à droite) de classe $C^r$ de G dans X. Si les lois d’opérations infinitésimales associées à $f_1$ et $f_2$ sont égales, on a $f_1 = f_2$.*
   D’après le § 4, n° 7, cor. de la prop. 11, il existe un voisinage V de $\{e\} \times X$ dans $G \times X$ tel que $f_1$ et $f_2$ coïncident dans V. Donc $f_1 = f_2$ (lemme 4).

#### Lemme 5 {#lie-iii-s6-lem-5 .statement}

*Soient G un groupe topologique simplement connexe, X un espace topologique séparé, U un voisinage ouvert de e dans G, $\psi$ une application continue de $U \times X$ dans X telle que $\psi(e, x) = x$ et $\psi(s, \psi(t, x)) = \psi(st, x)$ quels que soient $x \in X$ et $s, t$ dans U tels que $st \in U$. Soit W un voisinage ouvert connexe symétrique de e tel que $W^3 \subset U$. Il existe une loi d’opération à gauche continue $\psi'$ de G dans X et une seule telle que $\psi'$ et $\psi$ coïncident dans $W \times X$. Si G est un groupe de Lie et X une variété de classe $C^r$, et si $\psi$ est de classe $C^r$, alors $\psi'$ est de classe $C^r$.
   L’unicité de $\psi$ résulte du lemme 4. Soit P le groupe des permutations de X. Pour $u \in W^3$, l’application $x \mapsto \psi(u, x)$ est un élément $f(u)$ de P, et
   $$
   f(u_1 u_2 u_3) = f(u_1) f(u_2) f(u_3)
   $$
   pour $u_1, u_2, u_3$ dans W. Appliquant le lemme 1 du n° 1, on obtient un morphisme $f'$ de G dans P qui prolonge $f|W$. Posons $\psi'(g, x) = f'(g)(x)$ pour tout $(g, x) \in G \times X$. Alors $\psi'$ est une loi d’opération à gauche de G dans X qui coïncide avec $\psi$ dans $W \times X$. Comme $\psi'(g, \psi'(g', x)) = \psi'(gg', x)$ pour $(g, g', x) \in G \times G \times X$, la continuité de $\psi$ dans $W \times X$ entraîne la continuité de $\psi'$ dans $gW \times X$ quel que soit $g \in G$. Donc $\psi'$ est continue. Si $\psi$ est de classe $C^r$, on voit de même que $\psi'$ est de classe $C^r$.

#### Théorème 5 {#lie-iii-s6-thm-5 .statement}

*Soient G un groupe de Lie simplement connexe, X une variété compacte de classe $C^r$ ($r \geq 2$), et $a \mapsto D_a$ une loi d’opération infinitésimale à gauche (resp. à droite) de classe $C^{r-1}$ de $L(G)$ dans X. Il existe une loi d’opération à gauche (resp. à droite) de classe $C^{r-1}$, et une seule, de G dans X telle que la loi d’opération infinitésimale associée soit $a \mapsto D_a$.
   L’unicité résulte de la prop. 16. D’après le § 4, n° 7, cor. 1 du th. 6, il existe un voisinage V de $\{e\} \times X$ dans $G \times X$, et un morceau de loi d’opération à gauche (resp. à droite) de classe $C^{r-1}$ de G dans X, défini dans V, tel que la loi d’opération infinitésimale associée soit $a \mapsto D_a$. Comme X est compacte, on peut supposer V de la forme $U \times X$, où U est un voisinage ouvert de e dans G. Il suffit alors d’appliquer le lemme 5.

### 9. Application exponentielle dans le groupe linéaire

#### Proposition 17 {#lie-iii-s6-prop-17 .statement}

Soient $\Delta$ l’ensemble des $z \in \mathbf{C}$ tels que $-\pi < \mathcal{J}(z) < \pi$, et $\Delta'$ l’ensemble des $z \in \mathbf{C}$ qui ne sont pas réels $\leqslant 0$. Soient $E$ un espace normable complet sur $\mathbf{C}$, $A$ (resp. $A'$) l’ensemble des $x \in \mathcal{L}(E)$ dont le spectre $\mathrm{Sp}\,x$ est contenu dans $\Delta$ (resp. dans $\Delta'$). Alors $A$ (resp. $A'$) est une partie ouverte de $\mathcal{L}(E)$ (resp. de $\mathbf{GL}(E)$), et les applications $\exp : A \to A'$ et $\log : A' \to A$ (TS, I, § 4, n° 9) sont des isomorphismes réciproques de variétés analytiques.

Cela résulte de TS, I, § 4, prop. 10 et n° 9.

#### Théorème 6 {#lie-iii-s6-thm-6 .statement}

Soient $E$ un espace hilbertien réel ou complexe, $U$ le groupe unitaire de $E$.

(i) L’ensemble $H$ des éléments hermitiens de $\mathcal{L}(E)$ est, pour la structure d’espace normé réel, un sous-espace vectoriel fermé de $\mathcal{L}(E)$ admettant un supplémentaire topologique.

(ii) L’ensemble $H'$ des éléments $\geqslant 0$ de $\mathbf{GL}(E)$ est une sous-variété analytique réelle de $\mathbf{GL}(E)$.

(iii) La restriction à $H$ de l’application $\exp$ est un isomorphisme de variétés analytiques réelles de $H$ sur $H'$.

(iv) L’application $(h, u) \mapsto (\exp h)u$ de $H \times U$ dans $\mathbf{GL}(E)$ est un isomorphisme de variétés analytiques réelles.

Rappelons que, si $x \in \mathcal{L}(E)$, on note $x^*$ l’adjoint de $x$. Soit $H_1$ l’ensemble des $x \in \mathcal{L}(E)$ tels que $x^* = -x$. La formule $x = \frac{1}{2}(x + x^*) + \frac{1}{2}(x - x^*)$ prouve que, pour sa structure d’espace normé réel, $\mathcal{L}(E)$ est somme directe topologique de $H$ et $H_1$, d’où (i).

Supposons $K = \mathbf{C}$. Avec les notations de la prop. 17, $H'$ est l’ensemble des $h \in H \cap A'$ tels que $\mathrm{Sp}\,h \subset \mathbf{R}_+^*$. Comme $\exp(\mathbf{R}) = \mathbf{R}_+^*$, (ii) et (iii) résultent de la prop. 17 et de TS, I, § 4, prop. 8 et § 6, n° 5. L’application $(h, u) \mapsto y = (\exp h)u$ de $H \times U$ dans $\mathbf{GL}(E)$ est bijective d’après TS, I, § 6, prop. 15. Elle est analytique réelle d’après ce qui précède. L’application $y \mapsto h = \frac{1}{2} \log(y y^*)$ est analytique réelle, donc aussi l’application $y \mapsto u = (\exp h)^{-1}y$. D’où (iv).

Supposons $K = \mathbf{R}$. Soient $\tilde{E}$ l’espace hilbertien complexifié de $E$ et $J$ l’application $\xi + i\eta \mapsto \xi - i\eta$ (pour $\xi, \eta$ dans $E$) de $\tilde{E}$ dans $\tilde{E}$. Notons $\tilde{H}, \tilde{H}', \tilde{U}$ les ensembles définis pour $\tilde{E}$ comme $H, H', U$ pour $E$. Alors $H$ (resp. $H', U$) s’identifie à l’ensemble des $x \in \tilde{H}$ (resp. $\tilde{H}', \tilde{U}$) tels que $J x J^{-1} = x$. Les propriétés (ii), (iii), (iv) résultent alors facilement de (i) et des propriétés analogues dans le cas complexe.

#### Proposition 18 {#lie-iii-s6-prop-18 .statement}

Soient $E$ un espace normable complet sur $\mathbf{C}$, $v \in \mathcal{L}(E)$, et $g = \exp v$. On suppose que $\mathrm{Sp}(v)$ ne contient aucun des points $2i\pi n$ avec $n \in \mathbf{Z} - \{0\}$. Alors, pour tout $x \in E$, les conditions $vx = 0$ et $gx = x$ sont équivalentes.

Cela résulte du lemme 2 du n° 4, appliqué à la fonction $z \mapsto e^z - 1$.

#### Corollaire 1 {#lie-iii-s6-prop-18-cor-1 .statement}

Soient $E$ un espace normable complet sur $\mathbf{C}$, $F$ l’espace des applications n-linéaires continues de $E^n$ dans $E$. Pour tout $v \in \mathcal{L}(E)$, soit $\sigma(v)$ l’élément de $\mathcal{L}(F)$ défini par
$$
(\sigma(v)f)(x_1, \ldots, x_n) = v(f(x_1, \ldots, x_n)) - \sum_{i=1}^n f(x_1, \ldots, vx_i, \ldots, x_n).
$$
Pour tout $g \in \mathbf{GL}(E)$, soit $\rho(g)$ l’élément de $\mathbf{GL}(F)$ défini par
$$
(\rho(g)f)(x_1, \ldots, x_n) = g(f(g^{-1}x_1, \ldots, g^{-1}x_n)).
$$
Soit $u \in \mathcal{L}(E)$ tel que tout $z \in \mathrm{Sp}\,u$ vérifie $|\mathcal{J}(z)| < \frac{2\pi}{n+1}$. Alors, pour tout $f \in F$, les conditions $\sigma(u)f = 0$ et $\rho(\exp u)f = f$ sont équivalentes.

On a $\mathbf{L}(\rho) = \sigma$ (\S 3, no 11, cor. 1 de la prop. 41), donc $\rho(\exp u) = \exp \sigma(u)$ (no 4, cor. 3 de la prop. 10). Compte tenu de la prop. 18, il suffit alors de prouver que $\mathrm{Sp}\,\sigma(u)$ ne rencontre pas $2i\pi(\mathbf{Z} - \{0\})$. Or cela résulte du lemme suivant:

#### Lemme 6 {#lie-iii-s6-lem-6 .statement}

Si $v \in \mathcal{L}(E)$, on a $\mathrm{Sp}\,\sigma(v) \subset \mathrm{Sp}\,v + \mathrm{Sp}\,v + \cdots + \mathrm{Sp}\,v$ où la somme comporte $n+1$ termes.

Définissons des éléments $v_0, v_1, \ldots, v_n$ de $\mathcal{L}(F)$ en posant, pour tout $f \in F$,
$$
\begin{align*}
(v_0f)(x_1, \ldots, x_n) &= v(f(x_1, \ldots, x_n)) \\
(v_if)(x_1, \ldots, x_n) &= -f(x_1, \ldots, vx_i, \ldots, x_n) \quad \text{pour } 1 \leq i \leq n.
\end{align*}
$$
Alors $\sigma(v) = \sum_{i=0}^n v_i$, et les $v_i$ sont deux à deux permutables. Soit $A$ la sous-algèbre fermée pleine de $\mathcal{L}(F)$ engendrée par les $v_i$; elle est commutative (TS, I, \S 1, no 4), et $\mathrm{Sp}_{\mathcal{L}(F)} v' = \mathrm{Sp}_A v' \subset \sum_{i=0}^n \mathrm{Sp}\,v_i$ (TS, I, \S 3, prop. 3 (ii)). Or, si $\lambda \in \mathbf{C}$ est tel que $v - \lambda$ soit inversible, il est clair que les $v_i - \lambda$ sont inversibles, donc $\mathrm{Sp}\,v_i \subset \mathrm{Sp}\,v$ pour tout $i$.

#### Corollaire 2 {#lie-iii-s6-lem-6-cor-2 .statement}

Soient $E$ une algèbre normable complète sur $\mathbf{C}$, et $w \in \mathcal{L}(E)$. On suppose que tout $z \in \mathrm{Sp}\,w$ vérifie $|\mathcal{J}(z)| < \frac{2\pi}{3}$. Les conditions suivantes sont équivalentes:
(i) $w$ est une dérivation de $E$;
(ii) $\exp w$ est un automorphisme de $E$.

Cela résulte du cor. 1 où l’on fait $n = 2$ et où l’on prend pour $f$ la multiplication de $E$.

#### Proposition 19 {#lie-iii-s6-prop-19 .statement}

Soient $E$ un espace normable complet sur $\mathbf{C}$, $v \in \mathcal{L}(E)$, et $g = \exp v$. On suppose que tout $z \in \mathrm{Sp}\,v$ vérifie $-\pi < \mathcal{J}(z) < \pi$. Alors, pour tout sous-espace vectoriel fermé $E'$ de $E$, les conditions $v(E') \subset E'$ et $g(E') = E'$ sont équivalentes.

La condition $v(E') \subset E'$ entraîne $g(E') \subset E'$ et $g^{-1}(E') \subset E'$ donc $g(E') = E'$. Supposons $g(E') = E'$. Utilisons les notations $\Delta, \Delta'$ de la prop. 17. Puisque $\mathrm{Sp}\,v$

#### Corollaire {#lie-iii-s6-n9-cor-1 .statement}

*Soient E un espace normable complet sur $\mathbf{C}$, $v \in \mathcal{L}(E)$, et $g = \exp v$. On suppose que tout $z \in Sp\ v$ vérifie $-\frac{\pi}{2} < \mathcal{J}(z) < \frac{\pi}{2}$. Alors, pour tout sous-espace vectoriel fermé M de $\mathcal{L}(E)$, les conditions $gMg^{-1} = M$ et $[v, M] \subset M$ sont équivalentes.*

Soient $F = \mathcal{L}(E)$, $g'$ l’application $f \mapsto gfg^{-1}$ de $F$ dans $F$, et $v'$ l’application $f \mapsto [v, f]$ de $F$ dans $F$. On a $g' = \exp v'$ (n° 4, cor. 3 de la prop. 10, et § 3, n° 11, cor. 1 de la prop. 41). Le lemme 6 prouve que $-\pi < \mathcal{J}(z) < \pi$ pour tout $z \in Sp\ v'$. Il suffit alors d’appliquer la prop. 19.

### 10. Complexification d’un groupe de Lie réel de dimension finie

#### Lemme 7 {#lie-iii-s6-lem-7 .statement}

*Soient B un groupe, A un sous-groupe distingué de B, C le groupe B/A, i : A → B et p : B → C les morphismes canoniques. Soient A' un groupe, f un homomorphisme de A dans A'. Soit ω un morphisme de B dans le groupe des automorphismes de A'. On suppose que, pour $a \in A, a' \in A', b \in B$, on a*

$$
f(bab^{-1}) = \omega(b)f(a), \quad \omega(a)a' = f(a)a'f(a)^{-1}.
$$

*Soient B'' le produit semi-direct de B par A' relatif à ω, q le morphisme canonique de B'' sur B.*

(i) *L’application $a \mapsto (f(a^{-1}), i(a))$ de A dans B'' est un morphisme de A sur un sous-groupe distingué D de B''. Soient B' = B''/D, et $i': A' \to B'$, $g : B \to B'$ les morphismes de A' et B dans B' déduits par passage au quotient des injections canoniques de A' et B dans B''.

(ii) *Le morphisme $p \circ q$ de B'' dans C définit par passage au quotient un morphisme $p'$ de B' dans C.

(iii) *i' est injectif, $p'$ est surjectif, $\mathrm{Ker}(p') = \mathrm{Im}(i')$, et le diagramme ci-dessous est commutatif*

(4)

$$
\begin{array}{ccc}
A & \xrightarrow{i} & B & \xrightarrow{p} & C \\
\downarrow f & & \downarrow g & & \downarrow \mathrm{Id}_C \\
A' & \xrightarrow{i'} & B' & \xrightarrow{p'} & C.
\end{array}
$$

(iv) Si $b \in \mathbf{B}$ et $a' \in \mathbf{A}'$, on a
$$
g(b)i'(a')g(b)^{-1} = i'(\omega(b)a').
$$
(i) Pour $a_1, a_2$ dans $\mathbf{A}$, on a, dans $\mathbf{B}''$,
$$
(f(a_1^{-1}), i(a_1))(f(a_2^{-1}), i(a_2)) = (f(a_1^{-1})(\omega(a_1)f(a_2^{-1})), i(a_1)i(a_2))
= (f(a_1^{-1})f(a_1a_2^{-1}a_1^{-1}), i(a_1a_2)) = (f((a_1a_2)^{-1}), i(a_1a_2))
$$
donc $a \mapsto (f(a^{-1}), i(a))$ est un homomorphisme $h$ de $\mathbf{A}$ dans $\mathbf{B}''$. Soient $a \in \mathbf{A}$, $a' \in \mathbf{A}'$, $b \in \mathbf{B}$; on a, dans $\mathbf{B}''$,
$$
bh(a)b^{-1} = bf(a^{-1})ab^{-1} = (\omega(b)f(a^{-1}))(bab^{-1})
= f(ba^{-1}b^{-1})(bab^{-1}) = h(bab^{-1})
$$
$$
a'h(a){a'}^{-1} = a'f(a^{-1})a{a'}^{-1} = a'f(a^{-1})(\omega(a){a'}^{-1})a
= a'f(a^{-1})f(a){a'}^{-1}f(a^{-1})a = h(a)
$$
donc $h(\mathbf{A}) = \mathbf{D}$ est distingué dans $\mathbf{B}''$.
(ii) Pour $a \in \mathbf{A}$, on a
$$
(p \circ q)(h(a)) = p(q(f(a^{-1})a)) = p(a) = e
$$
donc $p \circ q$ est trivial dans $\mathbf{D}$.
(iii) Soit $a' \in \mathbf{A}'$ tel que $i'(a') = e$; on a $a' \in \mathbf{D}$, donc il existe un $a \in \mathbf{A}$ tel que $a' = f(a^{-1})a$; cela entraîne $a = e$, d’où $a' = e$; ainsi, $i'$ est injectif. Comme $p$ et $q$ sont surjectifs, $p'$ est surjectif.
Notons $r$ le morphisme canonique de $\mathbf{B}''$ sur $\mathbf{B}'$. Soient $a' \in \mathbf{A}'$, $b \in \mathbf{B}$, et $b' = r(a'b)$. Si $b' \in \operatorname{Im}(i')$, il existe $a'_1 \in \mathbf{A}'$ tel que $b' = r(a'_1)$; alors il existe $a \in \mathbf{A}$ tel que $a'b = a'_1f(a^{-1})a$, d’où $b = a \in \mathbf{A}$, et
$$
p'(b') = p(q(a'b)) = p(b) = e;
$$
ainsi, $\operatorname{Im}(i') \subset \operatorname{Ker}(p')$. Conservons les notations $a', b, b'$, mais supposons $b' \in \operatorname{Ker}(p')$; alors $e = p'(b') = p(q(a'b)) = p(b)$, donc $b \in \mathbf{A}$, d’où
$$
b' = r(a'f(b)f(b^{-1})b) = r(a'f(b)) \in \operatorname{Im}(i');
$$
ainsi, $\operatorname{Ker}(p') \subset \operatorname{Im}(i')$.
Si $a \in \mathbf{A}$, on a
$$
i'(f(a)) = r(f(a)) = r(f(a)f(a^{-1})a) = r(a) = g(i(a)).
$$
Si $b \in \mathbf{B}$, on a
$$
p'(g(b)) = p(b)
$$
donc le diagramme (4) est commutatif.
(iv) Soient $b \in \mathbf{B}$, $a' \in \mathbf{A}'$. On a
$$
g(b)i'(a')g(b)^{-1} = r(b)r(a')r(b)^{-1} = r(ba'b^{-1})
= r(\omega(b)a') = i'(\omega(b)a').
$$

#### Proposition 20 {#lie-iii-s6-prop-20 .statement}

Soit G un groupe de Lie réel de dimension finie.

(i) Il existe un groupe de Lie complexe $\tilde{G}$ et un morphisme $\mathbf{R}$-analytique $\gamma$ de G dans $\tilde{G}$ ayant les propriétés suivantes: pour tout groupe de Lie complexe H et tout morphisme $\mathbf{R}$-analytique $\varphi$ de G dans H, il existe un morphisme $\mathbf{C}$-analytique $\psi$ de $\tilde{G}$ dans H et un seul tel que $\varphi = \psi \circ \gamma$.

(ii) Si $(\tilde{G}', \gamma')$ a les mêmes propriétés que $(G, \gamma)$, il existe un isomorphisme $\theta$ et un seul de $\tilde{G}$ sur $\tilde{G}'$ tel que $\theta \circ \gamma = \gamma'$.

(iii) L’application $\mathbf{C}$-linéaire de $L(G) \otimes \mathbf{C}$ dans $L(\tilde{G})$ qui prolonge $L(\gamma)$ est surjective; en particulier $\dim_{\mathbf{C}}(\tilde{G}) \leq \dim_{\mathbf{R}}(G)$.

L’assertion (ii) est évidente. Prouvons l’existence d’un couple $(\tilde{G}, \gamma)$ avec les propriétés (i) et (iii).

a) Supposons d’abord G connexe. Soient $g = L(G)$, $g_{\mathbf{C}} = g \otimes_{\mathbf{R}} \mathbf{C}$ la complexification de g, S (resp. S’) le groupe de Lie réel (resp. complexe) simplement connexe d’algèbre de Lie g (resp. $g_{\mathbf{C}}$), $\sigma$ l’unique morphisme $\mathbf{R}$-analytique de S dans S’ tel que $L(\sigma)$ soit l’injection canonique de g dans $g_{\mathbf{C}}$. Soient $\pi$ l’unique morphisme $\mathbf{R}$-analytique de S sur G tel que $L(\pi) = \mathrm{Id}_{L(G)}$, et F = Ker $\pi$.

![Diagramme commutatif](https://i.imgur.com/3Q5z5QG.png)

Pour tout groupe de Lie complexe H et tout morphisme $\mathbf{R}$-analytique $\varphi$ de G dans H, $L(\varphi): g \to L(H)$ possède un unique prolongement $\mathbf{C}$-linéaire à $g_{\mathbf{C}}$, et cette extension est de la forme $L(\varphi^*)$, où $\varphi^*$ est un morphisme $\mathbf{C}$-analytique de S’ dans H. On a

$$
L(\varphi \circ \pi) = L(\varphi) \circ L(\pi) = L(\varphi) = L(\varphi^*) \circ L(\sigma) = L(\varphi^* \circ \sigma),
$$

donc $\varphi \circ \pi = \varphi^* \circ \sigma$. Par suite $\varphi^*(\sigma(F)) = \varphi(\pi(F)) = \{e\}$, d’où

$$
\sigma(F) \subset \mathrm{Ker}\, \varphi^*.
$$

Soit P l’intersection des $\mathrm{Ker}\, \varphi^*$ pour $\varphi$ variable. C’est un sous-groupe de Lie distingué de S’ (n° 2, cor. 3 de la prop. 1). Soient $\tilde{G} = S'/P$, et $\lambda: S' \to \tilde{G}$ le morphisme canonique. On a $\sigma(F) \subset P$, donc il existe un morphisme $\mathbf{R}$-analytique $\gamma$ et un seul de G dans $\tilde{G}$ tel que $\gamma \circ \pi = \lambda \circ \sigma$. Si $\psi: \tilde{G} \to H$ désigne le morphisme déduit de $\varphi^*$ par passage au quotient, on a

$$
(\psi \circ \gamma) \circ \pi = \psi \circ (\lambda \circ \sigma) = \varphi^* \circ \sigma = \varphi \circ \pi
$$

d’où $\psi \circ \gamma = \varphi$. Il est clair que $L(\psi)$, donc $\psi$, sont déterminés de manière unique par l’égalité $\psi \circ \gamma = \varphi$. On a ainsi prouvé que le couple $(\tilde{G}, \gamma)$ possède les propriétés (i) et (iii).

b) Passons au cas général. Soient $F$ la composante neutre de $G$, $M = G/F$, $i : F \to G$ et $p : G \to M$ les morphismes canoniques. Appliquons à $F$ la partie a) de la démonstration. On obtient un couple $(\tilde{F}, \delta)$. Pour tout $g \in G$, $\mathrm{Int}\,g|F = \omega'(g)$ est un automorphisme de $F$. D’après la propriété universelle de $\tilde{F}$, il existe un automorphisme $\omega(g)$ du groupe de Lie complexe $\tilde{F}$, et un seul, tel que $\delta \circ \omega'(g) = \omega(g) \circ \delta$. Il est clair que $\omega$ est un morphisme de $G$ dans $\mathrm{Aut}(\tilde{H})$. Si $g \in G$ et $f \in F$, on a
$$
\delta(gf g^{-1}) = (\delta \circ \omega'(g)) (f) = (\omega(g) \circ \delta)(f) = \omega(g)(\delta(f)).
$$
Si $f \in F$, on a $\delta \circ (\mathrm{Int}_F f) = (\mathrm{Int}_{\tilde{F}} \delta(f)) \circ \delta$, et $\mathrm{Int}_{\tilde{F}} \delta(f)$ est un automorphisme du groupe de Lie complexe $\tilde{F}$; donc $\mathrm{Int}_{\tilde{F}} \delta(f) = \omega(f)$.

On peut donc appliquer le lemme 7, ce qui donne un diagramme

$$
\begin{array}{ccc}
F & \xrightarrow{i} & G & \xrightarrow{p} & M \\
\downarrow{\delta} & & \downarrow{\gamma} & & \downarrow{\mathrm{Id}} \\
\tilde{F} & \xrightarrow{\tilde{i}} & \tilde{G} & \xrightarrow{\tilde{p}} & M.
\end{array}
$$

Identifions $\tilde{F}$ à un sous-groupe distingué de $\tilde{G}$ grace à $\tilde{i}$. Le groupe $\tilde{G}$ est engendré par $\tilde{F}$ et $\gamma(G)$; donc les automorphismes de $\tilde{F}$ définis par les éléments de $\tilde{G}$ sont des automorphismes de la structure de groupe de Lie complexe. D’après le § 1, n° 9, prop. 18, il existe une structure de groupe de Lie complexe et une seule sur $\tilde{G}$ telle que $\tilde{F}$ soit un sous-groupe de Lie ouvert de $\tilde{G}$. Nous munirons désormais $\tilde{G}$ de cette structure. Comme $\delta$ est $\mathbf{R}$-analytique, $\gamma$ est $\mathbf{R}$-analytique.

Le couple $(\tilde{G}, \gamma)$ possède la propriété (iii) de la proposition. Montrons qu’il possède la propriété (i). Soient $H$ un groupe de Lie complexe et $\psi$ un morphisme $\mathbf{R}$-analytique de $G$ dans $H$. Il existe un morphisme $\mathbf{C}$-analytique $\eta$ de $\tilde{F}$ dans $H$ tel que $\eta \circ \delta = \varphi|F$. Soit $g \in G$. Les applications
$$
f \mapsto \eta(\omega(g)f), \quad f \mapsto \varphi(g)\eta(f)\varphi(g)^{-1}
$$
de $\tilde{F}$ dans $H$ sont des morphismes $\mathbf{C}$-analytiques; elles coïncident dans $\delta(F)$, car, si $f' \in F$, on a
$$
\varphi(g)\eta(\delta(f'))\varphi(g)^{-1} = \varphi(g)\varphi(f')\varphi(g)^{-1} = \varphi(gf'g^{-1})
= \eta(\delta(gf'g^{-1})) = \eta(\omega(g)\delta(f'));
$$
par suite, $\eta(\omega(g)f) = \varphi(g)\eta(f)\varphi(g)^{-1}$ pour tout $g \in G$ et tout $f \in \tilde{F}$. Si $G'$ désigne le produit semi-direct de $G$ et $\tilde{F}$ relatif à $\omega$, il existe donc un morphisme $\zeta$ du groupe $G'$ dans $H$ qui coïncide avec $\varphi$ dans $G$ et avec $\eta$ dans $\tilde{F}$. Pour $f \in F$, on a
$$
\zeta(\delta(f^{-1})f) = \eta(\delta(f^{-1}))\varphi(f) = \varphi(f^{-1})\varphi(f) = e.
$$

Donc $\zeta$ définit par passage au quotient un morphisme $\psi$ de $\tilde{G}$ dans $H$. On a $\psi \circ \gamma = \varphi$ et $\psi \circ \tilde{i} = \eta$; cette dernière égalité entraîne que $\psi$ est $\mathbf{C}$-analytique.

Enfin, soit $\psi'$ un morphisme $\mathbf{C}$-analytique de $\tilde{G}$ dans $H$ tel que $\varphi = \psi' \circ \gamma$. Alors
$$
\psi' \circ \tilde{i} \circ \delta = \psi' \circ \gamma \circ i = \varphi \circ i = \psi \circ \tilde{i} \circ \delta
$$
donc $\psi' \circ \tilde{i} = \psi \circ \tilde{i}$. Comme $\tilde{G}$ est engendré par $\tilde{i}(\tilde{F})$ et $\gamma(G)$, on a $\psi' = \psi$.

#### Définition 4 {#lie-iii-s6-def-4 .statement}

*On dit que* $(\tilde{G}, \gamma)$, *ou simplement* $\tilde{G}$, *est la complexification universelle de* $G$.

#### Remarque 1 {#lie-iii-s6-n10-rem-1 .statement}

Soit $(\tilde{G}, \gamma)$ la complexification universelle de $G$. Soit $G_0$ (resp. $\tilde{G}_0$) la composante neutre de $G$ (resp. $\tilde{G}$). D’après la démonstration de la prop. 20, $(\tilde{G}_0, \gamma|G_0)$ est la complexification universelle de $G_0$, et le morphisme composé
$$
G \to \tilde{G} \to \tilde{G}/\tilde{G}_0
$$
définit par passage au quotient un isomorphisme de $G/G_0$ sur $\tilde{G}/\tilde{G}_0$.

#### Remarque 2 {#lie-iii-s6-n10-rem-2 .statement}

Supposons $G$ simplement connexe. Soient $g = L(G)$, $g_C$ la complexification de $g$, $S'$ le groupe de Lie complexe simplement connexe d’algèbre de Lie $g_C$, $\sigma$ le morphisme de $G$ dans $S'$ tel que $L(\sigma)$ soit l’injection canonique de $g$ dans $g_C$. Reprenons les notations de la démonstration de la prop. 20, partie *a*). Si $H = S'$ et $\varphi = \sigma$, on a $\varphi^* = \mathrm{Id}_{S'}$. Donc $(S', \sigma)$ est la complexification universelle de $G$. On notera que $\sigma$ n’est pas injectif en général (exerc. 16); toutefois *son noyau est discret* puisque $L(\sigma)$ est injectif. D’autre part, soit $\theta$ l’involution de $g_C$ définie par $g$, et soit $\eta$ l’automorphisme correspondant du groupe de Lie réel sous-jacent à $S'$; soit ${S'}^n$ l’ensemble des points de $S'$ invariants par $\eta$; c’est un sous-groupe de Lie réel de $S'$ d’algèbre de Lie $g$ (\S 3, n° 8, cor. 1 de la prop. 29). D’après le n° 1, cor. 1 de la prop. 1, $\sigma(G)$ est le sous-groupe intégral réel de $S'$ d’algèbre de Lie $g$, donc $\sigma(G)$ *est la composante neutre de* ${S'}^n$; en particulier $\sigma(G)$ est un sous-groupe de Lie réel de $S'$.

## EXERCICES {#lie-iii-s6-exercises}

See the [exercises for § 6](exercises/s6/).
