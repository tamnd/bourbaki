---
book: ta
book_title: Topologie algébrique
chapter: I
chapter_title: REVÊTEMENTS
section: 6
section_title: Espaces simplement connexes
lang: fr
source: ta-i-iv-fr
book_pages: TA I.120-TA I.137, TA I.149-TA I.150
pdf_pages: 0136-0153, 0165-0166
extraction: native
subsections:
    - "no": 1
      title: Revêtement universel
      page: 120
      pdf_page: 136
    - "no": 2
      title: Parties convexes d’un espace numérique
      page: 122
      pdf_page: 138
    - "no": 3
      title: Espaces simplement connexes
      page: 124
      pdf_page: 140
    - "no": 4
      title: Produit d’un espace par un espace simplement connexe
      page: 129
      pdf_page: 145
    - "no": 5
      title: Groupes d’homéomorphismes des espaces simplement connexes
      page: 133
      pdf_page: 149
statements: 37
exercises: 6
content_sha256: 55a3d9d969cfe0bffca545e5628334848137b5a6db2aaf667e32616875d4bf8b
---

## § 6. ESPACES SIMPLEMENT CONNEXES

### 1. Revêtement universel

#### Définition 1 {#ta-i-s6-def-1 .statement tag=01RR}

On appelle ensemble pointé un ensemble X muni de l’un de ses éléments, appelé point-base. L’ensemble X muni du point $x$ est parfois noté $(X, x)$. Soient $(X, x)$ et $(Y, y)$ des ensembles pointés ; on appelle application pointée de $(X, x)$ dans $(Y, y)$ une application $f$ de X dans Y telle que $f(x) =y$.

On définit de façon analogue les notions d’espace topologique pointé, d’application continue pointée, de revêtement pointé d’un espace topologique pointé, etc.

Si $(X, x)$ et $(Y, y)$ sont des espaces topologiques pointés, l’ensemble des applications continues pointées de $(X, x)$ dans $(Y, y)$ est noté $\mathscr{C}((X, x); (Y, y))$.

Au lieu de dire « soit $f$ une application pointée de $(X, x)$ dans $(Y, y)$ », on emploie souvent la phrase suivante : « soit $f: (X, x)\rightarrow (Y, y)$ une application pointée ».

Soit B un espace topologique et soit $b$ un point de B.

#### Définition 2 {#ta-i-s6-def-2 .statement tag=01RS}

On dit qu’un revêtement pointé $(E, x)$ de $(B, b)$ est un revêtement universel si, pour tout revêtement pointé $(E', x')$ de $(B, b)$, il existe un unique morphisme de revêtements de B, $f: E\rightarrow E'$, tel que $f(x) =x'$.

Si $(E, x)$ et $(E', x')$ sont des revêtements universels de $(B, b)$, l’unique B-morphisme de $(E, x)$ dans $(E', x')$ est un isomorphisme de B-espaces.

Soit E un revêtement connexe de B et soit $x$ un point de la fibre $E_b$. Supposons que, pour tout revêtement pointé $(E', x')$ de $(B, b)$, il existe un morphisme $f: E\rightarrow E'$ de revêtements de B tel que $f(x) =x'$. Un tel morphisme $f$ est alors unique (I, p. 34, cor. 1 de la prop. 11), donc $(E, x)$ est un revêtement universel de $(B, b)$. *Nous verrons plus loin (I, p. 126, cor. de la prop. 3) que c’est en particulier le cas si tout revêtement de E est trivialisable.*

#### Proposition 1 {#ta-i-s6-prop-1 .statement tag=01RT}

Soit B un espace topologique connexe et localement connexe et soit $b$ un point de B. Soit $(E, x)$ un revêtement universel de $(B, b)$. Alors, E est un revêtement galoisien de B et tout revêtement de B est associable à E.

L’espace E est localement connexe, car B l’est. Soit $E_0$ la composante connexe de $x$ dans E, de sorte que l’espace $(E_0, x)$ est un revêtement pointé de $(B, b)$ (I, p. 80, cor. 1 de la prop. 6). Il existe alors un unique morphisme de revêtements $f: E\rightarrow E_0$ tel que $f(x) =x$. Si $i$ désigne l’injection canonique de $E_0$ dans E, l’application $i\circ f: E\rightarrow E$ est un morphisme de revêtements qui applique $x$ sur $x$, de même que l’application Id$_E$; puisque $(E, x)$ est un revêtement universel de $(B, b)$, on a donc $i\circ f=$ Id$_E$. Cela entraîne que $i$ est surjectif, donc $E_0= E$. Par suite, E est connexe.

Soit $y$ un point de $E_b$ et considérons le revêtement pointé $(E, y)$ de $(B, b)$ ; il existe par hypothèse un unique morphisme de revêtements $f: E\rightarrow E$ tel que $f(x) =y$. L’application $s: E\rightarrow E\times_BE$ définie par $t\mapsto (t, f(t))$ est une section continue de l’application pr$_1: E\times_BE\rightarrow E$. D’après le cor. 4 de I, p. 81, cela démontre que le revêtement $E\times_BE$ de E donné par l’application pr$_1$ est trivialisable. Le revêtement E est donc galoisien (th. 2 de I, p. 102). Il résulte alors de I, p. 112, corollaire de la prop. 10, que tout revêtement de B est associable à E.

#### Corollaire {#ta-i-s6-n1-cor-1 .statement tag=01RU}

Soit B un espace topologique localement connexe. Soit $b$ un point de B et soit $(E, x)$ un revêtement universel de $(B, b)$. Pour un sous-espace A de B, les deux propriétés suivantes sont équivalentes :

(i) Le revêtement E est trivialisable au-dessus de A ;

(ii) Tout revêtement de B est trivialisable au-dessus de A.

La propriété (ii) implique évidemment la propriété (i). La réciproque résulte de ce que tout revêtement de B est associable au revêtement E (I, p. 105, prop. 7).

### 2. Parties convexes d’un espace numérique

Soit E l’espace numérique à $n$ dimensions *(ou, plus généralement, un espace vectoriel topologique sur $\mathbf{R}$)$*$. Pour tout couple $(x, y)$ de points de E, on appelle segment (resp. segment ouvert) d’extrémités $x$ et $y($cf. EVT, II, p. 7) l’ensemble des points de E de la forme $tx+$ $(1-t)y$, pour $t\in [0,1]$ (resp. pour $t\in ]0,1[$). Soit A un sous-ensemble de E. On dit que l’ensemble A est convexe si pour tout couple $(x, y)$ de points de A et tout $t\in \mathbf{I}$, le point $tx+ (1-t)y$ appartient à A.

*Une partie convexe est connexe par arcs.*

#### Lemme 1 {#ta-i-s6-lem-1 .statement tag=01RV}

Soit E l’espace numérique à $n$ dimensions et soit A une partie convexe et compacte de E dont 0 est un point intérieur. Pour tout $x\in E$, notons $p_A(x)$ la borne inférieure dans $\overline{\mathbf{R}}$ de l’ensemble des nombres réels $t >0$ tels que $x\in tA$.

L’application $p_A$ est finie, continue, et vérifie les propriétés suivantes :

(i) Pour tout $x\in E$ tel que $x= 0\not$ , on a $p_A(x)>0$ ;

(ii) Pour tout $s\in \mathbf{R}_+$ et tout $x\in E$, on a $p_A(sx) =sp_A(x)$.

(iii) Pour tous $x$ et $y\in E$, on a $p_A(x+y)\leqslant p_A(x) +p_A(y)$.

(iv) Pour qu’un point $x$ de E appartienne à A, il faut et il suffit que $p_A(x)\leqslant 1$.

