---
book: var
book_title: Variétés différentielles et analytiques
chapter: "2"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 15
section_title: Variétés d’applications
lang: fr
source: var-fr
pdf_pages: 0174-0180
extraction: ocr
subsections:
    - "no": 1
      title: Fonctions de classe $C^{r,s}$
      page: 0
      pdf_page: 174
    - "no": 2
      title: Variété de classe $C^{r,s}$ au-dessus d’une variété de classe $C^r$
      page: 0
      pdf_page: 176
    - "no": 3
      title: Variétés de sections et variétés d’applications
      page: 0
      pdf_page: 178
statements: 0
exercises: 0
content_sha256: 47894c25c40367c68b455261d80abc0b0ca0569826499d939d8b09720496f1ec
---

## § 15. Variétés d’applications[^1]

Dans ce paragraphe, on suppose $K=\mathbf{R}$ ou $\mathbf{C}$. La lettre $r$ désigne un entier $\geq 1$ et la lettre $s$ un élément de $\mathbf{N}_K$ tel que $s\geq r$; on a $s=\omega$ si $K=\mathbf{C}$.

### 15.1. Fonctions de classe $C^{r,s}$

Dans ce n°, $E$ désigne un espace de Banach réel, $F_1$ et $F_2$ des espaces de Banach sur $K$, $V$ un ouvert de $E\times F_1$ et $f$ une application de $V$ dans $F_2$. On munit $E$, $F_1$ et $F_2$ de normes compatibles avec leurs structures d’espaces de Banach.

### 15.1.1 («Cas différentiable»).

On suppose $K=\mathbf{R}$ et $s\neq\omega$. On dit que $f$ est de classe $C^{r,s}$ (ou simplement $C^{r,s}$) si elle possède des dérivées partielles itérées $D_E^pD_{F_1}^qf$ (1.7.2) continues pour tout couple d’entiers positifs $(p,q)$ tels que $p\leq r$ et $p+q\leq s$. Il revient au même de dire que les dérivées partielles itérées $D_{F_1}^qf$ existent et sont de classe $C^r$ pour tout entier $q$ tel que $0\leq q\leq s-r$. Si $s=r$, cela équivaut à dire que $f$ est de classe $C^r$; si $s\geq r+1$, cela équivaut à dire que $f$ est de classe $C^r$ et $D_{F_1}f$ de classe $C^{r,s-1}$.

Si $f$ est de classe $C^{r,s}$, et si $p\leq r$, $p+q+1\leq s$, la fonction $D_E^pD_{F_1}^qf$ a une dérivée partielle par rapport à $F_1$ donnée par:

$$
D_{F_1}(D_E^pD_{F_1}^qf)=D_E^pD_{F_1}^{q+1}f.
$$

### 15.1.2 («Cas analytique»).

On suppose $s=\omega$. Pour tout entier $k\geq 0$, notons $P_k(F_1;F_2)$ l’espace des polynômes-continus homogènes de degré $k$ sur $F_1$ à valeurs dans $F_2$, muni de la norme définie dans l’Appendice du premier fascicule, p. 88, A.2.

On dit que $f$ est de classe $C^{r,\omega}$ (ou simplement $C^{r,\omega}$ s’il n’y a pas d’ambiguïté sur $K$) si, pour tout point $(x_0,y_0)\in V$, il existe un voisinage $U$ de $x_0$ dans $E$, des nombres réels $R>0$ et $M\geq 0$ et des fonctions $h_k:U\to P_k(F_1;F_2)$ ($k\in\mathbf{N}$), de classe $C^r$ (pour la structure de variété différentielle sous-jacente à la structure de K-variété de $P_k(F_1; F_2)$), tels que:

(i) $U \times (y_0 + B(R)) \subset V$, où $B(R)$ est la boule ouverte de rayon $R$ dans $F_1$;

(ii) si $x \in U$ et $p \leq r$, on a $\sum_{k=0}^{\infty} \| D^p h_k(x) \| R^k \leq M$;

(iii) si $x \in U$ et $t \in B(R)$, on a $\sum_{k=0}^{\infty} h_k(x)(t) = f(x, y_0 + t)$.

Ces propriétés entraînent:

(iv) Pour tout $t \in B(R)$, la fonction $x \mapsto f(x, y_0 + t)$ est de classe $C^r$ dans $U$, et l’on a

