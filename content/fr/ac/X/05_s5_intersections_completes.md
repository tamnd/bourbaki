---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 5
section_title: Intersections complètes
lang: fr
source: ac-x-fr
pdf_pages: 0061-0069, 0164-0167
extraction: ocr
subsections:
    - "no": 1
      title: Idéal engendré par une suite complètement sécante
      page: 0
      pdf_page: 61
    - "no": 2
      title: Caractérisation des idéaux complètement sécants
      page: 63
      pdf_page: 62
    - "no": 3
      title: Idéaux complètement sécants et anneaux réguliers
      page: 65
      pdf_page: 64
    - "no": 4
      title: Anneaux gradués réguliers
      page: 66
      pdf_page: 65
    - "no": 5
      title: Suites régulières et extension des scalaires
      page: 0
      pdf_page: 67
    - "no": 6
      title: Idéaux complètement sécants et extension des scalaires
      page: 70
      pdf_page: 69
statements: 17
exercises: 11
content_sha256: 88c868cf777a1fb3d37328fd5ea267c57fb35ffc01909e91577ffeb6df4cfb40
---

## § 5. INTERSECTIONS COMPLÈTES

### 1. Idéal engendré par une suite complètement sécante

Définition 1. Soient $A$ un anneau, $J$ un idéal de $A$. On dit que l’idéal $J$ est complètement sécant au point $p$ de $V(J)$ si l’idéal $J_p$ de $A_p$ est engendré par une suite complètement sécante pour $A_p$. On dit que $J$ est complètement sécant s’il l’est en tous les points de $V(J)$.

Si l’idéal $J$ de $A$ est complètement sécant, il en est de même de l’idéal $S^{-1}J$ de $S^{-1}A$ pour toute partie multiplicative $S$ de $A$.

Tout idéal engendré par une suite complètement sécante est complètement sécant. Plus précisément :

#### Proposition 1 {#ac-x-s5-prop-1 .statement}

Soient $A$ un anneau, $J$ un idéal de $A$, engendré par une suite finie $x = (x_1, \ldots, x_r)$ d’éléments de $A$. Les conditions suivantes sont équivalentes :

