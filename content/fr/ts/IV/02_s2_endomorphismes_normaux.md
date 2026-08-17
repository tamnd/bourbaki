---
book: ts
book_title: Théories spectrales
chapter: IV
chapter_title: THÉORIE SPECTRALE HILBERTIENNE
section: 2
section_title: Endomorphismes normaux
lang: fr
source: ts-iii-v-fr
book_pages: TS IV.179-TS IV.195, TS IV.319-TS IV.330
pdf_pages: 0192-0208, 0332-0343
extraction: native
subsections:
    - "no": 1
      title: Compléments sur les espaces $L^p(X, \mu)$
      page: 179
      pdf_page: 192
    - "no": 2
      title: Image essentielle d’une fonction mesurable
      page: 181
      pdf_page: 194
    - "no": 3
      title: Fonctions universellement mesurables
      page: 182
      pdf_page: 195
    - "no": 4
      title: L’algèbre stellaire $L^{\infty}(X, \mu)$
      page: 185
      pdf_page: 198
    - "no": 5
      title: Endomorphismes de multiplication
      page: 186
      pdf_page: 199
    - "no": 6
      title: Mesures spectrales
      page: 190
      pdf_page: 203
    - "no": 7
      title: Algèbres stellaires commutatives d’endomorphismes d’un espace hilbertien
      page: 191
      pdf_page: 204
    - "no": 8
      title: Continuité du calcul fonctionnel
      page: 194
      pdf_page: 207
statements: 32
exercises: 28
content_sha256: 165363ebfb20ce8155dd3b050619ce5cedef07b4b1c442c9a028bba02ac122b4
---

## § 2. ENDOMORPHISMES NORMAUX

Dans tout ce paragraphe, les espaces hilbertiens considérés sont complexes, sauf mention du contraire.

### 1. Compléments sur les espaces $L^p(X, \mu)$

#### Proposition 1 {#ts-iv-s2-prop-1 .statement tag=02YO}

Soit X un espace topologique localement compact. Soient $\mu$ une mesure positive sur X et $p\in [1,+\infty [$. Soit $(X_i)_{i\in I}$ une famille localement dénombrable (INT, IV, p. 190, § 5, n$^o9$, déf. 7) de parties localement compactes deux à deux disjointes de X telle que le complémentaire de la réunion des $X_i$ soit localement $\mu$-négligeable. Soient $\varphi_i$ la fonction caractéristique de $X_i$ et $\mu_i$ la mesure induite par $\mu$ sur $X_i$ (INT, IV, p. 186, §5, n$^o7$, déf. 4).

a) L’application $p_i:f\mapsto f \varphi_i$ est un projecteur de $\mathscr{L}^p(X, \mu)$ et définit par passage aux quotients un projecteur $\widetilde{p}_i$ de $L^p(X, \mu)$. Ce dernier est un orthoprojecteur de $L^2(X, \mu)$ si $p= 2$;

b) L’application $f\mapsto f|X_i$ induit un isomorphisme isométrique de l’image de $p_i$ sur l’espace $\mathscr{L}^p(X_i, \mu_i)$ et définit par passage aux quotients un isomorphisme isométrique de l’image de $\widetilde{p}_i$ sur $L^p(X_i, \mu_i)$, par le truchement duquel on identifie ces deux espaces ;

c) La somme des espace $L^p(X_i, \mu_i)$ est totale dans l’espace $L^p(X, \mu)$. Dans le cas $p= 2$, l’espace $L^2(X, \mu)$ est la somme hilbertienne des espaces $L^2(X_i, \mu_i)$.

L’assertion a) est élémentaire. L’assertion b) résulte du scholie de INT, V, p. 84, § 7, n$^o1$.

Soit $q\in ]1,+\infty ]$ l’exposant conjugué de $p$. On identifie le dual de $L^p(X, \mu)$ avec $L^q(X, \mu)$ (INT, V, p. 61, § 5, n$^o8$, th. 4). Soit $f$ une fonction dans $\mathscr{L}^q(X, \mu)$ dont la classe $\widetilde{f}$ dans $L^q(X, \mu)$ vérifie $\langle \widetilde{f} ,\widetilde{p}_i(\varphi )\rangle = 0$ pour tout $i\in I$ et tout $\varphi \in L^p(X, \mu)$. Comme l’image de $p_i$ contient $\mathscr{K}(X_i)$, il en résulte que la mesure $(f|X_i)\cdot \mu_i$ sur $X_i$ est nulle, ce qui signifie que la restriction de $f$ à $X_i$ est localement $\mu_i$-négligeable sur $X_i$ (INT, V, p. 46, § 5, n$^o3$, cor. 2). Puisque le complémentaire dans X de la réunion des $X_i$ est localement $\mu$-négligeable, on en conclut que la fonction $f$ est localement $\mu$-négligeable sur X (INT, IV, p. 190, § 5, n$^o9$ et p. 172, n$^o2$, prop. 5). La classe de $f$ est alors nulle dans $L^q(X, \mu)$ (en utilisant INT, V, p. 8, § 1, n$^o3$, lemme 1 et corollaire de la proposition 9 lorsque $p\not = 1)$. D’après le théorème de Hahn–Banach (EVT, II, p. 46, cor. 1), la première partie de l’assertion c) en résulte.

Si $p= 2$, l’image de $p_i$ est orthogonale à celle $p_j$ pour tous $i\not =j$, puisque $X_i$ et $X_j$ sont alors disjoints, d’où la dernière assertion.

#### Proposition 2 {#ts-iv-s2-prop-2 .statement tag=02YP}