Pour $x\in E$, notons $\|x\|$ la norme euclidienne de $x$ (TG, VI, p. 7). Comme A est compact, il existe un nombre réel $M>0$ tel que tout point $x$ de A vérifie $\|x\|\leqslant M$. Comme 0 est un point intérieur de A, il existe un nombre réel $m >0$ tel que tout point $x$ de E tel que $\|x\|\leqslant m$ appartienne à A. Par suite, on a la relation $\|x\|/M\leqslant p_A(x)\leqslant \|x\|/m$, pour tout $x\in E$. En particulier, $p_A(0) = 0$ et $p_A(x)= 0\not$ si $x= 0\not$ .

Les assertions (ii) et (iv) résultent immédiatement de la définition de l’application $p_A$.

Soient $x$ et $y$ des points de E. Soient $x'$ et $y'$ des points de A tels que $x=p_A(x)x'$ et $y=p_A(y)y'$. Si $x$ et $y$ ne sont pas tous deux nuls, $p_A(x) +p_A(y)>0$ et l’on a

$$
x+y=p_A(x)x'+p_A(y)y'
$$

$$
= (p_A(x) +p_A(y))(\frac{p_A(x)}{p_A(x) + p_A(y)}x'+\frac{p_A(y)}{p_A(x) + p_A(y)}y')
$$

Comme A est convexe, cela démontre que $x+y$ appartient à $(p_A(x) +$ $p_A(y))A$, d’où $p_A(x+y)\leqslant p_A(x) +p_A(y)$. Si $x=y= 0$, cette inégalité est encore vérifiée, car $p_A(0) = 0$. Cela démontre l’assertion (iii).

Appliquant cette inégalité à $x+y$ et $-y$, on en déduit que, pour tout couple $(x, y)$ de points de E, on a

$|p_A(x+y)-p_A(x)|\leqslant$ max($p_A(y), p_A(-y)$)$\leqslant m^{-1}\|y\|$.

Cela démontre que l’application $p_A$ est continue, d’où le lemme.

L’application $p_A$ est appelée jauge de la partie convexe A.

#### Proposition 2 {#ta-i-s6-prop-2 .statement tag=01RW}

Soit E l’espace numérique à $n$ dimensions et soit A une partie convexe et compacte de E dont 0 est un point intérieur. Il existe une unique bijection $u$ de E sur lui-même vérifiant les trois propriétés suivantes :

(i) Pour tout $x\in E$ et tout $t\in \mathbf{R}_+,u(tx) =tu(x)$ ;

(ii) Pour tout $x\in E$, il existe $\lambda \in \mathbf{R}_+$ tel que $u(x) =\lambda x$;

(iii) On a $u(A) =\mathbf{B}_n$.

L’application $u$ est un homéomorphisme et induit, par passage aux sous-espaces, un homéomorphisme de A sur $\mathbf{B}_n$, un homéomorphisme de l’intérieur de A sur l’intérieur de $\mathbf{B}_n$ et un homéomorphisme de la frontière de A dans E sur la sphère $\mathbf{S}_{n-1}$.

Soit $p_A$ la jauge de la partie convexe A. Soit $x\in E$ et soit $t\in \mathbf{R}_+$; pour que $x\in tA$, il faut et il suffit que $p_A(x)\leqslant t$. Comme A est compacte, il existe un nombre réel M tel que $\|x\|\leqslant M$ pour tout $x\in A$.

Soit $u$ une application vérifiant les conditions de la proposition. On a $u(0) = 0$. Soit $x\in E-\{0\}$ et soit $\lambda \in \mathbf{R}_+$ tel que $u(x) =\lambda x$. Pour tout $t\in \mathbf{R}_+$ tel que $tx\in A$, on a $u(tx) =t\lambda x$. Comme $u$ est injective, $\lambda = 0\not$ . Comme $u(A)$ est contenu dans $\mathbf{B}_n$, on a aussi $\lambda \leqslant p_A(x)/\|x\|$. Posons $z=x/\|x\|$; c’est un point de $\mathbf{S}_{n-1}$. Pour que $z$ possède un antécédent dans A par $u$, il faut et il suffit que le point $(\lambda \|x\|)^{-1}x$ appartienne à A, c’est-à-dire $\lambda \|x\|\geqslant p_A(x)$, i.e. $\lambda \geqslant p_A(x)/\|x\|$. Cela implique l’unicité d’une telle application $u$.

Notons alors $u$ l’application de E dans lui-même qui applique 0 sur 0 et $x$ sur $(p_A(x)/\|x\|)x$, pour tout $x\in E-\{0\}$.

D’après le lemme $1,u$ est continue en tout point de E $-\{0\}$. On a $\|u(x)\|=p_A(x)$ pour tout $x\in E$ et $p_A(x)\rightarrow 0$ lorsque $x\rightarrow 0$ (loc. cit.) ; par conséquent, $u$ est continue en 0. Par suite, $u$ est continue.

Le seul antécédent de 0 par $u$ est 0. Soit $y\in E-\{0\}$. Pour qu’un élément $x$ de E vérifie $u(x) =y$, il faut et il suffit que $x= (\|y\|/p_A(y))y$. Cela entraîne que $u$ est une bijection continue de E sur lui-même. Sa réciproque est l’application $v:y\mapsto (\|y\|/p_A(y))y$. Comme $p_A$ est continue et ne s’annule qu’en 0, l’application $v$ est continue en tout point de E $-\{0\}$; l’inégalité $p_A(y)\geqslant \|y\|/M$ entraîne que $\|v(y)\|\leqslant M\|y\|$ pour tout $y\in E$. Il s’ensuit que $v$ est continue. Par suite, l’application $u$ est un homéomorphisme de E sur lui-même. Comme les relations $p_A(x)\leqslant 1$ et $x\in A$ sont équivalentes, on a aussi $u(X) =\mathbf{B}_n$. La proposition en résulte.

#### Exemple {#ta-i-s6-n2-exa-1 .statement tag=01RX}

