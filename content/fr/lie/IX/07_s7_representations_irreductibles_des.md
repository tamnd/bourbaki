---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: GROUPES DE LIE RÉELS COMPACTS
section: 7
section_title: Représentations irréductibles des groupes de Lie compacts connexes
lang: fr
source: lie-ix-fr
book_pages: LIE IX.66-LIE IX.78, LIE IX.125-LIE IX.126
pdf_pages: 0069-0081, 0128-0129
extraction: ocr
subsections:
    - "no": 1
      title: Caractères dominants
      page: 66
      pdf_page: 69
    - "no": 2
      title: Le plus grand poids d’une représentation irréductible
      page: 67
      pdf_page: 70
    - "no": 3
      title: L'anneau $R(G)$
      page: 70
      pdf_page: 73
    - "no": 4
      title: La formule des caractères
      page: 72
      pdf_page: 75
    - "no": 5
      title: Degré des représentations irréductibles
      page: 75
      pdf_page: 78
    - "no": 6
      title: Éléments de Casimir
      page: 77
      pdf_page: 80
statements: 27
exercises: 8
content_sha256: 94bec922e39b175a95c2e9bac03d80b3eef4ba42c5399288591e184c2d1b2a9f
---

## § 7. REPRÉSENTATIONS IRRÉDUCTIBLES DES GROUPES DE LIE COMPACTS CONNEXES $^1$

On conserve les notations du § 6. On appelle représentation de G tout homomorphisme continu (donc analytique) de G dans un groupe $\mathbf{GL}(V)$, où V est un espace vectoriel complexe de dimension finie. Toute représentation de G est semi-simple (§ 1, n° 1).

On choisit une chambre C de t (§ 5, n° 2), et on pose $\Gamma(T)_{++} = \overline{C} \cap \Gamma(T)$.

### 1. Caractères dominants

On note $X_+$ l’ensemble des éléments $\lambda$ de $X(T)$ tels que $\langle \lambda, x \rangle \geqslant 0$ pour tout $x \in \Gamma(T)_{++}$, c’est-à-dire tels que la forme linéaire $\delta(\lambda): t_C \to \mathbf{C}$ applique la chambre C de t dans $i\mathbf{R}_+$.

On munit $X(T)$ de la structure de groupe ordonné pour laquelle les éléments positifs sont ceux de $X_+$; on pose $R_+ = R(G, T) \cap X_+$ et $R_- = -R_+$. Les éléments de $R_+$ sont appelés racines positives, ceux de $R_-$ racines négatives; toute racine est, soit positive, soit négative (VI, § 1, n° 6, th. 3). Une racine positive qui n’est pas somme de deux racines positives est dite simple; toute racine positive est somme de racines simples (loc. cit.); les racines simples forment une base du sous-groupe de $X(T)$ engendré par les racines, sous-groupe qui s’identifie à $X(T/C(G))$ (§ 4, n° 4); les réflexions par rapport aux racines simples engendrent le groupe de Weyl $W = W_G(T)$ (VI, § 1, n° 5, th. 2).

#### Lemme 1 {#lie-ix-s7-lem-1 .statement tag=01FZ}

Soit $\lambda$ un élément de $X(T)$. Les conditions suivantes sont équivalentes :
(i) On a $\lambda - w(\lambda) \geqslant 0$ (resp. $> 0$) pour tout $w \in W$ tel que $w \neq 1$;
(ii) pour tout $w \in W$ tel que $w \neq 1$, $\lambda - w(\lambda)$ est combinaison linéaire à coefficients positifs (resp. positifs et non tous nuls) des racines simples;
(iii) on a $\langle \lambda, K_\alpha \rangle \geqslant 0$ (resp. $> 0$) pour toute racine positive $\alpha$;
(iv) on a $\langle \lambda, K_\alpha \rangle \geqslant 0$ (resp. $> 0$) pour toute racine simple $\alpha$.

L’équivalence de (iii) et (iv) est immédiate. Puisque l’ensemble des $K_\alpha$ s’identifie au système de racines inverse de $R(G, T)$ (§ 4, n° 5), l’équivalence de (i) et (iii) résulte de VI, § 1, n° 6, prop. 18 et corollaire. L’implication (ii) $\Rightarrow$ (i) est triviale, et l’implication opposée résulte de loc. cit.

$^1$ Dans ce paragraphe et le suivant, nous référons par le sigle TS à un chapitre à paraître du livre de Théories Spectrales et consacré aux représentations linéaires des groupes compacts.

On note $X_{++}$ l’ensemble des éléments de $X(T)$ tels que $\langle \lambda, K_\alpha \rangle \geqslant 0$ pour toute racine positive $\alpha$. Les éléments de $X_{++}$ sont dits dominants. Ils forment un domaine fondamental pour l’action de $W$ dans $X(T)$ (VI, § 1, n° 10). On a $X_{++} \subset X_+$.

Si $G$ est simplement connexe, il existe pour chaque racine simple $\alpha$ un élément $\varpi_\alpha$ de $X(T)$ tel que $\langle \varpi_\beta, K_\alpha \rangle = \delta_{\alpha \beta}$ pour toute racine simple $\beta$, c’est-à-dire $s_\alpha(\varpi_\alpha) = \varpi_\alpha - \alpha, s_\beta(\varpi_\alpha) = \varpi_\alpha$ pour toute racine simple $\beta \neq \alpha$; les $\varpi_\alpha$ sont appelés les poids dominants fondamentaux ; ils forment une base du groupe commutatif $X(T)$ et du monoïde commutatif $X_{++}$ : plus précisément, tout élément $\lambda$ de $X(T)$ s’écrit sous la forme $\lambda = \sum_\alpha \langle \lambda, K_\alpha \rangle \varpi_\alpha$.

On note $\rho$ l’élément de $X(T) \otimes \mathbf{Q}$ tel que
$$
2 \rho = \sum_{\alpha \in R_+} \sigma .
$$
On a $\langle \rho, K_\alpha \rangle = 1$ pour toute racine simple $\alpha$ (VI, § 1, n° 10, prop. 29). Si $G$ est simplement connexe, $\rho$ est la somme des poids dominants fondamentaux.

### 2. Le plus grand poids d’une représentation irréductible

