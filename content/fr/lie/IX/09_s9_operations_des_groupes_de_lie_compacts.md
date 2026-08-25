---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: GROUPES DE LIE RÉELS COMPACTS
section: 9
section_title: Opérations des groupes de Lie compacts sur les variétés
lang: fr
source: lie-ix-fr
book_pages: LIE IX.88-LIE IX.99, LIE IX.128-LIE IX.132
pdf_pages: 0091-0102, 0131-0135
extraction: ocr
subsections:
    - "no": 1
      title: Plongement d'une variété au voisinage d'une partie compacte
      page: 88
      pdf_page: 91
    - "no": 2
      title: Le théorème de plongement équivariant
      page: 91
      pdf_page: 94
    - "no": 3
      title: Tubes et transversales
      page: 93
      pdf_page: 96
    - "no": 4
      title: Types d’orbites
      page: 95
      pdf_page: 98
statements: 19
exercises: 3
content_sha256: 4a92032670e9fc2442150f4089aaa919bb20e103a1988b1b3b09efe766298b79
---

## § 9. OPÉRATIONS DES GROUPES DE LIE COMPACTS SUR LES VARIÉTÉS

Dans ce paragraphe, on désigne par X une variété réelle de classe $C^r$ ($1 \leq r \leq \omega$), séparée et localement de dimension finie.

### 1. Plongement d'une variété au voisinage d'une partie compacte

#### Lemme 1 {#lie-ix-s9-lem-1 .statement tag=01HE}

Soient T et T' deux espaces topologiques, A et A' des parties compactes de T et T' respectivement, W un voisinage de A × A' dans T × T'. Il existe un voisinage ouvert U de A dans T et un voisinage ouvert U' de A' dans T' tels qu'on ait U × U' ⊂ W.

Soit $x \in A$; il existe des ouverts $U_x$ de T et $U'_x$ de T' tels que $\{ x \} \times A' \subset U_x \times U'_x \subset W$: en effet, on peut recouvrir la partie compacte $\{ x \} \times A'$ de T × T' par un nombre fini d'ouverts contenus dans W, de la forme $U_i \times U'_i$, avec $x \in U_i$; il suffit de prendre $U_x = \bigcap_i U_i$ et $U'_x = \bigcup_i U'_i$.

Puisque A est compact, il existe des points $x_1, ..., x_m$ de A tels que $A \subset \bigcup_i U_{x_i}$; posons $U = \bigcup_i U_{x_i}$ et $U' = \bigcap_i U'_{x_i}$. On a alors $A \times A' \subset U \times U' \subset W$, d'où le lemme.

Dans la suite de ce numéro, on désigne par Y une variété séparée de classe $C^r$.

#### Proposition 1 {#lie-ix-s9-prop-1 .statement tag=01HF}

Soient $\varphi : X \to Y$ un morphisme de classe $C^r$, A une partie compacte de X. Les conditions suivantes sont équivalentes :

(i) La restriction de $\varphi$ à A est injective, et $\varphi$ est une immersion en tout point de A ;
(ii) il existe un voisinage ouvert U de A tel que $\varphi$ induise un plongement de U dans Y.

Lorsque ces conditions sont réalisées, on dit que $\varphi$ est un plongement au voisinage de A.

Démontrons que (i) entraîne (ii), l'implication opposée étant évidente. Sous l'hypothèse (i), il existe un ouvert V de X contenant A tel que la restriction de $\varphi$ à V soit une immersion (VAR, R, 5.7.1). Notons $\Gamma$ l'ensemble des points (x, y) de V × V tels que $\varphi(x) = \varphi(y)$, et $\Delta$ la diagonale de V × V. Alors $\Delta$ est une partie ouverte de $\Gamma$ : en effet, pour tout $x \in V$, il existe un voisinage $U_x$ de x tel que la restriction de $\varphi$ à $U_x$ soit injective, c'est-à-dire que l'on ait $\Gamma \cap (U_x \times U_x) = \Delta \cap (U_x \times U_x)$.

Puisque Y est séparée, $\Gamma$ est fermé dans V × V ; par suite le complémentaire W de $\Gamma - \Delta$ dans V × V est ouvert. Par hypothèse, W contient A × A ; le lemme 1 entraîne qu'il existe un ouvert U' de V contenant A tel que $U' \times U' \subset W$, c'est-à-dire que la restriction de $\varphi$ à U' soit injective. De plus il existe un voisinage ouvert U de A dont l'adhérence est compacte et contenue dans U' (TG, I, p. 65, prop. 10). Alors $\varphi$ induit un homéomorphisme de $\overline{U}$ sur $\varphi(\overline{U})$, et par suite de U sur $\varphi(U)$; il en résulte que la restriction de $\varphi$ à U est un plongement (VAR, R, 5.8.3).

#### Proposition 2 {#lie-ix-s9-prop-2 .statement tag=01HG}

*Supposons la variété Y paracompacte ; soit A une partie de X, et soit $\varphi : X \to Y$ un morphisme de classe $C^r$ qui induit un homéomorphisme de A sur $\varphi(A)$, et qui est étale en tout point de A. Il existe alors un voisinage ouvert U de A tel que $\varphi$ induise un isomorphisme de U sur une sous-variété ouverte de Y.*

Quitte à restreindre X et Y, on peut supposer $\varphi$ étale et surjectif. Notons $\sigma : \varphi(A) \to A$ l’homéomorphisme réciproque de $\varphi|A$. Puisque Y est métrisable (VAR, R, 5.1.6), $\varphi(A)$ admet un système fondamental de voisinages paracompacts ; d’après TG, XI, il existe alors un voisinage ouvert V de $\varphi(A)$ dans Y et une application continue $s : V \to X$, qui coïncide avec $\sigma$ sur $\varphi(A)$, telle que $\varphi(s(y)) = y$ pour tout $y \in V$. De plus, $s$ est topologiquement étale, donc $s(V)$ est un ouvert U contenant A. Alors $\varphi$ induit un homéomorphisme $\varphi'$ de U sur V ; d’après VAR, R, 5.7.8, $\varphi'$ est un isomorphisme.

Dans la suite de ce numéro, on suppose $r \neq \omega$.

#### Proposition 3 {#lie-ix-s9-prop-3 .statement tag=01HH}