L’ensemble $[0,1]^n$ est une partie convexe, compacte et d’intérieur non vide de $\mathbf{R}^n$. Il résulte de la proposition 2 de I, p. 123 qu’il est homéomorphe à la boule euclidienne fermée. Plus précisément, pour tout point $x$ de l’intérieur $]0,1[^n$ et tout point $b$ de la boule euclidienne ouverte, il existe un homéomorphisme de $[0,1]^n$ sur $\mathbf{B}_n$ qui applique $x$ sur $b$ et induit par passage aux sous-espaces un homéomorphisme de $]0,1[^n$ sur la boule euclidienne ouverte, ainsi qu’un homéomorphisme de la frontière de $[0,1]^n$ sur la sphère $\mathbf{S}_{n-1}$.

Par suite, toute partie convexe, compacte et d’intérieur non vide de $\mathbf{R}^n$ est homéomorphe à un pavé (loc. cit.).

### 3. Espaces simplement connexes

#### Définition 3 {#ta-i-s6-def-3 .statement tag=01RY}

On dit qu’un espace topologique est simplement connexe si tous ses revêtements sont trivialisables.

Un espace simplement connexe est connexe. En effet, si un espace X est réunion disjointe de deux ouverts non vides U et V, l’injection canonique de U dans X est un revêtement qui n’est pas trivialisable.

L’espace vide est simplement connexe. Tout espace topologique réduit à un point est simplement connexe.

#### Remarque 1 {#ta-i-s6-n3-rem-1 .statement tag=01RZ}

Soient B un espace topologique simplement connexe et $(E, p)$ un revêtement de B. Si l’espace E est connexe et non vide, l’application $p$ est un homéomorphisme. Soient, par exemple, G un groupe topologique connexe et H un sous-groupe discret de G, de sorte que l’application canonique $p: G\rightarrow G/H$ fait de G un revêtement de $G/H$ (I, p. 100, cor. 2 du th. 1). Si l’espace $G/H$ est simplement connexe, l’application $p$ est un homéomorphisme et H est le sous-groupe à un élément.

#### Remarque 2 {#ta-i-s6-n3-rem-2 .statement tag=01S0}

Soit B un espace topologique dont tout point possède un voisinage simplement connexe ; alors tout revêtement d’un revêtement de B est un revêtement de B. Considérons en effet un revêtement $(E, p)$ de B ainsi qu’un revêtement $(F, q)$ de E. Démontrons que $(F, p\circ q)$ est un revêtement de B. La question étant locale dans B, nous pouvons supposer que l’espace B est simplement connexe et donc que E est un revêtement trivialisable de B. Soit V une composante connexe de E. Elle est ouverte et fermée et $p|V: V\rightarrow B$ est un homéomorphisme (I, p. 69, proposition 1) ; par suite, l’espace V est simplement connexe. Toute composante connexe W de $\overset{-1}{q}(V)$ est ouverte et fermée dans $\overset{-1}{q}(V)$, donc dans F et l’application $q$ induit un homéomorphisme de W sur V. L’application $p\circ q$ fait donc de F un revêtement de B, trivialisable (loc. cit.).

#### Proposition 3 {#ta-i-s6-prop-3 .statement tag=01S1}

Soit B un espace topologique. Soit $(E, p)$ un revêtement de B et soit $y$ un point de E. Soit X un espace topologique simplement connexe, soient $f: X\rightarrow B$ une application continue et $x$ un point de X tels que $f(x) =p(y)$. Il existe un unique relèvement continu $g: X\rightarrow E$ de l’application $f$ tel que $g(x) =y$.

Les applications $g$ cherchées correspondent bijectivement (I, p. 9, prop. 3) aux sections continues $s$ du revêtement pr$_1: X\times_BE\rightarrow X$ telles que $s(x) = (x, y)$. Une telle section existe car l’espace X est simplement connexe ; elle est unique car l’espace X est connexe (I, p. 34, cor. 1 de la prop. 11).

#### Exemple 1 {#ta-i-s6-n3-exa-1 .statement tag=01S2}

Soit X un espace topologique simplement connexe et soit $f$ une fonction continue de X dans $\mathbf{C}^*$. Rappelons (I, p. 101, exemple 6) que l’application $z\mapsto e^z$ fait de $\mathbf{C}$ un revêtement de $\mathbf{C}^*$. D’après la prop. 3, il existe une fonction continue $h: X\rightarrow \mathbf{C}$ telle que $f(x) =e^{h(x)}$ pour tout $x\in X$. Si $h': X\rightarrow \mathbf{C}$ est une autre fonction continue telle que $f(x) =e^{h'(x)}$ pour tout $x\in X$, il existe un entier $q\in \mathbf{Z}$ tel que $h'=h+ 2\pi iq$.

De même, soit $n$ un entier $>0$ ; l’application $z\mapsto z^n$ fait de $\mathbf{C}^*$ un revêtement de lui-même (I, p. 101, exemple 5). Il existe donc une fonction continue $k$ de X dans $\mathbf{C}^*$ telle que $k(x)^n=f(x)$ pour tout $x\in X$, par exemple la fonction $k(x) =e^{h(x)/n}$. Si $k': X\rightarrow \mathbf{C}^*$ est une autre fonction continue telle que $k'(x)^n=f(x)$ pour tout $x\in X$, il existe une racine $n^e$ de l’unité $\mu\in \mathbf{C}$ telle que $k'=\mu k$.

#### Corollaire {#ta-i-s6-n3-cor-1 .statement tag=01S3}

Soit B un espace topologique et soit $b$ un point de B. Soit E un revêtement simplement connexe de B. Pour tout point $x$ de $E_b$, l’espace pointé $(E, x)$ est un revêtement universel de $(B, b)$.

#### Proposition 4 {#ta-i-s6-prop-4 .statement tag=01S4}

Le produit de deux espaces simplement connexes dont l’un est localement connexe est un espace simplement connexe.

Soient X et Y des espaces simplement connexes et supposons que Y soit localement connexe. L’espace $X\times Y$ est connexe, car X et Y le sont (I, p. 124). Soit $(Z, f)$ un revêtement non vide de $X\times Y$ ; démontrons qu’il est trivialisable. D’après le corollaire 2 de I, p. 70, il suffit de démontrer que pour tout point $z_0$ de Z, il existe une section continue $s$ de $f$ telle que $s(f(z_0)) =z_0$. Soit donc $z_0$ un point de Z. Posons $(x_0, y_0) =f(z_0)$. Le sous-espace $X\times  \{y_0\}$ de $X\times Y$ est homéomorphe à X. Par suite, le revêtement déduit de Z au-dessus de $X\times  \{y_0\}$ est trivialisable et possède une section continue $\sigma$ telle que $\sigma (x_0, y_0) =z_0$. De même, pour tout point $x$ de X, il existe une section continue $\tau_x$ de $f$ au-dessus de $\{x\}\times Y$ telle que $\tau_x(x, y_0) =\sigma (x, y_0)$. Pour $(x, y)\in X\times Y$, posons $s(x, y) =\tau_x(x, y)$. L’application $s$ est une section de $f$ et l’on a $s(x_0, y_0) =z_0$. Comme l’espace Y est connexe et localement connexe, il résulte du th. 1 de I, p. 35 que l’application $s$ est continue.

#### Proposition 5 {#ta-i-s6-prop-5 .statement tag=01S5}

Un espace topologique connexe et localement connexe, tel que l’intersection de deux parties ouvertes connexes quelconques soit connexe, est un espace simplement connexe.

Soit B un tel espace topologique. Soit $(E, p)$ un revêtement de B, soit $x$ un point de E et notons $b=p(x)$. Il s’agit de démontrer qu’il existe une section continue $s$ de $p$ telle que $s(b) =x$ (cor. 2, I, p. 70). Soit $\mathscr{S}$ l’ensemble des couples $(U, s_U)$ où U est une partie ouverte connexe de B contenant $b$ et $s_U$ une section continue de $p_U:\overset{-1}{p}(U)\rightarrow U$ telle que $s_U(b) =x$. L’ensemble $\mathscr{S}$ n’est pas vide ( I, p. 34, prop. 10). Soient $(U, s_U)$ et $(V, s_V)$ des éléments de $\mathscr{S}$. Alors, $s_U|U\cap V$ et $s_V|U\cap V$ sont des sections continues de $p_{U\cap V}$ qui prennent la valeur $x$ en $b$. Par hypothèse, $U\cap V$ est connexe ; on a donc $s_U|U\cap V =s_V|U\cap V$ (I, p. 34, cor. 1 de la prop. 11). Soit A la réunion des ouverts U lorsque $(U, s_U)$ parcourt $\mathscr{S}$ et soit $s: A\rightarrow E$ l’unique application telle que $s|U =s_U$ pour tout couple $(U, s_U)\in \mathscr{S}$. L’ensemble A est ouvert et connexe (TG, I, p. 81, prop. 2), il contient $b$, et $s$ est une section continue de $p_A$ telle que $s(b) =x$. Il suffit maintenant de démontrer que l’ensemble A est fermé, ce qui entraînera qu’il est égal à B.