A toute représentation $\tau : G \to \mathbf{GL}(V)$, associons l’homomorphisme $L(\tau)_\mathbf{C}$ de la $\mathbf{C}$-algèbre de Lie $g_\mathbf{C}$ dans $\mathrm{End}(V)$ prolongeant la représentation linéaire $L(\tau)$ de $g$ dans l’espace vectoriel réel sous-jacent à $V$ (III, § 3, n° 11). D’après la prop. 7 du § 4, n° 3, l’application $\delta$ de $X(T)$ dans $\mathrm{Hom}_\mathbf{C}(t_\mathbf{C}, \mathbf{C}) = t_\mathbf{C}^*$ applique bijectivement l’ensemble des poids de $\tau$ relativement à $T$ sur l’ensemble des poids de $L(\tau)_\mathbf{C}$ relativement à la sous-algèbre de Cartan $t_\mathbf{C}$ de $g_\mathbf{C}$.

#### Lemme 2 {#lie-ix-s7-lem-2 .statement tag=01G0}

Soit $\varphi$ une représentation linéaire de l’algèbre de Lie complexe $g_\mathbf{C}$ dans un espace vectoriel complexe $V$ de dimension finie. Pour qu’il existe une représentation $\tau$ de $G$ dans $V$ telle que $L(\tau)_\mathbf{C} = \varphi$, il faut et il suffit que $\varphi$ soit semi-simple et que les poids de $t_\mathbf{C}$ dans $V$ appartiennent à $\delta(X(T))$.

S’il existe une représentation $\tau$ de $G$ telle que $L(\tau)_\mathbf{C} = \varphi$, alors $\varphi$ est semi-simple car $G$ est connexe et $\tau$ semi-simple (III, § 6, n° 5, cor. 2 à la prop. 13), et les poids de $t_\mathbf{C}$ dans $V$ appartiennent à l’image de $\delta$. La condition est donc nécessaire ; démontrons qu’elle est suffisante. Si $\varphi$ est semi-simple, $V$ est somme directe des $V_\mu(t_\mathbf{C})$, où $\mu$ parcourt l’ensemble des poids de $t_\mathbf{C}$ dans $V$ (VII, § 2, n° 4, cor. 3 au th. 2) ; si tous ces poids appartiennent à l’image de $\delta$, il existe une représentation $\tau_T$ de $T$ dans $V$ telle que $L(\tau_T)_\mathbf{C} = \varphi|_{t_\mathbf{C}}$ : il suffit en effet de poser $\tau_T(t)v = t^\lambda v$ pour $t \in T$ et $v \in V_{\delta(\lambda)}(t_\mathbf{C})$. Le lemme résulte alors de la prop. 8 du § 2, n° 6.

#### Théorème 1 {#lie-ix-s7-thm-1 .statement tag=01G1}

a) Soit $\tau : G \to \mathbf{GL}(V)$ une représentation irréductible de $G$. Alors l’ensemble des poids de $\tau$ (relativement à $T$) possède un plus grand élément $\lambda$, celui-ci est dominant, et l’espace $V_\lambda(T)$ est de dimension 1.

b) Pour que deux représentations irréductibles de $G$ soient équivalentes, il faut et il suffit que leurs plus grands poids soient égaux.

c) Pour tout élément dominant $\lambda$ de $X(T)$, il existe une représentation irréductible de $G$ de plus grand poids $\lambda$.

D’après le lemme 2, les classes d’équivalence de représentations irréductibles de $G$ correspondent bijectivement aux classes de représentations irréductibles de dimension finie de $g$ dont les poids appartiennent à $\delta(X(T))$.

Notons $\mathcal{C}g_c$ le centre et $\mathcal{D}g_c$ l’algèbre de Lie dérivée de $g_c$, de sorte que $g_c = \mathcal{C}g_c \oplus \mathcal{D}g_c$. Pour toute forme linéaire $\mu$ sur $t_c \cap \mathcal{D}g_c$, notons $E(\mu)$ le $\mathcal{D}g_c$-module simple introduit en VIII, § 6, n° 3 ; pour toute forme linéaire $v$ sur $\mathcal{C}g_c$, notons $C(v)$ le $\mathcal{C}g_c$-module de dimension 1 sur $\mathbf{C}$ associé. Alors les $g_c$-modules $C(v) \otimes E(\mu)$ sont simples, et d’après VIII, § 7, n° 2, cor. 2 au th. 1 et A, VIII, § 11, n° 1, th. 1, tout $g_c$-module simple de dimension finie est isomorphe à un $g_c$-module $C(v) \otimes E(\mu)$; de plus (*loc. cit.*) $C(v) \otimes E(\mu)$ est de dimension finie si et seulement si $\mu(H_\alpha)$ est entier positif pour toute racine simple $\alpha$. Si l’on note $v + \mu$ la forme linéaire sur $t_c$ qui induit $v$ sur $\mathcal{C}g_c$ et $\mu$ sur $t_c \cap \mathcal{D}g_c$, on a $(v + \mu)(H_\alpha) = \mu(H_\alpha)$; de plus, les poids de $C(v) \otimes E(\mu)$ sont les $v + \lambda$, où $\lambda$ parcourt les poids de $E(\mu)$, donc sont de la forme $v + \mu - \theta$, avec $\theta \in \delta(X_+)$ (VIII, § 6, n° 2, lemme 2).

On en conclut que le $g$-module $C(v) \otimes E(\mu)$ est de dimension finie si et seulement si $(v + \mu)(H_\alpha)$ est entier positif pour toute racine simple $\alpha$, et que ses poids appartiennent à $\delta(X(T))$ si et seulement si $v + \mu$ appartient à $\delta(X(T))$. La conjonction de ces deux conditions signifie que $v + \mu$ appartient à $\delta(X_{++})$; dans ce cas, $v + \mu$ est le plus grand poids de $C(v) \otimes E(\mu)$. On a donc construit pour tout élément dominant $\lambda$ de $X(T)$ une représentation irréductible de $G$ dont $\lambda$ est le plus grand poids, et obtenu ainsi, à équivalence près, toutes les représentations irréductibles de $G$. Comme les vecteurs de poids $v + \mu$ dans $C(v) \otimes E(\mu)$ forment un sous-espace de dimension 1, on a ainsi achevé la démonstration.

#### Corollaire {#lie-ix-s7-n2-cor-1 .statement tag=01G2}

*Le groupe* $G$ *possède une représentation linéaire fidèle (de dimension finie)*.

Observons d’abord que tout élément de $X(T)$ est égal à la différence de deux éléments dominants : plus précisément, soit $\varpi$ un élément de $X_{++}$ tel que $\langle \varpi, K_\alpha \rangle > 0$ pour toute racine simple $\alpha$; pour tout $\lambda \in X(T)$, il existe un entier positif $n$ tel qu’on ait $\langle \lambda + n \varpi, K_\alpha \rangle \geqslant 0$ pour toute racine simple $\alpha$, c’est-à-dire (n° 1, lemme 1) $\lambda + n \varpi \in X_{++}$.