Soit X un espace localement compact dénombrable à l’infini. Soit $\mu$ une mesure positive sur X. Pour tout $p\in [1,+\infty [$, l’espace $L^p(X, \mu)$ est de type dénombrable.

Soit $(U_n)_{n\in\mathbf{N}}$ une suite d’ouverts relativement compacts de X dont la réunion est égale à X et qui vérifient $U_n\subset U_{n+1}$ pour tout $n\in \mathbf{N}$ (TG, I, p. 68, prop. 15). Pour tout $n\in \mathbf{N}$, l’espace $\mathscr{K}(X,\overline{U}_n)$ s’identifie à un sous-espace fermé de l’espace de Banach $\mathscr{C}(U_n)$ (INT, III, p. 40, § 1, n$^o1)$; puisque ce dernier espace est de type dénombrable (TG, X, p. 25, corollaire), il en est de même de $\mathscr{K}(X,\overline{U}_n)$ (TG, IX, p. 19, cor., (i)). Soit $\mathscr{F}_n$ une partie dénombrable dense de $\mathscr{K}(X,\overline{U}_n)$.

Soit $f\in \mathscr{L}^p(X, \mu)$ et soit $\varepsilon  >0$. Il existe un entier $n\in \mathbf{N}$ tel que $\int_{X-U_n}|f|^p< \varepsilon /2$, et il existe $g\in \mathscr{F}_n$ telle que $\int_{\overline{U}_n}|f-g|^p< \varepsilon /2$. La réunion des classes dans $L^p(X, \mu)$ des éléments des ensembles $\mathscr{F}_n$ est donc dense dans $L^p(X, \mu)$, ce qui conclut la démonstration (TG, IX, p. 18, prop. 12).

### 2. Image essentielle d’une fonction mesurable

Dans ce numéro, on désigne par X un espace topologique localement compact, et par $\mu$ une mesure positive sur X.

#### Définition 1 {#ts-iv-s2-def-1 .statement tag=02YQ}

Soit Y un espace topologique. Pour toute fonction mesurable $g$ de X dans Y, l’image $\mu$-essentielle de $g$ est le sous-ensemble des $y\in Y$ tels que, pour tout voisinage ouvert U de $y$, l’ensemble $\overset{-1}{g}(U)$ n’est pas localement $\mu$-négligeable dans X (INT, IV, p. 172, § 5, n$^o2$, déf. 3).

#### Lemme 1 {#ts-iv-s2-lem-1 .statement tag=02YR}

Soient $g$ une fonction $\mu$-mesurable de X dans un espace topologique Y et S son image $\mu$-essentielle. L’ensemble des éléments $x\in X$ tel que $g(x)$ n’appartienne pas à S est localement $\mu$-négligeable dans X.

Soit $Z =\overset{-1}{g}(Y$ - S) l’ensemble en question.

Supposons d’abord que X est compact et $g$ continue. Dans ce cas, la mesure image $g(\mu)$ est définie (INT, V, p. 69, § 6, n$^o1$, déf. 1) puisque $\mu$ est une mesure bornée. Il résulte des définitions que l’image $\mu$-essentielle de $g$ est le support de la mesure $g(\mu) ($cf. INT, V, p. 70, § 6, n$^o2$, cor. 2), d’où $\mu(Z) =g(\mu)(Y$ - S) = 0 (INT, IV, p. 118, § 2, n$^o2$, prop. 5).

Considérons maintenant le cas général. Soit C un sous-ensemble compact de X, et soit $\varepsilon  >0$ un nombre réel. Puisque $g$ est mesurable, il existe un sous-ensemble compact $C_1\subset C$ tel que $\mu(C$- $C_1)\leqslant \varepsilon$ et tel que $g|C_1$ est continue (INT, IV, p. 169, § 5, n$^o1$, prop. 1). On a alors

$\mu(Z\cap C)\leqslant \mu(C$ - $C_1) +\mu(Z\cap C_1)\leqslant \varepsilon +\mu(Z\cap C_1)$.

Soit $\mu_1$ la mesure induite par $\mu$ sur $C_1$ (INT, IV, p. 186, § 5, n$^o7$, déf. 4). Soit $S_1$ l’image $\mu_1$-essentielle de $g|C_1$. On a $Z\cap C_1\subset$ $(g|C_1)^{-1}(Y$ - $S_1)$. D’après le premier cas, l’ensemble $Z\cap C_1$ est donc $\mu_1$-négligeable, et par conséquent $\mu$-négligeable (INT, IV, p. 187, § 5, n$^o7$, lemme 2, (i)). L’inégalité ci-dessus devient $\mu(Z\cap C)\leqslant \varepsilon$; puisque $\varepsilon$ et C sont arbitraires, l’ensemble Z est localement $\mu$-négligeable (INT, IV, p. 172, § 5, n$^o2$, prop. 5).

#### Lemme 2 {#ts-iv-s2-lem-2 .statement tag=02YS}

Soit $g$ une fonction continue de X dans $\mathbf{C}$. L’image $\mu$-essentielle de $g$ est l’adhérence de l’image par $g$ du support de $\mu$.

Soit Y le support de $\mu$. Si $z\in \mathbf{C}$ n’est pas adhérent à $g$(Y), alors il existe un voisinage ouvert U de $z$ tel que l’ouvert $\overset{-1}{g}(U)$ ne rencontre pas Y et est donc localement $\mu$-négligeable ; cela signifie que $z$ n’appartient pas à l’image $\mu$-essentielle de $g$.

Réciproquement, si $z\in \mathbf{C}$ est adhérent à $g$(Y), alors pour tout voisinage ouvert U de $z$, l’ensemble $\overset{-1}{g}(U)$ est un ouvert dans X qui rencontre Y. Il n’est donc pas $\mu$-négligeable, et puisque c’est un ouvert, il n’est pas localement $\mu$-négligeable (INT, IV, p. 172, § 5, n$^o2$, cor. 2). Donc $z$ appartient à l’image $\mu$-essentielle de $g$.

#### Lemme 3 {#ts-iv-s2-lem-3 .statement tag=02YT}

Soient $g$ une fonction continue de X dans $\mathbf{C}$ et S son image $\mu$-essentielle. On suppose que S n’est pas vide et que $0\in /S$ et on note $\delta$ la distance de 0 à S. On a $\delta  >0$.

Posons $h(x) = 1/g(x)$ si $g(x)\not = 0$ et $h(x) = 0$ sinon. La fonction $h$ appartient à $\mathscr{L}^{\infty}(X, \mu)$. Soit $\widetilde{h}$ la classe de $h$ dans $L^{\infty}(X, \mu)$. On a alors la formule $\delta^{-1}=\|\widetilde{h}\|_{\infty}$.

Soit U un voisinage ouvert de 0 tel que l’ouvert $Z =\overset{-1}{g}(U)$ est localement $\mu$-négligeable, donc négligeable (INT, IV, p. 172, § 5, n$^o2$, cor. 2). Soit Y le support de $\mu$; on a $Y\subset X$ - Z. La restriction de la fonction $h$ à X - Z est continue et bornée, donc $h\in \mathscr{L}^{\infty}(X, \mu)$ et la norme de $\widetilde{h}$ dans $\mathscr{L}^{\infty}(X, \mu)$ est égale à la norme de sa restriction à X - Z. De plus, pour tout $\alpha \in \mathbf{R}_+$, l’ensemble des $x\in X$ - Z tels que $|h(x)|> \alpha$ est un ouvert dans X - Z ; il est donc localement $\mu$-négligeable si et seulement s’il ne rencontre pas Y (INT, IV, loc. cit. et INT, III, p. 66, § 3, n$^o2$, déf. 1). Par conséquent, on a

1

$\|\widetilde{h}\|_{\infty}=$ sup,

$$
_{x\in Y}|g(x)|
$$

d’où

1

= inf $|g(x)|=$ inf $|\lambda |=$ inf $|\lambda |$

$\|\widetilde{h}\|\infty x\in Y\lambda \in g(Y)\lambda \in g(Y)$

qui est égal à $\delta$ d’après le lemme précédent.

### 3. Fonctions universellement mesurables

Dans ce numéro, X est un espace topologique localement compact. On rappelle (INT, V, p. 28, § 3, n$^o4$, déf. 2) qu’une application $f$ de X dans un espace topologique Y est universellement mesurable si elle est $\mu$-mesurable pour toute mesure positive $\mu$ sur X. Il suffit pour cela que $f$ soit $\mu$-mesurable pour toute mesure positive $\mu$ à support compact sur X (INT, V, p. 28, § 4, n$^o3$, prop. 6).

#### Lemme 4 {#ts-iv-s2-lem-4 .statement tag=02YU}

Soient Y et Z des espaces topologiques localement compacts, $f: X\rightarrow Y$ et $g: Y\rightarrow Z$ des applications universellement mesurables. L’application $g\circ f: X\rightarrow Z$ est universellement mesurable.

Soit $\mu$ une mesure positive à support compact sur X et soit C son support. La restriction de $f$ à C est $(\mu|$C)-propre. L’application $g$ est mesurable relativement à la mesure image $(f|C)(\mu|C)$, donc l’application $(g\circ f)|C =g\circ (f|C)$ est $(\mu|$C)-mesurable. Par conséquent, l’application $g\circ f$ est $\mu$-mesurable. Le lemme en résulte.

On note $\mathscr{L}_u(X)$ l’espace vectoriel des fonctions à valeurs complexes qui sont universellement mesurables sur X et $\mathscr{L}_u^{\infty}(X)$ le sous-espace des fonctions $f\in \mathscr{L}_u(X)$ qui sont bornées sur X. Pour $f\in \mathscr{L}_u^{\infty}$(X), on note $\|f\|_{\infty}=$ sup$_{x\in X}|f(x)|$.

#### Proposition 3 {#ts-iv-s2-prop-3 .statement tag=02YV}

a) L’ensemble $\mathscr{L}_u(X)$ est une sous-algèbre involutive de l’algèbre involutive des fonctions de X dans $\mathbf{C}$;

b) L’ensemble $\mathscr{L}_u^{\infty}(X)$ est une sous-algèbre de $\mathscr{L}_u(X)$ et l’application définie par $f\mapsto  \|f\|_{\infty}$ est une norme sur $\mathscr{L}_u^{\infty}(X)$ pour laquelle $\mathscr{L}_u^{\infty}(X)$ est une algèbre stellaire unifère;