*Soit A une partie compacte de X. L’ensemble $\mathcal{P}$ des morphismes $\varphi \in \mathcal{C}^r(X;Y)$ qui sont des plongements au voisinage de A est ouvert dans $\mathcal{C}^r(X;Y)$ pour la topologie de la $C^r$-convergence compacte (\S 6, no 4).*

Il suffit évidemment de démontrer la proposition pour $r = 1$.

*a)* Montrons d’abord que la partie J de $\mathcal{C}^1(X;Y)$ formée des morphismes qui sont des immersions en tout point de A est ouverte. Considérons l’application $j_A : \mathcal{C}^1(X;Y) \times A \to J^1(X,Y)$ telle que $j_A(\varphi, x) = j_x^1(\varphi)$ (VAR, R, 12.1).

Par définition de la topologie de $\mathcal{C}^1(X;Y)$, l’application $\tilde{j}_A : \varphi \mapsto j_A(\varphi, .)$ de $\mathcal{C}^1(X;Y)$ dans $\mathcal{C}(A;J^1(X,Y))$ est continue ; on déduit alors de TG, X, p. 28, th. 3 que $j_A$ est continue.

D’autre part, soit M l’ensemble des jets $j$ de $J^1(X,Y)$ dont l’application tangente $T(j) : T_{s(j)}(X) \to T_{b(j)}(Y)$ (VAR, R, 12.3.4) est injective. L’ensemble M est ouvert dans $J^1(X,Y)$ : en effet, il suffit de vérifier cette assertion lorsque X est un ouvert d’un espace vectoriel $\mathbf{E}$ de dimension finie, et Y un ouvert d’un espace de Banach F ; on est alors ramené (VAR, R, 12.3.1) à prouver que l’ensemble des applications linéaires continues injectives est ouvert dans $\mathcal{L}(E;F)$, ce qui résulte de TS, III, § 2, no 7, prop. 16.

On conclut de ce qui précède que l’ensemble $j_A^{-1}(M)$ est ouvert dans $\mathcal{C}^1(X;\overline{Y}) \times A$, donc que son complémentaire $\mathcal{F}$ est fermé. Puisque A est compact, la projection $\mathrm{pr}_1 : \mathcal{C}^1(X;Y) \times A \to \mathcal{C}^1(X;Y)$ est un morphisme propre, donc fermé ; par conséquent l’ensemble J, qui est égal à $\mathcal{C}^1(X;Y) - \mathrm{pr}_1(\mathcal{F})$, est ouvert dans $\mathcal{C}^1(X;Y)$.

*b)* Soit H le sous-ensemble de $J \times A \times A$ formé des éléments $(f, x, y)$ tels que $f(x) = f(y)$. Il est clair que H contient $J \times \Delta$, où $\Delta$ désigne la diagonale du produit $A \times A$ ; montrons que $H' = H - (J \times \Delta)$ est fermé dans $J \times A \times A$. Comme $\mathcal{P}$ est le complémentaire dans J de l’image de H’ par la projection propre $\mathrm{pr}_1 : J \times A \times A \to J$, cela entraînera la proposition.

La topologie de $C^1(X; Y)$ étant plus fine que la topologie de la convergence compacte, l’application $(\varphi, x) \mapsto \varphi(x)$ de $C^1(X, Y) \times A$ dans $Y$ est continue (TG, X, p. 28, cor. 1); on en déduit que $H$ est fermé dans $J \times A \times A$. Il suffit donc de montrer que $J \times \Delta$ est ouvert dans $H$, autrement dit que pour tout $\varphi \in J$ et tout $x \in A$, il existe un voisinage $\Omega$ de $\varphi$ dans $J$ et un voisinage $B$ de $x$ dans $X$ tels que pour tout morphisme $\psi$ de $\Omega$, la restriction de $\psi$ à $A \cap B$ soit injective.

La proposition résulte donc du lemme suivant :

#### Lemme 2 {#lie-ix-s9-lem-2 .statement tag=01HI}

*Soient $x$ un point de $X$, $\varphi : X \to Y$ un morphisme de classe $C^1$ qui est une immersion en $x$. Il existe un voisinage $\Omega$ de $\varphi$ dans $C^1(X; Y)$ et un voisinage $B$ de $x$ dans $X$ tels que pour tout $\psi \in \Omega$, la restriction de $\psi$ à $B$ soit injective.*

Soit $U$ un voisinage ouvert de $x$, relativement compact, isomorphe à un espace vectoriel de dimension finie, et tel que $\varphi(\overline{U})$ soit contenu dans un domaine de carte $V$. L’ensemble $\Omega_0$ des $\psi \in C^1(X; Y)$ tels que $\psi(\overline{U}) \subset V$ est ouvert dans $C^1(X; Y)$, et l’application de restriction $\Omega_0 \to C^1(U; V)$ est continue ; on est donc ramené à démontrer le lemme pour $X = U$ et $Y = V$, autrement dit on peut supposer que $X$ est un espace vectoriel de dimension finie et $Y$ un espace de Banach. Choisissons des normes sur $X$ et $Y$.

L’application linéaire $D\varphi(x) : X \to Y$ est injective ; notons $q$ sa conorme (TS, III, § 2, n° 6), de sorte qu’on a par définition $\| D\varphi(x).t \| \geq q \| t \|$ pour tout $t \in X$. Soit $\varepsilon \in \mathbf{R}$ tel que $0 < \varepsilon < q/2$, et soit $B$ une boule fermée de centre $x$ telle qu’on ait $\| D\varphi(u) - D\varphi(x) \| \leq \varepsilon$ pour tout $u \in B$. Notons $\Omega$ le sous-ensemble de $C^1(X; Y)$ formé des morphismes $\psi$ tels que $\| D\psi(u) - D\varphi(u) \| \leq \varepsilon$ pour tout $u \in B$ ; il est ouvert par définition de la topologie de $C^1(X; Y)$. Pour $\psi \in \Omega$, posons $\psi_0 = \psi - D\varphi(x)$. On a $\| D\psi_0(u) \| \leq 2\varepsilon$ pour tout $u \in B$, et par conséquent $\| \psi_0(u) - \psi_0(v) \| \leq 2\varepsilon \| u - v \|$ quels que soient $u$ et $v$ dans $B$ (VAR, R, 2.2.3). On en déduit

$$
\| \psi(u) - \psi(v) \| \geq \| D\varphi(x).(u - v) \| - \| \psi_0(u) - \psi_0(v) \| \geq (q - 2\varepsilon) \| u - v \|.
$$

