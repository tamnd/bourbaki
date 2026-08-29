---
book: evt
book_title: Topological Vector Spaces
chapter: V
chapter_title: ESPACES HILBERTIENS (THÉORIE ÉLÉMENTAIRE)
section: 3
section_title: Produit tensoriel d’espaces hilbertiens
lang: fr
source: evt-i-v-fr
book_pages: EVT V.25-EVT V.37, EVT V.72
pdf_pages: 0287-0299, 0334-0334
extraction: ocr
subsections:
    - "no": 1
      title: Produit tensoriel d’espaces préhilbertiens
      page: 25
      pdf_page: 287
    - "no": 2
      title: Produit tensoriel hilbertien d’espaces hilbertiens
      page: 28
      pdf_page: 290
    - "no": 3
      title: Puissances symétriques hilbertiennes
      page: 29
      pdf_page: 291
    - "no": 4
      title: Puissances extérieures hilbertiennes
      page: 33
      pdf_page: 295
    - "no": 5
      title: Multiplication extérieure
      page: 35
      pdf_page: 297
statements: 19
exercises: 2
content_sha256: e0bde61bd2ef5221c91f98a1a93655e2dfe09109667defb62d5d7f6085ea0b7e
---

## § 3. PRODUIT TENSORIEL D’ESPACES HILBERTIENS

### 1. Produit tensoriel d’espaces préhilbertiens

Soient $E_1$ et $E_2$ deux espaces préhilbertiens, et soit $F = E_1 \otimes E_2$ le produit tensoriel des espaces vectoriels $E_1$ et $E_2$. Soient $x_1 \in E_1$ et $x_2 \in E_2$; comme l’application $(y_1, y_2) \mapsto \langle x_1 | y_1 \rangle \langle x_2 | y_2 \rangle$ de $E_1 \times E_2$ dans $K$ est bilinéaire, il existe une forme linéaire $\varphi_{x_1, x_2}$ sur $E_1 \otimes E_2$ telle que

$$
\varphi_{x_1, x_2}(y_1 \otimes y_2) = \langle x_1 | y_1 \rangle \langle x_2 | y_2 \rangle
$$

pour $y_1 \in E_1$ et $y_2 \in E_2$. Soit $z \in F$. L’application $(x_1, x_2) \mapsto \overline{\varphi_{x_1, x_2}(z)}$ de $E_1 \times E_2$ dans $K$ est bilinéaire ; cela se voit en écrivant $z$ sous la forme $z = \sum_{i=1}^n y_{i,1} \otimes y_{i,2}$ avec $y_{i,1} \in E_1$ et $y_{i,2} \in E_2$ pour $1 \leq i \leq n$. Il existe donc une forme linéaire $\psi_z$ sur $F = E_1 \otimes E_2$ telle que

$$
\psi_z(x_1 \otimes x_2) = \overline{\varphi_{x_1, x_2}(z)} \quad (x_1 \in E_1, x_2 \in E_2).
$$

On pose $\Phi(z, t) = \psi_z(t)$ pour $z, t$ dans $F$. On voit aussitôt que $\Phi$ est une forme sesquilinéaire sur $E_1 \otimes E_2$ caractérisée par

$$
\Phi(x_1 \otimes x_2, y_1 \otimes y_2) = \langle x_1 | y_1 \rangle \langle x_2 | y_2 \rangle
$$

(cf. A, IX, § 1, no 11).

#### Proposition 1 {#evt-v-s3-prop-1 .statement}

La forme sesquilinéaire $\Phi$ sur $E_1 \otimes E_2$ est hermitienne et positive, donc munit $E_1 \otimes E_2$ d’une structure d’espace préhilbertien. Cet espace est séparé si $E_1$ et $E_2$ le sont.

La formule $\Phi(z, t) = \overline{\Phi(t, z)}$ résulte de (3) lorsque $z = x_1 \otimes x_2$ et $t = y_1 \otimes y_2$. Le cas général s’en déduit par linéarité, donc $\Phi$ est hermitienne.

Supposons que $E_1$ et $E_2$ soient séparés et prouvons que la forme hermitienne $\Phi$ est positive et séparante. Soit $z = \sum_{i=1}^n x_i \otimes y_i$ un élément non nul de $F = E_1 \otimes E_2$.

Soit $(e_1, ..., e_m)$ une base orthonormale du sous-espace de $E_1$ engendré par $x_1, ..., x_n$ (V, p. 23, cor. 1). Il existe des éléments $f_1, ..., f_m$ non tous nuls de $E_2$ tels que $z = \sum_{i=1}^m e_i \otimes f_i$, d'où

$$
\Phi(z, z) = \sum_{i,j=1}^m \Phi(e_i \otimes f_i, e_j \otimes f_j)
$$
$$
= \sum_{i,j} \langle e_i|e_j \rangle \langle f_i|f_j \rangle = \sum_{i=1}^m \|f_i\|^2 > 0.
$$

Revenons au cas général, et prouvons que $\Phi$ est positive. Soient $\tilde{E}_i$ l’espace préhilbertien séparé associé à $E_i$ et $\pi_i$ l’application canonique de $E_i$ sur $\tilde{E}_i$ ($i = 1, 2$). Posons $\pi = \pi_1 \otimes \pi_2$. Soit $\tilde{\Phi}$ la forme hermitienne sur $\tilde{E}_1 \otimes \tilde{E}_2$ construite de manière analogue à $\Phi$. On a évidemment

$$
\Phi(z, t) = \tilde{\Phi}(\pi(z), \pi(t)) \quad (z \in F, t \in F),
$$

et comme $\tilde{\Phi}$ est positive, il en est de même de $\Phi$.

L’espace préhilbertien défini dans la prop. 1 s’appelle le produit tensoriel des espaces préhilbertiens $E_1$ et $E_2$; il se note $E_1 \otimes_2 E_2$. On écrira désormais $\langle z|t \rangle$ pour $\Phi(z, t)$, d’où par définition

$$(4)$$
$$
\langle x_1 \otimes x_2|y_1 \otimes y_2 \rangle = \langle x_1|y_1 \rangle \langle x_2|y_2 \rangle;
$$

on écrit aussi $\|z\|_2$ ou $\|z\|$ pour $\langle z|z \rangle^{1/2}$. De (4), on déduit

$$(5)$$
$$
\|x_1 \otimes x_2\|_2 = \|x_1\| \cdot \|x_2\|,
$$

de sorte que l’application bilinéaire $(x_1, x_2) \mapsto x_1 \otimes x_2$ de $E_1 \times E_2$ dans $E_1 \otimes_2 E_2$ est continue.

Pour $i = 1, 2$, soit $F_i$ un sous-espace vectoriel de $E_i$, muni de la structure d’espace préhilbertien induite. Alors $F_1 \otimes F_2$ s’identifie à un sous-espace vectoriel de $E_1 \otimes E_2$ (A, II, p. 108). La formule (4) montre que $F_1 \otimes F_2$, muni de la structure d’espace préhilbertien induite par celle de $E_1 \otimes_2 E_2$, n’est autre que $F_1 \otimes_2 F_2$. Nous identifierons désormais $F_1 \otimes_2 F_2$ à un sous-espace préhilbertien de $E_1 \otimes_2 E_2$.