c) L’algèbre $\mathscr{L}_u(X)$ contient $\mathscr{C}(X)$ et $\mathscr{L}_u^{\infty}(X)$ contient $\mathscr{C}_b(X)$;

d) Toute fonction borélienne de X dans $\mathbf{C}$ (TG, IX, p. 61, déf. 5) appartient à $\mathscr{L}_u(X)$;

e) Pour toute suite $(f_n)_{n\in\mathbf{N}}$ dans $\mathscr{L}_u(X)$ qui converge simplement vers une fonction $f$ de X dans $\mathbf{C}$, on a $f\in \mathscr{L}_u(X)$.

Les assertions a) et c) résultent des définitions (cf. INT, IV, p. 175, § 5, n$^o3$, cor. 3). L’assertion d) est une conséquence de INT, IV, p. 179, § 5, n$^o5$, th. 4, puisque l’image réciproque par une fonction borélienne de toute partie borélienne de $\mathbf{C}$ est une partie borélienne de X, qui est universellement mesurable (INT, V, p. 28, § 3, n$^o4)$. Enfin, l’assertion e) résulte du théorème d’Egoroff (INT, IV, p. 175, § 5, n$^o4$, th. 2).

Pour démontrer l’assertion b), il suffit de remarquer que e) implique, a fortiori, qu’une limite uniforme de fonctions universellement mesurables est universellement mesurable.

Il peut exister des fonctions universellement mesurables sur X qui ne sont pas boréliennes. En effet, si X est métrisable, la fonction caractéristique d’un sous-ensemble souslinien de X est universellement mesurable (cf. INT, IV, p. 171, § 5, n$^o1$, cor. 2) ; or, dans tout espace polonais non dénombrable, il existe un sous-ensemble souslinien qui n’est pas borélien (« théorème de Souslin » ; cela résulte de TG, IX, p. 120, exerc. 8 et du fait que pour tout espace polonais X non dénombrable, il existe une bijection borélienne $X\rightarrow \mathbf{N}^{\mathbf{N}}$ dont la réciproque est borélienne).

#### Lemme 5 {#ts-iv-s2-lem-5 .statement tag=02YW}

Soit $\mu$ une mesure positive sur X. Soient $g$ une fonction $\mu$-mesurable de X dans $\mathbf{C}$ et S son image $\mu$-essentielle. Pour toute fonction $f\in \mathscr{L}_u(S)$, l’application $h$ de X dans $\mathbf{C}$ telle que $h(x) = 0$ si $g(x)\in /S$ et $h(x) =f(g(x))$ si $g(x)\in S$ est $\mu$-mesurable.

Soient $x\in X$ et U un voisinage ouvert relativement compact de $x$. L’ensemble N = U - $(U\cap \overset{-1}{g}(S))$ est $(\mu|$U)-négligeable. Pour tout entier $n\geqslant 1$, soit $V_n$ un ouvert tel que $N\subset V_n\subset U$ et $\mu(V_n-N)<1/n$ (INT, IV, p. 116, § 1, n$^o4$, prop. 19).

La restriction $\widetilde{g}$ de $g$ à U- $V_n$ est $\mu|(U$- $V_n$)-propre et son image est contenue dans S. Puisque $f$ est universellement mesurable, l’application $x\mapsto f(g(x))$ de U - $V_n$ dans $\mathbf{C}$ est mesurable par rapport à la mesure $\mu|(U$ - $V_n)$ (INT, V, p. 71, § 6, n$^o2$, prop. 3). L’application $h_n$ de X dans $\mathbf{C}$ telle que $h_n(x) = 0$ si $x /\in U$ - $V_n$ et $h_n(x) =f(g(x))$ si $x\in U$ - $V_n$ est donc $\mu$-mesurable (INT, IV, p. 193, § 5, n$^o10$, prop. 16).

Comme $h_n(x)\rightarrow h(x)$ pour $\mu$-presque tout $x\in U$, la restriction de $h$ à U est $\mu$-mesurable (INT, IV, p. 175, § 5, n$^o4$, th. 2). On conclut que $h$ est $\mu$-mesurable d’après le principe de localisation (INT, IV, p. 171, § 4, n$^o2$, prop. 4).

#### Remarque {#ts-iv-s2-n3-rem-1 .statement tag=02YX}

Sous les hypothèses du lemme, notons par abus de langage $f\circ g$ la fonction $h$ définie dans le lemme.

Si $g=g_1$ localement $\mu$-presque partout sur X, les fonctions $g$ et $g_1$ ont même image $\mu$-essentielle et on a $f\circ g=f\circ g_1$.

Si $g$ est une fonction $\mu$-mesurable définie $\mu$-presque sur X, on notera également $f\circ g$ la fonction $f\circ g_1$ où $g_1$ est une fonction $\mu$-mesurable définie sur X égale à $g$ localement $\mu$-presque partout.

### 4. L’algèbre stellaire $L^{\infty}(X, \mu)$

Soit X un espace topologique localement compact et soit $\mu$ une mesure positive sur X. On considère l’algèbre stellaire commutative $L^{\infty}(X, \mu)$ (exemple 4 de I, p. 103).

#### Lemme 6 {#ts-iv-s2-lem-6 .statement tag=02YY}

Soit $g\in \mathscr{L}^{\infty}(X, \mu)$. Le spectre de la classe de $g$ dans $L^{\infty}(X, \mu)$ est égal à l’image $\mu$-essentielle de $g$.

Notons $\widetilde{g}$ la classe de $g$ dans $L^{\infty}(X, \mu)$ et S l’image $\mu$-essentielle de $g$. Soit $z\in \mathbf{C}-$ S. Par définition, il existe un voisinage ouvert U de $z$ tel que $Y =\overset{-1}{g}(U)$ est localement $\mu$-négligeable. La fonction $h$ définie par $h(x) = (g(x)-z)^{-1}$ si $x /\in Y$, et $h(x) = 0$ si $x\in Y$, appartient alors à $\mathscr{L}^{\infty}(X, \mu)$. Sa classe $\widetilde{h}$ dans $L^{\infty}(X, \mu)$ vérifie $(\widetilde{g}-z)\widetilde{h}= 1$, puisque $(g(x)-z)h(x) = 1$ pour tout $x$ n’appartenant pas à l’ensemble localement $\mu$-négligeable Y. Donc $z\in \mathbf{C}-$ Sp($\widetilde{g}$).

Réciproquement, soit $z\in \mathbf{C}-$ Sp($\widetilde{g}$). Soit $h\in \mathscr{L}^{\infty}(X, \mu)$ une fonction dont la classe est l’inverse de $\widetilde{g}-z$ dans $L^{\infty}(X, \mu)$. Il existe un nombre réel $M>0$ tel que $|h(x)|\leqslant M$ localement $\mu$-presque partout, et de plus on a $(g(x)-z)h(x) = 1$ localement $\mu$-presque partout. Soit U la boule ouverte de centre $z$ et de rayon $M^{-1}$ dans $\mathbf{C}$; alors $\overset{-1}{g}(U)$ est contenu dans l’ensemble localement $\mu$-négligeable

$-1$

$$
h(]M,+\infty [)\cup  \{x\in X|(g(x)-z)h(x)\not = 1\}
$$

donc $z\in \mathbf{C}-$ S. On a démontré le lemme.

#### Proposition 4 {#ts-iv-s2-prop-4 .statement tag=02YZ}

