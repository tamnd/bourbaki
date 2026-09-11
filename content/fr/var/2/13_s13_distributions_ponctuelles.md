---
book: var
book_title: Variétés différentielles et analytiques
chapter: "2"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 13
section_title: Distributions ponctuelles
lang: fr
source: var-fr
pdf_pages: 0152-0161
extraction: ocr
subsections:
    - "no": 1
      title: Tenseurs symétriques et espaces de Banach
      page: 0
      pdf_page: 152
    - "no": 2
      title: Distributions ponctuelles
      page: 0
      pdf_page: 153
    - "no": 3
      title: Distributions ponctuelles et espaces tangents
      page: 0
      pdf_page: 156
    - "no": 4
      title: Produit tensoriel de distributions ponctuelles
      page: 0
      pdf_page: 157
    - "no": 5
      title: Coproduits
      page: 0
      pdf_page: 159
    - "no": 6
      title: Distributions à support fini
      page: 0
      pdf_page: 160
    - "no": 7
      title: Affaiblissement de structure
      page: 0
      pdf_page: 161
statements: 0
exercises: 0
content_sha256: 4e1cfc6fb0ea10651026181a15c455ecd575a63746635f7a5b12e614beb9bb93
---

## § 13. Distributions ponctuelles

### 13.1. Tenseurs symétriques et espaces de Banach

### 13.1.1. Soit E un module sur un anneau commutatif A. Si n est un entier $\geq 0$, on note $TS^n(E)$ le module des tenseurs symétriques de rang n de E (A, III, p. 71 et A, IV, § 5, no 2); la somme directe des $TS^n(E)$ est notée $TS(E)$. Si r est un entier, soit l’un des symboles $\infty,\omega$, on pose

$$
TS^{(r)}(E)=\bigoplus_{n\leq r}TS^n(E)\quad\text{et}\quad TS^{(r)+}(E)=\bigoplus_{1\leq n\leq r}TS^n(E);
$$

par suite, si $r\geq 0$, $TS^{r}(E)$ est somme directe de $TS^{(0)}(E)=A$ et de $TS^{(r)+}(E)$. On a $TS^{(1)+}(E)=E$ et $TS^{(\infty)}(E)=TS^{(\omega)}(E)=TS(E)$.

Si $n$ est un entier $\geq 0$, et si $x\in E$, on note $\gamma_n(x)$ l’élément $x\otimes\cdots\otimes x$ de $TS^n(E)$; pour $n=0$, $\gamma_0(x)=1$.

### 13.1.2. (« Applications polynomiales »). On suppose que A est intègre infini et que E est un A-module libre. Soit F un A-module. Une application $f:E\rightarrow F$ est dite polynomiale homogène de degré n si elle satisfait aux conditions équivalentes suivantes (cf. A, IV, § 5, no 9):

a) Il existe une application linéaire $\tilde f:TS^n(E)\rightarrow F$ telle que $f(x)=\tilde f(\gamma_n(x))$ pour tout $x\in E$.

b) Il existe une application multilinéaire $u:E^n\rightarrow F$ telle que $f(x)=u(x,\ldots,x)$ pour tout $x\in E$.

Supposons que ce soit le cas. L’application $\tilde f$ vérifiant a) est alors unique; si $t\in TS^n(E)$, on note $\langle f,t\rangle$ l’élément $\tilde f(t)$. Si $u:E^n\rightarrow F$ vérifie b), l’application linéaire correspondante de $\otimes^nE$ dans F coïncide dans le sous-module $TS^n(E)$. Lorsque $n!$ est inversible dans A, on peut choisir $u$ symétrique, et cela de façon unique.

### 13.1.3. Soient E un espace de Banach sur K et F un espace polynômé séparé sur K. Soient U un voisinage ouvert de 0 dans E, $f:U\rightarrow F$ une application de classe $C^r$ ($r\in\mathbf{N}_K$), et $t$ un élément de $TS^{(r)}(E)$, cf. 13.1.1 (appliqué à l’anneau $A=K$). Soit $k$ un entier $\leq r$ tel que $t\in TS^{(k)}(E)$. On peut décomposer $t$ et $f$ de façon unique en

$$
t=t_0+\cdots+t_k,\qquad \text{avec }t_i\in TS^i(E)
$$

et

$$
f=f_0+\cdots+f_k+h,
$$

où $f_i$ est un polynôme-continu homogène de degré $i$ ($0 \leq i \leq k$) et où $h$ a un contact d’ordre $\geq k$ avec 0 au point 0. On pose alors

$$
\langle f, t \rangle = \sum_{i=0}^{k} \langle f_i, t_i \rangle;
$$

c’est un élément de F qui ne dépend pas du choix de $k$.

