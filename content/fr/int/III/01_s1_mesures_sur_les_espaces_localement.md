---
book: int
book_title: Integration
chapter: III
chapter_title: Mesures sur les espaces localement compacts
section: 1
section_title: Mesures sur les espaces localement compacts
lang: fr
source: int-i-iv-fr
pdf_pages: 0044-0068, 0100-0105
extraction: ocr
subsections:
    - "no": 1
      title: Fonctions continues à support compact
      page: 0
      pdf_page: 44
    - "no": 2
      title: Propriétés d’approximation
      page: 0
      pdf_page: 47
    - "no": 3
      title: Définition d’une mesure
      page: 0
      pdf_page: 51
    - "no": 4
      title: Produit d’une mesure par une fonction continue
      page: 0
      pdf_page: 54
    - "no": 5
      title: Mesures réelles. Mesures positives
      page: 0
      pdf_page: 55
    - "no": 6
      title: Valeur absolue d’une mesure complexe
      page: 0
      pdf_page: 58
    - "no": 7
      title: Définition d’une mesure par prolongement
      page: 0
      pdf_page: 60
    - "no": 8
      title: Mesures bornées
      page: 0
      pdf_page: 60
    - "no": 9
      title: Topologie vague sur l’espace des mesures
      page: 0
      pdf_page: 63
    - "no": 10
      title: Convergence compacte dans $\mathcal{M}(X; \mathbf{C})$
      page: 0
      pdf_page: 66
statements: 43
exercises: 3
content_sha256: 4c82eb80ef376848737949f80fb7a3ad9d014c13df3c51654fa25334b04f9dd7
---

## § 1. Mesures sur un espace localement compact

### 1. Fonctions continues à support compact

#### Définition 1 {#int-iii-s1-def-1 .statement}

Soient X un espace topologique, E un espace vectoriel sur R, ou l’espace $\bar{\mathbf{R}}$. On appelle support d’une application f de X dans E et l’on note Supp (f) le plus petit ensemble fermé S dans X tel que $f(x) = 0$ dans $X - S$ (en d’autres termes, S est l’adhérence dans X de l’ensemble des $x \in X$ tels que $f(x) \neq 0$).

Soient X un espace localement compact, E un espace vectoriel topologique sur R ou sur C ; rappelons que l’on note $\mathcal{C}(X;E)$ l’espace vectoriel des applications continues de X dans E ; lorsque $E = \mathbf{R}$ ou $E = \mathbf{C}$ on supprimera la mention de E dans cette notation s’il n’en résulte pas de confusion. Nous noterons $\mathcal{K}(X;E)$ le sous-espace de $\mathcal{C}(X;E)$ formé des applications continues à support compact ; pour toute partie A de X, nous noterons $\mathcal{C}(X,A;E)$ (resp. $\mathcal{K}(X,A;E)$) le sous-espace de $\mathcal{C}(X;E)$ (resp. $\mathcal{K}(X;E)$) formé des applications f telles que $\operatorname{Supp}(f) \subset A$. Si $E = \mathbf{R}$ ou $E = \mathbf{C}$, on écrit $\mathcal{K}(X)$ (resp. $\mathcal{K}(X,A)$) au lieu de $\mathcal{K}(X;\mathbf{R})$ ou $\mathcal{K}(X;\mathbf{C})$ (resp. $\mathcal{K}(X,A;\mathbf{R})$ ou $\mathcal{K}(X,A;\mathbf{C})$) si aucune confusion n’en résulte ; on désigne par $\mathcal{K}_+(X)$ le cône convexe pointé formé des fonctions $\geq 0$ de $\mathcal{K}(X,\mathbf{R})$.

Pour toute partie compacte K de X, l’espace $\mathcal{K}(X,K;E)$ s’identifie à un sous-espace de l’espace de fonctions continues $\mathcal{C}(K;E)$ (savoir le sous-espace des applications continues de K dans E nulles dans la frontière de K). Lorsqu’on munit $\mathcal{C}(K;E)$ de la topologie de la convergence uniforme dans K, $\mathcal{K}(X,K;E)$ est un sous-espace fermé de $\mathcal{C}(K;E)$. En particulier, lorsque E est un espace de Fréchet (resp. un espace de Banach), il en est de même de $\mathcal{K}(X, K; E)$, car si la topologie de $E$ est définie par les semi-normes $p_n$ (resp. la norme $x \mapsto \|x\|$), la topologie de $\mathcal{K}(X, K; E)$ est définie par les semi-normes $f \mapsto \sup_{x \in K} p_n(f(x))$ (resp. la norme $f \mapsto \sup_{x \in K} \|f(x)\|$, notée $\|f\|$).

L’espace $\mathcal{K}(X; E)$ est réunion de la famille filtrante croissante des sous-espaces $\mathcal{K}(X, K; E)$, où $K$ parcourt l’ensemble des parties compactes de $X$; en outre, si $K_1 \subset K_2$ sont deux parties compactes de $X$, l’injection canonique $\mathcal{K}(X, K_1; E) \to \mathcal{K}(X, K_2; E)$ est continue pour les topologies définies ci-dessus. Si $E$ est localement convexe, on peut donc définir sur $\mathcal{K}(X; E)$ la topologie limite inductive des topologies localement convexes des $\mathcal{K}(X, K; E)$ (*Esp. vect. top.*, chap. II, 2e éd., § 4, n° 4); sauf mention expresse du contraire, c’est toujours de cette topologie qu’il s’agira lorsque nous considérerons $\mathcal{K}(X; E)$ comme un espace vectoriel topologique.

#### Proposition 1 {#int-iii-s1-prop-1 .statement}

Soient $X$ un espace localement compact, $E$ un espace localement convexe séparé.

(i) L’espace localement convexe $\mathcal{K}(X; E)$ est séparé. Pour toute partie compacte $K$ de $X$, la topologie induite par celle de $\mathcal{K}(X; E)$ sur $\mathcal{K}(X, K; E)$ est la topologie de la convergence uniforme dans $K$, et chacun des sous-espaces $\mathcal{K}(X, K; E)$ est fermé dans $\mathcal{K}(X; E)$.

(ii) Si $E$ est produit d’un nombre fini d’espaces localement convexes $E_i$ ($1 \leq i \leq n$), l’application $f \mapsto (\mathrm{pr}_i \circ f)$ est un isomorphisme de l’espace $\mathcal{K}(X; E)$ sur l’espace produit $\prod_{1 \leq i \leq n} \mathcal{K}(X; E_i)$.

(iii) Si $X$ est somme d’une famille d’espaces localement compacts $(X_\lambda)_{\lambda \in L}$, l’application $f \mapsto (f|X_\lambda)_{\lambda \in L}$ est un isomorphisme de l’espace $\mathcal{K}(X; E)$ sur l’espace somme directe topologique de la famille $(\mathcal{K}(X_\lambda; E))_{\lambda \in L}$.

