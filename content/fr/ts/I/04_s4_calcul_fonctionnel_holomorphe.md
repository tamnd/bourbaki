---
book: ts
book_title: Théories spectrales
chapter: I
chapter_title: ALGÈBRES NORMÉES
section: 4
section_title: Calcul fonctionnel holomorphe
lang: fr
source: ts-i-ii-fr
book_pages: TS I.49-TS I.88, TS I.172-TS I.177
pdf_pages: 0062-0101, 0185-0190
extraction: native
subsections:
    - "no": 1
      title: Germes de fonctions holomorphes
      page: 49
      pdf_page: 62
    - "no": 2
      title: Énoncé du théorème principal
      page: 51
      pdf_page: 64
    - "no": 3
      title: Suites adaptées et formes différentielles associées
      page: 52
      pdf_page: 65
    - "no": 4
      title: Construction des applications $\Theta_{\boldsymbol{a}}$
      page: 58
      pdf_page: 71
    - "no": 5
      title: Propriétés des applications $\Theta_{\boldsymbol{a}}$
      page: 61
      pdf_page: 74
    - "no": 6
      title: Théorèmes d’approximation
      page: 67
      pdf_page: 80
    - "no": 7
      title: Existence et unicité du calcul fonctionnel holomorphe
      page: 70
      pdf_page: 83
    - "no": 8
      title: Substitution dans le calcul fonctionnel
      page: 72
      pdf_page: 85
    - "no": 9
      title: Calcul fonctionnel holomorphe en une variable
      page: 74
      pdf_page: 87
    - "no": 10
      title: Exponentielle et logarithme
      page: 78
      pdf_page: 91
    - "no": 11
      title: Partitions de l’espace des caractères
      page: 79
      pdf_page: 92
    - "no": 12
      title: Partitions du spectre d’un élément
      page: 81
      pdf_page: 94
    - "no": 13
      title: Calcul fonctionnel holomorphe dans une algèbre normable complète réelle ou complexe
      page: 85
      pdf_page: 98
    - "no": 14
      title: Cas d’une algèbre sans élément unité
      page: 88
      pdf_page: 101
statements: 55
exercises: 18
content_sha256: 01f7d92569861302816b91ad977439840048381ad2f72762735ba146e3c5ff15
---

## § 4. CALCUL FONCTIONNEL HOLOMORPHE

### 1. Germes de fonctions holomorphes

Soient E et F des espaces de Banach complexes. On rappelle (cf. VAR, R1, p. 26, 3.2.1, p. 22, 3.1 et p. 88, App.) qu’une application holomorphe définie sur un ouvert U de E et à valeurs dans F est une application $f: U\rightarrow F$ telle que, pour tout $x\in U$, il existe une série convergente

$$
f_x=\sum_{k\geqslant 0}f_{x,k}
$$

vérifiant $f(x+y) =f_x(y)$ pour tout $y\in E$ assez proche de 0, où $f_{x,k}: E\rightarrow \mathbf{C}$ est un polynôme homogène continu de degré $k$ sur E à valeurs dans F, c’est-à-dire une application de la forme

$$
f_{x,k}(y) =\widetilde{f}_{x,k}(y, . . . , y)
$$

où $\widetilde{f}_{x,k}: E^k\rightarrow F$ est une application $k$-multilinéaire continue. On note $\mathscr{O}(U; F)$ l’espace vectoriel complexe des fonctions holomorphes sur U à valeurs dans F muni de la topologie de la convergence compacte. C’est un espace vectoriel topologique localement convexe, dont la topologie est définie par les semi-normes $f\mapsto$ sup$_{z\in K}\|f(z)\|$, où K parcourt l’ensemble des parties compactes de U.

Soient G un espace de Banach complexe et V une partie ouverte de G. Pour toute application holomorphe $\varphi : V\rightarrow$ U, l’application $\varphi^*:f\mapsto f\circ \varphi$ est une application linéaire continue de $\mathscr{O}(U; F)$ dans $\mathscr{O}(V; F)$.

Si H est un espace de Banach complexe et $\varphi : F\rightarrow H$ une application linéaire continue, alors l’application $f\mapsto \varphi \circ f$ est une application linéaire continue de $\mathscr{O}(U; F)$ dans $\mathscr{O}(U; H)$, notée $\varphi_*$.

Soit $n$ un entier naturel et posons $E =\mathbf{C}^n$. Soient K une partie compacte de $\mathbf{C}^n$ et $\mathscr{U}$ l’ensemble filtrant décroissant des voisinages ouverts de K. Si $U,U'\in \mathscr{U}$ et $U'\subset U$, l’application de restriction des fonctions de $\mathscr{O}(U; F)$ dans $\mathscr{O}(U'; F)$ est continue. La limite inductive des espaces $\mathscr{O}(U; F)$ pour ces applications est notée $\mathscr{O}(K; F)$. Les éléments de $\mathscr{O}(K; F)$ s’appellent les germes de fonctions holomorphes au voisinage de K et à valeurs dans F.

L’espace $\mathscr{O}(K; F)$ est muni de la topologie limite inductive des topologies localement convexes des $\mathscr{O}(U; F)$ (EVT, II, p. 31, exemple II). Soient X un espace vectoriel topologique localement convexe et $\varphi :\mathscr{O}(K; F)\rightarrow X$ une application. Pour tout voisinage ouvert U de K, l’application $\mathscr{O}(U; F)\rightarrow X$ déduite de $\varphi$ par composition avec l’application canonique $\mathscr{O}(U; F)\rightarrow \mathscr{O}(K; F)$ est notée $\varphi^U$. L’application $\varphi$ est continue si et seulement si $\varphi^U$ est continue pour tout U (EVT, II, p. 29, prop. 5, (iii)).

Soit $m$ un entier naturel. Soient L une partie compacte de $\mathbf{C}^m$ et V un voisinage ouvert de L. Soit $\varphi : V\rightarrow \mathbf{C}^n$ une application holomorphe telle que $\varphi (L)\subset K$. Les applications linéaires continues

$-1$

$$
\mathscr{O}(U; F)^{\varphi}\leftarrow^{^*}\rightarrow \mathscr{O}(\overset{-1}{\varphi}(U); F)^{\varphi^{\varphi}}\leftarrow^{^{(U)}}\rightarrow \mathscr{O}(L; F)
$$

pour U voisinage ouvert de K, induisent une application linéaire continue $\varphi^*:\mathscr{O}(K; F)\rightarrow \mathscr{O}(L; F)$ (loc. cit.).

Soient H un espace de Banach complexe et $\varphi : F\rightarrow H$ une application linéaire continue. Les applications linéaires continues

$$
\mathscr{O}(U; F)^{\varphi}\leftarrow_{_*}\rightarrow \mathscr{O}(U; H)^{\varphi}\leftarrow^{^U}\rightarrow \mathscr{O}(K; F)
$$

où U parcourt l’ensemble des voisinages ouverts de K dans $\mathbf{C}^n$, induisent une application linéaire continue $\varphi_*$ de $\mathscr{O}(K; F)$ dans $\mathscr{O}(K; H)$ (loc. cit.). On notera parfois $\varphi \circ f=\varphi_*(f)$.

Pour tout voisinage ouvert U de K, la restriction à K est une application linéaire continue $\mathscr{O}(U; F)\rightarrow \mathscr{C}(K; F)$ ; ces applications induisent une application linéaire continue $\mathscr{O}(K; F)\rightarrow \mathscr{C}(K; F)$, appelée évaluation des germes de fonctions holomorphes sur K.

Soit A une algèbre de Banach unifère complexe. Les espaces $\mathscr{O}(U; A)$ et $\mathscr{O}(K; A)$ sont des algèbres unifères. Si $A\not=\{0\}$, on peut identifier canoniquement $\mathscr{O}(U;\mathbf{C})$ (resp. $\mathscr{O}(K;\mathbf{C})$) à la sous-algèbre $\mathscr{O}(U;\mathbf{C})\cdot 1$ de $\mathscr{O}(U; A)$ (resp. à la sous-algèbre $\mathscr{O}(K;\mathbf{C})\cdot 1$ de $\mathscr{O}(K; A)$). On posera $\mathscr{O}(U) =\mathscr{O}(U;\mathbf{C})$ et $\mathscr{O}(K) =\mathscr{O}(K;\mathbf{C})$.

### 2. Énoncé du théorème principal

Soit X un ensemble. Si $m\leqslant n$, on notera $\pi_{m,n}$ l’application de $X^n$ dans $X^m$ telle que $\pi_{m,n}(\boldsymbol{x}) = (x_1, . . . , x_m)$ pour tout $\boldsymbol{x}= (x_1, . . . , x_n)\in X^n$.

Soit A une algèbre de Banach unifère sur $\mathbf{C}$. Pour tout entier $n\geqslant 1$ et tout $\boldsymbol{a}\in A^n$, on note Sp$^n(\boldsymbol{a})$ le spectre simultané Sp$^{\{1,...,n\}}_A(\boldsymbol{a})$ (déf. 2 de I, p. 42). C’est une partie compacte de $\mathbf{C}^n$. Pour tout entier $m$ tel que $1\leqslant m\leqslant n$, on a $\pi_{m,n}$(Sp$^n(\boldsymbol{a})) =$ Sp$^m(\pi_{m,n}(\boldsymbol{a}))$ (I, p. 41, n$^o6$). L’application linéaire continue

$\pi_{m,n}^*:\mathscr{O}$(Sp$^m(\pi_{m,n}(\boldsymbol{a})); A)\longrightarrow \mathscr{O}$(Sp$^n(\boldsymbol{a}); A)$

est un morphisme d’algèbres unifères.

Soit A une algèbre de Banach unifère commutative sur $\mathbf{C}$. Soit $n\geqslant 1$ un entier. On appelle calcul fonctionnel holomorphe en $n$ variables sur A la donnée, pour tout $\boldsymbol{a}\in A^n$, d’une application

$\Theta_{\boldsymbol{a}}:\mathscr{O}$(Sp$^n(\boldsymbol{a}); A)\longrightarrow A$

vérifiant les conditions :

(CF1) Pour tout $\boldsymbol{a}\in A^n$, l’application $\Theta_{\boldsymbol{a}}$ est un morphisme continu d’algèbres unifères.

(CF2) Si $\boldsymbol{a}= (a_1, . . . , a_n)$, et si $z_1, . . . , z_n$ désignent les germes au voisinage de Sp$^n(\boldsymbol{a})$ des fonctions coordonnées sur $\mathbf{C}^n$, on a

$$
\Theta_{\boldsymbol{a}}(z_1) =a_1, . . . ,\Theta_{\boldsymbol{a}}(z_n) =a_n
$$

#### Remarque {#ts-i-s4-n2-rem-1 .statement tag=029U}

Si le radical de l’algèbre A est nul, on peut omettre la condition de continuité dans (CF1) (cf. prop. 9 de I, p. 40).

On appelle calcul fonctionnel holomorphe sur A la donnée, pour tout entier $n\geqslant 1$, d’un calcul fonctionnel holomorphe en $n$ variables sur A, vérifiant :

(CF3) Quels que soient les entiers $m$ et $n$ tels que $1\leqslant m\leqslant n$, et quels que soient $\boldsymbol{a}\in A^n$ et $f\in \mathscr{O}$(Sp$^m(\pi_{m,n}(\boldsymbol{a}); A)$, on a

$$
\Theta_{\boldsymbol{a}}(\pi^*_{m,n}(f)) = \Theta_{\pi_{m,n}(\boldsymbol{a})}(f)
$$

L’objet de ce paragraphe est de démontrer le théorème suivant :

#### Théorème 1 {#ts-i-s4-thm-1 .statement tag=029V}

Soit A une algèbre de Banach unifère commutative complexe. Il existe un unique calcul fonctionnel holomorphe sur A.

La démonstration de ce théorème occupera les n$^{os}3$ à 7.

### 3. Suites adaptées et formes différentielles associées

Dans ce numéro, et jusqu’au numéro 5, on note A une algèbre de Banach unifère commutative complexe et $n$ un entier $\geqslant 1$.

Quand nous parlerons de fonctions indéfiniment dérivables sur une partie ouverte de $\mathbf{C}^n$, il s’agira de fonctions indéfiniment dérivables pour la structure sous-jacente de variété réelle. Les notions de calcul différentiel utilisées seront relatives à cette structure.

#### Définition 1 {#ts-i-s4-def-1 .statement tag=029W}

Soit $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$, soit $h:\mathbf{C}^n\rightarrow \mathbf{C}$ une application et soient $u_1, . . . , u_n$ des applications de $\mathbf{C}^n$ dans A. On dit que la suite $(h, u_1, . . . , u_n)$ est adaptée à $\boldsymbol{a}$ si

(i) L’application $h$ est indéfiniment dérivable, de support compact, et égale à 1 au voisinage de Sp$^n(\boldsymbol{a})$ ;

(ii) Les applications $u_1, . . . ,u_n$ sont indéfiniment dérivables ;

(iii) Pour tout $\boldsymbol{z}= (z_1, . . . , z_n)\in \mathbf{C}^n$, on a

$$
h(\boldsymbol{z}) + (z_1-a_1)u_1(\boldsymbol{z}) +\cdots + (z_n-a_n)u_n(\boldsymbol{z}) = 1 \tag{1}
$$

La forme différentielle de degré $2n$ sur $\mathbf{C}^n$, à coefficients dans A, définie par

$$
\omega =\bigwedge_{i=1}^n(du_i\wedge dz_i)
$$

est appelée la forme différentielle associée à $(h, u_1, . . . , u_n)$.

Si $(h, u_1, . . . , u_n)$ est adaptée à $\boldsymbol{a}$, alors on obtient en différentiant (1) l’égalité

$$
dh=-\sum_{i=1}^nu_idz_i-\sum_{i=1}^n(z_i-a_i)du_i \tag{2}
$$

d’où, pour tout $i$ tel que $1\leqslant i\leqslant n$, la relation

$$
dh\wedge dz_i\wedge \bigwedge_{j\not=i}(du_j\wedge dz_j) =-(z_i-a_i)\omega \tag{3}
$$

#### Lemme 1 {#ts-i-s4-lem-1 .statement tag=029X}

Soient U un ouvert de $\mathbf{C}^n$ et K un sous-ensemble compact de U. Il existe une application indéfiniment dérivable $h$ de $\mathbf{C}^n$ dans $\mathbf{C}$, égale à 1 sur K et à support compact inclus dans U.

Soit V un voisinage ouvert relativement compact de K tel que $\overline{V}$ est inclus dans U (TG, I, p. 65, prop. 10). Il existe une fonction indéfiniment dérivable $h$ de $\mathbf{C}^n$ dans $\mathbf{C}$ dont le support est inclus dans V et qui est égale à 1 sur K (VAR, R1, p. 40, 5.3.6). Cette fonction a les propriétés demandées.

#### Exemple {#ts-i-s4-n3-exa-1 .statement tag=029Y}

On suppose que $n= 1$. Soit $a\in A$. Pour tout voisinage ouvert U de Sp($a$), il existe une application indéfiniment dérivable $h$ de $\mathbf{C}$ dans $\mathbf{C}$ à support compact contenu dans U, égale à 1 au voisinage de Sp($a$) (VAR, R1, p. 40, 5.3.6). Posons

$$
u(z) = (1-h(z))(z-a)^{-1}
$$

pour $z\in \mathbf{C}-$ Sp($a$) et $u(z) = 0$ si $z\in$ Sp($a$). Le couple $(h, u)$ est adapté à $a$ et la forme différentielle associée est $\omega =du\wedge dz$.

#### Lemme 2 {#ts-i-s4-lem-2 .statement tag=029Z}

Soit $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$. Il existe des applications indéfiniment dérivables $v_1, . . . , v_n$ de $\mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$ dans A telles que

$$
(z_1-a_1)v_1(\boldsymbol{z}) +\cdots + (z_n-a_n)v_n(\boldsymbol{z}) = 1
$$

pour tout $\boldsymbol{z}= (z_1, . . . , z_n)\in \mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$.

Soit $\boldsymbol{w}= (w_1, . . . , w_n)\in \mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$. Par définition du spectre simultané, il existe $b_1, . . . , b_n$ dans A tels que

$$
(w_1-a_1)b_1+\cdots + (w_n-a_n)b_n= 1
$$

(I, p. 41, n$^o6$). Il existe un voisinage ouvert $W_{\boldsymbol{w}}$ de $\boldsymbol{w}$ tel que l’élément $(z_1-a_1)b_1+\cdots + (z_n-a_n)b_n$ de A est inversible si $\boldsymbol{z}= (z_1, . . . , z_n)$ appartient à $W_{\boldsymbol{w}}$. Pour tout entier $j$ tel que $1\leqslant j\leqslant n$ et tout $\boldsymbol{z}$ dans $W_{\boldsymbol{w}}$, soit alors

$n-1$

$$
u_j(\boldsymbol{z}) =b_j\sum_{i=1}(z_i-a_i)b_i
$$

Les fonctions $u_1, u_2, . . . , u_n$ de $W_{\boldsymbol{w}}$ dans A ainsi définies sont indéfiniment dérivables dans $W_{\boldsymbol{w}}$, et on a

$$
(z_1-a_1)u_1(\boldsymbol{z}) +\cdots + (z_n-a_n)u_n(\boldsymbol{z}) = 1
$$

pour tout $\boldsymbol{z}$ dans $W_{\boldsymbol{w}}$.

Puisque la famille $(W_{\boldsymbol{w}})_{\boldsymbol{w}\in\mathbf{C}^{n-}Sp^n(\boldsymbol{a})}$ est un recouvrement ouvert de $\mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$, il existe un recouvrement ouvert localement fini $\mathscr{W}= (W_{\lambda})_{\lambda\in L}$ (TG, I, p. 70, th. 5) et, pour tout $\lambda \in L$, des fonctions $u_{1\lambda}, . . . , u_{n\lambda}$, à valeurs dans A, définies et indéfiniment dérivables dans $W_{\lambda}$, telles que $(z_1-a_1)u_{1\lambda}(\boldsymbol{z}) +\cdots + (z_n-a_n)u_{n\lambda}(\boldsymbol{z}) = 1$ pour tout $\boldsymbol{z}$ dans $W_{\lambda}$. Soit $(f_{\lambda})_{\lambda\in L}$ une partition de l’unité subordonnée au recouvrement $\mathscr{W}$ formée de fonctions indéfiniment dérivables (VAR, R1, p. 40, 5.3.6). Soit $i$ un entier tel que $1\leqslant i\leqslant n$. Pour tout $\lambda \in L$, soit $u'_{i\lambda}$ l’application de $\mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$ dans A obtenue en prolongeant par 0 la fonction $f_{\lambda}u_{i\lambda}$ dans $(\mathbf{C}^n-$ Sp$^n(\boldsymbol{a}))-W_{\lambda}$. Les fonctions $u'_{i\lambda}$ sont indéfiniment dérivables. La famille (Supp($u'_{i\lambda}$))$_{\lambda\in L}$ étant localement finie, la fonction $v_i=\sum_{\lambda\in L}u'_{i\lambda}$ est définie et indéfiniment dérivable dans

$\mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$.

Soit $\boldsymbol{z}\in \mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$. Notons $L'$ l’ensemble fini des $\lambda \in L$ tels que $\boldsymbol{z}\in W_{\lambda}$. Alors

$$
\sum_{i=1}^n(z_i-a_i)v_i(\boldsymbol{z}) =\sum_{\lambda\in L'}\sum_{i=1}^n(z_i-a_i)u'_{i\lambda}(\boldsymbol{z})
$$

$$
=\sum_{\lambda\in L'}f_{\lambda}(\boldsymbol{z})\sum_{i=1}^n(z_i-a_i)u_{i\lambda}(\boldsymbol{z}) =\sum_{\lambda\in L'}f_{\lambda}(\boldsymbol{z})\cdot 1 = 1
$$

#### Lemme 3 {#ts-i-s4-lem-3 .statement tag=02A0}

Soit $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$. Soit $h$ une application de $\mathbf{C}^n$ dans $\mathbf{C}$, indéfiniment dérivable, égale à 1 au voisinage de Sp$^n(\boldsymbol{a})$ et à support compact. Il existe des applications indéfiniment dérivables $u_1, . . . , u_n$ de $\mathbf{C}^n$ dans A telles que la suite $(h, u_1, . . . , u_n)$ soit adaptée à $\boldsymbol{a}$.

Soient $v_1, . . . ,v_n$ des applications de $\mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$ dans A, indéfiniment dérivables, telles que

$$
\sum_{j=1}^n(z_j-a_j)v_j(\boldsymbol{z}) = 1
$$

pour $\boldsymbol{z}$ dans $\mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$ (lemme 2). Soit $i$ un entier tel que $1\leqslant i\leqslant n$. Posons $u_i(\boldsymbol{z}) = (1-h(\boldsymbol{z}))v_i(\boldsymbol{z})$ si $\boldsymbol{z}\in \mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$ et $u_i(\boldsymbol{z}) = 0$ si $\boldsymbol{z}\in$ Sp$^n(\boldsymbol{a})$. Les applications $u_i$ sont indéfiniment dérivables dans $\mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$ et nulles dans un voisinage de Sp$^n(\boldsymbol{a})$, donc indéfiniment dérivables dans $\mathbf{C}^n$. L’égalité (1) est vraie dans Sp$^n(\boldsymbol{a})$ car les fonctions $u_i$ sont nulles sur Sp$^n(\boldsymbol{a})$ et $h$ est égale à 1 au voisinage de Sp$^n(\boldsymbol{a})$. Elle est aussi vraie sur $\mathbf{C}^n-$ Sp$^n(\boldsymbol{a})$ par construction.

#### Lemme 4 {#ts-i-s4-lem-4 .statement tag=02A1}

Soit $\boldsymbol{a}\in A^n$. Soient $(h, u_1, . . . , u_n)$ une suite adaptée à $\boldsymbol{a}$ et $\omega$ la forme différentielle associée.

a) Pour $i= 1,2, . . . , n$, il existe une forme différentielle $\beta_i$ sur $\mathbf{C}^n$, de degré $n-1$, à coefficients dans A, telle que

$(z_i-a_i)\omega =d(h\beta_i\wedge dz_1\wedge  \cdots  \wedge dz_n)$ ;

b) La forme différentielle $\omega$ est à support compact inclus dans le support de $h$;

c) Il existe une forme différentielle $\beta$ sur $\mathbf{C}^n$, de degré $n-1$, à coefficients dans A, telle que

$$
(n+ 1)h\omega -\omega =d(h\beta \wedge dz_1\wedge  \cdots  \wedge dz_n)
$$

Soit $i$ un entier tel que $1\leqslant i\leqslant n$. Il existe $\varepsilon_i\in  \{-1,1\}$ tel que

$$
\varepsilon_i\bigwedge_{j\not=i}du_j\wedge dz_1\wedge  \cdots  \wedge dz_n=dz_i\wedge \bigwedge_{j\not=i}(du_j\wedge dz_j)
$$

Posons $\beta_i=\varepsilon_i\bigwedge_{j\not=i}du_j$, de sorte que le terme de gauche dans cette formule est $\beta_i\wedge dz_1\wedge  \cdots  \wedge dz_n$ et que $d\beta_i= 0$. Ainsi

$$
d h\beta_i\wedge dz_1\wedge  \cdots  \wedge dz_n=dh\wedge \beta_i\wedge dz_1\wedge  \cdots  \wedge dz_n=
$$

$$
dh\wedge dz_i\wedge \bigwedge_{j\not=i}(du_j\wedge dz_j) = (z_i-a_i)\omega
$$

d’après la formule (3), d’où l’assertion a).

On déduit de l’assertion a) et de la formule (1) la relation

