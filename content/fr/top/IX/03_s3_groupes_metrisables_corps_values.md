---
book: top
book_title: General Topology
chapter: IX
chapter_title: UTILISATION DES NOMBRES RÉELS EN TOPOLOGIE GÉNÉRALE
section: 3
section_title: Groupes métrisables ; corps valués ; espaces et algèbres normés
lang: fr
source: top-v-x-fr
book_pages: TG IX.23-TG IX.41, TG IX.99-TG IX.101
pdf_pages: 0143-0161, 0219-0221
extraction: ocr
subsections:
    - "no": 1
      title: Groupes topologiques métrisables
      page: 23
      pdf_page: 143
    - "no": 2
      title: Corps valués
      page: 28
      pdf_page: 148
    - "no": 3
      title: Espaces normés sur un corps valué
      page: 31
      pdf_page: 151
    - "no": 4
      title: Espaces quotients et espaces produits d’espaces normés
      page: 34
      pdf_page: 154
    - "no": 5
      title: Fonctions multilinéaires continues
      page: 35
      pdf_page: 155
    - "no": 6
      title: Familles absolument sommables dans un espace normé
      page: 36
      pdf_page: 156
    - "no": 7
      title: Algèbres normées sur un corps valué
      page: 37
      pdf_page: 157
statements: 49
exercises: 13
content_sha256: 0c2545a1d4e317e78a476a40c85d16bd6b75ce5f22c7788ca310ca01fca0b6dd
---

## § 3. GROUPES MÉTRISABLES; CORPS VALUÉS; ESPACES ET ALGÈBRES NORMÉS

### 1. Groupes topologiques métrisables

#### Proposition 1 {#top-ix-s3-prop-1 .statement}

*Pour que les structures uniformes droite et gauche d’un groupe topologique G soient métrisables, il faut et il suffit que G soit séparé et que l’élément neutre e de G possède un système fondamental dénombrable de voisinages.*

La condition est évidemment nécessaire. Réciproquement, si elle est remplie, soit $(V_n)$ un système fondamental de voisinages de $e$; si $U_n$ désigne l’ensemble des couples $(x, y)$ de $G \times G$ tels que $x^{-1}y \in V_n$, les $U_n$ forment un système fondamental dénombrable d’entourages de la structure uniforme gauche de $G$; comme en outre cette structure est séparée, elle est métrisable (IX, p. 15, th. 1). Même démonstration pour la structure uniforme droite de $G$.

Nous dirons qu’un groupe topologique $G$ est métrisable si sa topologie est métrisable; la prop. 1 montre alors que ses deux structures uniformes sont métrisables.

On peut préciser ce résultat à l’aide de la notion suivante:

#### Définition 1 {#top-ix-s3-def-1 .statement}

Sur un groupe $G$, noté multiplicativement, on dit qu’une distance $d$ est invariante à gauche (resp. invariante à droite) si, quels que soient $x, y, z$ dans $G$, on a $d(zx, zy) = d(x, y)$ (resp. $d(xz, yz) = d(x, y)$).

#### Proposition 2 {#top-ix-s3-prop-2 .statement}

La structure uniforme gauche (resp. droite) d’un groupe métrisable $G$ peut être définie par une distance invariante à gauche (resp. à droite).

Supposons en effet que le système fondamental $(V_n)$ de voisinages de $e$ soit formé de voisinages symétriques tels que $V_{n+1}^3 \subset V_n$ pour tout $n$; les entourages $U_n$ correspondants de la structure uniforme gauche sont alors des entourages symétriques tels que $U_{n+1}^3 \subset U_n$. Le procédé employé dans la démonstration de la prop. 2 de IX, p. 6 fournit à partir de la suite d’entourages $(U_n)$ une distance $d$ sur $G$ compatible avec la structure uniforme gauche de $G$; en outre, comme pour tout $z \in G$, l’application $(x, y) \mapsto (zx, zy)$ laisse invariant chacun des $U_n$, la définition même de $d$ montre que $d$ est une distance invariante à gauche. Raisonnement analogue pour la structure uniforme droite.

On notera que, si les deux structures uniformes de $G$ sont distinctes, la distance $d$ n’est pas invariante à droite, et par suite on a en général $d(x^{-1}, y^{-1}) \neq d(x, y)$.

En particulier, si $G$ est un groupe commutatif métrisable, sa structure uniforme est définie par une distance invariante $d$; si $G$ est noté additivement, on a $d(x, y) = d(0, y - x) = d(0, x - y)$; on pose souvent $d(0, x) = |x|$ (ou $d(0, x) = \|x\|$); on a donc $d(x, y) = |x - y|$. La fonction $|x|$ satisfait aux trois conditions suivantes:

a) $|-x| = |x|$ pour tout $x \in G$;
b) $|x + y| \leq |x| + |y|$ quels que soient $x, y$ dans $G$;
c) La relation $|x| = 0$ est équivalente à $x = 0$.

Réciproquement:

#### Proposition 3 {#top-ix-s3-prop-3 .statement}

Soient $G$ un groupe commutatif noté additivement, $x \mapsto |x|$ une application de $G$ dans $\mathbf{R}_+$ satisfaisant aux conditions a), b), c) précédentes. La fonction $d(x, y) = |x - y|$ est une distance invariante sur $G$; la topologie $\mathcal{T}$ qu’elle définit sur $G$ est compatible avec la structure de groupe de $G$, et la structure uniforme qu’elle définit est identique à la structure uniforme du groupe topologique obtenu en munissant $G$ de la topologie $\mathcal{T}$.

La fonction $d(x, y)$ est bien une distance sur $G$, car la relation $d(x, y) = 0$ équivant à $x = y$ d’après c), on a $d(y, x) = d(x, y)$ d’après a), et
$$
d(x, y) = |(x - z) + (z - y)| \leq |x - z| + |z - y| = d(x, z) + d(z, y)
$$
d’après b). En outre, $d$ est une distance invariante puisque
$$
(x + z) - (y + z) = x - y.
$$
Pour tout $\alpha > 0$, soit $V_\alpha$ l’ensemble des $x \in G$ tels que $|x| < \alpha$; les $V_\alpha$ forment un système fondamental $\mathcal{S}$ de voisinages de 0 pour la topologie $\mathcal{T}$, et comme $d$ est invariante, pour tout $a \in G$, $a + \mathcal{S}$ est un système fondamental de voisinages de $a$ pour la topologie $\mathcal{T}$. D’après a), les $V_\alpha$ sont symétriques, et d’après b), on a $V_\alpha + V_\alpha \subset V_{2\alpha}$; la topologie $\mathcal{T}$ est donc compatible avec la structure de groupe de $G$ (III, p. 4). La dernière partie de la proposition est immédiate.

Les conditions $a), b), c)$ sont équivalentes à la condition c) jointe à la condition
$$
b') \qquad |x - y| \leq |x| + |y|.
$$
En effet, il est évident que a) et b) entraînent $b')$. Réciproquement, en prenant $x = 0$ dans $b')$, et tenant compte de c), on voit que $|-y| \leq |y|$, d’où en remplaçant $y$ par $-y$, $|-y| = |y|$, ce qui donne a); en remplaçant $y$ par $-y$ dans $b')$, on obtient alors b).

#### Proposition 4 {#top-ix-s3-prop-4 .statement}

*Si $G$ est un groupe métrisable, tout groupe quotient séparé $G/H$ de $G$ est métrisable; si en outre $G$ est complet, $G/H$ est complet.*¹

La première partie de la proposition résulte de ce que, dans $G/H$, l’élément neutre admet un système fondamental dénombrable de voisinages: en effet, si $(V_n)$ est un système fondamental de voisinages de $e$ dans $G$, les images canoniques $\dot{V}_n$ des ensembles $V_n$ dans $G/H$ forment un système fondamental de voisinages de l’élément neutre de $G/H$ (III, p. 13, prop. 17).

Pour montrer que, si $G$ est complet, il en est de même de $G/H$, il suffit (IX, p. 17, prop. 9) de voir que toute suite de Cauchy $(\dot{x}_n)$ pour la structure uniforme gauche de $G/H$, est convergente; on peut toujours supposer (en extrayant au besoin une suite partielle de $(\dot{x}_n)$) que, pour tout couple d’indices $p, q$ tels que $p \geq n, q \geq n$, on a $\dot{x}_p^{-1}\dot{x}_q \in \dot{V}_n$; cela signifie que, pour tout couple de points $y \in \dot{x}_p, z \in \dot{x}_q$, on a $y^{-1}z \in HV_n = V_nH$; il en résulte que, pour tout $y \in \dot{x}_p$, l’intersection de $\dot{x}_q$ et du voisinage $yV_n$ de $y$ n’est pas vide. Supposons alors la suite $(V_n)$ choisie de sorte que $V_{n+1}^2 \subset V_n$, et définissons par récurrence une suite $(x_n)$ de points de $G$, de sorte que $x_n \in \dot{x}_n$ et $x_{n+1} \in x_n V_n$, ce qui est possible d’après ce qui précède; on en conclut par récurrence que pour tout $p > 0$, on a
$$
x_{n+p} \in x_n V_n V_{n+1} \cdots V_{n+p-1} \subset x_n V_{n-1}.
$$
La suite $(x_n)$ est donc une suite de Cauchy dans $G$ et converge par suite vers un