Par suite la restriction de $\psi$ à $B$ est injective, d’où le lemme.

#### Proposition 4 {#lie-ix-s9-prop-4 .statement tag=01HJ}

*Soit $A$ une partie compacte de $X$. Il existe un espace vectoriel $E$ de dimension finie et un morphisme $\varphi \in C^r(X; E)$ ($r \neq \omega$) qui est un plongement au voisinage de $A$.

Soit $(U_i, \varphi_i, E_i)_{i \in I}$ une famille finie de cartes de $X$ dont les domaines recouvrent $A$. On convient d’étendre $\varphi_i$ en une application de $X$ dans $E_i$ (encore notée $\varphi_i$) en posant $\varphi_i(x) = 0$ pour $x \notin U_i$. Soit $(V_i)_{i \in I}$ un recouvrement de $A$ par des ouverts de $X$, tel que $\overline{V_i} \subset U_i$ pour tout $i \in I$ (l’existence d’un tel recouvrement résulte du cor. 1 de TG, IX, p. 48, appliqué à l’espace compact $X'$ obtenu en adjoignant à $X$ un point à l’infini et au recouvrement de $X'$ formé par les ouverts $U_i$ ($i \in I$) et $X' - A$). Pour tout $i \in I$, soit $\alpha_i$ une fonction numérique de classe $C^r$ sur $X$, égale à 1 en tout point de $V_i$, et de support contenu dans $U_i$ (VAR, R, 5.3.6.).

Considérons l’application $\varphi : X \to \bigoplus_{i \in I} (E_i \oplus \mathbf{R})$ définie par

$$
\varphi(x) = (\alpha_i(x) \varphi_i(x), \alpha_i(x))_{i \in I}.
$$

Pour tout $i \in I$, l’application $\alpha_i \varphi_i$ est de classe $C^r$ (puisque ses restrictions à $U_i$ et au complémentaire du support de $\alpha_i$ le sont), et sa restriction à $V_i$ est un plongement ; il en résulte que $\varphi$ est un morphisme de classe $C^r$ et est une immersion en tout point de $A$. Montrons que la restriction de $\varphi$ à $A$ est injective. Soient $x, y$ deux points de $A$ tels que $\varphi(x) = \varphi(y)$, et soit $i \in I$ tel que $x \in V_i$. On a alors $\alpha_i(x) = 1$, donc $\alpha_i(y) = 1$, ce qui entraîne $y \in U_i$; mais on a aussi $\varphi_i(x) = \varphi_i(y)$, d’où $x = y$ puisque $\varphi_i$ induit un plongement de $U_i$ dans $E_i$.

On peut démontrer $^1$ que toute variété séparée dénombrable à l’infini de dimension pure $n$ se plonge dans $\mathbf{R}^{2n}$; pour un résultat moins fort, cf. exercice 2.

### 2. Le théorème de plongement équivariant

Dans ce numéro, on suppose $r \neq \omega$.

#### Lemme 3 {#lie-ix-s9-lem-3 .statement tag=01HK}

Soit $G$ un groupe topologique compact opérant continûment sur un espace topologique $X$; soient $A$ une partie de $X$, stable par $G$, et $W$ un voisinage de $A$. Il existe alors un voisinage ouvert $V$ de $A$ stable par $G$ et contenu dans $W$.

Posons $F = X - W$ et $V = X - GF$. Alors $V$ est ouvert (TG, III, p. 28, cor. 1), stable par $G$, et on a $A \subset V \subset W$.

#### Théorème 1 {#lie-ix-s9-thm-1 .statement tag=01HL}

Soient $G$ un groupe de Lie compact, $(g, x) \mapsto gx$ une loi d’opération à gauche de classe $C^r$ de $G$ dans $X$, et $A$ une partie compacte de $X$. Il existe une représentation linéaire analytique $\rho$ de $G$ dans un espace vectoriel $E$ de dimension finie, un morphisme $\varphi : X \to E$ de classe $C^r$, compatible avec les opérations de $G$, et un voisinage ouvert $U$ de $A$, stable par $G$, tels que la restriction de $\varphi$ à $U$ soit un plongement.

Remplaçant $A$ par la partie compacte $GA$, on se ramène au cas où $A$ est stable par $G$.

Soit $E_0$ un espace vectoriel de dimension finie tel qu’il existe un élément de $\mathscr{C}^r(X; E_0)$ qui soit un plongement au voisinage de $A$ (no 1, prop. 4); l’ensemble $\mathcal{P}$ des morphismes possédant cette propriété est donc un ouvert non vide de $\mathscr{C}^r(X; E_0)$ (no 1, prop. 3). Considérons la représentation linéaire continue du groupe compact $G$ dans l’espace $\mathscr{C}^r(X; E_0)$ (\$ 6, no 4, lemme 4). D’après le théorème de Peter-Weyl (TS, à paraître), la réunion des sous-espaces de dimension finie, stables par $G$, est dense dans $\mathscr{C}^r(X; E_0)$; il existe donc un élément $\varphi_0$ de $\mathcal{P}$ tel que les applications $x \mapsto \varphi_0(gx)$, pour $g \in G$, engendrent un sous-espace vectoriel $E_1$ de *dimension finie* de $\mathscr{C}^r(X; E_0)$, évidemment stable pour l’action de $G$.

Prenons alors pour $E$ l’espace $\mathrm{Hom}_{\mathbf{R}}(E_1, E_0)$, pour $\rho$ la représentation de $G$ dans $E$ déduite de l’action sur $E_1$, et pour $\varphi : X \to E$ l’application qui à $x \in X$ associe l’application linéaire $\psi \mapsto \psi(x)$ de $E_1$ dans $E_0$. C’est un morphisme de classe $C^r$; pour $x \in X, g \in G, \psi \in E_1$, on a (en notant $\tau(g)$ l’automorphisme $x \mapsto gx$ de $X$) :

$$
\varphi(gx)(\psi) = \psi(gx) = \varphi(x)(\psi \circ \tau(g)) = (\rho(g)\varphi(x))(\psi).
$$

$^1$ Voir H. Whitney, The self-intersection of a smooth $n$-manifold in $2n$-space, Ann. of Math., 45 (1944), 220-246.

Soit $\alpha : \mathrm{Hom}_{\mathbf{R}}(E_1, E_0) \to E_0$ l’application linéaire $u \mapsto u(\varphi_0)$; on a $\alpha \circ \varphi = \varphi_0$, de sorte que $\varphi$ est un plongement au voisinage de $A$ puisque $\varphi_0$ en est un. Il existe donc un voisinage ouvert $U$ de $A$ tel que la restriction de $\varphi$ à $U$ soit un plongement ; on peut choisir $U$ stable par $G$ d’après le lemme 3, d’où le théorème.

#### Corollaire 1 {#lie-ix-s9-thm-1-cor-1 .statement tag=01HM}

Supposons $X$ compacte. Il existe une représentation linéaire analytique $\rho$ de $G$ dans un espace vectoriel $E$ de dimension finie et un plongement $\varphi : X \to E$ tels que $\varphi(gx) = \rho(g) \varphi(x)$ pour $g \in G, x \in X$.

#### Corollaire 2 {#lie-ix-s9-thm-1-cor-2 .statement tag=01HN}

Soit $H$ un sous-groupe fermé de $G$. Il existe une représentation linéaire analytique de $G$ dans un espace vectoriel $E$ de dimension finie et un point $v \in E$ de fixateur $H$.

Appliquons le cor. 1 à l’opération canonique de $G$ sur la variété compacte $G/H$. On obtient alors une représentation linéaire analytique $\rho : G \to \mathrm{GL}(E)$, et un plongement $\varphi : G/H \to E$ tels que $\varphi(gx) = \rho(g) \varphi(x), g \in G, x \in G/H$. Soient $\overline{e} \in G/H$ la classe de $e \in G$, et $v = \varphi(\overline{e})$ son image. Pour tout $g \in G$, on a $\rho(g) v = v \iff \varphi(g \overline{e}) = \varphi(\overline{e}) \iff g \overline{e} = \overline{e} \iff g \in H$.

#### Corollaire 3 {#lie-ix-s9-thm-1-cor-3 .statement tag=01HO}

Supposons $X$ paracompacte. Il existe un espace hilbertien réel $E$, une représentation unitaire continue $^1 \rho$ de $G$ dans $E$ et un plongement $\varphi : X \to E$ de classe $C^r$, tels qu’on ait $\varphi(gx) = \rho(g) \varphi(x)$ pour tout $g \in G$ et tout $x \in X$.

L’espace $X/G$ est localement compact (TG, III, p. 33, prop. 11). Ses composantes connexes sont les images des composantes connexes de $X$, qui sont dénombrables à l’infini (TG, I, p. 70, th. 5) ; elles sont donc elles-mêmes dénombrables à l’infini, ce qui entraîne que $X/G$ est paracompact (loc. cit.). Il existe donc un recouvrement localement fini $(U'_\alpha)_{\alpha \in I}$ de $X/G$ par des ouverts relativement compacts, et un recouvrement $(V'_\alpha)_{\alpha \in I}$ tel que $\overline{V}'_\alpha \subset U'_\alpha$ pour tout $\alpha \in I$ (TG, IX, p. 48, cor. 1) ; par image réciproque, on en déduit deux recouvrements localement finis $(U_\alpha)_{\alpha \in I}$ et $(V_\alpha)_{\alpha \in I}$ de $X$ par des ouverts relativement compacts stables par $G$, tels que $\overline{V}_\alpha \subset U_\alpha$ pour tout $\alpha \in I$.

Pour tout $\alpha \in I$, il existe une représentation $\rho_\alpha$ de $G$ dans un espace vectoriel réel $E_\alpha$ de dimension finie et un morphisme $\varphi_\alpha \in \mathscr{C}^r(X; E_\alpha)$, compatible aux opérations de $G$, dont la restriction à $U_\alpha$ est un plongement (th. 1). Pour $\alpha \in I$, soit $a_\alpha$ une fonction numérique de classe $C^r$ sur $X$, égale à 1 sur $V_\alpha$ et à 0 en dehors de $U_\alpha$ (VAR, R, 5.3.6).

Posons $b_\alpha(x) = \int_G a_\alpha(gx) \, dx$ pour $x \in X$. La fonction $b_\alpha$ est de classe $C^r$, invariante par $G$ (\S 6, n° 4, cor. 2), égale à 1 sur $V_\alpha$ et à 0 en dehors de $U_\alpha$. Munissons chaque $E_\alpha$ d’un produit scalaire hilbertien invariant par $G$ (\S 1, n° 1), et $R$ de sa structure hilbertienne canonique ; soit $E$ l’espace somme hilbertienne de la famille $(E_\alpha \oplus R)_{\alpha \in I}$, et soit $\rho$ la représentation de $G$ dans $E$ déduite des $\rho_\alpha$ et de l’action triviale de $G$ sur $R$.

$^1$ C’est-à-dire (TS, à paraître) une représentation linéaire continue (INT, VIII, § 2, n° 1) telle que l’opérateur $\rho(g)$ soit unitaire pour tout $g \in G$.

Pour $x \in X$, posons $\varphi(x) = (b_\alpha(x)\ \varphi_\alpha(x),\ b_\alpha(x))_{\alpha \in I}$. Alors $\varphi$ est un morphisme de classe $C^r$ de $X$ dans $E$, compatible avec les opérations de $G$; on vérifie comme dans la démonstration de la prop. 4 (n° 1) que $\varphi$ est un plongement, ce qui entraîne le corollaire.

### 3. Tubes et transversales

#### Lemme 4 {#lie-ix-s9-lem-4 .statement tag=01HP}

Soient $H$ un groupe de Lie compact, $\rho : H \to GL(V)$ une représentation continue (donc analytique) de $H$ dans un espace vectoriel réel de dimension finie, $W$ un voisinage de l’origine dans $V$. Il existe un voisinage ouvert de l’origine $B$, contenu dans $W$, stable par $H$, et un isomorphisme analytique $u : V \to B$, compatible aux opérations de $H$, tel que $u(0) = 0$ et $Du(0) = \mathrm{Id}_V$.

Choisissons un produit scalaire sur $V$ invariant par $H$ (\$ 1, n° 1). Il existe un nombre réel $r > 0$ tel que la boule ouverte $B$ de rayon $r$ soit contenue dans $W$; elle est évidemment stable par $H$. Posons $u(v) = r(r^2 + \|v\|^2)^{-1/2} v$ pour tout $v \in V$; alors $u$ est une application analytique bijective de $V$ dans $B$, compatible avec les opérations de $H$, et son application réciproque $w \mapsto r(r^2 - \|w\|^2)^{-1/2} w$ est analytique. On a de plus $u(0) = 0$ et $Du(0) = \mathrm{Id}_V$.

#### Proposition 5 {#lie-ix-s9-prop-5 .statement tag=01HQ}

Soient $H$ un groupe de Lie compact, $(h, x) \mapsto hx$ une loi d’opération à gauche de classe $C^r$ de $H$ dans $X$, $x$ un point de $X$ fixe sous l’action de $H$. Le groupe $H$ opère alors linéairement sur l’espace vectoriel $T = T_x(X)$; il existe un plongement ouvert $\varphi : T \to X$ de classe $C^r$, compatible avec les opérations de $H$, tel que $\varphi(0) = x$ et que $T_0(\varphi)$ soit l’application identique de $T$.

Soit $(U, \psi, E)$ une carte de $X$ en $x$, telle que $U$ soit stable par $H$ (n° 2, lemme 3) et qu’on ait $\psi(x) = 0$. Identifions $E$ à $T$ par $T_x(\psi)$, et posons

$$
\psi^\#(y) = \int_H h.\psi(h^{-1}y)\ dh \quad \text{pour} \quad y \in U,
$$

où $dh$ est la mesure de Haar sur $H$ de masse totale 1.

Alors (\$ 6, n° 4, cor. 1) $\psi^\#$ est un morphisme de classe $C^r$ de $U$ dans $T$, compatible avec les opérations de $H$, tel que $\psi^\#(x) = 0$ et $d_x \psi^\# = \mathrm{Id}_T$. Il existe donc un ouvert $U' \subset U$ contenant $x$, et un voisinage ouvert $V$ de 0 dans $T$, tels que $\psi^\#$ induise un isomorphisme $\theta : U' \to V$. Quitte à restreindre $U'$ et $V$, on peut supposer qu’ils sont stables par $H$ et qu’il existe un isomorphisme $u : T \to V$ compatible aux opérations de $H$ (lemme 4). Il suffit alors de prendre $\varphi = \theta^{-1} \circ u$.

Rappelons (VAR, R, 6.5.1) que si $G$ est un groupe de Lie, $H$ un sous-groupe de Lie de $G$ et $Y$ une variété dans laquelle $H$ opère à gauche, on note $G \times^H Y$ le quotient de la variété produit $G \times Y$ par l’opération à droite $((g, y), h) \mapsto (gh, h^{-1}y)$ de $H$; c’est une variété dans laquelle le groupe de Lie $G$ opère naturellement à gauche ; la projection $G \times^H Y \to G/H$ est une fibration de fibre $Y$. Si de plus $Y$ est un espace vectoriel de dimension finie sur lequel $H$ opère linéairement, $G \times^H Y$ est muni d'une structure naturelle de $G$-fibré vectoriel de base $G/H$ (VAR, R, 7.10.2).

Soit $G$ un groupe de Lie opérant proprement sur la variété $X$ (TG, III, p. 27, déf. 1) de façon que la loi d'opération $(g, x) \mapsto gx$ soit de classe $C^r$. Pour tout point $x$ de $X$, l'orbite $Gx$ de $x$ est alors une sous-variété fermée de $X$, isomorphe à l'espace homogène de Lie $G/G_x$, où $G_x$ est le fixateur de $x$ dans $G$ (cf. III, § 1, no 7, prop. 14, (ii), et TG, III, p. 29, prop. 4); celui-ci est un groupe de Lie compact (loc. cit.).

#### Proposition 6 {#lie-ix-s9-prop-6 .statement tag=01HR}

*Supposons la variété $X$ paracompacte; soient $x$ un point de $X$, $G_x$ son fixateur.* Il existe une représentation linéaire analytique de dimension finie $\tau : G_x \to \mathbf{GL}(W)$, et un plongement ouvert $\alpha : G \times^{G_x} W \to X$ de classe $C^r$, compatible avec les opérations de $G$, qui applique la classe de $(e, 0) \in G \times W$ sur $x$.

Posons $T = T_x(X)$. Soit $W$ un sous-espace de $T$, stable par $G_x$, supplémentaire de $T_x(Gx)$ dans $T$ (par exemple l'orthogonal de $T_x(Gx)$ relativement à un produit scalaire sur $T$ invariant par $G_x$). Soit d'autre part $\varphi : T \to X$ un morphisme possédant les propriétés énoncées dans la prop. 5 (relativement à $H = G_x$). Considérons le morphisme $\lambda : G \times W \to X$ défini par $\lambda(g, w) = g\varphi(w)$. Il induit par passage au quotient un morphisme $\mu : G \times^{G_x} W \to X$ de classe $C^r$, compatible avec les opérations de $G$, qui applique la classe $z$ de $(e, 0)$ sur $x$.

Montrons que $\mu$ est étale au point $z$. On a

$$
\dim(G \times^{G_x} W) = \dim(G) + \dim(W) - \dim(G_x) = \dim(Gx) + \dim(W) = \dim(T),
$$

et il suffit donc de montrer que $\mu$ est submersif en $z$, ou encore que $\lambda$ est submersif en $(e, 0)$. Or, l'application tangente $T_{(e,0)}(\lambda) : T_e(G) \oplus W \to T$ est égale à $T_e(\rho(x)) + i$, où $\rho(x)$ est l'application orbitale $g \mapsto gx$ et $i$ l'injection canonique de $W$ dans $T$; comme on a $\operatorname{Im} T_e(\rho(x)) = T_x(Gx)$, l'application $T_{(e,0)}(\lambda)$ est surjective, et $\mu$ est étale en $z$.

Nous allons démontrer qu'il existe un voisinage ouvert $\Omega$ de $Gz$ dans $G \times^{G_x} W$, stable par $G$, tel que $\mu$ induise un isomorphisme de $\Omega$ sur un ouvert de $X$. Cela entraînera la proposition : en effet, l'image réciproque de $\Omega$ dans $G \times W$ est stable par $G$, donc de la forme $G \times B$, où $B$ est un ouvert de $W$ contenant l'origine et stable par $G_x$; quitte à restreindre $\Omega$, on peut supposer qu'il existe un isomorphisme $u : W \to B$, compatible aux opérations de $G_x$ (lemme 4). Il est clair que le morphisme composé

$$
\alpha : G \times^{G_x} W \xrightarrow{(\mathrm{Id},u)} G \times^{G_x} B \xrightarrow{\mu} X
$$

satisfait aux conditions de l'énoncé.

La proposition résulte donc du lemme suivant :

#### Lemme 5 {#lie-ix-s9-lem-5 .statement tag=01HS}

*Soient $Z$ une variété séparée de classe $C^r$, munie d'une loi d'opération à gauche $m : G \times Z \to Z$ de classe $C^r$, et $\mu : Z \to X$ un morphisme (de classe $C^r$) compatible avec les opérations de $G$. Soient $z$ un point de $Z$, et $x = \mu(z)$. On suppose que $\mu$ est étale en $z$, et que le fixateur de $z$ dans $G$ est égal au fixateur $G_x$ de $x$. Il existe alors un voisinage ouvert $\Omega$ de l'orbite $Gz$, stable par $G$, tel que $\mu$ induise un isomorphisme de $\Omega$ sur un ouvert de $X$.*

Puisque $\mu$ est compatible avec les opérations de $G$, il est étale en tout point de $Gz$; comme l’application canonique $G/G_x \to Gx$ est un homéomorphisme, il en est de même de l’application de $Gz$ dans $Gx$ induite par $\mu$. Il résulte donc de la prop. 2 du n° 1 qu’il existe un voisinage ouvert $U$ de $Gz$ dans $Z$ tel que $\mu$ induise un plongement ouvert de $U$ dans $X$.

Puisque $G$ opère proprement dans $X$, il existe un voisinage ouvert $V$ de $x$ et une partie compacte $K$ de $G$ tels qu’on ait $gV \cap V = \varnothing$ pour $g \notin K$ (TG, III, p. 31, prop. 7); on a en particulier $e \in K$. L’ensemble $W_1$ des points $y \in Z$ tels que $Ky \subset U$ est ouvert dans $Z$: en effet, $Z - W_1$ est l’image du fermé $(K \times Z) - m^{-1}(U)$ par la projection propre $pr_2 : K \times Z \to Z$. Posons $W = W_1 \cap \mu^{-1}(V)$; c’est un ouvert de $Z$, contenant $z$, et satisfaisant aux conditions suivantes :
(i) $KW \subset U$, et en particulier $W \subset U$;
(ii) $\mu(W) \subset V$.

Posons $\Omega = GW$ et considérons la restriction de $\mu$ à $\Omega$. C’est un morphisme étale, puisque tout point de $\Omega$ est conjugué par $G$ à un point de $U$. Montrons qu’il est injectif : soient $g, h$ dans $G$ et $u, v$ dans $W$ tels que $\mu(gu) = \mu(hv)$. Posons $k = g^{-1}h$; on a $\mu(u) = k\mu(v)$, d’où $k \in K$ d’après (ii). Mais $kv$ et $u$ appartiennent à $U$ par (i); on a donc $u = kv$ puisque la restriction de $\mu$ à $V$ est injective, d’où $gu = hv$. Ainsi la restriction de $\mu$ à $\Omega$ est injective, et par suite (VAR, R, 5.7.8) est un isomorphisme sur une sous-variété ouverte de $X$, ce qui termine la démonstration.

Sous les conditions de la proposition 6, l’image de $\alpha$ est un voisinage ouvert $T$ de l’orbite $A$ de $x$, muni d’une structure de fibré vectoriel de base $A$, pour laquelle la section nulle est l’orbite $A$ elle-même. Un tel voisinage s’appelle un tube linéaire (autour de l’orbite considérée). Pour chaque point $a \in A$, la fibre $Y_a$ de cette fibration vectorielle est une sous-variété de $X$, stable par le fixateur $G_a$ de $a$, et telle que le morphisme de $G \times^{G_a} Y_a$ dans $X$ qui applique la classe de $(g, y) \in G \times Y_a$ sur $gy \in X$ induise un isomorphisme de classe $C^r$ de $G \times^{G_a} Y_a$ sur $T$. On dit que $Y_a$ est la transversale en $a$ du tube $T$. On remarquera que l’espace tangent en $a$ à $Y_a$ est canoniquement isomorphe à $Y_a$ et que c’est un supplémentaire de $T_a(A)$ dans $T_a(X)$; le fibré vectoriel $T$ de base $A$ est donc canoniquement isomorphe au fibré normal de $A$ dans $X$ (VAR, R, 8.1.3).

### 4. Types d’orbites

Soit $G$ un groupe topologique opérant continûment dans un espace topologique séparé $E$. Pour chaque point $x$ de $E$, notons $G_x$ le fixateur de $x$ dans $G$, et supposons que l’application canonique $G/G_x \to Gx$ soit un homéomorphisme; c’est le cas notamment dans les deux cas suivants :
a) les topologies de $G$ et $E$ sont discrètes ;
b) $G$ opère proprement dans $E$ (TG, III, p. 29, prop. 4), par exemple, $G$ est compact (TG, III, p. 28, prop. 2).
Notons $\mathcal{C}$ l’ensemble des classes de conjugaison de sous-groupes fermés de $G$.