#### Proposition 2 {#evt-v-s3-prop-2 .statement}

*Pour $i = 1, 2$, soient $E_i$ et $F_i$ deux espaces préhilbertiens séparés et $u_i \in \mathcal{L}(E_i; F_i)$. L’application linéaire $u_1 \otimes u_2$ de $E_1 \otimes_2 E_2$ dans $F_1 \otimes_2 F_2$ est continue et l’on a*

$$
\|u_1 \otimes u_2\| = \|u_1\| \cdot \|u_2\|.
$$

Considérons sur $E_1$ la forme hermitienne positive

$$
f(x_1, y_1) = \|u_1\|^2 \langle x_1|y_1 \rangle - \langle u_1(x_1)|u_1(y_1) \rangle.
$$

D’après la prop. 1 (V, p. 25), il existe une forme hermitienne positive $\Phi$ sur $E_1 \otimes E_2$ telle que l’on ait
$$
\Phi(x_1 \otimes x_2, y_1 \otimes y_2) = f(x_1, y_1) \langle x_2 | y_2 \rangle =
= \|u_1\|^2 \langle x_1 \otimes x_2 | y_1 \otimes y_2 \rangle - \langle (u_1 \otimes 1)(x_1 \otimes x_2)| (u_1 \otimes 1)(y_1 \otimes y_2) \rangle
$$
pour $x_1, y_1$ dans $E_1$ et $x_2, y_2$ dans $E_2$. Par linéarité, on a donc
$$
\Phi(z, t) = \|u_1\|^2 \langle z | t \rangle - \langle (u_1 \otimes 1)(z)|(u_1 \otimes 1)(t) \rangle
$$
pour $z, t$ dans $E_1 \otimes E_2$. Comme $\Phi$ est positive, on a $\Phi(z, z) \geq 0$, c’est-à-dire $\|(u_1 \otimes 1).z\|_2 \leq \|u_1\|. \|z\|_2$ pour $z \in E_1 \otimes_2 E_2$, d’où $\|u_1 \otimes 1\| \leq \|u_1\|$. On prouve de même l’inégalité $\|1 \otimes u_2\| \leq \|u_2\|$, et comme on a $u_1 \otimes u_2 = (u_1 \otimes 1) \circ (1 \otimes u_2)$, on a donc
$$
\|u_1 \otimes u_2\| \leq \|u_1\| \cdot \|u_2\| .
$$
D’autre part, on a
$$
\|u_1\| \cdot \|u_2\| = \sup_{\|x_1\| \leq 1, \|x_2\| \leq 1} \|u_1(x_1)\| \cdot \|u_2(x_2)\|
= \sup_{\|x_1\| \leq 1, \|x_2\| \leq 1} \|(u_1 \otimes u_2)(x_1 \otimes x_2)\|_2 \leq \|u_1 \otimes u_2\|,
$$
ce qui achève la démonstration de la prop. 2. C.Q.F.D.

Soient $E_1, ..., E_n$ des espaces préhilbertiens ($n \geq 2$). On définit par récurrence le produit tensoriel $E_1 \otimes_2 ... \otimes_2 E_n$ (noté aussi $\bigotimes_{i=1}^n E_i$) par
$$
E_1 \otimes_2 ... \otimes_2 E_n = (E_1 \otimes_2 ... \otimes_2 E_{n-1}) \otimes_2 E_n .
$$
On a donc, par définition du produit scalaire,
$$
\langle x_1 \otimes ... \otimes x_n | y_1 \otimes ... \otimes y_n \rangle = \prod_{i=1}^n \langle x_i | y_i \rangle ,
$$
et en particulier $^1$
$$
\|x_1 \otimes ... \otimes x_n\|_2 = \|x_1\| ... \|x_n\| ,
$$
pour $x_i, y_i$ dans $E_i$ ($1 \leq i \leq n$). Si les $E_i$ sont séparés, il en est de même de $E_1 \otimes_2 ... \otimes_2 E_n$.

Soient $F_1, ..., F_n$ des espaces préhilbertiens et $u_i \in \mathcal{L}(E_i; F_i)$ pour $1 \leq i \leq n$. La prop. 2 entraîne par récurrence sur $n$ que $u_1 \otimes ... \otimes u_n$ est une application linéaire continue de $E_1 \otimes_2 ... \otimes_2 E_n$ dans $F_1 \otimes_2 ... \otimes_2 F_n$ et que l’on a
$$
\|u_1 \otimes ... \otimes u_n\| = \|u_1\| ... \|u_n\| .
$$

$^1$ On pose encore $\|z\|_2 = \langle z | z \rangle^{1/2}$ pour $z$ dans $E_1 \otimes_2 ... \otimes_2 E_n$.

Soit $\sigma \in \mathcal{S}_n$ une permutation de l’ensemble $\{1, 2, ..., n\}$. Vu (6), l’application linéaire $p_\sigma$ de $E_1 \otimes_2 ... \otimes_2 E_n$ sur $E_{\sigma^{-1}(1)} \otimes_2 ... \otimes_2 E_{\sigma^{-1}(n)}$ caractérisée par

$$
p_\sigma(x_1 \otimes ... \otimes x_n) = x_{\sigma^{-1}(1)} \otimes ... \otimes x_{\sigma^{-1}(n)}
$$

est un isomorphisme d’espaces préhilbertiens (« commutativité du produit tensoriel »).

De même, considérons une partition de $\{1, 2, ..., n\}$ en $m$ intervalles consécutifs $I_1, ..., I_m$ avec $I_k = [a_k, a_{k+1} - 1]$ pour $1 \leq k \leq m$. Posons

$$
F_k = \bigotimes_{i=a_k}^{a_{k+1}-1} E_i \quad (1 \leq k \leq m).
$$

L’isomorphisme canonique de $F_1 \otimes ... \otimes F_m$ sur $E_1 \otimes ... \otimes E_n$ qui transforme

$$
\bigotimes_{k=1}^m \bigotimes_{i=a_k}^{a_{k+1}-1} x_i
$$

en $x_1 \otimes ... \otimes x_n$ (A, II, p. 72) est un isomorphisme d’espaces préhilbertiens (« associativité du produit tensoriel »).

### 2. Produit tensoriel hilbertien d’espaces hilbertiens

#### Définition 1 {#evt-v-s3-def-1 .statement}

Soient $E_1, ..., E_n$ des espaces hilbertiens. On appelle produit tensoriel hilbertien des $E_i$, et l’on note $E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n$ (ou $\hat{\otimes}_{1 \leq i \leq n} E_i$) le complété de l’espace préhilbertien séparé $E_1 \otimes_2 ... \otimes_2 E_n$.

Soient $F_1, ..., F_n$ des espaces hilbertiens et $u_i \in \mathcal{L}(E_i; F_i)$ pour $1 \leq i \leq n$. L’application linéaire continue $u_1 \otimes ... \otimes u_n$ se prolonge alors en une application linéaire continue $u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n$ de $E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n$ dans $F_1 \hat{\otimes}_2 ... \hat{\otimes}_n F_n$. On a

$$
\|u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n\| = \|u_1\| ... \|u_n\|
$$