(i) la suite $x$ est complètement sécante pour $A$ ;
(ii) (resp. (ii')) pour tout idéal premier (resp. maximal) $p \in V(J)$, l’image de $x$ dans $A_p$ est complètement sécante pour $A_p$ ;
(iii) (resp. (iii')) pour tout idéal premier (resp. maximal) $p \in V(J)$, l’idéal $J$ est complètement sécant en $p$ et l’image de $x$ dans le $\kappa(p)$-espace vectoriel $\kappa(p) \otimes_A J$ en forme une base.

Lorsque $A$ est noethérien, ces conditions sont encore équivalentes à :

(iv) pour tout entier $n \geq 0$, le $A/J$-module $J^n / J^{n+1}$ est libre, et les images des monômes $x_1^{\alpha_1} \ldots x_r^{\alpha_r}$ de degré total $n$ en forment une base.

Soit $p$ un idéal premier de $A$ ; notons $x_p$ l’image dans $A_p$ de la suite $x$. Pour tout entier $i \geq 0$, le $A_p$-module $H_i(x_p, A_p)$ est isomorphe à $(H_i(x, A))_p$ (A, X, p. 151, 2)) ; il est nul si $p$ ne contient pas $J$, puisqu’on a alors $J_p = A_p$ (A, X, p. 148, cor. 2). L’équivalence de (i), (ii) et (ii') résulte de là et de II, § 3, n° 3, cor. 2 du th. 1. D’autre part l’équivalence de (ii) et (iii) et celle de (ii') et (iii') résultent du § 1, n° 3, cor. 2 du th. 1.

L’implication (i) $\Rightarrow$ (iv) est une conséquence du th. 1 de A, X, p. 160. Enfin la condition (iv) implique par localisation la condition analogue pour les $(A_p/J_p)$-modules $J_p^n / J_p^{n+1}$ pour tout $p \in V(J)$, et celle-ci entraîne (ii) d’après le cor. 1 de A, X, p. 160.

#### Remarque 1 {#ac-x-s5-n1-rem-1 .statement}

Lorsque l’anneau $A$ est noethérien, on peut remplacer dans les conditions (ii) et (ii') « complètement sécante » par « régulière » (A, X, p. 160, cor. 1).

On prendra garde qu’il n’en est pas ainsi dans la condition (i) : une suite complètement sécante pour A n’est pas nécessairement A-régulière (exerc. 1).

#### Remarque 2 {#ac-x-s5-n1-rem-2 .statement}

Soient A un anneau, J un idéal de type fini de A et p un idéal premier de A contenant J. D’après le cor. 2 du th. 1 du § 1, n° 3, on a

$$
\operatorname{prof}_{A_p}(J_p; A_p) \leq [\kappa(p) \otimes_A J : \kappa(p)]
$$

et il y a égalité si et seulement si J est complètement sécant en p.

Supposons que J soit distinct de A et engendré par une suite complètement sécante $(x_1, \ldots, x_r)$. On a alors (prop. 4 du § 1, n° 3, et prop. 1 ci-dessus)

$$
\operatorname{prof}_A(J; A) = \inf_{p \in V(J)} \operatorname{prof}_{A_p}(J_p; A_p) = r.
$$

Si de plus A est noethérien, on a $\operatorname{codim}(V(J), \operatorname{Spec}(A)) \leq r$ (VIII, § 3, n° 3, prop. 4) et $\operatorname{prof}_A(J; A) \leq \operatorname{codim}(V(J), \operatorname{Spec}(A))$ ($§ 1$, n° 7, prop. 12), d’où finalement

$$
\operatorname{prof}_A(J; A) = r = \operatorname{codim}(V(J), \operatorname{Spec}(A)) = \operatorname{ht}(J).
$$

### 2. Caractérisation des idéaux complètement sécants

Soient A un anneau et J un idéal de A. Le A-module gradué $\bigoplus_{n \in \mathbf{N}} J^n$ possède une structure naturelle de A-algèbre graduée, déduite de la multiplication dans l’anneau A ; l’application identique de J dans $J^1$ se prolonge donc en un homomorphisme surjectif de A-algèbres graduées, dit canonique

$$
\alpha_J : S_A(J) \longrightarrow \bigoplus_{n \in \mathbf{N}} J^n.
$$

Par extension des scalaires à l’anneau $A/J$, on déduit de $\alpha_J$ un homomorphisme surjectif de $A/J$-algèbres graduées, également dit canonique

$$
\beta_J : S_{A/J}(J/J^2) \longrightarrow \operatorname{gr}_J(A),
$$

avec $\operatorname{gr}_J(A) = \bigoplus_{n \in \mathbf{N}} J^n / J^{n+1}$.

#### Théorème 1 {#ac-x-s5-thm-1 .statement}

Soient A un anneau noethérien et J un idéal de A. Les conditions suivantes sont équivalentes :

(i) l’idéal J est complètement sécant ;
(ii) l’idéal J est complètement sécant en tout idéal maximal $m \in V(J)$ ;
(iii) le $A/J$-module $J/J^2$ est projectif et l’homomorphisme canonique $\alpha_J : S_A(J) \longrightarrow \bigoplus_{n \in \mathbf{N}} J^n$ est bijectif ;
(iv) le $A/J$-module $J/J^2$ est projectif et l’homomorphisme canonique $\beta_J : S_{A/J}(J/J^2) \longrightarrow \operatorname{gr}_J(A)$ est bijectif.

(i) ⇒ (ii) : c’est trivial.

(ii) ⇒ (iii) : supposons la condition (ii) satisfaite. Il suffit de prouver que pour tout idéal maximal m de A, le A_m/J_m-module J_m/J_m^2 est libre et l’homomorphisme $\alpha_{J_m} : S_{A_m}(J_m) \longrightarrow \bigoplus_n J_m^n$ est bijectif (II, § 5, n° 2, th. 1 et § 3, n° 3, th. 1). Mais ces assertions sont triviales lorsque m n’appartient pas à V(J) puisqu’on a alors J_m = A_m, et elles résultent de A, X, p. 160, th. 1 et p. 161, remarque, lorsque m appartient à V(J).

(iii) ⇒ (iv) : c’est clair.

(iv) ⇒ (i) : supposons la condition (iv) satisfaite ; soit p un idéal premier de A contenant J. Alors le A_p/J_p-module J_p/J_p^2 est libre. Soit x = (x_1, ..., x_r) une suite d’éléments de J_p relevant une base de J_p/J_p^2. La suite x engendre J_p (lemme de Nakayama), et satisfait par construction à la condition (iv) de la prop. 1. Par suite l’idéal J_p de A_p est complètement sécant, et J est complètement sécant en p.

Remarque 1. Supposons l’idéal J complètement sécant ; soit (x_1, ..., x_r) une suite d’éléments de J, telle que pour tout idéal maximal m ∈ V(J) les images canoniques des x_i dans J/mJ forment une base de ce A/m-espace vectoriel. Alors le A/J-module J/J^2 est libre et les images canoniques dans J/J^2 des x_i en forment une base : il suffit en effet de vérifier que les images des x_i forment une base du A_m/J_m-module J_m/J_m^2 pour tout m ∈ V(J) (II, § 3, n° 3, th. 1), ce qui résulte de loc. cit., n° 2, prop. 5 et cor. 2, puisque le A_m/J_m-module J_m/J_m^2 est projectif (th. 1).

#### Corollaire 1 {#ac-x-s5-thm-1-cor-1 .statement}

Soient $\hat{A}$ l’anneau séparé complété de A pour la topologie J-adique et $\hat{J} = J\hat{A}$ le séparé complété de J. Pour que l’idéal $\hat{J}$ de $\hat{A}$ soit complètement sécant, il faut et il suffit que l’idéal J de A soit complètement sécant.

En effet, l’application canonique gr_J(A) → gr_J(\hat{A}) est un isomorphisme d’anneaux gradués ; il suffit donc d’appliquer le critère (iv).

Plus généralement :

#### Corollaire 2 {#ac-x-s5-thm-1-cor-2 .statement}

Soient ρ : A → B un homomorphisme d’anneaux noethériens faisant de B un A-module plat, et J un idéal de A.

a) Si J est complètement sécant, l’idéal JB de B est complètement sécant.

b) Supposons que l’idéal JB de B soit complètement sécant et que tout idéal maximal m ∈ V(J) soit l’image réciproque d’un idéal maximal de B. Alors l’idéal J est complètement sécant. C’est le cas par exemple si B est un A-module fidèlement plat.

Remarquons d’abord que, puisque le A-module B est plat, $J^n \otimes_A B$ s’identifie à $J^nB$ et $(J^n/J^{n+1}) \otimes_{A/J} (B/JB)$ à $J^nB/J^{n+1}B$ pour tout entier $n \geq 0$. L’assertion a) résulte alors du critère (iii). Sous les hypothèses de b), le A/J-module B/JB est fidèlement plat (I, § 2, n° 7, cor. 2 de la prop. 8 et § 3, n° 5, prop. 9) et J est complètement sécant d’après le critère (iv), compte tenu de I, § 3, n° 1, prop. 2 et n° 6, prop. 12. La dernière assertion résulte de la prop. 8 de I, § 3, n° 5.

#### Corollaire 3 {#ac-x-s5-thm-1-cor-3 .statement}

Soient $A$ un anneau noethérien et $J$ un idéal complètement sécant de $A$. Si $A$ est un anneau de Macaulay (resp. de Gorenstein), il en est de même de $A/J$.

Soit en effet $m$ un idéal maximal de $A$ contenant $J$. L’idéal $J_m$ de $A_m$ est engendré par une suite $A_m$-régulière ; donc $(A/J)_m$ est un anneau de Macaulay (resp. de Gorenstein) d’après l’exemple 6 du § 2, n° 5 (resp. l’exemple 2 du § 3, n° 9).

#### Remarque 2 {#ac-x-s5-n2-rem-2 .statement}

On dit qu’un anneau noethérien $A$ est un anneau d’intersection complète si, pour tout idéal maximal $m$ de $A$, l’anneau local complet $\widehat{A_m}$ est isomorphe au quotient d’un anneau noethérien local complet régulier par un idéal complètement sécant. Il résulte du cor. 3 ci-dessus et du cor. 2 de la prop. 12 du § 3, n° 8 qu’un tel anneau est un anneau de Gorenstein.

### 3. Idéaux complètement sécants et anneaux réguliers

#### Proposition 2 {#ac-x-s5-prop-2 .statement}

Soit $A$ un anneau noethérien. Les conditions suivantes sont équivalentes :

(i) $A$ est régulier ;
(ii) tout idéal maximal de $A$ est complètement sécant ;
(iii) tout idéal $J$ de $A$ tel que $A/J$ soit régulier est complètement sécant.

(i) $\Rightarrow$ (iii) : supposons l’anneau $A$ régulier ; soit $J$ un idéal de $A$ tel que $A/J$ soit régulier et soit $p$ un idéal premier de $A$ contenant $J$. Alors les anneaux locaux $A_p$ et $A_p/J_p$ sont réguliers, donc $J_p$ est engendré par une suite complètement sécante pour $A_p$ (VIII, § 5, n° 3, cor. 2 et prop. 2), ce qui signifie que $J$ est complètement sécant en $p$.

(iii) $\Rightarrow$ (ii) : c’est clair puisqu’un corps est un anneau régulier.

(ii) $\Rightarrow$ (i) : soit $m$ un idéal maximal de $A$ ; sous l’hypothèse (ii), l’idéal maximal $mA_m$ de $A_m$ est engendré par une suite complètement sécante pour $A_m$, donc $A_m$ est régulier (VIII, § 5, n° 2, th. 1). Par conséquent $A$ est régulier.

#### Proposition 3 {#ac-x-s5-prop-3 .statement}

Soient $A$ un anneau noethérien et $J$ un idéal de $A$ tel que $A/J$ soit régulier. Les conditions suivantes sont équivalentes :

(i) l’idéal $J$ est complètement sécant ;
(ii) pour tout idéal premier (resp. maximal) $p$ de $A$ contenant $J$, l’anneau $A_p$ est régulier ;
(iii) l’anneau séparé complété de $A$ pour la topologie $J$-adique est régulier.

D’après le th. 1, la condition (i) signifie que pour tout idéal premier (resp. maximal) $p$ de $A$ contenant $J$, l’idéal $J_p$ de l’anneau local $A_p$ est engendré par une suite complètement sécante pour $A_p$. Puisque $A_p/J_p$ est régulier par hypothèse, cette dernière condition équivaut à ce que $A_p$ soit régulier (VIII, § 5, n° 3, prop. 2 et son cor. 2) ; cela prouve l’équivalence de (i) et (ii). L’équivalence de (ii) et (iii) résulte du § 4, n° 2, cor. 3 de la prop. 4.

#### Proposition 4 {#ac-x-s5-prop-4 .statement}

Soient $A$ un anneau régulier, $J$ un idéal de $A$ et $A_0$ un sous-anneau de $A$ tel que l’homomorphisme canonique $A_0 \to A/J$ soit bijectif.

a) L’idéal $J$ est complètement sécant, le $A_0$-module $J/J^2$ est projectif de type fini, et l’anneau $A_0$ est régulier.