Soit $a$ un point de B adhérent à A et soit V un voisinage ouvert connexe de $a$ tel que le revêtement E soit trivialisable au-dessus de V. Il existe un point $c$ dans $A\cap V$ et une section continue $s_V$ de $p_V$ telle que $s_V(c) =s(c)$. Soit $A'$ l’ouvert $A\cup V$. Comme $A\cap V$ est connexe, il existe une section continue $s'$ de $p_{A'}$ qui prolonge $s$ et $s_V($I, p. 35, cor. 3 de la prop. 11) ; le couple $(A', s')$ appartient à $\mathscr{S}$ et $A'$ est donc contenu dans A. Par suite, $a$ appartient à A et A est fermé.

#### Corollaire {#ta-i-s6-n3-cor-2 .statement tag=01S6}

Tout intervalle de la droite réelle $\mathbf{R}$ est simplement connexe.

En effet, les sous-espaces connexes de $\mathbf{R}$ sont les intervalles (TG, IV, p. 8, th. 4) et l’intersection de deux intervalles est un intervalle.

#### Exemple 2 {#ta-i-s6-n3-exa-2 .statement tag=01S7}

L’espace numérique à $n$ dimensions $\mathbf{R}^n$ (TG, VI, p. 1) est simplement connexe. Il est en effet produit d’espaces simplement connexes et localement connexes (I, p. 126, prop. 4 et cor. de la prop. 5 ci-dessus). Il en est de même de tout pavé ouvert ou fermé de $\mathbf{R}^n$. Un parallélotope, une boule euclidienne, ouvert ou fermé, dans $\mathbf{R}^n$ sont simplement connexes car homéomorphes à un pavé (TG, VI, p. 10, prop. 2 et I, p. 124, exemple).

#### Proposition 6 {#ta-i-s6-prop-6 .statement tag=01S8}

Soit X un espace topologique. Soient $U_1$ et $U_2$ des sous-espaces ouverts ( resp. fermés) de X tels que $X = U_1\cup U_2$. Supposons que $U_1$ et $U_2$ soient simplement connexes et que leur intersection $U_1\cap U_2$ soit connexe et non vide. Alors, l’espace X est simplement connexe.

Soit $(E, p)$ un revêtement de X et soit $y$ un point de E. Il suffit de démontrer qu’il existe une section continue $s$ de $p$ telle que $s(p(y)) =y$ (I, p. 70, cor. 2 de la prop. 1). Supposons par exemple que $p(y)$ appartienne à $U_1$. Il existe alors une section continue $s_1: U_1\rightarrow E$ de $p_{U_1}$ telle que $s_1(p(y)) =y$. Soit $x$ un point de $U_1\cap U_2$; il existe une section continue $s_2$ de $p_{U_2}$ telle que $s_2(x) =s_1(x)$. D’après le corollaire 3 de la proposition 11 de I, p. 34, il existe une section continue $s$ de $p$ prolongeant à la fois $s_1$ et $s_2$.

#### Exemple 3 {#ta-i-s6-n3-exa-3 .statement tag=01S9}

Pour $n\geqslant 2$, la sphère $\mathbf{S}_n$ (TG, VI, p. 10) est simplement connexe. En effet, la sphère $\mathbf{S}_n$ est réunion de deux hémisphères fermés homéomorphes à $\mathbf{B}_n$ dont l’intersection est homéomorphe à $\mathbf{S}_{n-1}($cf. TG, VI, p. 12). Pour $n\geqslant 2$, la sphère $\mathbf{S}_{n-1}$ est connexe, d’où l’assertion.

En revanche, le cercle $\mathbf{S}_1$ n’est pas simplement connexe. En effet, l’application continue $p:\mathbf{R}\rightarrow \mathbf{S}_1$ définie par $p(\theta ) =$ (cos $\theta$, sin $\theta$ ) fait de $\mathbf{R}$ un revêtement de degré infini de $\mathbf{S}_1$, connexe, donc qui n’est pas trivialisable.

#### Exemple 4 {#ta-i-s6-n3-exa-4 .statement tag=01SA}

Soit E un espace vectoriel de dimension finie $n$ sur $\mathbf{R}$ et soit F un sous-espace affine de E de codimension $p\geqslant 3$. L’ensemble $\mathbf{R}^p-\{0\}$ est homéomorphe à $\mathbf{R}\times \mathbf{S}_{p-1}$ (TG, VI, p. 10, cor. 2), donc est simplement connexe, puisque $\mathbf{R}$ et $\mathbf{S}_{p-1}$ sont localement connexes et simplement connexes (I, p. 126, prop. 4). L’ensemble E-F, homéomorphe à $\mathbf{R}^{n-p}\times$ $(\mathbf{R}^p-\{0\})$, est donc simplement connexe (loc. cit.).

#### Proposition 7 {#ta-i-s6-prop-7 .statement tag=01SB}

Soit X un espace topologique. Soient $U_1$ et $U_2$ des sous-espaces ouverts ( resp. fermés) connexes de X tels que $X = U_1\cup$ $U_2$. Si l’espace X est simplement connexe, alors $U_1\cap U_2$ est connexe.

Posons $U = U_1\cap U_2$ et supposons par l’absurde que l’espace U ne soit pas connexe. Nous allons construire un revêtement connexe de X de degré infini ; un tel revêtement n’est pas trivialisable.

Par hypothèse, l’ensemble U est la réunion de deux ensembles A et B disjoints, non vides et ouverts (resp. fermés) dans X. Pour $i\in  \{1,2\}$, soit $Y_i$ le $U_i$-espace $(U_i\times \mathbf{Z}$, pr$_1)$ et soit $Z_i$ le sous-espace $U\times \mathbf{Z}$ de $Y_i$. L’application $h: Z_1\rightarrow Z_2$ définie par

$(x, n)$ si $x\in A$ et $n\in \mathbf{Z}$

$$
h(x, n) =
$$

$(x, n+ 1)$ si $x\in B$ et $n\in \mathbf{Z}$

est un homéomorphisme. Soit Y l’espace obtenu par recollement de $Y_1$ et $Y_2$ le long de $Z_1$ et $Z_2$ au moyen de l’homéomorphisme $h$ (TG, I, p. 17).

Pour $i\in  \{1,2\}$, l’application canonique $g_i$ de $Y_i$ dans Y est un homéomorphisme de $Y_i$ sur une partie ouverte (resp. fermée) de Y (loc. cit., prop. 9). Pour tout entier $n\in \mathbf{Z}$, les ensembles $g_i(U_i\times  \{n\})$, $i\in  \{1,2\}$, sont connexes ; comme A et B ne sont pas vides, $g_1(U_1\times \{n\})$ rencontre $g_2(U_2\times  \{n\})$ et $g_2(U_2\times  \{n+1\})$. Il en résulte que l’espace Y est connexe (TG, I, p. 81, corollaire).

Pour $x\in U$ et $n\in \mathbf{Z}$, on a (pr$_1\circ h$)$(x, n) =x=$ pr$_1(x, n)$. Il existe donc une unique application continue $p: Y\rightarrow X$ telle que $p\circ g_i=$ pr$_1$ pour $i\in  \{1,2\}$. Démontrons que le X-espace $(Y, p)$ est un revêtement. Par construction, les fibres de l’application $p$ sont homéomorphes à l’espace discret $\mathbf{Z}$.

Pour $i\in  \{1,2\}$, l’application $g_i$ définit par passage aux sous-espaces un isomorphisme de $U_i$-espaces de $U_i\times \mathbf{Z}$ sur $\overset{-1}{p}(U_i)$.

Par définition de l’espace Y, il existe une unique application $k$ de $(X-A)\times \mathbf{Z}$ dans Y telle que $k(x, n) =g_1(x, n)$ pour $x\in (U_1-A)\times \mathbf{Z}$ et $k(x, n) =g_2(x, n-1)$ pour $x\in (U_2-A)\times \mathbf{Z}$; c’est un isomorphisme de (X-A)-espaces de $(X-A)\times \mathbf{Z}$ sur $\overset{-1}{p}(X-A)$. De même, il existe une unique application $k'$ de $(X-B)\times \mathbf{Z}$ dans Y qui coïncide avec $g_1$ dans $(U_1-B)\times \mathbf{Z}$ et avec $g_2$ dans $(U_2-B)\times \mathbf{Z}$ et c’est un isomorphisme de (X-B)-espaces de $(X-B)\times \mathbf{Z}$ sur $\overset{-1}{p}(X-B)$.

Cela démontre que le X-espace $(Y, p)$ est trivialisable au-dessus des parties $U_1,U_2$, X-A et X-B. On a $U_1\cup U_2= X$; si $U_1$ et $U_2$ sont ouverts dans X, cela démontre que $(Y, p)$ est un revêtement de X. Il en est de même lorsque $U_1$ et $U_2$ sont fermés dans X car alors, X-A et X-B sont des ouverts de X dont la réunion est X. La proposition est ainsi démontrée.

#### Corollaire {#ta-i-s6-n3-cor-3 .statement tag=01SC}

Soit X un espace topologique simplement connexe et soit A une partie connexe de X. Si le complémentaire de A est connexe, sa frontière l’est aussi.

Soient $X_1$ et $X_2$ les adhérences de A et de X-A respectivement. Les ensembles $X_1$ et $X_2$ sont fermés et connexes (TG, I, p. 81, prop. 1) ; on a $X_1\cup X_2= X$ et leur intersection $X_1\cap X_2$ est égale à la frontière de A. Il suffit alors d’appliquer la proposition 7.

### 4. Produit d’un espace par un espace simplement connexe

#### Proposition 8 {#ta-i-s6-prop-8 .statement tag=01SD}

Soit B un espace topologique. Soit T un espace simplement connexe et localement connexe. Soit E un revêtement de $B\times T$, de projection $p$, et soit $t$ un point de T. Notons $E_t$ l’espace $\overset{-1}{p}(B\times  \{t\})$ ; muni de l’application $p_t=$ pr$_1\circ p|E_t: E_t\rightarrow B$, c’est un revêtement de B. Il existe alors un unique $(B\times T)$-isomorphisme du revêtement $(E_t\times T, p_t\times$ Id$_T)$ sur le revêtement E qui applique $(x, t)$ sur $x$ pour tout $x\in E_t$.

On peut supposer que B n’est pas vide. Soit $x$ un point de $E_t$. D’après la proposition 3 de I, p. 125 appliquée au revêtement E et à l’application continue $T\rightarrow B\times T,u\mapsto (p_t(x), u)$, il existe une unique application continue $f_x: T\rightarrow E$ telle que $f_x(t) =x$ et $p(f_x(u)) =$ $(p_t(x), u)$ pour tout $u\in T$. Soit $h: E_t\times T\rightarrow E$ l’application définie par $h(x, u) =f_x(u)$. On a $h(x, t) =x$ et $p\circ h=p_t\times$ Id$_T$. L’application $h$ est un relèvement à E de l’application $p_t\times$ Id$_T$. La restriction de $h$ à $E_t\times  \{t\}$ est continue, de même que la restriction de $h$ à $\{x\} \times T$ pour tout point $x$ de $E_t$. Comme l’espace T est localement connexe, l’application $h$ est continue ( I, p. 37, cor. 1 du th. 1).

Soit $b$ un point de B. Par construction, l’application $h$ induit une bijection de la fibre $\overset{-1}{p_{t}}(b)\times  \{t\}$ de $E_t\times T$ sur la fibre $\overset{-1}{p}(b, t)$ de E en $(b, t)$. Comme l’espace T est connexe et localement connexe, l’application $h$ est bijective (I, p. 84, cor. de la prop. 7). C’est donc un $B\times T$-isomorphisme (I, p. 30, cor. 2 de la prop. 6).

Soit $h'$ un $(B\times T)$-isomorphisme du revêtement $(E_t\times T, p_t\times$ Id$_T)$ sur le revêtement E qui applique $(x, t)$ sur $x$ pour tout point $x\in E_t$. Pour tout $x\in E_t$, les applications $u\mapsto h(x, u)$ et $u\mapsto h'(x, u)$ sont égales (I, p. 34, cor. 1 de la prop. 11). On a donc $h=h'$.

#### Corollaire 1 {#ta-i-s6-prop-8-cor-1 .statement tag=01SE}

Sous les hypothèses de la prop. 8, si $t$ et $t'$ sont deux points de T, les revêtements $E_t$ et $E_{t'}$ sont B-isomorphes.