$$
D_E^p f(x, y_0 + t) = \sum_{k=0}^{\infty} D^p h_k(x)(t) \quad \text{si } p \leq r \text{ et } x \in U.
$$

On ne change pas la définition des fonctions de classes $C^{r,\omega}$ si l’on remplace la condition (ii) ci-dessus par l’une des deux conditions suivantes:

(ii’) Les $h_k$ définissent un morphisme de classe $C^r$ de $U$ dans l’espace de Banach réel sous-jacent au K-espace de Banach $\mathscr{H}_R(F_1; F_2)$ (3.1.1 et 3.1.2).

(ii’’) Les $h_k$ définissent un morphisme de classe $C^r$ de $U$ dans l’espace de Banach réel sous-jacent au K-espace de Banach $\tilde{\mathscr{H}}_R(F_1; F_2)$ (3.1.5).

15.1.3. Supposons $K = \mathbf{R}$. Pour que $f$ soit de classe $C^{r,\omega}_R$, il faut et il suffit que $f$ soit de classe $C^{r,\infty}$ (15.1.1) et que, pour tout $(x_0, y_0) \in V$, il existe un voisinage $V_0$ de $(x_0, y_0)$ dans $V$ et des nombres réels positifs $A$ et $M$ tels que

$$
\frac{1}{q!} \| D_E^p D_{F_1}^q f(x, y) \| \leq A \cdot M^q
$$

pour tout $p \leq r$, tout $q \geq 0$ et tout $(x, y) \in V_0$.

15.1.4. Supposons $K = \mathbf{C}$. Pour que $f$ soit de classe $C^{r,\omega}_C$, il faut et il suffit que les deux conditions suivantes soient vérifiées:

a) $f$ est de classe $C^{r,\omega}_R$ pour les structures réelles sous-jacentes à $F_1$ et $F_2$.

b) Pour tout $(x, y) \in V$, $D_{F_1} f(x, y)$ est une application $\mathbf{C}$-linéaire de $F_1$ dans $F_2$.

Lorsque $F_1$ est de dimension finie, on peut remplacer a) par:

a’) $f$ est de classe $C^r$.

15.1.5. L’ensemble des applications de classe $C^{r,s}$ de $V$ dans $F_2$ ne dépend pas du choix des normes sur $E, F_1, F_2$.

15.1.6. Soit $B$ une variété différentielle de classe $C^r$, soit $W$ un ouvert de $B \times F_1$, et soit $\rho$ une application de $W$ dans $F_2$. Soit $c = (U, \varphi, E_c)$ une carte de la variété $B$. Notons $W_c$ l’ouvert de $E_c \times F_1$ image par $\varphi \times \mathrm{Id}_{F_1}$ de $W \cap (U \times F_1)$ et $\rho_c$ l’application de $W_c$ dans $F_2$ telle que

$$
\rho_c(\varphi(x), y) = \rho(x, y) \quad \text{si } (x, y) \in W \cap (U \times F_1).
$$

L’application $\rho : W \to F_2$ est dite de classe $C^{r,s}$ si, pour toute carte $c$ de la variété $B$, l’application $\rho_c : W_c \to F_2$ est de classe $C^{r,s}$ au sens de 15.1.1 et 15.1.2; il suffit que cette condition soit réalisée pour une famille de cartes dont les domaines recouvrent $B$. Une telle application $\rho$ est de classe $C^r$ (pour les structures réelles sous-jacentes de $B \times F_1$ et $F_2$); sa restriction à l’ensemble $W \cap (\{b\} \times F_1)$ est un K-morphisme de classe $C^s$ pour tout $b \in B$.

15.1.7. Soient $B_1$ et $B_2$ des variétés différentielles de classe $C^r$, et $g : B_1 \to B_2$ un morphisme de classe $C^r$. Soit $W_1$ (resp. $W_2$) un ouvert de $B_1 \times F_1$ (resp. de $B_2 \times F_2$) et soit $h$ une application de $W_1$ dans $W_2$. On dit que $h$ est un $g$-morphisme de classe $C^{r,s}$ si $pr_1 \circ h = g \circ pr_1$ et si $pr_2 \circ h$ est une application de classe $C^{r,s}$ (15.1.6) de $W_1$ dans $F_2$.