Par conséquent, il existe une famille finie $(\lambda_i)_{i \in I}$ d’éléments de $X_{++}$ engendrant le $\mathbf{Z}$-module $X(T)$. Pour $i \in I$, soit $\tau_i$ une représentation irréductible de $G$ de plus grand poids $\lambda_i$ (th. 1); soit $\tau$ la représentation somme directe des $\tau_i$. Par construction l’ensemble $P(\tau, T)$ des poids de $\tau$ (relativement à $T$) engendre le $\mathbf{Z}$-module $X(T)$. Il résulte alors de la prop. 6 du § 4, n° 3, que l’homomorphisme $\tau$ est injectif, d’où le corollaire.

#### Remarque 1 {#lie-ix-s7-n2-rem-1 .statement tag=01G3}

Soit $n_+$ la sous-algèbre de $g_c$ somme des $g^\alpha$ pour $\alpha > 0$. Soient $\tau : G \to \mathbf{GL}(V)$ une représentation irréductible, $\lambda \in X_{++}$ son plus grand poids et $\tau' : g_c \to \mathbf{gl}(V)$ la représentation déduite de $\tau$. Alors $V_\lambda(T)$ est le sous-espace formé des vecteurs $v$ de $V$ tels que $\tau'(x) v = 0$ pour tout $x \in n_+$.

Cela résulte en effet de l’énoncé correspondant pour les $g_c$-modules $C(v) \otimes E(\mu)$ (VIII, § 6, n° 2, prop. 3).

#### Remarque 2 {#lie-ix-s7-n2-rem-2 .statement tag=01G4}

Soit $\Theta(G)$ l’algèbre des fonctions représentatives continues de $G$ à valeurs dans $\mathbf{C}$ (A, VIII). On fait opérer $G$ sur $\Theta(G)$ par translations à droite et à gauche. Pour chaque $\lambda \in X_{++}$, soit $(V_\lambda, \tau_\lambda)$ une représentation irréductible de $G$ de plus grand poids $\lambda$ (th. 1), et $(V_\lambda^*, \check{\tau}_\lambda)$ la représentation contragrédiente (III, § 3, n° 11); alors d’après TS, la représentation de $G \times G$ dans $\Theta(G)$ est isomorphe à la somme directe, pour $\lambda$ parcourant $X_{++}$, des représentations $(V_\lambda \otimes V_\lambda^*, \tau_\lambda \otimes \check{\tau}_\lambda)$. On déduit alors de la remarque 1 l’énoncé suivant : *Soit $\lambda \in X_{++}$, et soit $E_\lambda$ le sous-espace vectoriel de $\Theta(G)$ formé des fonctions représentatives continues $f$ sur $G$ telles que $f(gt) = \lambda(t)^{-1}f(g)$ pour tout $g \in G$ et tout $t \in T$, et que $f*x = 0$ pour tout $x \in n_- = \bigoplus_{\alpha < 0} g^\alpha$. Alors $E_\lambda$ est stable par les translations à gauche, et la représentation de $G$ dans $E_\lambda$ par translations à gauche est irréductible, de plus grand poids $\lambda$*.

#### Remarque 3 {#lie-ix-s7-n2-rem-3 .statement tag=01G5}

Soit $\tau : G \to \mathbf{GL}(V)$ une représentation irréductible. Il existe un élément $v$ de $X(C(G))$ tel que $\tau(s)v = v(s)v$ pour $s \in C(G)$, $v \in V$ : en effet $\tau(C(G))$ est contenu dans le commutant de $\tau(G)$, qui est égal à $C^*$. $1_V$ (A, VIII, § 3, n° 2, th. 1). Pour tout poids $\lambda$ de $\tau$, la restriction de $\lambda$ à $C(G)$ est égale à $v$.

#### Remarque 4 {#lie-ix-s7-n2-rem-4 .statement tag=01G6}

On généralise sans peine à la situation actuelle les définitions et énoncés de VIII, § 7, n°s 2 à 5 ; nous en laissons les détails au lecteur.

#### Proposition 1 {#lie-ix-s7-prop-1 .statement tag=01G7}

*Soit $\tau : G \to \mathbf{GL}(V)$ une représentation irréductible de $G$, de plus grand poids $\lambda \in X_{++}$. Soit $m$ l’entier $\sum_{\alpha \in \mathbf{R}_+} \langle \lambda, K_\alpha \rangle$, et soit $w_0$ l’élément du groupe de Weyl tel que $w_0(R_+) = R_-$ (VI, § 1, n° 6, cor. 3 de la prop. 17). On est alors dans l’un des trois cas suivants :

a) $w_0(\lambda) = -\lambda$ et $m$ est pair. Il existe alors une forme bilinéaire symétrique séparante sur $V$, invariante par $G$ ; la représentation $\tau$ est de type réel (Appendice II).

b) $w_0(\lambda) \neq -\lambda$. Toute forme bilinéaire sur $V$ invariante par $G$ est nulle ; la représentation $\tau$ est de type complexe (loc. cit.).

c) $w_0(\lambda) = -\lambda$ et $m$ est impair. Il existe une forme bilinéaire alternée séparante sur $V$ invariante par $G$ ; la représentation $\tau$ est de type quaternionien (loc. cit.).

Si la restriction de $\tau$ à $C(G)_0$ n’est pas triviale, on est alors dans le cas b).

Une forme bilinéaire $B$ sur $V$ est invariante par $G$ si et seulement si elle est invariante par $g_c$ (III, § 6, n° 5, cor. 3). Si $G$ est semi-simple, la proposition résulte donc de VIII, § 7, n° 5, prop. 12 et de la prop. 3 de l’Appendice II.

Dans le cas général, posons $C(G)_0 = S$, et identifions $X(T/S)$ à un sous-groupe de $X(T)$ (stable par $W$). Si $\tau(S) = \{ 1_V \}$, $\tau$ induit par passage au quotient une représentation $\tau' : G/S \to \mathbf{GL}(V)$, de plus grand poids $\lambda$ ; la proposition résulte dans ce cas de ce qui précède, appliqué à $G/S$.

Supposons $\tau(S) \neq \{ 1_V \}$. Il existe un élément non nul $v$ de $X(S)$ tel que $\tau(s) = v(s)_V$ pour tout $s \in S$ (remarque 3). Alors $v$ est l’image de $\lambda$ par l’homomorphisme de restriction $X(T) \to X(S)$ ; puisque $W$ opère trivialement sur $X(S)$, l’égalité $w_0(\lambda) = -\lambda$ entraînerait $v = -v$, ce qui est impossible : on a donc $w_0(\lambda) \neq -\lambda$.