Soit $g\in \mathscr{L}^{\infty}(X, \mu)$. Notons $\widetilde{g}$ la classe de $g$ dans $L^{\infty}(X, \mu)$ et S le spectre de $\widetilde{g}$. L’application $f\mapsto f\circ g$ (remarque, p. 184) est l’application de calcul fonctionnel de $\mathscr{C}(S)$ dans $L^{\infty}(X, \mu)$ associée à $\widetilde{g}$.

Soit $f\in \mathscr{C}(S)$. La fonction $h=f\circ g$ est $\mu$-mesurable (lemme 5 de IV, p. 184) et bornée. Notons $f\widetilde{\circ}g$ sa classe dans $L^{\infty}(X, \mu)$. L’application $f\mapsto f\widetilde{\circ}g$ est un morphisme continu d’algèbres involutives unifères de $\mathscr{C}(S)$ dans $L^{\infty}(X, \mu)$. Puisque $g(x)$ appartient à S localement $\mu$-presque partout (lemme 1 de IV, p. 181 et lemme 6), ce morphisme associe à l’application identique de S la classe $\widetilde{g}$ de la fonction $g$. Il coïncide donc avec l’application de calcul fonctionnel de $\widetilde{g}$ (prop. 7 de I, p. 111).

### 5. Endomorphismes de multiplication

