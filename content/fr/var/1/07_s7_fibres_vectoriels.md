---
book: var
book_title: Variétés différentielles et analytiques
chapter: "1"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 7
section_title: Fibrés vectoriels
lang: fr
source: var-fr
pdf_pages: 0068-0085
extraction: ocr
subsections:
    - "no": 1
      title: Définition des fibrés vectoriels
      page: 0
      pdf_page: 68
    - "no": 2
      title: Morphismes de fibrés vectoriels
      page: 0
      pdf_page: 69
    - "no": 3
      title: Morphismes multilinéaires
      page: 0
      pdf_page: 71
    - "no": 4
      title: Sections
      page: 0
      pdf_page: 72
    - "no": 5
      title: Sous-fibrés vectoriels, fibrés vectoriels quotients, suites exactes
      page: 0
      pdf_page: 74
    - "no": 6
      title: Foncteurs vectoriels
      page: 0
      pdf_page: 76
    - "no": 7
      title: Sommes directes, fibrés d’applications multilinéaires, dual
      page: 0
      pdf_page: 78
    - "no": 8
      title: Fibrés d’applications multilinéaires alternées
      page: 0
      pdf_page: 79
    - "no": 9
      title: Produits tensoriels, espaces tensoriels, algèbre extérieure
      page: 0
      pdf_page: 81
    - "no": 10
      title: Fibrés vectoriels et fibrés principaux
      page: 0
      pdf_page: 83
    - "no": 11
      title: Changement de structure
      page: 0
      pdf_page: 85
statements: 0
exercises: 0
content_sha256: fe137a4e6ae9d21a89fb2166378f27a2362444957d7ddf2dad763fead7f89cf4
---

## § 7. Fibrés vectoriels

Dans tout ce paragraphe, la lettre B désigne une variété de classe $C^r$ ($r \geqslant 1$) et la lettre M désigne un ensemble muni d'une application $\pi$ de M dans B. On dit que B est la base de M et pour tout $b \in B$, on désigne par $M_b$ et on appelle fibre de M en $b$ le sous-ensemble $\pi^{-1}(b)$ de M.

### 7.1. Définition des fibrés vectoriels

7.1.1. Une carte vectorielle de M est un triplet $t = (U, \varphi, F)$, où U est un ouvert de B, où F est un espace de Banach et $\varphi$ une bijection de $\pi^{-1}(U)$ sur $U \times F$ telle que $\pi(\varphi^{-1}(b, h)) = b$ pour tout $b \in B$ et tout $h \in F$. On dit que U est le domaine de la carte vectorielle t et que t est une carte vectorielle de M en $b \in B$ si $b \in U$. Pour tout $b \in U$, on note $t_b$ la bijection de F sur $M_b$ définie par $t_b(h) = \varphi^{-1}(b, h)$ pour $h \in F$.

7.1.2. On dit que deux cartes vectorielles $t = (U, \varphi, F)$ et $t' = (U', \varphi', F')$ de M sont $C^r$-compatibles (ou simplement compatibles) s'il existe une application $\lambda$ de classe $C^r$ de la variété $U \cap U'$ dans l'espace de Banach $\mathcal{L}(F; F')$ telle que:

$$
t_b = t'_b \circ \lambda(b) \quad \text{pour tout } b \in U \cap U'.
$$

7.1.3. On dit qu'un ensemble de cartes vectorielles de M est un $C^r$-atlas vectoriel (ou simplement atlas vectoriel) de M s'il se compose de cartes vectorielles deux à deux $C^r$-compatibles dont les domaines ont B pour réunion. On dit que deux atlas vectoriels $\mathcal{A}$ et $\mathcal{B}$ de M sont $C^r$-équivalents (ou équivalents) si $\mathcal{A} \cup \mathcal{B}$ est encore un atlas vectoriel de M. Cette relation est une relation d'équivalence.

7.1.4. Une structure de fibré vectoriel de classe $C^r$ (de base B) sur M est la donnée d'une classe d'atlas vectoriels équivalents (Ens., Chap. II, § 6, n° 9). Une carte vectorielle appartenant à un atlas vectoriel de cette classe est appelée une carte vectorielle du fibré vectoriel M.

Soit M un fibré vectoriel de base B. Pour tout $b \in B$, il existe sur la fibre $M_b$ une structure d'espace de Banach et une seule telle que, pour toute carte vectorielle $t = (U, \varphi, F)$ du fibré vectoriel M en $b$, l'application $t_b$ soit un isomorphisme de F sur $M_b$.

Soit $c = (U, \psi, E)$ une carte de la variété B et soit $t = (U, \varphi, F)$ une carte vectorielle du fibré vectoriel M, de même domaine U. Pour $x \in \pi^{-1}(U)$, posons:

$$
\alpha(x) = (\psi(\pi(x)), t_{\pi(x)}^{-1}(x)).
$$

Alors, le triplet $(\pi^{-1}(U), \alpha, E \times F)$ est une carte de l’ensemble $M$. Il existe sur $M$ une structure de variété de classe $C'$ et une seule (dite sous-jacente à $M$) pour laquelle toutes les cartes ainsi obtenues sont des cartes de la variété $M$. Le triplet $(M, B, \pi)$ est alors une fibration (6.1.1).

7.1.5. Soit $F$ un espace de Banach. Posons $M = B \times F$, l’application étant la première projection. Il existe sur $M$ une structure de fibré vectoriel (de base $B$) et une seule pour laquelle $(B, \mathrm{Id}_M, F)$ est une carte vectorielle. On dit que $B \times F$ muni de cette structure est le fibré vectoriel trivial de base $B$ et de fibre $F$ et on le note parfois $F_B$. La structure de variété de $F_B$ est la structure de variété produit et pour tout $b \in B$, l’application $h \mapsto (b, h)$ est un isomorphisme d’espaces de Banach de $F$ sur la fibre de $F_B$ au point $b \in B$. On note souvent $0$ un fibré vectoriel trivial de fibre réduite à $0$.

7.1.6. Soit $M$ un fibré vectoriel de base $B$. Pour $b \in B$, on appelle rang de $M$ en $b$ et on note $\mathrm{rg}_b(M)$, la dimension (finie ou $+\infty$) de l’espace de Banach $M_b$. On a $\dim_x M = \dim_b B + \mathrm{rg}_b M$ pour $b = \pi(x)$. La fonction $b \mapsto \mathrm{rg}_b M$ est localement constante. On dit que $M$ est de rang fini si $\mathrm{rg}_b M < +\infty$ pour tout $b \in B$.

### 7.2. Morphismes de fibrés vectoriels

7.2.1. Soient $B$ et $B'$ deux variétés et soit $f$ un morphisme de $B$ dans $B'$. Soient $M$ un fibré vectoriel de base $B$ et $M'$ un fibré vectoriel de base $B'$. On dit qu’une application $g$ de $M$ dans $M'$ est un $f$-morphisme de fibrés vectoriels si la condition suivante est réalisée :

