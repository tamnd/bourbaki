---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 19
section_title: Algèbres de quaternions
lang: fr
source: alg-viii-fr
book_pages: A VIII.353-A VIII.363
pdf_pages: 0356-0366
extraction: native
subsections:
    - "no": 1
      title: Propriétés générales des algèbres de quaternions
      page: 353
      pdf_page: 356
    - "no": 2
      title: Centre des algèbres de quaternions
      page: 355
      pdf_page: 358
    - "no": 3
      title: Simplicité des algèbres de quaternions
      page: 355
      pdf_page: 358
    - "no": 4
      title: Critères pour qu’une algèbre de quaternions soit un corps
      page: 357
      pdf_page: 360
    - "no": 5
      title: Algèbres sur un corps ordonné maximal
      page: 359
      pdf_page: 362
statements: 16
exercises: 8
content_sha256: 4d8e0cf5236836667cbbaa2a8cb527fe85f1043aab46f74caa68aaf232b4d638
---

## § 19. ALGÈBRES DE QUATERNIONS

Dans ce paragraphe, la lettre K désigne un corps commutatif.

### 1. Propriétés générales des algèbres de quaternions

Soient $\alpha , \beta , \gamma$ des éléments de K et soit F l’algèbre de quaternions de type $(\alpha , \beta , \gamma )$. Rappelons (III, p. 18) que F est une K-algèbre associative et unifère possédant une base $(1, i, j, k)$ sur K satisfaisant aux relations

$$
i^2=\alpha +\beta i,j^2=\gamma ,ij=k,ji=\beta j-k \tag{1}
$$

C’est une algèbre cayleyenne (III, p. 15, déf. 1) dont la conjugaison satisfait à

$$
\overline{i}=\beta -i,\overline{j}=-j,\overline{k}=-k \tag{2}
$$

Rappelons que la trace et la norme cayleyennes de F sont les applications $T_F$ et $N_F$ de F dans K définies par $T_F(q) =q+\overline{q}$ et $N_F(q) =qq$.

Le sous-espace vectoriel E de F de base $(1, i)$ est une sous-algèbre cayleyenne commutative de F ; c’est une algèbre quadratique de type $(\alpha , \beta )$ et F s’identifie à l’extension cayleyenne de E définie par $\gamma$ (III, p. 17). Pour tout $z\in E$, on a $zj=jz$. Tout élément $q$ de F s’écrit de manière unique sous la forme $x+jy$, avec $x, y\in E$, et l’on a

$$
\overline{q}=\overline{x}-jy,T_F(q) =x+\overline{x},N_F(q) =xx-\gamma yy \tag{3}
$$

#### Proposition 1 {#alg-viii-s19-prop-1 .statement tag=00LQ}

Le polynôme caractéristique d’un élément $q$ de F est égal à $(X^2-T_F(q)X + N_F(q))^2$.

D’après ce qui précède, l’algèbre F est un E-module à droite libre de base $(1, j)$. Par conséquent, F[X] est un E[X]-module à droite libre de base $(1, j)$. Notons $u$ l’endomorphisme du E[X]-module à droite F[X] défini par $u(P) = (X-q)P$ pour tout $P\in F[X]$. Le polynôme caractéristique de $q$ est le déterminant de $u$ considéré comme endomorphisme du K[X]-module F[X]. D’après la prop. 6 de III, p. 112, il est égal à N(det $u$), où N désigne la norme de E[X] à K[X]. Écrivons $q$ sous la forme $x+jy$, avec $x, y\in E$. La matrice de $u$ par rapport à la base $(1, j)$ est $\begin{pmatrix} X-x & -\gamma y \\ -y & X-\overline{x} \end{pmatrix}$ ; son déterminant est égal à $D = (X-x)(X-\overline{x})-\gamma yy= X^2-T_F(q)X + N_F(q) ($cf. formule (3)). Comme D appartient à K[X], on a $N(D) = D^2$, d’où la prop. 1.

#### Remarque 1 {#alg-viii-s19-n1-rem-1 .statement tag=00LR}