(i) Notons que, sur $\mathcal{K}(X; E)$, la topologie de la convergence uniforme dans $X$ est compatible avec la structure d’espace vectoriel de $\mathcal{K}(X; E)$, car pour toute $f \in \mathcal{K}(X; E)$, de support (compact) $S$, l’ensemble $f(X) = f(S) \cup \{0\}$ est compact, donc borné dans $E$ (*Esp. vect. top.*, chap. III, § 3, n° 1, prop. 1). Comme cette topologie $\mathcal{T}_0$ est localement convexe et induit sur chacun des $\mathcal{K}(X, K; E)$ la topologie de la convergence uniforme dans $K$, il en est de même de la topologie limite inductive $\mathcal{T}$ sur $\mathcal{K}(X; E)$ (*Esp. vect. top.*, chap. II, 2e éd., § 4, n° 4, Remarque); en outre $\mathcal{T}$ est plus fine que $\mathcal{T}_0$ et $\mathcal{T}_0$ est séparée, donc $\mathcal{T}$ est séparée. Enfin, supposons qu’une fonction $f \in \mathcal{K}(X; E)$ soit adhérente à $\mathcal{K}(X, K; E)$; par définition, il existe une partie compacte $K' \supset K$ de $X$ telle que $f \in \mathcal{K}(X, K'; E)$. D’après ce qui précède, $f$ est adhérent à $\mathcal{K}(X, K; E)$ dans l’espace $\mathcal{K}(X, K'; E)$, donc appartient à $\mathcal{K}(X, K; E)$.

(ii) Le critère de continuité dans une limite inductive (*Esp. vect. top.*, chap. II, 2e éd., § 4, n° 4, prop. 5) montre aussitôt que l’application $f \mapsto (\mathrm{pr}_i \circ f)$ est continue et qu’il en est de même de l’application réciproque (pour cette dernière, il suffit de remarquer que si, pour toute fonction $f_i \in \mathcal{K}(X; E_i)$, on désigne par $f'_i$ l’application de $X$ dans $E$ telle que $\mathrm{pr}_i \circ f'_i = f_i$, $\mathrm{pr}_j \circ f'_i = 0$ pour $j \neq i$, chacune des applications $f_i \mapsto f'_i$ est continue).

(iii) Toute partie compacte $K$ de $X$ ne rencontre que les $X_\lambda$ d’une sous-famille *finie* $(X_\lambda)_{\lambda \in H}$ de $(X_\lambda)_{\lambda \in L}$, et il est immédiat que si l’on pose $K_\lambda = K \cap X_\lambda$ pour $\lambda \in H$, l’application $f \mapsto (f|X_\lambda)_{\lambda \in H}$ est un isomorphisme de $\mathcal{K}(X, K; E)$ sur $\prod_{\lambda \in H} \mathcal{K}(X_\lambda, K_\lambda; E)$. Inversement, pour toute fonction $f_\lambda \in \mathcal{K}(X_\lambda; E)$, soit $f''_\lambda$ l’application de $X$ dans $E$ telle que $f''_\lambda|X_\lambda = f_\lambda$ et $f''_\lambda|X_\mu = 0$ pour $\mu \neq \lambda$; il est immédiat que l’application $f_\lambda \mapsto f''_\lambda$ de $\mathcal{K}(X_\lambda; E)$ dans $\mathcal{K}(X; E)$ est continue. L’assertion (iii) résulte de ces remarques et du critère de continuité dans les limites inductives (*Esp. vect. top.*, chap. II, 2e éd., § 4, n° 4, prop. 5).

#### Proposition 2 {#int-iii-s1-prop-2 .statement}

Soient $X$ un espace localement compact, $E$ un espace localement convexe séparé.
(i) Si $E$ est un espace de Fréchet, l’espace $\mathcal{K}(X; E)$ est tonnelé.
(ii) Si $X$ est paracompact, alors, pour tout ensemble borné $B$ de $\mathcal{K}(X; E)$, il existe une partie compacte $K$ de $X$ telle que $B \subset \mathcal{K}(X, K; E)$.

Supposons que $E$ soit un espace de Fréchet. Pour toute partie compacte $K$ de $X$, $\mathcal{K}(X, K; E)$ est alors un espace de Fréchet, donc tonnelé, et l’on sait qu’une limite inductive d’espaces tonnelés est tonnelée (*Esp. vect. top.*, chap. III, § 1, n° 2, cor. 2 de la prop. 2), d’où (i).

Si $X$ est paracompact, on sait (*Top. gén.*, chap. I, 3e éd., § 9, n° 10, th. 5) que $X$ est *somme* d’une famille $(X_\lambda)_{\lambda \in L}$ d’espaces localement compacts *dénombrables à l’infini*; donc (prop. 1, (iii)), $\mathcal{K}(X; E)$ est *somme directe topologique* de la famille de sous-espaces $\mathcal{K}(X_\lambda; E)$ ($\lambda \in L$). En vertu de la caractérisation des ensembles bornés dans une somme directe topologique (Esp. vect. top., chap. III, 2e éd.), tout ensemble borné dans $\mathcal{H}(X; E)$ est contenu dans la somme d’un nombre fini de sous-espaces $\mathcal{H}(X_\lambda; E)$, et il suffira de prouver que tout ensemble borné dans $\mathcal{H}(X_\lambda; E)$ est contenu dans un sous-espace $\mathcal{H}(X_\lambda, K_\lambda; E)$, où $K_\lambda$ est compact dans $X_\lambda$. On est ainsi ramené au cas où $X$ est dénombrable à l’infini, autrement dit réunion d’une suite d’ouverts relativement compacts $U_n$ tels que $\overline{U}_n \subset U_{n+1}$ (Top. gén., chap. I, 3e éd., § 9, no 9, prop. 15). Alors $\mathcal{H}(X; E)$ est limite inductive stricte de la suite d’espaces $\mathcal{H}(X, \overline{U}_n; E)$, d’où l’assertion (ii) (Esp. vect. top., chap. III, § 2, no 4, prop. 6).

Nous dirons qu’une partie $H$ de $\mathcal{H}(X; E)$ est strictement compacte si elle est compacte, et s’il existe une partie compacte $K$ de $X$ telle que $H \subset \mathcal{H}(X, K; E)$. Il résulte aussitôt de la prop. 2 que si $X$ est un espace localement compact paracompact et si $E$ est séparé, tout ensemble compact dans $\mathcal{H}(X; E)$ est strictement compact. On peut donner des exemples d’espaces localement compacts $X$ (non paracompacts) tels qu’il existe dans $\mathcal{H}(X; R)$ des ensembles compacts mais non strictement compacts (exerc. 3 et 4).

En vertu du th. d’Ascoli (Top. gén., chap. X, 2e éd., § 2, no 5, cor. 3 du th. 2), rappelons qu’une partie strictement compacte $H$ de $\mathcal{H}(X; E)$, contenue dans $\mathcal{H}(X, K; E)$, est caractérisée par les conditions suivantes : 1° elle est fermée ; 2° elle est équicontinue ; 3° pour tout $x \in K$, l’ensemble $H(x)$ est relativement compact dans $E$.

#### Corollaire {#int-iii-s1-n1-cor-1 .statement}

Soient $X$ un espace localement compact et paracompact ; si $E$ est un espace localement convexe quasi-complet, l’espace $\mathcal{H}(X; E)$ est quasi-complet.

En effet, il suffit, en vertu de la prop. 2, (ii), de remarquer que pour toute partie compacte $K$ de $X$, $\mathcal{H}(X, K; E)$ est un sous-espace fermé de $C(K; E)$, qui est quasi-complet, toute partie bornée de $C(K; E)$ étant formée de fonctions prenant leurs valeurs dans une même partie bornée de $E$.

### 2. Propriétés d’approximation

#### Lemme 1 {#int-iii-s1-lem-1 .statement}

Soient $X$ un espace localement compact, $K$ une partie compacte de $X$, $(V_k)_{1 \leq k \leq n}$ un recouvrement fini de $K$ par des ensembles ouverts dans X. Alors il existe n applications continues $f_k$ de X dans $[0, 1]$, telles que le support de $f_k$ soit contenu dans $V_k$ pour $1 \leq k \leq n$, et que l’on ait $\sum_{k=1}^n f_k(x) \leq 1$ pour tout $x \in X$, et $\sum_{k=1}^n f_k(x) = 1$ pour tout $x \in K$.

En effet, soit $X'$ l’espace compact obtenu en adjoignant à X un point à l’infini $\omega$ (Top. gén., chap. I, 3e éd., § 9, n° 8, th. 4); les ensembles $V_0 = X' - K$ et $V_k$ ($1 \leq k \leq n$) forment un recouvrement ouvert de $X'$. Soit $(f_k)_{0 \leq k \leq n}$ une partition continue de l’unité subordonnée à ce recouvrement de $X'$ (Top. gén., chap. IX, 2e éd., § 4, n° 3, prop. 3); les fonctions $f_k$ d’indice $k \geq 1$ répondent aux conditions du lemme.

#### Lemme 2 {#int-iii-s1-lem-2 .statement}

Soient X un espace localement compact, K une partie compacte de X, E un espace localement convexe, q une semi-norme continue sur E, $\Phi$ un ensemble équicontinu d’applications de X dans E, de supports contenus dans K. Alors, pour tout $\varepsilon > 0$, il existe une partition continue de l’unité $(\varphi_j)_{0 \leq j \leq n}$ sur X, possédant les propriétés suivantes :
(i) Pour $1 \leq j \leq n$, on a $\operatorname{Supp}(\varphi_j) \subset K$.
(ii) Si $x_j$ est un point quelconque de $\operatorname{Supp}(\varphi_j)$ pour $1 \leq j \leq n$, on a, pour toute fonction $f \in \Phi$ et pour tout $x \in X$:
$$
q\left(f(x) - \sum_{j=1}^n \varphi_j(x)f(x_j)\right) \leq \varepsilon.
$$
Pour tout y appartenant à la frontière de K, on a $f(y) = 0$ pour toute $f \in \Phi$, donc il existe un voisinage ouvert $V_y$ de y dans X tel que, pour tout $z \in V_y$ et toute $f \in \Phi$, on ait $q(f(z)) \leq \varepsilon/2$. Soit $K'$ l’ensemble des points de K n’appartenant à aucun des $V_y$ lorsque y parcourt la frontière de K ; $K'$ est compact et contenu dans l’intérieur de K. L’ensemble $\Phi$ est uniformément équicontinu dans K ; donc il existe un recouvrement ouvert fini $(U_j)_{1 \leq j \leq n}$ de $K'$ formé d’ensembles ouverts dans X, contenus dans K, tels que pour tout couple de points $x, y$ d’un même $U_j$, on ait $q(f(x) - f(y)) \leq \varepsilon/2$ quelle que soit $f \in \Phi$. D’après le lemme 1, il existe n applications continues $\varphi_j$ de X dans $[0, 1]$ ($1 \leq j \leq n$) telles que $\operatorname{Supp}(\varphi_j) \subset U_j$ et que l’on ait $\sum_{j=1}^n \varphi_j(x) \leq 1$ dans X et

$$
\sum_{j=1}^{n} \varphi_j(x) = 1 \text{ dans } K'. \text{ Pour } x_j \in \operatorname{Supp}(\varphi_j) \ (1 \leq j \leq n) \text{ et } f \in \Phi, \text{ on a donc, pour tout } x \in U_j,
$$
$$
q(f(x)\varphi_j(x) - f(x_j)\varphi_j(x)) = \varphi_j(x)q(f(x) - f(x_j)) \leq \frac{\varepsilon}{2}\varphi_j(x)
$$
et cette relation est encore vraie si $x \notin U_j$ puisqu’alors $\varphi_j(x) = 0$. Par addition on en déduit, pour tout $x \in X$,
$$
(2) \quad q(f(x)(1 - \varphi_0(x)) - \sum_{j=1}^{n} \varphi_j(x)f(x_j)) \leq \frac{\varepsilon}{2}(1 - \varphi_0(x))
$$
en posant $\varphi_0 = 1 - \sum_{j=1}^{n} \varphi_j$; d’où (1) pour $x \in K'$ puisqu’alors $\varphi_0(x) = 0$; on a aussi (1) pour $x \notin K$, le premier membre étant alors nul. Enfin, pour $x \in K - K'$, on a $q(f(x)\varphi_0(x)) \leq \varepsilon/2$ par définition de $K'$, donc cette relation et (2) entraînent encore (1) dans ce cas.

Soit $X$ un espace localement compact; pour tout espace de Banach $E$ (réel ou complexe), nous désignerons par $C^b(X;E)$ l’espace vectoriel des applications continues et bornées de $X$ dans $E$; on sait que la topologie de la convergence uniforme dans $X$ est compatible avec la structure d’espace vectoriel (réel, resp. complexe) de $C^b(X;E)$, et est définie par la norme
$$
(3) \quad \|f\| = \sup_{x \in X} \|f(x)\|.
$$
En outre, l’espace normé ainsi défini est un espace de Banach (Top. gén., chap. X, 2e éd., § 3, n° 2 et n° 1, cor. 2 de la prop. 3); la topologie définie par cette norme sur $\mathcal{K}(X;E)$ (autrement dit la topologie de la convergence uniforme dans $X$) est moins fine que la topologie limite inductive définie sur $\mathcal{K}(X;E)$ au n° 1.

#### Proposition 3 {#int-iii-s1-prop-3 .statement}

Soient $X$ un espace localement compact, $X'$ l’espace compact obtenu par adjonction à $X$ d’un point à l’infini $\omega$ (Top. gén., chap. I, 3e éd., § 9, n° 8, th. 4), $E$ un espace de Banach. L’adhérence de $\mathcal{K}(X;E)$ dans l’espace normé $C^b(X;E)$ est l’espace vectoriel des fonctions continues dans $X$, à valeurs dans $E$ et tendant vers 0 au point $\omega$.

Soit en effet $f \in C^b(X;E)$ une fonction adhérente à $\mathcal{K}(X;E)$; pour tout $\varepsilon > 0$ il existe une fonction $g \in \mathcal{K}(X;E)$, telle que ||f(x) - g(x)|| \leq \varepsilon pour tout x \in X ; si K est le support de g, on a donc ||f(x)|| \leq \varepsilon pour tout x \in C K, donc f(x) tend vers 0 lorsque x tend vers \omega. Inversement, si f possède cette propriété, pour tout \varepsilon > 0 il existe un ensemble compact K \subset X tel que ||f(x)|| \leq \varepsilon pour tout x \in C K. En vertu du lemme 1, il existe une application continue h de X dans [0, 1], à support compact, égale à 1 dans K ; on a donc ||f(x)h(x)|| \leq \varepsilon dans C K et f(x) = f(x)h(x) dans K ; comme fh est à support compact et que ||f(x) - f(x)h(x)|| \leq 2\varepsilon pour tout x \in X, la proposition est démontrée.

Nous noterons \mathcal{C}^0(X ; E) le sous-espace de \mathcal{C}^b(X ; E) formé des fonctions tendant vers 0 au point à l’infini \omega ; c’est donc le complété de l’espace normé \mathcal{K}(X ; E).

#### Proposition 4 {#int-iii-s1-prop-4 .statement}

Soient X un espace localement compact, E un espace localement convexe ; alors l’espace \mathcal{K}(X ; E) est partout dense dans \mathcal{C}(X ; E) pour la topologie de la convergence compacte.

En effet, pour tout ensemble compact K \subset X, il existe une fonction h \in \mathcal{K}(X ; \mathbf{R}) égale à 1 dans K, en vertu du lemme 1 ; pour toute fonction f \in \mathcal{C}(X ; E), la fonction hf, qui appartient à \mathcal{K}(X ; E), est égale à f dans K, d’où notre assertion.

#### Proposition 5 {#int-iii-s1-prop-5 .statement}

Soient X un espace localement compact, E un espace localement convexe réel (resp. complexe). Pour toute partie compacte K de X, l’espace vectoriel \mathcal{K}(X, K ; \mathbf{R}) \otimes_{\mathbf{R}} E (resp. \mathcal{K}(X, K ; \mathbf{C}) \otimes_{\mathbf{C}} E) (identifié à un ensemble d’applications de X dans E, cf. Alg., chap. II, 3e éd., § 7, n° 7, cor. de la prop. 15) est dense dans \mathcal{K}(X, K ; E) ; l’espace vectoriel \mathcal{K}(X ; \mathbf{R}) \otimes_{\mathbf{R}} E (resp. \mathcal{K}(X ; \mathbf{C}) \otimes_{\mathbf{C}} E) est dense dans \mathcal{K}(X ; E).

La seconde assertion étant conséquence évidente de la première, il suffit de prouver celle-ci. Or, appliquons le lemme 2 en prenant \Phi réduit à un élément f de \mathcal{K}(X, K ; E) ; on a alors, pour tout x \in X

$$
q(f(x) - \sum_{j=1}^n \varphi_j(x)f(x_j)) \leq \varepsilon
$$

où les \varphi_j appartiennent à \mathcal{K}(X, K ; \mathbf{R}) ; comme l’application $x \mapsto \sum_{j=1}^n \varphi_j(x)f(x_j)$ est canoniquement identifiée à l’élément

$$
\sum_{j=1}^{n} \varphi_j \otimes f(x_j),
$$
cela démontre la proposition, par définition de la topologie de $\mathcal{K}(X, K ; E)$.

### 3. Définition d’une mesure

#### Définition 2 {#int-iii-s1-def-2 .statement}

On apelle mesure (ou mesure complexe) sur un espace localement compact X, toute forme linéaire continue sur $\mathcal{K}(X ; \mathbf{C})$.

Si $\mu$ est une mesure sur un espace localement compact X, la valeur de cette mesure pour une fonction $f \in \mathcal{K}(X ; \mathbf{C})$ s’appelle l’intégrale de $f$ par rapport à $\mu$; outre les notations générales $\mu(f)$ et $\langle f, \mu \rangle$, on emploie aussi, pour la désigner, les notations $\int f d\mu, \int \mu, \int f(x) d\mu(x)$ et $\int f(x)\mu(x)$; pour l’emploi de la lettre x, voir Ens., chap. I, § 1, n° 1.

En vertu du critère de continuité dans les limites inductives (Esp. vect. top., chap. II, 2e éd., § 4, n° 4, prop. 5), dire que $\mu$ est une mesure sur X signifie encore que $\mu$ est une forme linéaire sur $\mathcal{K}(X ; \mathbf{C})$ satisfaisant à la condition suivante: pour toute partie compacte K de X, il existe un nombre $M_K$ telle que, pour toute fonction $f \in \mathcal{K}(X ; \mathbf{C})$ dont le support est contenu dans K, on ait
(4)
$$
|\mu(f)| \leq M_K \cdot \|f\| \quad (\text{avec } \|f\| = \sup_{x \in X} |f(x)|).
$$
Plus généralement:

#### Proposition 6 {#int-iii-s1-prop-6 .statement}

Soient X un espace localement compact; (K_\alpha) une famille de parties compactes de X dont les intérieurs $\dot{K}_\alpha$ forment un recouvrement de X. Pour qu’une forme linéaire $\mu$ sur $\mathcal{K}(X ; \mathbf{C})$ soit une mesure sur X, il faut et il suffit que, pour tout $\alpha$, il existe un nombre $M_\alpha$ tel que l’on ait
(5)
$$
|\mu(f)| \leq M_\alpha \cdot \|f\|
$$
pour toute fonction $f \in \mathcal{K}(X, K_\alpha ; \mathbf{C})$.

La condition étant évidemment nécessaire, il suffit de prouver que (5) entraîne (4) pour toute partie compacte K de X. Or K est recouvert par un nombre fini d’ensembles ouverts $\dot{K}_{\alpha_i}$ (1 $\leq i \leq n$); appliquant à K et aux $\dot{K}_{\alpha_i}$ le lemme 1 du n° 2, il existe des fonctions $g_i \geq 0$ continues dans X, telles que $\operatorname{Supp}(g_i) \subset K_{\alpha_i}$,
$$
0 \leq \sum_{i=1}^{n} g_i(x) \leq 1
$$

pour tout $x \in X$ et $\sum_{i=1}^n g_i(x) = 1$ pour $x \in K$. Pour toute fonction $f \in \mathcal{K}(X, K ; C)$, on peut donc écrire $f = \sum_{i=1}^n fg_i$, et on a
$$
fg_i \in \mathcal{K}(X, K_{x_i} ; C),
$$
et $\| fg_i \| \leq \| f \|$; si $M = \sum_{i=1}^n M_{x_i}$, on a donc la relation (4).

Nous désignerons par $\mathcal{M}(X ; C)$, ou simplement $\mathcal{M}(X)$ si aucune confusion n’en résulte, l’espace vectoriel des mesures sur $X$, autrement dit le dual de $\mathcal{K}(X ; C)$. On sait que pour tout ensemble $\mathfrak{S}$ de parties bornées de $\mathcal{K}(X ; C)$, on a défini sur $\mathcal{M}(X ; C)$ la $\mathfrak{S}\text{-topologie}$, qui est localement convexe (*Esp. vect. top.*, chap. IV, § 2, n° 3). Nous désignerons l’espace vectoriel topologique obtenu en munissant $\mathcal{M}(X ; C)$ de la $\mathfrak{S}\text{-topologie}$ par $\mathcal{M}_{\mathfrak{S}}(X ; C)$, ou $\mathcal{M}_{\mathfrak{S}}(X)$.

#### Proposition 7 {#int-iii-s1-prop-7 .statement}

*Pour tout ensemble $\mathfrak{S}$ de parties bornées de $\mathcal{K}(X ; C)$ qui est un recouvrement de $\mathcal{K}(X ; C)$, l’espace $\mathcal{M}_{\mathfrak{S}}(X ; C)$ est séparé et quasi-complet.*

Cela résulte de ce que $\mathcal{K}(X ; C)$ est tonnelé (*Esp. vect. top.*, chap. III, § 3, n° 7, cor. 2 du th. 4).

*Exemples de mesures.* — I. *Mesures atomiques*. Soient $X$ un espace localement compact, $a$ un point de $X$; l’application $f \mapsto f(a)$ de $X$ dans $C$ vérifie évidemment la condition (4) avec $M_K = 1$ pour toute partie compacte $K$ de $X$ contenant $a$, donc est une mesure sur $X$, qu’on désigne par $\varepsilon_a$; on dit que c’est la *mesure de Dirac* au point $a$, ou encore la mesure définie par la *masse unité placée au point* $a$.

Plus généralement, soit $\alpha$ une application de $X$ dans $C$, telle que, pour toute partie compacte $K$ de $X$, on ait $\sum_{x \in K} |\alpha(x)| < +\infty$. Alors, pour toute fonction $f \in \mathcal{K}(X, K ; C)$, la somme
$$
\mu(f) = \sum_{x \in X} \alpha(x) f(x)
$$
est définie, étant égale à $\sum_{x \in K} \alpha(x) f(x)$; il est clair que $\mu$ est une forme linéaire sur $\mathcal{K}(X ; C)$, et que pour $f \in \mathcal{K}(X, K ; C)$, on a
$$
|\mu(f)| \leq \left( \sum_{x \in K} |\alpha(x)| \right) \cdot \| f \|
$$
autrement dit la condition (4) est vérifiée.

On dit qu’une mesure $\mu$ sur $X$ est *atomique* s’il existe une application $\alpha$ de $X$ dans $\mathbf{C}$ telle que $\sum_{x \in K} |\alpha(x)| < +\infty$ pour toute partie compacte $K$ de $X$, et telle que $\mu$ soit égale à la mesure définie comme ci-dessus. Si $N$ est l’ensemble des $x \in X$ tels que $\alpha(x) \neq 0$, la condition imposée à $\alpha$ entraîne que pour toute partie compacte $K$ de $X$, $K \cap N$ est *dénombrable*. On dit aussi que $\mu$ est définie par *les masses* $\alpha(x)$ *placées aux points* $x \in N$. Si l’on suppose que $N \cap K$ est *fini* pour tout ensemble compact $K \subset X$, on a évidemment $\sum_{x \in K} |\alpha(x)| < +\infty$; il revient au même de dire que $N$ est un sous-espace *fermé et discret* de $X$, car tout point de $X$ possède alors un voisinage compact ne contenant qu’un nombre fini de points de $N$, et inversement, s’il en est ainsi, toute partie compacte de $X$ peut être recouverte par un nombre fini de tels voisinages. Lorsque $N$ est fermé et discret, toute mesure atomique définie par une fonction $\alpha$ telle que $\alpha(x) = 0$ dans $\mathbf{C}N$ est appelée mesure *discrète* sur $X$ (cf. § 2, n° 5).

II. *Mesure de Lebesgue.* Pour toute fonction $f \in \mathcal{K}(\mathbf{R}; \mathbf{C})$, il existe un intervalle compact $[a, b]$ de $\mathbf{R}$ en dehors duquel $f$ est nulle. L’intégrale
$$
I(f) = \int_{-\infty}^{+\infty} f(x) \, dx = \int_a^b f(x) \, dx
$$
est donc définie; en outre, d’après le th. de la moyenne (*Fonct. var. réelle*, chap. II, § 1, n° 5, prop. 6), on a $|I(f)| \leq (b - a) \|f\|$; cela montre que $f \mapsto I(f)$ est une mesure sur $\mathbf{R}$, qu’on appelle *mesure de Lebesgue*.

Pour tout intervalle $J$ (borné ou non) de $\mathbf{R}$, on appelle de même *mesure de Lebesgue sur* $J$ la mesure $f \mapsto \int_J f(x) \, dx$, forme linéaire sur $\mathcal{K}(J; \mathbf{C})$ (l’intégrale ayant un sens puisqu’il existe un intervalle compact $[a, b]$ contenu dans $J$ en dehors duquel $f$ est nulle).

III. Soit $g$ une application continue d’un intervalle compact $I \subset \mathbf{R}$ dans $\mathbf{C}$, admettant une dérivée continue dans $I$. Soit $\Gamma = g(I)$, qui est un sous-espace compact de $\mathbf{C}$; l’application
$$
f \mapsto \int_I f(g(t))g'(t) \, dt
$$
de $\mathcal{C}(\Gamma; \mathbf{C})$ dans $\mathbf{C}$ est une forme linéaire continue en vertu du th. de la moyenne, donc une *mesure complexe sur* $\Gamma$; l’intégrale relative à cette mesure s’écrit aussi $\int_{\Gamma} f(z)\,dz$, bien qu’elle dépende, non seulement de $\Gamma$, mais de $g$.

#### Remarque {#int-iii-s1-n3-rem-1 .statement}

La donnée d’une mesure $\mu$ sur un espace localement compact $X$ définit sur $X$ (avec la topologie de $X$) une structure $\mathcal{S}$. Soient $X_1$ un second ensemble, $\varphi$ une application bijective de $X$ sur $X_1$; conformément aux définitions générales (Ens. R, § 9), la structure $\mathcal{S}_1$ obtenue en transportant à $X_1$ la structure $\mathcal{S}$ de $X$ au moyen de $\varphi$, se définit de la façon suivante. On transporte par $\varphi$ la topologie de $X$ à $X_1$; les fonctions de $\mathscr{K}(X_1; \mathbf{C})$ sont alors les fonctions $f$ telles que $f \circ \varphi$ appartienne à $\mathscr{K}(X; \mathbf{C})$, et la mesure $\mu_1$ sur $X_1$ est définie par $\mu_1(f) = \mu(f \circ \varphi)$.

En particulier, un automorphisme de la structure $\mathcal{S}$ est un homéomorphisme $\sigma$ de $X$ sur lui-même tel que l’on ait

$$
\mu(f) = \mu(f \circ \sigma)
$$

pour toute fonction $f \in \mathscr{K}(X; \mathbf{C})$; on dit encore alors que la mesure $\mu$ est invariante par l’homéomorphisme $\sigma$.

#### Exemple {#int-iii-s1-n3-exa-1 .statement}

La mesure de Lebesgue sur $\mathbf{R}$ est invariante par toute translation du groupe additif $\mathbf{R}$. En effet, pour toute fonction $f \in \mathscr{K}(\mathbf{R}; \mathbf{C})$ et tout nombre réel $a$, on a, par la formule du changement de variables (Fonct. var. réelle, chap. II, § 2, n° 1, formule (1))

$$
\int_{-\infty}^{+\infty} f(x + a)\,dx = \int_{-\infty}^{+\infty} f(t)\,dt.
$$

Pour une généralisation, voir chap. VII.

### 4. Produit d’une mesure par une fonction continue

Soient $X$ un espace localement compact, $g$ une application continue de $X$ dans $\mathbf{C}$. Il est clair que $f \mapsto gf$ est une application linéaire de $\mathscr{K}(X; \mathbf{C})$ dans lui-même; montrons que cette application est continue. En effet, pour toute partie compacte $K$ de $X$, et toute fonction $f \in \mathscr{K}(X, K; \mathbf{C})$, on a $gf \in \mathscr{K}(X, K; \mathbf{C})$; en outre, si $b_K = \sup_{x \in K} |g(x)|$, on a $\|gf\| \leq b_K \|f\|$, d’où notre assertion (Esp. vect. top., chap. II, 2e éd., § 4, n° 4, prop. 5). La transposée de cette application linéaire continue (Esp. vect. top., chap. II, 2e éd., § 6, n° 4) est donc une application linéaire de $\mathscr{M}(X; \mathbf{C})$ dans lui-même, que l’on note $\mu \mapsto g.\mu$ (ou $\mu \mapsto g\mu$ si cela n’entraîne pas confusion). Si $\nu = g.\mu$, on a donc, pour toute fonction $f \in \mathcal{K}(X; \mathbf{C})$,

(6) $$
\langle f, v \rangle = \langle gf, \mu \rangle
$$

ou encore

$$
\int f(x)\, dv(x) = \int f(x)g(x)\, d\mu(x)
$$

(ce que l’on abrège sous la forme $dv(x) = g(x)\, d\mu(x)$). On dit que $g.\mu$ est le produit de la mesure $\mu$ par la fonction $g$, ou encore la mesure de densité $g$ par rapport à $\mu$ (cf. chap. V, § 5). Si $g_1, g_2$ sont deux applications continues de $X$ dans $\mathbf{C}$, $\mu_1, \mu_2$ deux mesures sur $X$, on a

$$
(g_1 + g_2).\mu = g_1.\mu + g_2.\mu, \qquad g.(\mu_1 + \mu_2) = g.\mu_1 + g.\mu_2,
$$
$$
(g_1g_2).\mu = g_1.(g_2.\mu).
$$

On a en outre $1.\mu = \mu$ (1 désignant ici la fonction constante égale à 1 dans $X$); muni de la loi de composition externe $(g, \mu) \mapsto g.\mu$ et de sa structure additive, l’ensemble $\mathcal{M}(X; \mathbf{C})$ est donc un module sur l’anneau $\mathcal{C}(X; \mathbf{C})$.

### 5. Mesures réelles. Mesures positives

Soit $X$ un espace localement compact. L’espace vectoriel réel $\mathcal{K}(X; \mathbf{R})$ est un sous-espace de l’espace vectoriel réel sous-jacent à l’espace vectoriel complexe $\mathcal{K}(X; \mathbf{C})$; en outre, l’application $(f_1, f_2) \mapsto f_1 + if_2$ est un isomorphisme de l’espace vectoriel topologique produit $\mathcal{K}(X; \mathbf{R}) \times \mathcal{K}(X; \mathbf{R})$ sur l’espace vectoriel topologique réel $\mathcal{K}(X; \mathbf{C})$ (n° 1, prop. 1).

Pour toute mesure (complexe) $\mu \in \mathcal{M}(X; \mathbf{C})$, la restriction $\mu_0$ de $\mu$ à $\mathcal{K}(X; \mathbf{R})$ est une application $\mathbf{R}$-linéaire continue de $\mathcal{K}(X; \mathbf{R})$ dans $\mathbf{C}$; cette restriction détermine d’ailleurs $\mu$, car si $f = f_1 + if_2$ avec $f_1, f_2$ dans $\mathcal{K}(X; \mathbf{R})$, on a $\mu(f) = \mu_0(f_1) + i\mu_0(f_2)$. Réciproquement, soit $\mu_0$ une application $\mathbf{R}$-linéaire continue de $\mathcal{K}(X; \mathbf{R})$ dans $\mathbf{C}$; il est clair que l’application

$$
f_1 + if_2 \mapsto \mu_0(f_1) + i\mu_0(f_2)
$$

est une mesure (complexe) sur $X$. On peut donc identifier toute mesure sur $X$ à sa restriction à $\mathcal{K}(X; \mathbf{R})$.

Soit $\mu$ une mesure sur $X$. On appelle mesure conjuguée de $\mu$ la mesure $\bar{\mu}$ définie par $\bar{\mu}(f) = \overline{\mu(\bar{f})}$ pour toute fonction $f \in \mathcal{K}(X; \mathbf{C})$; il est clair en effet que $\bar{\mu}$ est une forme $\mathbf{C}$-linéaire et qu’elle est continue dans $\mathcal{K}(X; \mathbf{C})$; on a évidemment $\bar{\mu} = \mu$, et pour deux mesures $\mu, \nu$ et deux scalaires $\alpha, \beta$ dans $\mathbf{C}$,

$$
(\alpha \mu + \beta \nu) = \overline{\alpha} \cdot \bar{\mu} + \overline{\beta} \cdot \bar{\nu}.
$$

Plus généralement, pour toute fonction $g \in \mathcal{C}(X; \mathbf{C})$ et toute mesure $\mu$ sur $X$, on a

(7)

$$
\overline{g \cdot \mu} = \overline{g} \cdot \bar{\mu}
$$

comme il résulte aussitôt de la définition (n° 4).

On dit qu’une mesure $\mu$ sur $X$ est réelle si $\bar{\mu} = \mu$; d’après ce qui précède, il revient au même de dire que pour toute fonction $f \in \mathcal{K}(X; \mathbf{R})$, $\mu(f)$ est un nombre réel. Si l’on identifie une mesure réelle à sa restriction à $\mathcal{K}(X; \mathbf{R})$, on peut donc dire que l’ensemble des mesures réelles sur $X$ est le dual de l’espace localement convexe réel $\mathcal{K}(X; \mathbf{R})$; c’est un espace vectoriel réel que l’on note $\mathcal{M}(X; \mathbf{R})$ (ou parfois $\mathcal{M}(X)$ lorsque cela ne crée pas de confusion). La mesure de Lebesgue sur $\mathbf{R}$ est une mesure réelle, ainsi que la mesure de Dirac $\varepsilon_a$ pour tout point $a \in X$. Si $g \in \mathcal{C}(X; \mathbf{R})$ et si $\mu$ est une mesure réelle, il en est de même de $g \cdot \mu$ en vertu de (7).

Soit $\mu$ une mesure (complexe) sur $X$. En vertu de la définition précédente, les mesures $\mu_1 = (\mu + \bar{\mu})/2$ et $\mu_2 = (\mu - \bar{\mu})/2i$ sont réelles; on les appelle respectivement partie réelle et partie imaginaire de $\mu$ et on les note respectivement $\Re \mu$ et $\Im \mu$; ces mesures sont encore caractérisées par le fait que, pour toute fonction $f \in \mathcal{K}(X; \mathbf{R})$, on a

$$
\mu_1(f) = \Re(\mu(f)), \qquad \mu_2(f) = \Im(\mu(f)).
$$

On a évidemment

$$
\mu = \mu_1 + i \mu_2, \qquad \bar{\mu} = \mu_1 - i \mu_2.
$$

L’espace $\mathcal{K}(X; \mathbf{R})$ des fonctions numériques continues dans $X$ et à support compact est évidemment un espace de Riesz pour la relation d’ordre $f \leqslant g$. Nous dirons qu’une mesure réelle $\mu$ sur $X$ est positive si, pour toute fonction $f \geqslant 0$ appartenant à $\mathcal{K}(X; \mathbf{R})$, on a $\mu(f) \geqslant 0$; c’est donc une forme linéaire positive sur l’espace de Riesz $\mathcal{K}(X; \mathbf{R})$ (chap. II, § 2, n° 1, déf. 1). Inversement:

#### Théorème 1 {#int-iii-s1-thm-1 .statement}

Toute forme linéaire positive sur l’espace de Riesz $\mathcal{K}(X; \mathbf{R})$ est une mesure réelle (positive) sur $X$.

En effet, soit $\mu$ une forme linéaire positive sur $\mathcal{K}(X; \mathbf{R})$, et soit $K$ une partie compacte de $X$. Il existe une application continue $f_0$ de $X$ dans $[0, 1]$, à support compact, telle que $f_0(x) = 1$ dans $K$ (n° 2, lemme 1). Pour toute fonction $g \in \mathcal{K}(X, K; \mathbf{R})$, on a donc $-\|g\|f_0 \leq g \leq \|g\|f_0$, et par suite $|\mu(g)| \leq \|g\|\cdot\mu(f_0)$, ce qui démontre le théorème.

On désigne par $\mathcal{M}_+(X)$ le cône pointé des mesures positives sur $X$ (ou ce qui revient au même, le cône des formes linéaires positives sur l’espace de Riesz $\mathcal{K}(X; \mathbf{R})$).

#### Théorème 2 {#int-iii-s1-thm-2 .statement}

*Toute mesure réelle sur un espace localement compact $X$ est différence de deux mesures positives.*

En vertu du th. 1 et du chap. II, § 2, n° 2, th. 1, tout revient à prouver qu’une mesure réelle $\mu$ sur $X$ est une forme linéaire relativement *bornée* sur l’espace de Riesz $\mathcal{K}(X; \mathbf{R})$. Or, soit $f$ une fonction continue $\geq 0$ dans $X$, à support compact $K$; la relation $0 \leq g \leq f$ dans $\mathcal{K}(X; \mathbf{R})$ entraîne que $\|g\| \leq \|f\|$ et que le support de $g$ est contenu dans $K$. Par hypothèse, il existe un nombre $M_K \geq 0$ tel que l’on ait $|\mu(h)| \leq M_K\cdot\|h\|$ pour toute fonction $h \in \mathcal{K}(X, K; \mathbf{R})$; on a donc $|\mu(g)| \leq M_K\cdot\|g\| \leq M_K\cdot\|f\|$, ce qui prouve le théorème.

L’espace $\mathcal{M}(X; \mathbf{R})$ des mesures réelles sur $X$ est donc identique à l’espace des formes linéaires relativement bornées sur l’espace de Riesz $\mathcal{K}(X; \mathbf{R})$; rappelons que dans $\mathcal{M}(X; \mathbf{R})$, la relation d’ordre $\mu \leq v$ signifie que $v - \mu$ est une mesure positive, ou encore que, pour toute fonction $f \in \mathcal{K}_+(X)$, on a $\mu(f) \leq v(f)$.

#### Théorème 3 {#int-iii-s1-thm-3 .statement}

*L’espace $\mathcal{M}(X; \mathbf{R})$ des mesures réelles sur un espace localement compact $X$ est complètement réticulé.*

Cela résulte du chap. II, § 2, n° 2, th. 1.

Conformément aux notations du chap. II, § 2, on posera, pour toute mesure *réelle* $\mu$ sur $X$,

$$
\mu^+ = \sup (\mu, 0) \qquad \mu^- = \sup (-\mu, 0), \qquad |\mu| = \sup (\mu, -\mu);
$$

on a $\mu = \mu^+ - \mu^-$, $|\mu| = \mu^+ + \mu^-$ et $\inf(\mu^+, \mu^-) = 0$. En outre, pour toute fonction $f \in \mathcal{K}_+(X)$, on a

$$
\int f d\mu^+ = \sup_{0 \leq g \leq f, g \in \mathcal{K}(X)} \int g\, d\mu
$$

et

$$
\int f d|\mu| = \sup_{|g| \leq f,\ g \in \mathcal{K}(X)} \int g\ d\mu
$$

d’où en particulier, pour toute fonction $f \in \mathcal{K}(X; \mathbf{R})$

$$
|\int f d\mu| \leq \int |f|\ d|\mu|.
$$

Cette inégalité est encore vraie si $f \in \mathcal{K}(X; \mathbf{C})$; en effet, en multipliant $f$ par un nombre complexe de valeur absolue 1 (ce qui ne modifie pas les deux membres), on peut supposer que $\int f\ d\mu \geq 0$. Alors $|\int f\ d\mu| = \int f\ d\mu = \int (\Re f)\ d\mu \leq \int |\Re f|\ d|\mu| \leq \int |f|\ d|\mu|$.

### 6. Valeur absolue d’une mesure complexe

Soit $\mu$ une mesure complexe sur un espace localement compact $X$; pour toute fonction $f \in \mathcal{K}_+(X)$, le nombre réel positif

$$
L(f) = \sup_{|g| \leq f,\ g \in \mathcal{K}(X; \mathbf{C})} |\int g\ d\mu|
$$

est *fini*, car la relation $|g| \leq f$ entraîne $\operatorname{Supp}(g) \subset \operatorname{Supp}(f)$ et $\|g\| \leq \|f\|$, donc notre assertion résulte de la formule (4) du n° 3. Montrons que $L$ se prolonge d’une seule manière en une *mesure positive* sur $X$; compte tenu du n° 5, th. 1, et du chap. II, § 2, n° 1, prop. 3, il suffira de montrer que si $f_1, f_2$ sont deux fonctions de $\mathcal{K}_+(X)$, on a $L(f_1 + f_2) = L(f_1) + L(f_2)$. Or, si $|g_1| \leq f_1,\ |g_2| \leq f_2,\ g_1$ et $g_2$ étant deux fonctions de $\mathcal{K}(X; \mathbf{C})$, on a $|g_1 + \zeta g_2| \leq f_1 + f_2$ quel que soit le nombre complexe $\zeta$ de valeur absolue 1, donc

$$
|\mu(g_1 + \zeta g_2)| = |\mu(g_1) + \zeta \mu(g_2)| \leq L(f_1 + f_2).
$$

Mais on peut supposer $\zeta$ choisi de sorte que

$$
|\mu(g_1) + \zeta \mu(g_2)| = |\mu(g_1)| + |\mu(g_2)|;
$$

comme $|\mu(g_i)|$ est arbitrairement voisin de $L(f_i)$ ($i = 1, 2$) cela prouve que $L(f_1) + L(f_2) \leq L(f_1 + f_2)$. Considérons d’autre part une fonction $g \in \mathcal{K}(X; \mathbf{C})$ telle que $|g| \leq f_1 + f_2$. La fonction $g_i$ égale à $gf_i/(f_1 + f_2)$ aux points où $f_1(x) + f_2(x) \neq 0$, à 0 ailleurs ($i = 1, 2$), est continue dans $X$, car $f_i/(f_1 + f_2)$ ($i = 1, 2$) est continue en tout point où $f_1(x) + f_2(x) \neq 0$ et on a $|g_i(x)| \leq |g(x)|$ pour tout $x \in X$, ce qui prouve la continuité de $g_i$ aux points où $f_1(x) + f_2(x) = 0$ ($i = 1, 2$), puisqu’en ces points on a aussi $g(x) = 0$. Il est clair que $|g_i| \leq f_i$ ($i = 1, 2$) et $g = g_1 + g_2$, donc $|\mu(g)| \leq |\mu(g_1)| + |\mu(g_2)| \leq L(f_1) + L(f_2)$; comme $|\mu(g)|$ est arbitrairement voisin de $L(f_1 + f_2)$, on a $L(f_1 + f_2) \leq L(f_1) + L(f_2)$, ce qui achève de prouver notre assertion.

Lorsque $\mu$ est une mesure réelle, il résulte de la formule (9) que l’on a $|\mu| \leq L$ ; mais d’autre part, en vertu de la fin du n° 5, on a, pour $g \in \mathcal{K}(X; \mathbf{C})$ et $|g| \leq f \in \mathcal{K}_+(X)$, $|\int g\,d\mu| \leq \int |g|\cdot d|\mu| \leq \int f\,d|\mu|$, donc par définition $L \leq |\mu|$, autrement dit $L = |\mu|$.

On désigne encore la mesure positive $L$ par $|\mu|$ pour une mesure complexe quelconque $\mu$, et on dit que $|\mu|$ est la valeur absolue de $\mu$. La définition de $|\mu|$ s’écrit donc

(12)
$$
|\mu|(f) = \sup_{|g| \leq f,\, g \in \mathcal{K}(X; \mathbf{C})} |\mu(g)|
$$
et par suite on a, pour toute fonction $g \in \mathcal{K}(X; \mathbf{C})$
(13)
$$
|\int g\,d\mu| \leq \int |g|\,d|\mu|.
$$

Il est clair que pour tout scalaire $\alpha \in \mathbf{C}$ et toute mesure $\mu$ sur X, on a
(14)
$$
|\alpha \mu| = |\alpha|\cdot|\mu|.
$$

D’autre part, si $\mu$ et $\nu$ sont deux mesures sur X, $f$ une fonction de $\mathcal{K}_+(X)$, $g$ une fonction de $\mathcal{K}(X; \mathbf{C})$ telle que $|g| \leq f$, on a
$$
\left| \int g\,d(\mu + \nu) \right| = \left| \int g\,d\mu + \int g\,d\nu \right| \leq \int f\,d|\mu| + \int f\,d|\nu|
$$
d’où
(15)
$$
|\mu + \nu| \leq |\mu| + |\nu|.
$$
Avec les mêmes notations, les relations $|g| \leq f$ et $|\bar{g}| \leq f$ sont équivalentes, donc on a
(16)
$$
|\overline{\mu}| = |\mu|.
$$
On déduit de (14), (15) et (16) que l’on a
(17)
$$
|\mathcal{R}\mu| \leq |\mu|, \quad |\mathcal{I}\mu| \leq |\mu|, \quad |\mu| \leq |\mathcal{R}\mu| + |\mathcal{I}\mu|.
$$

#### Proposition 8 {#int-iii-s1-prop-8 .statement}

Si $\mu$ est une mesure sur X, on a, pour toute fonction $h \in \mathcal{C}(X; \mathbf{C})$,
(18)
$$
|h \cdot \mu| \leq |h|\cdot|\mu|.
$$

En effet, si $f \in \mathcal{K}_+(X)$ et si $g \in \mathcal{K}(X; \mathbf{C})$ est tel que $|g| \leq f$, on a, en vertu de (13), $|\int gh\,d\mu| \leq \int |gh|\,d|\mu| \leq \int f|h|\,d|\mu|$, ce qui prouve (18).

### 7. Définition d’une mesure par prolongement

Soit X un espace localement compact; si V est un sous-espace vectoriel dense dans $\mathcal{K}(X; \mathbf{C})$, il est clair que deux mesures $\mu_1, \mu_2$ sur X qui coïncident dans V sont égales, et que toute forme linéaire sur V continue pour la topologie induite par celle de $\mathcal{K}(X; \mathbf{C})$ se prolonge (d’une seule manière) en une mesure sur X. Un critère plus maniable pour les mesures positives est le suivant:

#### Proposition 9 {#int-iii-s1-prop-9 .statement}

Soit V un sous-espace vectoriel de $\mathcal{K}(X; \mathbf{R})$ possédant la propriété suivante:
(P) Pour toute partie compacte K de X, il existe une fonction $f \in V$ telle que $f \geqslant 0$ et que $f(x) > 0$ pour tout $x \in K$.
Dans ces conditions, toute forme linéaire positive sur V pour l’ordre induit par celui de $\mathcal{K}(X; \mathbf{R})$ (chap. II, § 2, n° 1, déf. 1) se prolonge en une mesure positive sur X (qui est unique lorsque V est dense dans $\mathcal{K}(X; \mathbf{R})$).

Pour toute fonction $f \in \mathcal{K}(X; \mathbf{R})$, de support K, il existe une fonction $g \in V$ telle que $f \leqslant g$: il y a en effet une fonction $h \geqslant 0$ dans V telle que $h(x) > 0$ pour tout $x \in K$; si l’on pose $\alpha = \inf_{x \in K} h(x)$, on a donc $\alpha > 0$, et la fonction $(\alpha^{-1} \| f \|)h = g$ répond à la question. Il suffit par suite d’appliquer le th. 1 du n° 5 et la prop. 1 d’Esp. vect. top., chap. II, 2e éd., § 3, n° 1.

### 8. Mesures bornées

Soit X un espace localement compact. Comme la topologie induite sur $\mathcal{K}(X; \mathbf{C})$ par celle de $C^b(X; \mathbf{C})$ est moins fine que la topologie limite inductive sur $\mathcal{K}(X; \mathbf{C})$, une mesure sur X n’est pas nécessairement continue pour la topologie de la convergence uniforme dans X.

#### Définition 3 {#int-iii-s1-def-3 .statement}

On dit qu’une mesure sur un espace localement compact X est bornée si elle est continue dans $\mathcal{K}(X; \mathbf{C})$ pour la topologie de la convergence uniforme.

Il revient au même de dire qu’il existe un nombre fini M $\geqslant 0$ tel que pour toute fonction $f \in \mathcal{K}(X; \mathbf{C})$, on ait
(19) $|\mu(f)| \leqslant M \| f \|$ (où $\| f \|$ est définie par la formule (3) du n° 2).

Dire que $\mu$ est une mesure bornée signifie donc que $\mu$ appartient au dual de l’espace $\mathcal{H}(X; \mathbf{C})$ normé par $\|f\|$; nous désignerons ce dual par $\mathcal{M}^1(X; \mathbf{C})$ (ou simplement $\mathcal{M}^1(X)$ si cela n’entraîne pas de confusion). On sait que $\mathcal{M}^1(X; \mathbf{C})$ est muni d’une norme, $\|\mu\|$ étant le plus petit des nombres $M \geqslant 0$ pour lesquels l’inégalité (19) a lieu pour toute fonction $f \in \mathcal{H}(X; \mathbf{C})$, ou encore
$$
\|\mu\| = \sup_{\|f\| \leqslant 1, f \in \mathcal{H}(X; \mathbf{C})} |\mu(f)|.
$$
Muni de cette norme, on sait que $\mathcal{M}^1(X; \mathbf{C})$ est un espace de Banach (*Esp. vect. top.*, chap. IV, § 5, n° 1).

La définition de $\|\mu\|$ par la formule (20) s’étend à toute mesure $\mu$ sur $X$ et on dit encore, par abus de langage, que $\|\mu\|$ est la norme de $\mu$; pour que $\mu$ soit bornée, il faut et il suffit que $\|\mu\|$ soit fini.

Si $X$ est compact, toute mesure sur $X$ est bornée.

#### Exemple 1 {#int-iii-s1-n8-exa-1 .statement}

La mesure $\varepsilon_a$ définie par la masse unité en un point $a \in X$ est bornée, et on a $\|\varepsilon_a\| = 1$.

#### Exemple 2 {#int-iii-s1-n8-exa-2 .statement}

La mesure de Lebesgue sur $\mathbf{R}$ n’est pas bornée : en effet, pour tout entier $n > 0$, il existe une fonction $f \in \mathcal{H}(\mathbf{R}; \mathbf{C})$, à valeurs dans $[0, 1]$ et égale à 1 dans l’intervalle $[-n, n]$ (n° 2, lemme 1); on a donc $\|f\| = 1$ et
$$
\int_{-\infty}^{+\infty} f(x)\, dx \geqslant \int_{-n}^{n} f(x)\, dx = 2n,
$$
ce qui prouve qu’il n’existe aucun nombre fini $M$ vérifiant la relation (19).

#### Exemple 3 {#int-iii-s1-n8-exa-3 .statement}

Sur la droite numérique $\mathbf{R}$, l’application
$$
f \mapsto \int_{-\infty}^{+\infty} \frac{f(x)\, dx}{1 + x^2}
$$
est une mesure bornée, car pour toute fonction $f \in \mathcal{H}(\mathbf{R}; \mathbf{C})$, on a
$$
\left| \int_{-\infty}^{+\infty} \frac{f(x)\, dx}{1 + x^2} \right| \leqslant \|f\| \int_{-\infty}^{+\infty} \frac{dx}{1 + x^2} = \pi \cdot \|f\|.
$$

Comme les relations $\|f\| \leqslant 1$ et $\|\bar{f}\| \leqslant 1$ sont équivalentes, il résulte de (20) que pour toute mesure $\mu$ sur $X$, on a
$$
\|\bar{\mu}\| = \|\mu\|.
$$

#### Proposition 10 {#int-iii-s1-prop-10 .statement}

*Pour toute mesure $\mu$ sur $X$, on a*
$$
\|\mu\| = \sup_{0 \leqslant f \leqslant 1, f \in \mathcal{H}(X; \mathbf{R})} |\mu|(f).
$$

En effet, compte tenu de la formule (12) qui définit la valeur absolue d’une mesure, le second membre de (22) s’écrit

$$
\sup_{0 \leq f \leq 1, f \in \mathcal{K}(X; \mathbf{R})} \left( \sup_{|g| \leq f, g \in \mathcal{K}(X; \mathbf{C})} |\mu(g)| \right) = \sup_{||g|| \leq 1, g \in \mathcal{K}(X; \mathbf{C})} |\mu(g)|.
$$

#### Corollaire 1 {#int-iii-s1-prop-10-cor-1 .statement}

*Pour toute mesure $\mu$ sur $X$, les normes de $\mu$ et de $|\mu|$ sont égales ; pour que $\mu$ soit bornée, il faut et il suffit que $|\mu|$ le soit.*

#### Corollaire 2 {#int-iii-s1-prop-10-cor-2 .statement}

*Pour toute mesure $\mu$ sur un espace compact $X$, on a*

$$
\|\mu\| = |\mu|(1) = \int d|\mu|.
$$

Cette formule sera généralisée au chap. IV, § 4, n° 7.

Sur un espace *compact* $X$, pour toute mesure $\mu$ (complexe) sur $X$, le nombre complexe $\mu(1)$ est appelé la *masse totale* de $\mu$. Lorsque $\mu$ est *positive*, sa masse totale est donc égale à sa norme. Lorsque $\mu$ est une mesure positive sur un espace *compact* $X$, de masse totale égale à 1, on dit encore que sa valeur $\mu(f)$ pour une fonction continue $f \in \mathcal{C}(X; \mathbf{C})$ est la *moyenne* de $f$ par rapport à la mesure $\mu$.

#### Corollaire 3 {#int-iii-s1-prop-10-cor-3 .statement}

*Pour toute mesure réelle $\mu$ sur un espace localement compact $X$, on a*

$$
\|\mu\| = \sup_{\|f\| \leq 1, f \in \mathcal{K}(X; \mathbf{R})} |\mu(f)|.
$$

Il suffit d’utiliser la formule (22) et l’expression (9) de $|\mu|(f)$ lorsque $\mu$ est une mesure réelle et $f \in \mathcal{K}_+(X)$.

L’ensemble des mesures réelles bornées est donc le dual de l’espace *normé* $\mathcal{K}(X; \mathbf{R})$; on le note $\mathcal{M}^1(X; \mathbf{R})$, ou $\mathcal{M}^1(X)$ s’il n’en résulte pas de confusion. L’injection canonique

$$
\mathcal{M}^1(X; \mathbf{R}) \to \mathcal{M}^1(X; \mathbf{C})
$$

est une *isométrie* en vertu de (24).

#### Proposition 11 {#int-iii-s1-prop-11 .statement}

*Si $\mu$ et $\nu$ sont deux mesures positives sur $X$, on a* $\|\mu + \nu\| = \|\mu\| + \|\nu\|$.

En effet, les fonctions $f \in \mathcal{K}(X; \mathbf{R})$ telles que $0 \leq f \leq 1$ forment un ensemble filtrant S pour la relation $\leq$. Pour une mesure positive $\mu$ sur $X$, il résulte donc de (22) et du th. de la limite monotone, que l’on a $\| \mu \| = \lim_{f \in S} \mu(f)$; la conclusion de la proposition en résulte aussitôt.

#### Corollaire 1 {#int-iii-s1-prop-11-cor-1 .statement}

Si $\mu$ et $\nu$ sont deux mesures positives sur $X$ telles que $\mu \leq \nu$, on a $\| \mu \| \leq \| \nu \|$; en particulier, si $\nu$ est bornée, $\mu$ l’est aussi.
En effet, on a $\| \nu \| = \| \mu \| + \| \nu - \mu \|$.

#### Corollaire 2 {#int-iii-s1-prop-11-cor-2 .statement}

Pour toute mesure réelle $\mu$ sur $X$, on a
$$
\| \mu \| = \| \mu^+ \| + \| \mu^- \|.
$$
En effet (cor. 1 de la prop. 10), la norme de $\mu$ est égale à celle de $|\mu| = \mu^+ + \mu^-$.

#### Proposition 12 {#int-iii-s1-prop-12 .statement}

Si $\mu$ est une mesure bornée sur $X$ et $g$ une application continue et bornée de $X$ dans $\mathbf{C}$, la mesure $g.\mu$ est bornée et l’on a $\| g.\mu \| \leq \| g \| . \| \mu \|$.
En effet, pour toute fonction $f \in \mathcal{K}(X; \mathbf{C})$, on a
$$
|\mu(fg)| \leq \| \mu \| . \| fg \| \leq \| \mu \| . \| g \| . \| f \|.
$$

### 9. Topologie vague sur l’espace des mesures

Soit $X$ un espace localement compact. Sur l’espace $\mathcal{M}(X; \mathbf{C})$, on peut considérer la topologie de la convergence simple dans $\mathcal{K}(X; \mathbf{C})$, que nous appellerons topologie vague sur $\mathcal{M}(X; \mathbf{C})$.
Comme $\mathcal{K}(X; \mathbf{C}) = \mathcal{K}(X; \mathbf{R}) + i \mathcal{K}(X; \mathbf{R})$, la topologie vague sur $\mathcal{M}(X; \mathbf{C})$ est définie par les semi-normes $\sup_{1 \leq i \leq n} |\mu(f_i)|$, où $(f_i)_{1 \leq i \leq n}$ est une suite finie quelconque de fonctions de $\mathcal{K}(X; \mathbf{R})$ (ou de $\mathcal{K}_+(X)$). Dire qu’un filtre $\mathfrak{F}$ sur $\mathcal{M}(X; \mathbf{C})$ converge vaguement vers une mesure $\mu_0$ signifie que, pour toute fonction $f \in \mathcal{K}(X; \mathbf{R})$, on a $\mu_0(f) = \lim_{\mu, \mathfrak{F}} \mu(f)$. Pour toute fonction $f \in \mathcal{K}(X; \mathbf{C})$, l’application $\mu \mapsto \mu(f)$ est une forme linéaire vaguement continue dans l’espace $\mathcal{M}(X; \mathbf{C})$.

#### Proposition 13 {#int-iii-s1-prop-13 .statement}

Soient $X$ un espace localement compact, et, pour tout $x \in X$, soit $\varepsilon_x$ la mesure de Dirac au point $x$. L’application $x \mapsto \varepsilon_x$ est un homéomorphisme de $X$ sur un sous-espace de l’espace $\mathcal{M}(X; \mathbf{C})$ des mesures sur $X$, muni de la topologie vague. En outre, si $X'$ désigne l’espace compact obtenu en adjoignant à $X$ un point à l’infini $\omega$, $\varepsilon_x$ tend vers 0 lorsque $x$ tend vers $\omega$.

Pour toute fonction $f \in \mathcal{H}(X; \mathbf{C})$, on a $\langle f, \varepsilon_x \rangle = f(x)$; comme $f$ est continue, cela prouve que l’application $x \mapsto \varepsilon_x$ est continue. Si $x, y$ sont deux points distincts de $X$, il existe une fonction $f \in \mathcal{H}(X; \mathbf{C})$ telle que $f(x) = 1, f(y) = 0$ (n° 2, lemme 1), ce qui prouve que $\varepsilon_x \neq \varepsilon_y$; donc l’application $x \mapsto \varepsilon_x$ est injective. En outre, pour toute fonction $f \in \mathcal{H}(X; \mathbf{C})$, $\langle f, \varepsilon_x \rangle$ tend vers 0 par définition lorsque $x$ tend vers $\omega$, donc $x \mapsto \varepsilon_x$ se prolonge par continuité à $X' = X \cup \{\omega\}$ en prenant la valeur 0 au point $\omega$. Cette application prolongée est encore injective, puisque $\varepsilon_x \neq 0$ pour tout $x \in X$. C’est donc un homéomorphisme de l’espace compact $X'$ sur un sous-espace de $\mathcal{M}(X; \mathbf{C})$, puisque $\mathcal{M}(X; \mathbf{C})$ est séparé pour la topologie vague ($Top.$ gén., chap. I, 3$^e$ éd., § 9, n° 4, cor. 2 du th. 2).

#### Proposition 14 {#int-iii-s1-prop-14 .statement}

Dans l’espace $\mathcal{M}(X; \mathbf{C})$ des mesures sur un espace localement compact $X$, le cône $\mathcal{M}_+(X)$ des mesures positives est complet pour la structure uniforme déduite de la topologie vague (et par suite vaguement fermé dans $\mathcal{M}(X; \mathbf{C})$).

En effet, considérons un filtre de Cauchy $\Phi$ pour la structure uniforme vague sur $\mathcal{M}_+(X)$; par définition, $\mu_0(f) = \lim_{\mu, \Phi} \mu(f)$ existe pour toute fonction $f \in \mathcal{H}(X; \mathbf{C})$, et en vertu du principe de prolongement des inégalités, on a $\mu_0(f) \geqslant 0$ pour toute fonction $f \in \mathcal{H}_+(X)$; $\mu_0$ est par suite une mesure positive sur $X$ (n° 5, th. 1).

On notera que l’espace $\mathcal{M}(X; \mathbf{C})$ (ou $\mathcal{M}(X; \mathbf{R})$) lui-même *n’est pas nécessairement complet* pour la structure uniforme vague (*Esp. vect. top.*, chap. IV, § 1, exerc. 11).

#### Corollaire {#int-iii-s1-n9-cor-1 .statement}

*Si $A$ et $B$ sont deux parties vaguement fermées de $\mathcal{M}_+(X)$, $A + B$ est vaguement fermé dans $\mathcal{M}_+(X)$ (donc aussi dans $\mathcal{M}(X; \mathbf{C})$).*

C’est en effet une propriété générale des cônes saillants faiblement complets dans les espaces localement convexes (*Esp. vect. top.*, chap. II, 2$^e$ éd., § 6, n° 8, cor. 2 de la prop. 11).

#### Proposition 15 {#int-iii-s1-prop-15 .statement}

*Soit $H$ une partie de $\mathcal{M}(X; \mathbf{C})$. Les propriétés suivantes sont équivalentes*:
    a) $H$ est vaguement bornée.
    b) $H$ est vaguement relativement compacte.