Pour tout point $b_0 \in B$, il existe une carte vectorielle $t = (U, \varphi, F)$ de $M$ en $b_0$, une carte vectorielle $t' = (U', \varphi', F')$ de $M'$ en $f(b_0)$ et une application $\lambda$ de classe $C'$ de $U$ dans $\mathcal{L}(F; F')$ telles que $f(U) \subset U'$ et que $g_b \circ t_b = t'_{f(b)} \circ \lambda(b)$ pour tout $b \in U$, où $g_b$ est la restriction de $g$ à $M_b$.

Sous ces hypothèses, $g$ est un morphisme de variétés et pour tout $b \in B$, $g$ induit une application linéaire continue de $M_b$ dans $M'_{f(b)}$. On appelle rang vectoriel de $g$ en $b \in B$ et on note $\mathrm{rg}_b(g)$ le rang (fini ou $+\infty$) de l’application linéaire $g_b$.

Réciproquement, si $r \geqslant \infty$ ou si $M$ est de rang fini, un $f$-morphisme de fibrations de $(M, B, \pi)$ dans $(M', B', \pi')$ qui induit sur chaque fibre $M_b$ une application linéaire de $M_b$ dans $M'_{f(b)}$ (pour tout $b \in B$), est un $f$-morphisme de fibrés vectoriels.

7.2.2. Soit de plus $f'$ un morphisme de $B'$ dans une variété $B''$. Si $g$ est un $f$-morphisme de $M$ dans $M'$, et si $g'$ est un $f'$-morphisme de $M'$ dans un fibré vectoriel $M''$ de base $B''$, l’application $g' \circ g$ est un $(f' \circ f)$-morphisme de $M$ dans $M''$. On a $(g' \circ g)_b = g'_{f(b)} \circ g_b$ pour tout $b$ dans $B$.

7.2.3. Soient M et M' deux fibrés vectoriels de même base B. On appelle B-morphisme, ou simplement morphisme de M dans M' tout Id_B-morphisme. Le composé de deux morphismes est un morphisme.

Soit g un morphisme de fibrés vectoriels de M dans M'; si g est bijectif, c'est un isomorphisme de la variété M sur la variété M', l'application réciproque $g^{-1}$ est un morphisme de fibrés vectoriels de M' dans M et l'on a $(g^{-1})_b = g_b^{-1}$ pour tout b dans B. L'application g est alors un isomorphisme de fibrés vectoriels.

7.2.4. Soit f un morphisme d'une variété B' dans B et soit M un fibré vectoriel de base B. Posons $M' = B' \times_B M$ et notons $\pi'$ (resp. g) la restriction à M' de la projection de $B' \times M$ sur B' (resp. M). Il existe sur M' une structure de fibré vectoriel de base B' (relativement à $\pi'$) et une seule pour laquelle g est un f-morphisme. On dit que M' est le fibré vectoriel de base B' image réciproque de M par f et on le note $f^*M$; le f-morphisme g est appelé le f-morphisme canonique de $f^*M$ dans M.

La structure de variété de $f^*M$ est celle du produit fibré des variétés B' et M au dessus de B (5.11.2); pour tout $b \in B'$, l'application $x \mapsto (b, x)$ est un isomorphisme d'espaces de Banach de $M_{f(b)}$ sur $(f^*M)_b$.

La formation des images réciproques de fibrés vectoriels est transitive.

Soit N' un fibré vectoriel de base B' et soit h un f-morphisme de N' dans M. Il existe un B'-morphisme $\tilde{h}$ et un seul de N' dans $f^*M$ tel que $h = g \circ \tilde{h}$.

Soient N un fibré vectoriel de base B et v un B-morphisme de N dans M. Il existe un B'-morphisme et un seul, noté $f^*v$, de $f^*N$ dans $f^*M$ tel que le diagramme

$$
\begin{array}{ccc}
f^*N & \xrightarrow{f^*v} & f^*M \\
\downarrow & & \downarrow \\
N & \xrightarrow{v} & M
\end{array}
$$

soit commutatif.

7.2.5. Soit B' une sous-variété de B et soit i l'injection canonique de B' dans B. Si M est un fibré vectoriel de base B, l'image réciproque $i^*M$ s'appelle le fibré vectoriel induit sur B' par M et se note $M|B'$. Si $t = (U, \varphi, F)$ est une carte vectorielle de M, alors $(U \cap B', \varphi|\pi^{-1}(U \cap B'), F)$ est une carte vectorielle de $M|B'$. Le f-morphisme canonique de $M|B'$ dans M est un isomorphisme de variétés de $M|B'$ sur la sous-variété $\pi^{-1}(B')$ de M.

7.2.6. Soit f un morphisme d'une variété B' dans B et soit M (resp. M') un fibré vectoriel de base B (resp. B'). On appelle f-comorphisme de M dans M' un B'-morphisme de $f^*M$ dans M'. Lorsque B = B' et $f = \mathrm{Id}_B$, la donnée d’un $f$-comorphisme de $M$ dans $M'$ équivaut à la donnée d’un $B$-morphisme de $M$ dans $M'$.

Soit $g$ un $f$-comorphisme de $M$ dans $M'$. Pour tout $b \in B'$, l’application $g_b : x \mapsto g(b, x)$ de $M_{f(b)}$ dans $M'_b$ est une application linéaire continue.

Soit de plus $f'$ un morphisme d’une variété $B''$ dans $B'$ et soit $h$ un $f'$-comorphisme de $M'$ dans un fibré vectoriel $M''$ de base $B''$. L’application $h \circ f^*g$ de ${f'}^*(f^*M) = (f \circ f')^*M$ dans $M''$ est alors un $(f \circ f')$-comorphisme de $M$ dans $M''$, noté $h \circ g$. Pour $b \in B''$, on a

$$
(h \circ g)_b = h_b \circ g_{f'(b)}.
$$

### 7.3. Morphismes multilinéaires

7.3.1. Soient $M_1, \ldots, M_d$ et $N$ des fibrés vectoriels de base $B$, et soit $u$ une application de l’ensemble $M_1 \times_B \cdots \times_B M_d$ dans $N$. On dit que $u$ est un *morphisme multilinéaire* (ou $d$-linéaire) si la condition suivante est réalisée:

*Pour tout $b_0 \in B$, il existe un voisinage ouvert $U$ de $b_0$ dans $B$, des cartes vectorielles $t^j = (U, \varphi^j, F^j)$ de $M_j$ (pour $1 \leq j \leq d$) et $t = (U, \varphi, F)$ de $N$, et une application $\lambda$ de classe $C^r$ de $U$ dans l’espace de Banach $\mathcal{L}(F^1, \ldots, F^d; F)$ des applications $d$-linéaires continues de $F^1 \times \cdots \times F^d$ dans $F$, tels que*:

$$
(t_b \circ \lambda(b))(x_1, \ldots, x_d) = u(t_b^1(x_1), \ldots, t_b^d(x_d))
$$

*pour tout $b \in U$ et tous $x_j \in F^j$*.

Tout morphisme multilinéaire $u$ est un morphisme de variétés du produit fibré $M_1 \times_B \cdots \times_B M_d$ dans $N$ et induit pour tout $b \in B$ une application $d$-linéaire continue $u_b$ de $(M_1)_b \times \cdots \times (M_d)_b$ dans $N_b$.

Si $f$ est un morphisme de $B$ dans une variété $B'$, un morphisme multilinéaire de $M_1 \times_B \cdots \times_B M_d$ dans un fibré vectoriel $M'$ de base $B'$ est par définition le composé d’un morphisme multilinéaire de $M_1 \times_B \cdots \times_B M_d$ dans $f^*M'$ avec le $f$-morphisme canonique de $f^*M'$ dans $M'$.

Un morphisme bilinéaire est encore appelé un *accouplement*. Pour $d = 1$, un morphisme linéaire est un morphisme au sens de 7.2.1. Pour $d = 0$, un morphisme 0-linéaire s’identifie à une *section* de $N$ (7.4).

7.3.2. On appelle *fibré en algèbres* de base $B$ un fibré vectoriel $A$ de base $B$, muni d’un accouplement de $A \times_B A$ dans $A$. Chaque fibre $A_b$ est alors munie d’une structure de $K$-algèbre. Si pour tout $b \in B$, l’algèbre $A_b$ a un élément unité, noté $e_b$, l’application $b \mapsto e_b$ est une section de $A$ (cf. 7.4). On dit qu’un fibré en algèbres $A$ est *localement trivial* si, pour tout point $b_0$ de $B$, il existe une carte vectorielle $t = (U, \varphi, E)$ de $A$ au point $b_0$ et une structure de $K$-algèbre sur $E$ telles que $t_b$ soit un isomorphisme d’algèbres de $E$ sur $A_b$ pour tout $b \in U$.

7.3.3. Soit $A$ un fibré en algèbres associatives avec élément unité de base $B$. On appelle *fibré en A-modules* de base $B$ un fibré vectoriel $M$ de base $B$ muni d’un accouplement $m : A \times_B M \to M$ tel que l’application $m_b : A_b \times M_b \to M_b$ définisse, pour tout $b \in B$, une structure de $A_b$-module sur la fibre $M_b$.

Soient $M$ et $M'$ deux fibrés en $A$-modules. On appelle *A-homomorphisme* de $M$ dans $M'$ tout morphisme $g : M \to M'$ de fibrés vectoriels de base $B$ qui induit pour tout $b$ dans $B$ une application $A_b$-linéaire de $M_b$ dans $M'_b$.

Supposons $A$ localement trivial. On dit qu’un fibré $M$ en $A$-modules est *localement trivial* si pour tout point $b_0$ de $B$, il existe une carte vectorielle $t = (U, \varphi, E)$ de $A$ en $b_0$ comme dans 7.3.2, une carte vectorielle $t' = (U, \varphi', L)$ de $M$ en $b_0$, et une structure de $E$-module sur $L$ telles que, pour tout $b \in U$, $t'_b$ soit un $t_b$-isomorphisme du $A_b$-module $M_b$ sur le $E$-module $L$.

7.3.4. Soit $A$ une algèbre de Banach sur $K$ (par exemple un corps muni d’une structure de $K$-algèbre de dimension finie). Le fibré trivial $A_B$ est alors un fibré en algèbres, localement trivial. Un fibré en $A_B$-modules $M$ localement trivial est encore appelé un fibré vectoriel sur $A$ (de base $B$). Les fibres $M_b$ sont alors des $A$-modules topologiques. Un $f$-morphisme $u$ de $M$ dans un autre fibré vectoriel sur $A$ est dit $A$-linéaire si les applications $u_b$ sont $A$-linéaires pour tout $b \in B$.

### 7.4. Sections

7.4.1. Soit $M$ un fibré vectoriel de base $B$. Pour tout ouvert $U$ de $B$, on note $\mathscr{S}_M^r(U)$ l’ensemble des sections de classe $C^r$ de $M$ sur $U$, c’est-à-dire des morphismes $s$ de classe $C^r$ de $U$ dans $M$ tels que $s(b) \in M_b$ pour tout $b \in U$. Cet ensemble est muni d’une structure de module sur l’anneau $\mathscr{C}^r(U)$ des fonctions morphiques par les règles:

(1)
$$
(s + s')(b) = s(b) + s'(b)
$$
(2)
$$
(\varphi \cdot s)(b) = \varphi(b) \cdot s(b)
$$
pour $s, s'$ dans $\mathscr{S}_M^r(U)$ et $\varphi$ dans $\mathscr{C}^r(U)$. Lorsque l’ouvert $U$ varie, on obtient un faisceau $\mathscr{S}_M^r$ d’applications de $B$ dans $M$ (cf. n° 5.4.1), appelé *faisceau des sections* de $M$.

7.4.2. Soient $M_1, \ldots, M_d$ et $N$ des fibrés vectoriels de base $M$ et $u$ un morphisme multilinéaire de $M_1 \times_B \ldots \times_B M_d$ dans $N$. Pour $1 \leq j \leq d$, donnons-nous une section $s_j$ de $M_j$ sur un ouvert $U$ de $B$; on définit une section $u(s_1, \ldots, s_d)$ de $N$ sur $U$ par la formule:
$$
u(s_1, \ldots, s_d)(b) = u_b(s_1(b), \ldots, s_d(b)) \quad \text{pour } b \in U.
$$

L’application $(s_1, \ldots, s_d) \mapsto u(s_1, \ldots, s_d)$ est $\mathcal{C}^r(U)$-multilinéaire. On la note parfois $\mathscr{S}(u)$.

7.4.3. Soit $f$ un morphisme d’une variété $B'$ dans $B$ et soit $M$ un fibré vectoriel de base $B$. Pour tout ouvert $U$ de $B$ et tout $s \in \mathscr{S}_M^r(U)$, l’application $x \mapsto (x, s(f(x)))$ est une section de classe $C^r$ de $f^*M$ sur l’ouvert $f^{-1}(U)$, notée $f^*s$ et appelée image réciproque de $s$ par $f$. L’application $s \mapsto f^*s$ de $\mathscr{S}_M^r(U)$ dans $\mathscr{S}_{f^*M}(f^{-1}(U))$ est semi-linéaire par rapport à l’homomorphisme $g \mapsto g \circ (f|f^{-1}(U))$ de $\mathcal{C}^r(U)$ dans $\mathcal{C}^r(f^{-1}(U))$.

Si de plus $N$ est un fibré vectoriel de base $B'$ et $g$ un $f$-comorphisme de $M$ dans $N$, on note parfois $\mathscr{S}(g)$ l’application $s \mapsto g \circ f^*s$ de $\mathscr{S}_M^r(U)$ dans $\mathscr{S}_N^r(f^{-1}(U))$.

7.4.4. Soit $M$ un fibré vectoriel de base $B$, *de rang fini*. On appelle *repère* de $M$ sur un ouvert $U$ de $B$ une suite finie $(s_1, \ldots, s_n)$ de sections de $M$ sur $U$ telle que $(s_1(b), \ldots, s_n(b))$ soit une *base* de l’espace vectoriel $M_b$ pour tout $b \in B$. La suite $(s_1, \ldots, s_n)$ est alors une base du $\mathcal{C}^r(U)$-module $\mathscr{S}_M^r(U)$. Si $f$ est un morphisme d’une variété $B'$ dans $B$, les sections $f^*s_j$ forment un repère de $f^*M$ sur $f^{-1}(U)$.

7.4.5. Soit $L$ un corps, muni d’une structure de $K$-algèbre de dimension finie et soit $(M, B, \pi)$ une fibration. Supposons donnée sur chaque fibre $M_b$ une structure d’espace vectoriel sur $L$, *de dimension finie*. Il existe alors au plus une structure de fibré vectoriel sur $L$ de base $B$ sur $M$, compatible avec l’application $\pi$, la structure de variété de $M$ et les structures $L$-vectorielles sur les fibres (7.3.4). Pour qu’il en existe une, il faut et il suffit que la condition suivante soit réalisée :

(FV) *Pour tout $b_0 \in B$, il existe un voisinage ouvert $U$ de $b_0$ dans $B$ et un isomorphisme de variétés $\varphi$ de $\pi^{-1}(U)$ sur le produit $U \times F$ de $U$ par un espace vectoriel $F$ sur $L$ de dimension finie, tel que pour tout $b \in U$, la bijection $\varphi_b$ de $M_b$ sur $F$ induite par $\varphi$ soit un isomorphisme d’espaces vectoriels sur le corps $L$.*

Les triplets $(U, \varphi, F)$ satisfaisant à (FV) sont alors des cartes vectorielles du fibré vectoriel $M$.

La condition (FV) est équivalente à :
(FV') *Pour tout $b_0 \in B$, il existe un entier $n$ et $n$ sections $s_1, \ldots, s_n$ de $M$ sur un voisinage ouvert $U$ de $b_0$ tels que l’application*
$$
(b, a_1, \ldots, a_n) \mapsto a_1 s_1(b) + \cdots + a_n s_n(b)
$$
*soit un isomorphisme de la variété $U \times L^n$ sur la variété $\pi^{-1}(U)$.*

7.4.6. Soient $M_1, \ldots, M_d$ et $N$ des fibrés vectoriels de base $B$, les $M_j$ étant de *rang fini*. Supposons donnée pour tout ouvert $U$ de $B$ une application $\varphi_U$ de $\mathscr{S}_{M_1}^r(U) \times \cdots \times \mathscr{S}_{M_d}^r(U)$ dans $\mathscr{S}_N^r(U)$, $\mathcal{C}^r(U)$-multilinéaire, telles que pour $V \subset U$ l’on ait:

$$
\varphi_U(s_1, \ldots, s_d)|V = \varphi_V(s_1|V, \ldots, s_d|V).
$$

Il existe alors un morphisme multilinéaire $u$ de $M_1 \times_B \ldots \times_B M_d$ dans $N$ et un seul tel que $\varphi_U(s_1, \ldots, s_d) = u(s_1, \ldots, s_d)$ quelles que soient les sections $s_j$ de $M$ sur l’ouvert $U$ de $B$.

7.4.7. Soit $f$ un morphisme d’une variété $B'$ dans $B$ et soit $M$ (resp. $M'$) un fibré vectoriel de base $B$ (resp. $B'$) et de rang fini. Supposons donnée pour tout ouvert $U$ de $B$ une application $\varphi_U$ de $\mathcal{S}_M^r(U)$ dans $\mathcal{S}_{M'}^{r'}(f^{-1}(U)), \mathcal{C}^r(U)$-semi-linéaire, telles que

$$
\varphi_U(s)|f^{-1}(V) = \varphi_V(s|V)
$$

pour tout ouvert $V \subset U$. Il existe alors un $f$-comorphisme $g$ et un seul de $M$ dans $M'$ tel que $\varphi_U(s) = \mathcal{S}(g)(s)$ pour tout $s \in \mathcal{S}_M^r(U)$.

*7.4.8. Soit $\mathcal{F}$ un faisceau de modules sur le faisceau d’anneaux $\mathcal{C}_B^r$. On dit que $\mathcal{F}$ est localement libre si pour tout $b \in B$, il existe un voisinage ouvert $U$ de $b$ et un entier $n$ tels que $\mathcal{F}|U$ soit isomorphe (comme faisceau de $\mathcal{C}_U^r$-modules) au faisceau $(\mathcal{C}_U^r)^n$.

Si $M$ est un fibré vectoriel de base $B$ de rang fini, le faisceau $\mathcal{S}_M^r$ est localement libre. Réciproquement, pour tout faisceau localement libre $\mathcal{F}$ sur $B$, il existe un fibré vectoriel $M$ et un isomorphisme de faisceaux de $\mathcal{S}_M^r$ sur $\mathcal{F}$. Si $M'$ est un autre fibré vectoriel de base $B$ de rang fini, l’application $g \mapsto \mathcal{S}(g)$ est une bijection de l’ensemble des $B$-morphismes de $M$ dans $M'$ sur l’ensemble des morphismes de faisceaux de $\mathcal{C}^r$-modules de $\mathcal{S}_M^r$ dans $\mathcal{S}_{M'}^{r'}$*

### 7.5. Sous-fibrés vectoriels, fibrés vectoriels quotients, suites exactes

Dans ce numéro, on appelle fibré vectoriel un fibré vectoriel de base $B$ et morphisme de fibré vectoriels un $\mathrm{Id}_B$-morphisme.

7.5.1. Soit $M$ un fibré vectoriel. Un sous-ensemble $M'$ de $M$ est appelé un sous-fibré vectoriel de $M$ si, pour tout point $b \in B$, il existe une carte vectorielle $t = (U, \varphi, E)$ de $M$ en $b$ et un sous-espace vectoriel fermé $F$ de $E$ admettant un supplémentaire topologique, tels que

$$
\varphi(\pi^{-1}(U) \cap M') = U \times F.
$$

Dans ces conditions, il existe sur $M'$ une structure de fibré vectoriel et une seule pour laquelle l’injection canonique de $M'$ dans $M$ est un morphisme. Pour chaque $b \in B$, la fibre $M'_b$ de $M'$ est le sous-espace vectoriel fermé $M' \cap M_b$ de $M_b$; $M'$ est une sous-variété fermée de $M$ et la structure de variété sous-jacente à la structure de fibré vectoriel de $M'$ coïncide avec celle induite par la structure de variété de $M$.

7.5.2. Soit $M'$ un sous-fibré vectoriel de $M$. Notons $R\{x, y\}$ la relation suivante entre points $x, y$ de $M$:
« il existe un élément $b$ de $B$ tel que $x \in M_b, y \in M_b$ et $x - y \in M'_b$ ». Alors $R$ est une relation d'équivalence régulière sur $M$ (cf. n° 5.9.7). Sur l'ensemble $M/R$, il existe une structure de fibré vectoriel et une seule telle que l'application canonique de $M$ sur $M/R$ soit un morphisme. On note $M/M'$ et l'on appelle quotient de $M$ par $M'$ le fibré vectoriel ainsi défini ; pour chaque point $b$ de $B$, le fibré $(M/M')_b$ est l'espace vectoriel topologique quotient $M_b/M'_b$ et la structure de variété sur $M/M'$ est quotient de celle de $M$.

7.5.3. Conservons les hypothèses de 7.5.2. Pour tout point $b_0$ de $B$, on peut trouver un voisinage ouvert $U$ de $b_0$, un espace de Banach $F$, somme directe de deux sous-espaces fermés $F'$ et $F''$, et un isomorphisme de fibrés vectoriels $\iota$ de $F_U$ sur $M|U$ avec les propriétés suivantes :
(i) La restriction $\iota'$ de $\iota$ à $U \times F'$ est un isomorphisme de $F'_U$ sur $M'|U$.
(ii) Si $\rho$ est l'application canonique de $M$ sur $M'' = M/M'$, et si $\iota''$ est la restriction de $\iota$ à $U \times F''$, l'application $\rho \circ \iota''$ est un isomorphisme de $F''_U$ sur $M''|U$.

7.5.4. Si un morphisme de fibrés vectoriels $g : L \to M$ a son image contenue dans $M'$, c'est un morphisme de fibrés vectoriels de $L$ dans $M'$.
Considérons maintenant un morphisme de fibrés vectoriels $h : M \to N$ et supposons que, pour tout $b$ dans $B$, la restriction de $h_b$ à $M'_b$ soit nulle. Si $\rho$ est le morphisme canonique de $M$ sur $M/M'$, il existe un morphisme $\bar{h}$ de $M/M'$ dans $N$ et un seul tel que $h = \bar{h} \circ \rho$.

7.5.5. Soient $P$ et $Q$ deux fibrés vectoriels, et $g$ un morphisme de $P$ dans $Q$; pour tout point $b$ de $B$, notons $N_b$ et $I_b$ respectivement le noyau et l'image de l'application linéaire $g_b : P_b \to Q_b$. Posons $N = \bigcup_{b \in B} N_b$ et $I = \bigcup_{b \in B} I_b$. On dit que le morphisme $g$ est localement direct si $N$ est un sous-fibré vectoriel de $P$ et $I$ un sous-fibré vectoriel de $Q$. Le morphisme $g$ définit alors par passage au quotient un isomorphisme de $P/N$ sur $I$. On dit que $N$ est le noyau de $g$ et on le note $\mathrm{Ker}\,g$. De même, le sous-fibré $I$ est appelé l'image de $g$ et est noté $\mathrm{Im}\,g$.
Si $r \geqslant \infty$, le morphisme $g$ est localement direct si et seulement si $g$ est une subimmersion. Si $P$ est de rang fini, le morphisme $g$ est localement direct si et seulement si le rang vectoriel de $g$ est localement constant ou encore si et seulement si $g$ est une subimmersion.

7.5.6. Soient $M \xrightarrow{f} M' \xrightarrow{g} M''$ deux morphismes de fibrés vectoriels. On dit que la suite $(f, g)$ est exacte localement directe si les deux morphismes $f$ et $g$ sont localement directs et si $\operatorname{Im} f = \operatorname{Ker} g$. Si $g \circ f = 0$, l’ensemble $D$ des points $b \in B$ tels que la suite $M_b \xrightarrow{f_b} M'_b \xrightarrow{g_b} M''_b$ soit exacte directe (c’est-à-dire tels que $\operatorname{Ker} f_b$ et $\operatorname{Im} g_b$ admettent des supplémentaires topologiques et que $\operatorname{Im} f_b = \operatorname{Ker} g_b$) est ouvert et la suite $M|D \xrightarrow{f} M'|D \xrightarrow{g} M''|D$ est exacte localement directe.

On définir de même les suites exactes localement directes de longueur quelconque. Par abus de langage, on dit parfois suite exacte directe au lieu de suite exacte localement directe.

7.5.7. Soit $0 \to M \xrightarrow{f} M' \xrightarrow{g} M'' \to 0$ une suite de morphismes de fibrés vectoriels. Pour que cette suite soit exacte localement directe, il faut et il suffit que $f$ soit un isomorphisme de $M$ sur un sous-fibré vectoriel $f(M)$ de $M'$ et que $g$ définisse par passage au quotient un isomorphisme du fibré vectoriel quotient $M'/f(M)$ sur $M''$.

### 7.6. Foncteurs vectoriels

Dans ce n° et dans les trois n°s suivants 7.7 à 7.9, la lettre I désigne un ensemble fini, réunion de deux sous-ensembles disjoints $I_+$ et $I_-$. On désigne par $\mathcal{V} = (V_i)_{i \in I}$ (et de manière analogue par $\mathcal{V}', \mathcal{V}'', \ldots$) une famille d’espaces de Banach indexée par $I$. On désigne par $\operatorname{Hom}(\mathcal{V}, \mathcal{V}')$ l’espace de Banach $\prod_{i \in I_+} \mathcal{L}(V_i; V'_i) \times \prod_{i \in I_-} \mathcal{L}(V'_i; V_i)$ et par $f = (f_i)$ un élément de $\operatorname{Hom}(\mathcal{V}, \mathcal{V}')$. On note $\operatorname{Id}_{\mathcal{V}}$ l’élément $(\operatorname{Id}_{V_i})_{i \in I}$ de $\operatorname{Hom}(\mathcal{V}, \mathcal{V})$. Pour $f \in \operatorname{Hom}(\mathcal{V}, \mathcal{V}')$ et $f' \in \operatorname{Hom}(\mathcal{V}', \mathcal{V}'')$, on note $f' \circ f$ l’élément de $\operatorname{Hom}(\mathcal{V}, \mathcal{V}'')$ dont les composantes sont données par:

$$
(f' \circ f)_i = f'_i \circ f_i \quad \text{si } i \in I_+
$$
$$
(f' \circ f)_i = f_i \circ f'_i \quad \text{si } i \in I_-
$$

7.6.1. On appelle foncteur vectoriel (resp. foncteur vectoriel en dimension finie) de type I et de classe $C^r$ la donnée pour toute famille $\mathcal{V} = (V_i)_{i \in I}$ d’espaces de Banach (resp. d’espaces vectoriels de dimension finie sur $K$) d’un espace de Banach $\tau(\mathcal{V})$ et pour tout $f \in \operatorname{Hom}(\mathcal{V}, \mathcal{V}')$ d’un élément $\tau(f) \in \mathcal{L}(\tau(\mathcal{V}); \tau(\mathcal{V}'))$, ces données étant assujetties aux deux conditions suivantes:
(a) On a $\tau(\operatorname{Id}_\mathcal{V}) = \operatorname{Id}_{\tau(\mathcal{V})}$ et $\tau(f' \circ f) = \tau(f') \circ \tau(f)$.
(b) L’application $\tau : \operatorname{Hom}(\mathcal{V}, \mathcal{V}') \to \mathcal{L}(\tau(\mathcal{V}); \tau(\mathcal{V}'))$ est de classe $C^r$.

7.6.2. Soit $\mathcal{M} = (M^i)_{i \in I}$ une famille de fibrés vectoriels de base $B$. Pour $b \in B$, posons $\mathcal{M}_b = (M^i_b)_{i \in I}$. Soit $\tau$ un foncteur vectoriel et soit $\tau(\mathcal{M})$ l’ensemble somme des $\tau(\mathcal{M}_b)$ pour $b \in B$; *il existe sur $\tau(\mathcal{M})$ une structure de fibré vectoriel et une seule* (de base $B$ relativement à l’application $\pi$ de $\tau(\mathcal{M})$ dans $B$ telle que pour tout $b \in B$, on ait $\tau(\mathcal{M}_b) = \{ b \}$) possédant la propriété suivante:

Soit $U$ un ouvert de $B$ et, pour tout $i$, soit $t^i = (U, \varphi_i, F_i)$ une carte vectorielle de $M^i$, de domaine $U$; posons $\mathcal{F} = (F_i)_{i \in I}$ et soit $\psi_b$ l’élément de $\mathrm{Hom}(\mathcal{M}_b, \mathcal{F})$ défini par $(\psi_b)_i = (t^i_b)^{-1}$ pour $i \in I_+$ et $(\psi_b)_i = t^i_b$ pour $i \in I_-$; pour $x \in \pi^{-1}(U)$, posons $\psi(x) = (\pi(x), \tau(\psi_{\pi(x)})(x))$. Alors le triplet $(U, \psi, \tau(\mathcal{F}))$ est une carte vectorielle du fibré vectoriel $\tau(\mathcal{M})$.

Muni de cette structure, $\tau(\mathcal{M})$ s’appelle le *fibré vectoriel déduit de la famille $\mathcal{M}$ par le foncteur vectoriel $\tau$*.

7.6.3. Soit $f$ un morphisme de $B$ dans une variété $B'$. Soit $\mathcal{M} = (M^i)$ (resp. $\mathcal{M}' = ({M'}^i)$) un famille indexée par $I$ de fibrés vectoriels de base $B$ (resp. $B'$). Pour tout $i \in I_+$, soit $g_i$ un $f$-morphisme de $M^i$ dans ${M'}^i$ et pour tout $i \in I_-$, soit $g_i$ un $f$-comorphisme de ${M'}^i$ dans $M^i$. Posons $g = (g_i)_{i \in I}$ et pour $b \in B$, posons $g_b = ((g_i)_b)_{i \in I}$ (cf. 7.2.1 et 7.2.6). *Il existe un $f$-morphisme et un seul, noté $\tau(g)$, de $\tau(\mathcal{M})$ dans $\tau(\mathcal{M}')$ tel que $\tau(g)_b = \tau(g_b)$ pour tout $b \in B$*.

Si en particulier $M^i = f^*{M'}^i$, les $g_i$ étant les morphismes ou comorphismes canoniques, alors le $B$-morphisme de $\tau(\mathcal{M})$ dans $f^*\tau(\mathcal{M}')$ défini par $\tau(g)$ (7.2.4) est un isomorphisme : on exprime ce fait en disant que $\tau$ *commute aux images réciproques*.

En particulier soit $B'$ une sous-variété de $B$ et posons $\mathcal{M}|B' = (M^i|B')_{i \in I}$. Les fibrés vectoriels $\tau(\mathcal{M})|B'$ et $\tau(\mathcal{M}|B')$ sont alors canoniquement $B'$-isomorphes.

7.6.4. Soient $\tau, \tau_1, \ldots, \tau_d$ des foncteurs vectoriels (de type $I$ et de classe $C'$). Un *morphism d-linéaire* $\theta$ de $(\tau_1, \ldots, \tau_d)$ dans $\tau$ est la donnée pour toute famille $\mathcal{V}$ d’espaces de Banach indexée par $I$ d’une application $d$-linéaire continue $\theta_{\mathcal{V}}$ de $\tau_1(\mathcal{V}) \times \cdots \times \tau_d(\mathcal{V})$ dans $\tau(\mathcal{V})$, cette donnée satisfaisant à la condition suivante : pour tout $f \in \mathrm{Hom}(\mathcal{V}', \mathcal{V}'')$ on a
$$
\tau(f) \circ \theta_{\mathcal{V}} = \theta_{\mathcal{V}''} \circ (\tau_1(f) \times \cdots \times \tau_d(f)).
$$
Pour $d = 1$, on dit simplement un *morphism* de $\tau_1$ dans $\tau$.

Soit alors $\mathcal{M}$ une famille indexée par $I$ de fibrés vectoriels de base $B$.
*Il existe un B-morphisme d-linéaire $\theta_{\mathcal{M}}$ et un seul de $\tau_1(\mathcal{M}) \times_B \cdots \times_B \tau_d(\mathcal{M})$ dans $\tau(\mathcal{M})$ tel que $(\theta_{\mathcal{M}})_b = \theta_{\mathcal{M}_b}$ pour tout $b \in B$*.

Avec les notations de 7.6.3., on a
$$
\tau(g) \circ \theta_{\mathcal{M}} = \theta_{\mathcal{M}'} \circ (\tau_1(g) \times \cdots \times \tau_d(g)).
$$
Si $d = 1$, et si $\theta$ est un isomorphisme (ce qui veut dire que $\theta_{\mathcal{V}}$ est un isomorphisme pour toute famille $\mathcal{V}$), alors $\theta_{\mathcal{M}}$ est un isomorphisme.

7.6.5. Les définitions et résultats des n°s 7.6.2 à 7.6.4 s’étendent au cas des foncteurs vectoriels en dimension finie, à condition de supposer partout les fibrés vectoriels donnés de rang fini.

Ils s’étendent également au cas suivant : soit L un corps muni d’une structure de K-algèbre de dimension finie ; on prend pour τ un foncteur vectoriel sur L (i.e. satisfaisant aux hypothèses de 7.6.1 où l’on a remplacé K par L), et on ne considère que des fibrés vectoriels sur L au sens de 7.3.4.

7.6.6. On appelle foncteur vectoriel (resp. en dimension finie) pour les isomorphismes la donnée pour tout espace de Banach V (resp. tout espace vectoriel de dimension finie sur K) d’un espace de Banach τ(V) et pour tout isomorphisme f de V sur un espace de Banach V’ d’un isomorphisme τ(f) de τ(V) sur τ(V’), ces données étant assujetties à la condition (a) de 7.6.1 et à la condition suivante :

(b’) L’application $f \mapsto \tau(f)$ du sous-ensemble ouvert de $\mathcal{L}(V; V')$ constitué par les isomorphismes de V sur V’, dans $\mathcal{L}(\tau(V); \tau(V'))$, est de classe $C^r$.

Les définitions et résultats des n°s précédents s’étendent au cas des foncteurs vectoriels pour les isomorphismes (en faisant $I_+ = \{1\}$ et $I_- = \varnothing$), à l’exception de ceux du premier alinéa du n° 7.6.3.

### 7.7. Sommes directes, fibrés d’applications multilinéaires, dual

7.7.1. On suppose que $I_- = \varnothing$. On définit un foncteur vectoriel σ appelé foncteur somme directe en posant $\sigma(\mathcal{V}) = \bigoplus_{i \in I} V_i$ et $\sigma(\mathfrak{f}) = \bigoplus_{i \in I} f_i$. Si $\mathcal{M} = (M^i)_{i \in I}$ est une famille de fibrés vectoriels de base B, le fibré vectoriel $\sigma(\mathcal{M})$ est appelé la somme directe des $M^i$ et est noté $\bigoplus_{i \in I} M^i$. Pour tout $b \in B$, la fibre en $b$ de $\bigoplus_{i \in I} M^i$ est la somme directe des fibres des $M^i$ en $b$.

Soit U un ouvert de B et soit $s_i \in \mathscr{F}_{M_i}(U)$ (pour $i \in I$). L’application $b \mapsto \sum_{i \in I} s_i(b)$ est alors une section, notée $\sum_i s_i$, de classe $C^r$ de $M = \bigoplus_{i \in I} M^i$ et l’application $(s_i)_{i \in I} \mapsto \sum_i s_i$ est un isomorphisme de $\mathscr{C}^r(U)$-modules de $\bigoplus_{i \in I} \mathscr{F}_{M_i}(U)$ sur $\mathscr{F}_M(U)$.

La variété sous-jacente à $\bigoplus_{i \in I} M^i$ s’identifie au produit fibré $\prod_B M^i$.

On désigne par $\mathrm{pr}_i$ le morphisme de fibrés vectoriels de $\bigoplus_{i \in I} M^i$ dans $M^i$ qui sur chaque fibre $\bigoplus_{i \in I} M^i_b$ est la i-ème projection. On définit de même l’injection canonique $j_i$ de $M^i$ dans $\bigoplus_{i \in I} M^i$.

Soit $f$ un morphisme de B dans une variété $B'$; soit H un second ensemble fini et soit $\mathcal{N} = (N^h)_{h \in H}$ une famille de fibrés vectoriels de base $B'$. L’application $u \to \bigoplus_{i \in I} (\mathrm{pr}_h \circ u \circ j_i)_{(h,i) \in H \times I}$ est une bijection de l’ensemble des $f$-morphismes de $\bigoplus_{i \in I} M^i$ dans $\bigoplus_{h \in H} N^h$ sur l’ensemble des matrices $(u_{h,i})_{(h,i) \in H \times I}$, où $u_{h,i}$ est un $f$-morphisme de $M^i$ dans $N^h$.

Si $I = \{1,2\}$, la suite
$$
0 \to M^{1} \xrightarrow{j_1} M^1 \oplus M^2 \xrightarrow{\mathrm{pr}_2} M^2 \to 0
$$
est exacte directe.

Inversement, soit $M$ un fibré vectoriel de base $B$ et soit $M'$ un sous-fibré vectoriel de $M$. Supposons que la variété $B$ soit paracompacte et que l’une des deux conditions suivantes soit satisfaite :
(i) $K$ est différent de $\mathbf{R}$ ou $\mathbf{C}$;
(ii) $K = \mathbf{R}, r \neq \omega$ et la variété $B$ admet des partitions de l’unité de classe $C^r$ (5.3.6).

Il existe alors un sous-fibré vectoriel $M''$ de $M$ tel que $M$ s’identifie à la somme directe $M' \oplus M''$.

7.7.2. Supposons que $I_+ = \{0\}$ et que $I_- = \{1,2,\ldots,d\}$. On définit un foncteur vectoriel $\eta_d$ de type $I$ et de classe $C^r$ en posant $\eta_d(\mathcal{V}) = \mathcal{L}(V_1,\ldots,V_d; V_0)$ et $\eta_d(f)(u) = f_0 \circ u \circ (f_1 \times \cdots \times f_d)$ pour $u \in \eta_d(\mathcal{V})$. Si $\mathcal{M} = (M_i)_{i \in I}$ est une famille de fibrés vectoriels de base $B$, le fibre vectoriel $\eta_d(\mathcal{M})$ se note $\mathcal{L}(M_1,\ldots,M_d; M_0)$.

Soit $u$ un morphisme multilinéaire de $M_1 \times_B \cdots \times_B M_d$ dans $M_0$. L’application $\hat{u} : b \mapsto u_b$ est alors une section de $\mathcal{L}(M_1,\ldots,M_d; M_0)$ et l’application $u \mapsto \hat{u}$ est bijective.

7.7.3. Gardons les notations de 7.7.2 et supposons de plus que $d = 1$. Le fibré vectoriel $\mathcal{L}(M_1; M_0)$ s’appelle alors le fibré des homomorphismes de $M_1$ dans $M_0$. Ses sections correspondent aux $B$-morphismes de $M_1$ dans $M_0$.

Si de plus $M_0$ est le fibré trivial $K_B$, le fibré vectoriel $\mathcal{L}(M_1; K_B)$ s’appelle le dual de $M = M_1$ et se note $M'$ : la fibre $(M')_b$ est l’espace des formes linéaires continues sur la fibre $M_b$ de $M$ au point $b \in B$.

Si $s$ (resp. $t$) est une section de $M$ (resp. $M'$) sur un ouvert $U$ de $B$, l’application $b \mapsto (b, \langle s(b), t(b) \rangle)$ est une section, notée $\langle s, t \rangle$ du fibré trivial $K_B$.$^1$

### 7.8. Fibrés d’applications multilinéaires alternées

Dans les nos 7.8.1 à 7.8.5, on suppose que $K$ est de caractéristique 0 ou que les fibrés vectoriels considérés sont de rang fini. On ignore si la définition du foncteur $\alpha_d$ donnée dans 7.8.1 peut se faire sans aucune restriction.

7.8.1. Prenons $I_+ = \{0\}, I_- = \{1\}$ et soit $d$ un entier $\geqslant 1$. On définit un

$^1$ Lorsque $M$ est de rang fini, on écrit $M^*$ au lieu de $M'$.

foncteur vectoriel $\alpha_d$ en désignant par $\alpha_d(\mathcal{V})$ l’espace de Banach des applications $d$-linéaires continues alternées de $V_1^d$ dans $V_0$ et en posant $\alpha_d(f)(u) = f_0 \circ u \circ f_1^d$ pour $u \in \alpha_d(\mathcal{V})$. Le fibré vectoriel $\alpha_d((M_1, M_0))$ se note $\mathrm{Alt}^d(M_1; M_0)$ et s’appelle le fibré vectoriel des applications $d$-linéaires alternées de $M_1$ dans $M_0$.

L’injection canonique de $\mathrm{Alt}^d(M_1; M_0)$ dans $\mathcal{L}(M_1, \ldots, M_1; M_0)$ est un morphisme de fibrés vectoriels ; $\mathrm{Alt}^d(M_1; M_0)$ est un sous-fibré vectoriel de $\mathcal{L}(M_1, \ldots, M_1; M_0)$.

On a $\mathrm{Alt}^1(M_1; M_0) = \mathcal{L}(M_1; M_0)$. On pose $\mathrm{Alt}^0(M_1; M_0) = M_0$.

Si $\omega$ est une section $^1$ de $\mathrm{Alt}^d(M_1; M_0)$ et si $s_1, \ldots, s_d$ sont des sections de $M_1$, il existe une section et une seule de $M_0$, notée $\omega(s_1, \ldots, s_d)$, telle que
$$
\omega(s_1, \ldots, s_d)(b) = \omega(b)(s_1(b), \ldots, s_d(b)) \quad \text{pour tout } b \in B.
$$

7.8.2 Soit $\varphi$ un accouplement de $N \times_B N'$ dans $N''$ (cf. n° 7.3.1) ; pour chaque $b$, on a une application bilinéaire $\varphi_b$ de $N_b \times N'_b$ dans $N''_b$ qui définit (cf. A, III, p. 142) une application bilinéaire de
$$
\mathrm{Alt}^d(M; N)_b \times \mathrm{Alt}^e(M; N')_b
$$
dans $\mathrm{Alt}^{d+e}(M; N'')_b$. La collection de ces applications bilinéaires définit un accouplement $u$ de
$$
\mathrm{Alt}^d(M; N) \times_B \mathrm{Alt}^e(M; N')
$$
dans $\mathrm{Alt}^{d+e}(M; N'')$; si $\omega$ et $\omega'$ sont respectivement des sections de $\mathrm{Alt}^d(M; N)$ et $\mathrm{Alt}^e(M; N')$ sur un ouvert $U$, la section $u(\omega, \omega')$ de $\mathrm{Alt}^{d+e}(M; N'')$ sur $U$ sera notée $\omega \wedge_\varphi \omega'$, et appelée le produit extérieur de $\omega$ et $\omega'$.
On a la formule :
(1) $$
(\omega \wedge_\varphi \omega')(s_1, \ldots, s_{d+e}) = \sum_\sigma \varepsilon_\sigma \varphi(\omega(s_{\sigma(1)}, \ldots, s_{\sigma(d)}), \omega'(s_{\sigma(d+1)}, \ldots, s_{\sigma(d+e)}))
$$
où les $s_i$ sont des sections de $M$ sur $U$, et où la sommation est étendue aux permutations $\sigma$ de $\{1, 2, \ldots, d+e\}$ telles que
$$
\sigma(1) < \cdots < \sigma(d) \quad \text{et} \quad \sigma(d+1) < \cdots < \sigma(d+e).
$$

7.8.3. Soient $M$ un fibré vectoriel et $A$ un fibré en algèbres, de base $B$. Supposons que les fibres $A_b$ de $A$ soient des algèbres associatives et commutatives, possédant un élément unité, noté $e_b$. Pour tout ouvert $U$ de $B$, nous noterons $\Omega^d(U)$ le $\mathcal{C}^r(U)$-module formé des sections du fibré $\mathrm{Alt}^d(M; A)$ et $\Omega^*(U)$ la somme directe des $\Omega^d(U)$ pour $d \geq 0$. Les multiplications sur chaque fibre définissent un accouplement de $A \times_B A$ dans $A$, d’où (7.8.2) une structure d’algèbre graduée sur $\Omega^*(U)$, qui est associative et anticommutative. La sous-algèbre $\Omega^0(U)$ est l’algèbre des

¹ Le lecteur aura soin de ne pas confondre cet emploi de la lettre $\omega$ avec celui défini p. 10.

sections de A. Un élément $\omega$ de $\Omega^1(U)$ s'identifie à un U-morphisme de $M|U$ dans $A|U$ (7.7.3): si $s \in \mathcal{S}'_M(U)$, nous noterons $\langle \omega, s \rangle$ la section $\omega(s)$ de A (7.4.2). Soient $s_j \in \mathcal{S}'_M(U)$ et $\omega_j \in \Omega^1(U)$ (pour $1 \leq j \leq d$); on a:

(2) $$
\omega(s_1, \ldots, s_d) = \det(\langle \omega_i, s_j \rangle) \quad \text{pour } \omega = \omega_1 \wedge \ldots \wedge \omega_d.
$$

7.8.4. Soit $d \geq 1$. Il existe un accouplement $i$ de $M \times_B \mathrm{Alt}^d(M; A)$ dans $\mathrm{Alt}^{d-1}(M; A)$ dont la restriction à chaque fibre est donnée par le produit intérieur droit (cf. A, III, p. 156). Si $s$ est une section de $M$ sur l'ouvert $U$ et si $\omega \in \Omega^d(U)$, on note $i(s)\omega$ la section $i(s, \omega)$ de $\mathrm{Alt}^{d-1}(M; A)$ sur $U$; on pose $i(s)\omega = 0$ pour $\omega$ dans $\Omega^0(U)$.

On associe ainsi à toute section $s$ de $M$ sur $U$ un endomorphisme du $\mathcal{C}'(U)$-module $\Omega^*(U)$. On a le formulaire:

(3) $$(i(s)\omega)(s_1, \ldots, s_{d-1}) = \omega(s, s_1, \ldots, s_{d-1}) \quad \text{pour } \omega \in \Omega^d(U), d \geq 1$$
(4) $$i(s) \circ i(s) = 0$$
(5) $$i(s)\omega = \langle \omega, s \rangle \quad \text{pour } \omega \in \Omega^1(U)$$
(6) $$i(s) . (\omega \wedge \omega') = i(s)\omega \wedge \omega' + (-1)^d \omega \wedge i(s)\omega' \quad \text{pour } \omega \in \Omega^d(U)$$
(7) $$i(s)(\omega_1 \wedge \ldots \wedge \omega_p) = \sum_{i=1}^p (-1)^{i+1} \langle \omega_i, s \rangle \omega_1 \wedge \ldots \wedge \hat{\omega}_i \wedge \ldots \wedge \omega_d.$$

Dans la dernière formule, les $\omega_i$ sont dans $\Omega^1(U)$ et le signe $\hat{}$ indique que le symbole qu'il surmonte doit être omis.

Toutes les opérations décrites ci-dessus sur les sections sont multilinéaires sur l'anneau $\mathcal{C}'(U; K)$.

7.8.5. Soit L une algèbre de Banach sur K. Les définitions et résultats des n° 7.7 et 7.8 s'étendent au cas des fibrés vectoriels sur L : on définit de manière analogue les fibrés d'applications L-multilinéaires ou L-multilinéaires alternées.

### 7.9. Produits tensoriels, espaces tensoriels, algèbre extérieure

On garde les notations de 7.6. De plus, on désigne par L un corps commutatif muni d'une structure de K-algèbre de dimension finie et on appelle fibré vectoriel un fibré vectoriel sur L, de base B et de rang localement fini.

7.9.1. Supposons que $I_- = \varnothing$. Si $\mathcal{V}$ et $\mathcal{V}'$ sont deux familles indexées par I d'espaces vectoriels de dimension finie sur L, on désigne par $\tau(\mathcal{V})$ le produit tensoriel des $V_i$ pour $i \in I$ (A, II, p. 71) et si $f \in \mathrm{Hom}(\mathcal{V}, \mathcal{V}')$, on pose $\tau(f) = \otimes f_i$. On définit ainsi un foncteur vectoriel sur L en dimension finie et si $\mathcal{M} = (M_i)_{i \in I}$ est une famille de fibrés vectoriels, on désigne par $\bigotimes_{i \in I} M_i$ et on appelle produit tensoriel (sur L) des $M_i$ le fibré vectoriel $\tau(\mathcal{M})$.

Si $s_i$ est une section de $M_i$ sur l’ouvert U de B (pour $i \in I$), l’application $b \mapsto \bigotimes_{i \in I} s_i(b)$ est une section de $\bigotimes_{i \in I} M_i$, notée $\bigotimes_{i \in I} s_i$. L’application $(s_i)_{i \in I} \mapsto \bigotimes_{i \in I} s_i$ est multilinéaire sur l’anneau $\mathcal{C}^r(U;L)$.

7.9.2. Les isomorphismes canoniques définis dans Alg., chap. II fournissent des isomorphismes de foncteurs vectoriels. Il en résulte d’après 7.6.4 des isomorphismes de fibrés vectoriels. Par exemple, on a des isomorphismes canoniques :

$$
(M_1 \oplus M_2) \otimes M_3 \longrightarrow (M_1 \otimes M_3) \oplus (M_2 \otimes M_3)
$$
$$
M_1^* \otimes M_2 \longrightarrow \mathcal{L}(M_1; M_2)
$$

etc.

7.9.3. Soit M un fibré vectoriel et soient I et J deux ensembles finis disjoints. Le fibré tensoriel $T^I_J(M)$ est défini comme le produit tensoriel $\bigotimes_{\alpha \in I \cup J} M_\alpha$, où $M_\alpha = M$ si $\alpha \in I$, et $M_\alpha = M^*$ si $\alpha \in J$, $M^*$ désignant le dual de M (A, III, p. 63). La fibre $T^I_J(M)_b$ de ce fibré en un point $b$ est égale à l’espace tensoriel $T^I_J(M_b)$ défini en Alg., loc. cit. Lorsque $I = \{1, \ldots, p\}$ et $J = \{p+1, \ldots, p+q\}$, on écrit $T^p_q(M)$ au lieu de $T^I_J(M)$; on a
$$
T^p_q(M) = (\bigotimes^p M) \otimes (\bigotimes^q M^*).
$$
La donnée d’un ordre total sur I et sur J définit un isomorphisme canonique de $T^I_J(M)$ sur $T^p_q(M)$.

7.9.4. Si I (resp. J) est réunion de deux sous-ensembles disjoints I' et I'' (resp. J' et J''), $T^I_J(M)$ s’identifie canoniquement au produit tensoriel $T^{I'}_{J'}(M) \otimes T^{I''}_{J''}(M)$. En particulier, si $s'$ (resp. $s''$) est une section de $T^{I'}_{J'}(M)$ (resp. de $T^{I''}_{J''}(M)$), le produit tensoriel $s' \otimes s''$ s’identifie à une section de $T^I_J(M)$.

7.9.5. Le dual de $T^I_J(M)$ s’identifie à $T^J_I(M)$.

7.9.6. Soient $i \in I$ et $j \in J$. Pour tout $b \in B$, l’homomorphisme de contraction des indices $i$ et $j$ est défini (cf. Alg., loc. cit.); c’est un homomorphisme $(c^i_j)_b : T^I_J(M_b) \to T^{I-\{i\}}_{J-\{j\}}(M_b)$. La collection des $(c^i_j)_b$ définit un morphisme d’espaces fibrés vectoriels
$$
c^i_j : T^I_J(M) \to T^{I-\{i\}}_{J-\{j\}}(M),
$$

appelé encore contraction des indices $i$ et $j$. On définit de même la contraction des indices $i_1, \ldots, i_k$ de $I$ avec les indices $j_1, \ldots, j_k$ de $J$.

7.9.7. Soit $d$ un entier $\geqslant 0$; soient $V$ et $V'$ deux espaces vectoriels de dimension finie sur $L$ et $f \in \mathrm{Hom}_L(V, V')$; posons $\lambda_d(V) = \bigwedge^d(V)$ et $\lambda_d(f) = \bigwedge^d(f)$. On définit ainsi un foncteur vectoriel sur $L$ en dimension finie et, si $M$ est un fibré vectoriel, on note $\bigwedge^d(M)$ et on appelle puissance extérieure $d$-ème de $M$ (sur $L$) le fibré vectoriel $\lambda_d(M)$.

L’application canonique de $\bigotimes^d V$ sur $\bigwedge^d(V)$ définit un morphisme de foncteurs vectoriels, d’où un morphisme, dit canonique, de $\bigotimes^d M$ dans $\bigwedge^d(M)$. Ce morphisme est surjectif.

Les isomorphismes canoniques de l’espace des applications $d$-multilinéaires alternées sur l’espace $\bigwedge^d(V^*)$ ou sur $(\bigwedge^d(V))^*$ fournissent des isomorphismes, dits canoniques, du fibré vectoriel $\mathrm{Alt}^d(M; L)$ des applications $d$-multilinéaires alternées sur $L$, sur le fibré vectoriel $\bigwedge^d(M^*)$ ou sur $(\bigwedge^d(M))^*$.

7.9.8. Posons maintenant $\lambda(V) = \bigwedge(V)$ et $\lambda(f) = \bigwedge(f)$; on définit encore ainsi un foncteur vectoriel sur $L$ en dimension finie. Le fibré vectoriel $\lambda(M)$ se note $\bigwedge(M)$. Sa fibre $\bigwedge(M)_b$ en $b \in B$ est l’algèbre extérieure (sur $L$) de la fibre $M_b$. Le fibré vectoriel $\bigwedge(M)$ est un fibré vectoriel en algèbres localement trivial.

Les définitions et propriétés des produits intérieurs données en Alg., chap. III, 3e éd., § 10 s’étendent immédiatement aux sections des fibrés vectoriels $\bigwedge(M)$ et $\bigwedge(M^*)$ (cf. aussi les formules (1) à (7) des n° 7.8.2 à 7.8.4).

7.9.9. Soit $M$ un fibré vectoriel. Pour tout entier $n$, soit $B_n$ l’ensemble (ouvert) des points $b \in B$ tels que la dimension (sur $L$) de $M_b$ soit égale à $n$. Pour $b \in B_n$, posons $N_b = \bigwedge^n(M_b)$ et soit $N$ l’ensemble somme des $N_b$ pour $b \in B$. Il existe sur $N$ une structure de fibré vectoriel et une seule telle que l’application évidente de $N|B_n$ dans $\bigwedge^n(M)|B_n$ soit un isomorphisme pour tout $n$. Muni de cette structure, le fibré vectoriel $N$ de rang un en chaque point se note $\det(M)$.

### 7.10. Fibrés vectoriels et fibrés principaux

7.10.1. Soit $F$ un espace de Banach. On dit qu’un fibré vectoriel $M$ de base $B$ est pur de type $F$ si toutes les fibres $M_b$ de $M$ (pour $b \in B$) sont isomorphes (comme espaces de Banach) à $F$.

Soit $M$ un fibré vectoriel de base $B$ pur de type $F$ et soit $P$ la sous-variété ouverte du fibré vectoriel $\mathcal{L}(F_B; M)$ composée des couples $(b, u)$ où $b \in B$ et où $u$ est un isomorphisme de $F_b = F$ sur $M_b$. Le groupe $\mathrm{GL}(F)$ des automorphismes de $F$ opère à droite sur $P$ en posant $(b, u) \cdot g = (b, u \circ g)$ pour $(b, u) \in P$ et $g \in \mathrm{GL}(F)$. Notons $\pi_P$ l’application $(b, u) \mapsto b$ de P dans B. Le quadruplet $\lambda = (P, GL(F), B, \pi_P)$ (où $GL(F)$ est muni de sa structure canonique de variété de groupe (5.12.2)) est une fibration principale (6.2.1): on l’appelle la fibration des repères de M. L’application $((b, u), h) \mapsto u(h)$ de $P \times F$ dans M munit M d’une structure de fibré associé à $\lambda$, de fibre type F (6.5.1).

Lorsque $F = K^n$, on peut identifier un isomorphisme $u$ de F sur $M_b$ à la base de $M_b$ image par $u$ de la base canonique de $K^n$. L’espace fibré des repères de M s’identifie alors à la sous-variété ouverte de $M \times_B \ldots \times_B M$ formée des bases $(e_1, \ldots, e_n)$ des différentes fibres $M_b$.

Soit U un ouvert de B et soit $t = (U, \varphi, E)$ une carte vectorielle de M de domaine U, avec $E = F$. L’application $b \mapsto (b, t_b)$ est alors une section de P, notée $\tilde{t}$, et l’application $t \mapsto \tilde{t}$ est une bijection de l’ensemble des cartes vectorielles de M de la forme $(U, \varphi, F)$ sur l’ensemble des sections de P sur U.

7.10.2. Réciproquement, soit $\lambda = (Q, G, B, \pi_Q)$ une fibration principale et soit $\varphi$ un homomorphisme de variétés de groupe de G dans le groupe $GL(F)$ des automorphismes d’un espace de Banach F. Faisons opérer G à gauche sur F en posant $g . h = \varphi(g)(h)$ ($h \in F, g \in G$). Soit M un espace fibré associé à $\lambda$, de fibre type F, et soit $\rho : Q \times F \to M$ son application repère (6.5.1). Soit $\pi$ l’application de M dans B définie par
$$
\pi(\rho(q, h)) = \pi_Q(q) \quad (q \in Q \text{ et } h \in F).
$$
Soit s une section de Q sur un ouvert U de B; l’application
$$
\tilde{s} : (b, h) \mapsto (s(b), h)
$$
est alors une bijection de $U \times F$ sur $\pi^{-1}(U)$. Il existe sur le couple $(M, \pi)$ une structure de fibré vectoriel de base B et une seule pour laquelle les triplets $t_s = (U, \tilde{s}^{-1}, F)$ sont des cartes vectorielles (pour toute section s de Q). La structure de variété sous-jacente à cette structure est celle de l’espace fibré associé à $\lambda$.

Soit $q \in Q$; posons $b = \pi_Q(q)$ et soit $u$ l’isomorphisme de F sur $M_b$ défini par $u(h) = \rho(q, h)$ (pour $h \in F$). L’application $f : q \mapsto (b, u)$ est un B-morphisme de fibrations principales, compatible avec $\varphi$, de $(Q, G, B, \pi_Q)$ dans le fibré des repères $(P, GL(F), B, \pi_P)$ du fibré vectoriel M.

7.10.3. Reprenons les notations du n° 7.6. Pour tout $i \in I$, soit
$$
\lambda_i = (P_i, G_i, B, \pi_i)
$$
une fibration principale de base B et supposons que $G_i$ opère à gauche sur un espace de Banach $V_i$ au moyen d’un homomorphisme
$$
\varphi_i : G_i \to GL(V_i).
$$
Soit $M_i$ un espace fibré associé à $\lambda_i$ de fibre type $V_i$. Posons $\mathcal{M} = (M_i)_{i \in I}$ et $\mathcal{V} = (V_i)_{i \in I}$ et soit $\lambda$ la fibration principale produit des $\lambda_i$ au dessus de B (6.2.5). Posons $\hat{\lambda} = (\mathbf{P}, G, B, \pi_p)$, avec $G = \prod_{i \in I} G_i$.

Soit maintenant $\tau$ un foncteur vectoriel. Pour $g = (g_i) \in G$, soit $\varphi(g)$ l’élément de $\mathrm{Hom}(\mathcal{V}, \mathcal{V})$ défini par:

$$
\varphi(g)_i = \varphi_i(g_i) \quad \text{si } i \in I_+
$$
$$
\varphi(g)_i = \varphi_i(g_i)^{-1} \quad \text{si } i \in I_-
$$

Le groupe $G$ opère alors sur $\tau(\mathcal{V})$ au moyen du morphisme $g \mapsto \tau(\varphi(g))$ de $G$ dans $\mathbf{GL}(\tau(\mathcal{V}))$.

Soit d’autre part $x = (x_i)$ un point de $\mathbf{P}$ et soit $b = \pi_p(x)$. Pour chaque $i$, l’application $\theta_{x_i}$ définie au n° 6.5.2 est un isomorphisme de $V_i$ sur $(M_i)_b$. Soit $\theta_x$ l’élément de $\mathrm{Hom}(\mathcal{V}, ((M_i)_b)_{i \in I})$ défini par:

$$
(\theta_x)_i = \theta_{x_i} \quad \text{si } i \in I_+
$$
$$
(\theta_x)_i = \theta_{x_i}^{-1} \quad \text{si } i \in I_-
$$

Soit $\rho$ l’application $(x, h) \mapsto (b, \tau(\theta_x)(h))$ de $\mathbf{P} \times \tau(\mathcal{V})$ dans le fibré vectoriel $\tau(\mathcal{M})$; l’application $\rho$ munit $\tau(\mathcal{M})$ d’une structure d’espace fibré associé à $\lambda$ de fibre type $\tau(\mathcal{V})$.

Ces considérations se généralisent au cas de foncteurs vectoriels en dimension finie, ou de foncteurs vectoriels sur un corps $L$ muni d’une structure de K-algèbre de dimension finie.

### 7.11. Changement de structure

Les structures et opérations décrits dans ce paragraphe sont compatibles avec les changements de structure décrits aux numéros 5.13 et 5.14.