d’après la formule (8) de V, p. 27. De plus, si $1_E$ désigne l’application identique de tout espace hilbertien $E$, on a

$$
1_{E_1} \hat{\otimes}_2 ... \hat{\otimes}_2 1_{E_n} = 1_E \quad \text{avec} \quad E = E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n.
$$

Enfin, si $G_1, ..., G_n$ sont des espaces hilbertiens et $v_i \in \mathcal{L}(F_i; G_i)$ pour $1 \leq i \leq n$, on a

$$
(v_1 \circ u_1) \hat{\otimes}_2 ... \hat{\otimes}_2 (v_n \circ u_n) = (v_1 \hat{\otimes}_2 ... \hat{\otimes}_2 v_n) \circ (u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n).
$$

On laisse au lecteur le soin de formuler la « commutativité » et « l’associativité » du produit tensoriel hilbertien, par application de ce qui a été dit ci-dessus pour les espaces préhilbertiens.

#### Remarque {#evt-v-s3-n2-rem-1 .statement}

Soient $E_1, ..., E_n$ des espaces préhilbertiens séparés, et $\hat{E}_1, ..., \hat{E}_n$ leurs complétés respectifs. Alors $E_1 \otimes_2 ... \otimes_2 E_n$ est un sous-espace préhilbertien de $\hat{E}_1 \otimes_2 ... \otimes_2 \hat{E}_n$. Comme l’application $(x_1, ..., x_n) \mapsto x_1 \otimes ... \otimes x_n$ de $\hat{E}_1 \times ... \times \hat{E}_n$ dans $\hat{E}_1 \otimes_2 \ldots \otimes_2 \hat{E}_n$ est continue, $E_1 \otimes_2 \ldots \otimes_2 E_n$ est dense dans $\hat{E}_1 \otimes_2 \ldots \otimes_2 \hat{E}_n$.

\* A fortiori \* le complété de $E_1 \otimes_2 \ldots \otimes_2 E_n$ n’est autre que l’espace hilbertien $\hat{E}_1 \otimes_2 \ldots \otimes_2 \hat{E}_n$. Ce complété se note parfois simplement $E_1 \otimes_2 \ldots \otimes_2 E_n$ (ou $\bigotimes_{1 \leq i \leq n} E_i$).

#### Proposition 3 {#evt-v-s3-prop-3 .statement}

*Soient* $E_1, \ldots, E_n$ *des espaces hilbertiens*. *On suppose que pour* $1 \leq i \leq n$, *l’espace* $E_i$ *est somme hilbertienne d’une famille* $(E_{i,\alpha})_{\alpha \in A(i)}$ *de sous-espaces vectoriels fermés.* *Alors* $E_1 \hat{\otimes}_2 \ldots \hat{\otimes}_2 E_n$ *est somme hilbertienne de la famille des sous-espaces* $E_{1,\alpha_1} \hat{\otimes}_2 \ldots \hat{\otimes}_2 E_{n,\alpha_n}$ *pour* $(\alpha_1, \ldots, \alpha_n)$ *parcourant* $A(1) \times \cdots \times A(n)$.

Vu la formule (6) de V, p. 27, les sous-espaces $E_{1,\alpha_1} \hat{\otimes}_2 \ldots \hat{\otimes}_2 E_{n,\alpha_n}$ de $E_1 \hat{\otimes}_2 \ldots \hat{\otimes}_2 E_n$ sont deux à deux orthogonaux. Pour chaque entier $i$ compris entre 1 et $n$, l’ensemble $\bigcup_{\alpha \in A(i)} E_{i,\alpha}$ est total dans $E_i$, et l’application multilinéaire $(x_1, \ldots, x_n) \mapsto x_1 \otimes \ldots \otimes x_n$ est continue. Il en résulte que la réunion des sous-espaces $E_{1,\alpha_1} \hat{\otimes}_2 \ldots \hat{\otimes}_2 E_{n,\alpha_n}$ est totale, d’où la prop. 3.

#### Corollaire 1 {#evt-v-s3-prop-3-cor-1 .statement}

*Pour* $1 \leq i \leq n$, *soit* $(e_{i,\alpha})_{\alpha \in A(i)}$ *une base orthonormale de* $E_i$. *Alors la famille des vecteurs* $e_{1,\alpha_1} \otimes \ldots \otimes e_{n,\alpha_n}$ *pour* $(\alpha_1, \ldots, \alpha_n)$ *parcourant* $A(1) \times \cdots \times A(n)$, *est une base orthonormale de* $E_1 \hat{\otimes}_2 \ldots \hat{\otimes}_2 E_n$.

#### Corollaire 2 {#evt-v-s3-prop-3-cor-2 .statement}

*Soient* $E_1$ *et* $E_2$ *deux espaces hilbertiens*, *et* $(e_i)_{i \in I}$ *une base orthonormale de* $E_1$. *Soit* $(y_i)_{i \in I}$ *une famille d’éléments de* $E_2$ *telle que* $\sum_{i \in I} \| y_i \|^2 < + \infty$. *Alors la famille* $(e_i \otimes y_i)_{i \in I}$ *est sommable dans* $E_1 \hat{\otimes}_2 E_2$; *de plus tout élément de* $E_1 \otimes E_2$ *s’écrit de manière unique sous la forme* $\sum_{i \in I} e_i \otimes y_i$ *avec* $\sum_{i \in I} \| y_i \|^2 < + \infty$.

Soit $F_i$ la droite de $E_1$ engendrée par $e_i$ ($i \in I$). Alors $E_1$ est somme hilbertienne de la famille des sous-espaces $(F_i)_{i \in I}$. D’après la prop. 3, l’espace $E_1 \hat{\otimes}_2 E_2$ est somme hilbertienne de la famille des sous-espaces $(F_i \hat{\otimes}_2 E_2)_{i \in I}$, d’où le cor. 2.

#### Exemple 1 {#evt-v-s3-n2-exa-1 .statement}

D’après le cor. 1, l’espace $\ell^2(I) \hat{\otimes}_2 \ell^2(J)$ est canoniquement isomorphe à $\ell^2(I \times J)$, le produit tensoriel $x \otimes y$ de $x = (x_i)_{i \in I}$ et $y = (y_j)_{j \in J}$ s’identifiant à la famille $(x_i y_j)_{i \in I, j \in J}$. De même, d’après le cor. 2, $\ell^2(I) \hat{\otimes}_2 E$ s’identifie à $\ell^2_E(I)$, de sorte que l’on ait $(x_i)_{i \in I} \otimes y = (x_i y)_{i \in I}$ pour tout $y$ dans l’espace hilbertien $E$.

#### Exemple 2 {#evt-v-s3-n2-exa-2 .statement}

Soient* $X$ *un espace topologique séparé*, *et* $\mu$ *une mesure positive sur* $X$. *Soit* $E$ *un espace hilbertien*. *On peut identifier canoniquement* $L^2(X, \mu) \hat{\otimes}_2 E$ *à* $L^2_E(X, \mu) : \dot{f}$ *est la classe de la fonction scalaire* $f$ *de carré intégrable sur* $X$, *et si* $a$ *appartient à* $E$, *alors* $f \otimes a$ *est la classe de la fonction* $x \mapsto f(x).a$ *à valeurs dans* $E$.