#### Corollaire 2 {#ta-i-s6-prop-8-cor-2 .statement tag=01SF}

Sous les hypothèses de la prop. 8, soient $(E, p)$ et $(E', p')$ des revêtements de $B\times T$ et soit $k: E_t\rightarrow E'_t$ un B-morphisme. Il existe un unique $(B\times T)$-morphisme $\widetilde{k}: E\rightarrow E'$ qui prolonge $k$. Si $k$ est un B-isomorphisme, $\widetilde{k}$ est un $(B\times T)$-isomorphisme.

D’après la proposition 8, on peut supposer qu’il existe des revêtements F et $F'$ de B tels que E et $E'$ soient respectivement les $(B\times T)$-espaces $F\times T$ et $F'\times T$. On a alors $E_t= F\times  \{t\},E'_t= F'\times  \{t\}$ et l’application $k$ s’écrit $(x, t)\mapsto (k'(x), t)$, où $k'$ est un B-morphisme de F dans $F'$. L’application $k'\times$Id$_T$ est un $B\times T$-morphisme qui prolonge $k$; c’est un isomorphisme si $k$ en est un.

Soit $\widetilde{k}: E\rightarrow E'$ un $(B\times T)$-morphisme qui prolonge $k$. Soit $x$ un point de F. Notons $q$ la projection de F et posons $b=q(x)$. Les applications $u\mapsto \widetilde{k}(x, u)$ et $u\mapsto (k'(x), u)$ sont des relèvements dans $E'$ de l’application $u\mapsto (b, u)$ de T dans $B\times T$. Elles coïncident en $t$. Comme l’espace T est connexe, elles sont égales. Ainsi, $\widetilde{k}$ est le $(B\times T)$-morphisme $k'\times$ Id$_T: F\times T\rightarrow F'\times T$.

#### Corollaire 3 {#ta-i-s6-prop-8-cor-3 .statement tag=01SG}

Soient B et $B'$ des espaces topologiques, soit T un espace topologique simplement connexe et localement connexe. Soit $f: B'\times T\rightarrow B$ une application continue et soit E un revêtement de B. Étant donnés un point $t$ de T et un relèvement continu $g_t: B'\times \{t\} \rightarrow E$ de $f|B'\times  \{t\}$ à E, il existe un unique relèvement continu $g$ de $f$ à E prolongeant $g_t$.