Soit X un espace topologique localement compact et soit $\mu$ une mesure positive sur X. Soit $p\in [1,+\infty [$.

Soit $g\in \mathscr{L}^{\infty}(X, \mu)$. Notons $m_g$ l’application $f\mapsto g\cdot f$ de $\mathscr{L}^p(X, \mu)$ dans lui-même. L’application $m_g$ est linéaire et continue puisque

$$
N_p(m_g(f))\leqslant N_{\infty}(g)N_p(f) \tag{1}
$$

pour toute fonction $f\in \mathscr{L}^p(X, \mu)$. En particulier, la fonction $m_g(f)$ est $\mu$-négligeable si $f$ est $\mu$-négligeable. L’application $m_g$ induit donc, par passage aux quotients, un endomorphisme de $L^p(X, \mu)$, qui sera noté $\widetilde{m}_g$.

#### Lemme 7 {#ts-iv-s2-lem-7 .statement tag=02Z0}

Soit $g\in \mathscr{L}^{\infty}(X, \mu)$. L’endomorphisme $\widetilde{m}_g$ de $L^p(X, \mu)$ est injectif si et seulement si l’ensemble des $x\in X$ tels que $g(x) = 0$ est localement $\mu$-négligeable.

Notons A l’ensemble des $x\in X$ tels que $g(x) = 0$.

Supposons que A est localement $\mu$-négligeable. Soit $f\in \mathscr{L}^p(X, \mu)$ et $\widetilde{f}$ sa classe dans $L^p(X, \mu)$. Supposons que $\widetilde{m}_g(\widetilde{f}) = 0$. Par définition, c’est le cas si et seulement si la fonction $f g$ est $\mu$-négligeable, de sorte que l’ensemble B des $x\in X$ tels que $f(x)g(x)\not = 0$ est $\mu$-négligeable. La fonction $f$ est nulle en dehors de $A\cup B$, donc est $\mu$-négligeable. Cela implique que l’endomorphisme $\widetilde{m}_g$ est injectif.

Réciproquement, supposons que A n’est pas localement $\mu$-négligeable. Soit C une partie compacte de X telle que $A\cap C$ n’est pas $\mu$-négligeable, et soit $\varphi$ la fonction caractéristique de $A\cap C$. La classe de la fonction $\varphi$ dans $L^p(X, \mu)$ n’est pas nulle, mais celle de $m_g(\varphi )$ l’est, donc $m_g$ n’est pas injectif.

Puisque le produit d’une fonction localement $\mu$-négligeable et d’une fonction $\mu$-négligeable est $\mu$-négligeable, l’endomorphisme $\widetilde{m}_g$ ne dépend que de la classe de $g$ dans $L^{\infty}(X, \mu)$. Pour $\widetilde{g}\in L^{\infty}(X, \mu)$, on note également $\widetilde{m}_g$ l’endomorphisme $\widetilde{m}_g$ de $L^p(X, \mu)$ pour toute fonction $g\in \mathscr{L}^{\infty}(X, \mu\widetilde{)}$ dont $\widetilde{g}$ est la classe. On dit que $\widetilde{m}_g$ est l’endomorphisme de multiplication par $\widetilde{g}$ dans $L^p(X, \mu)$.

#### Proposition 5 {#ts-iv-s2-prop-5 .statement tag=02Z1}

Soit $p\in [1,+\infty [$. L’application $m:g\mapsto \widetilde{m}_g$ de $L^{\infty}(X, \mu)$ dans $\mathscr{L}(L^p(X, \mu))$ est un morphisme isométrique d’algèbres de Banach unifères.

Pour $a,b$ dans $\mathbf{C}$ et $g_1,g_2$ dans $L^{\infty}(X, \mu)$, on vérifie aussitôt que $\widetilde{m}_{ag_1+bg_2}=a\widetilde{m}g_1+b\widetilde{m}_{g_2}$, donc l’application $\widetilde{m}$ est linéaire. De plus, on a $\widetilde{m}_1= 1_{L^p(X,\mu)}$ et $\widetilde{m}_{g_1g_2}=\widetilde{m}_{g_1}\widetilde{m}_{g_2}$, donc l’application $\widetilde{m}$ est un morphisme d’algèbres unifères de $L^{\infty}(X, \mu)$ dans $\mathscr{L}(L^p(X, \mu))$.

La formule (1) ci-dessus démontre que $\widetilde{m}$ est de norme $\leqslant 1$.

Soient $g\in \mathscr{L}^{\infty}(X, \mu)$ et $\widetilde{g}$ sa classe dans $L^{\infty}(X, \mu)$. Soit $\varepsilon  >$ 0. L’ensemble Y des $x\in X$ tels que $|g(x)|>\|\widetilde{g}\|_{\infty}-\varepsilon$ n’est pas localement $\mu$-négligeable. Il existe donc un sous-ensemble compact C de X tel que $\mu(Y\cap C)>0$. Soit $\varphi$ la fonction caractéristique de $Y\cap C$. Comme

$\int 1/p\int 1/p$

$\|\widetilde{m}_g(\varphi )\|_p=|\varphi g|^pd\mu\geqslant |\varphi g|^pd\mu$

X Y

$$
\geqslant (\|\widetilde{g}\|_{\infty}-\varepsilon )\mu(Y\cap C)^{1/p}= (\|\widetilde{g}\|_{\infty}-\varepsilon )\|\varphi \|_p
$$

il vient $\|\widetilde{m}_{\widetilde{g}}\|\geqslant \|\widetilde{g}\|_{\infty}-\varepsilon$. Puisque $\varepsilon$ est arbitraire, on en déduit que $\|\widetilde{m}_{\widetilde{g}}\|\geqslant \|\widetilde{g}\|_{\infty}$, ce qui démontre que $\widetilde{m}$ est isométrique.

#### Lemme 8 {#ts-iv-s2-lem-8 .statement tag=02Z2}

Soit $(g_n)$ une suite bornée dans $\mathscr{L}^{\infty}(X, \mu)$ convergeant simplement $\mu$-presque partout. Soit $\widetilde{m}\in L^{\infty}(X, \mu)$ la classe de sa limite. Alors $\widetilde{m}_{g_n}$ converge vers $\widetilde{m}_{\widetilde{g}}$ dans l’espace $\mathscr{L}(L^p(X, \mu))$ muni de la topologie de la convergence simple.

Soit $f\in \mathscr{L}^p(X, \mu)$. La suite $(g_nf)$ est bornée dans $\mathscr{L}^p(X, \mu)$ et converge simplement $\mu$-presque partout vers $gf$. D’après le théorème de Lebesgue (INT, IV, p. 137, § 3, n$^o7$, th. 6), la suite $(g_nf)$ converge vers $gf$ dans $\mathscr{L}^p(X, \mu)$, et l’assertion en résulte.

On va considérer maintenant le cas où $p= 2$.

#### Proposition 6 {#ts-iv-s2-prop-6 .statement tag=02Z3}

L’application $m:g\mapsto \widetilde{m}_g$ est un morphisme unifère isométrique de l’algèbre stellaire $L^{\infty}(X, \mu)$ dans l’algèbre stellaire $\mathscr{L}(L^2(X, \mu))$.

En particulier, pour tout $g\in L^{\infty}(X, \mu)$, l’endomorphisme de multiplication $\widetilde{m}_g$ est normal; il est hermitien si et seulement si $g$ est localement $\mu$-presque partout à valeurs réelles.

D’après la prop. 5, l’application $\widetilde{m}$ est un morphisme injectif et isométrique d’algèbres de Banach unifères de $L^{\infty}(X, \mu)$ dans $\mathscr{L}(L^2(X, \mu))$. Soit $g\in \mathscr{L}^{\infty}(X, \mu)$. Pour $f_1$ et $f_2\in \mathscr{L}^2(X, \mu)$, on a

$$
\langle f_1|\widetilde{m}_g(f_2)\rangle =\int_X\overline{f_1(x)}g(x)f_2(x)d\mu(x) =\langle \widetilde{m}_{\overline{g}}(f_1)|f_2\rangle
$$

dont il résulte que $\widetilde{m}^*_g=\widetilde{m}_{\overline{g}}$, ce qui démontre que $m$ est un morphisme involutif. Les dernières assertions en résultent (cf. I, p. 106, prop. 5).

#### Corollaire {#ts-iv-s2-n5-cor-1 .statement tag=02Z4}

Soit $g\in L^{\infty}(X, \mu)$.

a) Le spectre de $\widetilde{m}_g$ dans $\mathscr{L}(L^2(X, \mu))$ est l’image $\mu$-essentielle de $g$;

b) L’endomorphisme $\widetilde{m}_g$ est positif si et seulement si $g$ est localement $\mu$-presque partout à valeurs positives;

c) Pour toute fonction $f\in \mathscr{C}$ (Sp($\widetilde{m}_g$)), on a $f(\widetilde{m}_g) =\widetilde{m}_{f\circ g}$.

Puisque $\widetilde{m}$ est injective, on a Sp($\widetilde{m}_g$) $=$ Sp($g$) d’après la prop. 5 de I, p. 106 ; le résultat découle alors du lemme 6 de IV, p. 185, de la proposition 4 de IV, p. 185 et de la définition 6 de I, p. 115.

#### Proposition 7 {#ts-iv-s2-prop-7 .statement tag=02Z5}

L’image du morphisme $\widetilde{m}$ de $L^{\infty}(X, \mu)$ dans $\mathscr{L}(L^2(X, \mu))$ est une sous-algèbre commutative maximale de l’algèbre $\mathscr{L}(L^2(X, \mu))$.

Il suffit de démontrer que si $u\in \mathscr{L}(L^2(X, \mu))$ est un endomorphisme qui commute à $\widetilde{m}_g$ pour toute fonction $g\in \mathscr{L}^{\infty}(X, \mu)$, alors $u$ appartient à l’image de $\widetilde{m}$. Soit $u$ un tel endomorphisme.

On note $\widetilde{f}$ la classe dans $L^2(X, \mu)$ d’une fonction $f\in \mathscr{L}^2(X, \mu)$. Notons $v$ l’application linéaire de $\mathscr{L}^2(X, \mu)$ dans $L^2(X, \mu)$ définie par $f\mapsto u(\widetilde{f})$. On a $v\circ m_g=\widetilde{m}_g\circ v$ pour tout $g\in \mathscr{L}^{\infty}(X, \mu)$.

Pour toute partie $\mu$-mesurable Y de X, on note $\varphi_Y$ sa fonction caractéristique ; l’endomorphisme $\widetilde{m}_{\varphi_Y}$ est un orthoprojecteur de $L^2(X, \mu)$.

Supposons d’abord que X est compact, de sorte que la classe de la fonction constante 1 appartient à $L^2(X, \mu)$. Soit $g$ une fonction dans $\mathscr{L}^2(X, \mu)$ dont la classe dans $L^2(X, \mu)$ est $v(1)$.

Soient $c$ un nombre réel positif et Y l’ensemble des $x\in X$ tels que $|g(x)|\geqslant c$; c’est un ensemble $\mu$-mesurable. On a dans $L^2(X, \mu)$ les égalités $\varphi_{\widetilde{Y}}g=\widetilde{m}_{\varphi_Y}(v(1)) =v(m_{\varphi_Y}(1)) =v(\varphi_Y)$.

Comme de plus $|c\varphi_Y|\leqslant |g\varphi_Y|$, on obtient

$$
c^2\mu(Y) =\int_X(c\varphi_Y)^2d\mu\leqslant \int_X|\varphi_Yg|^2d\mu=\|\widetilde{u}(\varphi_Y)\|^2\leqslant \|u\|^2\mu(Y)
$$

Cette inégalité implique que $\mu(Y) = 0$ si $c >\|u\|$, de sorte que la fonction $g$ est bornée $\mu$-presque partout par $\|u\|$. Pour toute fonction $f\in \mathscr{C}$(X), on a enfin

$$
u(\widetilde{f}) =v(m_f(1)) =\widetilde{m}_f(v(1)) =\widetilde{m}_f(\widetilde{g}) =\widetilde{m}_g(\widetilde{f})
$$

d’où l’égalité $u=\widetilde{m}_g$, et en particulier $N_{\infty}(g) =\|u\|$.

Considérons maintenant le cas général. Il existe une famille localement dénombrable $(X_i)_{i\in I}$ de parties compactes deux à deux disjointes de X telle que Z = X $-\bigcup_{i\in I}X_i$ est localement $\mu$-négligeable (INT, IV, p .190, § 5, n$^o9$, prop. 14). Notons $\mu_i$ la mesure induite par $\mu$ sur $X_i$ (INT, IV, p. 186, § 5, n$^o7$, déf. 4).

D’après la prop. 1 de IV, p. 179, pour tout $i\in I$, l’image $E_i$ de $\widetilde{m}_{\varphi_{Xi}}$ s’identifie à $L^2(X_i, \mu_i)$ par $f\mapsto f|X_i$. Pour toute fonction $g\in \mathscr{L}^{\infty}(X, \mu)$, l’endomorphisme de multiplication $\widetilde{m}_g$ commute avec $\widetilde{m}_{\varphi_{Xi}}$, donc laisse stable $E_i$, et l’endomorphisme de $E_i$ déduit de $\widetilde{m}_g$ par passage aux sous-espaces coïncide avec l’endomorphisme de multiplication par $g|X_i$ sur $L^2(X_i, \mu_i)$.

Comme $u$ commute avec $m_{\varphi_{Xi}}$, il laisse également stable le sous-espace $E_i$. Notons $u_i$ l’endomorphisme de $L^2(X_i, \mu_i)$ déduit de $u$ par passage aux sous-espaces.

L’application de $\mathscr{L}^{\infty}(X, \mu)$ dans $\mathscr{L}^{\infty}(X_i, \mu_i)$ définie par $g\mapsto g|X_i$ étant surjective, l’hypothèse implique que $u_i$ commute avec $\widetilde{m}_g$ pour toute fonction $g\in \mathscr{L}^{\infty}(X_i, \mu_i)$. D’après la première partie de la démonstration, il existe une fonction $g_i\in \mathscr{L}^{\infty}(X_i, \mu_i)$ telle que $u_i=\widetilde{m}_{g_i}$ et $N_{\infty}(g_i)\leqslant \|u_i\|\leqslant \|u\|$.

La fonction $g$ sur X qui coïncide avec $g_i$ sur $X_i$ et qui est nulle sur Z est bornée et $\mu$-mesurable (INT, IV, p. 193, § 5, n$^o10$, prop. 16) donc $g\in \mathscr{L}^{\infty}(X, \mu)$. Pour tout $i\in I$, la restriction de $u$ à $E_i$ coïncide avec celle de $\widetilde{m}_g$; on a $u=m_g$ par conséquent d’après la prop. 1, c) de IV, p. 179.