b) Soit $\varphi : J/J^2 \to J$ une section $A_0$-linéaire de la surjection canonique $J \to J/J^2$. L’homomorphisme de $A_0$-algèbres $S_{A_0}(J/J^2) \longrightarrow A$ prolongeant $\varphi$ s’étend en un isomorphisme du complété de l’anneau gradué $S_{A_0}(J/J^2)$ sur le séparé complété de $A$ pour la topologie $J$-adique.

a) Soit $\mathfrak{p}$ un idéal premier de $A$ contenant $J$. On a $\mathfrak{p} = (\mathfrak{p} \cap A_0) \oplus J$ et par suite $\mathfrak{p}^2 = (\mathfrak{p} \cap A_0)^2 \oplus \mathfrak{p}J$, donc $\mathfrak{p}^2 \cap J = \mathfrak{p}J$. Notons $i$ l’injection canonique de $J$ dans $\mathfrak{p}$. D’après ce qui précède l’application $i \otimes 1_{A/\mathfrak{p}} : J \otimes_A A/\mathfrak{p} \longrightarrow \mathfrak{p} \otimes_A A/\mathfrak{p}$ est injective, et il en est de même de $i_p \otimes 1_{\kappa(\mathfrak{p})} : J_p \otimes_{A_p} \kappa(\mathfrak{p}) \longrightarrow \mathfrak{p}A_p \otimes_{A_p} \kappa(\mathfrak{p})$. Le lemme de Nakayama implique que l’idéal $J_p$ de $A_p$ est engendré par une partie d’un système de coordonnées de l’anneau local régulier $A_p$. D’après la prop. 2 de VIII, § 5, n° 3, l’anneau $A_p/J_p$ est régulier et l’idéal $J_p$ est complètement sécant. Ainsi $J$ est complètement sécant, l’anneau $A_0$, isomorphe à $A/J$, est régulier, et le $A_0$-module $J/J^2$ est projectif de type fini d’après le th. 1 (n° 2).