13.1.4. Soient E et E’ deux espaces de Banach, U un voisinage ouvert de 0 dans E et $\varphi : U \to E'$ une application de classe $C^r$ telle que $\varphi(0) = 0$. Soit $t \in TS^{(r)}(E)$. Il existe un élément $t' \in TS^{(r)}(E')$ et un seul tel que, quels que soient l’espace polynormé séparé F, le voisinage ouvert U’ de 0 dans E’, et l’application $f : U' \to F$ de classe $C^r$, on ait

(*) $$
\langle f, t' \rangle = \langle f \circ \varphi, t \rangle.
$$

Cet élément $t'$ se note $\varphi_*(t)$. L’application

$$
\varphi_* : TS^{(r)}(E) \to TS^{(r)}(E')
$$

ainsi définie est linéaire.

### 13.2. Distributions ponctuelles

Dans ce numéro, X désigne une variété de classe $C^r$, et $x$ un point de X.

13.2.1. Soit $\mathscr{A}$ l’ensemble des couples $(c, t)$, où $c = (U, \varphi, E)$ est une carte de X centrée en $x$, et où $t \in TS^{(r)}(E)$. Deux éléments $((U, \varphi, E), t)$ et $((U', \varphi', E'), t')$ de $\mathscr{A}$ sont dits équivalents si $t' = \gamma_*(t)$, où $\gamma = \varphi' \circ \varphi^{-1}$. On obtient ainsi une relation d’équivalence sur $\mathscr{A}$; une classe d’équivalence pour cette relation est appelée une distribution ponctuelle en $x$ sur X.

Soit $T_x^{(r)}(X)$ l’ensemble des distributions ponctuelles en $x$ sur X. Si $c$ est une carte de X centrée en $x$, l’application

$$
\theta_c : TS^{(r)}(E) \to T_x^{(r)}(X)
$$

qui, à $t$, fait correspondre la classe de $(c, t)$, est une bijection. Dans tout ce qui suit, on munit $T_x^{(r)}(X)$ de la structure de K-espace vectoriel obtenue en transportant celle de $TS^{(r)}(E)$ par $\theta_c$; cette structure ne dépend pas du choix de $c$. De même, si $k \leq r$, on note $T_x^{(k)}(X)$ et $T_x^{(k)+}(X)$ les images de $TS^{(k)}(E)$ et $TS^{(k)+}(E)$ par $\theta_c$; elles ne dépendent pas du choix de $c$. Un élément de $T_x^{(r)}(X)$ est dit d’ordre $\leq k$ s’il appartient à $T_x^{(k)}(X)$. On a

$$
T_x^{(k)}(X) = T_x^{(0)}(X) \oplus T_x^{(k)+}(X).
$$

Il existe un élément et un seul $\varepsilon_x$ de $T_x^{(0)}(X)$ tel que l’on ait $\theta_c(1) = \varepsilon_x$ pour toute carte $c$ de X centrée en $x$. Si $t$ est une distribution ponctuelle en $x$, on appelle terme constant de $t$ l’élément $\lambda$ de K tel que $t - \lambda \varepsilon_x \in T_x^{(r)+}(X)$; on dit que $t$ est sans terme constant si son terme constant est nul.

13.2.2. Soit F un espace polynormé séparé, et soit $f$ une fonction de classe $C^r$ à valeurs dans F, définie sur un voisinage de $x$. Soit $t$ une distribution ponctuelle en $x$ sur X.

Considérons une carte $c = (U, \varphi, E)$ de $X$ centrée en $x$, et posons $f_c = f \circ \varphi^{-1}$ et $t_c = \theta_c^{-1}(t)$; l’élément $\langle f_c, t_c \rangle$ de $F$ défini en 13.1.3 ne dépend pas du choix de $c$; on le note $\langle f, t \rangle$. On a $\varepsilon_x(f) = f(x)$.¹ Le terme constant de $t$ est $\langle 1, t \rangle$.

Si $F'$ est un espace polynormé séparé et si $u : F \to F'$ est linéaire continue, on a $\langle u \circ f, t \rangle = u(\langle f, t \rangle)$.

Supposons que $F$ soit un espace de Banach, et que $t$ soit d’ordre $\leq k$, avec $k$ fini. Soit $j \in J_x^k(X, F)$, cf. 12.1.2, et soit $f \in j$. Alors $\langle f, t \rangle$ ne dépend que du jet $j$; on le note $\langle j, t \rangle$. L’application de $T_x^{(k)}(X) \times J_x^k(X, F)$ dans $F$ ainsi définie est bilinéaire. Lorsque $F = K$, on a posé $J_x^k(X, F) = P_x^k(X)$, cf. 12.6.2, et l’on obtient une *forme bilinéaire* sur $T_x^{(k)}(X) \times P_x^k(X)$.

13.2.3. Soit $\varphi : X \to Y$ un morphisme de variétés de classe $C^r$ et soit $y = \varphi(x)$. Soit $c = (U, \psi, E)$ une carte de $X$ centrée en $x$ et soit $c' = (U', \psi', E')$ une carte de $Y$ centrée en $y$; soit $\tilde{\varphi}$ l’expression de $\varphi$ dans ces cartes (5.3.2), et soit $\tilde{\varphi}_*$ l’application correspondante de $TS^{(r)}(E)$ dans $TS^{(r)}(E')$, cf. 13.1.4. Il existe une application linéaire et une seule, notée $T_x^{(r)}(\varphi)$ ou $\varphi_*$, de $T_x^{(r)}(X)$ dans $T_y^{(r)}(Y)$, rendant commutatif le diagramme

$$
\begin{array}{ccc}
TS^{(r)}(E) & \xrightarrow{\tilde{\varphi}_*} & TS^{(r)}(E') \\
\downarrow_{\theta_c} & & \downarrow_{\theta_c} \\
T_x^{(r)}(X) & \xrightarrow{\varphi_*} & T_y^{(r)}(Y).
\end{array}
$$

Cette application ne dépend pas du choix de $c$ et $c'$. Si $t \in T_x^{(r)}(X)$, on dit que $\varphi_*(t)$ est l’*image* de $t$ par $\varphi$. On a $\varphi_*(\varepsilon_x) = \varepsilon_y$. Si $k \leq r$, on a
$$
\varphi_*(T_x^{(k)}(X)) \subset T_y^{(k)}(Y) \quad \text{et} \quad \varphi_*(T_x^{(k)+}(X)) \subset T_y^{(k)+}(Y).
$$

Si $\varphi' : X \to Y$ est un morphisme de classe $C^r$ appliquant $x$ sur $y$, on a $\varphi_* = \varphi'_*$ si et seulement si $j_x^r(\varphi) = j_x^r(\varphi')$, cf. 12.1.

Si $\varphi$ est une immersion (resp. une submersion) en $x$, $\varphi_*$ est injectif (resp. surjectif); la réciproque est vraie si $\dim_y Y < +\infty$.

Si $\varphi' : Y \to Z$ est un morphisme de variétés de classe $C^r$, et si $t \in T_x^{(r)}(X)$, on a $(\varphi' \circ \varphi)_*(t) = \varphi'_*(\varphi_*(t))$.

Soit $F$ un espace polynormé séparé, et soit $f$ une fonction de classe $C^r$ à valeurs dans $F$, définie dans un voisinage de $y$. On a alors
$$(1)$$
$$
\langle f, \varphi_*(t) \rangle = \langle f \circ \varphi, t \rangle \quad \text{pour tout } t \in T_x^{(r)}(X).
$$
Pour $t$ donné, les relations (1) (pour $f$ et $F$ variables) *caractérisent* $\varphi_*(t)$; lorsque $\dim_y Y < +\infty$, on peut se borner à $F = K$.

13.2.4. Supposons que $X$ soit une sous-variété ouverte d’un *espace de Banach* $E$. Notons $\varphi_x$ l’application $y \mapsto y - x$ de $X$ dans $E$; la carte $c = (X, \varphi_x, E)$ est centrée

¹ Lorsque $K = \mathbf{R}$ ou $\mathbf{C}$ et que $X$ est localement compacte, la formule précédente conduit à identifier la distribution ponctuelle $\varepsilon_x$ à la *mesure de Dirac* $\varepsilon_x$ définie en JNT, III, § 1, n° 3. Plus généralement, toute mesure à support fini dans $X$ s’identifie à une distribution à support fini au sens du n° 13.6.

en $x$. On identifie alors $T_x^{(r)}(X)$ à $TS^{(r)}(E)$ au moyen de $\theta_c^{-1}$; en particulier, on a $T_x^{(\infty)}(X) = TS(E)$.

Soit $F$ un espace de Banach, soit $u : E \to F$ une application linéaire continue, et soient $x \in E, y \in F$ tels que $u(x) = y$. Identifions comme ci-dessus $T_x^{(\infty)}(E)$ à $TS(E)$ et $T_y^{(\infty)}(F)$ à $TS(F)$. L’application
$$
u_* : TS(E) \to TS(F) \quad (\text{cf. } 13.2.3)
$$
coincide avec l’application $TS(u)$ induite par le prolongement canonique de $u$ à l’algèbre tensorielle.

13.2.5. Si $k \leq r$, on note $T^{(k)}(X)$ (resp. $T^{(k)+}(X)$) l’ensemble somme des $T_a^{(k)}(X)$ (resp. des $T_a^{(k)+}(X)$) pour $a \in X$. Une application $t : X \to T^{(k)}(X)$ telle que $t(a) \in T_a^{(k)}(X)$ pour tout $a \in X$ s’appelle un champ de distributions ponctuelles d’ordre $\leq k$.

Supposons $k$ fini et $X$ localement de dimension finie. Pour tout $a \in X$, la forme bilinéaire $(j, t) \mapsto \langle j, t \rangle$ (cf. 13.2.2) définit un isomorphisme $i_a$ de $T_a^{(k)}(X)$ sur le dual $P_a^k(X)^*$ de $P_a^k(X)$. Les $i_a$ définissent une bijection $i : T^{(k)}(X) \to P^k(X)^*$, où $P^k(X)^*$ désigne le dual du fibré vectoriel $P^k(X)$; par transport de structure au moyen de $i^{-1}$, on munit $T^{(k)}(X)$ d’une structure de fibré vectoriel de base $X$ et de classe $C^{r-k}$. Un champ de distributions ponctuelles d’ordre $\leq k$ est dit de classe $C^s$, avec $s \leq r - k$, si c’est une section de classe $C^s$ du fibré $T^{(k)}(X)$.

Soit $\varphi : X \to Y$ un morphisme de variétés de classe $C^r$ et supposons que $Y$ soit, comme $X$, localement de dimension finie. Alors $\varphi_* : T^{(k)}(X) \to T^{(k)}(Y)$ est un $\varphi$-morphisme de fibrés vectoriels de classe $C^{r-k}$.

13.2.6. Soit $k$ un entier tel que $0 \leq k \leq r$. Si $U$ est un ouvert d’un espace de Banach $E$ de dimension finie, le fibré vectoriel $T^{(k)}(U)$ s’identifie, grâce à 13.2.4, au fibré trivial de fibre $TS^{(k)}(E)$.

Prenons en particulier $E = K^n$, avec $n \geq 0$, et soit $(e_1, \ldots, e_n)$ la base canonique de $E$. Si $\alpha = (\alpha_1, \ldots, \alpha_n)$ est un élément de $\mathbf{N}^n$, notons $\Delta^\alpha$ l’élément $\gamma_{\alpha_1}(e_1) \ldots \gamma_{\alpha_n}(e_n)$ de $TS(E)$ (le produit utilisé étant le produit symétrique des tenseurs symétriques, cf. A, IV, § 5, n° 3).(1) Les $\Delta^\alpha$, pour $|\alpha| \leq k$, forment une base de $TS^{(k)}(E)$; si $a \in K^n$, on note $\Delta_a^\alpha$ les éléments correspondants de $T_a^{(k)}(E)$. Soient $F$ un espace polynormé séparé, et $f$ une fonction de classe $C^r$, à valeurs dans $F$, définie au voisinage de $a$; si $\alpha \in \mathbf{N}^n$, l’élément $\langle f, \Delta_a^\alpha \rangle$ coïncide avec l’élément $(\Delta^\alpha f)(a)$ défini en 2.5.3, 3.2.1 et 4.2.1.

Supposons $X$ localement de dimension finie, et soit $\xi = (\xi^1, \ldots, \xi^n)$ un système de coordonnées de $X$ dans un ouvert $U$. Si $a \in U$ et si $\alpha$ est un multi-indice tel que $|\alpha| \leq k$, on note $(\Delta_\xi^\alpha)_a$ la distribution ponctuelle en $a$ dont l’image par $\xi$ est la distribution ponctuelle $\Delta_{\xi(a)}^\alpha$ sur $K^n$; les champs de distributions
$$
\Delta_\xi^\alpha : a \mapsto (\Delta_\xi^\alpha)_a \quad (|\alpha| \leq k)
$$
forment un repère sur $U$ du fibré vectoriel $T^{(k)}(X)$. Si $f : U \to F$ est de classe $C^r$, on pose $\langle f, (\Delta_\xi^\alpha)_a \rangle = \Delta_\xi^\alpha f(a)$ et l’on note $\Delta_\xi^\alpha f$ la fonction $a \mapsto \Delta_\xi^\alpha f(a)$; c’est une fonction de classe $C^{r-k}$ dans $U$.

(1) Si $m = |\alpha|$ et si $\Sigma$ est l’ensemble des applications $\sigma$ de $\{1, \ldots, m\}$ dans $\{1, \ldots, n\}$ telles que $\mathrm{Card}\, \sigma^{-1}(i) = \alpha_i$, on a
$$
\Delta^\alpha = \gamma_{\alpha_1}(e_1) \ldots \gamma_{\alpha_n}(e_n) = \sum_{\sigma \in \Sigma} e_{\sigma(1)} \otimes \cdots \otimes e_{\sigma(n)}, \quad \text{cf. A, IV, § 5, n° 4.}
$$

### 13.3. Distributions ponctuelles et espaces tangents

Dans ce no, X désigne une variété de classe $C^r$.

### 13.3.1. Soit $x \in X$ et soit $k$ un entier $\leq r$. Soit $c=(U,\varphi,E)$ une carte de $X$ centrée en $x$; l’isomorphisme $\theta_c:T^S(X)(E)\to T_x(X)$ défini en 13.2.1 applique $T^S{}^{(k)}(E)$ sur $T_x^{(k)}(X)$ et $T^S{}^{(k-1)}(E)$ sur $T_x^{(k-1)}(X)$; par restriction et passage au quotient, il induit un isomorphisme

$$
\theta_{c,k}:T^S{}^{(k)}(E)=T^S{}^{(k)}(E)/T^S{}^{(k-1)}(E)\longrightarrow T_x^{(k)}(X)/T_x^{(k-1)}(X).
$$

D’autre part, $c$ définit un isomorphisme, déjà noté $\theta_c$, de $E$ sur l’espace tangent $T_x(X)$, cf. 5.5.1. Notons $i_k$ le composé

$$
T_x^{(k)}(X)/T_x^{(k-1)}(X)\xrightarrow{\theta_{c,k}^{-1}}T^S{}^{(k)}(E)\xrightarrow{T^S(\theta_c)}T^S{}^{(k)}(T_x(X)).
$$

L’isomorphisme $i_k$ est indépendant du choix de $c$; pour $k=1$, on l’utilise pour identifier $T_x^{(1)}(X)=T_x^{(1)}(X)/T_x^{(0)}(X)$ à l’espace tangent $T_x(X)$. Si $t\in T_x^{(k)}(X)$, on se permet de noter $i_k(t)$ l’image par $i_k$ de la classe de $t$ modulo $T_x^{(k-1)}(X)$.

Posons

$$
\operatorname{gr}_k T_x^{(r)}(X)=T_x^{(k)}(X)/T_x^{(k-1)}(X)
$$

et

$$
\operatorname{gr}T_x^{(r)}(X)=\bigoplus_{0\leq k\leq r}\operatorname{gr}_k T_x^{(r)}(X).
$$

On dit que $\operatorname{gr}T_x^{(r)}(X)$ est le gradué associé à la filtration croissante $(T_x^{(k)}(X))_{k\leq r}$ de $T_x^{(r)}(X)$. Les $i_k$ définissent un isomorphisme d’espaces vectoriels gradués

$$
i:\operatorname{gr}T_x^{(r)}(X)\longrightarrow T^S{}^{(r)}(T_x(X)).
$$

Si $r=\infty$ ou $\omega$, $i$ est un isomorphisme de $\operatorname{gr}T_x^{(r)}(X)$ sur $T^S(T_x(X))$. Lorsque l’on désire préciser $x$ (ou $X$, ou les deux), on écrit $i_x$ (ou $i_X$, ou $i_{x,X}$) à la place de $i$.

### 13.3.2. Outre les hypothèses ci-dessus, supposons que $X$ soit localement de dimension finie. Les isomorphismes $i_k$ relatifs aux différents points de $X$ définissent un isomorphisme de fibrés vectoriels

$$
i_k:T^{(k)}(X)/T^{(k-1)}(X)\longrightarrow TS^{(k)}(T(X))
$$

où $TS^{(k)}(T(X))$ désigne le fibré vectoriel de classe $C^{r-1}$ déduit de $T(X)$ par le foncteur vectoriel en dimension finie $TS^{(k)}$ (cf. 7.6.5). Pour $k\geq 1$, $i_k$ est un isomorphisme de classe $C^{r-k}$; pour $k=0$, c’est l’application identique du fibré trivial $K_X$.

### 13.3.3. **Exemple.** — Les hypothèses étant comme ci-dessus, soit $\xi=(\xi^1,\ldots,\xi^n)$ un système de coordonnées de $X$ en $x$. Notons $(\partial_i)_{1\leq i\leq n}$ la base de $T_x(X)$ définie par $\xi$ (cf. 5.5.8) et notons $(\Delta^\alpha_x)_{|\alpha|\leq k}$ celle de $T_x^{(k)}(X)$ définie en 13.2.6. On a :

$$
i_k(\Delta^\alpha_x)=0 \qquad \text{si } |\alpha|<k
$$

$$
i_k(\Delta^\alpha_x)=\gamma_{\alpha_1}(\partial_1,x)\cdots\gamma_{\alpha_n}(\partial_n,x)
\qquad \text{si } |\alpha|=k.
$$

[^1]

13.3.4. Supposons que K soit de caractéristique zéro ou que X soit localement de dimension finie. Soit k un entier tel que $0 \leq k \leq r$ et soit $x \in X$; soit F un espace de Banach. D’après 12.6.8, on a une suite exacte

(i)
$$
0 \to P_k(T_x(X); F) \xrightarrow{i} P_x^k(F_X) \xrightarrow{\sigma} P_x^{k-1}(F_X) \to 0,
$$
avec $\sigma = r^{k, k-1}$. D’autre part, d’après 13.3.1, on a une suite exacte

(ii)
$$
0 \leftarrow TS^k(T_x(X)) \xleftarrow{i} T_x^{(k)}(X) \xleftarrow{s} T_x^{(k-1)}(X) \leftarrow 0,
$$
où s est l’inclusion de $T_x^{(k-1)}(X)$ dans $T_x^{(k)}(X)$ et $i = i_k$. Ces suites exactes sont « accouplées dans F ». Plus précisément, écrivons-les sous la forme:

(i)
$$
0 \to A \xrightarrow{i} B \xrightarrow{\sigma} C \to 0
$$

(ii)
$$
0 \leftarrow A' \xleftarrow{i} B' \xleftarrow{s} C' \leftarrow 0.
$$

Si $a \in A$ et $a' \in A'$, l’élément $\langle a, a' \rangle$ de F est défini par 13.1.2; si $b \in B$ et $b' \in B'$, (resp. si $c \in C$ et $c' \in C'$), l’élément $\langle b, b' \rangle$ (resp. $\langle c, c' \rangle$) de F est défini par 13.2.2; on a alors:
$$
\langle ia, b' \rangle = \langle a, ib' \rangle \quad \text{et} \quad \langle \sigma b, c' \rangle = \langle b, sc' \rangle \quad \text{si} \quad a \in A,\ b \in B,\ b' \in B',\ c' \in C'.
$$

13.3.5. Soit Y une variété de classe $C^r$, soit $\varphi : X \to Y$ un morphisme de classe $C^r$ et soient $x \in X,\ y \in Y$ tels que $y = \varphi(x)$. L’application $\varphi_* : T_x^{(r)}(X) \to T_y^{(r)}(Y)$ définie en 13.2.3 est compatible avec les filtrations de ces espaces; elle définit par passage aux gradués associés une application linéaire
$$
\operatorname{gr}(\varphi_*) : \operatorname{gr}\ T_x^{(r)}(X) \to \operatorname{gr}\ T_y^{(r)}(Y).
$$
Notons d’autre part $TS^{(r)}(T_x(\varphi))$ l’application de $TS^{(r)}(T_x(X))$ dans $TS^{(r)}(T_y(Y))$ induite par le prolongement canonique $TS(T_x(\varphi))$ de $T_x(\varphi)$. Le diagramme

$$
\begin{array}{ccc}
\operatorname{gr}\ T_x^{(r)}(X) & \xrightarrow{\operatorname{gr}(\varphi_*)} & \operatorname{gr}\ T_y^{(r)}(Y) \\
\downarrow^{i_{X,x}} & & \downarrow^{i_{Y,y}} \\
TS^{(r)}(T_x(X)) & \xrightarrow{TS^{(r)}(T_x(\varphi))} & TS^{(r)}(T_y(Y))
\end{array}
$$

est commutatif.

13.3.6. Supposons que K soit de caractéristique zéro. En utilisant les isomorphismes $\varphi_M : S^k(M) \to TS^k(M)$ définis en A, IV, § 5, n° 8, on peut remplacer, dans tout ce qui précède, les $TS^k(T_x(X))$ par les puissances symétriques k-ièmes $S^k(T_x(X))$ de l’espace tangent $T_x(X)$.

### 13.4. Produit tensoriel de distributions ponctuelles

13.4.1. Soient $X_1$ et $X_2$ deux variétés de classe $C^r$, soient $x_1 \in X_1,\ x_2 \in X_2$ et $t_1 \in T_{x_1}^{(k_1)}(X_1),\ t_2 \in T_{x_2}^{(k_2)}(X_2)$ avec $k_1 + k_2 \leq r$. Posons $X = X_1 \times X_2,\ x = (x_1, x_2)$ et k = k_1 + k_2. Pour i = 1, 2, soit c_i = (U_i, \varphi_i, E_i) une carte de X_i centrée en x_i et notons $\tilde{t}_i$ l’élément de TS(E_i) tel que $\theta_c(\tilde{t}_i) = t_i$, cf. 13.2.1. Soit $\sigma$ l’isomorphisme canonique de TS(E_1) $\otimes$ TS(E_2) sur TS(E_1 $\times$ E_2), cf. A, IV, § 5, n° 5. L’élément $\sigma(\tilde{t}_1 \otimes \tilde{t}_2)$ est le produit symétrique de $\tilde{t}_1$ et $\tilde{t}_2$ (identifiés à des éléments de TS(E_1 $\times$ E_2) grâce aux injections canoniques TS(E_i) $\to$ TS(E_1 $\times$ E_2)); il appartient à TS^{(k)}(E_1 $\times$ E_2). Posons $c = c_1 \times c_2$; c’est une carte de X centrée en x. L’image par $\theta_c$ de $\sigma(\tilde{t}_1 \otimes \tilde{t}_2)$ est un élément de T_x^{(k)}(X), qui ne dépend pas du choix des cartes $c_i$. On l’appelle le produit direct, ou le produit tensoriel symétrique (ou même simplement le produit tensoriel) de $t_1$ et $t_2$ et on le note $t_1 \times t_2$ ou $t_1 \otimes t_2$.

On a $\varepsilon_{x_1} \otimes \varepsilon_{x_2} = \varepsilon_x$. Le terme constant de $t_1 \otimes t_2$ est le produit des termes constants de $t_1$ et de $t_2$.

L’isomorphisme $(y_1, y_2) \mapsto (y_2, y_1)$ de $X_1 \times X_2$ sur $X_2 \times X_1$ transforme $t_1 \otimes t_2$ en $t_2 \otimes t_1$.

13.4.2 (« Associativité et fonctorialité »). Soient $X_i$ ($i = 1, 2, 3$) des variétés de classe $C^r$, et soient $x_i \in X_i$, $t_i \in T^{(k_i)}_{x_i}(X_i)$ avec $k_1 + k_2 + k_3 \leq r$. On a
$$
(t_1 \otimes t_2) \otimes t_3 = t_1 \otimes (t_2 \otimes t_3);
$$
on note cette distribution ponctuelle $t_1 \otimes t_2 \otimes t_3$. On définit de même des produits tensoriels finis quelconques.

Soient $\varphi_1 : X_1 \to Y_1$ et $\varphi_2 : X_2 \to Y_2$ des morphismes de variétés de classe $C^r$, et soient $t_1 \in T^{(k_1)}(X_1)$, $t_2 \in T^{(k_2)}(X_2)$ avec $k_1 + k_2 \leq r$. On a
$$
(\varphi_1 \times \varphi_2)_*(t_1 \otimes t_2) = \varphi_{1*}(t_1) \otimes \varphi_{2*}(t_2).
$$

13.4.3. Les notations étant celles de 13.4.1, soient $F_1, F_2$ et F des espaces polynormés séparés, et $(u_1, u_2) \mapsto u_1 . u_2$ une application bilinéaire continue de $F_1 \times F_2$ dans F. Soit
$$
f_i : X_i \to F_i \quad (i = 1, 2)
$$
une application de classe $C^r$, et définissons $f_1 \otimes f_2 : X \to F$ par
$$
(f_1 \otimes f_2)(y_1, y_2) = f_1(y_1) . f_2(y_2).
$$
L’application $f_1 \otimes f_2$ est de classe $C^r$, et l’on a
$$
\langle f_1 \otimes f_2, t_1 \otimes t_2 \rangle = \langle f_1, t_1 \rangle . \langle f_2, t_2 \rangle.
$$

13.4.4. Les notations étant celles de 13.4.1, soit $f$ une application de classe $C^r$ de X dans un espace polynormé séparé F. Si $y_1 \in X_1$, notons $f_{y_1}$ l’application $y_2 \mapsto f(y_1, y_2)$ de $X_2$ dans F et posons $g(y_1) = \langle f_{y_1}, t_2 \rangle$. La fonction $g : X_1 \to F$ ainsi définie est de classe $C^{r - k_1}$, et l’on a
$$
\langle f, t_1 \otimes t_2 \rangle = \langle g, t_1 \rangle,
$$
autrement dit
$$
\langle f, t_1 \otimes t_2 \rangle = \langle y_1 \mapsto \langle y_2 \mapsto f(y_1, y_2), t_2 \rangle, t_1 \rangle.
$$
On a de même
$$
\langle f, t_1 \otimes t_2 \rangle = \langle y_2 \mapsto \langle y_1 \mapsto f(y_1, y_2), t_1 \rangle, t_2 \rangle.
$$

13.4.5. Les notations étant celles de 13.4.1, soit

$$
\alpha_{k_1, k_2} : T^{(k_1)}_{x_1}(X_1) \otimes T^{(k_2)}_{x_2}(X_2) \to T^{(k)}_x(X)
$$

l’application linéaire définie par l’application bilinéaire $(t_1, t_2) \mapsto t_1 \otimes t_2$; cette application est injective; elle est bijective si $k_1$ et $k_2$ sont infinis.

Si $n \leq r$, notons $T^{(n)}_x(X_1, X_2)$ le sous-espace vectoriel de $T^{(n)}_{x_1}(X_1) \otimes T^{(n)}_{x_2}(X_2)$ engendré par les sous-espaces $T^{(k_1)}_{x_1}(X_1) \otimes T^{(k_2)}_{x_2}(X_2)$ pour $k_1 + k_2 \leq n$. Il existe une application linéaire

$$
\alpha_n : T^{(n)}_x(X_1, X_2) \to T^{(n)}_x(X)
$$

et une seule qui prolonge les applications $\alpha_{k_1, k_2}$ définies ci-dessus; c’est un isomorphisme. Dans ce qui suit, on identifie $T^{(n)}_x(X)$, au moyen de $\alpha_n^{-1}$, au sous-espace vectoriel $T^{(n)}_x(X_1, X_2)$ de $T^{(n)}_{x_1}(X_1) \otimes T^{(n)}_{x_2}(X_2)$.

13.4.6. Conservons les notations de 13.4.5 et 13.3.1. Par passage au quotient, $\alpha_{k_1, k_2}$ définit une application linéaire

$$
\varepsilon_{k_1, k_2} : \operatorname{gr}_{k_1} T^{(r)}_{x_1}(X_1) \otimes \operatorname{gr}_{k_2} T^{(r)}_{x_2}(X_2) \to \operatorname{gr}_k T^{(r)}_x(X).
$$

Les applications $\varepsilon_{k_1, k_2}$ ($k_1 + k_2 \leq r$) sont les composantes d’une application linéaire graduée de degré zéro

$$
\varepsilon : \bigoplus_{k_1 + k_2 \leq r} (\operatorname{gr}_{k_1} T^{(r)}_{x_1}(X_1) \otimes \operatorname{gr}_{k_2} T^{(r)}_{x_2}(X_2)) \to \bigoplus_{k \leq r} \operatorname{gr}_k T^{(r)}_x(X)
$$

qui est un isomorphisme. Le diagramme

$$
\begin{array}{ccc}
\bigoplus_{k_1 + k_2 \leq r} (\operatorname{gr}_{k_1} T^{(r)}_{x_1}(X_1) \otimes \operatorname{gr}_{k_2} T^{(r)}_{x_2}(X_2)) & \xrightarrow{\varepsilon} & \operatorname{gr} T^{(r)}_x(X) \\
\downarrow i_{12} & & \downarrow i_X \\
\bigoplus_{k_1 + k_2 \leq r} (\mathrm{TS}^{k_1}(T_{x_1}(X_1)) \otimes \mathrm{TS}^{k_2}(T_{x_2}(X_2))) & \xrightarrow{\sigma} & \bigoplus_{k \leq r} \mathrm{TS}^k(T_{x_1}(X_1) \times T_{x_2}(X_2))
\end{array}
$$

est commutatif (dans ce diagramme, $i_{12}$ désigne l’homomorphisme induit par $i_{x_1} \otimes i_{x_2}$ et $\sigma$ est l’isomorphisme défini en A, IV, § 5, n° 5). Si $r$ est infini, ce diagramme s’écrit simplement:

$$
\begin{array}{ccc}
\operatorname{gr} T^{(\infty)}_{x_1}(X_1) \otimes \operatorname{gr} T^{(\infty)}_{x_2}(X_2) & \xrightarrow{\varepsilon} & \operatorname{gr} T^{(\infty)}_x(X) \\
\downarrow i_{x_1} \otimes i_{x_2} & & \downarrow i_X \\
\mathrm{TS}(T_{x_1}(X_1)) \otimes \mathrm{TS}(T_{x_2}(X_2)) & \xrightarrow{\sigma} & \mathrm{TS}(T_x(X)).
\end{array}
$$

### 13.5. Coproduits

Dans ce numéro, $X$ désigne une variété de classe $C^r$ et $x$ un point de $X$.

13.5.1. Soit $k \leq r$. Si $\Delta$ est l’application diagonale $y \mapsto (y, y)$ de $X$ dans $X \times X$, alors $\Delta_*$ applique $T^{(k)}_x(X)$ dans $T^{(k)}_{(x,x)}(X \times X)$, qui est un sous-espace vectoriel de

$T^{(k)}_x(X)\otimes T^{(k)}_x(X)$, cf. 13.4.5. On obtient ainsi une application linéaire, notée encore $\Delta_*$ (ou $c$) :

$$
T^{(k)}_x(X)\longrightarrow T^{(k)}_x(X)\otimes T^{(k)}_x(X);
$$

on l’appelle le coproduct attaché à $T^{(k)}_x(X)$. Muni de ce coproduct, $T^{(k)}_x(X)$ est une cogèbre coassociative et cocommutative (A, III, p. 144-145); elle admet pour counité la forme linéaire qui associe à une distribution ponctuelle son terme constant (13.2.1).
Si $k'\leq k$, l’inclusion de $T^{(k')}_x(X)$ dans $T^{(k)}_x(X)$ est un morphisme de cogèbres.
Si $c=(U,\varphi,\overline{E})$ est une carte de $X$ centrée en $x$, l’isomorphisme

$$
\theta_c:T^{(k)}(E)\longrightarrow T^{(k)}_x(X)
$$

est un isomorphisme de cogèbres, $T^{(k)}(E)$ étant muni du coproduit induit par celui de $T(E)$, cf. A, IV, § 5, no 7.
Si $\varphi:X\longrightarrow Y$ est un morphisme de variétés de classe $C^r$, l’application de $T^{(k)}(X)$ dans $T^{(k)}_{\varphi(x)}(Y)$ induite par $\varphi_*$ est un morphisme de cogèbres.

### 13.5.2. Soient $F_1$, $F_2$ et $F$ des espaces polynomés séparés, et $(u_1,u_2)\mapsto u_1.u_2$ une application bilinéaire continue de $F_1\times F_2$ dans $F$. Soit $t\in T^{(r)}_x(X)$ et soit

$$
c(t)=\sum_j u_j\otimes v_j\quad(u_j,v_j\text{ dans }T^{(r)}_x(X))
$$

son image par le coproduct. Soient $f_i:X\longrightarrow F_i$ $(i=1,2)$ des applications de classe $C^r$. On a

$$
\langle f_1.f_2,t\rangle=\sum_j\langle f_1,u_j\rangle\langle f_2,v_j\rangle,
$$

ce que l’on écrit, par abus de notation:

$$
\langle f_1.f_2,t\rangle=\langle f_1\otimes f_2,c(t)\rangle.
$$

### 13.5.3. Soit $t\in T^{(k)}_x(X)$, où $k\leq r$.

a) Pour que $c(t)=t\otimes 1$, il faut et il suffit que $t$ soit égal à $0$ ou à $\varepsilon_x$.

b) Pour que $c(t)=1\otimes t+\varepsilon_x\otimes t$, il faut et il suffit que $t$ soit un vecteur tangent, i.e. que l’on ait $t\in T^{(1)}_x(X)$.

### 13.6. Distributions à support fini

### 13.6.1. Soit $X$ une variété de classe $C^r$, et soit $k\leq r$. On note $\mathscr{T}^{(k)}(X)$ la somme directe des espaces $T^{(k)}_x(X)$, pour $x\in X$. Un élément de $\mathscr{T}^{(k)}(X)$ est appelé une distribution à support fini sur $X$, d’ordre $\leq k$. Si $f:X\longrightarrow F$ est une fonction de classe $C^r$ à valeurs dans un espace polynomé séparé $F$, et si

$$
t=\sum_{x\in X}t_x,
$$

où $t_x\in T^{(k)}_x(X)$ pour tout $x\in X$ est une distribution à support fini, on pose

$$
\langle f,t\rangle=\sum_{x\in X}\langle f,t_x\rangle.
$$

De même, on pose

$$
c(t)=\sum_{x\in X}c(t_x),
$$

ce qui munit $\mathscr{T}^{(k)}(X)$ d’une structure de cogèbre coassociative, cocommutative, et possédant une counité $t\mapsto\langle1,t\rangle$. Les inclusions

$$
\mathscr{T}^{(k')}(X)\longrightarrow\mathscr{T}^{(k)}(X),
$$

où $k'\leq k$, sont des morphismes de cogèbres.

Si $\varphi : X \to Y$ est un morphisme de variétés de classe $C^r$, les applications $T_x^{(k)}(\varphi) : T_x^{(k)}(X) \to T_{\varphi(x)}^{(k)}(Y)$ relatives aux divers points $x$ de $X$ définissent une application linéaire $\varphi_*$ de $\mathscr{T}^{(k)}(X)$ dans $\mathscr{T}^{(k)}(Y)$, qui est un morphisme de cogèbres.

Si $X_1$ et $X_2$ sont deux variétés de classe $C^r$, les applications $\alpha_k^{-1}$ (cf. 13.4.5) définissent une application linéaire
$$
\mathscr{T}^{(k)}(X_1 \times X_2) \to \mathscr{T}^{(k)}(X_1) \otimes \mathscr{T}^{(k)}(X_2)
$$
qui est injective; c'est un morphisme de cogèbres. Si $k = \infty$ ou $\omega$, c'est un isomorphisme de cogèbres.

13.6.2. Soit $X$ une variété de classe $C^r$, et soit $V$ un $K$-espace vectoriel de dimension finie. Un élément de $\mathscr{T}^{(r)}(X) \otimes V$ s'appelle une distribution à support fini sur $X$ à valeurs dans $V$. Lorsque $K = \mathbf{R}$, $V = \mathbf{C}$, une telle distribution est également appelée une distribution complexe à support fini sur $X$. Les définitions et résultats des n°s précédents s'étendent aussitôt, par linéarité, aux distributions à valeurs dans $V$.

### 13.7. Affaiblissement de structure

On suppose $K = \mathbf{R}$. Soit $r' \in \mathbf{N}_K$ tel que $r' \leq r$. Soit $X$ une variété de classe $C^r$, et soit $X'$ la variété de classe $C^{r'}$ obtenue par affaiblissement de structure (5.13.1). Soit $x \in X$, et soit $t \in T_x^{(k)}(X)$, avec $k \leq r'$. Choisissons une carte $c = (U, \varphi, E)$ de $X$ centrée en $x$, et soit $\tilde{t}$ l'élément de $TS^{(k)}(E)$ tel que $\theta_c(\tilde{t}) = t$. Comme $c$ est une carte de $X'$ centrée en $x$, l'élément $t' = \theta_c(\tilde{t})$ de $T_x^{(k)}(X')$ est défini; il ne dépend pas du choix de $c$. L'application $t \mapsto t'$ est une bijection de $T_x^{(k)}(X)$ sur $T_x^{(k)}(X')$ par laquelle on identifie ces deux espaces. Les identifications ainsi obtenues sont compatibles avec les opérations $\langle f, t \rangle, \varphi_*(t), t_1 \otimes t_2, c(t), \ldots$ des n°s précédents.

[^1]: Ici encore, le produit des $\gamma_{\alpha_i}(\partial_i,x)$ est un produit symétrique dans $TS(T_x(X))$.