¹ Il existe des groupes complets non métrisables $G$, contenant un sous-groupe fermé $H$ tel que $G/H$ ne soit pas complet (EVT, IV, § 4, exerc. 10 c).

point $a$; on en conclut aussitôt que l’image canonique $\hat{a}$ de $a$ dans $G/H$ est limite de la suite $(\hat{x}_n)$.

#### Corollaire {#top-ix-s3-n1-cor-1 .statement}

Soient $G$ un groupe métrisable complet, $G_0$ un sous-groupe partout dense dans $G$, $H_0$ un sous-groupe distingué fermé de $G_0$; si $H$ est l’adhérence de $H_0$ dans $G$, le groupe quotient $G_0/H_0$ admet alors un groupe complété isomorphe à $G/H$.

On sait que $H$ est un sous-groupe distingué de $G$ (III, p. 9, prop. 9) et la prop. 4 montre que $G/H$ est complet; si $\varphi$ est l’application canonique de $G$ sur $G/H$, il est clair d’autre part que $\varphi(G_0)$ est partout dense dans $G/H$. Le corollaire résulte donc de la prop. 21 de III, p. 14.

Dans ce qui suit, pour un espace uniforme $X$, nous noterons $i_X$ l’application canonique de $X$ dans son séparé complété $\hat{X}$, par $X_0 = i_X(X)$ le sous-espace uniforme de $\hat{X}$, qui est l’espace séparé associé à $X$; rappelons que la topologie de $X$ est l’image réciproque par $i_X$ de celle de $X_0$ (II, p. 23, prop. 12). Rappelons aussi que, pour toute application uniformément continue $f : X \to Y$, $\hat{f}$ désigne l’application uniformément continue de $\hat{X}$ dans $\hat{Y}$ telle que $\hat{f} \circ i_X = i_Y \circ f$ (II, p. 24, prop. 15); si $X$ est un sous-espace uniforme de $Y$ et $f$ l’injection canonique, $\hat{X}$ s’identifie à un sous-espace uniforme de $\hat{Y}$ et $\hat{f}$ à l’injection canonique de $\hat{X}$ dans $\hat{Y}$ (II, p. 26, cor. 1).

#### Proposition 5 {#top-ix-s3-prop-5 .statement}

Soit $X \xrightarrow{f} Y \xrightarrow{g} Z$ une suite exacte de morphismes stricts (III, p. 16) de groupes topologiques (A, II, p. 10, Remarque 5). Supposons que $X, Y, Z$ admettent des groupes séparés complétés métrisables. Alors $\hat{X} \xrightarrow{\hat{f}} \hat{Y} \xrightarrow{\hat{g}} \hat{Z}$ est une suite exacte de morphismes stricts.

Soient $N_f, N_g$ les noyaux respectifs de $f$ et $g$; écrivons $f = f_3 \circ f_2 \circ f_1$, où $f_1$ est le morphisme strict canonique $X \to X/N_f$, $f_2$ un isomorphisme de $X/N_f$ sur $N_g$ et $f_3$ l’injection canonique $N_g \to Y$. On sait déjà que $f_2$ est un isomorphisme de $\widehat{(X/N_f)}$ sur $\hat{N}_g$, et on vient de rappeler que $\hat{f}_3$ est un morphisme strict injectif de $\hat{N}_g$ dans $\hat{Y}$; si l’on montre que $\hat{f}_1$ est un morphisme strict surjectif de $\hat{X}$ sur $\widehat{(X/N_f)}$, il en résultera que $\hat{f}$ est un morphisme strict (III, p. 16, Remarque 2). D’autre part, soit $g_1$ le morphisme strict canonique $Y \to Y/N_g$; si l’on montre que $\hat{g}_1$ est un morphisme strict surjectif de noyau $\hat{N}_g$ (identifié à un sous-groupe de $\hat{Y}$), on verra comme ci-dessus que $\hat{g}$ est un morphisme strict, et la suite $\hat{X} \xrightarrow{\hat{f}} \hat{Y} \xrightarrow{\hat{g}} \hat{Z}$ sera exacte. On est donc ramené à prouver le lemme suivant:

#### Lemme 1 {#top-ix-s3-lem-1 .statement}

Soient $X$ un groupe topologique admettant un groupe séparé complété métrisable, $N$ un sous-groupe distingué de $X$, $Y = X/N$, $f : X \to Y$ le morphisme canonique. Alors $\hat{f} : \hat{X} \to \hat{Y}$ est un morphisme strict surjectif de noyau identifié canoniquement à $\hat{N}$.

Soit $f_0 : X_0 \to Y_0$ l’application qui coïncide avec $\hat{f}$ dans $X_0$; comme $i_X$ (resp. $i_Y$) est un morphisme strict surjectif de $X$ sur $X_0$ (resp. de $Y$ sur $Y_0$), $f_0$ est un morphisme strict surjectif (III, p. 17, Remarque 3). Or $X_0$ et $Y_0$ sont métrisables

(IX, p. 23, prop. 1); il résulte de IX, p. 26, corollaire, et de III, p. 25, prop. 8, que $\hat{f}_0 = \hat{f}$ est un morphisme strict surjectif et admet comme noyau l’adhérence $\hat{N}_0'$ dans $\hat{X} = \hat{X}_0$ du noyau $N_0'$ de $f_0$. Il nous suffira donc de prouver que $\hat{N}_0' = \hat{N}$. Or, $N_0'$ contient évidemment $N_0 = i_X(N)$; il suffira de voir que $N_0'$ est contenu dans l’adhérence $\overline{N}_0$ de $N_0$ dans $X_0$. Or, $U = i_X^{-1}(X_0 - \overline{N}_0) = X - i_X^{-1}(\overline{N}_0)$ est un ensemble ouvert dans $X$ qui ne rencontre pas $N$; comme $f$ est un morphisme strict surjectif, $V = f(U)$ est un ensemble ouvert dans $Y$ ne contenant pas l’élément neutre $e'$ de $Y$, donc ne rencontrant pas l’adhérence de $e'$; par suite $i_Y(V)$ ne contient pas l’élément neutre de $Y_0$. Mais $i_Y(V) = f_0(X_0 - \overline{N}_0)$ par définition de $U$, donc on a $N_0' \subset \overline{N}_0$, ce qui achève de prouver le lemme 1 et la prop. 5.

La prop. 5 s’applique en particulier lorsque $X, Y$ et $Z$ sont des groupes commutatifs dont les éléments neutres admettent des systèmes fondamentaux dénombrables de voisinages, puisque dans ce cas les séparés complétés existent (III, p. 26, th. 2). En particulier, si $X$ est un tel groupe commutatif, $N$ un sous-groupe quelconque de $X$, le séparé complété $\widehat{(X/N)}$ s’identifie canoniquement à $\hat{X}/\hat{N}$.

#### Corollaire {#top-ix-s3-n1-cor-2 .statement}

*Soient $X, Y$ deux groupes commutatifs métrisables, $u$ un morphisme strict de $X$ dans $Y$, $N$ son noyau, $P$ son image. Alors $\hat{u}$ est un morphisme strict de $\hat{X}$ dans $\hat{Y}$, de noyau $\hat{N} = \overline{N}$ (adhérence de $N$ dans $\hat{X}$) et d’image $\hat{P} = \overline{P}$ (adhérence de $P$ dans $Y$).*

#### Remarque {#top-ix-s3-n1-rem-1 .statement}

Soit $d$ une distance invariante à gauche définissant la topologie d’un groupe métrisable $G$; soit $H$ un sous-groupe distingué fermé de $G$. Pour deux points quelconques $\dot{x}, \dot{y}$ de $G/H$, considérons la distance $d(\dot{x}, \dot{y})$ des deux ensembles fermés $\dot{x}, \dot{y}$ dans $G$ (IX, p. 13); nous allons voir que cette fonction est une *distance invariante à gauche* sur $G/H$, définissant la topologie de ce groupe quotient. Notons d’abord que si $x \in \dot{x}, y \in \dot{y}$, on a $d(\dot{x}, \dot{y}) = d(x, Hy)$; en effet
$$
d(x, Hy) = \inf_{h \in H} d(x, hy),
$$
d’où aussitôt, pour tout $h' \in H$, $d(h'x, Hy) = d(x, Hy)$ en vertu de l’invariance à gauche de $d$, ce qui démontre notre assertion (IX, p. 13); pour tout point $\dot{z} \in G/H$, on a donc (IX, p. 13, formule (2))
$$
|d(\dot{x}, \dot{z}) - d(\dot{y}, \dot{z})| = |d(x, \dot{z}) - d(y, \dot{z})| \leq d(x, y),
$$
et comme cette inégalité est vraie quels que soient $x \in \dot{x}$ et $y \in \dot{y}$, on a $|d(\dot{x}, \dot{z}) - d(\dot{y}, \dot{z})| \leq d(\dot{x}, \dot{y})$, ce qui prouve que $d(\dot{x}, \dot{y})$ est une distance sur $G/H$. En outre, pour tout $z \in \dot{z}$, on a $d(\dot{zx}, \dot{zy}) = \inf_{h \in H} d(zx, hzy)$ d’après ce qui précède; mais comme $hzy = z(z^{-1}hz)y$ et que $z^{-1}hz$ parcourt $H$ lorsque $h$ parcourt $H$ ($H$ étant distingué), l’invariance à gauche de $d(x, y)$ prouve que l’on a $d(zx, Hzzy) = d(x, Hy) = d(\dot{x}, \dot{y})$. Enfin, si $V$ est un voisinage de $e$ dans $G$ défini par $d(e, x) < \alpha$, son image $\dot{V}$ dans $G/H$ est l’ensemble défini par $d(\dot{e}, \dot{x}) < \alpha$, ce qui achève de démontrer notre assertion.