Soient de même $B_3$ une variété de classe $C^r$, $W_3$ un ouvert de $B_3 \times F_3$, où $F_3$ est un K-espace de Banach, et $g'$ un morphisme de classe $C^r$ de $B_2$ dans $B_3$. Si $h$ (resp. $h'$) est un $g$-morphisme (resp. $g'$-morphisme) de classe $C^{r,s}$ de $W_1$ dans $W_2$ (resp. de $W_2$ dans $W_3$), le composé $h' \circ h$ est un $(g' \circ g)$-morphisme de classe $C^{r,s}$ de $W_1$ dans $W_3$.

### 15.2. Variété de classe $C^{r,s}$ au-dessus d’une variété de classe $C^r$

Dans tout ce n°, on note $B$ une variété différentielle de classe $C^r$.

15.2.1. Soit $X$ un ensemble muni d’une application $p : X \to B$. On appelle carte de $X$ au-dessus de $B$ un triplet $\theta = (V, \psi, F)$, où $V$ est une partie de $X$, $F$ un K-espace de Banach, et $\psi$ une bijection de $V$ sur un ouvert de $B \times F$ telle que $pr_1 \circ \psi = p|V$.

Soit $(\theta_i)_{i \in I} = ((V_i, \psi_i, F_i))_{i \in I}$ une famille de cartes de $X$ au-dessus de $B$. On dit que les $\theta_i$ sont $C^{r,s}$-compatibles si, pour tout couple d’éléments $i, j$ de $I$, les deux conditions suivantes sont satisfaites:

a) $\psi_i(V_i \cap V_j)$ est ouvert dans $B \times F_i$ et $\psi_j(V_i \cap V_j)$ est ouvert dans $B \times F_j$;
b) l’application $\psi_i \circ \psi_j^{-1}$ de $\psi_j(V_i \cap V_j)$ dans $\psi_i(V_i \cap V_j)$ est un $\mathrm{Id}_B$-morphisme de classe $C^{r,s}$ (15.1.7).

Une famille $((V_i, \psi_i, F_i))_{i \in I}$ de cartes de $X$ au-dessus de $B$ qui sont $C^{r,s}$-compatibles et dont les domaines $V_i$ recouvrent $X$ est appelée un $C^{r,s}$-atlas de $X$ (au-dessus de $B$). Deux $C^{r,s}$-atlas sont dits équivalents si leur réunion est un $C^{r,s}$-atlas; la relation de $C^{r,s}$-équivalence entre atlas est une relation d’équivalence. Une classe d’équivalence de $C^{r,s}$-atlas s’appelle une structure de variété de classe $C^{r,s}$ au-dessus de $B$ sur l’ensemble $X$; lorsque l’on désire préciser $K$, on écrit $C_K^{r,s}$ au lieu de $C^{r,s}$. Si $X$ est une variété de classe $C^{r,s}$ au-dessus de $B$, on dit que $p : X \to B$ est la projection de $X$; si $\theta$ est une carte de $X$ au-dessus de $B$, on dit que $\theta$ est une carte de la $C^{r,s}$-variété $X$ si $\theta$ appartient à un atlas de la classe d’équivalence définissant la structure de $X$.

15.2.2. Soit $X$ une variété de classe $C^{r,s}$ au-dessus de $B$, de projection $p$. Il existe sur $X$ une structure de variété différentielle de classe $C^r$ et une seule, telle que, pour toute carte $(V, \psi, F)$ de la $C^{r,s}$-variété $X$, l’ensemble $V$ soit ouvert dans $X$ et que $\psi$ soit un $C^r$-isomorphisme de la sous-variété ouverte $V$ de $X$ sur la sous-variété ouverte $\psi(V)$ de $B \times F$. Si l’on munit $X$ de cette structure, l’application $p : X \to B$ est une submersion de classe $C^r$.

Soit $b \in B$ et soit $X_b = p^{-1}(b)$. Il existe une structure de $K$-variété de classe $C^s$ sur $X_b$, et une seule, telle que, pour toute carte $\theta = (V, \psi, F)$ de la $C^{r,s}$-variété $X$, le triplet $\theta_b = (V \cap X_b, \operatorname{pr}_2 \circ \psi|_{(V \cap X_b)}, F)$ soit une carte de la variété $X_b$. La structure de variété différentielle de classe $C^r$ sous-jacente à cette structure est induite par la structure de variété différentielle de classe $C^r$ sur $X$ définie ci-dessus.

15.2.3. Exemples