b) Il résulte du th. 1 que l’homomorphisme canonique $\beta_J : S_{A_0}(J/J^2) \longrightarrow \mathrm{gr}_J(A)$ est bijectif. Soit $f : S_{A_0}(J/J^2) \longrightarrow A$ l’homomorphisme de $A_0$-algèbres prolongeant l’application $A_0$-linéaire $\varphi : J/J^2 \longrightarrow J$. Si l’on munit $A$ de la filtration $J$-adique et $S_{A_0}(J/J^2)$ de la filtration associée à sa graduation, $\beta_J$ s’identifie à l’homomorphisme déduit de $f$ par passage aux gradués associés. L’assertion b) résulte alors de III, § 2, n° 8, cor. 3 du th. 1.

### 4. Anneaux gradués réguliers

Soient $A_0$ un anneau et $P$ un $A_0$-module gradué de type $\mathbf{N}$ à degrés $> 0$. Notons $A$ l’anneau $S_{A_0}(P)$; il existe sur $A$ une unique graduation de type $\mathbf{N}$ pour laquelle $A_0$ est de degré 0 et $P$ est un sous-$A_0$-module gradué de $A$. Notons $A_+$ l’idéal $\bigoplus_{n>0} A_n$ de $A$. Alors l’application canonique $P \longrightarrow A_+/A_+^2$ est un isomorphisme de $A_0$-modules gradués (cf. A, III, p. 76, prop. 10).