c) $H$ est équicontinue.

d) *Pour toute partie compacte $K$ de $X$, il existe un nombre $M_K \geq 0$ tel que, pour toute $\mu \in H$ et toute fonction $f \in \mathcal{K}(X, K ; \mathbf{C})$, on ait $|\mu(f)| \leq M_K \|f\|$.*

Comme $\mathcal{K}(X ; \mathbf{C})$ est un espace tonnelé (n° 1, prop. 2), l’équivalence des propriétés a), b) et c) résulte d’*Esp. vect. top.*, chap. IV, § 2, n° 2, th. 1.

Il est clair que d) entraîne a). Enfin, si $H$ est équicontinue, l’ensemble des restrictions des mesures $\mu \in H$ à $\mathcal{K}(X, K ; \mathbf{C})$ est aussi équicontinu, d’où la condition d), puisque $\mathcal{K}(X, K ; \mathbf{C})$ est un espace normé.

\* Nous verrons au chap. IV, § 4, n° 6, que les conditions de la prop. 15 équivalent encore au fait que pour toute partie compacte $K$ de $X$, il existe une constante $M_K$ telle que $|\mu|(K) \leq M_K$ pour toute mesure $\mu \in H$.*

#### Corollaire 1 {#int-iii-s1-prop-15-cor-1 .statement}