(i) Lorsque $B$ est réduite à un point, la notion de variété de classe $C_K^{r,s}$ au-dessus de $B$ est équivalente à celle de $K$-variété de classe $C^s$.

(ii) Soit $Z$ une $K$-variété de classe $C^s$; prenons $X = B \times Z$ et $p = \operatorname{pr}_1$. Il existe sur $X$ une structure de variété de classe $C^{r,s}$ au-dessus de $B$, et une seule, telle que, pour toute carte $(U, \psi, L)$ de $Z$, $(B \times U, \operatorname{Id}_B \times \psi, L)$ soit une carte de $C^{r,s}$-variété $X$.

(iii) Soient $X$ une variété de classe $C^{r,s}$ au-dessus de $B$, et $Y$ un ouvert de $X$. La structure de variété de classe $C^{r,s}$ de $Y$ *induite* par celle de $X$ se définit comme dans le cas des variétés (cf. 5.2.3).

(iv) Soit $M$ un fibré vectoriel sur $K$ de base $B$ et de classe $C^r$ (7.3.4), et soit $\pi$ sa projection sur $B$. Il existe sur $M$ une structure de variété de classe $C_K^{r,\omega}$ au-dessus de $B$, et une seule, telle que, si $(U, \psi, F)$ est une carte $K$-vectorielle de $M$ (8.8.1), le triplet $(\pi^{-1}(U), \psi, F)$ soit une carte de la $C_K^{r,\omega}$-variété $M$.

15.2.4. Soient $X$ une variété de classe $C^{r,s}$ au-dessus de $B$, $p$ sa projection, $L$ un $K$-espace de Banach, et $f$ une application de $X$ dans $L$. On dit que $f$ est de classe $C^{r,s}$ si, pour toute carte $(V, \psi, F)$ de la $C^{r,s}$-variété $X$, l’application $(f|V) \circ \psi^{-1}$ de $\psi(V)$ dans $L$ est de classe $C^{r,s}$ (15.1.6). Une telle application est de classe $C^r$ et sa restriction à $X_b$ pour $b \in B$, est de classe $C^s$.

15.2.5. Soit $g : B \to B'$ un morphisme de variétés différentielles de classe $C^r$, soit $X$ (resp. $X'$) une variété de classe $C^{r,s}$ au-dessus de $B$ (resp. $B'$), et soit $h$ une application de $X$ dans $X'$. On dit que $h$ est un *g-morphisme de classe* $C^{r,s}$ si les trois conditions suivantes sont satisfaites:

a) $p' \circ h = g \circ p$;
b) $h$ est continue;
c) pour toute carte $(V', \psi', F')$ de la $C^{r,s}$-variété $X'$, l’application $\operatorname{pr}_2 \circ \psi' \circ h$ de $V = h^{-1}(V')$ dans $F'$ est de classe $C^{r,s}$ (au sens de 15.2.4) lorsqu’on munit l’ouvert $V$ de la structure induite par celle de $X$ (15.2.3, (iii)).

Lorsque $B = B'$ et $g = \operatorname{Id}_B$, on dit aussi que $h$ est un *B-morphisme de classe* $C^{r,s}$.

Pour qu’un B-morphisme de classe $C^{r,s}$ soit un B-isomorphisme de classe $C^{r,s}$, il suffit que ce soit un isomorphisme de classe $C^1$.

Soit $g': B' \to B''$ un morphisme de variétés de classe $C^r$ et soit $X''$ une variété de classe $C^{r,s}$ au-dessus de $B''$. Si $h: X \to X'$ est un $g$-morphisme de classe $C^{r,s}$ et $h': X' \to X''$ est un $g'$-morphisme de classe $C^{r,s}$, alors $h' \circ h$ est un $(g' \circ g)$-morphisme de classe $C^{r,s}$.

15.2.6. Soient $X$ une variété de classe $C^{r,s_j}_R$ au-dessus de $B$ et $p$ sa projection; on suppose $s \neq \omega$, $X$ séparée et $p$ propre (TG, I, § 10, n° 1). Alors, pour tout $b \in B$, il existe un voisinage ouvert $U$ de $b$ et un $C^{r,s}$-isomorphisme de $p^{-1}(U)$ sur $U \times X_b$, où $X_b = p^{-1}(b)$.

