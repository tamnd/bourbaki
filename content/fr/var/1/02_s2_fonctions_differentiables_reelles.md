---
book: var
book_title: Variétés différentielles et analytiques
chapter: "1"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 2
section_title: Fonctions différentiables réelles
lang: fr
source: var-fr
pdf_pages: 0015-0019
extraction: ocr
subsections:
    - "no": 1
      title: Fonctions dérivables en un point
      page: 0
      pdf_page: 15
    - "no": 2
      title: Le théorème des accroissements finis
      page: 0
      pdf_page: 15
    - "no": 3
      title: Fonctions de classe $C^r$ ($r \neq \omega$)
      page: 0
      pdf_page: 16
    - "no": 4
      title: Dérivées des fonctions de classe $C^r$
      page: 0
      pdf_page: 17
    - "no": 5
      title: Formule de Taylor
      page: 0
      pdf_page: 17
    - "no": 6
      title: Critères de dérivabilité
      page: 0
      pdf_page: 19
statements: 0
exercises: 0
content_sha256: 751c6249671612296169a2ada973673daef293ce7e4ae1a9d165e88250336f6c
---

## § 2. Fonctions différentiables réelles

Dans ce paragraphe, on suppose que K = R. La lettre E désigne un espace vectoriel normé sur R ; la lettre F désigne un espace vectoriel topologique localement convexe séparé sur R.

### 2.1. Fonctions dérivables en un point

2.1.1. Soit f une fonction définie au voisinage d’un point x_0 de E et à valeurs dans F. Soit u un élément de l’espace $\mathcal{L}(E; F)$ des applications linéaires continues de E dans F. Pour que f soit dérivable en x_0 et y admette u pour dérivée, il faut et suffit que l’on ait
$$
\lim_{h \to 0, h \neq 0} \frac{f(x_0 + h) - f(x_0) - u(h)}{\|h\|} = 0.
$$

2.1.2. Pour que f soit strictement dérivable en x_0, il faut et suffit que l’on ait
$$
\lim_{(h, k) \to (0, 0), h \neq k} \frac{f(x_0 + h) - f(x_0 + k) - Df(x_0) \cdot (h - k)}{\|h - k\|} = 0.
$$

2.1.3. Soient F_1 et F_2 deux espaces localement convexes séparés et soit u une application bilinéaire de F_1 × F_2 dans F, satisfaisant à la condition de continuité suivante :
(SC) Si ((a_n, b_n)) est une suite d’éléments de F_1 × F_2 convergeant vers un élément (a, b) ∈ F_1 × F_2, alors la suite (u(a_n, b_n)) converge vers u(a, b) dans F.

Soit f_i (pour i = 1, 2) une application d’un voisinage d’un point x_0 de E dans F_i. Si f_1 et f_2 sont dérivables en x_0, alors u(f_1, f_2) est dérivable en x_0 et l’on a :
$$
D(u(f_1, f_2))(x_0) \cdot h = u(Df_1(x_0) \cdot h, f_2(x_0)) + u(f_1(x_0), Df_2(x_0) \cdot h)
$$
pour tout $h \in E$.

### 2.2. Le théorème des accroissements finis

2.2.1. Soient x, y dans E, et [x, y] le segment fermé joignant ces deux points. Soit de plus f une application d’un voisinage de [x, y] dans l’espace F, dérivable en tout point de [x, y]. Alors f(x) − f(y) appartient à l’enveloppe convexe fermée de l’ensemble des points Df(z) · (x − y) pour z dans [x, y].

2.2.2. Soient U un ouvert connexe de E, et f une application de U dans

F, admettant une dérivée nulle en tout point de U; alors $f$ est constante dans U.

2.2.3. Soient U un ouvert *convexe* de E, et $f$ une application de U dans F, dérivable en tout point de U. Etant donnés une semi-norme continue $\gamma$ sur F et un nombre réel $M \geqslant 0$, les conditions suivantes sont équivalentes:
    (i) Pour tout $x$ dans U, on a $\|Df(x)\|_{\gamma} \leqslant M$.
    (ii) Pour tout $x$ et tout $y$ dans U, on a $\|f(x) - f(y)\|_{\gamma} \leqslant M \cdot \|x - y\|$.