D'autre part, si B est une forme bilinéaire sur V, invariante par G, on a, pour x, y dans V et s dans S,

$$
B(v(s)\ x,\ v(s)\ y) = B(x,\ y) = v(s)^2 B(x,\ y)
$$

ce qui entraîne $B = 0$, d'où la proposition.

Soit $\mathcal{S}_\mathbf{R}(G)$ l'ensemble des classes de représentations continues irréductibles de G dans des espaces vectoriels réels de dimension finie. La prop. 1 et les résultats de l'Appendice II établissent une bijection $\Phi : X_{++}/\Sigma \to \mathcal{S}_\mathbf{R}(G)$, où $\Sigma$ désigne le sous-groupe $\{1,\ -w_0\}$ de Aut(X(T)). Plus précisément, soit $\lambda \in X_{++}$, et soit $E_\lambda$ une représentation de G de plus grand poids $\lambda$; on a

$$
\Phi(\{\lambda,\ -w_0(\lambda)\}) = E_{\lambda[\mathbf{R}]} \quad \text{si} \quad \lambda \neq -w_0(\lambda) \quad \text{ou si} \quad \sum_{\alpha \in R^+} \langle \lambda, K_\alpha \rangle \notin 2\mathbf{Z},
$$

$$
\Phi(\{\lambda,\ -w_0(\lambda)\}) = E'_\lambda \quad \text{si} \quad \lambda = -w_0(\lambda) \quad \text{et} \quad \sum_{\alpha \in R^+} \langle \lambda, K_\alpha \rangle \in 2\mathbf{Z},
$$

où $E'_\lambda$ est une $\mathbf{R}$-structure sur $E_\lambda$ invariante par G.

### 3. L'anneau $R(G)$

Soit $R(G)$ l'anneau des représentations (continues dans des espaces vectoriels complexes de dimension finie) de G (A, VIII, § 10, n° 6). Si $\tau$ est une représentation de G, on note $[\tau]$ sa classe dans $R(G)$; si $\tau$ et $\tau'$ sont deux représentations de G, on a donc par définition

$$
[\tau] + [\tau'] = [\tau \oplus \tau']
$$
$$
[\tau][\tau'] = [\tau \otimes \tau'].
$$

Puisque toute représentation de G est semi-simple, le $\mathbf{Z}$-module $R(G)$ est libre et admet comme base l'ensemble des classes de représentations irréductibles de G, ensemble qui s'identifie à $X_{++}$ par le th. 1. L'application $\tau \mapsto L(\tau)_{(c)}$ induit un homomorphisme d'anneaux $l$ de $R(G)$ dans l'anneau $\mathcal{R}(g_c)$ des représentations de $g_c$ (VIII, § 7, n° 6).

Soit $\tau : G \to \mathbf{GL}(V)$ une représentation de G; considérons la graduation $(V_\lambda(T))_{\lambda \in X(T)}$ du C-espace vectoriel V. On note Ch(V), ou Ch(\tau), le caractère de l'espace vectoriel gradué V (VIII, § 7, n° 7); si l'on désigne par $(e^\lambda)_{\lambda \in X(T)}$ la base canonique de l'algèbre $\mathbf{Z}[X(T)] = \mathbf{Z}^{(X(T))}$, on a par définition

$$
\mathrm{Ch}(\tau) = \sum_{\lambda \in X(T)} (\dim V_\lambda(T))\ e^\lambda.
$$

On définit ainsi (loc. cit.) un homomorphisme d’anneaux, encore noté Ch, de R(G) dans $\mathbf{Z}[X(T)]$. Si G est semi-simple, on a un diagramme commutatif

$$
\begin{array}{ccc}
R(G) & \xrightarrow{\mathrm{Ch}} & \mathbf{Z}[X(T)] \\
\downarrow l & & \downarrow \tilde{\delta} \\
\mathcal{R}(g_c) & \xrightarrow{\mathrm{ch}} & \mathbf{Z}[\bar{P}]
\end{array}
$$

où P désigne le groupe des poids de $R(g_c, t_c)$, et $\tilde{\delta}$ l’homomorphisme déduit de $\delta$.

Le groupe de Weyl W opère par automorphismes dans le groupe X(T), donc dans l’anneau $\mathbf{Z}[X(T)]$. D’après la prop. 5 du § 4, no 3, l’image de Ch est contenue dans le sous-anneau $\mathbf{Z}[X(T)]^W$ formé des éléments invariants par W.

#### Proposition 2 {#lie-ix-s7-prop-2 .statement tag=01G8}

*L’homomorphisme Ch induit un isomorphisme de R(G) sur $\mathbf{Z}[X(T)]^W$*.

Pour $\lambda \in X_{++}$, notons $[ \lambda ]$ la classe dans R(G) de la représentation irréductible de plus grand poids $\lambda$. Puisque la famille $( [ \lambda ] )_{\lambda \in X_{++}}$ est une base du $\mathbf{Z}$-module R(G), il s’agit de démontrer l’assertion suivante :

*La famille $( \mathrm{Ch}[\lambda] )_{\lambda \in X_{++}}$ est une base du $\mathbf{Z}$-module $\mathbf{Z}[X(T)]^W$.*

Pour tout élément $u = \sum_{\lambda} a_{\lambda} e^{\lambda}$ de $\mathbf{Z}[X(T)]$, appelons termes maximaux de $u$ les $a_{\lambda} e^{\lambda}$ tels que $\lambda$ soit un élément maximal de l’ensemble des $\mu \in X(T)$ avec $a_{\mu} \neq 0$. Le th. 1 implique que $\mathrm{Ch}[\lambda]$ possède un unique terme maximal, à savoir $e^{\lambda}$. La proposition résulte donc du lemme suivant.

#### Lemme 3 {#lie-ix-s7-lem-3 .statement tag=01G9}

*Pour chaque $\lambda \in X_{++}$, soit $C_{\lambda}$ un élément de $\mathbf{Z}[X(T)]^W$ ayant pour unique terme maximal $e^{\lambda}$. Alors la famille $( C_{\lambda} )_{\lambda \in X_{++}}$ est une base de $\mathbf{Z}[X(T)]^W$.*

La démonstration est identique à celle de la prop. 3 de VI, § 3, no 4, en y remplaçant A par $\mathbf{Z}$, P par X(T) et $P \cap \overline{C}$ par $X_{++}$.