15.2.7. Soient $X$ une variété de classe $C^{r,s}_K$ au-dessus de $B$, $p$ sa projection, et $\sigma : B \to X$ une section de classe $C^r$. On appelle *voisinage tubulaire* de classe $C^{r,s}_K$ de $\sigma$ un triplet $(M, N, \varphi)$ où $M$ est un fibré $K$-vectoriel, de base $B$ et de classe $C^r$, $N$ est un voisinage ouvert de $\sigma(B)$ dans $X$, et $\varphi$ est un $B$-isomorphisme de classe $C^{r,s}_K$ de $N$ sur un ouvert de $M$ (cf. 15.2.3 (iv)), transformant la section $\sigma$ en la section nulle de $M$.

Supposons que $s \geq r + 1$ et que la variété $B$ soit paracompacte et admette des partitions de l’unité de classe $C^r$ (5.3.6); il existe alors des voisinages tubulaires de classe $C^{r,s}_K$ de $\sigma$.

### 15.3. Variétés de sections et variétés d’applications

15.3.1 (« Structure d’espace de Banach sur un espace de sections »). Soit $B$ une variété différentielle *compacte* de classe $C^r$; soit $M$ un fibré vectoriel sur $K$ (7.3.4) de base $B$ et de classe $C^r$; notons $M_r$ la variété différentielle de classe $C^r$ sous-jacente à $M$, et soit $\mathscr{S}_M^r(B)$ le $K$-espace vectoriel des sections de classe $C^r$ de $M$ (7.4.1). La topologie induite sur $\mathscr{S}_M^r(B)$ par la topologie de la $C^r$-convergence uniforme de $\mathscr{C}^r(B; M_r)$ (12.3.10) fait de $\mathscr{S}_M^r(B)$ un $K$-*espace de Banach*.

Soit $(U_i)_{i \in I}$ un recouvrement ouvert *fini* de $B$ et, pour tout $i \in I$, soient $c_i = (U_i, \varphi_i, E_i)$ une carte de $B$ et $t_i = (U_i, \psi_i, F_i)$ une carte $K$-vectorielle de $M$ (8.8.1). Munissons chacun des $E_i$ (resp. $F_i$) d’une norme compatible avec sa structure d’espace de Banach sur $\mathbf{R}$ (resp. $K$) et soit $(V_i)_{i \in I}$ un recouvrement fermé de $B$, tel que $V_i \subset U_i$ pour tout $i \in I$. Pour $f \in \mathscr{S}_M^r(B)$ et $i \in I$, notons $f_i$ l’application de $\varphi_i(U_i)$ dans $F_i$ obtenue par composition:

$$
\varphi_i(U_i) \xrightarrow{\phi_i^{-1}} U_i \xrightarrow{f} M|U_i \xrightarrow{\psi_i} U_i \times F_i \xrightarrow{\mathrm{pr}_2} F_i.
$$

Posons
$$
\|f\| = \operatorname{Sup}_{i \in I,\ p \leq r,\ x \in V_i} \|D^p f_i(\varphi_i(x))\|.
$$
L’application $f \mapsto \|f\|$ est une *norme* sur $\mathscr{S}_M^r(B)$, qui définit la structure d’espace de Banach sur $K$ de $\mathscr{S}_M^r(B)$.

Si $N$ est un ouvert de l’espace $M$, l’ensemble $\mathscr{S}^r(B; N)$ des sections $f \in \mathscr{S}_M^r(B)$ telles que $f(B) \subset N$ est ouvert dans $\mathscr{S}_M^r(B)$.

15.3.2. Soit $B$ une variété différentielle compacte de classe $C^r$, et soit $X$ une variété de classe $C^{r,s}_K (s \geq r + 1)$ au-dessus de B. Si N est un ouvert de X, notons $\mathscr{S}'(B; N)$ l’ensemble des sections de classe $C^r$ de X sur B dont l’image est contenue dans N. Il existe sur $\mathscr{S}'(B; X)$ une structure de K-variété de classe $C^{s-r}$, et une seule, telle que, pour toute section $\sigma \in \mathscr{S}'(B; X)$ et tout voisinage tubulaire $(M, N, \varphi)$ de classe $C^{r,s}_K$ de $\sigma$ (15.2.7), le triplet $(\mathscr{S}'(B; N), \varphi^*, \mathscr{S}'_M(B))$, où $\varphi^*$ est l’application $f \mapsto \varphi \circ f$, soit une carte de la K-variété $\mathscr{S}'(B; X)$.