2.2.4. Soit U un voisinage d’un point $x_0$ de E et soit $f$ une fonction définie dans le complémentaire de $x_0$ dans U, à valeurs dans F. Supposons que $f$ admet une dérivée $Df(x)$ en tout point $x$ de U, $x \neq x_0$, et que la fonction $x \mapsto Df(x)$ admet une limite $D_0$ quand $x$ tend vers $x_0$. Alors, si $\dim(E) \geqslant 2$, $f$ a une limite en $x_0$ et la fonction $f$ prolongée par continuité à U tout entier est dérivable de dérivée $D_0$ en $x_0$; il en est de même si $\dim(E) = 1$ et qu’on suppose que $f$ a une limite en $x_0$.

### 2.3. Fonctions de classe $C^r$ ($r \neq \omega$)

2.3.1. Soient U un ouvert de E et $f$ une application de U dans F. On définit la relation « $f$ est de classe $C^r$ » (pour $r \in \mathbf{N}$) par récurrence sur $r$ de la manière suivante:
    1) $f$ est de classe $C^0$ si et seulement si elle est continue;
    2) si $r$ est un entier $\geqslant 1$, la fonction $f$ est de classe $C^r$ si et seulement si elle est dérivable en tout point de U et si l’application dérivée $Df$ de U dans $\mathcal{L}(E; F)$ est de classe $C^{r-1}$.

Les fonctions de classe $C^r$ sont aussi appelées *fonctions r fois continûment dérivables*.

On dit que $f$ est *de classe $C^{\infty}$* (ou *indéfiniment dérivable*) si elle est de classe $C^r$ pour tout entier $r$.

Si $f$ est de classe $C^r$ dans U, alors $f$ est $p$ fois dérivable pour tout entier $p \leqslant r$ et la fonction $D^p f$ est de classe $C^{r-p}$.

2.3.2. Les applications de classe $C^r$ d’un ouvert U de E dans F forment un sous-espace vectoriel $\mathcal{C}^r(U; F)$ de l’espace de toutes les applications de U dans F. On a $\mathcal{C}^s(U; F) \subset \mathcal{C}^r(U; F)$ pour $s \geqslant r$.

2.3.3. Pour qu’une fonction $f$ soit de classe $C^1$ dans un ouvert U de E, il faut et il suffit qu’elle soit strictement dérivable en tout point de U.

Si E est un produit d’espaces normés $E_i$, une application $f$ d’un ouvert V de E dans F est de classe $C^r$ si et seulement si $f$ possède des dérivées partielles itérées $D_{i_1} \ldots D_{i_m} f$ continues pour tout entier $m \leqslant r$.

2.3.4. Soit G un espace normé et soit U un ouvert de E. Soient V un ouvert de G, $g \in \mathcal{C}^r(U; G)$ et $f \in \mathcal{C}^r(V; F)$. Si $g(U) \subset V$, l’application $f \circ g$ de U dans F est de classe $C^r$.

Soient $F_1$ et $F_2$ deux espaces localement convexes séparés et $u$ une application bilinéaire de $F_1 \times F_2$ dans F, hypocontinue par rapport à l’ensemble des parties bornées de $F_1$ (resp. $F_2$) (Esp. Vect. Top., ch. III, § 4, n° 2). Soient U un ouvert de E et $f_i \in \mathcal{C}^r(U; F_i)$ (pour $i = 1, 2$). Alors la fonction $u(f_1, f_2)$ appartient à $\mathcal{C}^r(U; F)$. Si E est de dimension finie, il suffit de supposer que $u$ satisfait à la condition (SC) du n° 2.1.3.

2.3.5. Si E est un produit d’espaces normés $E_i$ ($1 \leq i \leq n$) et si $f$ est une application $n$-linéaire continue de E dans F, alors $f$ est de classe $C^\infty$ et l’on a $D^p f = 0$ pour $p \geq n + 1$.