Pour tout $x \in E$, on appelle *type de l’orbite* de $x$, ou parfois type de $x$, la classe dans $\mathcal{C}$ de $G_x$; deux points d’une même orbite ont même type d’orbite (A, I, p. 52, prop. 2); deux orbites sont de même type si et seulement si elles sont isomorphes comme $G$-ensembles (A, I, p. 57, th. 1). Pour tout $t \in \mathcal{C}$, on note $E_{(t)}$ l’ensemble des points de $E$ de type $t$, c’est-à-dire la réunion des orbites de type $t$; c’est une partie stable de $E$. Pour $H \in t$, on écrit aussi $E_{(H)}$ pour $E_{(t)}$; par exemple, $E_{(G)}$ est le sous-espace fermé de $E$ formé des points fixés par $G$.

Munissons $\mathcal{C}$ de la relation de préordre suivante

$$
t \leq t' \iff \text{il existe } H \in t \text{ et } H' \in t' \text{ tels que } H \supset H'.
$$

Soient $\Omega$ et $\Omega'$ deux orbites de $G$ dans $E$, $t$ et $t'$ leurs types ; pour que $t \leq t'$, il faut et il suffit qu’il existe un $G$-morphisme (nécessairement surjectif et continu) de $\Omega'$ dans $\Omega$.