### 2. Corps valués

#### Définition 2 {#top-ix-s3-def-2 .statement}

On appelle valeur absolue sur un corps $K$ une application $x \mapsto |x|$ de $K$ dans $\mathbf{R}_+$, satisfaisant aux conditions suivantes :

$$
\begin{align*}
(\mathrm{VM}_I) &\quad |x| = 0 \text{ est équivalent à } x = 0; \\
(\mathrm{VM}_{II}) &\quad |xy| = |x| \cdot |y| \text{ quels que soient } x, y \text{ dans } K; \\
(\mathrm{VM}_{III}) &\quad |x + y| \leq |x| + |y| \text{ quels que soient } x, y \text{ dans } K.
\end{align*}
$$

D’après $(\mathrm{VM}_{II})$, on a $|x| = |1| \cdot |x|$, et comme il existe d’après $(\mathrm{VM}_I)$ au moins un $x$ tel que $|x| \neq 0$, on a $|1| = 1$; on en tire $1 = |-1|^2$, d’où également $|-1| = 1$, et par suite

$$
|-x| = |-1| \cdot |x| = |x|;
$$

on en conclut que $|x - y| \leq |x| + |y|$ quels que soient $x, y$. On peut encore dire que $d(x, y) = |x - y|$ est une distance invariante sur le groupe additif $K$, et l’application $x \mapsto |x|$ un homomorphisme du groupe multiplicatif $K^*$ des éléments $\neq 0$ de $K$, dans le groupe multiplicatif $\mathbf{R}_+^*$ des nombres réels $> 0$.

La distance invariante $|x - y|$ définit sur $K$ une topologie d’espace métrique compatible avec la structure de groupe additif de $K$ (IX, p. 24, prop. 3); mais en outre, cette topologie est compatible avec la structure de corps de $K$. En effet, la continuité de $xy$ dans $K \times K$ résulte de la relation

$$
xy - x_0 y_0 = (x - x_0)(y - y_0) + (x - x_0)y_0 + x_0(y - y_0)
$$

qui donne

$$
|xy - x_0 y_0| \leq |x - x_0| \cdot |y - y_0| + |x_0| \cdot |y - y_0| + |y_0| \cdot |x - x_0|.
$$

De même, la continuité de $x^{-1}$ en tout point $x_0 \neq 0$ résulte de l’identité $x^{-1} - x_0^{-1} = x^{-1}(x_0 - x)x_0^{-1}$, qui donne, d’après $(\mathrm{VM}_{II})$,

$$
|x^{-1} - x_0^{-1}| = \frac{|x - x_0|}{|x_0| \cdot |x|}.
$$

Or, si $\varepsilon > 0$ est tel que $\varepsilon < |x_0|$, la relation $|x - x_0| \leq \varepsilon$ entraîne $|x| \geq |x_0| - \varepsilon$, d’où

$$
|x^{-1} - x_0^{-1}| \leq \frac{\varepsilon}{|x_0|(|x_0| - \varepsilon)},
$$

ce qui établit la continuité de $x^{-1}$ au point $x_0$.

#### Définition 3 {#top-ix-s3-def-3 .statement}

On appelle corps valué un corps $K$ muni de la structure définie par la donnée d’une valeur absolue sur $K$.

Un corps valué sera toujours considéré comme muni de la topologie définie par sa valeur absolue, qui en fait un corps *topologique*. Si $K_0$ est un sous-corps d’un corps valué $K$, la restriction à $K_0$ de la valeur absolue sur $K$ est une valeur absolue sur $K_0$, qui définit sur $K_0$ la topologie induite par celle de $K$.

#### Exemple 1 {#top-ix-s3-n2-exa-1 .statement}

Soit $K$ un corps quelconque; pour tout $x \in K$, posons $|x| = 1$ si $x \neq 0$, et $|0| = 0$; l’application $x \mapsto |x|$ ainsi définie est une valeur absolue sur $K$, dite valeur absolue *impropre*. Pour que la topologie définie sur un corps $K$ par une valeur absolue $|x|$ soit *discrète*, il faut et il suffit que $|x|$ soit la valeur impropre. C’est évidemment suffisant; inversement, si la topologie de $K$ est discrète, $|x|$ ne peut prendre aucune valeur $\alpha > 0$ distincte de 1: car si on avait $|x_0| = \alpha < 1$, la suite $(x_0^n)$ serait formée de termes $\neq 0$ et convergerait vers 0; on passe de là au cas $\alpha > 1$ en considérant $x_0^{-1}$.

#### Exemple 2 {#top-ix-s3-n2-exa-2 .statement}

La valeur absolue d’un nombre réel (IV, p. 5) vérifie les axiomes (VM$_1$), (VM$_2$), (VM$_3$) et définit sur le corps $\mathbf{R}$ la topologie de la droite numérique. Sur le corps $\mathbf{C}$ des nombres complexes (identifié à $\mathbf{R}^2$) et sur le corps $\mathbf{K}$ des quaternions (identifié à $\mathbf{R}^4$) la norme euclidienne est de même une valeur absolue définissant respectivement la topologie de chacun de ces corps (VIII, p. 4 et p. 7).

#### Exemple 3 {#top-ix-s3-n2-exa-3 .statement}

Sur un corps $K$, une *valuation réelle* est une fonction $v$, définie dans $K^*$, à valeurs dans $\mathbf{R}$, satisfaisant aux conditions suivantes: *a)* pour $x \in K^*,\ y \in K^*$, $v(xy) = v(x) + v(y)$; *b)* si en outre $x + y \neq 0$, $v(x + y) \geq \inf(v(x), v(y))$. Si $a$ est un nombre réel quelconque $> 1$, on définit alors sur $K$ une *valeur absolue* en posant $|x| = a^{-v(x)}$ pour $x \neq 0$, et $|0| = 0$. En effet, de la relation $v(xy) = v(x) + v(y)$ pour $x \neq 0$ et $y \neq 0$, on déduit la relation $|xy| = |x| \cdot |y|$ pour ces valeurs de $x$ et $y$, et cette relation est trivialement vérifiée si l’un des éléments $x,\ y$ est nul; de même, de $v(x + y) \geq \inf(v(x), v(y))$ pour $x \neq 0,\ y \neq 0$ et $x + y \neq 0$, on déduit

$$
|x + y| \leq \sup(|x|, |y|) \leq |x| + |y|,
$$

et ces inégalités sont encore vérifiées si l’un des éléments $x,\ y,\ x + y$ est nul. En particulier, si $v_p(x)$ est la valuation *p*-adique sur le corps $\mathbf{Q}$ des nombres rationnels (exposant de $p$ dans la décomposition de $x$ en produit de facteurs premiers), la valeur absolue correspondante $|x|_p = p^{-v_p(x)}$ est dite *valeur absolue p-adique* sur le corps $\mathbf{Q}$.

#### Remarque {#top-ix-s3-n2-rem-1 .statement}

Si, dans un corps valué, $x$ est racine de l’unité, on a $|x| = 1$, car si $x^n = 1$ pour un entier $n > 0$, on en tire $|x|^n = 1$ d’où $|x| = 1$. En particulier, la seule valeur absolue sur un corps *fini* est la valeur absolue *impropre*, puisque tout élément $\neq 0$ du corps est racine de l’unité.

On dit qu’une valeur absolue sur un corps $K$ est *ultramétrique* si elle vérifie l’inégalité $|x + y| \leq \sup(|x|, |y|)$; le corps valué $K$ est alors dit *ultramétrique*; la valeur absolue impropre sur tout corps $K$, et la valeur absolue *p*-adique sur $\mathbf{Q}$ sont ultramétriques, mais il n’en est pas de même de la valeur absolue usuelle sur $\mathbf{R}$ ou sur $\mathbf{C}$.

#### Définition 4 {#top-ix-s3-def-4 .statement}

*On dit que deux valeurs absolues sur un corps $K$ sont équivalentes si elles définissent la même topologie sur $K$.*

La condition de l’énoncé est nécessaire, car l’ensemble des $x \in K$ tels que $|x|_1 < 1$ est identique à l’ensemble des $x$ tels que $\lim_{n \to \infty} x^n = 0$ pour la topologie définie par la valeur absolue $|x|_1$.