Compte tenu de la prop. 3 de I, p. 9, il s’agit de démontrer que toute section continue de $f^*(E)$ au-dessus de $B'\times  \{t\}$ se prolonge de manière unique en une section continue de $f^*(E)$. Or cela résulte du cor. 2 appliqué aux revêtements $(B'\times T$, Id$_{B'\times T})$ et $f^*E$ de $B'\times T$.

#### Remarque {#ta-i-s6-n4-rem-1 .statement tag=01SH}

Conservons les hypothèses et les notations de la proposition 8. Soit G un groupe topologique discret. Supposons que E soit un revêtement principal de groupe G. Si l’on munit les revêtements $E_t$ de B et $E_t\times T$ de $B\times T$ des structures de revêtement principal de groupe G déduites de celle de E (I, p. 92, exemples 1 et 4), alors les revêtements E et $E_t\times T$ sont des revêtements principaux isomorphes. Soit en effet $h: E_t\times T\rightarrow E$ l’unique $(B\times T)$-morphisme tel que $h(x, t) =x$ pour tout $x\in E_t$. Pour tout élément $g$ de G, l’application $(x, u)\mapsto h(x\cdot g, u)\cdot g^{-1}$ est un $(B\times T)$-morphisme qui applique $(x, t)$ sur $x$ pour tout $x\in E_t$, donc est égal à $h$. Cela prouve que $h$ est un $(B\times T)$-morphisme de revêtements principaux.

En particulier, sous les hypothèses précédentes, les revêtements principaux $E_t$ et $E_{t'}$ sont isomorphes, pour $t'\in T$. On démontre de même que si, dans le corollaire 2, E et $E'$ sont des revêtements principaux de groupe G et si $k$ est un B-isomorphisme de revêtements principaux de groupe G$,\widetilde{k}$ est un $(B\times T)$-isomorphisme de revêtements principaux.

#### Proposition 9 {#ta-i-s6-prop-9 .statement tag=01SI}

Soit B un espace topologique et soit $(E, p)$ un revêtement de B. Soit T un espace topologique simplement connexe, localement connexe et localement compact. Notons $\widetilde{p}:\mathscr{C}_c(T; E)\rightarrow \mathscr{C}_c(T; B)$ l’application $g\mapsto p\circ g$. Soit $t$ un point de T. Notons $e_E:\mathscr{C}_c(T; E)\rightarrow E$ l’application qui à $g\in \mathscr{C}_c(T; E)$ associe $g(t)$, et $e_B:\mathscr{C}_c(T; B)\rightarrow B$ l’application qui à $f\in \mathscr{C}_c(T; B)$ associe $f(t)$.

Le carré

$\mathscr{C}_c(T; E)^{e_E}$ E

$\widetilde{p}p$

$\mathscr{C}_c(T; B)^{e_B}$ B est cartésien.

Démontrons au préalable un lemme.

#### Lemme {#ta-i-s6-n4-lem-1 .statement tag=01SJ}

Soient X, Y, Z des espaces topologiques et soit $g: Y\rightarrow Z$ une application continue.

a) L’application $f\mapsto g\circ f$ de $\mathscr{C}_c(X; Y)$ dans $\mathscr{C}_c(X; Z)$ est continue.

b) Si l’espace topologique Z est séparé, l’application $h\mapsto h\circ g$ de $\mathscr{C}_c(Z; X)$ dans $\mathscr{C}_c(Y; X)$ est continue.

Étant données une partie compacte K de X, une partie ouverte U de Z et une application continue $f$ de X dans Y, pour que l’on ait $(g\circ f)(K)\subset U$, il faut et il suffit que l’on ait $f(K)\subset \overset{-1}{g}(U)$. La première assertion résulte donc de la définition de la topologie de la convergence compacte (TG, X, p. 26, déf. 1).

De même, soient K une partie compacte de Y et U une partie ouverte de X. Comme l’espace Z est supposé séparé, l’ensemble $g(K)$ est compact (TG, I, p. 63, cor. 1). Si $h$ est une application de Z dans X, la condition $(h\circ g)(K)\subset U$ n’est autre que la condition $h(g(K))\subset U$, d’où la deuxième assertion.

Démontrons maintenant la proposition 9. D’après le lemme, l’application $\widetilde{p}$ est continue ; d’après la remarque 1 de TG, X, p. 27, les applications $e_E$ et $e_B$ sont continues. Pour toute application $g\in \mathscr{C}_c(T; E)$, on a

$$
(p\circ e_E)(g) =p(g(t)) = (p\circ g)(t) =\widetilde{p}(g)(t) = (e_B\circ \widetilde{p})(g)
$$

si bien que le diagramme carré de la proposition est commutatif.

Soit $\varphi :\mathscr{C}_c(T; E)\rightarrow \mathscr{C}_c(T; B)\times_BE$ l’application continue définie par $\varphi (g) = (p\circ g, g(t))$ pour tout $g\in \mathscr{C}_c(T; E)$. D’après la proposition 3 de I, p. 125, elle est bijective. En effet, pour tout couple $(f, x)\in \mathscr{C}_c(T; B)\times_BE,\varphi^{-1}(f, x)$ est l’unique relèvement continu $g$ de $f$ à E tel que $g(t) =x$. Comme l’espace T est localement compact, l’application $\psi : (\mathscr{C}_c(T; B)\times_BE)\times T\rightarrow B$ définie par $\psi ((f, x), u) =f(u)$ est continue (TG, X, p. 28, cor. 1). D’après le corollaire 3 ci-dessus, l’application $\psi$ possède un unique relèvement continu $\theta : (\mathscr{C}_c(T; B)\times_B$ $E)\times T\rightarrow E$ tel que $\theta ((f, x), t) =x$ pour $(f, x)\in \mathscr{C}_c(T; B)\times_BE$. On a ainsi $\theta ((f, x), u) =\varphi^{-1}(f, x)(u)$ pour $(f, x)\in \mathscr{C}_c(T; B)\times_BE$ et $u\in T$. D’après le théorème 3 de TG, X, p. 28, l’application $(f, x)\mapsto \theta ((f, x),\cdot )$ de $\mathscr{C}_c(T; B)\times_BE$ dans $\mathscr{C}_c(T; E)$ est continue, c’est-à-dire $\varphi^{-1}$ est continue.

Ainsi, l’application $\varphi$ est un homéomorphisme de $\mathscr{C}_c(T; E)$ sur le produit fibré $\mathscr{C}_c(T; B)\times_BE$, d’où la proposition (I, p. 8, prop. 2).

### 5. Groupes d’homéomorphismes des espaces simplement connexes

Soit X un espace topologique connexe non vide et soit G un groupe discret opérant continûment à gauche dans X ; notons $e$ l’élément neutre de G. Soit M une partie de X telle que $G\cdot M = X$. On pose

$$
S =\{g\in G|g\cdot M\cap M=\not\emptyset \}
$$

On a $e\in S$ et $S = S^{-1}$.

Pour tout $x\in X$, notons $E_x$ l’ensemble des $g\in G$ tels que $x\in g\cdot M$. Soient $g, h\in E_x$; alors $g\cdot M\cap h\cdot M=\not\emptyset$, si bien que $g^{-1}h\in S$. En particulier, pour tout $x\in M$, on a $e\in E_x$ d’où $E_x\subset S$.

On fait l’une des deux hypothèses suivantes :

(i) L’ensemble M est ouvert ;

(ii) L’ensemble M est fermé et le recouvrement $(g\cdot M)_{g\in G}$ de X est localement fini.

#### Lemme 2 {#ta-i-s6-lem-2 .statement tag=01SK}

Pour tout point $x\in X$, l’application $\mu_x: E_x\times M\rightarrow X$ donnée par $(g, u)\mapsto g\cdot u$ est universellement stricte, et son image $E_x\cdot M$ est un voisinage de $x$ dans X. En particulier, $S\cdot M$ est un voisinage de M.

Sous l’hypothèse (i), l’application $\mu_x$ est ouverte, car $E_x\times M$ est ouvert dans $G\times M$. Son image est alors ouverte dans X.

Supposons maintenant l’hypothèse (ii) satisfaite. L’application $\mu_x$ est propre (TG, I, p. 6, prop. 4, et p. 75, th. 1), donc universellement stricte (I, p. 20, corollaire 11). En outre, $(G-E_x)\cdot M$ est une partie fermée de X qui ne contient pas $x$, si bien que $E_x\cdot M$ est un voisinage de $x$.

La dernière assertion résulte de ce que $E_x\subset S$ si $x\in M$.

#### Lemme 3 {#ta-i-s6-lem-3 .statement tag=01SL}

Le groupe G est engendré par S.