Si le $A_0$-module $P$ est gradué libre (A, II, p. 167, remarque 3) et si $(x_i)_{i \in I}$ est une base de $P$ formée d’éléments homogènes, la $A_0$-algèbre graduée $S_{A_0}(P)$ est isomorphe à l’algèbre de polynômes $A_0[(X_i)_{i \in I}]$, munie de la graduation pour laquelle chaque $X_i$ est homogène de degré $\deg(x_i)$. On appelle $A_0$-algèbre graduée de polynômes toute $A_0$-algèbre graduée de type $\mathbf{N}$, isomorphe à une $A_0$-algèbre graduée de la forme précédente.

Lorsque l’anneau $A_0$ est régulier et que le $A_0$-module $P$ est projectif de type fini, l’anneau $S_{A_0}(P)$ est régulier (§ 4, n° 2, cor. 4 de la prop. 4). Inversement :

#### Théorème 2 {#ac-x-s5-thm-2 .statement}

Soit $A$ un anneau régulier, gradué de type $\mathbf{N}$. L’anneau $A_0$ formé des éléments de degré 0 dans $A$ est régulier ; il existe un $A_0$-module projectif de type fini $P$ gradué à degrés $> 0$ tel que $A$ soit isomorphe comme $A_0$-algèbre graduée à $S_{A_0}(P)$.

Notons $P$ le $A_0$-module gradué $A_+/A_+^2$. D’après la prop. 4 du n° 3, l’anneau $A_0$ est régulier et le $A_0$-module $P$ est projectif et de type fini. Les composants homogènes de $P$ sont donc projectifs et il existe une section $A_0$-linéaire $\varphi : P \to A_+$, graduée de degré 0 , de la surjection canonique $A_+ \to P$. Soit $f : S_{A_0}(P) \longrightarrow \Lambda$ l’homomorphisme de $A_0$-algèbres graduées qui prolonge $\varphi$. D’après la prop. 4, $f$ s’étend en un isomorphisme du séparé complété de $S_{A_0}(P)$ pour la topologie $S_{A_0}(P)_+$-adique sur le séparé complété de $A$ pour la topologie $A_+$-adique. Par conséquent, $f$ est injectif et son image est dense dans $A$ pour la topologie $A_+$-adique. Mais puisque les topologies induites sur les composants homogènes de $A$ sont discrètes et que l’image de $f$ est un sous-module gradué, cela implique que $f$ est bijectif.

#### Corollaire 1 {#ac-x-s5-thm-2-cor-1 .statement}

*Soit B un anneau régulier, gradué à degrés positifs. Supposons que tout $B_0$-module projectif de type fini soit libre.*
a) *L’anneau $B_0$ est intègre et régulier et la $B_0$-algèbre $B$ est une $B_0$-algèbre graduée de polynômes, de type fini.*
b) *Soit A un sous-anneau gradué de B tel que $A_0 = B_0$ et que B soit un A-module de type fini. Les conditions suivantes sont équivalentes :
(i) le A-module B est gradué libre ;
(ii) le A-module B est plat ;
(iii) A est une $A_0$-algèbre graduée de polynômes, de type fini.*

D’après le th. 2, l’anneau $B_0$ est régulier, donc produit d’anneaux réguliers intègres ($§ 4$, n° 2, exemple 2). Pour tout élément idempotent $e$ de $B_0$, le $B_0$-module $B_0e$ est projectif, donc libre, ce qui entraîne $e = 0$ ou $1$; ainsi $B_0$ est intègre. L’assertion a) résulte alors du théorème 2 et de ce qu’un $B_0$-module gradué et projectif de type fini est gradué libre.