Soit $\Theta(G)$ (resp. $\Theta(T)$) la C-algèbre des fonctions représentatives continues sur G (resp. T), et soit $Z\Theta(G)$ (resp. $\Theta(T)^W$) la sous-algèbre formée de celles de ces fonctions qui sont centrales (resp. invariantes par W). L’application de restriction $\Theta(G) \to \Theta(T)$ induit un homomorphisme d’anneaux $r : Z\Theta(G) \to \Theta(T)^W$. D’autre part, l’application qui à une représentation $\tau$ associe son caractère (c’est-à-dire la fonction $g \mapsto \mathrm{Tr}\, \tau(g)$) se prolonge en un homomorphisme de C-algèbres $\mathrm{Tr} : C \otimes_{\mathbf{Z}} R(G) \to Z\Theta(G)$, qui, d’après TS, est un *isomorphisme*. De même, on déduit de l’injection canonique $X(T) \to \Theta(T)$ un isomorphisme de C-algèbres $\iota : C[X(T)] \to \Theta(T)$, qui induit un isomorphisme $\iota : C[X(T)]^W \to \Theta(T)^W$. Le diagramme

$$
\begin{array}{ccc}
C \otimes_{\mathbf{Z}} R(G) & \xrightarrow{1 \otimes \mathrm{Ch}} & C[X(T)]^W \\
\downarrow \mathrm{Tr} & & \downarrow 1 \\
Z\Theta(G) & \xrightarrow{r} & \Theta(T)^W
\end{array}
$$

est commutatif : en effet pour toute représentation $\tau : G \to GL(V)$ et tout $t \in T$ on a
$$
\operatorname{Tr} \tau(t) = \sum_{\lambda \in X(T)} (\dim V_\lambda(T)) \lambda(t) = \iota(\operatorname{Ch} \tau)(t)
$$
c'est-à-dire $(r \circ \operatorname{Tr})[\tau] = (\iota \circ \operatorname{Ch})[\tau]$.
On déduit alors de la proposition le résultat suivant.

#### Corollaire {#lie-ix-s7-n3-cor-1 .statement tag=01GA}

*L’application de restriction* $r : Z\Theta(G) \to \Theta(T)^W$ est bijective.

### 4. La formule des caractères

Dans ce numéro, on note le groupe $X(T)$ multiplicativement, et on considère ses éléments comme des fonctions sur $T$ à valeurs complexes. *On suppose que l’élément $\rho$ de $X(T) \otimes \mathbf{Q}$ appartient à $X(T)$*.

On désigne par $L^2(T)$ l’espace hilbertien des classes de fonctions complexes de carré intégrable sur $T$, et par $\Theta(T)$ le sous-espace formé des fonctions représentatives continues. D’après TS, $X(T)$ est une base orthonormale de $L^2(T)$ et une base algébrique de $\Theta(T)$.

Pour $f \in L^2(T)$ et $w \in W$, on note $^w f$ l’élément de $L^2(T)$ défini par $^w f(t) = f(w^{-1}(t))$; pour $\lambda \in X(T)$, on a donc $^w \lambda = w(\lambda)$. On note $\varepsilon : W \to \{1, -1\}$ la signature (unique homomorphisme tel que $\varepsilon(s) = -1$ pour toute réflexion $s$); pour $f \in L^2(T)$, on pose
$$
J(f) = \sum_{w \in W} \varepsilon(w) \ ^w f .
$$
Si $\lambda \in X_{++}$, les caractères $^w(\lambda \rho)$ sont tous distincts ; il suffit en effet de prouver qu’on a $^w(\lambda \rho) \neq \lambda \rho$ pour tout $w \neq 1$; or cela résulte du lemme 1 (n° 1) et de ce qu’on a $\langle \lambda \rho, K_\alpha \rangle = \langle \lambda, K_\alpha \rangle + 1 > 0$ pour toute racine positive $\alpha$. Par conséquent :
$$
\| J(\lambda \rho) \| ^2 = \operatorname{Card}(W) = w(G) .
$$

On dit qu’un élément $f \in L^2(T)$ est *anti-invariant si* $^w f = \varepsilon(w) f$ pour tout $w \in W$ (c’est-à-dire si $^s f = -f$ pour toute réflexion $s$). Montrons que $\frac{1}{w(G)} J$ est le *projecteur orthogonal* de $L^2(T)$ sur le sous-espace des éléments anti-invariants. En effet, soient $f, f'$ dans $L^2(T)$, avec $f'$ anti-invariant ; alors $J(f)$ est anti-invariant et l’on a
$$
\langle f', J(f) \rangle = \sum_{w \in W} \varepsilon(w) \langle f', ^w f \rangle = \sum_{w \in W} \langle ^w f', ^w f \rangle
= \sum_{w \in W} \langle f', f' \rangle = w(G) \langle f', f \rangle .
$$

#### Proposition 3 {#lie-ix-s7-prop-3 .statement tag=01GB}

*Les éléments* $J(\lambda \rho)/\sqrt{w(G)}$, *pour* $\lambda \in X_{++}$, *forment une base orthonormale du sous-espace des éléments anti-invariants de* $L^2(T)$, *et une base algébrique du sous-espace des éléments anti-invariants de* $\Theta(T)$.

La démonstration est identique à celle de VI, § 3, n° 3, prop. 1.

D'après VI, *loc. cit.*, prop. 2, on a

$$
J(\rho) = \rho \prod_{\alpha > 0} (1 - \alpha^{-1}) = \rho^{-1} \prod_{\alpha > 0} (\alpha - 1),
$$

donc

$$
J(\rho) \overline{J(\rho)} = \prod_{\alpha} (\alpha - 1).
$$

D'après le cor. 2 au th. 1 (§ 6, n° 2), on en déduit :

#### Lemme 4 {#lie-ix-s7-lem-4 .statement tag=01GC}

*Si $\varphi$ et $\psi$ sont deux fonctions continues centrales sur $G$, on a*

$$
\int_G \overline{\varphi(g)} \psi(g) dg = \frac{1}{w(G)} \int_T (\overline{\varphi(t) J(\rho)(t)}) \cdot (\psi(t) J(\rho)(t)) dt.
$$

Pour tout $\lambda \in X_{++}$, notons $\chi_\lambda$ le caractère d'une représentation irréductible de $G$ de plus grand poids $\lambda$.

**Théorème 2 (H. Weyl).** — *Pour tout $\lambda \in X_{++}$, on a $J(\rho) \cdot \chi_\lambda|T = J(\lambda \rho)$.*