Soit H le sous-groupe de G engendré par S. Soit $U = H\cdot M$ ; observons que U est la réunion des parties de la forme $h\cdot (S\cdot M)$, pour $h\in H$. Comme $S\cdot M$ est un voisinage de M (lemme 2), l’ensemble U est un voisinage de $H\cdot M = U$ ; il en résulte que U est ouvert dans X. Soient $g, g'\in G$ tels que $g\cdot U\cap g'\cdot U=\not\emptyset$; soient $h, h'\in H$ et $x, x'\in M$ tels que $gh\cdot x=g'h'\cdot x'$; alors $h^{-1}g^{-1}g'h'\cdot x'=x$, si bien que $h^{-1}g^{-1}g'h'\in S$ ; en particulier, $g^{-1}g'\in H$. Lorsque $g$ parcourt un système de représentants des classes à gauche modulo H, les ensembles $g\cdot U$ sont ainsi deux à deux disjoints ; puisque $G\cdot M = X$, ils recouvrent X. Comme X est connexe, il s’ensuit que (G : H) = 1, d’où H = G.

Soit T l’ensemble des couples $(s, t)$ d’éléments de G tels que $M\cap s\cdot$ $M\cap st\cdot M=\not\emptyset$; si $(s, t)\in T$, alors $s,t$ et $st$ appartiennent à S. Soit F le groupe $F(S,\mathbf{r})$ défini par l’ensemble générateur S et par l’ensemble $\mathbf{r}$ des relateurs $str^{-1}$ pour $r, s, t\in S$ tels que $(s, t)\in T$ et $r=st$; notons $\varepsilon$ son élément neutre et $\varphi : F\rightarrow G$ l’homomorphisme canonique (A, I, p. 86, prop. 9). Si $s\in S$, nous noterons $x_s$ l’élément de F, image de $s$ par l’application canonique de S dans F; pour tout $s\in S$, on a $\varphi (x_s) =s$. L’homomorphisme $\varphi$ est donc surjectif (lemme 3). Pour $(s, t)\in T$ et $r=st$, on a $x_r=x_sx_t$; on a donc $x_e=\varepsilon$, car $(e, e)\in T$ ; pour tout $s\in S$, on a aussi $x_{s^{-1}}=x^{-1}_s$ car $(s, s^{-1})\in T$.

Munissons l’ensemble F de la topologie discrète et notons Z l’espace topologique $F\times M$, muni de l’opération de F donnée par $(\gamma ,(g, x))\mapsto$ $(\gamma g, x)$, pour $\gamma$ et $g\in$ F et $u\in$ M. Soient $(g_1, u_1)$ et $(g_2, u_2)$ des éléments de Z ; nous dirons que $(g_1, u_1)$ est congru à $(g_2, u_2)$ s’il existe $s\in S$ tel que $g_2=g_1\cdot x_s$ et $s\cdot u_2=u_1$.

#### Lemme 4 {#ta-i-s6-lem-4 .statement tag=01SM}

La relation « $(g_1, u_1)$ est congru à $(g_2, u_2)$ » est une relation d’équivalence dans Z, compatible avec l’opération de F.

Cette relation est réflexive, car on a $x_e=\varepsilon$. Soient $(g_1, u_1)$ et $(g_2, u_2)$ des éléments de Z tels que $(g_1, u_1)$ soit congru à $(g_2, u_2)$. Soit $s\in S$ tel que $g_2=g_1x_s$ et $s\cdot u_2=u_1$; comme $x_{s^{-1}}=x^{-1}_s$, on a $g_1=g_2x_{s^{-1}}$ et $u_2=s^{-1}\cdot u_1$, donc $(g_2, u_2)$ est congru à $(g_1, u_1)$ ; par suite, cette relation est symétrique. Démontrons enfin qu’elle est transitive. Soient $(g_1, u_1)$, $(g_2, u_2)$ et $(g_3, u_3)$ des points de Z tels que $(g_1, u_1)$ et $(g_2, u_2)$ soient congrus, ainsi que $(g_2, u_2)$ et $(g_3, u_3)$. Soient $s$ et $t$ dans S tels que $g_2=g_1x_s$ et $s\cdot u_2=u_1$ d’une part, et $g_3=g_2x_t$ et $t\cdot u_3=u_2$ d’autre part. On a $u_1=s\cdot u_2=st\cdot u_3$, donc $u_1\in M\cap s\cdot M\cap st\cdot M$, ce qui montre que $(s, t)$ appartient à T et que $st$ appartient à S. On a alors $g_3=g_2x_t=g_1x_sx_t=g_1x_{st}$ et $u_1=st\cdot u_3$; par suite, $(g_1, u_1)$ et $(g_3, u_3)$ sont congrus. Ainsi, la relation « être congru » est une relation d’équivalence dans Z. Elle est compatible avec l’opération de F dans Z.

Soit Y l’espace topologique quotient de Z pour la relation d’équivalence définie ci-dessus. Notons $\pi : Z\rightarrow Y$ l’application canonique. Notons aussi $q: Z\rightarrow X$ l’application donnée par $(g, x)\mapsto \varphi (g)\cdot x$; elle est surjective (lemme 3). Par passage au quotient, l’application $q$ induit une application continue et surjective $p: Y\rightarrow X$ ; d’après le lemme 4, l’opération de F dans Z induit une opération continue de F dans Y telle que $p(g\cdot y) =\varphi (g)\cdot p(y)$ pour tout $g\in F$ et tout $y\in Y$. En particulier, le groupe N = Ker($\varphi$ ) opère continûment sur le X-espace $(Y, p)$.

#### Lemme 5 {#ta-i-s6-lem-5 .statement tag=01SN}

Si M est connexe, l’espace Y est connexe.

Soient $g\in F$ et $s\in S$. Soient $u$ et $v$ des éléments de M tels que $v=s\cdot u$; on a donc $\pi (g, v) =\pi (gx_s, u)$ et les ensembles $\pi (\{g\} \times M)$ et $\pi (\{gx_s\} \times M)$ de Y ont un point commun. Comme ils sont connexes, ils sont contenus dans la même composante connexe de Y. Puisque S est une partie symétrique du groupe G, et que $x_{s^{-1}}=x^{-1}_s$ pour tout $s\in S$, tout élément $g$ de F est de la forme $x_{s_1}. . . x_{s_n}$, où $n\in \mathbf{N}$ et $s_1, . . . , s_n$ sont des éléments de S. Par récurrence sur $n$, les ensembles $\pi (\{e\} \times M)$ et $\pi (\{g\} \times M)$ sont contenus dans la même composante connexe de Y, pour tout $g\in F$. Il en résulte que Y est connexe.

#### Lemme 6 {#ta-i-s6-lem-6 .statement tag=01SO}

Pour tout $x\in X$, le groupe N opère fidèlement et transitivement sur la fibre $\overset{-1}{p}(x)$.

Comme $p$ est surjective, la fibre $\overset{-1}{p}(x)$ n’est pas vide. Soient $y, y'\in$ $\overset{-1}{p}(x)$ ; démontrons qu’il existe un unique élément $n\in$ N tel que $n\cdot y=y'$. Soient $g, h\in$ F et soient $u, v\in$ M tels que $y=\pi (g, u)$ et $y'=\pi (h, v)$. Posons $s=\varphi (g^{-1}h)$. Comme $x=\varphi (g)\cdot u=\varphi (h)\cdot v$, on a $u=s\cdot v$, d’où $s\in S$. Il s’ensuit que $\varphi (h) =\varphi (gx_s)$, si bien qu’il existe $n\in N$ tel que $h=ngx_s$. Alors,

$$
y'=\pi (h, v) =\pi (ngx_s, v) =n\cdot \pi (gx_s, v) =n\cdot \pi (g, s\cdot v) =n\cdot y
$$