Démontrons b).

(i) $\Leftrightarrow$ (ii) : les $A_0$-modules gradués plats et de type fini sont gradués libres (II, $§ 5$, n° 2, cor. 2 du th. 1). L’équivalence de (i) et (ii) résulte donc de A, X, p. 144, prop. 8.

(ii) $\Leftrightarrow$ (iii) : puisque $B$ est entier sur $A$ et est une $A_0$-algèbre de type fini, $A$ est une $A_0$-algèbre de type fini (V, $§ 1$, n° 9, lemme 5), donc un anneau noethérien. L’équivalence de (ii) et (iii) résulte alors du cor. de la prop. 8 du $§ 4$, n° 5 et de a) appliqué à $A$.

#### Corollaire 2 {#ac-x-s5-thm-2-cor-2 .statement}

*Soient k un corps, B une k-algèbre graduée de polynômes, de type fini, et A une sous-algèbre graduée de B. Les conditions suivantes sont équivalentes :
(i) B est un $\Lambda$-module gradué libre ;
(ii) B est un A-module plat ;
(iii) on a $\operatorname{Tor}_1^\Lambda(k, B) = 0$ ;
(iv) l’algèbre A est une k-algèbre graduée de polynômes de type fini, et toute suite génératrice algébriquement libre de A formée d’éléments homogènes est B-régulière.*

Les implications (i) $\Rightarrow$ (ii) et (ii) $\Rightarrow$ (iii) sont claires, et l’implication (iii) $\Rightarrow$ (i) résulte de A, X, p. 144, prop. 8, a).

(iv) ⇒ (iii) : supposons la condition (iv) satisfaite, et soit x une suite génératrice algébriquement libre de A formée d’éléments homogènes. La suite x, étant A-régulière, est complètement sécante pour A (A, X, p. 157, prop. 5), de sorte que le A-module Tor_1^A(k, B) est isomorphe à H_1(x, B) (A, X, p. 159, remarque 3) ; mais ce dernier est nul, puisque la suite x est B-régulière.

Les corollaires 1 et 2 impliquent le lemme 5 de LIE, V, § 5, n° 5.

### 5. Suites régulières et extension des scalaires

#### Proposition 5 {#ac-x-s5-prop-5 .statement}

Soient ρ : A → B un homomorphisme local d’anneaux locaux noethériens, N un B-module de type fini, x = (x_1, ..., x_r) une suite d’éléments de m_B et u : A[T_1, ..., T_r] → B l’unique homomorphisme de A-algèbres tel que u(T_i) = x_i pour i = 1, ..., r. Les conditions suivantes sont équivalentes :

(i) l’homomorphisme u fait de N un A[T_1, ..., T_r]-module plat ;
(ii) le A-module N est plat et, pour tout A-module M, la suite x est M ⊗_A N-régulière ;
(iii) le A-module N est plat et la suite x est κ_A ⊗_A N-régulière ;
(iv) le A-module N/(x_1N + ... + x_rN) est plat et la suite x est N-régulière.

(i) ⇒ (ii) : posons T = (T_1, ..., T_r). Supposons que le A[T]-module N soit plat. Puisque A[T] est plat sur A, le A-module N est plat (I, § 2, n° 7, cor. 3 de la prop. 8). Soit M un A-module. La suite T est évidemment M[T]-régulière, donc M[T] ⊗_{A[T]} N-régulière, puisque N est plat sur A[T]. Or le A[T]-module M[T] ⊗_{A[T]} N s’identifie à M ⊗_A N, l’homothétie de rapport T_i correspondant à l’endomorphisme 1_M ⊗ (x_i)_N. La condition (ii) est donc satisfaite.

(ii) ⇒ (iii) : c’est trivial.

(iii) ⇒ (iv) : cela résulte de la prop. 10 du § 1, n° 6.

(iv) ⇒ (i) : notons t l’idéal de A[T] engendré par T. Le (A[T]/t)-module N/tN est plat par hypothèse et N est idéalement séparé pour t (III, § 5, n° 4, prop. 2). Pour démontrer que N est plat sur A[T], il suffit de prouver, vu le th. 1 de loc. cit., n° 2, que le A-module Tor_1^{A[T]}(A[T]/t, N) est nul. Mais puisque la suite T est A[T]-régulière, ce module est isomorphe à H_1(T, N) (A, X, p. 159, remarque 3), qui est nul puisque la suite T est N-régulière (loc. cit., p. 157, prop. 5).