La fonction $J(\rho) \cdot \chi_\lambda|T$ est anti-invariante par $W$, et est combinaison linéaire à coefficients entiers des éléments de $X(T)$. D'après VI, § 3, n° 3, prop. 1, elle s'écrit donc $\sum_\mu a_\mu J(\mu \rho)$, où $\mu$ parcourt $X_{++}$, et où les $a_\mu$ sont entiers et tous nuls sauf un nombre fini d'entre eux ; puisque $\int_G |\chi_\lambda(g)|^2 dg = 1$ (TS), il résulte de la prop. 3 et du lemme 4 que l'on a $\sum_\mu (a_\mu)^2 = 1$; les $a_\mu$ sont donc tous nuls, sauf l'un d'entre eux qui vaut 1 ou -1. Mais le coefficient de $\lambda$ dans $\chi_\lambda|T$ vaut 1 (th. 1), donc le coefficient de $\lambda \rho$ dans $J(\rho) \cdot \chi_\lambda|T$ vaut 1 (VI, § 3, n° 3, remarque 2), ce qui implique $a_{\lambda \rho} = 1$, d'où le théorème.

#### Corollaire 1 {#lie-ix-s7-lem-4-cor-1 .statement}

*Avec les notations du n° 3, on a dans $\mathbf{Z}[X(T)]$*

$$
\left( \sum_{w \in W} \varepsilon(w) e^{w \rho} \right) \mathrm{Ch}[\lambda] = \sum_{w \in W} \varepsilon(w) e^{w \lambda} e^{w \rho} \quad \text{pour tout } \lambda \in X_{++}.
$$

Cela résulte du théorème et de la commutativité du diagramme (2) (n° 3).

#### Corollaire 2 {#lie-ix-s7-lem-4-cor-2 .statement}

*Pour tout $\lambda \in X_{++}$ et tout élément régulier $t$ de $T$, on a*

$$
\chi_\lambda(t) = \frac{\sum_w \varepsilon(w) \lambda(wt) \rho(wt)}{\sum_w \varepsilon(w) \rho(wt)}
$$

*où les deux sommations sont étendues aux éléments $w$ de $W$.*

En effet, $J(\rho)(t)$ n'est pas nul, puisque $t$ est régulier (formule (4)).

Si $\varphi$ est une fonction centrale sur $G$, la restriction de $\varphi$ à $T$ est invariante par $W$, donc $J(\rho) \cdot \varphi|T$ est anti-invariante par $W$. Par ailleurs, d'après TS et le th. 1, la famille $(\chi_\lambda)_{\lambda \in X^+}$ est une base algébrique de l’espace des fonctions représentatives centrales sur G et une base orthonormale de l’espace $\mathrm{ZL}^2(G)$ des classes de fonctions centrales de carré intégrable sur G.

On déduit donc de la prop. 3 et du th. 2 :

#### Corollaire 3 {#lie-ix-s7-lem-4-cor-3 .statement}

*L’application qui, à chaque fonction continue centrale $\varphi$ sur G, associe la fonction $w(G)^{-1/2}J(\rho)\ (\varphi|T)$ induit un isomorphisme de l’espace des fonctions représentatives centrales sur G sur l’espace des éléments anti-invariants de $\Theta(T)$ ; elle se prolonge par continuité en un isomorphisme d’espaces hilbertiens de $\mathrm{ZL}^2(G)$ sur le sous-espace des éléments anti-invariants de $L^2(T)$.*

#### Corollaire 4 {#lie-ix-s7-lem-4-cor-4 .statement}

*Soit $\varphi$ une fonction continue centrale sur G. On a*

$$
\int_G \overline{\chi_\lambda(g)}\ \varphi(g)\ dg = \int_T \overline{\lambda(t)} \prod_{\alpha > 0} (1 - \alpha(t)^{-1})\ \varphi(t)\ dt = \int_T \overline{\lambda\rho(t)}.\varphi(t)\ J(\rho)\ (t)\ dt .
$$

En effet, d’après le lemme 4 et le th. 2, on a

$$
\int_G \overline{\chi_\lambda(g)}\ \varphi(g)\ dg = \frac{1}{w(G)} \int_T \overline{\chi_\lambda(t)\ J(\rho)\ (t)}\ (\varphi(t)\ J(\rho)\ (t))\ dt
$$
$$
= \frac{1}{w(G)} \int_T \overline{J(\lambda\rho)\ (t)}\ \varphi(t)\ J(\rho)\ (t)\ dt .
$$

Mais la fonction $t \mapsto \varphi(t)\ J(\rho)\ (t)$ est anti-invariante et $\frac{1}{w(G)}\ J(\lambda\rho)$ est la projection orthogonale de $\lambda\rho$ sur le sous-espace des éléments anti-invariants de $L^2(T)$, donc

$$
\frac{1}{w(G)} \int_T \overline{J(\lambda\rho)\ (t)}\ \varphi(t)\ J(\rho)\ (t)\ dt = \int_T \overline{\lambda\rho(t)}\ \varphi(t)\ J(\rho)\ (t)\ dt ;
$$

enfin, d’après la formule (3), on a $\overline{\rho(t)}\ J(\rho)\ (t) = \prod_{\alpha > 0} (1 - \alpha(t)^{-1})$, d’où le corollaire.

#### Remarque 1 {#lie-ix-s7-n4-rem-1 .statement tag=01GI}

Pour tout $w \in W$, posons $\rho_w = {}^w\rho/\rho$ ; on a

(6)
$$
\sum_w \varepsilon(w)\ \rho_w = \prod_{\alpha > 0} (1 - \alpha^{-1}) = \rho^{-2} \prod_{\alpha > 0} (\alpha - 1) .
$$

Si $t$ est un élément régulier de T, on tire de (5)

(7)
$$
\chi_\lambda(t) = \frac{\sum_w \varepsilon(w)\ {}^w\lambda(t)\ \rho_w(t)}{\sum_w \varepsilon(w)\ \rho_w(t)} = \frac{\sum_w \varepsilon(w)\ {}^w\lambda(t)\ \rho_w(t)}{\prod_{\alpha > 0} (1 - \alpha(t)^{-1})} .
$$

Notons que $\rho_w$ est combinaison linéaire à coefficients entiers de racines, donc appartient à $X(T)$ même si l’on ne suppose pas $\rho \in X(T)$. Il en résulte que la formule (7) est valable sans l’hypothèse $\rho \in X(T)$ : on peut en effet pour la démontrer remplacer $G$ par un revêtement connexe convenable, et on est ramené au cor. 2.

#### Remarque 2 {#lie-ix-s7-n4-rem-2 .statement tag=01GJ}

De même, la première égalité du cor. 4 reste valable sans l’hypothèse $\rho \in X(T)$.