Supposons la caractéristique de K différente de 2 et posons $i'=$ $2i-\beta$. Alors $(1, i')$ est une base de E sur K et l’on a ${i'}^2= 4\alpha +\beta^2$. Il en résulte que E est isomorphe à l’algèbre quadratique de type $(4\alpha +\beta^2,0)$ et F à l’algèbre de quaternions de type $(4\alpha +\beta^2,0, \gamma )$.

#### Remarque 2 {#alg-viii-s19-n1-rem-2 .statement tag=00LS}

L’algèbre de quaternions de type $(\alpha ,0, \gamma )$ est isomorphe à l’algèbre de quaternions de type $(\gamma ,0, \alpha )$ (III, p. 18). Elle est aussi isomorphe à l’algèbre de quaternions de type $(\alpha a^2,0, \gamma c^2)$ pour tout couple $(a, c)$ d’éléments non nuls de K.

#### Remarque 3 {#alg-viii-s19-n1-rem-3 .statement tag=00LT}

Soit $q$ un élément de F. Pour que $q$ soit nilpotent, il faut et il suffit que son polynôme caractéristique soit égal à $X^4$, c’est-à-dire que $T_F(q) = N_F(q) = 0$ et on a alors $q^2= 0$.

#### Exemple {#alg-viii-s19-n1-exa-1 .statement tag=00LU}

L’algèbre de matrices $\mathbf{M}_2(K)$ est isomorphe à l’algèbre de quaternions de type $(0,1,1)$. Considérons en effet l’algèbre quadratique $E = K\times K$ (de type $(0,1)$) et l’algèbre de quaternions $F = E + Ej$, extension cayleyenne de E définie par l’élément $\gamma = 1$. L’application $(a, b)\rightarrow \begin{pmatrix} a & 0 \\ 0 & b \end{pmatrix}$ est un homomorphisme d’algèbres de E dans $\mathbf{M}_2(K)$. Comme l’on a, pour $a, b$ dans K,

0 1 0 1 1 0 0 1 $a$ 0 $b$ 0 0 1

= =.

1 0 1 0 0 1 1 0 0 $b$ 0 $a$ 1 0

cet homomorphisme se prolonge en un homomorphisme d’algèbres $\theta : F\longrightarrow \mathbf{M}_2(K)$ défini par

$$
()a c
$$

$\theta (a, b) + (c, d)j$ =.

$$
d b
$$

Cet homomorphisme est bijectif. Lorsque la caractéristique de K est différente de 2, l’algèbre $\mathbf{M}_2(K)$ est aussi isomorphe à l’algèbre de quaternions de type $(1,0,1)$ (remarque 1).

### 2. Centre des algèbres de quaternions

Soient $\alpha ,\beta ,\gamma$ des éléments de K et soit F l’algèbre de quaternions de type $(\alpha , \beta , \gamma )$.

#### Proposition 2 {#alg-viii-s19-prop-2 .statement tag=00LV}

a) Supposons le corps K de caractéristique différente de 2. Si $\gamma$ ou $4\alpha +\beta^2$ est non nul, le centre de F est égal à K ; sinon il est de dimension 2 et engendré par 1 et $ij-ji$.

b) Supposons le corps K de caractéristique 2. Si $\beta \not= 0$, le centre de F est égal à K ; si $\beta = 0$, l’algèbre F est commutative.

D’après la formule (30) de III, p. 18, on a

$$
ij-ji=-\beta j+ 2k,jk-kj=\beta \gamma -2\gamma i,ki-ik=-2\alpha j-\beta k \tag{4}
$$

Pour qu’un élément $q=x+yi+zj+tk$ de F soit central, il faut et il suffit qu’il commute avec $i$ et $j$, c’est-à-dire qu’on ait

(5) $2z+\beta t=-\beta z+ 2\alpha t= 0$ et $2\gamma t=\beta \gamma t= 2y=\beta y= 0$.