*Soit $v$ une mesure positive sur $X$; l’ensemble des mesures $\mu$ telles que $|\mu| \leq v$ est vaguement compact.*

#### Corollaire 2 {#int-iii-s1-prop-15-cor-2 .statement}

*L’ensemble des mesures $\mu$ telles que $\|\mu\| \leq a$ ($a$ nombre fini $> 0$ quelconque) est vaguement compact.*

#### Corollaire 3 {#int-iii-s1-prop-15-cor-3 .statement}

*Si $X$ est compact, l’ensemble des mesures positives $\mu$ sur $X$ telles que $\|\mu\| = 1$ est vaguement compact.*

En effet, c’est l’intersection de l’ensemble vaguement compact (cor. 2) des mesures $\mu$ telles que $\|\mu\| \leq 1$, et des ensembles vaguement fermés définis respectivement par les relations $\mu \geq 0$ et $\mu(1) = 1$ (n° 8, cor. 2 de la prop. 10).

#### Corollaire 4 {#int-iii-s1-prop-15-cor-4 .statement}

Dans l’espace $\mathcal{M}(X ; \mathbf{C})$, l’application $\mu \mapsto \|\mu\|$ est semi-continue inférieurement pour la topologie vague.

C’est une conséquence immédiate du cor. 2.