Soient $Y$ un espace topologique séparé et $v$ une mesure positive sur $Y$. On peut de manière analogue identifier les espaces hilbertiens $L^2(X, \mu) \hat{\otimes}_2 L^2(Y, v)$ et $L^2(X \times Y, \mu \otimes v)$; alors $f \otimes g$ s’identifie à la classe de la fonction $(x, y) \mapsto f(x) g(y)$ sur $X \times Y$. \*

### 3. Puissances symétriques hilbertiennes

Soit $E$ un espace hilbertien, et soit $n$ un entier positif. On notera $\hat{T}^n(E)$ ou $E^{\hat{\otimes} n}$ le produit tensoriel de $n$ espaces hilbertiens égaux à $E$. Autrement dit, $\hat{T}^n(E)$ est le complété de l’espace $\mathbf{T}^n(E) = E \otimes \ldots \otimes E$ ($n$ facteurs) pour la structure d’espace préhilbertien séparé définie par

$$
\langle x_1 \otimes \ldots \otimes x_n | y_1 \otimes \ldots \otimes y_n \rangle = \prod_{i=1}^n \langle x_i | y_i \rangle .
$$

Si $(e_i)_{i \in I}$ est une base orthonormale de $E$, la famille des vecteurs $e_{i_1} \otimes \ldots \otimes e_{i_n}$ pour $i_1, \ldots, i_n$ dans $I$, est une base orthonormale de $\hat{\mathbf{T}}^n(E)$ (V, p. 29, cor. 1). On a $\hat{\mathbf{T}}^0(E) = \mathbf{K}$.

Soit $\sigma \in \mathfrak{S}_n$ une permutation de l’ensemble $\{1, 2, \ldots, n\}$. D’après V, p. 28, il existe un automorphisme $p_\sigma$ de $\hat{\mathbf{T}}^n(E)$ caractérisé par

$$
p_\sigma(x_1 \otimes \ldots \otimes x_n) = x_{\sigma^{-1}(1)} \otimes \ldots \otimes x_{\sigma^{-1}(n)} .
$$

On a $p_{\sigma \tau} = p_\sigma p_\tau$ pour $\sigma, \tau$ dans $\mathfrak{S}_n$, et par suite l’endomorphisme $\Pi_n = \frac{1}{n!} \sum_{\sigma \in \mathfrak{S}_n} p_\sigma$ de l’espace vectoriel $\hat{\mathbf{T}}^n(E)$ est l’orthoprojecteur sur le sous-espace des éléments invariants par $\mathfrak{S}_n$. Par ailleurs (A, III, p. 71), $\Pi_n$ applique le produit tensoriel « algébrique » $\mathbf{T}^n(E)$ sur le sous-espace $\mathbf{TS}^n(E)$ des tenseurs symétriques d’ordre $n$. Autrement dit, l’image de $\Pi_n$ est le complété de l’espace $\mathbf{TS}^n(E)$ muni d’un produit scalaire induit par celui de $\mathbf{T}^n(E)$; on notera $\widehat{\mathbf{TS}}^n(E)$ ce complété.

Soit $\mathbf{S}^n(E)$ la puissance symétrique $n$-ième de l’espace vectoriel $E$ (A, III, p. 67). L’application canonique de $\mathbf{T}^n(E)$ sur $\mathbf{S}^n(E)$ définit par restriction un isomorphisme $\lambda_n$ de $\mathbf{TS}^n(E)$ sur $\mathbf{S}^n(E)$. On vérifie aussitôt que l’isomorphisme réciproque est donné par

$$
\mu_n(x_1 \ldots x_n) = \Pi_n(x_1 \otimes \ldots \otimes x_n) = \frac{1}{n!} \sum_{\sigma \in \mathfrak{S}_n} x_{\sigma^{-1}(1)} \otimes \ldots \otimes x_{\sigma^{-1}(n)}
$$

pour $x_1, \ldots, x_n$ dans $E$.

On définit sur $\mathbf{S}^n(E)$ une structure d’espace préhilbertien séparé en posant

$$
\langle u | v \rangle = n! \langle \mu_n(u) | \mu_n(v) \rangle .
$$

On a donc plus explicitement (comparer avec la formule (29) de A, III, p. 153)

$$
\langle x_1 \ldots x_n | y_1 \ldots y_n \rangle = \sum_{\sigma \in \mathfrak{S}_n} \prod_{i=1}^n \langle x_i | y_{\sigma(i)} \rangle ,
$$

et en particulier

$$
\langle x^n | y^n \rangle = n! \langle x | y \rangle^n .
$$

On note $\hat{\mathbf{S}}^n(E)$ le complété de l’espace préhilbertien $\mathbf{S}^n(E)$ et $\hat{\mathbf{S}}(E)$ la somme hilbertienne externe des espaces hilbertiens $\hat{\mathbf{S}}^n(E)$. On peut montrer (V, p. 72, exerc. 1) que la multiplication dans l’algèbre $\mathbf{S}(E)$ ne se prolonge pas par continuité à $\hat{\mathbf{S}}(E)$ lorsque $E$ n’est pas réduit à 0.

#### Proposition 4 {#evt-v-s3-prop-4 .statement}

Soit $(e_i)_{i\in I}$ une base orthonormale de l’espace hilbertien $E$. Pour tout $\alpha$ dans $\mathbf{N}^{(I)}$, posons

$$
z_\alpha = \prod_{i\in I} e_i^{\alpha_i}/(\alpha_i!)^{1/2}.
$$

Alors $(z_\alpha)_{\alpha\in\mathbf{N}^{(I)}}$ est une base orthonormale de $\hat{S}(E)$.

Soit $E_0$ le sous-espace vectoriel de $E$ engendré par les vecteurs $e_i$ pour $i$ parcourant $I$. Alors les $z_\alpha$ forment une base de l’espace vectoriel $S(E_0)$ (A, III, p. 75). Or $E_0$ est dense dans $E$, et l’application multilinéaire $(x_1, ..., x_n) \mapsto x_1 ... x_n$ de $E \times \cdots \times E$ dans $S(E)$ est continue pour tout $n \geq 1$; donc $S(E_0)$ est dense dans $S(E)$. Il suffit donc de prouver que la famille des $z_\alpha$ est orthonormale. Remarquons d’abord que $\hat{S}^n(E)$ et $\hat{S}^m(E)$ sont orthogonaux pour $n \neq m$. Il suffit donc de prouver la formule

$$
\langle z_\alpha | z_\beta \rangle = \begin{cases}
1 & \text{si } \alpha = \beta \\
0 & \text{si } \alpha \neq \beta
\end{cases}
$$

lorsque $|\alpha| = \sum_{i\in I} \alpha_i$ et $|\beta| = \sum_{i\in I} \beta_i$ sont égaux à un même entier $n$.

Considérons une partition $(P_i)_{i\in I}$ de l’ensemble $\{1, 2, ..., n\}$ telle que Card $P_i = \alpha_i$ pour tout $i \in I$. Posons $x_k = e_i$ si $k$ appartient à $P_i$, d’où $x_1 ... x_n = \prod_{i\in I} e_i^{\alpha_i}$. On définit de manière analogue $(Q_i)_{i\in I}$ et les $y_k$ de sorte que Card $Q_i = \beta_i$ et $y_1 ... y_n = \prod_{i\in I} e_i^{\beta_i}$.