Soient $x, x'$ dans $E$, $t$ et $t'$ leurs types ; pour que $t \leq t'$, il faut et il suffit qu’il existe $a \in G$ tel que $a G_{x'} a^{-1} \subset G_x$.

#### Lemme 6 {#lie-ix-s9-lem-6 .statement tag=01HT}

*Soit $G$ un groupe de Lie.*

*a)* *Toute suite décroissante de sous-groupes compacts de $G$ est stationnaire.*

*b)* *Soient $H$ et $H'$ deux sous-groupes compacts de $G$, tels que $H \subset H'$ et qu’il existe un isomorphisme (de groupes topologiques) de $H'$ sur $H$. On a alors $H = H'$.*

*c)* *Muni de la relation $t \leq t'$, l’ensemble $\mathcal{C}$ est un ensemble ordonné noethérien* (E, III, p. 51).

*a)* Soit $(H_i)_{i \geq 1}$ une suite décroissante de sous-groupes compacts de $G$; ce sont des sous-groupes de Lie (III, § 8, n° 2, th. 2). La suite d’entiers $(\dim H_i)_{i \geq 1}$ est décroissante, donc stationnaire, et il existe un entier $N$ tel que les sous-groupes $H_i$ aient tous la même composante neutre pour $i \geq N$. Alors la suite décroissante d’entiers positifs $(H_i : (H_i)_0)_{i \geq N}$ est stationnaire, donc on a $H_i = H_{i+1}$ pour $i$ assez grand.