Supposons inversement que $|x|_1 < 1$ entraîne $|x|_2 < 1$. Alors $|x|_1 > 1$ entraîne $|x|_2 > 1$, puisqu’on a $|x^{-1}|_1 < 1$, et par suite $|x^{-1}|_2 < 1$. Comme par hypothèse la valeur absolue $|x|_1$ n’est pas impropre, il existe un $x_0 \in K$ tel que $|x_0|_1 > 1$; posons $a = |x_0|_1, \ b = |x_0|_2, \ \rho = \log b / \log a > 0$. Soit $x \in K^*$, et posons $|x|_1 = |x_0|^{\gamma}$. Si $m$ et $n$ sont des entiers tels que $n > 0$ et $m/n > \gamma$, on a $|x|_1 < |x_0|_1^{m/n}$, d’où $|x^n/x_0^m|_1 < 1$, et par suite $|x^n/x_0^m|_2 < 1$, $|x|_2 < |x_0|_2^{m/n}$. De même, si $m/n < \gamma$, on voit que $|x|_2 > |x_0|_2^{m/n}$. On en conclut $|x|_2 = |x_0|^{\gamma}$, autrement dit $\log|x|_2 = \gamma \log b = \gamma \rho \log a = \rho \log|x|_1$, ou $|x|_2 = |x|_1^{\rho}$; il est immédiat que les voisinages de 0 pour les topologies définies par $|x|_1$ et $|x|_2$ sur $K$ sont alors identiques.

Inversement, pour toute valeur absolue $|x|$ sur $K$, la fonction $|x|^{\rho}$ est une valeur absolue sur $K$ (équivalente à $|x|$) pour tout nombre $\rho$ tel que $0 < \rho \leq 1$. En effet, il suffit de vérifier l’inégalité $|x + y|^{\rho} \leq |x|^{\rho} + |y|^{\rho}$; or, on a $|x + y|^{\rho} \leq (|x| + |y|)^{\rho}$; tout revient donc à montrer que, si $a > 0, b > 0$, on a $(a + b)^{\rho} \leq a^{\rho} + b^{\rho}$ pour $0 < \rho \leq 1$. Or, si on pose $c = a/(a + b), d = b/(a + b)$, on a $c + d = 1$ et l’inégalité à démontrer s’écrit $1 \leq c^{\rho} + d^{\rho}$; elle résulte immédiatement des relations $c^{\rho} \geq c, d^{\rho} \geq d$ qui sont évidentes puisque $0 < c \leq 1, 0 < d \leq 1$ et $0 < \rho \leq 1$.

On en conclut que l’ensemble des valeurs de $r > 0$ telles que $|x|^r$ soit une valeur absolue est un intervalle fini ou infini d’origine 0 dans $\mathbf{R}$; s’il est fini, il est évidemment fermé, car si, pour deux éléments quelconques $x, y$ de $K$, on a $|x + y|^r \leq |x|^r + |y|^r$ pour $0 < r < r_0$, l’inégalité a encore lieu par continuité pour $r = r_0$. Lorsque $|x|^r$ est une valeur absolue pour tout nombre $r > 0$, on a, pour deux éléments quelconques $x, y$ de $K$

$$
|x + y| \leq (|x|^r + |y|^r)^{1/r}
$$

pour tout $r > 0$. Or, si $a$ et $b$ sont deux nombres $\geq 0$, on a $\lim_{r \to \infty} (a^r + b^r)^{1/r} = \sup(a, b)$, car, en supposant par exemple $b \leq a$, on a

$$
a \leq (a^r + b^r)^{1/r} \leq 2^{1/r} a
$$

d’où la formule cherchée, en faisant croître $r$ indéfiniment.

On voit donc que, si $|x|^r$ est une valeur absolue pour tout $r > 0$, on a

$$
|x + y| \leq \sup(|x|, |y|)
$$

autrement dit la valeur absolue $|x|$ est ultramétrique.

#### Remarque {#top-ix-s3-n2-rem-2 .statement}

La démonstration de la prop. 6 (IX, p. 29) prouve que, si la topologie définie sur $K$ par $|x|_2$ est moins fine que celle définie par $|x|_1$, et si $|x|_1$ n’est pas impropre, $|x|_1$ et $|x|_2$ sont équivalentes, car la relation $|x|_1 < 1$ entraîne alors $|x|_2 < 1$. Autrement dit, les topologies définies sur $K$ par deux valeurs absolues non impures ne peuvent être comparables que si elles sont identiques.

#### Proposition 7 {#top-ix-s3-prop-7 .statement}

L’anneau complété $\hat{K}$ d’un corps $K$ valué par une valeur absolue $|x|$ est un corps, et la fonction $|x|$ se prolonge par continuité en une valeur absolue sur $\hat{K}$, qui définit la topologie de $\hat{K}$.

Soit $\mathfrak{F}$ un filtre de Cauchy sur $K$ (pour la structure uniforme additive) tel que 0 ne soit pas adhérent à $\mathfrak{F}$; pour voir que $\hat{K}$ est un corps, il suffit d’établir que l’image de $\mathfrak{F}$ par l’application $x \mapsto x^{-1}$ est une base de filtre de Cauchy (III, p. 56, prop. 7). Or, il existe par hypothèse un nombre $\alpha > 0$ et un ensemble $A \in \mathfrak{F}$ tels que $|x| \geq \alpha$ pour tout $x \in A$; d’autre part, pour tout $\varepsilon > 0$, il existe un ensemble $B \in \mathfrak{F}$ tel que $B \subset A$ et, pour tout couple d’éléments $x, y$ de $B$, $|x - y| \leq \varepsilon$; on en conclut

$$
|x^{-1} - y^{-1}| = \frac{|x - y|}{|x| \cdot |y|} \leq \frac{\varepsilon}{\alpha^2},
$$

d’où la première partie de la proposition. La distance invariante $|x - y| = d(x, y)$ se prolonge par continuité à $\hat{K} \times \hat{K}$, en une distance sur $\hat{K}$ (IX, p. 12, prop. 1) qui définit la topologie de $\hat{K}$ et est invariante en vertu du principe de prolongement des identités; nous la désignerons encore par $d(x, y)$. Si on pose $|x| = d(0, x)$ pour $x \in \hat{K}$, il est clair que $|x|$ est le prolongement par continuité de la fonction $|x|$ sur $K$, et est donc une valeur absolue sur $\hat{K}$ d’après le principe de prolongement des identités.

### 3. Espaces normés sur un corps valué

#### Définition 5 {#top-ix-s3-def-5 .statement}

Étant donné un espace vectoriel $E$ (à gauche par exemple) sur un corps valué non discret $K$, on appelle norme sur $E$ une application $x \mapsto p(x)$ de $E$ dans $\mathbf{R}_+$, satisfaisant aux axiomes suivants:

(NO_I) $p(x) = 0$ est équivalente à $x = 0$;
(NO_{II}) $p(x + y) \leq p(x) + p(y)$ quels que soient $x$ et $y$ dans $E$;
(NO_{III}) $p(t x) = |t| p(x)$ quels que soient $t \in K$ et $x \in E$.

Les espaces normés que l’on rencontre le plus souvent ont pour corps des scalaires l’un des corps $\mathbf{R}$ ou $\mathbf{C}$ (muni de la valeur absolue usuelle). Nous étudierons les propriétés particulières à ces espaces normés dans le livre consacré aux espaces vectoriels topologiques.

De (NO_{III}) on déduit en particulier que $p(-x) = p(x)$; par suite, si on pose $d(x, y) = p(x - y)$, $d$ est une distance invariante sur le groupe additif $E$, et définit sur $E$ une topologie d’espace métrique compatible avec la structure de groupe additif de $E$ (IX, p. 24, prop. 3); en outre, l’application $(t, x) \mapsto t x$ est continue dans $K \times E$; en effet, on a

$$
t x - t_0 x_0 = (t - t_0)(x - x_0) + (t - t_0)x_0 + t_0(x - x_0)
$$

et par suite

$$
p(t x - t_0 x_0) \leq |t - t_0| p(x - x_0) + |t - t_0| p(x_0) + |t_0| p(x - x_0)
$$

ce qui montre que le premier membre peut être rendu aussi petit qu’on veut en prenant $|t - t_0|$ et $p(x - x_0)$ assez petits.

#### Définition 6 {#top-ix-s3-def-6 .statement}

On appelle espace normé sur un corps valué non discret K un espace vectoriel E sur le corps K, muni de la structure définie par la donnée d’une norme sur E.

Un espace normé sera toujours considéré comme muni de la topologie et de la structure uniforme définies par sa norme.

On appelle espace normable sur K un espace vectoriel sur K, muni d’une topologie qui peut être définie par une norme.

#### Exemple 1 {#top-ix-s3-n3-exa-1 .statement}

Sur un corps valué non discret K, considéré comme espace vectoriel (à gauche ou à droite) par rapport à lui-même, la valeur absolue $|x|$ est une norme.

#### Exemple 2 {#top-ix-s3-n3-exa-2 .statement}

L’expression $\| \mathbf{x} \| = \sqrt{\sum_{i=1}^{n} x_i^2}$, que nous avons appelée norme euclidienne sur l’espace $\mathbf{R}^n$ (VI, p. 7) est évidemment une norme au sens de la déf. 5 (IX, p. 31).

Il en est de même des fonctions $\sup_{1 \leq i \leq n} |x_i|$ et $\sum_{i=1}^{n} |x_i|$.

#### Exemple 3 {#top-ix-s3-n3-exa-3 .statement}

Soit $\mathscr{B}(E)$ l’ensemble des fonctions $f$ définies dans un ensemble E, prenant leurs valeurs dans un corps valué non discret K, et telles que la fonction numérique $x \mapsto |f(x)|$ soit bornée dans E. Cet ensemble est évidemment un sous-espace vectoriel de l’espace vectoriel $K^E$ (à droite ou à gauche) des applications de E dans K. Si on pose $p(f) = \sup_{x \in E} |f(x)|$, $p$ est une norme sur l’espace vectoriel $\mathscr{B}(E)$ (cf. X, p. 20).