#### Corollaire {#ts-iv-s2-n5-cor-2 .statement tag=02Z6}

Soit $u$ un endomorphisme de l’espace hilbertien $L^2(X, \mu)$ permutable à $\widetilde{m}_g$ pour toute fonction $g\in \mathscr{K}(X)$. Alors il existe un unique élément $f\in L^{\infty}(X, \mu)$ tel que $u=\widetilde{m}_f$.

D’après la prop. 7, il suffit de démontrer que $u$ commute avec $\widetilde{m}_g$ pour tout $g\in \mathscr{L}^{\infty}(X, \mu)$. Soient $h_1$ et $h_2$ des éléments de $\mathscr{L}^2(X, \mu)$ de classes $\widetilde{h}_1$ et $\widetilde{h}_2$ dans $L^2(X, \mu)$. Soit $k_1$ (resp. $k_2)$ une fonction dans $\mathscr{L}^2(X, \mu)$ dont la classe est $u(\widetilde{h}_1)$ (resp. $u^*(\widetilde{h}_2))$.

Notons $h=h_1\overline{k}_2-k_1\overline{h}_2$; on a $h\in \mathscr{L}^1(X, \mu)$. Définissons la mesure $\nu =h\cdot \mu$ sur X ; elle est bornée. Pour tout $g\in \mathscr{L}^{\infty}(X, \mu)$, on a

$$
\langle \widetilde{h}_2|u(\widetilde{m}_g(\widetilde{h}_1))-\widetilde{m}_g(u(\widetilde{h}_1))\rangle =\langle u^*(\widetilde{h}_2)|\widetilde{m}_g(\widetilde{h}_1)\rangle  - \langle \widetilde{h}_2|\widetilde{m}_g(u(\widetilde{h}_1))\rangle
$$

$$
=\int_Xg\cdot h_1\cdot \overline{k}_2d\mu-\int_Xg\cdot k_1\cdot \overline{h}_2d\mu=\nu (g)
$$

On a donc par hypothèse $\nu (g) = 0$ pour toute fonction $g\in \mathscr{K}$ (X), c’est-à-dire $\nu = 0$. Par conséquent, il vient

$$
\langle \widetilde{h}_2|u(\widetilde{m}_g(\widetilde{h}_1))-\widetilde{m}_g(u(\widetilde{h}_1))\rangle =\nu (g) = 0
$$

pour tout $g\in \mathscr{L}^{\infty}(X, \mu)$. Puisque c’est le cas pour tous $h_1$ et $h_2$ dans $\mathscr{L}^2(X, \mu)$, on a $u\circ \widetilde{m}_g=\widetilde{m}_g\circ u$.

#### Remarque {#ts-iv-s2-n5-rem-1 .statement tag=02Z7}

Dans la suite, on notera souvent simplement $m_g$ l’endomorphisme de multiplication par $g$ sur $L^p(X, \mu)$.

### 6. Mesures spectrales

Dans ce numéro, on fixe un espace hilbertien complexe E.

Rappelons que si A est une algèbre stellaire unifère commutative, on note $\mathsf{X}(A)$ l’espace topologique compact de ses caractères unifères (cor. 1 de I, p. 29) et $\mathscr{G}_A$ la transformation de Gelfand de A (déf. 5 de I, p. 7) qui est un isomorphisme isométrique d’algèbres unifères involutives de A sur $\mathscr{C}(\mathsf{X}(A))$ (th. 1 de I, p. 108). On notera $\mathscr{H}_A$ l’isomorphisme réciproque.

#### Lemme 9 {#ts-iv-s2-lem-9 .statement tag=02Z8}

Soit A une sous-algèbre stellaire unifère commutative de $\mathscr{L}(E)$. Pour tous $x$ et $y$ dans E, l’application $\mu$ de $\mathsf{X}(A)$ dans $\mathbf{C}$ définie par $\mu(f) =\langle x|\mathscr{H}_A(f)y\rangle$ pour tout $f\in \mathscr{C}(\mathsf{X}(A))$ est une mesure bornée sur l’espace compact $\mathsf{X}(A)$. Elle est positive si $x=y$. Sa norme est $\leqslant \|x\| \|y\|$, avec égalité si $x=y$.

L’application $\mu$ est linéaire. Pour toute fonction $f\in \mathscr{C}(\mathsf{X}$(A)), on a

$$
|\mu(f)|\leqslant \|x\| \|y\| \|\mathscr{H}_A(f)\|=\|x\| \|y\| \|f\|
$$

donc $\mu$ est une mesure bornée sur $\mathsf{X}(A)$ de norme $\leqslant \|x\| \|y\|$.

Supposons que $x=y$. Pour toute fonction positive $f\in \mathscr{C}(\mathsf{X}$(A)), l’élément $\mathscr{H}_A(f)$ est un élément positif de A (exemple 1 de I, p. 115), donc un élément positif de $\mathscr{L}$ (E), d’où $\mu(f) =\langle x|\mathscr{H}_A(f)(x)\rangle \geqslant 0$ (prop. 8 de I, p. 138). Ceci montre que $\mu$ est une mesure positive. Comme $\mu(1) =\|x\|^2$, la masse totale de $\mu$ est $\|x\|^2$ (INT, III, p. 58, § 1, n$^o8$, cor. 2).

#### Définition 2 {#ts-iv-s2-def-2 .statement tag=02Z9}

Soit A une sous-algèbre stellaire unifère commutative de $\mathscr{L}(E)$. Pour tous $x$ et $y$ dans E, la forme linéaire $f\mapsto  \langle x|\mathscr{H}_A(f)y\rangle$ sur $\mathscr{C}(\mathsf{X}(A))$ s’appelle la mesure spectrale de $(x, y)$ relative à A. Si $x=y$, on dit que c’est la mesure spectrale de $x$ relative à A.

#### Remarque {#ts-iv-s2-n6-rem-1 .statement tag=02ZA}

Soit A une sous-algèbre stellaire unifère commutative de $\mathscr{L}(E)$. Pour tous $x$ et $y$ dans E, notons $\mu_{x,y}$ la mesure spectrale de $(x, y)$ relativement à A. L’application définie par $(x, y)\mapsto \mu_{x,y}$ de $E\times E$ dans $\mathscr{M}^1(\mathsf{X}(A))$ est sesquilinéaire.

Soit $u$ un endomorphisme normal de E et A la sous-algèbre stellaire unifère de $\mathscr{L}(E)$ engendrée par $u$. Elle est commutative. L’espace $\mathsf{X}(A)$ s’identifie à Sp($u$) par l’application $\chi \mapsto \chi (u)$ (lemme 10 de I, p. 109). La mesure spectrale $\mu_{x,y}$ de $(x, y)$ relative à A s’identifie donc à une mesure sur Sp($u$), appelée la mesure spectrale de $(x, y)$ relative à $u$. Pour toute fonction $f\in \mathscr{C}$ (Sp($u$)), on a alors

$$
\int f d\mu_{x,y}=\langle x|f(u)y\rangle
$$

Sp($u$)

d’après la déf. 5 de I, p. 110.

### 7. Algèbres stellaires commutatives d’endomorphismes d’un espace hilbertien

#### Définition 3 {#ts-iv-s2-def-3 .statement tag=02ZB}

Soient A une algèbre sur $\mathbf{C}$ et E un espace vectoriel topologique complexe. Soit $\pi$ une représentation de A dans E. On dit qu’un élément $x$ de E est un vecteur cyclique pour $\pi$ si l’ensemble des éléments $\pi (a)x$ pour $a\in A$ est total dans E.