*b)* Soit $f$ un isomorphisme de $H'$ sur $H$. La suite $(f^n(H))_{n \geq 0}$ est une suite décroissante de sous-groupes compacts de $G$, de sorte qu’on a $f^n(H) = f^{n+1}(H)$ pour $n$ assez grand, d’après *a)*. Comme $f$ est un isomorphisme, ceci entraîne $f(H) = H = f(H')$, d’où $H = H'$.

*c)* Soient $t, t' \in \mathcal{C}$ tels que $t \leq t'$ et $t' \leq t$. Il existe alors $H, H_1 \in t$ et $H', H'_1 \in t'$ tels que $H \supset H'$ et $H_1 \subset H'_1$. Soient $g$ et $g'$ deux éléments de $G$ tels que $H_1 = g H g^{-1}$ et $H'_1 = g' H' g'^{-1}$; posons $u = g'^{-1} g$. On a

$$
u H u^{-1} \subset H' \subset H ;
$$

d’après *b)*, ceci entraîne $u H u^{-1} = H$, donc $H' = H$ et $t' = t$. L’ensemble $\mathcal{C}$ est donc ordonné, et noethérien d’après *a)*.

#### Théorème 2 {#lie-ix-s9-thm-2 .statement tag=01HU}

*Soit $G$ un groupe de Lie opérant proprement sur $X$, de façon que la loi d’opération $(g, x) \mapsto gx$ soit de classe $C^r$. On suppose $X$ paracompacte.*