Corollaire. Soient k un corps, Λ une k-algèbre locale noethérienne, x = (x_1, ..., x_r) une suite d’éléments de m_A et M un Λ-module de type fini. Soient Ā et Ĝ les complétés de A et M pour leur topologie (x_1Ā + ... + x_rĀ)-adique ; notons u : k[T_1, ..., T_r] → Ā l’unique homomorphisme de k-algèbres tel que u(T_i) = x_i pour i = 1, ..., r, et ū : k[[T_1, ..., T_r]] → Ā l’unique homomorphisme continu qui le prolonge. Les conditions suivantes sont équivalentes :

(i) la suite $x$ est $M$-régulière ;
(ii) l’homomorphisme $u$ fait de $M$ un $k[T_1, \ldots, T_r]$-module plat ;
(iii) l’homomorphisme $\hat{u}$ fait de $\hat{M}$ un $k[[T_1, \ldots, T_r]]$-module plat.
L’équivalence de (i) et (ii) résulte de l’équivalence des conditions (i) et (iv) de la prop. 5 ; l’équivalence de (ii) et (iii) résulte de III, § 5, n° 4, prop. 4.

Ces résultats permettent de caractériser les modules macaulayens dans deux cas importants. Notons $\Lambda$ un anneau local noethérien, $M$ un $\Lambda$-module de type fini. Il est équivalent de dire que le $\Lambda$-module $M$ est macaulayen ou que le $\widehat{\Lambda}$-module $\hat{M}$ est macaulayen (§ 2, n° 7, cor. 4 de la prop. 8). Nous supposerons désormais que l’anneau local noethérien $\Lambda$ est complet.

1) Supposons d’abord que $\Lambda$ possède un sous-corps ; il admet alors un corps de représentants $k$ (IX, § 3, n° 3, th. 1). Soit $(x_1, \ldots, x_r)$ une suite sécante maximale pour $M$ ; notons $u : k[[T_1, \ldots, T_r]] \longrightarrow \Lambda$ l’unique homomorphisme continu tel que $u(T_i) = x_i$ pour $i = 1, \ldots, r$. D’après le lemme 4 b) de IX, § 2, n° 5 et la remarque 1 de VIII, § 3, n° 2, $A/\mathrm{Ann}(M)$ est un $k[[T_1, \ldots, T_r]]$-module de type fini et par suite $M$ est un $k[[T_1, \ldots, T_r]]$-module de type fini. Cela étant, les conditions suivantes sont équivalentes :
(i) le $k[[T_1, \ldots, T_r]]$-module $M$ est libre ;
(ii) le $\Lambda$-module $M$ est macaulayen.

En effet, il est équivalent de dire que $M$ est un $\Lambda$-module macaulayen ou que la suite $(x_1, \ldots, x_r)$ est $M$-régulière (§ 2, n° 3, th. 1). D’après le cor. ci-dessus, cette dernière condition signifie que le $k[[T_1, \ldots, T_r]]$-module $M$ est plat, ou encore qu’il est libre puisqu’il est de type fini.

2) Supposons que le corps résiduel $\kappa_\Lambda$ de $\Lambda$ soit de caractéristique $p > 0$ et que l’on ait $\dim(M/pM) < \dim(M)$. Soit $(x_1, \ldots, x_r)$ une suite sécante maximale pour $M/pM$, de sorte que $(p1_\Lambda, x_1, \ldots, x_r)$ est une suite sécante maximale pour $M$. Soit $C$ un $p$-anneau de longueur $+\infty$, de corps résiduel $\kappa_\Lambda$ (IX, § 2, n° 3, prop. 5). Il existe un homomorphisme $u_0$ de $C$ dans $\Lambda$ qui induit l’identité sur les corps résiduels ; soit $u : C[[T_1, \ldots, T_r]] \longrightarrow \Lambda$ l’unique homomorphisme prolongeant $u_0$ et appliquant $T_i$ sur $x_i$ pour tout $i$. Il résulte comme précédemment de loc. cit., n° 5, lemme 4 que $u$ fait de $M$ un $C[[T_1, \ldots, T_r]]$-module de type fini. Les conditions suivantes sont équivalentes :
(i) le $C[[T_1, \ldots, T_r]]$-module $M$ est libre ;
(ii) le $\Lambda$-module $M$ est macaulayen.