Soit $u\in \mathscr{L}(E)$ un endomorphisme de E. On dit que $x\in E$ est un vecteur cyclique pour $u$ si c’est un vecteur cyclique pour la représentation identique de la sous-algèbre stellaire engendrée par $u$ dans $\mathscr{L}(E)$.

#### Proposition 8 {#ts-iv-s2-prop-8 .statement tag=02ZC}

Soit E un espace hilbertien complexe. Soit A une sous-algèbre stellaire unifère commutative de $\mathscr{L}(E)$. Soit $x$ un élément de E. Posons $E_x= A\cdot x$ et notons $\mu_x$ la mesure spectrale de $x$ relative à A.

Il existe un unique isomorphisme isométrique $\theta_x$ de $L^2(\mathsf{X}(A), \mu_x)$ sur $E_x$ tel que $\theta_x(f) =\mathscr{H}_A(f)(x)$ pour toute fonction $f\in \mathscr{C}(\mathsf{X}(A))$. Pour tout élément $a\in A$, l’espace $E_x$ est stable par $a$, et si on note $a_x$ l’endomorphisme de $E_x$ déduit de $a$ par passage aux sous-espaces, alors on a $a_x\circ \theta_x=\theta_x\circ m_{\mathscr{G}_A(a)}$.

Soit $\widetilde{\theta}_x$ l’application linéaire de $\mathscr{C}(\mathsf{X}(A))$ dans $E_x$ définie par

$$
\widetilde{\theta}_x(f) =\mathscr{H}_A(f)(x)
$$

Pour toute fonction $f\in \mathscr{C}(\mathsf{X}$(A)), on a

$$
\|\widetilde{\theta}_x(f)\|^2=\langle \mathscr{H}_A(f)x|\mathscr{H}_A(f)x\rangle =\langle x|\mathscr{H}_A(|f|^2)x\rangle =\int_{\mathsf{X}(A)}|f|^2d\mu_x
$$

Puisque $\mathscr{C}(\mathsf{X}(A))$ est dense dans $\mathscr{L}^2(\mathsf{X}(A), \mu_x)$, il existe une unique application linéaire isométrique de $L^2(\mathsf{X}(A), \mu_x)$ dans $E_x$ qui prolonge $\widetilde{\theta}_x$; on la note $\theta_x$. L’application $\theta_x$ est surjective puisque son image est fermée (lemme 8 de I, p. 107) et contient $A\cdot x$. C’est donc un isomorphisme isométrique.

Soit $a\in A$. Notons $g=\mathscr{G}_A(a)\in \mathscr{C}(\mathsf{X}(A))$. L’espace $E_x$ est stable par $a$. Pour $f\in \mathscr{C}(\mathsf{X}$(A)), on a alors

$$
\widetilde{\theta}_x(m_g(f)) =\mathscr{H}_A(\mathscr{G}_A(a)f)x= (a\circ \mathscr{H}_A(f))x=a(\widetilde{\theta}_x(f))
$$

et il en résulte que $\theta_x\circ m_g=a_x\circ \theta_x$.

#### Corollaire {#ts-iv-s2-n7-cor-1 .statement tag=02ZD}

Soit E un espace hilbertien complexe. Soit A une sous-algèbre stellaire unifère commutative de $\mathscr{L}(E)$ admettant un vecteur cyclique $x$. Soit $\mu_x$ la mesure spectrale de $x$ relative à A. Il existe un unique isomorphisme isométrique

$$
\theta_x: L^2(\mathsf{X}(A), \mu_x)\rightarrow E
$$

tel que $\theta_x(f) =\mathscr{H}_A(f)$ pour toute fonction $f\in \mathscr{C}(\mathsf{X}(A))$. Pour tout $a$ dans A, on a $a\circ \theta_x=\theta_x\circ m_{\mathscr{G}_A(a)}$.

En effet, on a alors $E_x= E$ et $a_x=a$ pour tout $a\in A$.

Soit E un espace hilbertien complexe. Soit $x\in E$ et soit A une sous-algèbre stellaire unifère commutative de $\mathscr{L}(E)$. Notons $E_x$ le sous-espace fermé $A\cdot x$ de E. Pour tout $a\in A$, on a alors $a(E_x)\subset E_x$. Notons $A_x$ la sous-algèbre stellaire unifère commutative de $\mathscr{L}(E_x)$ formée des endomorphismes de $E_x$ déduits des éléments de A par passage aux sous-espaces. Le vecteur $x$ est un vecteur cyclique pour $A_x\subset \mathscr{L}(E_x)$.

#### Proposition 9 {#ts-iv-s2-prop-9 .statement tag=02ZE}

Il existe un sous-ensemble C de E tel que E est somme hilbertienne des espaces $E_x$ pour $x\in$ C. Si E est de type dénombrable, l’ensemble C est dénombrable.

Soit $\mathscr{O}$ l’ensemble des parties C de E telles que les sous-espaces $E_x$ pour $x\in C$ soient deux à deux orthogonaux. L’ensemble $\mathscr{O}$, ordonné par l’inclusion, est de caractère fini (E, III, p. 34, déf. 2) puisque C appartient à $\mathscr{O}$ si et seulement si les ensembles formés de deux éléments de C appartiennent à $\mathscr{O}$. D’après E, III, p. 35, th. 1, il existe un élément maximal C de $\mathscr{O}$.

Soit F le sous-espace fermé de E engendré par les sous-espaces $E_x$ pour $x\in C$. Il suffit de démontrer que $F^{\circ}$ est réduit à 0 pour achever la preuve de la proposition. Soit $y$ un élément de $F^{\circ}$. Pour tout $x\in C$ et tous $a$ et $b$ dans A, on a $\langle a(y)|b(x)\rangle =\langle y|a^*b(x)\rangle = 0$ puisque $a^*b(x)$ appartient à $E_x$, donc à F. Comme les éléments $a(y)$ (resp. $b(x))$ engendrent un sous-espace dense de $E_y$ (resp. $E_x)$, on a donc $E_y\subset E^{\circ}_x$. Puisque C est maximal dans $\mathscr{O}$, cela signifie que $E_y$ est réduit à 0, donc que $y= 0$.

Supposons que E est de type dénombrable. Comme $E_x$ est non nul pour tout $x\in C$ non nul, tout ensemble C tel que E est somme hilbertienne des espaces $E_x$ pour $x\in C$ est dénombrable.

#### Théorème 1 {#ts-iv-s2-thm-1 .statement tag=02ZF}

Soit A une sous-algèbre stellaire unifère commutative de $\mathscr{L}(E)$. Il existe un espace topologique localement compact X, une mesure positive $\mu$ sur X, un isomorphisme isométrique $\theta$ de $L^2(X, \mu)$ sur E et un morphisme isométrique d’algèbres stellaires $\pi$ de A dans $\mathscr{C}_b(X)$ tels que pour tout $a\in A$, on ait

$$
a\circ \theta =\theta \circ m_{\pi(a)}
$$

D’après la prop. 9, il existe une partie C de E telle que E soit la somme hilbertienne des sous-espaces $E_x$ pour $x\in C$. Soit X l’espace topologique localement compact $\mathsf{X}(A)\times C$, où C est muni de la topologie discrète. Il existe une unique mesure $\mu$ sur X telle que $\mu|(\mathsf{X}(A)\times  \{x\})$ s’identifie à la mesure spectrale $\mu_x$ de $x$ pour tout $x\in C$ (INT, III, p. 65, § 2, n$^o1$, prop. 1) ; cette mesure est positive (cf. loc. cit.). On a alors une décomposition en somme hilbertienne

$$
L^2(X, \mu) =\bigoplus_{x\in C}L^2(\mathsf{X}(A), \mu_x)
$$