$$
\omega =h\omega + (1-h)\omega =h\omega +\sum_{i=1}^n(z_i-a_i)u_i\omega
$$

$$
=h\omega +\sum_{i=1}^nu_id(h\beta_i\wedge dz_1\wedge  \cdots  \wedge dz_n)
$$

d’où Supp($\omega$ )$\subset$ Supp($h$), ce qui prouve b).

Enfin, posons

$\beta =\sum_{i=1}^n\varepsilon_iu_i\bigwedge_{j\not=i}du_j=\sum_{i=1}^nu_i\beta_i$, et $\tau =h\beta dz_1\wedge  \cdots  \wedge dz_n$.

On a $d\beta =\sum_idu_i\wedge \beta_i$ et donc

$$
d\beta \wedge dz_1\wedge  \cdots  \wedge dz_n=\sum_idu_i\wedge dz_i\wedge \bigwedge_{j\not=i}(du_j\wedge dz_j) =n\omega
$$

Ainsi

$$
d\tau =dh\wedge \beta \wedge dz_1\wedge  \cdots  \wedge dz_n+hd\beta \wedge dz_1\wedge  \cdots  \wedge dz_n
$$

$$
=\sum_{i=1}^nu_idh\wedge dz_i\wedge \bigwedge_{j\not=i}(du_j\wedge dz_j) +nh\omega
$$

$$
=-\sum_{i=1}^nu_i(z_i-a_i)\omega +nh\omega = (h-1)\omega +nh\omega = (n+ 1)h\omega -\omega
$$

compte tenu des formules (3) et (1), d’où c).

Nous nous proposons maintenant d’étudier comment la forme différentielle $\omega$ associée à une suite adaptée à $\boldsymbol{a}$ varie en fonction de cette suite. Nous dirons que des suites $(h, u_1, . . . , u_n)$ et $(h', u'_1, . . . , u'_n)$ adaptées à $\boldsymbol{a}$ sont liées s’il existe une forme différentielle $\psi$ de degré $n-1$ sur $\mathbf{C}^n$, à coefficients dans A et à support contenu dans la réunion des supports de $h$ et de $h'$, telle que les formes différentielles associées $\omega$ et $\omega '$ vérifient

$$
\omega -\omega '=d(\psi \wedge dz_1\wedge dz_2\wedge  \cdots  \wedge dz_n)
$$

Commençons par une modification élémentaire :

#### Lemme 5 {#ts-i-s4-lem-5 .statement tag=02A2}

Soit $\boldsymbol{a}\in A^n$, soit $(h, u_1, . . . , u_n)$ une suite adaptée à $\boldsymbol{a}$, et soit $\omega$ la forme différentielle associée.

Soit $w$ une application indéfiniment dérivable de $\mathbf{C}^n$ dans A et soient $i$ et $j$ des entiers distincts compris entre 1 et $n$. Définissons $u'_1, . . . , u'_n$ par

$$
u'_i=u_i+ (z_j-a_j)w,u'_j=u_j-(z_i-a_i)w
$$

$u'_k=u_k$ pour $k\not=i, j$.

Alors la suite $(h, u'_1, . . . , u'_n)$ est adaptée à $\boldsymbol{a}$ et est liée à la suite $(h, u_1, . . . , u_n)$.

Notons $d\boldsymbol{z}=dz_1\wedge  \cdots  \wedge dz_n$. Comme

$$
\sum_{k=1}^n(z_k-a_k)u'_k(\boldsymbol{z}) =\sum_{k=1}^n(z_k-a_k)u_k(\boldsymbol{z}) +w(\boldsymbol{z})(z_j-a_j)(z_i-a_i)
$$

$$
-w(\boldsymbol{z})(z_i-a_i)(z_j-a_j) = 1-h(\boldsymbol{z})
$$

pour tout $z\in \mathbf{C}^n$, la suite $(h, u'_1, . . . , u'_n)$ est adaptée à $\boldsymbol{a}$. De plus, on a

$$
du'_i\wedge du'_j\wedge dz_1\wedge  \cdots  \wedge dz_n=
$$

$$
du_i+w dz_j+ (z_j-a_j)dw\wedge du_j-w dz_i-(z_i-a_i)dw\wedge d\boldsymbol{z}
$$

= $du_i\wedge du_j-(z_i-a_i)du_i\wedge dw-(z_j-a_j)du_j\wedge dw\wedge d\boldsymbol{z}$ Il existe donc $\varepsilon \in  \{-1,1\}$ tel que $\varepsilon (\omega -\omega ')$ est égal à

$$
du'_i\wedge du'_j\wedge \bigwedge_{k\not=i,j}du'_k\wedge d\boldsymbol{z}-du_i\wedge du_j\wedge \bigwedge_{k\not=i,j}du_k\wedge d\boldsymbol{z}
$$

$$
=-(z_i-a_i)du_i\wedge dw+ (z_j-a_j)du_j\wedge dw\wedge \bigwedge_{k\not=i,j}du_k\wedge d\boldsymbol{z}
$$

$$
=-\sum_{k=1}^n(z_k-a_k)du_k\wedge dw\wedge \bigwedge_{k\not=i,j}du_k\wedge d\boldsymbol{z}
$$

et, compte tenu de (2), ceci est égal à

$$
dh\wedge dw\wedge \bigwedge_{k\not=i,j}du_k\wedge d\boldsymbol{z}=dh dw\wedge \bigwedge_{k\not=i,j}du_k\wedge d\boldsymbol{z}
$$

d’où le résultat.

#### Lemme 6 {#ts-i-s4-lem-6 .statement tag=02A3}

Soit $\boldsymbol{a}\in A^n$. Toutes les suites adaptées à $\boldsymbol{a}$ sont liées.

Soient $(h, u_1, . . . , u_n)$ et $(h', u'_1, . . . , u'_n)$ des suites adaptées à $\boldsymbol{a}$, et notons $\omega$ et $\omega '$ les formes différentielles associées.

Définissons les applications indéfiniment dérivables

$$
w_{ij}=u'_iu_j-u_iu'_j,1\leqslant i\leqslant n,1\leqslant j\leqslant n
$$

$$
s_i=u'_ih-u_ih',1\leqslant i\leqslant n
$$

de sorte que $w_{ji}=-w_{ij}$, et Supp($s_i$)$\subset$ Supp($h$)$\cup$ Supp($h'$).

Posons $u''_i=u'_i-s_i,\boldsymbol{u}= (u_1, . . . , u_n)$ et $\boldsymbol{u}''= (u''_1, . . . , u''_n)$. Notons aussi $\boldsymbol{v}_{ij}$ l’application de $\mathbf{C}^n$ dans $A^n$ dont la $i$-ème composante est $(z_j-a_j)w_{ij}$, dont la $j$-ème composante est $(z_i-a_i)w_{ji}=-(z_i-a_i)w_{ij}$, et dont les autres composantes sont nulles. Alors on a

$$
\boldsymbol{u}''=\boldsymbol{u}+\sum_{i<j}\boldsymbol{v}_{ij}
$$

En effet, pour tout entier $k$ tel que $1\leqslant k\leqslant n$, la $k$-ème composante du membre de droite est

$$
u_k+\sum^{k-1}_{i=1}(z_i-a_i)w_{ki}+\sum_{j=k+1}^n(z_j-a_j)w_{kj}=u_k+\sum_{i=1}^n(z_i-a_i)w_{ki}
$$

$$
=u_k+u'_k\sum_{i=1}^n(z_i-a_i)u_i-u_k\sum_{i=1}^n(z_i-a_i)u'_i
$$

$$
=u_k+ (1-h)u'_k-(1-h')u_k=u'_k-s_k
$$

Par récurrence, on déduit du lemme 5, appliqué aux entiers $i$ et $j$ et aux applications $w_{ij}$, que la suite $(h, u''_1, . . . , u''_n)$ est adaptée à $\boldsymbol{a}$ et est liée à $(h, u_1, . . . , u_n)$. Soit $\omega ''$ la forme différentielle associée à $(h, u''_1, . . . , u''_n)$. Comme $u''_i=u'_i-s_i$, on a

$$
\omega ''-\omega '=d(u'_1-s_1)\wedge dz_1\wedge  \cdots  \wedge d(u'_n-s_n)\wedge dz_n-
$$

$$
du'_1\wedge dz_1\wedge  \cdots  \wedge du'_n\wedge dz_n
$$

qui s’exprime comme une combinaison linéaire, avec coefficients 1 ou $-1$, de formes différentielles de la forme

$$
\xi_{I_1,I_2}=\bigwedge_{i\in I_1}ds_i\wedge \bigwedge_{i\in I_2}du'_i\wedge dz_1\wedge  \cdots  \wedge dz_n
$$

où $I_1$ (resp. $I_2)$ est une partie non vide (resp. une partie) de $\{1, . . . , n\}$. Chaque forme différentielle $\xi_{I_1,I_2}$ s’écrit aussi sous la forme

$$
d(\widetilde{\psi}\wedge dz_1\wedge  \cdots  \wedge dz_n)
$$

où le support de la forme différentielle $\widetilde{\psi}$ est contenu dans le support de $s_i$ pour tout $i\in I_1$. Comme $I_1$ est non-vide, ce support est contenu dans Supp($h$)$\cup$ Supp($h'$). Par conséquent, $(h, u''_1, . . . , u''_n)$ est liée à $(h', u'_1, . . . , u'_n)$, et le lemme en résulte en écrivant

$$
\omega -\omega '= (\omega -\omega '') + (\omega ''-\omega ')
$$

### 4. Construction des applications $\Theta_{\boldsymbol{a}}$

Soit $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$ et soit U un voisinage ouvert de Sp$^n(\boldsymbol{a})$. Soit $h$ une application indéfiniment dérivable, égale à 1 au voisinage de Sp$^n(\boldsymbol{a})$ et telle que le support de $h$ soit compact et contenu dans U (lemme 1 de I, p. 52). D’après le lemme 3 de I, p. 54, il existe des applications indéfiniment dérivables $(u_1, . . . , u_n)$ de $\mathbf{C}^n$ dans A telles que la suite $(h, u_1, . . . , u_n)$ soit adaptée à $\boldsymbol{a}$. Soit $\omega$ la forme différentielle associée ; elle est à support compact contenu dans U (lemme 4 de I, p. 54). Il existe une fonction indéfiniment dérivable $\psi$ à support compact dans U et à valeurs dans A telle que

$$
\omega =\psi  dx_1\wedge dy_1\wedge  \cdots  \wedge dx_n\wedge dy_n
$$

où $x_j+iy_j$ sont les fonctions coordonnées sur $\mathbf{C}^n$, identifié avec $\mathbf{R}^{2n}$. Soit $\mu$ la mesure de Lebesgue sur $\mathbf{R}^{2n}$.

Soit $f\in \mathscr{C}(U; A)$. La forme différentielle $f \omega |U$ sur U est continue et à support compact. La mesure vectorielle associée à cette forme différentielle (VAR, R2, 10.4.3 et 10.4.4) est la mesure vectorielle $f \psi \cdot \mu$; c’est une mesure de base $\mu$ (INT, VI, §2, n$^o4$, déf. 4), son support est compact et contenu dans le support de $\omega$. Cette mesure est majorable relativement à la norme de A (INT, VI, §2, n$^o4$, prop. 8) ; on note $\|f \omega \|$ la mesure positive sur $\mathbf{C}^n$ qui lui est associée (INT, VI, §2, n$^o3$, déf. 3).

D’après INT, VI, §2, n$^o4$, prop. 8, b), on a

$$
\|f \omega \|=\|f \psi \cdot \mu\|=\|f \psi \| \cdot \mu=\|f\| \|\omega \|
$$

En particulier, l’intégrale de la forme différentielle $f \omega$ sur U vérifie

$$
\int_Uf \omega \leqslant \int_U\|f\| \|\omega \|
$$

(INT, VI, §2, n$^o3$, prop. 5).

#### Lemme 7 {#ts-i-s4-lem-7 .statement tag=02A4}

Pour toute fonction $f\in \mathscr{O}(U; A)$, l’intégrale $\int_Uf \omega$ est un élément de A qui ne dépend que de $\boldsymbol{a}$ et du germe de $f$ au voisinage de Sp$^n(\boldsymbol{a})$. Il vérifie l’inégalité

(4) $\int f \omega \leqslant \int\|\omega \|$ sup $\|f(z)\|$,

U U $z\in$Supp($h$)

et

$$
\int_U(af)\omega =a\int_Uf \omega
$$

pour tout $a\in A$.

On a vu ci-dessus que l’intégrale est définie pour $f\in \mathscr{C}(U; A)$ et vérifie

$\int f \omega \leqslant \int\|f\| \|\omega \|\leqslant \int\|\omega \|$ sup $\|f(z)\|$.

U U U $z\in$Supp($h$)

De plus, pour tout $a\in A$ et tout $f\in \mathscr{C}(U; A)$, on a

$$
\int_U(af)\omega =a\int_Uf \omega
$$

(INT, VI, §2, n$^o2$, prop. 2 appliqué à la multiplication par $a)$.

Soit $(h', u'_1, . . . , u'_n)$ une suite adaptée à $\boldsymbol{a}$ telle que Supp($h'$)$\subset U$. Soit $\omega '$ la forme différentielle associée. D’après le lemme 6 de I, p. 57, il existe une forme différentielle $\psi$ sur $\mathbf{C}^n$ de degré $n-1$, à coefficients dans A et à support contenu dans Supp($h$)$\cup$ Supp($h'$)$\subset U$, telle que