On notera que l’application $\mu \mapsto |\mu|$ de $\mathcal{M}(X ; \mathbf{C})$ dans lui-même n’est pas nécessairement continue pour la topologie vague (exerc. 4).

#### Proposition 16 {#int-iii-s1-prop-16 .statement}

Soient $K$ une partie compacte de $X$, $H$ une partie vaguement bornée de $\mathcal{M}(X ; \mathbf{C})$; alors la forme bilinéaire $(f, \mu) \mapsto \langle f, \mu \rangle$ est continue dans $\mathcal{K}(X, K ; \mathbf{C}) \times H$ lorsqu’on munit $\mathcal{K}(X, K ; \mathbf{C})$ de la topologie de la convergence uniforme et $H$ de la topologie vague.

En effet, il existe un nombre $M \geq 0$ tel que, pour toute fonction $f \in \mathcal{K}(X, K ; \mathbf{C})$ et toute mesure $\mu \in H$, on ait
$$
|\mu(f)| \leq M \|f\|
$$
(prop. 15). Si $\mu_0$ et $\mu$ sont deux mesures appartenant à $H$, $f_0$ et $f$ deux fonctions de $\mathcal{K}(X, K ; \mathbf{C})$, on a donc
$$
|\mu(f) - \mu_0(f_0)| = |\mu(f - f_0) + \mu(f_0) - \mu_0(f_0)| \\
\leq M \|f - f_0\| + |\mu(f_0) - \mu_0(f_0)|
$$
et cette dernière quantité est arbitrairement petite avec $\|f - f_0\|$ et $|\mu(f_0) - \mu_0(f_0)|$, ce qui démontre la proposition.