*a)* *L’application qui, à chaque point de $X$, associe son type d’orbite, possède la propriété de semi-continuité suivante : soit $x \in X$ et soit $t \in \mathcal{C}$ son type d’orbite ; il existe un voisinage ouvert stable $U$ de $x$ tel que, pour tout $u \in U$, le type de $u$ soit $\geq t$.*

b) Pour tout $t \in \mathcal{T}$, $X_{(t)}$ est une sous-variété de $X$, la relation d'équivalence dans $X_{(t)}$ déduite de l'opération de $G$ est régulière (VAR, R, 5.9.5), et le morphisme $X_{(t)} \to X_{(t)}/G$ est une fibration.

c) Supposons $X/G$ connexe. Alors l'ensemble des types d'orbite des éléments de $X$ possède un plus grand élément $\tau$; de plus, $X_{(\tau)}$ est une partie ouverte et dense de $X$ et $X_{(\tau)}/G$ est connexe.

Soient $x$ un point de $X$ et $t \in \mathcal{T}$ son type. Pour démontrer $a)$ et $b)$, on peut remplacer $X$ par un ouvert stable contenant $x$, donc (prop. 6) supposer que $X$ est de la forme $G \times^H W$, où $W$ est l'espace d'une représentation linéaire analytique de dimension finie d'un sous-groupe compact $H$ de $G$, le point $x$ étant l'image $p(e, 0)$ de $(e, 0) \in G \times W$ par la projection canonique $p : G \times W \to G \times^H W$. Si $u = p(g, y) \in G \times^H W$ et $a \in G$, alors $au = u$ si et seulement s'il existe $h \in H$ avec $(ag, y) = (gh^{-1}, hy)$ c'est-à-dire si $a \in gH_yg^{-1}$. On a donc $G_u = gH_yg^{-1}$; en particulier $G_x = H$, donc $G_u$ est conjugué à un sous-groupe de $G_x$, ce qui prouve que le type de $u$ est $\geq t$, d'où $a)$.

Par ailleurs, pour que $u$ soit de type $t$, il faut et il suffit que $G_u$ soit conjugué à $H$ dans $G$, ou encore que $H_y$ soit conjugué à $H$ dans $G$; d'après le lemme 6, $b)$, cela signifie que $H_y = H$, donc que $y$ est fixé par $H$. Si $W'$ est le sous-espace vectoriel de $W$ formé des éléments fixés par $H$, il en résulte que $X_{(t)}$ s'identifie à $G \times^H W'$, donc aussi à $G/H \times W'$, d'où $b)$.

Pour démontrer $c)$, observons que l'hypothèse de connexité de $X/G$ entraîne que $X$ est pure de dimension finie : en effet, pour tout $k \geq 0$, notons $X_k$ l'ensemble des points $x \in X$ tels que $\dim_x X = k$; alors $X_k$ est ouvert et fermé dans $X$, et stable par $G$, de sorte que $X$ est égal à l'un des $X_k$.