2.3.6. Supposons que E et F soient des espaces de Banach. Soit $f$ une fonction de classe $C^r$ (avec $r \geq 1$) définie dans un voisinage d’un point $x_0$ de E et à valeurs dans F. Soit $y_0 = f(x_0)$ et supposons que $Df(x_0)$ soit un isomorphisme de E sur F. Alors $f$ induit un homéomorphisme $g$ d’un voisinage de $x_0$ sur un voisinage de $y_0$ (1.5) et l’application réciproque de $g$ est de classe $C^r$ au voisinage de $y_0$.

### 2.4. Dérivées des fonctions de classe $C^r$

2.4.1. Soit $f$ une application de classe $C^r$ d’un ouvert U de E dans F. Pour tout $x \in U$, et tout entier $s$ avec $s \leq r$, l’application multilinéaire $D^s f(x)$ est symétrique.

2.4.2. Supposons de plus E de dimension finie et soit $(e_1, \ldots, e_n)$ une base de E. Les dérivées partielles $\partial_{i_1} \ldots \partial_{i_s} f$ dépendent symétriquement des indices $i_1, \ldots, i_s$. Soit $\alpha_k$ le nombre de fois que l’indice $k$ intervient dans la suite $i_1, \ldots, i_s$ et soit $\alpha = (\alpha_1, \ldots, \alpha_n)$. On pose alors:

$$
\partial^{\alpha} f = \partial_1^{\alpha_1} \ldots \partial_n^{\alpha_n} f = \partial_{i_1} \ldots \partial_{i_s} f
$$

Lorsque les coordonnées relatives à la base $(e_1, \ldots, e_n)$ sont notées $x_1, \ldots, x_n$, on écrit aussi $\partial^{\alpha} f$ sous la forme:

$$
\frac{\partial^{|\alpha|} f}{\partial x_1^{\alpha_1} \ldots \partial x_n^{\alpha_n}}
$$

### 2.5. Formule de Taylor

2.5.1. Soit $r$ un entier $\geq 1$ et soit $f$ une application de classe $C^r$ d’un ouvert U de E dans F. Pour $x \in U$, $h \in E$ et $p \leq r$, convenons d’écrire $D^p f(x_0) \cdot h^p$ au lieu de $D^p f(x_0) \cdot (h, \ldots, h)$. Si le segment $[x, x + h]$ est contenu dans $U$, on a la formule (« formule de Taylor »):

$$
f(x + h) = \sum_{p=0}^{r-1} \frac{1}{p!} D^p f(x) \cdot h^p + v_r(x; h)
$$

où le « reste » $v_r(x; h)$ est donné par :

$$
v_r(x; h) = \int_0^1 \frac{(1-t)^{r-1}}{(r-1)!} D^r f(x + th) \cdot h^r \, dt
$$

On a :

$$
v_r(x; h) \equiv \frac{1}{r!} D^r f(x) \cdot h^r \quad \text{mod } o(\|h\|^r) \quad \text{quand } h \text{ tend vers } 0
$$

et

$$
f(x + h) \equiv \sum_{p=0}^r \frac{1}{p!} D^p f(x) \cdot h^p \quad \text{mod } o(\|h\|^r)
$$

quand $h$ tend vers zéro.

2.5.2. Soit de plus $\gamma$ une semi-norme continue sur $F$; si l’on a $\|D^r f(z)\|_\gamma \leq M$ pour tout point $z$ du segment $[x, x + h]$, alors on a :

$$
\|v_r(x; h)\|_\gamma \leq \frac{M}{r!} \|h\|^r
$$

2.5.3. Supposons en outre que $E = \mathbf{R}^n$. On a alors :

$$
f(x + h) \equiv \sum_{|\alpha| \leq r} \Delta^\alpha f(x) h^\alpha \quad \text{mod } o(\|h\|^r) \quad \text{quand } h \text{ tend vers } 0
$$

en posant :

$$
\Delta^\alpha f(x) = \frac{1}{\alpha!} \partial^\alpha f(x)
$$

2.5.4. Soient $f$ et $g$ deux fonctions de classe $C^r$ sur un ouvert $U$ de $E$, à valeurs dans $F$. Pour que $f$ et $g$ aient en un point $x$ de $U$ un contact d’ordre $\geq r$, il faut et il suffit que l’on ait $D^p f(x) = D^p g(x)$ pour tout entier $p$ avec $0 \leq p \leq r$. Lorsque $E$ est de dimension finie, cela revient à dire que les dérivées partielles itérées d’ordre $\leq r$ de $f$ et de $g$ (par rapport à une base de $E$) sont égales au point $x$.