Dans ce qui suit, on munit $\mathscr{S}'(B; X)$ de cette structure.

15.3.3. Soit X une variété différentielle compacte de classe $C^r$, et soit Y une K-variété de classe $C^s (s \geq r + 1)$. Soit $\mathscr{C}^r(X; Y)$ l’ensemble des applications de classe $C^r$ de X dans Y (autrement dit, à valeurs dans la variété de classe $C^r$ sous-jacente à Y, cf. 5.13.1 et 5.14.2). On munit $\mathscr{C}^r(X; Y)$ de la structure de K-variété de classe $C^{s-r}$ obtenue en l’identifiant à $\mathscr{S}'(X; X \times Y)$, cf. 15.2.3, (ii) et 15.3.2. On l’appelle la variété des applications de classe $C^r$ de X dans Y. Sa topologie est celle de la $C^r$-convergence uniforme (12.3.10).

Supposons Y séparée ; il en est alors de même de $\mathscr{C}^r(X; Y)$. De plus, l’ensemble des immersions (resp. plongements, submersions, submersions surjectives, morphismes étales, isomorphismes) de classe $C^r$ de X dans Y est un ouvert de $\mathscr{C}^r(X; Y)$.

Soient $X'$ une variété différentielle compacte de classe $C^r$, $\varphi : X' \to X$ un morphisme de variétés différentielles de classe $C^r$ et $\psi : Y \to Y'$ un morphisme de K-variétés de classe $C^s$. L’application $f \mapsto \psi \circ f \circ \varphi$ est un morphisme de classe $C^{s-r}$ de $\mathscr{C}^r(X; Y)$ dans $\mathscr{C}^r(X'; Y')$.

15.3.4 (« Affaiblissement de structure »). Gardons les hypothèses et notations de 15.3.3. Soit de plus $s' \in \mathbf{N}_R$ avec $r < s' \leq s$ et soit $Y_{s'}$ la variété réelle de classe $C^{s'}$ sous-jacente à Y (5.13 et 5.14.2). La structure de variété réelle de classe $C^{s'-r}$ de $\mathscr{C}^r(X; Y_{s'})$ est sous-jacente à la structure de K-variété de classe $C^{s-r}$ de $\mathscr{C}^r(X; Y)$.

15.3.5. Soient X et $X'$ des variétés différentielles compactes de classe $C^r$ et $C^{r'}$ respectivement, avec $r' < r$; et soit Y une K-variété de classe $C^s$, avec $s \geq r + 1$. Soit $t = \operatorname{Inf}(r - r', s - r)$. L’application $(f, g) \mapsto g \circ f$ est un morphisme de classe $C^t$ de $\mathscr{C}^{r'}(X'; X) \times \mathscr{C}^r(X; Y)$ dans $\mathscr{C}^{r'}(X'; Y)$.

15.3.6 (« Espace tangent à $\mathscr{C}^r(X; Y)$ »). Les hypothèses étant celles de 15.3.3, soit $f \in \mathscr{C}^r(X; Y)$ et soit $\xi$ un vecteur tangent en $f$ à la variété $\mathscr{C}^r(X; Y)$. Si $x \in X$, notons $\varepsilon_x$ l’application $g \mapsto g(x)$ de $\mathscr{C}^r(X; Y)$ dans Y ; c’est un morphisme de classe $C^{s-r}$. L’image par $T_f(\varepsilon_x)$ de $\xi$ est un élément $\xi_x$ de $T_{f(x)}(Y)$; l’application $x \mapsto \xi_x$ est un relèvement de classe $C^r$ de $f$ dans $T(Y)$ (cf. 8.6.1) et on peut l’identifier à une section de classe $C^r$ du fibré vectoriel $f^*T(Y)$ de base X. On obtient de cette façon un isomorphisme de l’espace tangent $T_f(\mathscr{C}^r(X; Y))$ sur l’espace de Banach $\mathscr{S}'_{f^*T(Y)}(X)$.

15.3.7 (« Interprétation de $\mathscr{C}^p(X; \mathscr{C}^q(Y; Z))$ »). Soient X et Y des variétés différentielles compactes de classe $C^p$ et $C^q$ respectivement ($1 \leq p \leq +\infty, 1 \leq q < +\infty$), et soit Z une K-variété de classe $C^s$, avec $s \geq p + q$. Soit $f : X \times Y \to Z$ une application continue; pour tout $x \in X$, notons $f_x$ l’application $y \mapsto f(x, y)$ de $Y$ dans $Z$. Les deux propriétés suivantes sont équivalentes:

a) Quelles que soient les cartes $c = (U, \varphi, E)$ de $X$, $d = (V, \psi, F)$ de $Y$ et $e = (W, \theta, G)$ de $Z$ telles que $f(U \times V) \subset W$, les dérivées partielles $D_E^{p'} D_F^{q'} f'$ de l’expression $f'$ de $f$ dans les cartes $c \times d$ et $e$ (5.3.2) existent et sont continues pour $p' \leq p$ et $q' \leq q$.

b) Pour tout $x \in X$, l’application $f_x$ est de classe $C^q$ et l’application $x \mapsto f_x$ est un morphisme de classe $C^p$ de $X$ dans la variété $\mathscr{C}^q(Y ; Z)$.

15.3.8. Soit $Y$ une $K$-variété compacte de classe $C^s$, avec $s \geq r + 1$, et soit $\mathrm{Diff}'(Y)$ le groupe des automorphismes de classe $C^r$ de la variété réelle $Y_r$, de classe $C^r$ sous-jacente à $Y$. L’ensemble $\mathrm{Diff}'(Y)$ est ouvert dans $\mathscr{C}^r(Y ; Y) = \mathscr{C}^r(Y_r ; Y)$; on le munit de la structure de $K$-variété de classe $C^{s-r}$ induite par celle de $\mathscr{C}^r(Y ; Y)$. La loi de composition $(f, g) \mapsto g \circ f$ fait de $\mathrm{Diff}'(Y)$ un groupe topologique. Par contre, la structure de variété de classe $C^{s-r}$ n’est pas en général compatible avec la structure de groupe de $\mathrm{Diff}'(Y)$. Pour $f \in \mathrm{Diff}'(Y)$, l’application $g \mapsto g \circ f$ de $\mathrm{Diff}'(Y)$ dans lui-même est de classe $C^{s-r}$, mais l’application $g \mapsto f \circ g$ n’est pas en général de classe $C^1$. En particulier, $\mathrm{Diff}'(Y)$ n’est pas en général un groupe de Lie.$^{(1)}$

$^1$ Supposons $s = \infty$. Soit $\mathrm{Diff}^\infty(Y)$ le groupe des automorphismes de classe $C^\infty$ de $Y$; munissons-le de la topologie la moins fine rendant continues les injections canoniques $\mathrm{Diff}^\infty(Y) \to \mathrm{Diff}'(Y)$ pour tout entier $r \geq 1$. Soit d’autre part $\mathrm{Diff}^0(Y)$ le groupe des homéomorphismes de $Y$, muni de la topologie de la convergence uniforme (TG, X, § 3, n° 5, prop. 11). Si dim $Y \geq 1$, il est impossible de trouver un groupe de Lie $G$ et des homomorphismes continus de $\mathrm{Diff}^\infty(Y)$ dans $G$ et de $G$ dans $\mathrm{Diff}^0(Y)$ dont le composé soit l’injection canonique (cf. LIE, III, § 4, exerc. 7).

[^1]: Les définitions et résultats de ce paragraphe s’étendent sans modifications essentielles au cas où l’espace de Banach $E$ du n° 15.1 est remplacé par un demi-espace fermé et au cas où la variété $B$ des n° 15.1.6 à 15.3.2 (resp. la variété $X$ du n° 15.3.3) est remplacée par une pièce d’une variété (11.1.2). En particulier, l’espace des applications de classe $C^r$ du segment $\{0,1\}$ dans une $K$-variété $Y$ de classe $C^s$ ($s>r$) a une structure naturelle de $K$-variété de classe $C^{r,s}$. Une autre généralisation possible consiste à remplacer $E$ et $B$ (resp. $X$) par des espaces topologiques (resp. par un espace topologique compact) et à prendre $r=0$. Ainsi, si $X$ est un espace compact et $Y$ une $K$-variété de classe $C^s$, l’ensemble $C^0(X;Y)$ des applications continues de $X$ dans $Y$ a une structure naturelle de $K$-variété de classe $C^s$ (la topologie sous-jacente étant celle de la convergence uniforme). Nous laissons au lecteur le soin de développer ces brèves indications.