Supposons d’abord la caractéristique de K différente de 2. Si $\gamma$ est non nul, les égalités (5) entraînent $y=t= 0$ puis $z= 0$, d’où $q\in K$. Si $\gamma = 0$ et $4\alpha +\beta^2\not= 0$, elles entraînent $y=z=t= 0$ d’où $q\in K$. Si $\gamma = 4\alpha +\beta^2= 0$, le système (5) se réduit à $y= 2z+\beta t= 0$, d’où $q=x+t/2(ij-ji)$, ce qui conclut la preuve de a).

Supposons maintenant le corps K de caractéristique 2. Le système (5) s’écrit alors $\beta t=\beta z=\beta y= 0$, d’où b).

### 3. Simplicité des algèbres de quaternions

#### Proposition 3 {#alg-viii-s19-prop-3 .statement tag=00LW}

Soient $\alpha ,\beta ,\gamma$ des éléments de K et soit F une algèbre de quaternions de type $(\alpha , \beta , \gamma )$. Notons $T_F$ et $N_F$ sa trace et sa norme cayleyennes. Les conditions suivantes sont équivalentes :

(i) L’algèbre F est centrale et simple ;

(ii) Pour tout élément non nul $x$ de F, il existe $y\in F$tel que $T_F(xy)\not= 0$;

(iii) On a $(4\alpha +\beta^2)\gamma \not= 0$.

Supposons qu’elles soient satisfaites. Alors, pour tout $x$ appartenant à F, le polynôme caractéristique réduit de $x$ est $X^2-T_F(x)X + N_F(x)$. En particulier, $T_F(x)$est la trace réduite de $x$ et $N_F(x)$sa norme réduite.

(i)$\Rightarrow$(ii) : Si l’algèbre F est centrale et simple, il résulte de la prop. 1 de VIII, p. 353 et de la définition de la trace réduite (VIII, p. 334, déf. 2) que $T_F$ est sa trace réduite d’où (ii) (VIII, p. 336, prop. 5).

(ii)$\Leftrightarrow$(iii) : Soit $(e_i)_{1\leqslant i\leqslant 4}$ une base de F de type $(\alpha , \beta , \gamma )$ (III, p 18). La matrice $(T_F(e_ie_j))$ est égale à

2 $\beta$ 0 0

$\beta 2\alpha +\beta^2$ 0 0

.

0 0 $2\gamma \beta \gamma$

0 0 $\beta \gamma -2\alpha \gamma$

Son déterminant est $-\gamma^2(4\alpha +\beta^2)^2$. L’équivalence des conditions (ii) et (iii) résulte de V, p. 47, lemme 1.

(iii)$\Rightarrow$(i) : Supposons $(4\alpha +\beta^2)\gamma \not= 0$. On a alors $\gamma \not= 0$ et on a $\beta \not= 0$ si K est de caractéristique 2. D’après la prop. 2, l’algèbre F est centrale. Soit $x$ un élément du radical de Jacobson de F. Pour tout $y\in F,xy$ est nilpotent, donc $T_F(xy) = 0$ (remarque 3 de VIII, p. 354). Comme (ii) est équivalent à (iii), on a $x= 0$. Cela prouve que F est une K-algèbre semi-simple. Puisque son centre est K, elle est simple.

La dernière assertion résulte de la prop. 1 et de la définition du polynôme caractéristique réduit (VIII, p. 333, déf. 1).

Notons $p$ la caractéristique de K. D’après la prop. 3, si $p\not= 2$, toute algèbre de quaternions sur K de type $(\alpha ,0, \gamma )$, avec $\alpha$ et $\gamma$ dans $K^*$, est centrale et simple. Si $p= 2$, toute algèbre de quaternions de type $(\alpha ,1, \gamma )$, avec $\alpha \in K$ et $\gamma \in K^*$, est centrale et simple. Inversement :

#### Proposition 4 {#alg-viii-s19-prop-4 .statement tag=00LX}

Soit A une algèbre centrale et simple de degré 4 sur K. Notons $p$ la caractéristique de K.

a) Si $p\not= 2$, il existe des éléments non nuls $\alpha$ et $\gamma$ de K tels que l’algèbre A soit isomorphe à l’algèbre de quaternions de type $(\alpha ,0, \gamma )$.