$$
\omega -\omega '=d(\psi \wedge dz_1\wedge  \cdots  \wedge dz_n)
$$

Soit $f\in \mathscr{O}(U; A)$. L’application $f$ étant holomorphe, on a

$$
^n\partial f
$$

$$
df=\sum dz_i
$$

$$
\partial z_i
$$

$i=1$

(VAR, R2, p. 24, 8.8.9) et donc

$$
f(\omega -\omega ') =f d(\psi \wedge dz_1\wedge  \cdots  \wedge dz_n) =d(f \psi \wedge dz_1\wedge  \cdots  \wedge dz_n)
$$

D’après la formule de Stokes (VAR, R2, p. 48, 11.2.3), on a alors

$$
\int_Uf(\omega -\omega ') = 0
$$

Ainsi l’élément $\int_Uf \omega$ ne dépend pas du choix de la suite $(h, u_1, . . . , u_n)$.

Démontrons pour conclure que $\int_Uf \omega$ ne dépend que du germe de $f$ au voisinage de Sp$^n(\boldsymbol{a})$. Soient U et $U'$ des voisinages ouverts de Sp$^n(\boldsymbol{a})$. Soient $f\in \mathscr{O}(U; A)$ et $f'\in \mathscr{O}(U'; A)$ telles que $f$ et $f'$ coïn-cident sur un voisinage ouvert $U''$ de Sp$^n(\boldsymbol{a})$. Il existe une application $h$ de $\mathbf{C}^n$ dans $\mathbf{C}$, indéfiniment dérivable, égale à 1 au voisinage de Sp$^n(\boldsymbol{a})$, et à support compact inclus dans $U''$ (lemme 1 de I, p. 52), et il existe $(u_1, . . . , u_n)$ telle que la suite $(h, u_1, . . . , u_n)$ est adaptée à $\boldsymbol{a}$ (lemme 3 de I, p. 54). Soit $\omega$ la forme différentielle associée. Comme Supp($\omega$ )$\subset$ Supp($h$)$\subset U''$ (lemme 4, b) de I, p. 54), on a

$$
\int_Uf \omega =\int_{U''}f \omega =\int_{U''}f'\omega =\int_{U'}f'\omega
$$

ce qui achève la démonstration.

Ce lemme démontre qu’il existe une unique application A-linéaire $\Theta_{\boldsymbol{a}}$ de $\mathscr{O}$(Sp$^n(\boldsymbol{a}); A)$ dans A telle que

$n$! $\int$

$$
\Theta_{\boldsymbol{a}}(f) =_n\widetilde{f \omega} \tag{5}
$$

$$
(2i\pi )_U
$$

pour tout ouvert U et tout représentant $\widetilde{f}\in \mathscr{O}(U; A)$ d’un germe $f\in \mathscr{O}$(Sp$^n(\boldsymbol{a}); A)$. L’application linéaire $\Theta_{\boldsymbol{a}}$ est continue d’après l’inégalité (4) et EVT, II, p. 29, prop. 5.

### 5. Propriétés des applications $\Theta_{\boldsymbol{a}}$

On rappelle (VAR, R2, p. 46 et p. 47, 11.1.3, d)) que si K est une partie compacte de $\mathbf{C}$, il existe un système fondamental de voisinages compacts V de K qui sont des pièces de $\mathbf{C}$ (c’est-à-dire, pour tout $x\in V$, il existe une carte $(U, \varphi ,\mathbf{C})$ de $\mathbf{C}$ en $x$ tel que $\varphi (U\cap K)$ est un ouvert d’un demi-espace fermé de $\mathbf{C})$. On note alors $\partial V$ le bord de la pièce V muni de l’orientation déduite de l’orientation de $\mathbf{C}$ (VAR, R2, p. 47) et $dz$ la différentielle de l’injection $\partial V\rightarrow \mathbf{C}$.

#### Proposition 1 {#ts-i-s4-prop-1 .statement tag=02A5}

Soit $a$ un élément de A, soit U un voisinage ouvert de Sp($a$), et soit $f\in \mathscr{O}(U; A)$. Soit V un voisinage compact de Sp($a$) contenu dans U et tel que V soit une pièce de $\mathbf{C}$.

Alors $z\mapsto f(z)(z-a)^{-1}$ est continue sur $\partial V$, la forme différentielle $f(z)(z-a)^{-1}dz$ est intégrable sur $\partial V$ et on a

1 $\int_{-1}$

$$
\Theta_a(f) =f(z)(z-a)dz
$$

$$
2i\pi_{\partial V}
$$

Soit $h$ une application de $\mathbf{C}$ dans $\mathbf{C}$, indéfiniment dérivable, égale à 1 au voisinage de Sp($a$) et à support compact contenu dans l’intérieur de V (lemme 1 de I, p. 52). Soit $u$ une application de $\mathbf{C}$ dans A telle que $(h, u)$ est adaptée à $a($cf. exemple 3 de I, p. 53). La forme différentielle associée est $\omega =du\wedge dz$. Il vient $f \omega =f du\wedge dz=d(f u dz)$ puisque $f$ est holomorphe. De plus, $u(z) = (z-a)^{-1}$ sur le bord de V. Par ailleurs, la forme différentielle $f u dz$ est de classe $C^1$ sur U. Donc

$$
2i\pi \Theta_a(f) =\int_Vd(f u dz) =\int_{\partial V}f u dz=\int_{\partial V}f(z)(z-a)^{-1}dz
$$

d’après la formule (5) et la formule de Stokes pour la pièce V (VAR, R2, p. 47, 11.2.3).

#### Corollaire {#ts-i-s4-n5-cor-1 .statement tag=02A6}

Soit $a\in A$. On a $\Theta_a(1) = 1$.

Soit $R> \varrho (a)$ un nombre réel. Soit V le disque fermé de centre 0 et de rayon R, de sorte que Sp($a$)$\subset \mathring{V}$. C’est une pièce de $\mathbf{C}$ dont le bord $\partial V$ est le cercle de centre 0 et de rayon R. Pour $z\in \mathbf{C}-\mathring{V}$, on a la formule $(z-a)^{-1}=z^{-1}(1-z^{-1}a)^{-1}=\sum^{+\infty}_{j=1}z^{-j}a^{j-1}$. La série converge

uniformément pour $z\in \partial V$. On a donc

1 $+\infty j-1\int-j$

$$
\Theta_a(1) =\sum azdz= 1
$$

$$
2i\pi_{j=1\partial V}
$$

puisque

$$
\int_{\partial V}z^jdz= 0
$$

pour tout entier $j\not=-1$ et

$$
\int_{\partial V}z^{-1}dz= 2i\pi
$$

(VAR, R2, p. 44, 10.4.5, et p. 47, 11.2.1, exemple).

#### Lemme 8 {#ts-i-s4-lem-8 .statement tag=02A7}

Soit U un ouvert de $\mathbf{C}^n$. Soit $\omega_1$ une forme différentielle continue de degré $n$ dans U à support compact et à valeurs dans A (resp. $\omega_2$ une forme différentielle continue de degré 2 dans $\mathbf{C}$ à support compact et à valeurs dans $\mathbf{C})$. Notons $\pi_1$ et $\pi_2$ les projections canoniques de $U\times \mathbf{C}$ sur U et $\mathbf{C}$. La forme différentielle $\pi_1^*\omega_1\wedge \pi_2^*\omega_2$ sur $U\times \mathbf{C}$ est continue à support compact et à valeurs dans A. On a

$$
\int_{U\times\mathbf{C}}\pi_1^*\omega_1\wedge \pi^*_2\omega_2=\int_{\mathbf{C}}\omega_2(\int_U\omega_1
$$

Soient $\mu_n$ la mesure de Lebesgue sur $\mathbf{C}^n$ et $\mu_1$ la mesure de Lebesgue sur $\mathbf{C}$. Il existe $\psi_1\in \mathscr{K}(U; A)$ et $\psi_2\in \mathscr{K}(\mathbf{C})$ tels que la mesure vectorielle associée à $\omega_1$ est égale à $\psi_1\cdot \mu_n$, et la mesure vectorielle associée à $\omega_2$ est égale à $\psi_2\cdot \mu_1$. La mesure vectorielle associée à la forme différentielle $\pi^*_1\omega_1\wedge \pi_2^*\omega_2$ est $(\psi_1\otimes \psi_2)\cdot \mu_n\otimes \mu_1$.

Soit $\ell$ une forme linéaire continue sur A. D’après INT, VI, §2, n$^o2$, déf. 2 et la définition de la mesure produit (INT, III, §4, n$^o1$, déf. 1), il vient

$$
\ell \int_{U\times\mathbf{C}}\pi_1^*\omega_1\wedge \pi^*_2\omega_2=\int_{U\times\mathbf{C}}\ell \circ (\psi_1\otimes \psi_2)\mu_n\otimes \mu_1
$$

$$
=\int\psi_2(z)\ell (\psi_1(x))d\mu_n(x)d\mu_1(z)
$$

= $\int^{U\times\mathbf{C}}_{\mathbf{C}}\psi_2(z)d\mu_1(z)\int_U\ell (\psi_1(x))d\mu_n(x)$

= $\int_{\mathbf{C}}\psi_2\mu_1\ell \int_U\psi_1\mu_n$, d’où le résultat (INT VI, loc. cit.).

#### Lemme 9 {#ts-i-s4-lem-9 .statement tag=02A8}

Soit $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$. Soient $p\in \mathbf{N}$ et $\boldsymbol{a}'$ = $(a_{n+1}, . . . , a_{n+p})\in A^p$. Alors on a $\Theta_{(\boldsymbol{a},\boldsymbol{a}')}\circ \pi_{n,n+p}^*= \Theta_{\boldsymbol{a}}$. En particulier, on a $\Theta_{\boldsymbol{a}}(1) = 1$.