#### Exemple 4 {#top-ix-s3-n3-exa-4 .statement}

Sur l’espace vectoriel $\mathscr{C}(I)$ des fonctions continues numériques (finies) définies dans l’intervalle $I = [0, 1]$, la fonction $p(x) = \int_0^1 |x(t)|\ dt$ est une norme.*

#### Exemple 5 {#top-ix-s3-n3-exa-5 .statement}

Lorsque K est un corps valué non discret ultramétrique (IX, p. 29), on appelle ultranorme sur un espace vectoriel E sur K, une norme sur E vérifiant l’inégalité (qui entraîne (NOII)):

$$
p(\mathbf{x} + \mathbf{y}) \leq \sup(p(\mathbf{x}), p(\mathbf{y})).
$$

Les normes qu’on rencontre dans les applications (lorsque K est ultramétrique) sont des ultranormes.

Nous dirons que, dans un espace normé E, la boule B (fermée) de centre 0 et de rayon 1, c’est-à-dire l’ensemble des $\mathbf{x} \in E$ tels que $p(\mathbf{x}) \leq 1$, est la boule unité de E. Montrons qu’un système fondamental de voisinages de 0 dans E est formé par les transformées de la boule unité par les homothéties $\mathbf{x} \mapsto t \mathbf{x}$, où $t$ parcourt l’ensemble des éléments $\neq 0$ de K. En effet, l’image de B par cette homothétie est la boule fermée de centre 0 et de rayon $|t|$; il suffit donc de montrer que pour tout nombre réel $r > 0$, il existe $t \in K$ tel que $0 < |t| < r$. Or, comme la valeur absolue de K n’est pas impropre, il existe $t_0 \in K$ tel que $0 < |t_0| < 1$; il suffit de prendre $t = t_0^n$, avec $n$ entier assez grand, pour que $|t| = |t_0|^n < r$.

#### Définition 7 {#top-ix-s3-def-7 .statement}

On dit que deux normes sur un espace vectoriel E (sur un corps valué non discret K) sont équivalentes si elles définissent la même topologie sur E.

#### Proposition 8 {#top-ix-s3-prop-8 .statement}

Pour que deux normes $p, q$ sur un espace vectoriel E soient équivalentes, il faut et il suffit qu’il existe deux nombres $a > 0, b > 0$ tels que, pour tout $\mathbf{x} \in E$, on ait

(1)
$$
a \cdot p(\mathbf{x}) \leq q(\mathbf{x}) \leq b \cdot p(\mathbf{x}).
$$

Ces inégalités sont en effet suffisantes, car de la relation $a.p(\mathbf{x}) \leq q(\mathbf{x})$, on déduit que pour tout $r > 0$, la boule fermée de centre 0 et de rayon $ar$, relative à la norme $q$, est contenue dans la boule fermée de centre 0 et de rayon $r$, relative à la norme $p$; donc la topologie définie par $q$ est plus fine que la topologie définie par $p$; l’inégalité $q(\mathbf{x}) \leq b.p(\mathbf{x})$ montre de même que la topologie définie par $p$ est plus fine que celle définie par $q$, donc les deux topologies sont identiques.

Montrons maintenant que les inégalités (1) sont nécessaires. Si la topologie définie par $q$ est plus fine que la topologie définie par $p$, la boule unité pour la norme $p$ contient une boule fermée de centre 0 et de rayon $\alpha > 0$ pour la norme $q$; autrement dit, la relation $q(\mathbf{x}) \leq \alpha$ entraîne $p(\mathbf{x}) \leq 1$. Si $t_0 \in \mathbf{K}$ est tel que $0 < |t_0| < 1$, pour tout $\mathbf{x} \neq 0$ dans $E$, il existe un entier rationnel $k$ et un seul tel que $\alpha |t_0| < q(t_0^k \mathbf{x}) \leq \alpha$; on a donc $p(t_0^k \mathbf{x}) \leq 1$, d’où

$$
p(\mathbf{x}) \leq \frac{1}{|t_0|^k} \leq \frac{1}{\alpha |t_0|} q(\mathbf{x});
$$

en posant $a = \alpha |t_0|$ on a bien $a.p(\mathbf{x}) \leq q(\mathbf{x})$ pour tout $\mathbf{x} \neq 0$, et la relation est encore vraie pour $\mathbf{x} = 0$. On voit de même que si la topologie définie par $p$ est plus fine que celle définie par $q$, il existe $b > 0$ tel que $q(\mathbf{x}) \leq b.p(\mathbf{x})$.

#### Exemple {#top-ix-s3-n3-exa-6 .statement}

Dans l’espace $\mathbf{R}^n$, les trois normes $\sqrt{\sum_{i=1}^n x_i^2}$, $\sup_{1 \leq i \leq n} |x_i|$ et $\sum_{i=1}^n |x_i|$ sont équivalentes, car on a

$$
\sup_{1 \leq i \leq n} |x_i| \leq \sqrt{\sum_{i=1}^n x_i^2} \leq \sum_{i=1}^n |x_i| \leq n \cdot \sup_{1 \leq i \leq n} |x_i|.
$$

On notera que pour deux normes équivalentes sur $E$, les ensembles bornés sont les mêmes.

#### Proposition 9 {#top-ix-s3-prop-9 .statement}

*Soient $E$ un espace normé sur un corps valué non discret $K$, $p$ la norme sur $E$, $\hat{E}$ le groupe topologique additif complété du groupe additif $E$. La fonction $(t, \mathbf{x}) \mapsto t \mathbf{x}$ se prolonge par continuité à $\hat{K} \times \hat{E}$, et définit sur $\hat{E}$ une structure d’espace vectoriel par rapport à $\hat{K}$; la norme $p$ se prolonge par continuité à $\hat{E}$ en une norme $\bar{p}$ qui définit la topologie de $\hat{E}$.*

Le prolongement par continuité de $t \mathbf{x}$ est un cas particulier du théorème de prolongement d’une application bilinéaire continue d’un produit $E \times F$ de deux groupes commutatifs dans un troisième $G$ (III, p. 50, th. 1); on a $1.\mathbf{x} = \mathbf{x}$ et $t(u \mathbf{x}) = (tu)\mathbf{x}$ pour $t \in \hat{K}$, $u \in \hat{K}$ et $\mathbf{x} \in \hat{E}$, d’après le principe de prolongement des identités; donc la loi externe $(t, \mathbf{x}) \mapsto t \mathbf{x}$ définit bien sur $\hat{E}$ une structure d’espace vectoriel par rapport à $\hat{K}$. D’autre part, la distance invariante $d(\mathbf{x}, \mathbf{y}) = p(\mathbf{x} - \mathbf{y})$ se prolonge à $\hat{E} \times \hat{E}$ en une distance invariante $\bar{d}$ sur $\hat{E}$ (IX, p. 12, prop. 1), qui définit la topologie de $\hat{E}$; si on pose $\bar{p}(\mathbf{x}) = \bar{d}(0, \mathbf{x})$, $\bar{p}$ est le prolongement de $p$ à $\hat{E}$ par continuité, et satisfait aux axiomes (NO_I) et (NO_{II}); en vertu de la continuité de $t \mathbf{x}$ dans $\hat{K} \times \hat{E}$, elle satisfait aussi à la condition (NO_{III}) (principe de prolongement des identités), donc est bien une *norme* sur $\hat{E}$.

Lorsqu’on considère sur un espace vectoriel E une structure déterminée d’espace normé, on désigne le plus souvent la norme d’un vecteur x par la notation $\|x\|$, si cette notation ne peut prêter à confusion.

### 4. Espaces quotients et espaces produits d’espaces normés

#### Proposition 10 {#top-ix-s3-prop-10 .statement}

Soient E une espace normé sur un corps valué non discret K, H un sous-espace vectoriel fermé de E. Si, pour toute classe $\dot{x} \in E/H$, on pose $\| \dot{x} \| = \inf_{x \in \dot{x}} \|x\|$, la fonction $\| \dot{x} \|$ est une norme sur l’espace vectoriel E/H, et la topologie définie par cette norme est la topologie quotient de celle de E par H.

En effet (IX, p. 27, Remarque), $d(\dot{x}, \dot{y}) = \| \dot{x} - \dot{y} \|$ est une distance invariante sur E/H, définissant la topologie quotient de celle de E par H. Il reste seulement à voir que $\| t \dot{x} \| = |t| \cdot \| \dot{x} \|$, ce qui résulte aussitôt de la définition de $\| \dot{x} \|$ (IV, p. 26, formule (23)).

La norme $\| \dot{x} \|$ peut encore s’interpréter de la manière suivante: c’est la distance (dans E) de tout point $x \in \dot{x}$ au sous-espace H, car l’ensemble des points de $\dot{x}$ est identique à l’ensemble des $x - z$, où z parcourt H.

#### Proposition 11 {#top-ix-s3-prop-11 .statement}