b) Si $p= 2$, il existe un élément $\alpha$ de K et un élément $\gamma$ de $K^*$ tels que l’algèbre A soit isomorphe à l’algèbre de quaternions de type $(\alpha ,1, \gamma )$.

D’après le théorème de Wedderburn (VIII, p. 116, th. 1), il existe un entier $r\geqslant 1$ et un corps D de centre K tels que A soit isomorphe à $\mathbf{M}_r(D)$. On a alors $r^2[D : K] = [A : K] = 4$. Si $r= 2, A$ est isomorphe à $\mathbf{M}_2(K)$ et la proposition 4 résulte de l’exemple de VIII, p. 354 ; sinon, on a $r= 1$ et A est un corps de centre K. Il possède alors un sous-corps commutatif maximal E qui est une extension séparable de K ; comme A est de degré 4 sur K, l’extension E est de degré 2 sur K (VIII, p. 261, cor. 2). Elle est donc quadratique (III, p. 16). Soit $s$ la conjugaison dans E (III, p. 14). D’après le théorème de Skolem-Noether (VIII, p. 253, cor. 1), il existe un élément inversible $j$ de A tel que l’on ait $s(x) =jxj^{-1}$ pour tout $x$ dans E. Comme E est séparable sur K, on a $s\not=$ Id$_E$, d’où $j /\in E$; comme A est un espace vectoriel de dimension 4 sur K, c’est un espace vectoriel à gauche de dimension 2 sur E, d’où $A = E\oplus Ej$. Comme $s^2=$ Id$_E$, l’élément $j^2$ de A appartient au centre de A ; il existe donc un élément $\gamma$ de $K^*$ tel que $j^2=\gamma$.

Lorsque $p\not= 2$, il existe un élément $i$ de E et un élément $\alpha \in K^*$ tels que $E = K(i)$ et $i^2=\alpha$ (V, p. 86, exemple 3) ; dans ce cas, A est isomorphe à l’algèbre de quaternions de type $(\alpha ,0, \gamma )$. Lorsque $p= 2$, il existe un élément $i$ de E et un élément $\alpha$ de K tels que $E = K(i)$ et $i^2=i+\alpha$ (V, p. 89, exemple 2), de sorte que A est isomorphe à l’algèbre de quaternions de type $(\alpha ,1, \gamma )$.

#### Corollaire 1 {#alg-viii-s19-prop-4-cor-1 .statement tag=00LY}

Soit A une K-algèbre centrale et simple, de degré fini $>1$, dont tout élément est algébrique de degré $\leqslant 2$sur K. Alors A est isomorphe à une algèbre de quaternions sur K.

Si K est fini, l’algèbre A est isomorphe à une algèbre de matrices $\mathbf{M}_n(K)$ (VIII, p. 349, cor. 2), donc contient des éléments de degré $n$ sur K ; l’hypothèse entraîne $n= 2$, d’où le résultat dans ce cas (VIII, p. 354, exemple). Supposons le corps K infini. Soit L une sous-algèbre étale maximale de A. D’après V, p. 40, prop. 7, il existe un élément $x$ de A tel que la K-algèbre L soit égale à $K[x]$, donc par hypothèse de degré $\leqslant 2$. Comme on a $[A : K] = [L : K]^2$ (VIII, p. 260, prop. 4 et p. 258, prop. 3) on en déduit [A : K] = 4 ; le corollaire 1 résulte alors de la prop. 4.

#### Corollaire 2 {#alg-viii-s19-prop-4-cor-2 .statement tag=00LZ}

Soit $(E, s)$une algèbre cayleyenne sur K, telle que la K-algèbre E soit centrale, simple et de degré fini $>1$sur K. Alors E est isomorphe à une algèbre de quaternions sur K.

Tout élément $u$ de E satisfait à $u^2-T_E(u)u+ N_E(u) = 0$, donc la K-algèbre E est isomorphe à une algèbre de quaternions (cor. 1).

### 4. Critères pour qu’une algèbre de quaternions soit un corps