#### Remarque 3 {#lie-ix-s7-n4-rem-3 .statement tag=01GK}

On peut déduire le th. 2 de l’énoncé infinitésimal analogue (VIII, § 9, n° 1, th. 1) ; c’est le cas également pour le th. 3 du numéro suivant (qui est l’analogue du th. 2 de loc. cit., n° 2).

### 5. Degré des représentations irréductibles

On revient à la notation additive pour le groupe $X(T)$ et on ne suppose plus que $\rho$ appartienne à $X(T)$.

#### Théorème 3 {#lie-ix-s7-thm-3 .statement tag=01GL}

La dimension de l’espace d’une représentation irréductible de $G$ de plus grand poids $\lambda$ est donnée par

$$
\chi_\lambda(e) = \prod_{\alpha \in R_+} \frac{\langle \lambda + \rho, K_\alpha \rangle}{\langle \rho, K_\alpha \rangle}.
$$

Posons $\gamma = \frac{1}{2} \sum_{\alpha > 0} K_\alpha$, d’où $\delta(\alpha)(\gamma) = 2\pi i$ pour toute racine simple $\alpha$ (VI, § 1, n° 10, prop. 29). La droite $R\gamma$ n’est contenue dans aucun des hyperplans $\mathrm{Ker}\ \delta(\alpha)$, donc $\exp(z\gamma)$ est un élément régulier de $G$ pour tout $z \in \mathbf{R}^*$ assez petit ; pour tout $\mu \in X(T)$ et tout $z \in \mathbf{R}$, on a

$$
J(\mu)(\exp(z\gamma)) = \sum_{w \in W} \varepsilon(w)\ e^{z\delta(\mu)(w^{-1}\gamma)}.
$$

Admettons provisoirement le lemme suivant :

#### Lemme 5 {#lie-ix-s7-lem-5 .statement tag=01GM}

On a

$$
J(\mu)(\exp(z\gamma)) = e^{z\delta(\mu)(\gamma)} \prod_{\alpha > 0} (1 - e^{-z\delta(\mu)(K_\alpha)}).
$$

La fonction $J(\mu)(\exp(z\gamma))$ est donc le produit d’une fonction qui tend vers 1 lorsque $z$ tend vers 0 et de

$$
z^N \prod_{\alpha > 0} \delta(\mu)(K_\alpha) = (2\pi iz)^N \prod_{\alpha > 0} \langle \mu, K_\alpha \rangle
$$

où $N = \mathrm{Card}\ R_+$.

Supposons d’abord $\rho \in X(T)$ ; appliquant alors le cor. 2 au th. 2, on voit que, lorsque $z$ tend vers 0, $\chi_\lambda(z\gamma)$ tend vers

$$
\prod_{\alpha > 0} \langle \lambda + \rho, K_\alpha \rangle / \prod_{\alpha > 0} \langle \rho, K_\alpha \rangle,
$$

d’où le théorème en ce cas.

Dans le cas général, il suffit de remarquer qu’on peut toujours, pour démontrer le th. 3, remplacer G par un revêtement connexe convenable, et se réduire ainsi au cas précédent.

Démontrons maintenant le lemme 5. Soit $z \in \mathbf{C}$; notons $\varphi_z$ l’application de t dans la C-algèbre App(X(T), C) des applications de X(T) dans C, qui à $H \in t$ associe l’application

$$
\varphi_z(H): \mu \mapsto \mu(\exp zH) = e^{z \delta(\mu)(H)}.
$$

On a $\varphi_z(H + H') = \varphi_z(H) \varphi_z(H')$, de sorte qu’il existe un homomorphisme d’anneaux

$$
\psi_z : \mathbf{Z}[t] \to \mathrm{App}(X(T), \mathbf{C})
$$

tel que $\psi_z(e^H)(\mu) = e^{z \delta(\mu)(H)}$. D’autre part, d’après VI, § 3, n° 3, prop. 2, on a dans $\mathbf{Z}[t]$ la relation

$$
\sum_{w \in W} \varepsilon(w) e^{w \gamma} = e^\gamma \prod_{\alpha > 0} (1 - e^{-K_\alpha}).
$$

Appliquant l’homomorphisme $\psi_z$, en tenant compte de l’égalité

$$
\psi_z(e^{w \gamma})(\mu) = e^{z \delta(\mu)(w \gamma)} = e^{z \delta(w^{-1} \mu)(\gamma)},
$$

on en déduit la formule annoncée.

#### Corollaire 1 {#lie-ix-s7-lem-5-cor-1 .statement tag=01GN}

*Soit $\| \cdot \|$ une norme sur $X(T) \otimes \mathbf{R}$. Pour tout $\lambda \in X_{++}$, soit $d(\lambda)$ la dimension de l’espace d’une représentation irréductible de $G$ de plus grand poids $\lambda$.

a) *On a $\sup_{\lambda \in X_{++}} d(\lambda)/\| \lambda + \rho \|^\mathbf{N} < \infty$, où $\mathbf{N} = 1/2 (\dim G - \dim T)$.

b) *Si $G$ est semi-simple, on a $\inf_{\lambda \in X_{++}} d(\lambda)/\| \lambda + \rho \| > 0$.

a) Pour tout $\alpha \in \mathbf{R}_+$, il existe $A_\alpha > 0$ avec $|\langle \lambda + \rho, K_\alpha \rangle| \leq A_\alpha \| \lambda + \rho \|$, d’où $d(\lambda)/\| \lambda + \rho \|^\mathbf{N} \leq \prod_{\alpha > 0} A_\alpha / \langle \rho, K_\alpha \rangle$.

b) Supposons $G$ semi-simple, notons $\beta_1, ..., \beta_r$ les racines simples et posons $N_i = K_{\beta_i}$. On a

$$
d(\lambda) \geq \prod_{i=1}^r \frac{\langle \lambda + \rho, N_i \rangle}{\langle \rho, N_i \rangle} = \prod_{i=1}^r \langle \lambda + \rho, N_i \rangle;
$$

comme $\langle \lambda + \rho, N_i \rangle \geq \langle \rho, N_i \rangle = 1$, cela implique

$$
d(\lambda) \geq \sup_i | \langle \lambda + \rho, N_i \rangle | .
$$

Si $G$ est semi-simple, $x \mapsto \sup | \langle x, N_i \rangle |$ est une norme sur $X(T) \otimes \mathbf{R}$, nécessairement équivalente à la norme donnée, d’où b).

#### Corollaire 2 {#lie-ix-s7-lem-5-cor-2 .statement tag=01GO}

Supposons G semi-simple ; soit d un entier. L’ensemble des classes de représentations de G de dimension $\leq d$ est fini.