Soit $(E_i)_{1 \leq i \leq n}$ une famille finie d’espaces normés sur un corps valué non discret K; si, dans l’espace vectoriel produit $E = \prod_{i=1}^n E_i$, on pose, pour tout $x = (x_i)$, $\|x\| = \sup_{1 \leq i \leq n} \|x_i\|$, la fonction $\|x\|$ est une norme sur E, et définit sur cet espace la topologie produit de celles des $E_i$.

En effet, si $x = (x_i)$, $y = (y_i)$, on a $x + y = (x_i + y_i)$, donc
$$
\|x + y\| = \sup_i \|x_i + y_i\| \leq \sup_i (\|x_i\| + \|y_i\|)
$$
$$
\leq \sup_i \|x_i\| + \sup_i \|y_i\| = \|x\| + \|y\|.
$$

Il est clair d’autre part que $\| t x \| = |t| \cdot \|x\|$, et que $\|x\| = 0$ entraîne $\|x_i\| = 0$, donc $x_i = 0$ pour $1 \leq i \leq n$, c’est-à-dire $x = 0$; donc $\|x\|$ est bien une norme sur E. Par ailleurs, la relation $\|x\| < a$ équivaut aux n relations $\|x_i\| < a$, donc la norme $\|x\|$ définit bien sur E la topologie produit.

On montrerait de même que les fonctions $\sum_{i=1}^n \|x_i\|$ et $\sqrt{\sum_{i=1}^n \|x_i\|^2}$ sont des normes sur E; en vertu des inégalités (2) (IX, p. 33), les trois normes précédentes sont d’ailleurs équivalentes.

En particulier, sur l’espace vectoriel $K^n$ (à gauche ou à droite) sur K, si, pour $x = (x_i)_{1 \leq i \leq n}$, on pose
$$
p_1(x) = \sup_i |x_i|, \quad p_2(x) = \sum_{i=1}^n |x_i|, \quad p_3(x) = \sqrt{\sum_{i=1}^n |x_i|^2}
$$
les trois fonctions $p_1, p_2, p_3$ sont des normes équivalentes qui définissent sur $K^n$ la topologie produit de celles des facteurs K.

### 5. Fonctions multilinéaires continues

#### Théorème 1 {#top-ix-s3-thm-1 .statement}

Soient $E_i (1 \leq i \leq n)$ et $F$ des espaces normés sur un corps valué non discret $K$, et $f$ une application multilinéaire de $\prod_{i=1}^n E_i$ dans $F$. Pour que $f$ soit continue dans $\prod_{i=1}^n E_i$, il faut et il suffit qu’il existe un nombre $a > 0$ tel que, quels que soient les points $x_i \in E_i (1 \leq i \leq n)$, on ait

$$
\| f(x_1, x_2, \ldots, x_n) \| \leq a \cdot \| x_1 \| \cdot \| x_2 \| \cdots \| x_n \|.
$$

La condition est nécessaire. En effet, si $f$ est continue au point $(0, 0, \ldots, 0)$, il existe un nombre $b > 0$ tel que les conditions $\| x_i \| \leq b (1 \leq i \leq n)$ entraînent $\| f(x_i, \ldots, x_n) \| \leq 1$. Soit $t_0 \in K$ tel que $0 < |t_0| < 1$; pour tout point $(x_i) \in \prod_{i=1}^n E_i$ tel qu’aucun des $x_i$ ne soit nul, il existe $n$ entiers rationnels $k_i$ tels que $b |t_0| < \| t_0^{k_i} x_i \| \leq b$; par suite, on a

$$
|t_0|^{k_1 + k_2 + \cdots + k_n} \| f(x_1, \ldots, x_n) \| \leq 1;
$$

d’autre part on a $1/|t_0|^{k_i} \leq (1/b |t_0|) \| x_i \|$, d’où la relation (3), avec $a = 1/(b |t_0|)^n$; cette relation est évidemment encore vérifiée lorsque l’un des $x_i$ est nul.

La condition est suffisante. Montrons en effet que, si elle est remplie, $f$ est continue en tout point $(a_i)$ de $\prod_{i=1}^n E_i$. On peut écrire

$$
f(x_1, \ldots, x_n) - f(a_1, \ldots, a_n) = \prod_{i=1}^n f(a_1, \ldots, a_{i-1}, x_i - a_i, x_{i+1}, \ldots, x_n).
$$

Or, les conditions $\| x_i - a_i \| \leq r (1 \leq i \leq n)$ entraînent d’après (3)

$$
\| f(a_1, \ldots, a_{i-1}, x_i - a_i, x_{i+1}, \ldots, x_n) \| \leq a r \prod_{k \neq i}^n (\| a_k \| + r)
$$

d’où, en désignant par $c$ la borne supérieure des nombres $\| a_i \| (1 \leq i \leq n)$,

$$
\| f(x_1, \ldots, x_n) - f(a_1, \ldots, a_n) \| \leq n a r (c + r)^{n-1}.
$$

Comme le second membre est un polynôme en $r$ sans terme constant, il tend vers 0 avec $r$, ce qui prouve la continuité de $f$.

#### Remarque {#top-ix-s3-n5-rem-1 .statement}

Ce théorème entraîne deux propositions démontrées plus haut: d’une part, la continuité de la fonction bilinéaire $t x$ (IX, p. 31), en vertu de la relation $\| t x \| = |t| \cdot \| x \|$; d’autre part, la prop. 8 (IX, p. 32) en appliquant le th. 1 à l’application identique de $E$, considérée comme application linéaire de l’espace $E$ muni de la norme $p$ dans l’espace $E$ muni de la norme $q$ (ou vice-versa).

#### Corollaire 1 {#top-ix-s3-thm-1-cor-1 .statement}

Pour que $f$ soit continue dans $\prod_{i=1}^n E_i$, il faut et il suffit que $f$ soit bornée dans toute partie bornée de $\prod_{i=1}^n E_i$.

Comme les normes $\|x_i\|$ ($1 \leq i \leq n$) sont bornées lorsque $x = (x_1, \ldots, x_n)$ parcourt une partie bornée de $\prod_{i=1}^n E_i$, la nécessité de la condition résulte de l’inégalité (3). Inversement, s’il existe $c > 0$ tel que les $n$ relations $\|x_i\| \leq 1$ ($1 \leq i \leq n$) entraînent $\|f(x_1, \ldots, x_n)\| \leq c$, on voit comme dans la première partie de la démonstration du th. 1 que $f$ vérifie une inégalité de la forme (3).

#### Corollaire 2 {#top-ix-s3-thm-1-cor-2 .statement}

*Soient* $E, F$ *deux espaces normés sur un corps valué non discret* $K$. *Pour qu’une application linéaire surjective* $u$ *de* $E$ *dans* $F$ *soit un homéomorphisme, il faut et il suffit qu’il existe deux constantes* $a > 0,\ b > 0$ *telles que, pour tout* $x \in E$, *on ait* $a \|x\| \leq \|u(x)\| \leq b \|x\|$.

En effet, la condition est évidemment nécessaire en vertu du th. 1. Pour montrer qu’elle est suffisante, notons d’abord qu’elle entraîne que le noyau de $u$ est réduit à 0, donc que $u$ est bijective. En vertu du th. 1, elle entraîne ensuite que $u$ et $u^{-1}$ sont continues, d’où la conclusion.

### 6. Familles absolument sommables dans un espace normé

#### Définition 8 {#top-ix-s3-def-8 .statement}

*Dans un espace normé* $E$, *on dit qu’une famille* $(x_i)$ *de points de* $E$ *est absolument sommable, si la famille* $(\|x_i\|)$ *des normes des* $x_i$ *est sommable dans* $\mathbf{R}$.

Cette notion ne dépend qu’en apparence de la norme choisie sur $E$; en vertu de la prop. 8 de IX, p. 32, et du principe de comparaison des familles sommables de nombres réels, une famille absolument sommables pour une norme $p$ sur $E$ est absolument sommable pour toute norme *équivalente à* $p$.

Si $(x_i)_{i \in I}$ est une famille de points de $E$ sommable et absolument sommable, on a

$$
\left\| \sum_{i \in I} x_i \right\| \leq \sum_{i \in I} \|x_i\|.
$$

En effet, pour toute partie finie $J$ de $I$, on a $\left\| \sum_{i \in J} x_i \right\| \leq \sum_{i \in J} \|x_i\|$ et l’inégalité (4) en résulte par passage à la limite suivant l’ensemble ordonné filtrant des parties finies de $I$.

#### Proposition 12 {#top-ix-s3-prop-12 .statement}

*Dans un espace normé complet* $E$, *toute famille absolument sommable est sommable*.

En effet, si $(x_i)$ est une famille absolument sommable dans $E$, pour tout $\varepsilon > 0$, il existe une partie finie $J$ de l’ensemble d’indices $I$ telle que, pour toute partie finie $H$ de $I$ ne rencontrant pas $J$, on ait $\sum_{i \in H} \|x_i\| \leq \varepsilon$; on en conclut *a fortiori* $\left\| \sum_{i \in H} x_i \right\| \leq \varepsilon$, ce qui démontre la proposition, puisque $E$ est complet (critère de Cauchy, III, p. 38, th. 1).

On dit qu’une série de terme général $x_n$ est absolument convergente dans $E$ si la série de terme général $\|x_n\|$ est convergente dans $\mathbf{R}$; il revient au même de dire que la famille $(x_n)$ est absolument sommable; par suite (III, p. 44, prop. 9):