Soient $\alpha , \beta , \gamma$ des éléments du corps K et soit F l’algèbre de quaternions de type $(\alpha , \beta , \gamma )$. Comme au n$^o$ 1, notons $(1, i, j, k)$ la base canonique de F et E la sous-algèbre $K + Ki$ de F.

#### Proposition 5 {#alg-viii-s19-prop-5 .statement tag=00M0}

Les conditions suivantes sont équivalentes :

(i) L’algèbre de quaternions F est un corps ;

(ii) Il n’existe aucun élément non nul $q\in F$tel que $T_F(q) = N_F(q) = 0$;

(iii) Tout élément de F de carré nul est nul ;

(iv) Il n’existe aucun vecteur non nul $(x, y, z, t)$de $K^4$ tel que

$$
x^2+\beta xy-\alpha y^2-\gamma (z^2+\beta zt-\alpha t^2) = 0
$$

(v) Il n’existe aucun vecteur non nul $(x, y, z)$de $K^3$ tel que

$$
x^2+\beta xy-\alpha y^2-\gamma z^2= 0
$$

(vi) L’algèbre quadratique E est un corps et $\gamma$ n’est pas la norme d’un élément de E.

Pour qu’un élément $q$ de F soit inversible, il faut et il suffit que $N_F(q)$ soit différent de 0. L’équivalence de (i) et (iv) résulte donc de la formule (31) de III, p. 18 ; il est clair que (i) implique (iii) et que (iv) implique (v).

L’équivalence de (ii) et (iii) résulte de la remarque 3 de VIII, p. 354.

Supposons que F ne soit pas un corps. Si $\gamma (4\alpha +\beta^2)\not= 0$, l’algèbre F est centrale et simple de degré 4 sur K ; elle est isomorphe à l’algèbre $\mathbf{M}_2(K)$ (VIII, p. 116, th. 1) et contient donc un élément non nul de carré nul. Si $\gamma = 0$, on a $j^2= 0$. Si $4\alpha +\beta^2= 0$, on a $(2i-\beta )^2= 0$ et $2i-\beta \not= 0$ si K est de caractéristique différente de 2. Enfin, si K est de caractéristique 2 et que $\beta$ est nul, on a $T_F(q) = 0$ pour tout $q\in F$ (III, p. 18, formule (31)) ; comme F n’est pas un corps, il existe un élément non nul $q$ de F tel que $N_F(q) = 0$; on a $q^2= 0$. Cela démontre l’implication (iii)$\Rightarrow$(i).

Soit $q=x+yi$ un élément de E. On a $N_{E/K}(q) =x^2+\beta xy-\alpha y^2$. Supposons la condition (v) satisfaite. On a $N_{E/K}(q)-\gamma \not= 0$ et $N_{E/K}(q)\not= 0$ si $q\not= 0$, d’où (vi).

Enfin, supposons la condition (vi) satisfaite. Soit $q$ un élément non nul de F ; écrivons-le sous la forme $u+vj$, avec $u$ et $v$ dans E. Si $v$ est nul, $q$ est inversible. Si $v$ n’est pas nul, on a $N_F(q) = N_F(v)N_F(v^{-1}u+j) = N_{E/K}(v)(N_{E/K}(v^{-1}u)-\gamma )$ d’après III, p. 17, formule (24). Comme $\gamma$ n’est pas une norme, $N_F(q)$ n’est pas nul, et $q$ est inversible.

#### Remarque {#alg-viii-s19-n4-rem-1 .statement tag=00RQ}

Supposons que l’algèbre de quaternions F soit un corps. Il résulte de l’égalité $j^2=\gamma$ que l’on a $\gamma \not= 0$. D’après la prop. 2 de VIII, p. 355, le centre de F est égal à K, sauf si K est de caractéristique 2 et que $\beta$ est nul, auquel cas l’algèbre F est commutative.

### 5. Algèbres sur un corps ordonné maximal

Soit R un corps ordonné maximal (VI, p. 24). Soit C la R-algèbre quadratique de type $(-1,0)$; si $(1, i)$ est sa base canonique, on a $i^2=-1$. De plus, C est une clôture algébrique de R (VI, p. 25, th. 3). Soit H la R-algèbre de quaternions de type $(-1,0,-1)$. La table de multiplication de H dans sa base canonique $(1, i, j, k)$ est donnée par