Soit $n'$ un élément de N tel que $n'\cdot y=y'$. On a $n'\cdot \pi (g, u) =n\cdot \pi (g, u)$, d’où $\pi (n'g, u) =\pi (ng, u)$. Par conséquent, il existe $t\in S$ tel que $n'g=$ $ngx_t$; cette relation entraîne que $\varphi (x_t) =e$, d’où $t=e$ et $n=n'$.

#### Lemme 7 {#ta-i-s6-lem-7 .statement tag=01SP}

Muni de l’action de N, le X-espace $(Y, p)$ est un revêtement principal à gauche. Il est trivialisable au-dessus de M.

Soit $x\in X$ ; fixons un élément $g\in E_x$ ainsi qu’un élément $\overline{g}\in F$ tel que $\varphi (\overline{g}) =g$. On note $\mu_x: E_x\times M\rightarrow X$ l’application donnée par $(h, u)\mapsto h\cdot u$.

Soit $n\in N$, soient $h, k\in E_x$ et soient $u, v\in M$ tels que $h\cdot u=k\cdot v$; posons $s=g^{-1}h,t=h^{-1}k$ et $r=st=g^{-1}k$. Comme $x$ appartient à $g\cdot M\cap h\cdot M\cap k\cdot M$, le couple $(s, t)$ appartient à T, d’où $x_sx_t=x_r$. On a donc

$$
\pi (ngx_r, v) =\pi (ngx_sx_t, v) =\pi (ngx_s, t\cdot v) =\pi (ngx_s, u)
$$

Il existe ainsi une unique application $\theta : N\times (E_x\cdot M)\rightarrow Y$ telle que $\theta (n, h\cdot u) =\pi (ngx_{g^{-1}h}, u)$ pour tout $n\in N$, tout $h\in E_x$ et tout $u\in M$. On a

$$
p(\theta (n, h\cdot u)) =p(\pi (ngx_s, u)) =q(ngx_s, u) =\varphi (ngx_s)\cdot u=gs\cdot u=h\cdot u
$$

De plus, pour $n, n'\in N$ et $y\in E_x\cdot M$, on a $\theta (n'n, y) =n'\cdot \theta (n, y)$. L’application $\theta ': N\times (E_x\times M)\rightarrow Y$ donnée par $\theta '(n,(h, u)) =\theta (n, \mu_x(h, u))$ est continue ; comme l’application $\mu_x$ est universellement stricte (I, p. 133, lemme 2), l’application $\theta$ est continue. C’est une bijection de $N\times (E_x\cdot M)$ sur le sous-espace $Y\times_X(E_x\cdot M)$ de Y (lemme 6).

Soient $z= (k, v)\in Z$ et $(h, u)\in E_x\times M$ tels que $q(k, v) =\mu_x(h, u)$. Posons $s$ = $h^{-1}\varphi (\overline{k})$ ; comme $\varphi (\overline{k})\cdot v$ = $h\cdot u$, on a $s\in$ S. Posons alors $\lambda '(z,(h, u)) =kx^{-1}_sx_{h^{-1}g}\overline{g}^{-1}$; on a $\varphi (\lambda '(z,(h, u))) =$ $\varphi (\overline{k})s^{-1}h^{-1}gg^{-1}$ = $e$, donc $\lambda '(z,(h, u))\in$ N. On définit ainsi une application continue $\lambda ': Z\times_X(E_x\times M)\rightarrow N$. De plus, pour tout $z$ et $(h, u)$ comme ci-dessus, on a

$$
\theta (\lambda '(z,(h, u)), h\cdot u) =\pi (kx^{-1}_sx_{h^{-1}g}\overline{g}^{-1}gx_{g^{-1}h}, u)
$$

$$
=\pi (kx^{-1}_s, u) =\pi (k, s^{-1}\cdot u) =\pi (k, v) =\pi (z)
$$

et $\lambda '(z,(h, u))$ est l’unique élément $n$ de N tel que $\theta (n, h\cdot u) =\pi (z)$. Il existe en particulier une unique application

$$
\lambda : Y\times_X(E_x\cdot M)\rightarrow N
$$

telle que $\lambda (\pi (z), h\cdot u) =\lambda '(z,(h, u))$ pour tout $z\in Z$ et tout $(h, u)\in$ $E_x\times M$ tels que $q(z) =h\cdot u$. Elle est continue, car l’application $\mu_x$ est universellement stricte. Il en résulte que le $E_x\cdot M$-espace $Y_{E_x\cdot M}$ déduit de Y par changement de base, muni de l’opération de N, est un espace fibré principal de groupe N, trivialisable.

Le lemme est ainsi démontré.

#### Proposition 10 {#ta-i-s6-prop-10 .statement tag=01SQ}

Soit X un espace topologique non vide et connexe, soit G un groupe discret opérant continûment à gauche dans X et soit M une partie de X telle que $G\cdot M = X$. On fait l’une des deux hypothèses suivantes :

(i) L’ensemble M est ouvert ;

(ii) L’ensemble M est fermé et le recouvrement $(g\cdot M)_{g\in G}$ de X est localement fini.

Soit S l’ensemble des éléments $g\in G$ tels que $M\cap g\cdot M=\not\emptyset$, soit T l’ensemble des couples $(s, t)\in S\times S$ tels que $M\cap s\cdot M\cap st\cdot M=\not\emptyset$. Soit F le groupe $F(S,\mathbf{r})$ défini par l’ensemble générateur S et par l’ensemble $\mathbf{r}$ des relateurs $str^{-1}$ pour $r, s, t\in$ S tels que $(s, t)\in$ T et $r$ = $st$; pour $s\in S$, notons $x_s$ l’image de $s$ par l’application canonique de S dans F. Il existe un unique homomorphisme de groupes $\varphi : F\rightarrow G$ tel que $\varphi (x_s) =s$ pour tout $s\in S$. Il est surjectif ; c’est un isomorphisme si l’espace X est simplement connexe, ou, plus généralement, si tout revêtement de X qui est trivialisable au-dessus de M est trivialisable.

L’homomorphisme $\varphi$ est surjectif (I, p. 133, lemme 3). Avec les notations de ce n$^o$, le revêtement Y de X est trivialisable, puisqu’il est trivialisable au-dessus de M. D’après le lemme 5, Y est connexe. Par suite, $p: Y\rightarrow X$ est un homéomorphisme et le groupe N est réduit à l’élément neutre. Par conséquent, l’homomorphisme $\varphi : F\rightarrow G$ est un isomorphisme de groupes.

#### Proposition 11 {#ta-i-s6-prop-11 .statement tag=01SR}

Soient X un espace topologique simplement connexe et G un groupe discret opérant continûment à droite dans X. Si le sous-groupe de G engendré par la réunion des fixateurs des points de X est égal à G, l’espace $X/G$ est simplement connexe.

Soit $(E, p)$ un revêtement de $X/G$. Il s’agit de démontrer que, pour tout point $x$ de E, il existe une section continue $s$ de $p$ telle que $s\circ p(x) =x($I, p. 70, cor. 2 de la prop. 1). Notons $q: X\rightarrow X/G$ l’application canonique et choisissons un point $y$ de X tel que $q(y) =p(x)$. Comme l’espace X est simplement connexe, il existe une application continue $f: X\rightarrow E$ telle que $f(y) =x$ et $p\circ f=q($I, p. 125, prop. 3). Soient $z$ un point de X et $g$ un élément du sous-groupe de G fixateur de $z$. Les applications $t\mapsto f(t)$ et $t\mapsto f(t\cdot g)$ de X dans E sont des relèvements continus à E de l’application $q$ qui coïncident pour $t=z$. Comme l’espace X est connexe, elles sont égales (I, p. 34, cor. 1 de la prop. 11). Comme la réunion des sous-groupes fixateurs des points de X engendre G, on a $f(t\cdot g) =f(t)$ pour tout $t\in X$ et tout $g\in G$. Par passage au quotient, on déduit de $f$ une application continue $s: X/G\rightarrow E$ qui est une section continue de $p$ telle que $s(p(x)) =x$.

## EXERCICES {#ta-i-s6-exercises}

See the [exercises for § 6](exercises/s6/).