#### Corollaire 1 {#top-ix-s3-prop-12-cor-1 .statement}

Dans un espace normé complet $E$, toute série absolument convergente est commutativement convergente.

La réciproque de la prop. 11 est en général inexacte.

Considérons par exemple l’espace $\mathcal{B}(\mathbf{N})$ des suites bornées $x = (x_n)_{n \in \mathbf{N}}$ de nombres réels, avec la norme $\|x\| = \sup_n |x_n|$ (X, p. 20). Soit $x_m$ la suite $(x_{mn})_{n \in \mathbf{N}}$ telle que $x_{mn} = 0$ pour $n \neq m$, $x_{00} = 0$ et $x_{mn} = 1/m$ pour $m \geq 1$. On vérifie aussitôt que dans $\mathcal{B}(\mathbf{N})$ la suite $(x_m)_{m \in \mathbf{N}}$ est sommable et a pour somme l’élément $y = (y_n)$ tel que $y_0 = 0, y_n = 1/n$ si $n \geq 1$; mais comme $\|x_m\| = 1/m$, la suite des normes des $x_m$ n’est pas sommable dans $\mathbf{R}$.

On a vu toutefois (VII, p. 16) que, dans $\mathbf{R}^n$, toute famille sommable est absolument sommable.

#### Corollaire 2 {#top-ix-s3-prop-12-cor-2 .statement}

Si dans un espace normé $E$ toute série absolument convergente est convergente, alors $E$ est complet.

En effet, soit $(x_n)$ une suite de Cauchy dans $E$. Il existe une suite strictement croissante d’entiers $(n_k)$ telle que pour tout $k \geq 1$ on ait
$$
\|x_{n_{k+1}} - x_{n_k}\| \leq 2^{-k}.
$$
Par suite la série de terme général $(x_{n_{k+1}} - x_{n_k})(k \geq 1)$ est absolument convergente, donc convergente par hypothèse. Si $s$ est sa somme, $s + x_{n_1}$ est limite de la suite partielle $(x_{n_k})$; comme $(x_{n_k})$ est une suite de Cauchy, on en conclut qu’elle est convergente (II, p. 14, cor. 2 de la prop. 5), ce qui prouve que $E$ est complet.

### 7. Algèbres normées sur un corps valué

#### Définition 9 {#top-ix-s3-def-9 .statement}

Étant donnée une algèbre $A$ sur un corps valué commutatif non discret $K$, on dit qu’une norme $\|x\|$ sur $A$ (A étant considéré comme $K$-espace vectoriel) est compatible avec la structure d’algèbre de $A$ si elle vérifie la relation
$$
\|xy\| \leq \|x\| \cdot \|y\|
$$
quels que soient $x, y$ dans $A$. Une algèbre sur $K$, munie de la structure définie par une norme compatible avec sa structure d’algèbre, est appelée algèbre normée.

Si $A$ est une algèbre normée sur $K$, il est clair (IX, p. 35, th. 1) que l’application bilinéaire $(x, y) \mapsto xy$ de $A \times A$ dans $A$ est continue. Inversement, supposons que $A$ soit une algèbre sur $K$, munie d’une norme $p(x)$ telle que l’application $(x, y) \mapsto xy$ soit continue pour les topologies correspondantes; alors (IX, p. 35, th. 1), il existe une constante $a > 0$ telle que $p(xy) \leq ap(x)p(y)$. En remplaçant $p(x)$ par la norme équivalente (IX, p. 32, prop. 8) $a.p(x)$, on définit donc sur $A$ une structure d’algèbre normée. Lorsqu’une algèbre $A$ est munie d’une topologie pouvant être définie par une norme, et pour laquelle $(\mathbf{x}, \mathbf{y}) \mapsto \mathbf{x}\mathbf{y}$ est continue, on dit que l’algèbre topologique $A$ est *normable*.

Si $A$ est une algèbre normée, on déduit de (5), par récurrence sur $n$, que pour tout entier $n > 0$, on a

$$(6)$$
$$
\| \mathbf{x}^n \| \leq \| \mathbf{x} \| ^n .
$$

#### Exemple 1 {#top-ix-s3-n7-exa-1 .statement}

Soient $K$ un corps valué, $K'$ un sous-corps du centre de $K$ tel que la trace sur $K'$ de la valeur absolue $|x|$ de $K$ ne soit pas la valeur absolue impropre sur $K'$; $K$, muni de la norme $|x|$, est alors une algèbre normée sur $K'$.

#### Exemple 2 {#top-ix-s3-n7-exa-2 .statement}

Soient $K$ un corps commutatif valué non discret, $M_n(K)$ l’anneau des matrices carrées d’ordre $n$ sur $K$; on sait que, en tant qu’espace vectoriel sur $K$, $M_n(K)$ est isomorphe à $K^{n^2}$; si, pour toute matrice carrée d’ordre $n$ sur $K$, $X = (x_{ij})$, on pose $\| X \| = \sup_{i,j} |x_{ij}|$, on définit une norme sur $M_n(K)$, et la topologie définie par cette norme est identique à la topologie produit sur $K^{n^2}$ (IX, p. 34, prop. 11); il en résulte (vu la continuité des polynômes à un nombre quelconque de variables dans $K$) qu’une norme équivalente à la précédente est bien compatible avec la structre d’algèbre (par rapport à $K$) de $M_n(K)$.

#### Exemple 3 {#top-ix-s3-n7-exa-3 .statement}

L’ensemble $\mathscr{B}(E)$ des fonctions $f$ définies dans un ensemble $E$, prenant leurs valeurs dans un corps valué commutatif non discret $K$, et telles que $x \mapsto |f(x)|$ soit bornée dans $E$, est une algèbre sur $K$; la norme $\| f \| = \sup_{x \in E} |f(x)|$ est compatible avec la structure d’algèbre de $\mathscr{B}(E)$, car on a $\| fg \| \leq \| f \| \cdot \| g \|$

Soit $a$ un idéal bilatère fermé dans l’algèbre normée $A$; si, dans l’algèbre quotient $A/a$, on pose $\| \dot{\mathbf{x}} \| = \inf_{x \in \dot{\mathbf{x}}} \| \mathbf{x} \|$, on obtient sur $A/a$ une norme qui définit la topologie quotient de celle de $A$ par $a$ (IX, p. 34, prop. 10); comme pour $b > \| \dot{\mathbf{x}} \|$, $c > \| \dot{\mathbf{y}} \|$, il existe $\mathbf{x} \in \dot{\mathbf{x}}$ tel que $\| \mathbf{x} \| < b$ et $\mathbf{y} \in \dot{\mathbf{y}}$ tel que $\| \mathbf{y} \| < c$, on a $\| \mathbf{x}\mathbf{y} \| \leq \| \mathbf{x} \| \cdot \| \mathbf{y} \| < bc$, donc $\| \dot{\mathbf{x}}\dot{\mathbf{y}} \| \leq \| \dot{\mathbf{x}} \| \cdot \| \dot{\mathbf{y}} \|$, ce qui montre que $A/a$, muni de la norme $\| \dot{\mathbf{x}} \|$, est une algèbre normée.

De même, si $(A_i)_{1 \leq i \leq n}$ est une famille de $n$ algèbres normées sur un corps valué $K$, et si, dans l’algèbre produit $A = \sum_{i=1}^n A_i$, on pose, pour $\mathbf{x} = (\mathbf{x}_i)$, $\| \mathbf{x} \| = \sup_i \| \mathbf{x}_i \|$, on obtient sur $A$ une norme qui définit la topologie produit de celles des $A_i$ (IX, p. 34, prop. 11); comme $\mathbf{x}\mathbf{y} = (\mathbf{x}_i\mathbf{y}_i)$ et
$$
\| \mathbf{x}_i\mathbf{y}_i \| \leq \| \mathbf{x}_i \| \cdot \| \mathbf{y}_i \| \leq \| \mathbf{x} \| \cdot \| \mathbf{y} \|
$$
pour tout $i$, on a $\| \mathbf{x}\mathbf{y} \| \leq \| \mathbf{x} \| \cdot \| \mathbf{y} \|$, donc l’algèbre produit $A$, munie de la norme $\| \mathbf{x} \|$, est une algèbre normée.

Soit $A$ une algèbre normée sur un corps valué $K$. L’anneau complété $\hat{A}$ de $A$ (III, p. 51, prop. 6) est aussi muni d’une structure d’espace vectoriel par rapport à $\hat{K}$ (IX, p. 33, prop. 9), et on a évidemment, pour $t \in \hat{K}$, $\mathbf{x} \in \hat{A}$, $\mathbf{y} \in \hat{A}$, $t(\mathbf{x}\mathbf{y}) = (t\mathbf{x})\mathbf{y} = \mathbf{x}(t\mathbf{y})$ d’après le principe de prolongement des identités; $\hat{A}$ est donc une algèbre sur $\hat{K}$; d’autre part (IX, p. 33, prop. 9) la norme sur $A$ se prolonge par continuité en une norme sur $\hat{A}$, le principe de prolongement des inégalités montre que $\hat{A}$, munie de cette norme, est une algèbre normée sur le corps $\hat{K}$.