Comme on a $\pi_{n,n+p}=\pi_{n,n+1}\circ \cdots \circ \pi_{n+p-1,n+p}$, il suffit de démontrer la première assertion lorsque $p= 1$, ce qu’on suppose désormais. On note simplement $\pi =\pi_{n,n+1}$. Il suffit alors de démontrer que, pour tout voisinage ouvert U de Sp$^n(\boldsymbol{a})$, et toute fonction $f\in \mathscr{O}(U; A)$, on a $\Theta_{(\boldsymbol{a},a_{n+1})}(f\circ \pi ) = \Theta_{\boldsymbol{a}}(f)$. Notons $g=f\circ \pi$. Soit $h$ (resp. $h')$ une application de $\mathbf{C}^n$ dans $\mathbf{C}$ (resp. de $\mathbf{C}$ dans $\mathbf{C})$, indéfiniment dérivable, égale à 1 au voisinage de Sp$^n(\boldsymbol{a})$ (resp. de Sp($\boldsymbol{a}'$)), à support compact contenu dans U (resp. dans $\mathbf{C})$. Il existe des applications $(u_1, . . . , u_n)$ de $\mathbf{C}^n$ dans A, indéfiniment dérivables, telles que la suite $(h, u_1, . . . , u_n)$ est adaptée à $\boldsymbol{a}$ (lemme 3 de I, p. 54), et une application indéfiniment dérivable $u_{n+1}$ de $\mathbf{C}$ dans A telle que le couple $(h', u_{n+1})$ est adapté à $a_{n+1}($loc. cit.)

Pour $\boldsymbol{z}\in \mathbf{C}^n$ et $z_{n+1}\in \mathbf{C}$, notons $h''(\boldsymbol{z}, z_{n+1}) =h(\boldsymbol{z})h'(z_{n+1})$ et $u''_{n+1}(\boldsymbol{z}, z_{n+1}) =h(\boldsymbol{z})u_{n+1}(z_{n+1})$. Les fonctions $h''$ et $u''_{n+1}$ sont indéfiniment dérivables dans $\mathbf{C}^{n+1}$. La fonction $h''$ est égale à 1 au voisinage de Sp$^{n+1}(\boldsymbol{a}, a_{n+1})$, et a support compact contenu dans $U\times \mathbf{C}$. Pour tout $\boldsymbol{w}= (\boldsymbol{z}, z_{n+1})\in \mathbf{C}^{n+1}$, on a

$$
(z_1-a_1)(u_1\circ \pi )(\boldsymbol{w}) +\cdots + (z_n-a_n)(u_n\circ \pi )(\boldsymbol{w})
$$

$$
+ (z_{n+1}-a_{n+1})u''_{n+1}(\boldsymbol{w}) = 1-h(\boldsymbol{z}) +h(\boldsymbol{z})(1-h'(z_{n+1}))
$$

$$
= 1-h''(\boldsymbol{w})
$$

ce qui démontre que la suite $(h'', u_1\circ \pi , . . . , u_n\circ \pi , u''_{n+1})$ est adaptée à $(\boldsymbol{a}, a_{n+1})$. Soit $\omega$ la forme différentielle associée.

La forme différentielle $du_1\wedge dz_1\wedge  \cdots  \wedge du_n\wedge dz_n\wedge dh$ sur $\mathbf{C}^n$ est de degré $2n+ 1$, donc est nulle. Par suite

$$
\omega =d(u_1\circ \pi )\wedge dz_1\wedge  \cdots  \wedge d(u_n\circ \pi )\wedge dz_n\wedge du''_{n+1}\wedge dz_{n+1}
$$

$$
= (h\circ \pi )d(u_1\circ \pi )\wedge dz_1\wedge  \cdots  \wedge d(u_n\circ \pi )\wedge dz_n\wedge du_{n+1}\wedge dz_{n+1}
$$

Comme $g=f\circ \pi$, la formule (5) et le lemme 8 impliquent

$(n+$ 1)! $\int(n+$ 1)! $\int$

$$
\Theta_{\boldsymbol{a},\boldsymbol{a}'}(g) =g\omega =du_{n+1}\wedge dz_{n+1}
$$

$$
(2i\pi )^{n+1}_{U\times\mathbf{C}}(2i\pi )^{n+1}_{\mathbf{C}}
$$

$$
\times \int_Uf h du_1\wedge dz_1\wedge  \cdots  \wedge du_n\wedge dz_n
$$

D’une part, on a

$$
\int_{\mathbf{C}}du_{n+1}\wedge dz_{n+1}= 2i\pi \Theta^{\mathbf{C}}_{a_{n+1}}(1) = 2i\pi \cdot 1
$$

d’après le corollaire 5. D’autre part, la partie c) du lemme 4 de I, p. 54 et le fait que l’intégrale d’une forme fermée est nulle (VAR, R2, p. 48, 11.2.4) entraînent

$$
(n+ 1)\int_Uf hdu_1\wedge dz_1\wedge  \cdots  \wedge du_n\wedge dz_n=
$$

$$
\int(2i\pi )^n
$$

$$
f du_1\wedge dz_1\wedge  \cdots  \wedge du_n\wedge dz_n=\Theta_{\boldsymbol{a}}(f)
$$

$_Un$!

Ainsi on obtient

$(n+$ 1)! $(2i\pi )^n$

$$
\Theta_{\boldsymbol{a},\boldsymbol{a}'}(g) =\times \Theta_{\boldsymbol{a}}(f)\times 2i\pi = \Theta_{\boldsymbol{a}}(f)
$$

$(2i\pi )^{n+1}(n+$ 1)!

Finalement, la formule $\Theta_{\boldsymbol{a}}(1) = 1$ résulte de ce qui précède et du corollaire de la prop. 1.

#### Lemme 10 {#ts-i-s4-lem-10 .statement tag=02A9}

Soit $\boldsymbol{a}\in A^n$. Soient $g$ une fonction polynomiale sur $\mathbf{C}^n$ à coefficients dans A et $f\in \mathscr{O}$(Sp$^n(\boldsymbol{a}); A)$. On a $\Theta_{\boldsymbol{a}}(gf) =g(\boldsymbol{a})\Theta_{\boldsymbol{a}}(f)$. En particulier, on a $\Theta_{\boldsymbol{a}}(g) =g(\boldsymbol{a})$.

D’après le lemme 9, il suffit de démontrer la première assertion.

Notons $z_1, . . . , z_n$ les fonctions coordonnées sur $\mathbf{C}^n$. Puisque l’application $\Theta_{\boldsymbol{a}}$ est A-linéaire, il suffit de prouver l’assertion du lemme lorsque $g=z_1^{e_1}\cdots z^e_{n^n}$, où $(e_1, . . . , e_n)\in \mathbf{N}^n$. Procédant par récurrence sur $e_1+\cdots +e_n$, on se ramène au cas où il existe un entier $i$ tel que $1\leqslant i\leqslant n$ et $g=z_i$.

Soit U un voisinage ouvert de Sp$^n(\boldsymbol{a})$. Soit $(h, u_1, . . . , u_n)$ une suite adaptée à $\boldsymbol{a}$ telle que le support de $h$ est contenu dans U (lemme 1 de I, p. 52 et lemme 3 de I, p. 54), et soit $\omega$ la forme différentielle associée. D’après le lemme 4, a) de I, p. 54, il existe une forme différentielle $\beta$ telle que

$$
(z_i-a_i)\omega =d(h\beta \wedge dz_1\wedge  \cdots  \wedge dz_n)
$$

Par conséquent, pour toute fonction $f\in \mathscr{O}(U; A)$, on a

$$
(z_i-a_i)f \omega =f d(h\beta \wedge dz_1\wedge  \cdots  \wedge dz_n) =d(f h\beta \wedge dz_1\wedge  \cdots  \wedge dz_n)
$$

puisque $f$ est holomorphe, de sorte que $df\wedge dz_1\wedge  \cdots  \wedge dz_n= 0$. Appliquant la formule de Stokes (VAR, R2, p. 48, 11.2.4), on obtient $\int_U(z_i-a_i)f \omega = 0$, d’où

$n$! $\int n$! $\int$

$$
\Theta_{\boldsymbol{a}}(z_if) =z_if \omega =a_if \omega =a_i\Theta_{\boldsymbol{a}}(f)
$$

$$
(2i\pi )^n_U(2i\pi )^n_U
$$

d’après la formule (5). Le résultat en découle.

#### Proposition 2 {#ts-i-s4-prop-2 .statement tag=02AA}

Soient $\varrho_1, . . . , \varrho_n$ des réels $>0$ et soit $U\subset \mathbf{C}^n$ le polydisque produit des disques ouverts de centre 0 et de rayon $\varrho_i$. Soit

$$
\sum c(k_1, . . . , k_n)X^k_{1^1}\cdots X^k_{n^n}\in A[[X_1, . . . ,X_n]]
$$

$(k_1,...,k_n)\in \mathbf{N}^n$

une série formelle à coefficients dans A. Supposons que cette série converge dans U, et notons $f$ la fonction holomorphe dans U qui en est la somme.

Soit $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$ tel que $\varrho (a_i)< \varrho_i$ pour $1\leqslant i\leqslant n$. Alors Sp$^n(\boldsymbol{a})\subset U$, la famille $(c(k_1, . . . , k_n)a^k_{1^1}\cdots a^k_{n^n})$ d’éléments de A est absolument sommable, et

$$
\Theta_{\boldsymbol{a}}(f) =\sum c(k_1, . . . , k_n)a^k_{1^1}\cdots a^k_{n^n}
$$

$(k_1,...,k_n)\in \mathbf{N}^n$

Pour tout caractère $\chi$ de A et tout entier $i$ tel que $1\leqslant i\leqslant n$, on a $|\chi (a_i)|\leqslant \varrho (a_i)< \varrho_i$, donc Sp$^n(\boldsymbol{a})\subset U$ par définition du spectre simultané. Soient $z_1, . . . , z_n$ les restrictions à U des fonctions coordonnées sur $\mathbf{C}^n$. Alors la famille $(c(k_1, . . . , k_n)z_1^{k_1}\cdots z^k_{n^n})$ est sommable dans $\mathscr{O}(U; A)$ et de somme $f$. Compte tenu du lemme 10 et de la continuité de l’application $\Theta^U_{\boldsymbol{a}}$, la famille $(c(k_1, . . . , k_n)a^k_{1^1}. . . a^k_{n^n})$ est donc sommable dans A et de somme $\Theta_{\boldsymbol{a}}(f)$. Pour $1\leqslant i\leqslant n$, soit $\lambda_i$ un nombre réel tel que $\varrho (a_i)< \lambda_i< \varrho_i$. Il existe $M_i<+\infty$ tel que $\|a^k_i\|\leqslant M_i\lambda^k_i$ pour tout entier $k\geqslant 0$. On a alors

$$
\sum\|c(k_1, . . . , k_n)\| \|a^k_{1^1}\cdots a^k_{n^n}\|\leqslant
$$

$(k_1,...,k_n)\in \mathbf{N}^n$

$M_1\cdots M_n\sum\|c(k_1, . . . , k_n)\|\lambda^k_{1^1}\cdots \lambda^k_{n^n}$

$(k_1,...,k_n)\in \mathbf{N}^n$ qui est fini par hypothèse, donc la famille $(c(k_1, . . . , k_n)a^k_{1^1}\cdots a^k_{n^n})$ est absolument sommable.

#### Corollaire {#ts-i-s4-n5-cor-2 .statement tag=02AB}

Supposons A non nulle. Soit $\boldsymbol{a}\in \mathbf{C}^n\subset A^n$. On a Sp$^n_A(\boldsymbol{a}) =\{\boldsymbol{a}\}$. Pour tout germe $f\in \mathscr{O}(\{\boldsymbol{a}\}; A)$, on a $\Theta_{\boldsymbol{a}}(f) =f(\boldsymbol{a})$.

#### Proposition 3 {#ts-i-s4-prop-3 .statement tag=02AC}

Soient B une algèbre de Banach unifère commutative et $\varphi$ un morphisme unifère continu de A dans B. Soit $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$. Posons $\boldsymbol{b}= (\varphi (a_1), . . . , \varphi (a_n))$, de sorte que Sp$^n_B(\boldsymbol{b})\subset$ Sp$^n_A(\boldsymbol{a})$. Pour tout $f\in \mathscr{O}$(Sp$^n_A(\boldsymbol{a}); A)$, on a

$$
\varphi (\Theta_{\boldsymbol{a}}(f)) = \Theta_{\boldsymbol{b}}(\varphi_*(f))
$$

où $\varphi_*(f)$ désigne le germe de $\varphi \circ f$ au voisinage de Sp$^n_B(\boldsymbol{b})$.

Il suffit de démontrer que pour tout voisinage ouvert U de Sp$^n_A(\boldsymbol{a})$ et tout $f\in \mathscr{O}(U; A)$, on a $\varphi (\Theta_{\boldsymbol{a}}(f)) = \Theta_{\boldsymbol{b}}(\varphi \circ f)$, où $\varphi \circ f\in \mathscr{O}(U; B)$. Soit $(h, u_1, . . . , u_n)$ une suite adaptée à $\boldsymbol{a}$, où le support de $h$ est contenu dans U (lemme 1 de I, p. 52 et lemme 3 de I, p. 54). Notons $\omega$ la forme différentielle associée. Pour tout $\boldsymbol{z}\in \mathbf{C}^n$, on a

$$
\sum_{j=1}^n(z_j-b_j)\varphi (u_i(\boldsymbol{z})) =\varphi \sum_{j=1}^n(z_j-a_j)u_j(\boldsymbol{z})= 1-h(\boldsymbol{z})
$$

de sorte que la suite $(h, \varphi \circ u_1, . . . , \varphi \circ u_n)$ est adaptée à $\boldsymbol{b}$. Soit $\omega '$ la forme différentielle associée. Notons $\mu$ la mesure de Lebesgue sur $\mathbf{C}^n$. Soit $f\in \mathscr{O}(U; A)$. Écrivons $\psi \cdot \mu$ la mesure vectorielle associée à la forme différentielle $f \omega$. La mesure vectorielle associée à la forme différentielle

$$
(\varphi \circ f)\omega '= (\varphi \circ f)d(\varphi \circ u_1)\wedge dz_1\wedge  \cdots  \wedge d(\varphi \circ u_n)\wedge dz_n
$$

est égale à $(\varphi \circ \psi )\cdot \mu$. Donc, d’après la formule (5), et INT, VI, §2, n$^o2$, prop. 2, on a

$n$! $\int n$! $\int$

$$
\Theta_{\boldsymbol{b}}(\varphi \circ f) =(\varphi \circ f)\mu=\varphi \psi  \mu=\varphi (\Theta_{\boldsymbol{a}}(f))
$$

$$
(2i\pi )^n_U(2i\pi )^n_U
$$

comme il était demandé.

#### Corollaire 1 {#ts-i-s4-prop-3-cor-1 .statement tag=02AD}

Soient $\chi \in \mathsf{X}(A)$ et $\boldsymbol{a}\in A^n$. Pour tout germe $f\in \mathscr{O}$(Sp$^n(\boldsymbol{a}))$, on a $\chi (\Theta_{\boldsymbol{a}}(f)) =f(\chi (a_1), . . . , \chi (a_n))$.

C’est une conséquence de la proposition 3, appliquée au morphisme unifère continu $\chi : A\rightarrow \mathbf{C}$ (th. 1 de I, p. 29), et du corollaire de la prop. 2, appliqué à l’algèbre de Banach $\mathbf{C}$.

#### Remarque {#ts-i-s4-n5-rem-1 .statement tag=02AE}

Supposons que l’algèbre A soit sans radical. Soit $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$. D’après la prop. 8 de I, p. 38, l’application $\Theta^U_{\boldsymbol{a}}$ est l’unique application $\varphi$ de $\mathscr{O}(U)$ dans A telle que $\chi (\varphi (f)) =f(\chi (a_1), . . . , \chi (a_n))$ pour tout $\chi \in \mathsf{X}(A)$ et toute fonction $f\in \mathscr{O}(U)$.

#### Corollaire 2 {#ts-i-s4-prop-3-cor-2 .statement tag=02AF}

Soit $p$ un entier $\geqslant$ 1. Pour toute famille $(f_1, . . . , f_p)$ d’éléments de $\mathscr{O}$(Sp$^n(\boldsymbol{a}))$, on a

Sp$^p((\Theta_{\boldsymbol{a}}(f_1), . . . ,\Theta_{\boldsymbol{a}}(f_p))) = (f_1, . . . , f_p$)(Sp$^n(\boldsymbol{a}))$.

En particulier, pour tout $f\in \mathscr{O}$(Sp$^n(\boldsymbol{a}))$, on a Sp(Θ$_{\boldsymbol{a}}(f)) =f$(Sp$^n(\boldsymbol{a}))$.

Ceci résulte du cor. 1 et de la définition du spectre simultané.

#### Exemple {#ts-i-s4-n5-exa-1 .statement tag=02AG}

Soit A l’algèbre de Banach complexe des fonctions sur le cercle unité à série de Fourier absolument convergente (I, p. 19, exemple 8). Soit $\varphi \in$ A. Soit $f$ un germe de fonction holomorphe au voisinage de l’ensemble des valeurs de $\varphi$. Alors $\psi = \Theta_{\varphi}(f)$ est une série de Fourier absolument convergente qui pour tout $u\in \mathbf{U}$ vérifie $\psi (u) =f(\varphi (u))$ (cor. 1, appliqué aux caractères $\varphi \mapsto \varphi (u)$). Autrement dit, la fonction $f\circ \varphi$ sur le cercle unité a également une série de Fourier absolument convergente (« théorème de P. Lévy »). Ce résultat généralise le théorème de Wiener (I, p. 38, exemple 4), qui concerne le cas de la fonction $f(z) = 1/z$ sur $\mathbf{C}-\{0\}$ lorsque $\varphi$ ne s’annule pas.

### 6. Théorèmes d’approximation

Dans ce numéro, A est une algèbre de Banach unifère commutative complexe.

#### Proposition 4 {#ts-i-s4-prop-4 .statement tag=02AH}

Soit L une partie compacte polynomialement convexe de $\mathbf{C}^n$ et soit U un voisinage ouvert de L. Pour toute fonction $f\in \mathscr{O}(U; A)$, il existe une suite de fonctions polynomiales sur $\mathbf{C}^n$ à coefficients dans A qui converge vers $f|L$ dans $\mathscr{C}(L; A)$.

On peut supposer que L n’est pas vide et que A n’est pas nulle. Soit P (resp. $P_0)$ l’ensemble des restrictions à L des fonctions polynomiales sur $\mathbf{C}^n$ à coefficients dans A (resp. à coefficients dans $\mathbf{C})$. Soit B (resp. $B_0)$ l’algèbre de Banach adhérence de P (resp. de $P_0)$ dans $\mathscr{C}(L; A)$. Désignons par $\iota$ l’injection de A sur la sous-algèbre normée de B formée des fonctions constantes.

Soient $z_1, . . . , z_n$ les restrictions à L des fonctions coordonnées sur $\mathbf{C}^n$; ce sont des éléments de $B_0$, et, en posant $\boldsymbol{z}= (z_1, . . . , z_n)$, il vient Sp$^n_{B_0}(\boldsymbol{z}) = L$ d’après la prop. 15 de I, p. 47.

Soit $f\in \mathscr{O}(U; A)$. Par composition avec $\iota$, la fonction $f$ définit un élément $f_B=\iota \circ f$ de $\mathscr{O}(U; B)$. Comme Sp$^n_B(\boldsymbol{z})\subset$ Sp$^n_{B_0}(\boldsymbol{z})\subset U$, on peut former l’élément $b= \Theta_{\boldsymbol{z}}(f_B)$ de B. Soit $\boldsymbol{w}= (w_1, . . . , w_n)\in L$, et soit $\varphi$ le morphisme unifère continu $g\mapsto g(\boldsymbol{w})$ de B dans A. On a $\varphi \circ \iota =$ Id$_A$, de sorte que $\varphi \circ f_B=f$. Comme $\varphi (z_i) =w_i$, la prop. 3 de I, p. 66 implique $\varphi (\Theta_{\boldsymbol{z}}(f_B)) = \Theta_{\boldsymbol{w}}(\varphi \circ f_B)$. On a donc

$$
b(\boldsymbol{w}) =\varphi (b) =\varphi (\Theta_{\boldsymbol{z}}(f_B)) = \Theta_{\boldsymbol{w}}(\varphi \circ f_B) = \Theta_{\boldsymbol{w}}(f) =f(\boldsymbol{w})
$$

d’après le corollaire de la prop. 2 de I, p. 65. Ainsi, on a $f|L =b$; en particulier, $f|L$ appartient à B. Cela démontre la proposition.

#### Théorème 2 (Oka–Weil) {#ts-i-s4-thm-2 .statement tag=02AI}

Soient K une partie compacte polynomialement convexe de $\mathbf{C}^n$ et P l’ensemble des germes au voisinage de K de fonctions polynomiales sur $\mathbf{C}^n$ à coefficients dans A. Alors P est dense dans $\mathscr{O}(K; A)$. Plus précisément, tout élément de $\mathscr{O}(K; A)$ est limite d’une suite d’éléments de P.

Considérons un élément de $\mathscr{O}(K; A)$, germe d’une fonction $f\in$ $\mathscr{O}(U; A)$, où U est un voisinage ouvert de K. D’après le lemme 7 de I, p. 48, il existe un voisinage compact L de K contenu dans U qui est polynomialement convexe. Soit V l’intérieur de L ; c’est un voisinage de K.

D’après la proposition précédente, il existe une suite $(P_k)$ de fonctions polynomiales sur $\mathbf{C}^n$ à coefficients dans A qui converge vers $f|L$ dans $\mathscr{C}(L; A)$. En particulier, la suite $(P_k)$ converge vers $f|V$ dans $\mathscr{O}(V; A)$.

Par définition de la topologie sur $\mathscr{O}(K; A)$ (cf. EVT, II, p. 29, prop. 5), l’application canonique de $\mathscr{O}(V; A)$ dans $\mathscr{O}(K; A)$ est continue. Par conséquent, la suite des germes au voisinage de K des fonctions $P_k$ converge vers le germe de $f$ au voisinage de K dans l’espace $\mathscr{O}(K; A)$, ce qu’il fallait démontrer.

#### Corollaire 1 {#ts-i-s4-thm-2-cor-1 .statement tag=02AJ}

Soit U un voisinage ouvert de K. Soient $u_1$ et $u_2$ des applications continues de $\mathscr{O}(U; A)$ dans un espace topologique X se factorisant par $\mathscr{O}(K; A)$. Alors $u_1=u_2$ si et seulement si $u_1$ et $u_2$ coïn-cident sur l’ensemble des restrictions à K des fonctions polynomiales sur $\mathbf{C}^n$ à coefficients dans A.

#### Corollaire 2 {#ts-i-s4-thm-2-cor-2 .statement tag=02AK}

Soit E un espace de Banach. Soit K une partie compacte polynomialement convexe de $\mathbf{C}^n$. Soit P l’ensemble des germes au voisinage de K de fonctions polynomiales sur $\mathbf{C}^n$ à valeurs dans E. Alors tout élément de $\mathscr{O}(K; E)$ est limite d’une suite d’éléments de P.

Munissons E de la multiplication définie par $ab= 0$ pour tous $a$ et $b$ dans E (exemple 1 de I, p. 17). C’est une algèbre de Banach commutative. Soit A l’algèbre de Banach commutative unifère obtenue à partir de E par adjonction d’un élément unité. Puisque l’application canonique $\mathscr{O}(K; A)\rightarrow \mathscr{O}(K; E)$ est continue, l’assertion résulte du théorème de Oka-Weil appliqué à l’algèbre A.

Pour $n= 1$ et $A =\mathbf{C}$, on a aussi le résultat suivant, qui sera précisé par le corollaire 2 de I, p. 150.

#### Théorème 3 (Runge) {#ts-i-s4-thm-3 .statement tag=02AL}

Soient K une partie compacte de $\mathbf{C}$, et Q l’ensemble des germes de fonctions rationnelles holomorphes au voisinage de K. Alors Q est dense dans $\mathscr{O}(K)$.

D’après la définition de la topologie sur $\mathscr{O}(K)$, il suffit de démontrer que pour tout voisinage ouvert U de K, et tout sous-ensemble compact L de U, toute fonction $f\in \mathscr{O}(U)$ est limite de fonctions rationnelles continues sur L. On peut supposer que L est un voisinage compact de K.

Soit $Q'$ l’ensemble des restrictions à L des fonctions rationnelles sur $\mathbf{C}$ qui sont continues sur L, et soit C l’adhérence de $Q'$ dans $\mathscr{C}(L)$. C’est une algèbre sans radical.

Soit $z\in C$ l’application identique de L. Alors C est la sous-algèbre fermée pleine de $\mathscr{C}(L)$ engendrée par $z$ (lemme 2 de I, p. 6). On a donc Sp$_C(z) =$ Sp$_{\mathscr{C}(L)}(z) = L$. On peut alors former l’élément $c= \Theta_z(f)$ de C. Puisque C est sans radical, l’application du cor. 1 de I, p. 66 aux caractères $g\mapsto g(w)$ de C, pour tout $w\in L$, montre que $c$ coïncide avec la restriction de $f$ à L. Par définition de C, cela démontre que $f|L$ est limite uniforme sur L d’éléments de $Q'$, et cela termine la preuve du théorème.

### 7. Existence et unicité du calcul fonctionnel holomorphe

On suppose que A est une algèbre de Banach unifère complexe commutative.

#### Définition 2 {#ts-i-s4-def-2 .statement tag=02AM}

Soient $n\geqslant 1$ un entier et $\boldsymbol{a}\in A^n$. Soit U un voisinage ouvert de Sp$^n(\boldsymbol{a})$. On dit qu’une famille $\boldsymbol{a}'$ est un enveloppement de $(\boldsymbol{a},U)$ si $\boldsymbol{a}'\in \mathbf{C}^{n+p}$ prolonge $\boldsymbol{a}$ et si $U\times \mathbf{C}^p$ contient l’enveloppe polynomialement convexe de Sp$^{n+p}(\boldsymbol{a}')$.

#### Lemme 11 {#ts-i-s4-lem-11 .statement tag=02AN}

Soit $n\geqslant 1$ un entier. Soit $\boldsymbol{a}\in A^n$. Pour tout voisinage ouvert U de Sp$^n(\boldsymbol{a})$, il existe un enveloppement de $(\boldsymbol{a},U)$.

Soit $(a_{\lambda})_{\lambda\in\Lambda}$ une famille d’éléments de A prolongeant la famille $\boldsymbol{a}$ et engendrant topologiquement l’algèbre de Banach unifère A. Soit $\pi$ la projection canonique de $\mathbf{C}^{\Lambda}$ sur $\mathbf{C}^n$ et soit $U'=\pi^{-1}(U)$. Alors $U'$ est un voisinage de Sp$^{\Lambda}((a_{\lambda}))$, et Sp$^{\Lambda}((a_{\lambda}))$ est polynomialement convexe (I, p. 44, lemme 4). D’après le lemme 6 de I, p. 47, il existe une partie finie $\Lambda_0$ de Λ contenant $\{1,2, . . . , n\}$ telle que pr$_{\Lambda_0}(U')$ contienne l’enveloppe polynomialement convexe S de pr$_{\Lambda_0}$(Sp$^{\Lambda}((a_{\lambda})_{\lambda\in\Lambda})) =$ Sp$^{\Lambda_0}((a_{\lambda})_{\lambda\in\Lambda_0})$. Soit $p\geqslant 0$ l’entier tel que $\Lambda_0$ est de cardinal $n+p$, et soit $j$ une bijection de $\{1, . . . , n+p\}$ dans $\Lambda_0$ qui coïncide avec l’application identique sur $\{1, . . . , n\}$. La projection de S étant contenue dans U, la famille $(a_{j(k)})_{1\leqslant k\leqslant n+p}$ est un enveloppement de $(\boldsymbol{a},U)$.

#### Proposition 5 {#ts-i-s4-prop-5 .statement tag=02AO}

La donnée des applications $\Theta_{\boldsymbol{a}}$, pour $n\geqslant 1$ et $\boldsymbol{a}\in A^n$, est un calcul fonctionnel holomorphe sur A, c’est-à-dire que les conditions (CF1), (CF2) et (CF3) de I, p. 51 sont vérifiées.

Soient $n\geqslant 1$ un entier et $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$. L’application $\Theta_{\boldsymbol{a}}$ vérifie $\Theta_{\boldsymbol{a}}(z_i) =a_i$ pour tout $i$ tel que $1\leqslant i\leqslant n$ d’après le lemme 10 de I, p. 64, ce qui démontre la propriété (CF2). Le lemme 9 de I, p. 63 implique la propriété (CF3) des applications $\Theta_{\boldsymbol{a}}$.

L’application $\Theta_{\boldsymbol{a}}$ est A-linéaire et continue (I, p. 61, n$^o5$). Elle vérifie $\Theta_{\boldsymbol{a}}(1) = 1$ (lemme 9 de I, p. 63). Pour vérifier la condition (CF1), il reste à établir que $\Theta_{\boldsymbol{a}}$ est un morphisme d’algèbres. Pour cela, on va démontrer que $\Theta^U_{\boldsymbol{a}}$ est un morphisme d’algèbres pour tout voisinage ouvert U de Sp$^n(\boldsymbol{a})$.

Supposons d’abord que U contient l’enveloppe polynomialement convexe K de Sp$^n(\boldsymbol{a})$. Soient $f_1$ et $f_2$ des éléments de $\mathscr{O}(U; A)$. Il existe une suite $(f_{1,k})$ (resp. $(f_{2,k})$) de fonctions polynomiales qui converge vers $f_1$ (resp. vers $f_2)$ dans $\mathscr{O}(K; A)$ (théorème 2 de I, p. 68), donc dans $\mathscr{O}$(Sp$^n(\boldsymbol{a}); A)$. Pour tout entier $k$, on a

$$
\Theta^U_{\boldsymbol{a}}(f_{1,k})\Theta^U_{\boldsymbol{a}}(f_{2,k}) = \Theta^U_{\boldsymbol{a}}(f_{1,k}f_{2,k})
$$

d’après le lemme 10 de I, p. 64, d’où $\Theta^U_{\boldsymbol{a}}(f_1)\Theta^U_{\boldsymbol{a}}(f_2) = \Theta^U_{\boldsymbol{a}}(f_1f_2)$ en passant à la limite.

Considérons le cas général. Soient $\boldsymbol{a}'\in \mathbf{C}^{n+p}$ un enveloppement de $(\boldsymbol{a},U)$ (lemme 11) et $\pi : U\times \mathbf{C}^p\rightarrow U$ la projection canonique. Puisque $U\times \mathbf{C}^p$ contient l’enveloppe polynomialement convexe de Sp$^{n+p}(\boldsymbol{a}')$, on a

$$
\Theta^{U\times\mathbf{C}^p}_{\boldsymbol{a}'}(f_1\circ \pi )\Theta^{U\times\mathbf{C}^p}_{\boldsymbol{a}'}(f_2\circ \pi ) = \Theta^{U\times\mathbf{C}^p}_{\boldsymbol{a}'}(f_1f_2\circ \pi )
$$

pour $f_1$ et $f_2$ dans $\mathscr{O}(U; A)$ d’après le premier cas. Comme, pour toute fonction $f\in \mathscr{O}(U; A)$, on a $\Theta^{U\times\mathbf{C}^p}_{\boldsymbol{a}'}(f\circ \pi ) = \Theta^U_{\boldsymbol{a}}(f)$ (condition (CF3) précédemment démontrée), la conclusion en découle, et donc la condition (CF1).

Nous pouvons maintenant démontrer le théorème 1 de I, p. 51. La prop. 5 montre que la famille des applications $(\Theta_{\boldsymbol{a}})_{\boldsymbol{a}}$ est un calcul fonctionnel holomorphe sur A. Il ne reste donc qu’à établir l’unicité du calcul fonctionnel holomorphe sur A.

Soit $(\Psi_{\boldsymbol{a}})_{\boldsymbol{a}}$ une famille d’applications définies pour tout entier $n\geqslant 1$ et tout $\boldsymbol{a}\in A^n$ et vérifiant les conditions (CF1), (CF2), (CF3) du calcul fonctionnel holomorphe sur A (I, p. 51). Il suffit de prouver que pour tout entier $n\geqslant 1$, pour tout $\boldsymbol{a}\in A^n$ et pour tout voisinage ouvert U de $\boldsymbol{a}$, on a $\Theta^U_{\boldsymbol{a}}= \Psi^U_{\boldsymbol{a}}$.

Soient $n\geqslant 1$ et $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$. Soit U un voisinage ouvert de Sp$^n(\boldsymbol{a})$. Supposons d’abord que U contient l’enveloppe polynomialement convexe K de Sp$^n(\boldsymbol{a})$. Les morphismes $\Theta^U_{\boldsymbol{a}}$ et $\Psi^U_{\boldsymbol{a}}$ coïncident sur les fonctions polynomiales d’après les propriétés (CF1) et (CF2). D’après le corollaire du théorème 2 de I, p. 68 et la propriété de continuité (CF1), ces morphismes sont donc égaux.

Démontrons le cas général. Soient $\boldsymbol{a}'\in \mathbf{C}^{n+p}$ un enveloppement de $(\boldsymbol{a},U)$ et $\pi : U\times \mathbf{C}^p\rightarrow U$ la projection canonique. On a

$$
\Theta^U_{\boldsymbol{a}}= \Theta^{U\times\mathbf{C}^p}_{\boldsymbol{a}'}\circ \pi^*= \Psi^{U\times\mathbf{C}^p}_{\boldsymbol{a}'}\circ \pi^*= \Psi^U_{\boldsymbol{a}}
$$

d’après la propriété (CF3) et le cas précédent. Cela conclut la démonstration du théorème 1 de I, p. 51.

Remarquons que le th. 2 de I, p. 68 entraîne aussi le résultat d’unicité suivant :

#### Proposition 6 {#ts-i-s4-prop-6 .statement tag=02AP}

Soit $\boldsymbol{a}\in A^n$. On suppose Sp$^n(\boldsymbol{a})$ polynomialement convexe. Soient $z_1, . . . , z_n$ les germes au voisinage de Sp$^n(\boldsymbol{a})$ des fonctions coordonnées sur $\mathbf{C}^n$. Alors l’application $\Theta_{\boldsymbol{a}}$ est l’unique morphisme continu d’algèbres unifères $\varphi$ de $\mathscr{O}$(Sp$^n(\boldsymbol{a}); A)$ dans A tel que $\varphi (z_1) =a_1, . . . , \varphi (z_n) =a_n$.

Le lemme 10 de I, p. 64 et le corollaire de la proposition 2 de I, p. 65 justifient les notations suivantes pour le calcul fonctionnel holomorphe. Soient $n\geqslant 1$ et $\boldsymbol{a}\in A^n$. Pour tout germe $f\in \mathscr{O}(K; A)$ (resp. pour toute fonction holomorphe $f\in \mathscr{O}(U; A)$ sur un voisinage ouvert U de Sp$^n(\boldsymbol{a})$), on pose

$$
f(\boldsymbol{a}) = \Theta_{\boldsymbol{a}}(f) \tag{6}
$$

Cette notation est cohérente avec la notation introduite dans A, IV, p. 4, n$^o3$, si $f$ est un polynôme, d’après les propriétés (CF1) et (CF2).

Les propriétés (CF2) et (CF3) de I, p. 51 peuvent alors s’écrire

$$
z_i(\boldsymbol{a}) =a_i,1\leqslant i\leqslant n,(f\circ \pi_{m,n})(\boldsymbol{a}) =f(\pi_{m,n}(\boldsymbol{a}))
$$

### 8. Substitution dans le calcul fonctionnel

Avec les notations introduites ci-dessus, les énoncés du cor. 1 de I, p. 66 et du cor. 2 de I, p. 67 deviennent respectivement

$\chi (g(\boldsymbol{a})) =g(\chi (a_1), . . . , \chi (a_n))$, Sp($g(\boldsymbol{a})$) $=g$(Sp$^n(\boldsymbol{a}))$

pour $f\in \mathscr{O}$(Sp$^n(\boldsymbol{a}); A),\chi \in \mathsf{X}(A)$ et $g\in \mathscr{O}$(Sp$^n(\boldsymbol{a}))$.

Nous allons maintenant démontrer une propriété de substitution plus générale.

#### Théorème 4 {#ts-i-s4-thm-4 .statement tag=02AQ}

Soit A une algèbre de Banach unifère commutative complexe, soient $n\geqslant 1$ un entier et $\boldsymbol{a}= (a_1, . . . , a_n)\in A^n$. Soit $\boldsymbol{f}=$ $(f_1, . . . , f_p)$ où $f_1, . . . , f_p$ sont des éléments de $\mathscr{O}$(Sp$^n(\boldsymbol{a}))$. L’image de Sp$^n(\boldsymbol{a})$ par l’application $\boldsymbol{z}\mapsto \boldsymbol{f}(\boldsymbol{z}) = (f_1(\boldsymbol{z}), . . . , f_p(\boldsymbol{z}))$ est égale à Sp$^p(\boldsymbol{f}(\boldsymbol{a}))$.

Pour tout $g\in \mathscr{O}$(Sp$^p(\boldsymbol{f}(\boldsymbol{a})); A)$, le germe composé $g\circ \boldsymbol{f}$ est un élément de $\mathscr{O}$(Sp$^n(\boldsymbol{a}); A)$ et on a $g(\boldsymbol{f}(\boldsymbol{a})) = (g\circ \boldsymbol{f})(\boldsymbol{a})$.

La première assertion concernant l’image de Sp$^n(\boldsymbol{a})$ résulte du cor. 2 de I, p. 67. Pour démontrer la seconde, nous utiliserons le lemme suivant.

#### Lemme 12 {#ts-i-s4-lem-12 .statement tag=02AR}

Soit K l’enveloppe polynomialement convexe de Sp$^p(\boldsymbol{f}(\boldsymbol{a}))$. On a $g(\boldsymbol{f}(\boldsymbol{a})) = (g\circ \boldsymbol{f})(\boldsymbol{a})$ pour tout germe $g\in \mathscr{O}(K; A)$.

Soit Ψ l’application de $\mathscr{O}(K; A)$ dans A telle que $\Psi (g) = (g\circ \boldsymbol{f})(\boldsymbol{a})$. C’est un morphisme unifère continu, tel que $\Psi (z_j) =f_j(\boldsymbol{a})$, où $z_j$ est le germe de la $j$-ème fonction coordonnée sur $\mathbf{C}^p$. Lorsque $g$ est le germe d’une fonction polynomiale, on a donc $\Psi (g) =g(\boldsymbol{f}(\boldsymbol{a}))$. D’après le th. 2 de I, p. 68, cette formule reste valide pour tout $g\in \mathscr{O}(K; A)$.

Démontrons maintenant le théorème. Soient V un voisinage ouvert de Sp$^p(\boldsymbol{f}(\boldsymbol{a}))$ et $\widetilde{g}\in \mathscr{O}(V; A)$ une fonction holomorphe dont le germe au voisinage de Sp$^p(\boldsymbol{f}(\boldsymbol{a}))$ est égal à $g$. Soient $\boldsymbol{b}\in \mathbf{C}^{p+q}$ un enveloppement de $(\boldsymbol{f}(\boldsymbol{a}),V)$ (lemme 11 de I, p. 70) et $\pi : V\times \mathbf{C}^q\rightarrow V$ la projection canonique.

Soient $\widetilde{f}_1, . . . ,\widetilde{f}_p$ des fonctions holomorphes dont les germes sont $f_1, . . . , f_p$ et soit U un voisinage ouvert de Sp$^n(\boldsymbol{a})$ tel que $(\widetilde{f}_1, . . . ,\widetilde{f}_p)(U)\subset V$. Soit $\pi '$ la projection canonique de $U\times \mathbf{C}^q$ sur U. Notons $z_{n+1}, . . . , z_{n+q}$ les $q$ dernières fonctions coordonnées sur $\mathbf{C}^{n+q}$. Notons $h=\widetilde{g}\circ (\widetilde{f}_1, . . . ,\widetilde{f}_p)$ et

$$
\boldsymbol{c}= (a_1, . . . , a_n, b_{p+1}, . . . , b_{p+q})\in A^{n+q}
$$

L’application $\widetilde{g}\circ \pi$ est holomorphe dans le voisinage ouvert $V\times \mathbf{C}^q$ de l’enveloppe polynomialement convexe L de Sp$^{p+q}(\boldsymbol{b})$. D’après le lemme 12, appliqué à $\boldsymbol{c}$, aux germes au voisinage de L des fonctions

$$
(\widetilde{f}_1\circ \pi ', . . . ,\widetilde{f}_p\circ \pi ', z_{n+1}, . . . , z_{n+q})
$$

et au germe de $\widetilde{g}\circ \pi$, on a

$$
(g\circ \pi )(f_1\circ \pi ')(\boldsymbol{c}), . . . ,(f_p\circ \pi ')(\boldsymbol{c}), z_{n+1}(\boldsymbol{c}), . . . , z_{n+q}(\boldsymbol{c})= (h\circ \pi ')(\boldsymbol{c})
$$

Comme $\pi '(\boldsymbol{c}) =\boldsymbol{a}$, on a $(h\circ \pi ')(\boldsymbol{c}) =h(\boldsymbol{a})$ et $(f_i\circ \pi ')(\boldsymbol{c}) =f_i(\boldsymbol{a})$ pour $1\leqslant i\leqslant p$ (propriété (CF3) du calcul fonctionnel holomorphe). Comme, de plus, $z_{n+j}(\boldsymbol{c}) =b_{p+j}$ pour $1\leqslant j\leqslant q$ (propriété (CF2)), on a

$$
(g\circ \pi )(f_1(\boldsymbol{a}), . . . , f_p(\boldsymbol{a}), b_{p+1}, . . . , b_{p+q}) =h(\boldsymbol{a})
$$

dont on déduit $g(f_1(\boldsymbol{a}), . . . , f_p(\boldsymbol{a})) =h(\boldsymbol{a})$ en appliquant de nouveau la propriété (CF3).

### 9. Calcul fonctionnel holomorphe en une variable

#### Théorème 5 {#ts-i-s4-thm-5 .statement tag=02AS}

Soit A une algèbre de Banach unifère, non nécessairement commutative. Soient $a$ un élément de A et $z$ le germe de la fonction identique de $\mathbf{C}$ au voisinage de Sp$_A(a)$. Il existe un unique morphisme unifère continu $\varphi_a$ de $\mathscr{O}$(Sp$_A(a))$ dans A tel que $\varphi_a(z) =a$.

L’image de $\varphi_a$ est contenue dans la sous-algèbre fermée pleine de A engendrée par $a$. En particulier, elle est contenue dans le bicommutant de $a$.

Démontrons l’existence du morphisme $\varphi_a$. Soit B la sous-algèbre fermée pleine de A engendrée par $a$. Elle est commutative, et on a Sp$_B(a) =$ Sp$_A(a)$ (I, p. 5, n$^o5$). L’application $\Theta_a$ du calcul fonctionnel holomorphe sur B est un morphisme unifère continu de $\mathscr{O}$(Sp$_B(a))$ dans B tel que $\Theta_a(z) =a$ (théorème 1 de I, p. 51). Le morphisme composé de $\Theta_a$ et de l’injection canonique de B dans A est un morphisme unifère continu $\varphi_a$ de $\mathscr{O}$(Sp$_A(a))$ dans A tel que l’image de $z$ est $a$.

Démontrons l’unicité. Soit $\varphi '_a$ un morphisme unifère continu de $\mathscr{O}$(Sp$_A(a))$ dans A tel que $\varphi '_a(z) =a$. Alors $\varphi_a$ et $\varphi '_a$ coïncident sur l’ensemble des germes de polynômes au voisinage de Sp$_A(a)$, donc sur l’ensemble des germes de fractions rationnelles holomorphes au voisinage de Sp$_A(a)$. Or ces germes sont denses dans $\mathscr{O}$(Sp$_A(a))$ (I, p. 69, th. 3). Cela implique que $\varphi_a=\varphi '_a$.

La construction de $\varphi_a$ démontre que son image est contenue dans la sous-algèbre commutative B, qui est contenue dans le bicommutant de $a($I, p. 6).

Si le radical de l’algèbre A est nul, l’unicité du morphisme $\varphi_a$ est valide sans requérir qu’il soit continu (cf. prop. 9 de I, p. 40). Ce n’est pas le cas en général, cf. G. R. Allan, Embedding the algebra of formal power series in a Banach algebra, Proc. London Math. Soc. (3) 25 (1972), 329–340.

Pour toute algèbre de Banach A, tout élément $a$ de A et tout germe $f\in \mathscr{O}$(Sp$_A(a))$, on note $f(a)$ l’élément $\varphi_a(f)$ du théorème 5. Si A est une algèbre de Banach commutative, cet élément $f(a)$ coïncide avec l’élément $f(a)$ fourni par le calcul fonctionnel holomorphe sur une algèbre de Banach commutative (théorème 1 de I, p. 51).

Soit B la sous-algèbre fermée pleine de A engendrée par $a$, de sorte que Sp$_A(a) =$ Sp$_B(a)$. L’élément $f(a)$ de A appartient à B, et coïncide avec l’élément $f(a)$ calculé relativement à l’algèbre B.

#### Proposition 7 {#ts-i-s4-prop-7 .statement tag=02AT}

Soient A et B des algèbres de Banach unifères et $\varphi$ un morphisme unifère continu de A dans B. Soit $a\in$ A. Alors Sp$_B(\varphi (a))\subset$ Sp$_A(a)$ et on a $\varphi (f(a))$ = $f(\varphi (a))$ pour tout $f\in \mathscr{O}$(Sp$_A(a))$. En particulier, pour tout $\chi \in \mathsf{X}(A)$, on a $\chi (f(a)) =f(\chi (a))$.

Ceci résulte de la prop. 3 de I, p. 66.

#### Proposition 8 {#ts-i-s4-prop-8 .statement tag=02AU}

Soient A une algèbre de Banach unifère et $a\in A$. Soit $f\in \mathscr{O}$(Sp($a$)). On a $f$(Sp$_A(a)) =$ Sp$_A(f(a))$. De plus, pour tout $g\in \mathscr{O}$(Sp$_A(f(a)))$, on a $g\circ f\in \mathscr{O}$(Sp$_A(a))$ et $g(f(a)) = (g\circ f)(a)$.

Ceci résulte du th. 4.

#### Proposition 9 {#ts-i-s4-prop-9 .statement tag=02AV}

Soient A une algèbre de Banach unifère et $a\in A$. Soient U un voisinage ouvert de Sp$_A(a)$ et $f\in \mathscr{O}(U)$. Soit de plus V un voisinage compact de Sp$_A(a)$ contenu dans U tel que V est une pièce de U de bord orienté $\partial V$.

Pour tout entier $n\geqslant 0$, l’application $z\mapsto f(z)(z-a)^{-n-1}$ est continue sur $\partial V$, la forme différentielle $z\mapsto f(z)(z-a)^{-n-1}dz$ est intégrable sur $\partial V$ et on a

$_{(n)}n$! $\int_{-n-1}$

$$
f(a) =f(z)(z-a)dz \tag{7}
$$

$$
2i\pi_{\partial V}
$$

où $f^{(n)}\in \mathscr{O}(U)$ est la $n$-ème dérivée de $f$.

Procédons par récurrence sur $n$. Lorsque $n= 0$, le résultat résulte de la prop. 1 de I, p. 61. Supposons maintenant que l’assertion de la proposition est vraie pour l’entier $n\geqslant 0$. Soit $g\in \mathscr{O}(\mathbf{C}-$ Sp$_A(a); A)$ la fonction holomorphe définie par $g(z) = (z-a)^{-n-1}f(z)$. La forme différentielle $g'(z)dz$ = $dg$ est de classe $C^1$; comme la pièce V est compacte, la formule de Stokes (VAR, R2, p. 47, 11.2.3) implique

$$
\int_{\partial V}g'(z)dz=\int_{\partial V}dg= 0
$$

Comme $g'(z) = (z-a)^{-n-1}f'(z)-(n+1)(z-a)^{-n-2}f(z)$, en on déduit

$$
\int_{\partial V}f'(z)(z-a)^{-n-1}dz= (n+ 1)\int_{\partial V}f(z)(z-a)^{-n-2}dz
$$

En appliquant l’hypothèse de récurrence à $f'$, on obtient donc

$$
2i\pi_{(n+1)}\int_{-n-2}
$$

$$
f(a) = (n+ 1)f(z)(z-a)dz
$$

$n$! $\partial_V$

ce qui est l’assertion de la proposition pour l’entier $n+ 1$. Cela conclut la preuve.

#### Proposition 10 {#ts-i-s4-prop-10 .statement tag=02AW}

Soient A une algèbre de Banach unifère et U une partie ouverte de $\mathbf{C}$.

a) L’ensemble Ω des $a\in A$ tels que Sp$_A(a)\subset U$ est ouvert dans A ;

b) Soit $f\in \mathscr{O}(U)$. L’application $a\mapsto f(a)$ de Ω dans A est holomorphe, et en particulier continue.

Soit $a\in \Omega$. Il existe un voisinage compact V de Sp$_A(a)$ contenu dans U qui est une pièce de U (VAR, R2, p. 46 et p. 47, 11.1.3, d)).

Puisque la résolvante de $a$ tend vers 0 à l’infini (th. 1, c) de I, p. 24), l’application $z\mapsto  \|(z-a)^{-1}\|$ est bornée sur $\mathbf{C}-\mathring{V}$. Notons M sa borne supérieure. Si $h\in A$ est tel que $\|h\|\leqslant (2M)^{-1}$ et si $z\in \mathbf{C}-\mathring{V}$, on a

$$
z-(a+h) = (1-h(z-a)^{-1})(z-a)
$$

et $\|h(z-a)^{-1}\|\leqslant \frac{1}{2}$, donc $z-(a+h)$ est inversible et son inverse vérifie

$$
(z-(a+h))^{-1}= (z-a)^{-1}\sum_{n=0}^{\infty}(h(z-a)^{-1})^n \tag{8}
$$

avec $\|(h(z-a)^{-1})^n\|\leqslant 2^{-n}$ (prop. 2 de I, p. 22). Ainsi, Sp$_A(a+h)$ est contenu dans V, donc dans U, ce qui prouve que Ω est ouvert dans A.

Soit $f\in \mathscr{O}(U)$. Notons $m$ la borne supérieure de $|f(z)|$ pour $z\in \partial V$. Soit $a\in A$. Pour tout $h\in A$ tel que $\|h\|\leqslant (2M)^{-1}$, on a

1 $\int_{-1}$

$$
f(a+h) =f(z)(z-(a+h))dz
$$

$$
2i\pi_{\partial V}
$$

(prop. 9). La série (8) converge uniformément sur le bord de V, donc

$$
f(a+h) =\sum_{n=0}^{+\infty}f_{a,n}(h)
$$

où l’application $f_{a,n}$ de A dans A est définie par

1 $\int-1-1n$

$f_{a,n}(h) =f(z)(z-a)(h(z-a)$ ) $dz$.

$$
2i\pi_{\partial V}
$$

Pour tout $n\in \mathbf{N}$, la fonction $f_{a,n}$ est une fonction polynomiale homogène continue de degré $n$. De plus, il vient

$$
mM\int_{-(n+1)}
$$

$\|f_{a,n}(h)\|\leqslant \|dz\|$ 2

$$
\pi_{\partial V}
$$

(INT, VI, §2, n$^o3$, prop. 5). La série $\sum_nf_{a,n}(h)$ est donc absolument convergente pour $\|h\|\leqslant (2M)^{-1}$. Cela démontre que l’application qui à $a$ associe $f(a)$ est holomorphe sur Ω (VAR, R1, p. 26, 3.2.1).

#### Proposition 11 {#ts-i-s4-prop-11 .statement tag=02AX}

Soient A une algèbre de Banach unifère, $a\in A$ et U un voisinage ouvert de Sp$_A(a)$. Notons $\delta$ la distance de Sp$_A(a)$ à $\mathbf{C}-$ U. Soit $f\in \mathscr{O}(U)$.

a) Pour tout nombre réel $\eta$ tel que $0< \eta  < \delta$, il existe un nombre réel $C\geqslant 0$ tel que $\|f^{(n)}(a)\|\leqslant Cn$!$\eta^{-n}$ pour tout entier $n\in \mathbf{N}$;

b) Si $b\in A$ est permutable à $a$ et si $\varrho (b)< \delta$, on a Sp$_A(a+b)\subset U$, et