### 10. Convergence compacte dans $\mathcal{M}(X; \mathbf{C})$

Rappelons que la topologie de la convergence compacte sur $\mathcal{M}(X ; \mathbf{C})$ est la topologie de la convergence uniforme dans les parties compactes de $\mathcal{K}(X ; \mathbf{C})$. Nous appellerons topologie de la convergence strictement compacte sur $\mathcal{M}(X ; \mathbf{C})$ la topologie de la convergence uniforme dans les parties strictement compactes (n° 1) de $\mathcal{K}(X ; \mathbf{C})$.

#### Proposition 17 {#int-iii-s1-prop-17 .statement}

Sur l’espace $\mathcal{M}(X ; \mathbf{C})$, on considère les topologies suivantes ;
$\mathcal{T}_1$: la topologie de la convergence simple dans un ensemble total $T$ dans $\mathcal{K}(X ; \mathbf{C})$;
$\mathcal{T}_2$: la topologie vague;
$\mathcal{T}_3$: la topologie de la convergence strictement compacte;
$\mathcal{T}_4$: la topologie de la convergence compacte.
Chacune de ces topologies est moins fine que la suivante.
En outre:
(i) Les parties bornées sont les mêmes pour $\mathcal{T}_2, \mathcal{T}_3$ et $\mathcal{T}_4$.
(ii) Si $H$ est une partie vaguement bornée de $\mathcal{M}(X ; \mathbf{C})$, les topologies induites sur $H$ par les topologies $\mathcal{T}_1, \mathcal{T}_2, \mathcal{T}_3, \mathcal{T}_4$ sont identiques.
Une partie vaguement bornée $H$ de $\mathcal{M}(X ; \mathbf{C})$ est équicontinue (n° 9, prop. 15), donc la première assertion résulte d’Esp. vect. top., chap. III, § 3, n° 6, prop. 7, et la seconde de Top. gén., chap. X, 2e éd., § 2, n° 4, th. 1.