Si $(\mathbf{x}_\lambda)_{\lambda \in L}$ et $(\mathbf{y}_\mu)_{\mu \in M}$ sont deux familles absolument sommables dans une algèbre normée $A$, la famille $(\mathbf{x}_\lambda \mathbf{y}_\mu)_{(\lambda, \mu) \in L \times M}$ est absolument sommable puisque $\| \mathbf{x}_\lambda \mathbf{y}_\mu \| \leq \| \mathbf{x}_\lambda \| \cdot \| \mathbf{y}_\mu \|$ (IV, p. 35, prop. 1); si en outre $A$ est complète, ces trois familles sont sommables et on a $\sum_{(\lambda, \mu) \in L \times M} \mathbf{x}_\lambda \mathbf{y}_\mu = (\sum_{\lambda \in L} \mathbf{x}_\lambda) (\sum_{\mu \in M} \mathbf{y}_\mu)$ d’après l’associativité de la somme du premier membre (III, p. 40, formule (2)).

Lorsque l’algèbre normée $A$ possède un élément unité $e \neq 0$, l’application $t \mapsto te$ est un isomorphisme de la structure de corps de $K$ sur celle du sous-corps $Ke$ de $A$; cet isomorphisme est aussi un isomorphisme de la structure de corps topologique de $K$ sur celle de $Ke$ (la topologie sur ce dernier étant induite par celle de $A$), car la restriction $\| te \|$ de la norme de $A$ à $K$ est une norme équivalente à la valeur absolue $|t| = (1/\|e\|) \|te\|$. Lorsque $\|e\| = 1$, on a $\|te\| = |t|$; on peut alors identifier le corps valué $K$ au sous-corps normé $Ke$ de $A$, et en particulier écrire $1$ l’élément unité de $A$.

Il ne sera plus question, dans ce qui suit, que d’algèbres normées $A$ ayant un élément unité $e$; en faisant $x = y = e$ dans cette inégalité, on en déduit $\|e\| \geq 1$.

#### Proposition 13 {#top-ix-s3-prop-13 .statement}

*Si, dans $A$, la série de terme général $z^n$ est convergente, $e - z$ est inversible, et on a*

$$
(e - z)^{-1} = \sum_{n=0}^\infty z^n.
$$

*Inversement, si $\|z\| < 1$ et si $e - z$ est inversible, la série de terme général $z^n$ est convergente, et on a la formule (7).*

On a en effet, pour tout $p > 0$,

$$
(e - z) \sum_{n=0}^p z^n = e - z^{p+1}.
$$

Si la série de terme général $z^n$ est convergente et si $y$ est sa somme, $z^n$ tend vers 0 lorsque $n$ croît indéfiniment, donc en passant à la limite dans (8), on a $(e - z)y = e$, et on prouve de même que $y(e - z) = e$, c’est-à-dire que $y = (e - z)^{-1}$ (on notera que cette partie du raisonnement est valable dans un anneau topologique quelconque ayant un élément unité).

Inversement, si $\|z\| < 1$, comme on a $\|z^{p+1}\| \leq \|z\|^{p+1}$, $z^{p+1}$ tend vers 0 quand $p$ croît indéfiniment; en multipliant les deux membres de (8) à gauche par $(e - z)^{-1}$ et faisant croître $p$ indéfiniment, on voit que la série de terme général $z^n$ est convergente et a pour somme $(e - z)^{-1}$.

#### Corollaire {#top-ix-s3-n7-cor-1 .statement}

*Soit $A$ une algèbre normée complète; pour tout $z \in A$ tel que $\|z\| < 1$, $e - z$ est inversible dans $A$.*

En effet, la série de terme général $z^n$ est absolument convergente, puisque \|z^n\| \leq \|z\|^n \text{ pour } n > 0; \text{ elle est par suite convergente, puisque } A \text{ est complète (IX, p. 36, prop. 12).}

#### Proposition 14 {#top-ix-s3-prop-14 .statement}

Soit $G$ le groupe des éléments inversibles d’une algèbre normée complète $A$. Alors $G$ est un ensemble ouvert dans $A$; la topologie induite sur $G$ par celle de $A$ est compatible avec la structure de groupe de $G$; muni de cette topologie, $G$ est un groupe complet (pour chacune de ses deux structures uniformes).

Le cor. de la prop. 13 montre que $G$ contient un voisinage $V$ de $e$ dans $A$; pour tout $x_0 \in G$, les éléments de $x_0 V$ sont alors inversibles, et $x_0 V$ est un voisinage de $x_0$ dans $A$, puisque $x \mapsto x_0 x$ est alors un homéomorphisme de $A$ sur lui-même; donc $G$ est ouvert dans $A$.

Pour voir que la topologie induite sur $G$ par celle de $A$ est compatible avec la structure de groupe de $G$, il suffit de montrer que la fonction $x \mapsto x^{-1}$ est continue dans $G$. Pour cela, il suffit de prouver que si $x$ et $y$ appartiennent à $G$ et si

$$
\|x^{-1}\| \cdot \|x - y\| < 1
$$

on a

(9)
$$
\|x^{-1} - y^{-1}\| \leq \frac{\|x - y\| \cdot \|x^{-1}\|^2}{1 - \|x^{-1}\| \cdot \|x - y\|}.
$$

En effet, on peut écrire $x^{-1} - y^{-1} = x^{-1}(y - x)y^{-1}$ et il suffit donc de montrer que l’on a

(10)
$$
\|y^{-1}\| \leq \frac{\|x^{-1}\|}{1 - \|x^{-1}\| \cdot \|x - y\|}.
$$

Or on a $x^{-1}y = e - x^{-1}(x - y)$, et par suite $y^{-1} = (e - x^{-1}(x - y))^{-1}x^{-1}$.
Mais si $\|u\| < 1$, il résulte de la prop. 13 que l’on a

$$
\|(e - u)^{-1}\| \leq \sum_{n=0}^{\infty} \|u\|^n = (1 - \|u\|)^{-1}
$$

d’où l’égalité (10).

Pour établir enfin que la structure uniforme gauche de $G$ est une structure d’espace complet, montrons que tout filtre de Cauchy $\mathcal{F}$ pour cette structure, est un filtre de Cauchy pour la structure uniforme additive de $A$ et converge vers un point de $G$. En effet, pour tout $\varepsilon$ tel que $0 < \varepsilon < 1$, il existe un ensemble $M \in \mathcal{F}$ tel que, pour $x \in M$ et $y \in M$, on ait $\|x^{-1}y - e\| \leq \varepsilon$, ce qui entraîne $\|y - x\| \leq \varepsilon \|x\|$. Soit $a$ un point de $M$; pour tout $x \in M$, on a $\|x - a\| \leq \varepsilon \|a\|$, donc $\|x\| \leq (1 + \varepsilon)\|a\|$. D’autre part, il existe un ensemble $N \subset M$, appartenant à $\mathcal{F}$, et tel que $\|x^{-1}y - e\| \leq \frac{\varepsilon}{(1 + \varepsilon)\|a\|}$ pour $x \in N$ et $y \in N$; on en conclut que

$$
\|y - x\| \leq \frac{\varepsilon \|x\|}{(1 + \varepsilon)\|a\|} \leq \varepsilon,
$$

ce qui prouve que $\mathcal{F}$ est un filtre de Cauchy pour la structure uniforme additive de $A$, et par suite converge vers un point $x_0$, puisque

A est une algèbre complète. Comme $x_0$ est limite de $\mathfrak{F}$, on a, d’après le principe de prolongement des inégalités, $\| x^{-1} x_0 - e \| \leq \varepsilon$ pour tout $x \in M$; comme $\varepsilon < 1$, on en conclut que $x^{-1} x_0$ est inversible; par suite, il en est de même de $x_0$, c’est-à-dire que $x_0 \in G$.

#### Proposition 15 {#top-ix-s3-prop-15 .statement}

*Dans un corps valué complet, le groupe multiplicatif des éléments $\neq 0$ est un groupe complet.*

Il suffit de raisonner comme dans la prop. 14, en remplaçant la norme de A par la valeur absolue du corps considéré.

On notera qu’on ne peut pas appliquer directement la prop. 14, car un corps valué non commutatif n’est pas nécessairement une algèbre sur un corps valué commutatif *non discret* (la restriction au centre du corps de la valeur absolue peut être impropre).

#### Remarque {#top-ix-s3-n7-rem-1 .statement}

La prop. 14 est inexacte dans une algèbre normée non complète. Par exemple, dans l’algèbre $C(I)$ des fonctions numériques finies et continues dans $I = [0, 1]$ (la norme étant $\| x \| = \sup |x(t)|$), la sous-algèbre P formée des *polynômes* en t (restreints à I) n’est pas complète; si $x(t)$ est un polynôme non constant quelconque, $1 + \varepsilon x$ est arbitrairement voisin de l’élément unité 1 de P lorsque $\varepsilon$ est arbitrairement petit, mais $1 + \varepsilon x$ n’est pas inversible *dans* P. Toutefois, si A est une algèbre normée non complète, G le groupe des éléments inversibles de A, $\hat{A}$ l’algèbre normée complétée de A, G est un sous-groupe du groupe des éléments inversibles de $\hat{A}$, et par conséquent *la topologie induite sur G par celle de A est compatible avec sa structure de groupe*.

## EXERCICES {#top-ix-s3-exercises}

See the [exercises for § 3](exercises/s3/).