$\infty (n)$

$$
f(a)_n
$$

$f(a+b) =\sum b$,

$n$!

$n=0$

où la série converge absolument.

Soit $\eta$ un nombre réel tel que $0< \eta  < \delta$. Notons $\varepsilon =\delta -\eta  >0$. Soit K le voisinage compact de Sp$_A(a)$ formé des points de $\mathbf{C}$ dont la distance à Sp$_A(a)$ est $\leqslant \varepsilon /2$. Comme $f$ est holomorphe dans tout disque ouvert de rayon $\eta +\varepsilon /2$ dont le centre appartient à K, il existe, d’après les inégalités de Cauchy (VAR, R1, p. 29, 3.3.4), un nombre réel $C\geqslant 0$ tel que

$|f^{(n)}(z)|$ C

sup $\leqslant_n$

$_{z\in K}n$! $\eta$

pour tout entier $n\geqslant 0$. Alors l’assertion a) résulte de la prop. 1 de I, p. 61 appliquée à $f^{(n)}$ et à une pièce V contenue dans K.

Soit $b$ un élément de A permutable à $a$ tel que $\varrho (b)< \delta$. En remplaçant A par la sous-algèbre fermée pleine B engendrée par $a$ et $b$, qui vérifie Sp$_A(a) =$ Sp$_B(a)$ et Sp$_A(a+b) =$ Sp$_B(a+b)$, on se ramène pour démontrer b) au cas où A est commutative.