2.5.5. Soit $U$ un ouvert de $E \times \mathbf{R}^n$ de la forme $V \times I_1 \times \cdots \times I_n$, où $V$ est un ouvert de $E$ et $I_1, \ldots, I_n$ des intervalles ouverts de $\mathbf{R}$ contenant 0. Posons $U_0 = V$ et $U_j = V \times I_1 \times \cdots \times I_j$ pour $1 \leq j \leq n$. Etant donnée une fonction $f \in \mathcal{C}^r(U; F)$ (avec $1 \leq r \leq \infty$), il existe une suite et une seule de fonctions $f_j \in \mathcal{C}^{r-1}(U_j; F)$ (pour $0 \leq j \leq n$) telle que:

$$
f(x, t_1, \ldots, t_n) = f_0(x) + \sum_{j=1}^n t_j f_j(x, t_1, \ldots, t_j)
$$

pour $x \in V$ et $t_j \in I_j$. On a:

$$
f_0(x) = f(x, 0, \ldots, 0)
$$
$$
f_j(x, t_1, \ldots, t_j) = \int_0^1 \partial_j f(x, t_1, \ldots, t_{j-1}, t_j u, 0, \ldots, 0) du
$$

pour $1 \leq j \leq n$. Dans cette dernière formule, $\partial_j f$ désigne la $j$-ième dérivée partielle de la fonction $(t_1, \ldots, t_n) \mapsto f(x, t_1, \ldots, t_n)$.

### 2.6. Critères de dérivabilité

2.6.1. Supposons que $F$, outre sa topologie $\mathcal{T}$, soit muni d'une topologie moins fine $\mathcal{T}'$, qui fait aussi de $F$ un espace localement convexe séparé. Supposons en outre que $\mathcal{T}$ et $\mathcal{T}'$ satisfont à la condition suivante:
(S) Pour tout voisinage $V$ de 0 pour la topologie $\mathcal{T}$, il existe un voisinage $W$ de 0 pour $\mathcal{T}$ tel que l'enveloppe convexe $\mathcal{T}'$-fermée de toute partie $\mathcal{T}$-compacte de $W$ soit contenue dans $V$.

Soit $f$ une application d'un ouvert $U$ de $E$ dans $F$. Supposons que $f$ est de classe $C^r$ ($1 \leq r \leq \infty$) lorsque l'on munit $F$ de la topologie $\mathcal{T}'$, que $D^m f(x)$ est, pour tout $x$ de $U$, et tout entier $m \leq r$, une application multilinéaire continue de $E^m$ dans $F$ muni de la topologie $\mathcal{T}$ et que l'application $x \mapsto D^m f(x)$ est continue de $U$ dans $\mathcal{L}_m(E; F)$ ($F$ étant muni de la topologie $\mathcal{T}$). Alors $f$ est de classe $C^r$ lorsque l'on munit $F$ de la topologie $\mathcal{T}$ et ses dérivées $D^m f$ sont les mêmes pour $\mathcal{T}$ et pour $\mathcal{T}'$.

La condition (S) est en particulier réalisée s'il existe un système fondamental de voisinages de 0 pour la topologie $\mathcal{T}$ qui sont fermés pour la topologie $\mathcal{T}'$: c'est le cas si le dual de $F$ muni de $\mathcal{T}$ est identique au dual de $F$ muni de $\mathcal{T}'$. La condition (S) est également réalisée si $F$ muni de la topologie $\mathcal{T}$ est quasi-complet (*Esp. Vect. Top.*, ch. III, § 2, n° 5).

2.6.2. Soit $f$ une application d'un ouvert $U$ de $E$ dans $F$. Si $f$ est de classe $C^r$ (avec $0 \leq r \leq \infty$), les fonctions scalaires $u \circ f$ sont de classe $C^r$ pour toute forme linéaire continue $u$ sur $F$. Réciproquement si $F$ est quasi-complet et si les fonctions $u \circ f$ sont de classe $C^{r+1}$ pour tout $u \in F'$, alors $f$ est de classe $C^r$.