Rappelons que lorsque $X$ est paracompact, la topologie de la convergence strictement compacte coïncide avec la topologie de la convergence compacte (n° 1, prop. 2).

#### Proposition 18 {#int-iii-s1-prop-18 .statement}

Sur le cône $\mathcal{M}_+(X)$, les topologies induites par les topologies suivantes coïncident:

$\mathcal{T}_1$: la topologie de la convergence simple dans un sous-espace vectoriel V de $\mathscr{K}(X; \mathbf{C})$ dense dans $\mathscr{K}(X; \mathbf{C})$ et vérifiant la propriété (P) (n° 7, prop. 9);

$\mathcal{T}_2$: la topologie vague;

$\mathcal{T}_3$: la topologie de la convergence strictement compacte.

Comme tout filtre est intersection des ultrafiltres plus fins que lui (Top. gén., chap. I, 3e éd., § 6, n° 5, prop. 7), il suffit de montrer que si $\mathcal{U}$ est un ultrafiltre sur $\mathcal{M}_+(X)$, qui converge vers une mesure $\mu_0$ pour la topologie $\mathcal{T}_1$, il converge aussi vers $\mu_0$ pour $\mathcal{T}_3$. Soit donc K une partie compacte de X ; par hypothèse, il existe une fonction $h \in V$ qui est $\geqslant 0$ dans X et qui prend des valeurs $> 0$ dans K ; par suite, toute fonction $f \in \mathscr{K}(X, K; \mathbf{C})$ peut s’écrire $f = gh$, où $g \in \mathscr{K}(X, K; \mathbf{C})$, et si $c = \inf_{x \in K} h(x) > 0$, on a $\|g\| \leqslant c^{-1}\|f\|$. Par hypothèse, il existe un ensemble $H_0 \in \mathcal{U}$ tel que, pour toute mesure $\mu \in H_0$, on ait