Puisque $\varrho (b)< \delta$, on peut choisir $\eta$ tel que $\varrho (b)< \eta  < \delta$. Soient $V_1$ l’ensemble des points de $\mathbf{C}$ dont la distance à Sp$_A(a)$ est $< \delta -\eta$, et $V_2$ le disque ouvert de centre 0 et de rayon $\eta$ dans $\mathbf{C}$. Soit $g$ l’application $(z_1, z_2)\mapsto z_1+z_2$ de $V_1\times V_2$ dans U. Alors $h=f\circ g$ est l’application $(z_1, z_2)\mapsto f(z_1+z_2)$ de $V_1\times V_2$ dans $\mathbf{C}$. On a Sp$^2_A(a, b)\subset V_1\times V_2$, donc Sp$_A(a+b)\subset U$ (cf. cor. 2 de I, p. 67), et de plus $f(a+b) =h(a, b)$ d’après le th. 4 de I, p. 72. Or, dans l’espace $\mathscr{O}(V_1\times V_2)$, on a

$$
f^{(n)}(z_1)_n
$$

$$
h(z_1, z_2) =\sum z_2
$$

$_{n\geqslant 0}n$!

(VAR, R1, p. 29, 3.3.4) donc la série

$$
f^{(n)}(a)_n
$$

$$
\sum b
$$

$n$!

$n\geqslant 0$ converge dans A et sa somme est $h(a, b) =f(a+b)$. En outre, cette série est absolument convergente d’après l’assertion a).

### 10. Exponentielle et logarithme

On note exp la fonction exponentielle complexe de $\mathbf{C}$ dans $\mathbf{C}$ (FVR, III, p. 8, déf. 2). Elle est dérivable et vérifie exp$'=$ exp (FVR, III, p. 9, (26)) donc est holomorphe dans $\mathbf{C}$. Soient A une algèbre de Banach unifère et $a$ un élément de A. D’après la prop. 2 de I, p. 65 et la formule (9) de FVR, III, p. 16, on a

$\infty n$

$$
a
$$

(9) exp($a$) $=\sum$.

$n$!

$n=0$

Comme $\|a^n\|\leqslant \|a\|^n$, on voit que $\|$exp($a$)$\|\leqslant$ exp($\|a\|$) et que la série (9) converge uniformément dans toute boule de A. L’application $a\mapsto$ exp($a$) de A dans A est holomorphe (prop. 10 de I, p. 76). On note également parfois $e^a$ l’exponentielle de $a\in A$.