Comme les $e_i$ sont mutuellement orthogonaux, on a $\langle x_k | y_{\sigma(k)} \rangle = 0$ sauf s’il existe un indice $i \in I$ tel que $k \in P_i$ et $\sigma(k) \in Q_i$. D’après la formule (15), on a donc $\langle x_1 ... x_n | y_1 ... y_n \rangle = 0$ sauf s’il existe une permutation $\sigma \in S_n$ telle que $\sigma(P_i) = Q_i$ pour tout $i \in I$, ce qui entraîne $\alpha = \beta$. On a donc $\langle z_\alpha | z_\beta \rangle = 0$ pour $\alpha \neq \beta$. Le même raisonnement prouve que $\|x_1 ... x_n\|^2$ est égal au nombre des $\sigma \in S_n$ tels que $\sigma(P_i) = P_i$ pour tout $i \in I$, donc à $\prod_{i\in I} \alpha_i!$. On a donc $\|z_\alpha\| = 1$, d’où la proposition.

#### Corollaire {#evt-v-s3-n3-cor-1 .statement}

Supposons que l’espace hilbertien $E$ soit somme directe des sous-espaces orthogonaux $M$ et $N$. L’isomorphisme canonique $g$ de $S(M) \otimes S(N)$ sur $S(E)$ (A, III, p. 73) se prolonge de manière unique en un isomorphisme $h$ d’espaces hilbertiens de $\hat{S}(M) \hat{\otimes}_2 \hat{S}(N)$ sur $\hat{S}(E)$.

Soit $(e_i)_{i\in I}$ (resp. $(f_j)_{j\in J}$) une base orthonormale de l’espace hilbertien $M$ (resp. $N$) et soit $M_0$ (resp. $N_0$) le sous-espace vectoriel de $E$ engendré par les vecteurs $e_i$ (resp. $f_j$). Posons $E_0 = M_0 + N_0$ et notons $g_0$ l’isomorphisme canonique de $S(M_0) \otimes S(N_0)$ sur $S(E_0)$. Posons

$$
z_\alpha = \prod_{i\in I} e_i^{\alpha_i}/(\alpha_i!)^{1/2}, \quad t_\beta = \prod_{j\in J} f_j^{\beta_j}/(\beta_j!)^{1/2}
$$

pour $\alpha \in \mathbf{N}^{(I)}$ et $\beta \in \mathbf{N}^{(J)}$. D’après la prop. 4, on a ainsi défini des bases orthonormales $(z_\alpha)_{\alpha\in\mathbf{N}^{(I)}}$ pour $\hat{S}(M)$, $(t_\beta)_{\beta\in\mathbf{N}^{(J)}}$ pour $\hat{S}(N)$ et $(z_\alpha t_\beta)_{\alpha\in\mathbf{N}^{(I)}, \beta\in\mathbf{N}^{(J)}}$ pour $\hat{S}(E)$. Comme on a $z_\alpha t_\beta = g_0(z_\alpha \otimes t_\beta)$, et que les éléments $z_\alpha \otimes t_\beta$ forment une base orthonormale de $\hat{S}(M) \otimes_2 \hat{S}(N)$ (V, p. 29, cor. 1), on voit que $g_0$ se prolonge en un isomorphisme d’espaces hilbertiens $h : \hat{S}(M) \otimes_2 \hat{S}(N) \to \hat{S}(E)$. On a par construction
$$
h(x_1 \ldots x_m \otimes y_1 \ldots y_n) = x_1 \ldots x_m y_1 \ldots y_n
$$
quels que soient les vecteurs $x_1, \ldots, x_m$ de $M_0$ et les vecteurs $y_1, \ldots, y_n$ de $N_0$. Par continuité, la même relation a encore lieu pour des vecteurs $x_1, \ldots, x_m$ de $M$ et des vecteurs $y_1, \ldots, y_n$ de $N$; autrement dit, $h$ prolonge $g$. L’unicité de $h$ est claire.

Soient $E$ et $F$ deux espaces hilbertiens et $u \in \mathcal{L}(E ; F)$. L’application linéaire $\hat{T}^n(u) = u \otimes_2 \ldots \otimes_2 u$ ($n$ facteurs) de $\hat{T}^n(E)$ dans $\hat{T}^n(F)$ est continue de norme $\|u\|^n$ (V, p. 28, formule (10)). Par ailleurs, les formules (13) et (14) de V, p. 30, montrent qu’il existe un isomorphisme $\varphi_{n,E}$ de $\hat{S}^n(E)$ sur le sous-espace $\widehat{\mathbf{T}\mathbf{S}}^n(E)$ de $\hat{T}^n(E)$ et un seul tel que
$$
\varphi_{n,E}(x_1 \ldots x_n) = \frac{1}{(n!)^{1/2}} \sum_{\sigma \in S_n} x_{\sigma(1)} \otimes \ldots \otimes x_{\sigma(n)} \quad (x_1, \ldots, x_n \text{ dans } E) .
$$
Il existe donc une application linéaire continue $\hat{S}^n(u)$ de $\hat{S}^n(E)$ dans $\hat{S}^n(F)$ et une seule qui rende commutatif le diagramme

$$
\begin{array}{ccc}
\hat{S}^n(E) & \xrightarrow{\varphi_{n,E}} & \hat{T}^n(E) \\
\hat{S}^n(u) \downarrow & & \downarrow \hat{T}^n(u) \\
\hat{S}^n(F) & \xrightarrow{\varphi_{n,F}} & \hat{T}^n(F)
\end{array}
$$

Prouvons la formule
$$
\| \hat{S}^n(u) \| = \| u \|^n .
$$
D’une part, on a $\| \hat{S}^n(u) \| \leq \| \hat{T}^n(u) \| = \| u \|^n$. Par ailleurs, pour tout $x \in E$, on a $\hat{S}^n(u)(x^n) = u(x)^n$, $\| x^n \| = (n!)^{1/2} \| x \|^n$ et $\| u(x)^n \| = (n!)^{1/2} \| u(x) \|^n$, d’où
$$
\| \hat{S}^n(u) \| \| x \|^n \geq \| u(x) \|^n ;
$$
on en déduit aussitôt $\| \hat{S}^n(u) \| \geq \| u \|^n$, d’où la formule (19).

Il est clair qu’on a les formules
$$
\hat{S}^n(1_E) = 1_{\hat{S}_n(E)}
$$
$$
\hat{S}^n(v \circ u) = \hat{S}^n(v) \circ \hat{S}^n(u) \quad \text{pour} \quad v \in \mathcal{L}(F ; G) .
$$
Enfin, $\hat{S}^n(u)$ coïncide sur $S^n(E)$ avec l’application linéaire $S^n(u) : S^n(E) \to S^n(F)$ définie en A, III, p. 69 car elle transforme $x_1 \ldots x_n$ en $u(x_1) \ldots u(x_n)$ quels que soient $x_1, \ldots, x_n$ dans $E$.