$$
0 \leqslant \mu(h) \leqslant \mu_0(h) + 1 = b.
$$

Par suite, pour toute fonction $f \in \mathscr{K}(X; \mathbf{C})$, on a

$$
|\langle f, h.\mu \rangle| = |\langle hf, \mu \rangle| \leqslant \|f\|.\mu(h) \leqslant b\|f\|
$$

pour toute mesure $\mu \in H_0$; cela prouve que l’ensemble H des mesures $h.\mu$, où $\mu$ parcourt $H_0$, est vaguement borné. Si $\mathcal{U}_0$ est l’ultrafiltre induit par $\mathcal{U}$ sur $H_0$, l’image de $\mathcal{U}_0$ par l’application $\mu \mapsto h.\mu$ est la base d’un ultrafiltre $\mathfrak{F}$ sur H, et comme H est relativement compact pour la topologie de la convergence strictement compacte (prop. 17 et n° 9, prop. 15), $\mathfrak{F}$ est convergent vers une mesure $\nu_0$ pour cette topologie. Autrement dit, quels que soient $\varepsilon > 0$ et la partie compacte L de $\mathscr{K}(X, K; \mathbf{C})$ il existe une partie N de $H_0$ appartenant à $\mathcal{U}$, telle que, pour toute fonction $g \in L$ et tout couple de mesures $\mu, \mu'$ appartenant à N, on ait $|\langle g, h.\mu \rangle - \langle g, h.\mu' \rangle| \leqslant \varepsilon$, ou encore

$$
|\langle gh, \mu \rangle - \langle gh, \mu' \rangle| \leqslant \varepsilon.
$$

Or, nous avons vu plus haut que l’application $g \mapsto gh$ est un automorphisme de l’espace de Banach $\mathscr{K}(X, K; \mathbf{C})$. Nous avons donc montré que $\mathcal{U}$ est un filtre de Cauchy sur $\mathcal{M}_+(X)$ pour la topologie de la convergence strictement compacte. *A fortiori*, c’est un filtre de Cauchy pour la convergence vague, et la prop. 14 du n° 9 montre qu’il est vaguement convergent vers une mesure $\mu_1$; en outre, comme V est dense dans $\mathcal{K}(X; \mathbf{C})$, l’hypothèse entraîne que $\mu_1 = \mu_0$; enfin, comme $\mathcal{U}$ est un filtre de Cauchy pour la topologie de la convergence strictement compacte, il converge aussi vers $\mu_0$ pour cette topologie (Top. gén., chap. X, 2e éd., § 1, n° 5, prop. 5).

C.Q.F.D.

#### Corollaire {#int-iii-s1-n10-cor-1 .statement}

Si X est paracompact, les topologies induites sur $\mathcal{M}_+(X)$ par la topologie vague et par la topologie de la convergence compacte coïncident.

Par contre, les topologies induites sur $\mathcal{M}_+(X)$ par la topologie de la convergence compacte et la topologie de la convergence strictement compacte peuvent être distinctes lorsque X n’est pas paracompact (exerc. 3).

## EXERCICES {#int-iii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