Démontrons maintenant $c)$ par récurrence sur la dimension de $X$, l'assertion étant évidente pour $\dim X = 0$. Soit $\tau$ un élément maximal parmi les types d'orbite des points de $X$ (un tel élément existe d'après le lemme 6, $c$) ). Nous allons prouver l'assertion suivante :

c') Pour toute partie $A$ de $X_{(\tau)}$, ouverte et fermée dans $X_{(\tau)}$ et stable par $G$, l'adhérence $\overline{A}$ de $A$ dans $X$ est ouverte.

Cette assertion implique $c)$. En effet, notons d'abord que $X_{(\tau)}$ est ouvert dans $X$, d'après $a)$; l'assertion $c')$ entraîne que $\overline{X}_{(\tau)}$ est ouvert et fermé dans $X$, donc égal à $X$ puisqu'il est stable par $G$ et que $X/G$ est connexe. Soit $A$ une partie ouverte et fermée non vide de $X_{(\tau)}$, stable par $G$; d'après $c')$, $\overline{A}$ est ouverte et fermée dans $X$ et stable par $G$, donc égale à $X$; ceci entraîne que $A$ est dense dans $X_{(\tau)}$, donc égale à $X_{(\tau)}$. Par conséquent toute partie ouverte et fermée non vide de $X_{(\tau)}/G$ est égale à $X_{(\tau)}/G$, ce qui prouve que $X_{(\tau)}/G$ est connexe. Enfin puisque $X_{(\tau)}$ est dense dans $X$, il résulte de $a)$ que tout point de $X$ est de type $\leq \tau$; autrement dit $\tau$ est le plus grand élément parmi les types d'orbite des points de $X$.

Démontrons maintenant $c')$. On peut supposer $A$ non vide ; soit $x \in \overline{A}$. Il s'agit de montrer que $\overline{A}$ est un voisinage de $x$. Pour cela on peut, comme ci-dessus, supposer $X = G \times^H W$, avec $H$ compact, $x$ étant l'image canonique de $(e, 0)$. Supposons d'abord que $H$ opère trivialement dans $W$ : alors $X$ s'identifie à $(G/H) \times W$, et

X_{(\tau)}/G = X/G est homéomorphe à W, donc connexe ; on a alors A/G = X/G, d’où A = X. Nous supposerons désormais que H n’opère pas trivialement sur W. Choisissons sur W un produit scalaire invariant par le groupe compact H ; soit S la sphère unité de W (ensemble des vecteurs de norme 1). Notons que S/H est connexe : en effet si dim(W) ≥ 2, S est connexe, et si dim(W) = 1, S est un espace à deux points sur lequel H opère de façon non triviale. Posons Y = G ×^H S ; c’est une sous-variété fermée de X, stable par G, de codimension 1, et Y/G, qui est homéomorphe à S/H, est connexe. En vertu de l’hypothèse de récurrence, il existe donc un type d’orbite θ maximal pour Y, l’ensemble Y_{(θ)} est ouvert et dense dans Y, et Y_{(θ)}/G est connexe.

Considérons l’action de R^*_+ sur X déduite par passage au quotient de la loi d’opération (λ, (g, w)) ↦ (g, λw) de R^*_+ sur G × W. Deux points de X conjugués par cette action ont même type d’orbite ; par conséquent X_{(θ)} contient R^*_+ Y_{(θ)}, qui est un ouvert dense de X. Or X_{(τ)} est ouvert d’après a), donc rencontre X_{(θ)}, de sorte qu’on a θ = τ.

D’autre part, l’homéomorphisme (λ, w) ↦ λw de R^*_+ × S dans W − {0} (TG, VI, p. 10, prop. 3) induit un homéomorphisme de R^*_+ × (S/H) dans (R^*_+ S)/H, donc aussi de R^*_+ × (Y/G) dans (R^*_+ Y)/G, et de R^*_+ × (Y_{(θ)}/G) dans (R^*_+ Y_{(θ)})/G. Ainsi (R^*_+ Y_{(θ)})/G est connexe, et X_{(τ)}/G, qui contient un sous-ensemble dense connexe, est lui-même connexe (TG, I, p. 81, prop. 1). Par suite A est égal à X_{(τ)}, donc est dense dans X, et A est un voisinage de x. Ceci termine la démonstration du théorème.

Avec les notations du th. 2, c), les points de X_{(τ)} sont dits principaux et leurs orbites principales. Si x est un point de X, et si G ×^{G_x} W est un tube linéaire de X autour de l’orbite de x, le point x est principal si et seulement si G_x opère trivialement dans W, c’est-à-dire si le tube est de la forme (G/G_x) × W.

#### Exemple 1 {#lie-ix-s9-n4-exa-1 .statement tag=01HV}

Soit G un groupe de Lie compact connexe, opérant sur lui-même par automorphismes intérieurs. Le fixateur d’un élément x de G n’est autre que le centralisateur Z(x) de x dans G ; il contient tout tore maximal contenant x. Il en résulte que le plus grand type d’orbite τ est la classe de conjugaison des tores maximaux de G. L’ouvert G_{(τ)} est l’ensemble des éléments très réguliers de G (§ 5, no 1, remarque). Supposons G simplement connexe. Alors G_{(τ)} est égal à l’ensemble G_r des éléments réguliers de G (§ 5, no 2, remarque 2) ; si A est une alcôve d’une sous-algèbre de Cartan t de g = L(G), l’application composée π : A ↦^{exp} G_r ↦ G_r/Int(G) est un isomorphisme de variétés analytiques. C’est en effet un homéomorphisme (§ 5, no 2, cor. 1 à la prop. 2) ; soit a ∈ A, posons t = exp a et identifions T_t(G) à g par la translation γ(t). L’application tangente T_a(π) s’identifie alors à l’application composée de l’injection canonique t → g et de l’application de passage au quotient g → g/Im(Ad t^{-1} − 1). Puisque t est régulier, T_a(π) est un isomorphisme, d’où le résultat annoncé (VAR, R, 5.7.8).

#### Exemple 2 {#lie-ix-s9-n4-exa-2 .statement tag=01HW}

Soient E un espace affine réel euclidien, 𝓗 un ensemble d’hyperplans de E, W le groupe de déplacements de E engendré par les réflexions orthogonales par rapport aux hyperplans de $\mathfrak{H}$. On suppose que $\mathfrak{H}$ est stable par W et que le groupe W, muni de la topologie discrète, opère proprement dans E.

On peut appliquer ce qui précède à l’action de W sur E. Le fixateur d’un point x de E est le sous-groupe de W engendré par les réflexions par rapport aux hyperplans de $\mathfrak{H}$ contenant x (V, § 3, no 3, prop. 2). Par conséquent, le plus grand type d’orbite $\tau$ est la classe du sous-groupe $\{ \mathrm{Id}_E \}$, et $E_{(\tau)}$ est la réunion des chambres de E. On notera que dans ce cas le revêtement $E_{(\tau)} \to E_{(\tau)}/W$ est trivial, et en particulier que $E_{(\tau)}$ n’est pas connexe si $\mathfrak{H}$ est non vide.

## EXERCICES {#lie-ix-s9-exercises}

See the [exercises for § 9](exercises/s9/).