En effet la condition (ii) équivaut à dire que la suite $(x_1, \ldots, x_r)$ est $M$-régulière et que l’homothétie de rapport $p$ dans $M/(x_1M + \ldots + x_rM)$ est injective (§ 2, n° 3, th. 1). Or cette dernière condition signifie que le $C$-module $M/(x_1M + \ldots + x_rM)$ est sans torsion, donc plat ($\Lambda$, X, p. 9, exemple 7). Ainsi, compte tenu de la prop. 5, (iv) $\Leftrightarrow$ (i), la condition (ii) équivaut au fait que le $C[T_1, \ldots, T_r]$-module $M$ est plat, ou encore (III, § 5, n° 4, prop. 4) que le $C[[T_1, \ldots, T_r]]$-module $M$ est plat, c’est-à-dire libre puisqu’il est de type fini.

### 6. Idéaux complètement sécants et extension des scalaires

#### Proposition 6 {#ac-x-s5-prop-6 .statement}

Soient $\rho : A \to B$ un homomorphisme d’anneaux noethériens et $J$ un idéal de $B$. Les conditions suivantes sont équivalentes :

(i) le $A$-module $B/J$ est plat et l’idéal $J$ est complètement sécant ;

(ii) pour tout $q \in V(J)$, le $A$-module $B_q$ est plat et, pour toute $A$-algèbre $A'$ telle que l’anneau $\Lambda' \otimes_A B$ soit noethérien, l’idéal $J(A' \otimes_A B)$ de $A' \otimes_A B$ est complètement sécant ;

(iii) pour tout idéal maximal $n$ de $B$ contenant $J$, le $A$-module $B_n$ est plat et l’idéal $J(\kappa(\rho^{-1}(n)) \otimes_A B_n)$ de $\kappa(\rho^{-1}(n)) \otimes_A B_n$ est complètement sécant.

D’après le th. 1 du n° 2, la condition (i) équivaut à la condition (i') (resp. (i'')) suivante :

(i') (resp. (i'')) pour tout idéal premier (resp. maximal) $q$ de $B$ contenant $J$, le $A_{\rho^{-1}(q)}$-module $B_q/J_q$ est plat et l’idéal $J_q$ de $B_q$ est engendré par une suite $B_q$-régulière.

(i') $\Rightarrow$ (ii) : supposons (i') vérifiée. Soit $A'$ une $A$-algèbre telle que l’anneau $B' = A' \otimes_A B$ soit noethérien. Soit $q$ un idéal premier de $B$ contenant $J$; posons $p = \rho^{-1}(q)$. Puisque $B'_q$ s’identifie à $A'_p \otimes_{A_p} B_q$, il résulte de l’implication (iv) $\Rightarrow$ (ii) de la prop. 5 (n° 5) que l’idéal $JB'_q$ de $B'_q$ est engendré par une suite $B'_q$-régulière et que $B_q$ est plat sur $A_p$, donc sur $A$. Par ailleurs, pour tout idéal premier $r$ de $B'$ contenant $JB'$, l’image réciproque $q$ de $r$ dans $B$ contient $J$ et $B'_r$ s’identifie à un anneau de fractions de $B'_q$. Ainsi $JB'_r$ est un idéal complètement sécant de $B'_r$ et $JB'$ est un idéal complètement sécant de $B'$.

(ii) $\Rightarrow$ (iii) : c’est trivial.

(iii) $\Rightarrow$ (i'') : supposons (iii) vérifiée. Soit $n$ un idéal maximal de $B$ contenant $J$; posons $m = \rho^{-1}(n)$. Soit $x$ une suite d’éléments de $J_n$ dont les images dans $J_n/nJ_n$ forment une base de ce $\kappa(n)$-espace vectoriel. La suite $x$ engendre $J_n$; d’après la prop. 1 du n° 1, elle est $(\kappa(m) \otimes_A B_n)$-régulière. Comme le $A_m$-module $B_n$ est plat par hypothèse, il résulte de l’implication (iii) $\Rightarrow$ (iv) de la prop. 5 que la condition (i'') est satisfaite.

#### Remarque 1 {#ac-x-s5-n6-rem-1 .statement}

Supposons que les conditions équivalentes de la prop. 6 soient satisfaites. Comme $B/J$ est plat sur $A$, pour toute $A$-algèbre $A'$, la suite canonique de $A'$-modules
$$
0 \to A' \otimes_A J \to A' \otimes_A B \to A' \otimes_A (B/J) \to 0
$$
est donc exacte, et l’homomorphisme canonique $A' \otimes_A J \to J(A' \otimes_A B)$ est bijectif.

## EXERCICES {#ac-x-s5-exercises}

See the [exercises for § 5](exercises/s5/).