#### Exemple 1 {#evt-v-s3-n3-exa-1 .statement}

Soient $d \geq 1$ un entier et $\omega$ une fonction positive sur $\mathbf{R}^d$ localement intégrable par rapport à la mesure de Lebesgue $\mu$. Soit $E$ l’espace hilbertien $L^2(\mathbf{R}^d, \omega . \mu )$, et soit $S = S(E)$. Alors $S$ s’identifie à l’espace des suites $f = (f_n)_{n \geq 0}$, où chaque $f_n$ est une fonction sur $(\mathbf{R}^d)^n$ mesurable par rapport à la mesure de Lebesgue $\mu \otimes \ldots \otimes \mu$ ($n$ facteurs) et *invariante* par les permutations des $n$ facteurs dans $(\mathbf{R}^d)^n$, et telles que

$$
\|f\|^2 = \sum_{n=0}^\infty n! \int_{\mathbf{R}^d} \ldots \int_{\mathbf{R}^d} |f_n(x_1, \ldots, x_n)|^2 \omega(x_1) \ldots \omega(x_n) dx_1 \ldots dx_n
$$

soit fini. La norme $\|f\|$ dans $\mathbf{S}$ est définie par la formule (22). L’espace hilbertien $\mathbf{S}$ défini ci-dessus s’appelle l’*espace de Fock symétrique* correspondant au *poids* $\omega$.

#### Exemple 2 {#evt-v-s3-n3-exa-2 .statement}

Soient X un espace topologique séparé, $\mu$ une mesure positive de norme 1 sur X et E un sous-espace hilbertien de l’espace hilbertien réel $L^2_\mathbf{R}(X, \mu)$. On dit que E est un *espace gaussien* si les conditions équivalentes suivantes sont satisfaites :

a) pour tout $f \in E$, on a $$\int_X e^{is} d\mu = \exp(- \|f\|^2/2);$$

b) pour tout $f \in E$ de norme 1, l’image de la mesure $\mu$ par $f$ est la mesure
$$(2\pi)^{-1/2} e^{-x^2/2} dx.$$
sur $\mathbf{R}$.

*Supposons que E soit un espace gaussien.* Soient $f_1, \ldots, f_n$ des fonctions dont les classes $f_i$ appartiennent à E. On définit une fonction :$f_1 \ldots f_n$ : sur X (appelée « produit de Wick » de $f_1, \ldots, f_n$) par la formule

$$
:f_1 \ldots f_n: = \sum_{0 \leq 2p \leq n} (-1)^p \sum_{\sigma \in I_p} \prod_{i=1}^p \langle f_{\sigma(2i-1)}|f_{\sigma(2i)} \rangle \prod_{j=2p+1}^n f_{\sigma(j)},
$$

où $I_p$ est l’ensemble des permutations $\sigma$ de $\{1, 2, \ldots, n\}$ telles que l’on ait
$$
\begin{align*}
&\sigma(1) < \sigma(2), \ldots, \sigma(2p-1) < \sigma(2p) \\
&\sigma(1) < \sigma(3) < \cdots < \sigma(2p-1) \\
&\sigma(2p+1) < \sigma(2p+2) < \cdots < \sigma(n).
\end{align*}
$$

Il existe alors un *isomorphisme* $\varphi$ de $\hat{\mathbf{S}}(E)$ *sur un sous-espace hilbertien de* $L^2_\mathbf{R}(X, \mu)$ qui transforme en $:f_1 \ldots f_n:$ le produit $f_1' \ldots f_n'$ de $f_1', \ldots, f_n'$ calculé dans $\hat{\mathbf{S}}(E)$. Supposons que X soit un espace souslinien et qu’il existe une famille dénombrable $(f_n)$ de fonctions dont les classes appartiennent à E et qui séparent les points de X. Alors $\varphi$ est un isomorphisme de $\hat{\mathbf{S}}(E)$ sur $L^2_\mathbf{R}(X, \mu)$.

### 4. Puissances extérieures hilbertiennes