(prop. 1 de IV, p. 179, c) appliquée aux ensembles $\mathsf{X}(A)\times  \{x\}$ pour $x\in C)$. Il existe donc une unique isométrie $\theta : L^2(X, \mu)\rightarrow E$ qui coïncide avec $\theta_x: L^2(\mathsf{X}(A), \mu_x)\rightarrow E_x$ sur $L^2(\mathsf{X}(A), \mu_x)$ pour tout $x\in C$.

Soit $p: X\rightarrow \mathsf{X}(A)$ la projection canonique ; elle est surjective, donc l’application linéaire $p^*:\mathscr{C}_b(\mathsf{X}(A))\rightarrow \mathscr{C}(X)$ définie par $f\mapsto f\circ p$ est injective. Notons $\pi =p^*\circ \mathscr{G}_A$; c’est un morphisme injectif d’algèbres stellaires de A dans $\mathscr{C}_b(X)$; il est donc isométrique (prop. 9 de I, p. 112).

Soit $a\in A$. Pour tout $x\in C$, on a $a_x\circ \theta_x=\theta_x\circ m_{\mathscr{G}_A(a)}$. Les applications linéaires continues $a\circ \theta$ et $\theta \circ m_{\pi(a)}$ coïncident donc sur les sous-espaces $L^2(\mathsf{X}(A), \mu_x)$, et sont par conséquent égales.

#### Corollaire (Théorème spectral) {#ts-iv-s2-n7-cor-2 .statement tag=02ZG}

Soit E un espace hilbertien complexe. Soit $u\in \mathscr{L}(E)$ un endomorphisme normal de E. Il existe un espace topologique localement compact X, une mesure positive $\mu$ sur X, un isomorphisme isométrique $\theta$ de $L^2(X, \mu)$ sur E et une fonction continue et bornée $g$ sur X tels que $u=\theta \circ m_g\circ \theta^{-1}$.

Si $u$ admet un vecteur cyclique $x$, on peut prendre X = Sp($u$) et pour $g$ la fonction identique de X.

Il suffit d’appliquer le théorème 1 (resp. le corollaire de la proposition 8) à la sous-algèbre stellaire A de $\mathscr{L}(E)$ qui est engendrée par $u$, et de poser $g=\pi (u)$.

Cet énoncé réduit toute question portant sur un seul endomorphisme normal d’un espace hilbertien à une question similaire pour un opérateur de multiplication, ce qui en simplifie souvent l’étude (cf. par exemple l’exercice 19 de IV, p. 325).

### 8. Continuité du calcul fonctionnel

Dans ce numéro, on considère les propriétés de continuité du calcul fonctionnel par rapport aux deux variables.

Pour une algèbre stellaire A et un élément normal $a$ de A, et pour une fonction $f$ continue sur un sous-ensemble de $\mathbf{C}$ contenant Sp$_A(a)$, on note $f(a)$ l’élément obtenu par le calcul fonctionnel continu de $a$ appliqué à la restriction de $f$ au spectre de $a$.

#### Proposition 10 {#ts-iv-s2-prop-10 .statement tag=02ZH}

Soit A une algèbre stellaire unifère. Soit U un ouvert relativement compact dans $\mathbf{C}$. Notons $\Omega_n$ l’ensemble des éléments normaux de A tels que Sp$_A(a)$ est contenu dans U. L’application $(f, a)\mapsto f(a)$ de $\mathscr{C}(U)\times \Omega_n$ dans A est continue.

Notons $q$ l’application $(f, a)\mapsto f(a)$ de $\mathscr{C}(U)\times \Omega_n$ dans A. L’ensemble des applications de calcul fonctionnel $f\mapsto f(a)$ pour $a\in \Omega_n$ est équicontinu dans $\mathscr{L}(\mathscr{C}(U); A)$, puisque chacune est une application linéaire continue de norme $\leqslant 1$. Pour démontrer l’assertion, il suffit donc de vérifier que, pour tout $f\in \mathscr{C}$ (U), l’application de $\Omega_n$ dans A définie par $a\mapsto f(a)$ est continue (TG, X, p. 13, cor. 3).

Soit $\mathscr{A}$ l’ensemble des $f\in \mathscr{C}(U)$ telles que l’application $a\mapsto f(a)$ de $\Omega_n$ dans A est continue ; il faut démontrer que $\mathscr{A}=\mathscr{C}(U)$.

L’ensemble $\mathscr{A}$ est une sous-algèbre unifère involutive de $\mathscr{C}(U)$. Elle contient la fonction identique de U, donc elle sépare les points. Par conséquent, elle est dense dans $\mathscr{C}(U)$ (TG, X, p. 39, prop. 7). Démontrons qu’elle est fermée.

Soit $(f_n)$ une suite dans $\mathscr{A}$ qui converge vers $f\in \mathscr{C}(U)$. Soit $\varepsilon  >0$ et choisissons $n\in \mathbf{N}$ tel que $\|f-f_n\|_{\infty}\leqslant \varepsilon /4$. Pour tout $(a_1, a_2)\in \Omega^2_n$ on a

$$
\|f(a_1)-f(a_2)\|\leqslant 2\|f-f_n\|_{\infty}+\|f_n(a_1)-f_n(a_2)\|
$$

$$
\varepsilon
$$

$$
\leqslant +\|f_n(a_1)-f_n(a_2)\|
$$

2

Comme $f_n$ appartient à $\mathscr{A}$, il existe un voisinage V de $a_1$ dans $\Omega_n$ tel que $\|f_n(a_1)-f_n(a_2)\|\leqslant \varepsilon /2$ pour tout $a_2\in$ V. On a donc $\|f(a_1)-f(a_2)\|\leqslant \varepsilon$ pour tout $a_2\in V$. L’application $a\mapsto f(a)$ est donc continue en $a_1$; l’assertion est démontrée.

#### Corollaire 1 {#ts-iv-s2-prop-10-cor-1 .statement tag=02ZI}

Soit A une algèbre stellaire unifère et soit $A_n$ l’ensemble des éléments normaux de A. Munissons l’espace $\mathscr{C}(\mathbf{C})$ de la topologie de la convergence compacte. L’application $(f, a)\mapsto f(a)$ de $\mathscr{C}(\mathbf{C})\times A_n$ dans A est continue.

Soit $(f_0, a_0)\in \mathscr{C}(\mathbf{C})\times A_n$. Soit U un voisinage relativement compact du spectre de $a_0$. Soit V l’ensemble des éléments normaux $a$ de A tels que Sp$_A(a)\subset U$; c’est un voisinage ouvert de $a_0$ dans $A_n$ (I, p. 76, prop. 10). Pour tout $a\in V$ et toute fonction $f\in \mathscr{C}(\mathbf{C})$, on a $f(a) = (f|U)(a)$. Comme l’application $f\mapsto  \|f|U\|_{\infty}$ est une semi-norme continue sur $\mathscr{C}(\mathbf{C})$ muni de la topologie de la convergence compacte, la continuité de l’application $(f, a)\mapsto f(a)$ en $(f_0, a_0)$ résulte de la prop. 10.

#### Corollaire 2 {#ts-iv-s2-prop-10-cor-2 .statement tag=02ZJ}

Soit E un espace hilbertien complexe et soit $\mathscr{L}(E)_n$ l’ensemble des endomorphismes normaux de E. Munissons l’espace $\mathscr{C}(\mathbf{C})$ de la topologie de la convergence compacte. L’application de $\mathscr{C}(\mathbf{C})\times \mathscr{L}(E)_n$ dans $\mathscr{L}(E)$ définie par $(f, u)\mapsto f(u)$ est continue.

## EXERCICES {#ts-iv-s2-exercises}

Sauf mention du contraire, dans les exercices de ce paragraphe, E désigne un espace hilbertien complexe.

See the [exercises for § 2](exercises/s2/).