Lorsque $a$ est un endomorphisme d’un espace de Banach E, l’exponentielle exp($a$) ainsi définie dans l’algèbre de Banach $\mathscr{L}(E)$ coïncide avec celle définie dans FVR, IV, p. 27, déf. 1, d’après loc. cit. prop. 7 (3).

Pour tout élément $b$ de A qui est permutable à $a$, on a aussi

$$
^{\infty}b^n
$$

exp($a+b$) $=\sum$ exp($a$),

$n$!

$n=0$

(prop. 11 de I, p. 77), d’où

(10) exp($a+b$) $=$ exp($a$)$\cdot$ exp($b$).

En particulier, exp($a$) est inversible et

(11) exp($a$)$^{-1}=$ exp($-a$).

Soit B l’ensemble des $z\in \mathbf{C}$ tels que $-\pi  <\mathscr{I}z < \pi$. Soit F le complémentaire dans $\mathbf{C}$ de l’intervalle $\mathbf{R}_-$. La restriction de l’exponentielle à B induit par passage aux sous-espaces une bijection de B sur F (FVR, III, p. 10, n$^o7)$, dont la bijection réciproque sera notée log.

Si $a\in A$ est tel que Sp$_A(a)\subset F$, on peut former l’élément log($a$) de A. On a Sp$_A$(log($a$))$\subset B$, et

(12) exp(log($a$)) $=a$ d’après la prop. 8 de I, p. 75. Inversement, soit $b$ un élément de A tel que Sp$_A(b)\subset B$. On a Sp$_A$(exp($b$))$\subset F$ et

(13) log(exp($b$)) $=b$

(loc. cit.).

En particulier, si $a\in A$ est tel que $\varrho (a)<1$, on a Sp$_A(1-a)\subset F$ et on peut former log(1 $-a)$. Pour $n\geqslant 1$, la $n$-ème dérivée de $z\mapsto$ log(1$-z)$ est $z\mapsto  -(n-$1)!(1$-z)^{-n}$ Le développement en série entière de $z\mapsto$ log(1 $-z)$ au point 0 est donc

$$
^{\infty}z^n
$$

log(1 $-z) =-\sum$,

$$
n
$$

$n=1$

valide pour $|z|<1$ (VAR, R1, p. 30, 3.3.9). D’après la prop. 2 de I, p. 65, il vient

$$
^{\infty}a^n
$$

(14) log(1 $-a) =-\sum$.

$$
_{n=1}n
$$

#### Proposition 12 {#ts-i-s4-prop-12 .statement tag=02AY}

Soit A une algèbre de Banach unifère commutative. L’image de l’application exponentielle est la composante neutre du groupe G des éléments inversibles de A.

Les formules (10) et (11) prouvent que exp(A) est un sous-groupe de G. D’après ce qui précède (voir la formule (12)), ce sous-groupe contient la boule ouverte de centre 1 et de rayon 1. C’est donc un sous-groupe ouvert, et par suite fermé, de G. Par ailleurs, A est connexe et l’application $a\mapsto$ exp($a$) est continue, de sorte que exp(A) est connexe. Donc exp(A) est la composante neutre de G.

### 11. Partitions de l’espace des caractères

#### Proposition 13 {#ts-i-s4-prop-13 .statement tag=02AZ}

Soit A une algèbre de Banach unifère commutative. Soient $U_1$ et $U_2$ des ouverts de $\mathsf{X}(A)$ formant une partition de $\mathsf{X}(A)$. Alors il existe un unique idempotent $j$ de A tel que la transformée de Gelfand $\mathscr{G}(j)$ soit égale à 1 sur $U_1$ et à 0 sur $U_2$.

Identifions l’espace $\mathsf{X}(A)$ à une partie compacte de $\mathbf{C}^A$ par l’application $\chi \mapsto (\chi (a))_{a\in A}($cf. n$^o6$ de I, p. 6 et cor. du th. 1 de I, p. 29). Les parties $U_1$ et $U_2$ de l’espace uniforme $\mathbf{C}^A$ sont compactes et disjointes. D’après TG, II, p. 31, prop. 4, il existe une partie finie M de A et des parties ouvertes disjointes $V_1$ et $V_2$ de $\mathbf{C}^M$ telles que

$$
p(U_1)\subset V_1,p(U_2)\subset V_2
$$

où $p$ est la projection canonique de $\mathbf{C}^A$ sur $\mathbf{C}^M$.

Soient $a_1, . . . , a_n$ les éléments distincts de M, et identifions $\mathbf{C}^M$ à $\mathbf{C}^n$. On a Sp$^n_A(a_1, . . . , a_n)\subset p(\mathsf{X}(A))\subset V_1\cup V_2$ puisque $U_1\cup U_2=\mathsf{X}(A)$. Soit $f$ la fonction sur $V_1\cup V_2$ égale à 1 sur $V_1$ et à 0 sur $V_2$. On a $f\in \mathscr{O}(V_1\cup V_2)$. Posons $j=f(a_1, . . . , a_n)$. Comme $f^2=f$, on a $j^2=j$. D’après le cor. 1 de I, p. 66, on a $\chi (j) = 1$ si $\chi \in U_1$ et $\chi (j) = 0$ si $\chi \in U_2$, ce qui démontre l’existence de l’idempotent demandé.

D’autre part, si $j_1$ est un idempotent de A, les relations $j^2=j$ et $j_1^2=j_1$ impliquent $(j-j_1)(j+j_1-1) = 0$. Si $\mathscr{G}(j_1) =\mathscr{G}(j)$, la transformée de Gelfand de $j+j_1-1$ est à valeurs dans $\{-1,1\}$, donc $j+j_1-1$ est inversible (prop. 6 de I, p. 37), d’où $j=j_1$.

#### Corollaire {#ts-i-s4-n11-cor-1 .statement tag=02B0}

Soit A une algèbre de Banach unifère commutative. Les assertions suivantes sont équivalentes :

a) L’espace des caractères $\mathsf{X}(A)$ n’est pas connexe;

b) Il existe un élément idempotent de A différent de 0 et 1 ;

c) L’algèbre A est isomorphe au produit de deux algèbres de Banach non nulles.

La proposition démontre que a) implique b). Si $j$ est un idempotent de A, soient $I_1=jA$ et $I_2= (1-j)A$. Alors $I_1$ et $I_2$ sont des idéaux fermés de A, et $I_1+ I_2= A$. Si $j /\in  \{0,1\}$, les idéaux $I_1$ et $I_2$ sont distincts de A. D’autre part, l’idéal $I_1$ (resp. $I_2)$ est l’ensemble des éléments $x$ de A tels que $jx=x$ (resp. $(1-j)x=x)$, donc $I_1\cap I_2=\{0\}$. L’algèbre A s’identifie alors au produit $A/I_1\times A/I_2$. Ainsi, l’assertion b) implique c). Finalement, si A est isomorphe à $A_1\times A_2$, l’espace $\mathsf{X}(A)$ s’identifie à l’espace somme de $\mathsf{X}(A_1)$ et de $\mathsf{X}(A_2)$ (I, p. 6, n$^o6$), donc c) implique a).

#### Proposition 14 {#ts-i-s4-prop-14 .statement tag=02B1}

Soit A une algèbre de Banach commutative sans radical. Pour que A admette un élément unité, il faut et il suffit que $\mathsf{X}(A)$ soit compact.

La condition est nécessaire (I, p. 29, corollaire). Supposons $\mathsf{X}(A)$ compact. Soit $\widetilde{A}$ l’algèbre de Banach déduite de A par adjonction d’un élément unité, et identifions $\mathsf{X}'(A)$ à $\mathsf{X}(\widetilde{A})$. Le complémentaire de $\mathsf{X}(A)$ dans $\mathsf{X}(\widetilde{A})$ est réduit au caractère $\chi_0$ de $\widetilde{A}$ dont le noyau est A. Les parties $\mathsf{X}(A)$ et $\{\chi_0\}$ sont ouvertes dans $\mathsf{X}(\widetilde{A})$. D’après la prop. 13, il existe un élément $j\in A$ tel que $\chi (j) = 1$ pour $\chi \in \mathsf{X}(A)$, et $\chi_0(j) = 0$. On a donc $j\in A$.

Soit alors $x$ dans A. On a $\chi (jx) =\chi (x)$ pour tout $\chi \in \mathsf{X}(A)$, donc $jx=x$ puisque A est sans radical. Ainsi, $j$ est un élément unité de A.

#### Proposition 15 {#ts-i-s4-prop-15 .statement tag=02B2}

Soit A une algèbre de Banach commutative, soient $I_1$ un idéal de A et $F_1$ l’ensemble des $\chi \in \mathsf{X}(A)$ qui sont nuls sur $I_1$. Soit $F_2$ une partie de $\mathsf{X}(A)$ disjointe de $F_1$, fermée pour la topologie de Jacobson, et compacte pour la topologie faible. Alors il existe $u\in I_1$ tel que $\mathscr{G}(u) = 1$ sur $F_2$.

Soit $I_2$ l’intersection des noyaux des caractères appartenant à $F_2$. L’algèbre de Banach $A/I_2$ est sans radical (prop. 8 de I, p. 38). Puisque $F_2$ est fermé pour la topologie de Jacobson, les seuls éléments de $\mathsf{X}(A)$ nuls sur $I_2$ sont ceux de $F_2($cf. I, p. 13). Donc $F_2$, muni de la topologie induite par la topologie faible de $\mathsf{X}(A)$, s’identifie à $\mathsf{X}(A/I_2)$ muni de la topologie faible (I, p. 9, n$^o7$). Comme $F_2$ est faiblement compact, l’algèbre $A/I_2$ possède un élément unité (prop. 14).

On a alors $I_1+ I_2= A$. En effet, dans le cas contraire, $(I_1+ I_2)/I_2$ serait un idéal strict, donc contenu dans le noyau d’un caractère non nul de $A/I_2($I, p. 30, th. 2). Celui-ci définirait, par composition avec la projection canonique $A\rightarrow A/I_2$, un caractère non nul $\chi$ de A qui s’annulerait sur $I_1$ et $I_2$, et appartiendrait donc à $F_1\cap F_2$, contrairement à l’hypothèse.

Puisque $I_1+ I_2= A$, il existe $u\in I_1$ dont la classe dans $A/I_2$ est un élément unité de $A/I_2$. Alors $\chi (u) = 1$ pour tout $\chi \in F_2$, ce qui conclut la démonstration.

#### Corollaire {#ts-i-s4-n11-cor-2 .statement tag=02B3}

Soit A une algèbre de Banach commutative. Soient $F_1$ et $F_2$ deux parties disjointes de $\mathsf{X}(A)$, fermées pour la topologie de Jacobson. On suppose $F_2$ faiblement compacte. Alors il existe $u\in A$ tel que $\mathscr{G}(u) = 1$ sur $F_2$ et $\mathscr{G}(u) = 0$ sur $F_1$.

### 12. Partitions du spectre d’un élément

Soient A une algèbre de Banach unifère, $x\in A$, et K = Sp$_A(x)$. On note Π l’ensemble des parties de K qui sont ouvertes et fermées dans K. Soit B la sous-algèbre fermée pleine de A engendrée par $x$; elle est commutative.

Pour tout $H\in \Pi$, il existe un unique élément $f_H$ de $\mathscr{O}(K)$ égal à 1 au voisinage de H et à 0 au voisinage de K - H. On pose $j_H=f_H(x)$. L’élément $j_H$ est un idempotent de A, dit associé à $x$ et H, et on a les formules suivantes :

$$
j_{H\cap H'}=j_Hj_{H'}=j_{H'}j_H(H,H'\in \Pi ) \tag{15}
$$

$$
j_{H\cup H'}=j_H+j_{H'}-j_{H'}j_H(H,H'\in \Pi ) \tag{16}
$$

$$
j_{\emptyset}= 0,j_K= 1
$$

Soit $H\in \Pi$. On définit $A_H=j_HAj_H$. C’est une sous-algèbre fermée de A, admettant l’élément unité $j_H($cf. lemme 1 de I, p. 2). On pose également $B_H=j_HBj_H$ et $x_H=xj_H=j_Hx=j_Hxj_H\in B_H$.

Soit $g_H$ l’élément de $\mathscr{O}(K)$ défini par $g_H(z) =z$ au voisinage de H et $g_H(z) = 0$ au voisinage de K - H. On a $g_H(z) =f_H(z)z$ sur K, et donc $x_H=g_H(x)$. Il en résulte que, si $H\not= K$, on a

Sp$_A(x_H) =g_H(K) = H\cup  \{0\}$.

Soit $\lambda \in \mathbf{C}-$ H. Notons $h_{H,\lambda}$ l’élément de $\mathscr{O}(K)$ égal à $(\lambda -z)^{-1}$ au voisinage de H et à 0 au voisinage de K - H. On a $h_{H,\lambda}=f_Hh_{H,\lambda}$ et $(\lambda f_H-g_H)h_{H,\lambda}=f_H$. Si l’on note $R_H(x, \lambda ) =h_{H,\lambda}(x)$, on a donc $R_H(x, \lambda )\in B_H$ et

$$
R_H(x, \lambda )(\lambda j_H-x_H) = (\lambda j_H-x_H)R_H(x, \lambda ) =j_H \tag{17}
$$

$$
R_H(x, \lambda )j_{K-H}=j_{K-H}R_H(x, \lambda ) = 0
$$

En particulier, $\lambda \in \mathbf{C}-$ Sp$_{A_H}(x_H)$.

Soit maintenant $\lambda \in H$. Supposons que $\lambda j_H-x_H$ admette un inverse $y$ dans $A_H$. En utilisant les formules $j_Hy=y$ (car $y\in A_H)$ et $j_{K-H}R_{K-H}(x, \lambda ) = R_{K-H}(x, \lambda )$ (car $R_{K-H}(x, \lambda )\in A_{K-H})$, on trouve

$$
(\lambda -x)(y+ R_{K-H}(x, \lambda )) = (\lambda -x)(j_Hy+j_{K-H}R_{K-H}(x, \lambda )) =
$$

$$
(\lambda j_H-xj_H)y+ (\lambda j_{K-H}-xj_{K-H})R_{K-H}(x, \lambda ) =j_H+j_{K-H}= 1
$$

(grâce à la formule (17) appliquée à K - H). On vérifie de même que

$$
(y+ R_{K-H}(x, \lambda ))(\lambda -x) = 1
$$

Cela démontre que $\lambda -x$ admet dans A l’inverse $y+ R_{K-H}(x, \lambda )$, ce qui est absurde. Ainsi on a $\lambda \in$ Sp$_{A_H}(x_H)$. On conclut donc que

(18) Sp$_{A_H}(x_H) = H$. En particulier, si H est non vide, l’idempotent $j_H$ est non nul.

Les formules (17) et (18) prouvent que la fonction $\lambda \mapsto R_H(x, \lambda )$, définie dans $\mathbf{C}-$ H, est la résolvante de $x_H$ relativement à $A_H$.

#### Proposition 16 {#ts-i-s4-prop-16 .statement tag=02B4}

On conserve les notations précédentes. Soit $(H_i)_{1\leqslant i\leqslant n}$ une partition de Sp$_A(x)$ en éléments de Π.

a) L’algèbre B s’identifie canoniquement à l’algèbre $B_{H_1}\times \cdots \times B_{H_n}$;

b) On a $x_{H_i}x_{H_j}= 0$ pour $i\not=j$, et

$$
x=x_{H_1}+x_{H_2}+\cdots +x_{H_n}
$$

c) On a

$$
R(x, \lambda ) = R_{H_1}(x, \lambda ) +\cdots + R_{H_n}(x, \lambda ) \tag{19}
$$

pour tout $\lambda \in \mathbf{C}-$ Sp$_A(x)$. En particulier, si $H\in \Pi$, la résolvante $\lambda \mapsto R(x, \lambda )$ est égale au voisinage de H à la somme de $R_H(x, \lambda )$ et d’une fonction holomorphe.

La relation 1 = $j_{H_1}+\cdots +j_{H_n}$ est une décomposition de 1 en idempotents de B deux à deux orthogonaux, donc l’algèbre B s’identifie canoniquement à l’algèbre produit $B_{H_1}\times  \cdots  \times B_{H_n}$ (A, I, p. 105, prop. 10).

L’assertion b) résulte des relations correspondantes pour les fonctions $g_{H_i}$; l’assertion c) est une conséquence de a) et de l’égalité $R(x_H, \lambda ) = R_H(x, \lambda )$.

#### Proposition 17 {#ts-i-s4-prop-17 .statement tag=02B5}

Soit $\mu$ un point isolé de Sp$_A(x)$. Alors

a) Pour tout $\lambda \in \mathbf{C}-$ Sp$_A(x)$, on a

$R(x, \lambda ) = R_{\{\mu\}}(x, \lambda ) + R_{Sp_A(x)-\{\mu\}}(x, \lambda )$ ;

b) La fonction qui à $\lambda$ associe $R_{Sp_A(x)-\{\mu\}}(x, \lambda )$ est holomorphe dans $\mathbf{C}-$ Sp$_A(x)$ et au voisinage de $\mu$; de plus, la fonction qui à $\lambda$ associe $R_{\{\mu\}}(x, \lambda )$ est holomorphe dans $\mathbf{C}-\{\mu\}$;

c) On a