Soient E un espace hilbertien et $n$ un entier positif. Pour toute permutation $\sigma \in \mathfrak{S}_n$, notons $\varepsilon_\sigma$ sa signature ; posons $a_n = \frac{1}{n!} \sum_{\sigma \in \mathfrak{S}_n} \varepsilon_\sigma p_\sigma$ dans $\mathcal{L}(\hat{T}^n(E))$ (V, p. 30). Il est immédiat que $a_n$ est un orthoprojecteur, dont l’image $\overline{A'_n(E)}$ est l’adhérence dans $\hat{T}^n(E)$ de l’espace $A'_n(E)$ des tenseurs antisymétriques d’ordre $n$ (A, III, p. 82). Il existe un isomorphisme $\pi_n$ de $\Lambda^n(E)$ sur $A'_n(E)$ caractérisé par

$$
\pi_n(x_1 \wedge \ldots \wedge x_n) = a_n(x_1 \otimes \ldots \otimes x_n) = \frac{1}{n!} \sum_{\sigma \in \mathfrak{S}_n} \varepsilon_\sigma x_{\sigma(1)} \otimes \ldots \otimes x_{\sigma(n)}
$$

pour $x_1, \ldots, x_n$ dans E. On définit alors sur $\Lambda^n(E)$ une structure d’espace préhilbertien séparé en posant

$$
\langle u|v \rangle = n! \langle \pi_n(u)|\pi_n(v) \rangle.
$$

Plus explicitement, on a (comparer avec la formule (30) de A, III, p. 153)

$$(26)\quad \langle x_1 \wedge \ldots \wedge x_n | y_1 \wedge \ldots \wedge y_n \rangle = \det(\langle x_i | y_j \rangle)$$

quels que soient $x_1, \ldots, x_n$ et $y_1, \ldots, y_n$ dans E.

On note $\hat{\Lambda}^n(E)$ le complété de l’espace préhilbertien $\Lambda^n(E)$, et $\hat{\Lambda}(E)$ la somme hilbertienne externe des espaces hilbertiens $\hat{\Lambda}^n(E)$.

*Exemple. — \* Reprenons les notations de l’exemple 1 de V, p. 32. On peut alors identifier l’espace hilbertien $\hat{\Lambda}(E)$ à l’ensemble des suites $(f_n)_{n \geq 0}$ de fonctions mesurables qui rendent fini le nombre $\|f\|$ défini dans (22), et où chaque fonction $f_n$ est antisymétrique, c’est-à-dire satisfait à la relation

$$
f_n(x_{\sigma(1)}, \ldots, x_{\sigma(n)}) = \varepsilon_\sigma f_n(x_1, \ldots, x_n)
$$

pour toute permutation $\sigma \in S_n$. L’espace hilbertien $\hat{\Lambda}(E)$ s’appelle l’espace de Fock antisymétrique correspondant au poids $\omega_*$.

#### Proposition 5 {#evt-v-s3-prop-5 .statement}

*Soit $(e_i)_{i \in I}$ une base orthonormale de l’espace hilbertien E. Munissons I d’une structure d’ordre total. Alors l’ensemble des éléments $e_{i_1} \wedge \ldots \wedge e_{i_n}$ pour $i_1 < \cdots < i_n$ est une base orthonormale de $\hat{\Lambda}^n(E)$.

On sait (A, III, p. 86) que les éléments en question forment une base de l’espace vectoriel $\Lambda^n(E_0)$ où $E_0$ est le sous-espace vectoriel de E engendré par les vecteurs $e_i$. Par ailleurs, pour $i_1 < \cdots < i_n$, la matrice des produits scalaires $\langle e_{i_k} | e_{i_l} \rangle$ est la matrice unité d’ordre $n$; d’après (26), on a donc $\|e_{i_1} \wedge \ldots \wedge e_{i_n}\| = 1$. Enfin, si $(i_1, \ldots, i_n)$ et $(j_1, \ldots, j_n)$ sont deux suites strictement croissantes d’éléments de I; distinctes, il existe un élément $j_l$ distinct de $i_1, \ldots, i_n$ et donc on a $\langle e_{i_k} | e_{j_l} \rangle = 0$ pour $1 \leq k \leq n$, d’où $\langle e_{i_1} \wedge \ldots \wedge e_{i_n} | e_{j_1} \wedge \ldots \wedge e_{j_n} \rangle = 0$ d’après (26). Autrement dit, la famille des éléments $e_{i_1} \wedge \ldots \wedge e_{i_n}$, pour $i_1 < \cdots < i_n$, est orthonormale.

Or $E_0$ est dense dans E, et l’application $(x_1, \ldots, x_n) \mapsto x_1 \wedge \ldots \wedge x_n$ de $E \times \cdots \times E$ dans $\Lambda^n(E)$ est continue. Par conséquent, $\Lambda^n(E_0)$ est dense dans $\Lambda^n(E)$, d’où la proposition 5.

#### Corollaire {#evt-v-s3-n4-cor-1 .statement}

*Supposons que l’espace hilbertien E soit somme directe des sous-espaces orthogonaux M et N. L’isomorphisme canonique g de $\Lambda(M) \otimes \Lambda(N)$ sur $\Lambda(E)$ (A, III, p. 84) se prolonge de manière unique en un isomorphisme d’espaces hilbertiens de $\hat{\Lambda}(M) \otimes_2 \hat{\Lambda}(N)$ sur $\hat{\Lambda}(E)$.

La démonstration est analogue à celle du corollaire de la prop. 4 (V, p. 31).

Soient E et F deux espaces hilbertiens et $u \in \mathcal{L}(E ; F)$. On montre, comme dans le cas des puissances symétriques $\hat{S}^n(E)$ (V, p. 32), que l’application linéaire $\Lambda^n(u)$ de $\Lambda^n(E)$ dans $\Lambda^n(F)$ (A, III, p. 81) se prolonge en une application linéaire continue $\hat{\Lambda}^n(u)$ de $\hat{\Lambda}^n(E)$ dans $\hat{\Lambda}^n(F)$. On a les relations

$$(27)\quad \hat{\Lambda}^n(1_E) = 1_{\hat{\Lambda}^n(E)},$$
$$(28)\quad \hat{\Lambda}^n(v \circ u) = \hat{\Lambda}^n(v) \circ \hat{\Lambda}^n(u) \quad \text{si } v \text{ appartient à } \mathcal{L}(F ; G),$$
$$(29)\quad \| \hat{\Lambda}^n(u) \| \leq \| u \|^{n}.$$

On n’a pas en général égalité dans la formule (29) (TS, IV, § 6). Enfin, on a un isomorphisme $\psi_n = \psi_{n,E}$ de $\hat{\Lambda}^n(E)$ sur le sous-espace $\mathbf{A}'_n(E)$ de $\hat{T}^n(E)$ défini par
$$
(30) \quad \psi_n(x_1 \wedge \ldots \wedge x_n) = \frac{1}{(n!)^{1/2}} \sum_{\sigma \in S_n} \varepsilon_\sigma x_{\sigma(1)} \otimes \ldots \otimes x_{\sigma(n)} .
$$

### 5. Multiplication extérieure

Soit E un espace hilbertien. Pour tout entier $n \geqslant 0$, notons $\theta_n$ l’application canonique de $T^n(E)$ sur $\Lambda^n(E)$; on a donc
$$
(31) \quad \theta_n(x_1 \otimes \ldots \otimes x_n) = x_1 \wedge \ldots \wedge x_n
$$
pour $x_1, \ldots, x_n$ dans E. Soient $p$ et $q$ deux entiers positifs ; compte tenu des formules (30) et (31), on a
$$
(32) \quad u \wedge v = \theta_{p+q}\left( \frac{1}{(p!)^{1/2}} \psi_p(u) \otimes \frac{1}{(q!)^{1/2}} \psi_q(v) \right)
$$
pour $u \in \Lambda^p(E)$ et $v \in \Lambda^q(E)$. Comme on a $\| \theta_n \| \leq (n!)^{1/2}$, on obtient l’inégalité
$$
(33) \quad \| u \wedge v \| \leq \left( \frac{(p+q)!}{p! \, q!} \right)^{1/2} \| u \| \cdot \| v \|
$$
pour $u \in \Lambda^p(E)$ et $v \in \Lambda^q(E)$. Par suite, l’application $(u, v) \mapsto u \wedge v$ se prolonge par continuité en une application bilinéaire de $\hat{\Lambda}^p(E) \times \hat{\Lambda}^q(E)$ dans $\hat{\Lambda}^{p+q}(E)$, de norme au plus égale à $\left( \frac{(p+q)!}{p! \, q!} \right)^{1/2}$ (cf. V, p. 72, exerc. 2). On la note encore $(u, v) \mapsto u \wedge v$.

#### Proposition 6 {#evt-v-s3-prop-6 .statement}

*Soit E un espace hilbertien. On a*
$$
(34) \quad \| x \wedge u \| \leq \| x \| \cdot \| u \|
$$
*pour* $x \in E$ *et* $u \in \hat{\Lambda}(E)$.

On se ramène aussitôt au cas où $x$ est de norme 1.

Soit F le sous-espace hilbertien de E formé des vecteurs orthogonaux à $x$. Comme E est somme hilbertienne de F et de la droite $K.x$, il résulte aussitôt du corollaire de V, p. 34 que l’application $(v, w) \mapsto v + x \wedge w$ est un isomorphisme d’espaces hilbertiens de $\hat{\Lambda}(F) \oplus \hat{\Lambda}(F)$ sur $\hat{\Lambda}(E)$. Si $u = v + x \wedge w$ avec $v, w$ dans $\hat{\Lambda}(F)$, on a $x \wedge u = x \wedge v$, d’où $\| x \wedge u \| = \| v \| \leq (\| v \|^2 + \| w \|^2)^{1/2} = \| u \|$.

#### Corollaire 1 {#evt-v-s3-prop-6-cor-1 .statement}

*a)* *Soient* $x_1, \ldots, x_n$ *des éléments de l’espace hilbertien E. On a*
$$
(35) \quad \| x_1 \wedge \ldots \wedge x_n \| \leq \| x_1 \| \ldots \| x_n \|,
$$
*l’égalité ne pouvant avoir lieu que si l’un des* $x_i$ *est nul, ou la suite* $(x_1, \ldots, x_n)$ *orthogonale.*