Le cor. 1, b) entraîne que l’ensemble $X_d$ des éléments $\lambda$ de $X_{++}$ tels que $d(\lambda) \leq d$ est fini. Pour tout $\lambda$ dans $X_d$, soit $V_\lambda$ une représentation irréductible de plus grand poids $\lambda$; toute représentation de dimension $\leq d$ est isomorphe à une somme directe $\bigoplus_{\lambda \in X_d} V_\lambda^{n_\lambda}$, avec $n_\lambda \leq d$, d’où le corollaire.

### 6. Éléments de Casimir

D’après la prop. 3 du § 1, no 3, il existe sur g des formes bilinéaires symétriques négatives, séparantes et invariantes par Ad(G) (si G est semi-simple, on peut par exemple prendre la forme de Killing de g). Soit F une telle forme. Rappelons (I, § 3, no 7) qu’on appelle élément de Casimir associé à F l’élément $\Gamma$ du centre de l’algèbre enveloppante $U(g)$ tel que pour toute base $(e_i)$ de g satisfaisant à $F(e_i, e_j) = - \delta_{ij}$, on ait $\Gamma = - \sum e_i^2$.

On appellera dans la suite de ce chapitre éléments de Casimir de G les éléments de $U(g)$ obtenus ainsi à partir des formes bilinéaires symétriques invariantes séparantes et négatives sur g. Si $\Gamma$ est un élément de Casimir de G et $\tau : G \to GL(V)$ une représentation irréductible de G, alors l’endomorphisme $\Gamma_V$ de V est une homothétie (A, VIII, § 3, no 2, th. 1), dont nous noterons $\tilde{\Gamma}(\tau)$ le rapport.

#### Proposition 4 {#lie-ix-s7-prop-4 .statement tag=01GP}

Soit $\Gamma$ un élément de Casimir de G.

a) Si $\tau$ est une représentation irréductible de G, $\tilde{\Gamma}(\tau)$ est réel et positif. Si $\tau$ n’est pas la représentation unité, on a même $\tilde{\Gamma}(\tau) > 0$.

b) Il existe une forme quadratique $Q_\Gamma$ sur $X(T) \otimes \mathbf{R}$, et une seule, telle que, pour toute représentation irréductible $\tau$ de G, on ait

$$
\tilde{\Gamma}(\tau) = Q_\Gamma(\lambda + \rho) - Q_\Gamma(\rho),
$$

où $\lambda$ est le plus grand poids de $\tau$. La forme $Q_\Gamma$ est positive, séparante et invariante par W.

Soit F une forme bilinéaire symétrique négative et séparante sur g définissant $\Gamma$. Soit $\tau : G \to GL(V)$ une représentation irréductible de G ; soient $\langle , \rangle$ un produit scalaire hilbertien sur V invariant par G ($§ 1,$ no 1), et $(e_i)$ une base de g telle que $F(e_i, e_j) = - \delta_{ij}$. Alors, pour tout élément $v$ de V non invariant par G, on a

$$
\tilde{\Gamma}(\tau) \langle v, v \rangle = \langle v, \Gamma_V(v) \rangle = - \sum_i \langle v, (e_i)_V^2 v \rangle = \sum_i \langle v, (e_i)_V^*(e_i)_V v \rangle
$$
$$
= \sum_i \langle (e_i)_V v, (e_i)_V v \rangle > 0,
$$

d’où a).

Soit B la forme inverse sur $t_C^*$ de la restriction à $t_C$ de la forme bilinéaire sur $g_C$ déduite de F par extension des scalaires. D’après le corollaire à la prop. 7 de VIII, § 6, n° 4, on a $^1$ $\tilde{\Gamma}(\tau) = B(\delta(\lambda), \delta(\lambda + 2\rho))$. Étendons $\delta : X(T) \to t_c^*$ en une application R-linéaire de $X(T) \otimes \mathbf{R}$ dans $t_c^*$ et soit $Q_\Gamma$ la forme quadratique $x \mapsto B(\delta(x), \delta(x))$ sur $X(T) \otimes \mathbf{R}$; elle est séparante et invariante par W, et on a

$$
\tilde{\Gamma}(\tau) = B(\delta(\lambda + \rho), \delta(\lambda + \rho)) - B(\delta(\rho), \delta(\rho)) = Q_\Gamma(\lambda + \rho) - Q_\Gamma(\rho) .
$$

Montrons maintenant que la forme $Q_\Gamma$ est positive. En effet, si $x \in X(T) \otimes \mathbf{R}$, l’élément $\delta(x)$ de $t_c^*$ prend des valeurs imaginaires pures sur t, donc des valeurs réelles sur $i t$; on conclut en remarquant que, pour $y \in i t$, on a $F(y, y) \geqslant 0$.

Il nous reste à prouver l’assertion d’unicité de b). Soit Q une forme quadratique sur $X(T) \otimes \mathbf{R}$ satisfaisant à la condition exigée, et soit $\Phi$ (resp. $\Phi_\Gamma$) la forme bilinéaire associée à Q (resp. $Q_\Gamma$). Pour $\lambda, \mu \in X(T)_{++}$, on a

$$
\Phi(\lambda, \mu) = (Q(\lambda + \mu + \rho) - Q(\rho)) - (Q(\lambda + \rho) - Q(\rho)) - (Q(\mu + \rho) - Q(\rho))
= \Phi_\Gamma(\lambda, \mu) .
$$

Comme $X(T)_{++}$ engendre le R-espace vectoriel $X(T) \otimes \mathbf{R}$, on a donc $\Phi = \Phi_\Gamma$, d’où $Q = Q_\Gamma$.

#### Remarque {#lie-ix-s7-n6-rem-1 .statement tag=01GQ}

Soit $x \in g$. Il existe un nombre réel strictement positif A tel que, pour toute représentation irréductible $\tau : G \to \mathbf{GL}(V)$ et toute structure hilbertienne sur V invariante par G, on ait

$$
\| L(\tau)(x) \| ^2 \leqslant A. \tilde{\Gamma}(\tau) .
$$

En effet, avec les notations de la démonstration précédente, on peut choisir la base $(e_i)$ de g de façon que $x = a e_1, a \in \mathbf{R}$. Alors, pour $v \in V$, on a

$$
\langle x_v v, x_v v \rangle = |a|^2 \langle e_1 v, e_1 v \rangle \leqslant |a|^2 \tilde{\Gamma}(\tau) \langle v, v \rangle .
$$

## EXERCICES {#lie-ix-s7-exercises}

See the [exercises for § 7](exercises/s7/).