$$
i^2=j^2=k^2=-1,ij=-ji=k,-ik=ki=j,jk=-kj=i
$$

On identifie C à la sous-algèbre $R + Ri$ de H. Le conjugué d’un élément $q=x+yi+$ $zj+tk$ de H est $\overline{q}=x-yi-zj-tk$. La trace et la norme cayleyennes de $q$ sont données par

$$
T(q) =q+\overline{q}= 2x,N(q) =qq=x^2+y^2+z^2+t^2
$$

Comme R est un corps ordonné, on a $N(q)>0$ si $q\not= 0$, donc H est un corps, de centre R (VIII, p. 355, prop. 2). La trace et la norme réduites d’un élément $q$ de H sont $T(q)$ et $N(q)$ respectivement.

#### Théorème 1 {#alg-viii-s19-thm-1 .statement tag=00M1}

Soit D une R-algèbre de degré fini qui est un corps. Alors D est isomorphe à R, C ou H.

Notons Z le centre de D et soit L un sous-corps commutatif maximal de D. On a $[D : Z] = [L : Z]^2$ d’après VIII, p. 261, cor. 2 ; de plus, on a $[L : R]\leqslant 2$ puisque C est une clôture algébrique de R. Il y a donc trois cas possibles :

a) On a R = Z = L, d’où [D : Z] = 1 et D = R.

b) On a $R\not= Z$ et Z = L, d’où [D : Z] = 1 et D = L ; dans ce cas, D est isomorphe à C.

c) On a R = Z et [L : R] = 2, d’où [D : R] = 4. D’après la prop. 4 de VIII, p. 356, la R-algèbre D est isomorphe à une algèbre de quaternions de type $(\alpha ,0, \gamma )$ où $\alpha$ et $\gamma$ sont des éléments non nuls de R. Soit $i\in D$ - Z tel que $i^2=\alpha$. On a $\alpha \not= 0$. Si $\alpha  >0$, il existe $a\in R$ tel que $a^2=\alpha$ (VI, p. 25, th. 3) ; on a alors $(a-i)(a+i) = 0$, ce qui est absurde puisque D est un corps. On a donc $\alpha  <0$. On démontre de même l’inégalité $\gamma  <0$. Il existe alors des éléments $a$ et $c$ de $R^*$ tels que $\alpha =-a^2$ et $\gamma =-c^2($loc. cit.). L’algèbre D est donc isomorphe à l’algèbre de quaternions de type $(-1,0,-1)$ (VIII, p. 354, remarque 2), c’est-à-dire à H.

#### Remarque 1 {#alg-viii-s19-n5-rem-1 .statement tag=00M2}

Soit O l’algèbre d’octonions de type $(-1,0,-1,-1)$ sur R (III, p. 176). Soit D une algèbre cayleyenne alternative sur R telle que tout élément non nul de D ait un inverse. On peut démontrer (VIII, p. 362, exerc. 5) que D est isomorphe à R, C, H ou O.

#### Remarque 2 {#alg-viii-s19-n5-rem-2 .statement tag=00M3}

Ce qui précède s’applique au corps $\mathbf{R}$des nombres réels. Toute $\mathbf{R}$-algèbre de

degré fini qui est un corps est isomorphe à $\mathbf{R}, \mathbf{C}$ou $\mathbf{H}$.

#### Remarque 3 {#alg-viii-s19-n5-rem-3 .statement tag=00M4}

Soit A une algèbre normée sur le corps $\mathbf{R}$. Supposons que A soit un corps. Alors A est isomorphe à $\mathbf{R}, \mathbf{C}$ou $\mathbf{H}$(« théorème de Gelfand-Mazur ») (cf. AC, p. 123, th. 1 et TS, I, §2, n$^o5$, cor. $2$)$.*$

## EXERCICES {#alg-viii-s19-exercises}

See the [exercises for § 19](exercises/s19/).