$_{n\rightarrow}$lim$_{+\infty}\|(x-\mu)^nj_{\{\mu\}}\|^{1/n}= 0$

et, pour $\lambda \in \mathbf{C}-\{\mu\}$, la formule

$$
R_{\{\mu\}}(x, \lambda ) =\sum_{n=0}^{\infty}(\lambda -\mu)^{-n-1}(x-\mu)^nj_{\{\mu\}} \tag{20}
$$

Ce qui précède entraîne les assertions a) et b). Prouvons c). En remplaçant $x$ par $x-\mu$, on se ramène au cas où $\mu= 0$. Posons $H =\{0\}$; c’est une partie ouverte et fermée de Sp$_A(x)$. D’après la formule (18), le spectre de $x_H$ dans $A_H$ est $\{0\}$, donc $x_H$ est quasi-nilpotent, c’est-àdire que $\|x^nj_H\|^{1/n}=\|(xj_H)^n\|^{1/n}$ tend vers 0 quand $n$ tend vers $+\infty$. En outre, pour $\lambda \not= 0$, on a dans $A_H$

$$
(\lambda j_H-x_H)^{-1}=\sum_{n=0}^{\infty}\lambda^{-n-1}x^n_H
$$

(théorème 1 de I, p. 24, d)), d’où (20).

#### Corollaire 1 {#ts-i-s4-prop-17-cor-1 .statement tag=02B6}

Soient $\mu$ un point isolé de Sp$_A(x)$ et $p$ un entier strictement positif. Pour que $\mu$ soit un pôle d’ordre $p$ de la résolvante de $x($cf. VAR, R1, p. 30, 3.3.9), il faut et il suffit que $(x-\mu)^{p-1}j_{\{\mu\}}\not= 0$ et $(x-\mu)^pj_{\{\mu\}}= 0$.

#### Corollaire 2 {#ts-i-s4-prop-17-cor-2 .statement tag=02B7}

Soit $\mu$ un point isolé de Sp$_A(x)$. Soit Γ le bord orienté d’un disque ouvert Δ de centre $\mu$ tel que

Sp$_A(x)\cap (\Gamma \cup \Delta ) =\{\mu\}$.

Alors l’idempotent $j_{\{\mu\}}$ associé à $x$ et $\{\mu\}$ est donné par

1 $\int_{-1}$

$$
j_{\{\mu\}}=(z-x)dz
$$

$$
2i\pi_{\Gamma}
$$

*En d’autres termes, l’idempotent $j_{\{\mu\}}$ est le résidu en $\mu$ de la résolvante de $x.*$

Pour $z\in \mathbf{C}-$ Sp$_A(x)$, on a

$$
(z-u)^{-1}= R(x, z) = R_{\{\mu\}}(x, z) + R_H(x, z)
$$

où H = Sp$_A(x)-\{\mu\}$ (formule (19)). La fonction $z\mapsto R_H(x, z)$ est holomorphe dans $\mathbf{C}-$ H et au voisinage de $\{\mu\}$ (prop. 17, b)), donc

1 $\int$

$$
R_H(x, z)dz= 0
$$

$$
2i\pi_{\Gamma}
$$

(VAR, R2, p. 48, 11.2.5). La fonction $z\mapsto R_{\{\lambda\}}(x, z)$ est la résolvante de l’élément $j_{\{\mu\}}xj_{\{\mu\}}$ de l’algèbre unifère $A_{\{\mu\}}$. On a alors

1 $\int$

$$
j_{\{\mu\}}=R_{\{\mu\}}(x, z)dz
$$

$$
2i\pi_{\Gamma}
$$

d’après la prop. 9 de I, p. 75 appliquée à $A_{\{\mu\}}$ et à la fonction constante 1 au voisinage de $\Delta \cup \Gamma$. Le corollaire en résulte.

### 13. Calcul fonctionnel holomorphe dans une algèbre normable complète réelle ou complexe

Soit E un espace vectoriel topologique réel. L’espace vectoriel topologique $\mathbf{C}\otimes E$ complexifié de E (EVT, II, p. 65) est noté $E_{(\mathbf{C})}$ et E est identifié à un sous-espace vectoriel topologique réel de $E_{(\mathbf{C})}$ par l’application $x\mapsto 1\otimes x$.

#### Proposition 18 {#ts-i-s4-prop-18 .statement tag=02B8}

L’espace vectoriel topologique complexe $E_{(\mathbf{C})}$ est normable (resp. complet) si et seulement si E est normable (resp. complet).

L’espace vectoriel topologique réel sous-jacent à $E_{(\mathbf{C})}$ est isomorphe à $E\times E$. Ainsi $E_{(\mathbf{C})}$ est complet si et seulement si E est complet, et E est normable si $E_{(\mathbf{C})}$ l’est.

Supposons inversement que E est normable. Soient $p$ une norme qui définit la topologie de E et B la boule unité de $p$. Il existe un voisinage fermé équilibré V de 0 dans $E_{(\mathbf{C})}$ contenu dans $B +iB$ (EVT, II, p. 66). Les ensembles $\lambda V$, où $\lambda$ décrit $\mathbf{R}^*_+$, forment donc un système fondamental de voisinages de 0 dans $E_{(\mathbf{C})}$. La jauge de V est une norme sur $E_{(\mathbf{C})}$ qui définit la topologie de $E_{(\mathbf{C})}$, donc $E_{(\mathbf{C})}$ est normable.

#### Remarque {#ts-i-s4-n13-rem-1 .statement tag=02B9}

Soient E et F des espaces vectoriels topologiques normables sur K. L’espace vectoriel $\mathscr{L}(E; F)$ des applications linéaires continues de E dans F, muni de la topologie de la convergence bornée, est un espace vectoriel topologique normable (EVT, III, p. 14).

Soient E et F des espaces vectoriels topologiques normables sur $\mathbf{R}$. L’application $\mathbf{C}$-linéaire $\varphi :\mathscr{L}(E; F)_{(\mathbf{C})}\rightarrow \mathscr{L}(E_{(\mathbf{C})}; F_{(\mathbf{C})})$ définie par $\varphi (\lambda \otimes u) =\lambda u_{(\mathbf{C})}$ est un isomorphisme d’espaces vectoriels topologiques complexes. En particulier, le dual de $E_{(\mathbf{C})}$ s’identifie au complexifié du dual de E et l’algèbre normable $\mathscr{L}(E_{(\mathbf{C})})$ à la complexifiée de l’algèbre normable $\mathscr{L}(E)$.

Soit S une partie compacte de $\mathbf{C}$ stable par la conjugaison complexe. Considérons la $\mathbf{C}$-algèbre $\mathscr{O}(S)$ des germes de fonctions holomorphes à valeurs complexes au voisinage de S, munie de la structure d’espace localement convexe complexe définie au n$^o1$ de I, p. 49. Si U est un voisinage ouvert de S dans $\mathbf{C}$, et $h: U\rightarrow \mathbf{C}$ une fonction holomorphe, l’image V de U par la conjugaison complexe est un voisinage ouvert de S dans $\mathbf{C}$ et $h^*:w\mapsto \overline{h(\overline{w})}$ est une fonction holomorphe sur V. On en déduit par passage à la limite inductive une involution continue $f\mapsto f^*$ dans l’algèbre $\mathscr{O}(S)$. On a en particulier :

$$
(f+g)^*=f^*+g^*(f g)^*=f^*g^*(\lambda f)^*=\lambda f^*
$$

pour $f, g$ dans $\mathscr{O}(S)$ et $\lambda$ dans $\mathbf{C}$.

On note $\mathscr{O}_{\mathbf{R}}(S)$ l’ensemble des germes $f\in \mathscr{O}(S)$ tels que $f=f^*$. C’est une sous-$\mathbf{R}$-algèbre fermée pleine de $\mathscr{O}(S)$.

#### Proposition 19 {#ts-i-s4-prop-19 .statement tag=02BA}

Notons $z$ le germe dans $\mathscr{O}(S)$ de l’application identique de $\mathbf{C}$. Alors $\mathscr{O}_{\mathbf{R}}(S)$ est la plus petite sous-$\mathbf{R}$-algèbre fermée pleine de $\mathscr{O}(S)$ contenant $z$.

On a $z^*=z$, donc $z$ appartient à $\mathscr{O}_{\mathbf{R}}(S)$. Soit B une sous-$\mathbf{R}$-algèbre fermée pleine de $\mathscr{O}(S)$ contenant $z$. L’application $f\mapsto f+f^*$ de $\mathscr{O}(S)$ dans $\mathscr{O}_{\mathbf{R}}(S)$ est continue et surjective, et l’ensemble des germes de fonctions rationnelles holomorphes au voisinage de S est dense dans $\mathscr{O}(S)$ (th. 3 de I, p. 69). Pour démontrer que B contient $\mathscr{O}_{\mathbf{R}}(S)$, il suffit donc de démontrer que si $f$ est le germe d’une telle fonction rationnelle, on a $f+f^*\in B$.

Il existe des polynômes P et Q dans $\mathbf{C}[X]$ tels que Q ne s’annule en aucun point de S et que l’on ait $f=\frac{P(z)}{Q(z)}$. Notons $P^*$ et $Q^*$ les polynômes obtenus en remplaçant les coefficients de P et Q par leurs conjugués. On a alors $P(z)^*= P^*(z)$ et $Q(z)^*= Q^*(z)$. Comme S est stable par la conjugaison complexe, le polynôme $Q^*$ ne s’annule en aucun point de S. Les germes $Q^*(z)$ et (QQ$^*)(z)$ sont donc inversibles dans $\mathscr{O}(S)$, et

$_*P(z)P^*(z)$ (PQ$^*+ P^*Q)(z)$

$f+f$ = + $_*$ = $*$.

$Q(z)$ Q $(z)$ (QQ $)(z)$

Comme les polynômes PQ$^*+ P^*Q$ et QQ$^*$ sont à coefficients réels et que B est une sous-$\mathbf{R}$-algèbre pleine de $\mathscr{O}(S)$ contenant $z$, l’élément $f+f^*$ appartient à B. Cela conclut la preuve de la proposition.

Soit A une algèbre unifère normable complète sur $\mathbf{R}$. Soit $x$ un élément de A. Le spectre de l’élément $1\otimes x$ de l’algèbre $A_{(\mathbf{C})}$ est appelé le spectre complexe de $x$, et il est noté Sp$_{A_{(\mathbf{C})}}(x)$. Son intersection avec l’ensemble $\mathbf{R}$ n’est autre que le spectre Sp$_A(x)$ de $x$ relativement à A, que l’on appelle parfois le spectre réel de $x$. Le spectre complexe Sp$_{A_{(\mathbf{C})}}(x)$ est une partie compacte de $\mathbf{C}$, stable par la conjugaison complexe. Il n’est pas vide lorsque l’algèbre A n’est pas réduite à 0.

Soit $x$ un élément de A. Le rayon spectral de $1\otimes x\in A_{(\mathbf{C})}$ est égal au rayon spectral $\varrho (x)$ de $x$. C’est le plus petit nombre réel $r\geqslant 0$ tel que $|\lambda |\leqslant r$ pour tout $\lambda \in$ Sp$_{A_{(\mathbf{C})}}(x)$. On a

$\varrho (x) =_{n\rightarrow}$lim$_{+\infty}\|x^n\|^{1/n}=$ inf$_{n>0}\|x^n\|^{1/n}$

pour toute norme sur A qui définit la topologie de A. En effet, on peut supposer que la norme sur A est la restriction d’une norme sur $A_{(\mathbf{C})}$ qui définit la topologie de $A_{(\mathbf{C})}$ et appliquer la prop. 1 de I, p. 20.

Notons $u\mapsto \overline{u}$ l’endomorphisme de la $\mathbf{R}$-algèbre $A_{(\mathbf{C})}$ qui applique $\lambda \otimes a$ sur $\lambda \otimes a$. Il est continu.

#### Lemme {#ts-i-s4-n13-lem-1 .statement tag=02BB}

Pour tout $f\in \mathscr{O}$(Sp$_{A_{(\mathbf{C})}}(x))$, on a $f^*(1\otimes x) =\overline{f(1 \otimes x)}$.

Les applications $f\mapsto f(1\otimes x)$ et $f\mapsto \overline{f^*(1 \otimes x)}$ sont des homomorphismes unifères continus de $\mathbf{C}$-algèbres de $\mathscr{O}$(Sp($x$)) dans $A_{(\mathbf{C})}$ qui appliquent $z$ sur $1\otimes x$; elles sont donc égales (I, p. 74, th. 5).

#### Proposition 20 {#ts-i-s4-prop-20 .statement tag=02BC}

Pour tout $f\in \mathscr{O}_{\mathbf{R}}$(Sp$_{A_{(\mathbf{C})}}(x))$, il existe un unique élément $f(x)$ de A tel que $f(1\otimes x) = 1\otimes f(x)$ dans $A_{(\mathbf{C})}$. L’application $f\mapsto f(x)$ de $\mathscr{O}_{\mathbf{R}}$(Sp$_{A_{(\mathbf{C})}}(x))$ dans A est l’unique homomorphisme unifère continu de $\mathbf{R}$-algèbres qui applique sur $x$ le germe dans $\mathscr{O}_{\mathbf{R}}$(Sp$_{A_{(\mathbf{C})}}(x))$ de l’application identique de $\mathbf{C}$.

Notons S = Sp$_{A_{(\mathbf{C})}}(x)$. D’après le lemme ci-dessus, pour tout germe $f\in \mathscr{O}_{\mathbf{R}}$(Sp($x$)), on a $f(1\otimes x) =\overline{f(1 \otimes x)}$. La première assertion en résulte. Notons $z$ le germe dans $\mathscr{O}_{\mathbf{R}}(S)$ de l’application identique de $\mathbf{C}$. L’application $f\mapsto f(x)$ est un homomorphisme continu unifère de la $\mathbf{R}$-algèbre $\mathscr{O}_{\mathbf{R}}$(Sp($x$)) dans A, qui applique $z$ sur $x$. C’est le seul d’après la prop. 19, puisque tout morphisme ayant ces propriétés est déterminé de manière unique sur toute sous-$\mathbf{R}$-algèbre fermée pleine de $\mathscr{O}(S)$ contenant $z$.

Soit $f\in \mathscr{O}_{\mathbf{R}}$(Sp$_{A_{(\mathbf{C})}}(x))$. L’élément $f(x)$ appartient à toute sous-algèbre fermée pleine de A contenant $x$ (prop. 19), donc appartient au bicommutant de $x$ dans A. Le spectre complexe de $f(x)$ est égal à $f$(Sp($x$)) (I, p. 75, prop. 8). Pour tout $g\in \mathscr{O}_{\mathbf{R}}(f$(Sp$_{A_{(\mathbf{C})}}(x)))$, on a $g\circ f\in \mathscr{O}_{\mathbf{R}}$(Sp$_{A_{(\mathbf{C})}}(x))$ et (loc. cit.) $(g\circ f)(x) =g(f(x))$.

Soit U une partie ouverte de $\mathbf{C}$, stable par la conjugaison complexe. L’ensemble Ω des éléments $x$ de A dont le spectre complexe est contenu dans U est ouvert dans A (I, p. 76, prop. 10). Soit $f$ une fonction holomorphe sur U telle que $f^*=f$. L’application $x\mapsto f(x)$ de Ω dans A est analytique (loc. cit.).

Soient A, B des algèbres associatives unifères normables complètes sur $\mathbf{R}$ et $\varphi : A\rightarrow$ B un morphisme d’algèbres unifère continu. Soit $x\in A$. Le spectre complexe de $\varphi (x)$ est contenu dans celui de $x$ et, pour tout $f\in \mathscr{O}_{\mathbf{R}}$(Sp$_{A_{(\mathbf{C})}}(x))$, on a $f(\varphi (x)) =\varphi (f(x))$. Cela résulte aussitôt de l’énoncé analogue dans le cas complexe (I, p. 75, prop. 8).

### 14. Cas d’une algèbre sans élément unité

Soit A une algèbre normable complète non nécessairement unifère sur $K =\mathbf{R}$ ou $\mathbf{C}$. Notons $(\widetilde{A}, e)$ l’algèbre unifère déduite de A par adjonction d’un élément unité. Elle est normable et complète.

Soit $x$ un élément de A. Si $K =\mathbf{C}$, notons Sp$'(x) =$ Sp$_{\widetilde{A}}(x)$ le spectre de $x$ relativement à $\widetilde{A}$, et considérons un germe $f\in \mathscr{O}$(Sp$'(x))$. Si $K =\mathbf{R}$, notons Sp$'(x)$ le spectre complexe de l’élément $x$ de $\widetilde{A}$, et considérons un germe $f\in \mathscr{O}_{\mathbf{R}}$(Sp$'(x))$. Dans ces deux cas, 0 appartient à Sp$'(x)$, et l’élément $f(x)$ de $\widetilde{A}$ appartient à A si et seulement si $f$ vérifie $f(0) = 0$. En effet, la projection $\pi :\widetilde{A}\rightarrow Ke$ est un morphisme continu dont le noyau est A, et l’on a $\pi (f(x)) =f(\pi (x)) =f(0)$.

## EXERCICES {#ts-i-s4-exercises}

Dans les exercices ci-dessous, toutes les algèbres considérées sont sur $\mathbf{C}$, sauf mention explicite du contraire.

See the [exercises for § 4](exercises/s4/).