b) Soient $x_1, ..., x_n, y_1, ..., y_n$ des éléments de l’espace hilbertien E. On a

$$
|\det(\langle x_i, y_j \rangle)| \leq \|x_1\| ... \|x_n\| \cdot \|y_1\| ... \|y_n\|;
$$

si les vecteurs $x_i$ et $y_j$ sont non nuls, l’égalité a lieu dans (36) si et seulement si $(x_1, ..., x_n)$ et $(y_1, ..., y_n)$ sont deux bases orthogonales d’un même sous-espace vectoriel de E.

L’inégalité (35) résulte par récurrence sur $n$ de la prop. 6 ; l’inégalité (36) s’en déduit en appliquant l’inégalité de Cauchy-Schwarz dans $\Lambda^n(E)$ et la formule (26) de V, p. 34.

Supposons que la suite $(x_1, ..., x_n)$ soit orthogonale. On a

$$
\|x_1 \wedge ... \wedge x_n\|^2 = \det(\langle x_i|x_j \rangle) = \prod_{i=1}^n \|x_i\|^2
$$

puisque l’on a $\langle x_i|x_j \rangle = 0$ pour $i \neq j$.

Supposons maintenant que les vecteurs $x_1, ..., x_n$ ne soient pas nuls et ne forment pas une suite orthogonale. Comme $\|x_1 \wedge ... \wedge x_n\|$ dépend de manière symétrique des vecteurs $x_1, ..., x_n$, on peut supposer que $x_1$ n’est pas orthogonal au sous-espace F de E engendré par $x_2, ..., x_n$, et que F n’est pas réduit à 0. On peut décomposer $x_1$ sous la forme $x_1' + y$ avec $y \neq 0$ dans F et $x_1'$ orthogonal à F, d’où $\|x_1'\| < \|x_1\|$. Or $x_1 \wedge x_2 \wedge ... \wedge x_n = x_1' \wedge x_2 \wedge ... \wedge x_n$, d’où

$$
\|x_1 \wedge ... \wedge x_n\| \leq \|x_1'\| \|x_2\| ... \|x_n\|
< \|x_1\| \|x_2\| ... \|x_n\|.
$$

Supposons que les vecteurs $x_i$ et les vecteurs $y_j$ ne soient pas nuls. L’égalité dans la relation (36) équivaut à la conjonction des égalités

(37) $|\langle x_1 \wedge ... \wedge x_n|y_1 \wedge ... \wedge y_n \rangle| = \|x_1 \wedge ... \wedge x_n\| \cdot \|y_1 \wedge ... \wedge y_n\|$

(38) $\|x_1 \wedge ... \wedge x_n\| = \|x_1\| ... \|x_n\| , \quad \|y_1 \wedge ... \wedge y_n\| = \|y_1\| ... \|y_n\| .$

D’après la première partie de la démonstration, les égalités (38) signifient que chacune des suites $(x_1, ..., x_n)$ et $(y_1, ..., y_n)$ est orthogonale, ce qui entraîne $x_1 \wedge ... \wedge x_n \neq 0$ et $y_1 \wedge ... \wedge y_n \neq 0$. Sous ces conditions, la relation (37) signifie qu’il existe un scalaire $\lambda \neq 0$ tel que $y_1 \wedge ... \wedge y_n = \lambda x_1 \wedge ... \wedge x_n$ (V, p. 4, Remarque 1), autrement dit que $(x_1, ..., x_n)$ et $(y_1, ..., y_n)$ sont des bases d’un même sous-espace vectoriel de E (A, III, p. 172).

#### Corollaire 2 {#evt-v-s3-prop-6-cor-2 .statement}

Soit $(a_{ij})_{1 \leq i,j \leq n}$ une matrice hermitienne, à éléments complexes, de déterminant D. On suppose que l’on a l’inégalité

$$
\sum_{i,j=1}^n a_{ij} \overline{z}_i z_j \geq 0
$$

quels que soient les nombres complexes $z_1, ..., z_n$. On a alors

$$
0 \leq D \leq a_{11} ... a_{nn}.
$$

Supposons $D$ non nul ; l'égalité $D = a_{11} \ldots a_{nn}$ a lieu si et seulement si l'on a $a_{ij} = 0$ pour $i \neq j$.

Soit $\Phi$ la forme hermitienne sur l'espace vectoriel $\mathbf{C}^n$ donnée par
$$
\Phi(z, z') = \sum_{i,j=1}^n a_{ij} \overline{z}_i z'_j
$$
pour $z = (z_1, \ldots, z_n)$ et $z' = (z'_1, \ldots, z'_n)$ dans $\mathbf{C}^n$. Par hypothèse, $\Phi$ est positive.

Supposons d'abord que $\Phi$ soit séparante, c'est-à-dire $D$ non nul. Si $(e_1, \ldots, e_n)$ est la base canonique de $\mathbf{C}^n$, on a $\Phi(e_i, e_j) = a_{ij}$, et le cor. 2 résulte aussitôt du cor. 1, a) où l'on fait $x_i = e_i$.

Puisque $a_{ii} = \Phi(e_i, e_i) \geqslant 0$, on a aussi l'inégalité (40) si $D = 0$.

#### Corollaire 3 (« Inégalités de Hadamard ») {#evt-v-s3-prop-6-cor-3 .statement}

*Soit* $(a_{ij})_{1 \leqslant i,j \leqslant n}$ *une matrice à éléments complexes, de déterminant* $D$. *Posons*
$$
c_i = (\sum_{j=1}^n |a_{ij}|^2)^{1/2} \quad \text{pour} \quad 1 \leqslant i \leqslant n ,
$$
*et* $m = \sup_{i,j} |a_{ij}|$. *On a alors*
$$(41)$$
$$
|D| \leqslant c_1 \ldots c_n \leqslant m^n . n^{n/2} .
$$
*Si* $D \neq 0$, *pour que* $|D| = c_1 \ldots c_n$, *il faut et il suffit que les lignes* $y_i = (a_{ij})_{1 \leqslant j \leqslant n}$
*de la matrice* $(a_{ij})_{1 \leqslant i,j \leqslant n}$ *soient des vecteurs deux à deux orthogonaux*.

Munissons l'espace $\mathbf{C}^n$ du produit scalaire défini par
$$
\langle z|z' \rangle = \sum_{i=1}^n \overline{z}_i z'_i .
$$
Soient $(x_1, \ldots, x_n)$ la base canonique de $\mathbf{C}^n$ et $y_i$ le vecteur de composantes $a_{ij}$ pour $1 \leqslant j \leqslant n$. On a $\|x_i\| = 1$ et $\|y_i\| = c_i$ pour $1 \leqslant i \leqslant n$; on a aussi $\langle x_i|y_j \rangle = a_{ji}$. L'inégalité $|D| \leqslant c_1 \ldots c_n$ et la condition d'égalité sont alors des cas particuliers de V, p. 35, cor. 1. On a évidemment $c_i \leqslant m . n^{1/2}$, d'où $c_1 \ldots c_n \leqslant m^n . n^{n/2}$.

## EXERCICES {#evt-v-s3-exercises}

See the [exercises for § 3](exercises/s3/).
