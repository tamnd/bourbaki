---
book: ts
book_title: Théories spectrales
chapter: I
chapter_title: ALGÈBRES NORMÉES
section: 7
section_title: Spectre des endomorphismes des espaces de Banach
lang: fr
source: ts-i-ii-fr
book_pages: A I.127-A I.142, A I.187-A I.191
pdf_pages: 0140-0155, 0200-0204
extraction: native
subsections:
    - "no": 1
      title: Spectre d’un endomorphisme
      page: 127
      pdf_page: 140
    - "no": 2
      title: Projecteurs spectraux
      page: 129
      pdf_page: 142
    - "no": 3
      title: Points isolés du spectre
      page: 131
      pdf_page: 144
    - "no": 4
      title: Spectre de la transposée d’un endomorphisme
      page: 131
      pdf_page: 144
    - "no": 5
      title: Cas des espaces hilbertiens
      page: 132
      pdf_page: 145
    - "no": 6
      title: Image numérique
      page: 135
      pdf_page: 148
    - "no": 7
      title: Éléments positifs
      page: 138
      pdf_page: 151
    - "no": 8
      title: Décomposition polaire
      page: 139
      pdf_page: 152
statements: 24
exercises: 16
content_sha256: 01be4b24f732bc25a789742fe7965095764534270d93cf8168a9024d253ab214
---

## § 7. SPECTRE DES ENDOMORPHISMES DES ESPACES DE BANACH

Sauf mention du contraire, les espaces vectoriels considérés dans ce paragraphe sont des espaces vectoriels sur $\mathbf{C}$. On note $1_E$ l’application identique d’un espace vectoriel E. Un endomorphisme d’un espace vectoriel topologique E est une application linéaire continue de E dans E.

Soient E un espace vectoriel topologique et $u$ un endomorphisme de E. Si F est un sous-espace de E stable par $u$, on dira que l’endomorphisme de F déduit de $u$ par passage aux sous-espaces est l’endomorphisme de F déduit de $u$. On le notera $u|F$.

### 1. Spectre d’un endomorphisme

#### Définition 1 {#ts-i-s7-def-1 .statement tag=02G0}

Soit E un espace vectoriel topologique et soit $u$ un endomorphisme de E. On appelle spectre de $u$, et on note Sp($u$), le spectre de $u$ relativement à l’algèbre unifère $\mathscr{L}(E)$.

Soit E un espace vectoriel topologique et soit $u\in \mathscr{L}(E)$. Le spectre de $u$ est l’ensemble des nombres complexes $\lambda$ tels que $u-\lambda 1_E$ n’est pas un automorphisme de E. Si E est métrisable complet, c’est aussi l’ensemble des nombres complexes $\lambda$ tels que $u-\lambda 1_E$ n’est pas bijectif (EVT, I, p. 19, cor. 1).

Toute valeur propre de $u$ appartient au spectre de $u$, mais la réciproque est fausse en général.

Dans la suite de ce paragraphe, nous nous bornerons à étudier la notion de spectre dans le cas où E est un espace de Banach.

#### Lemme 1 {#ts-i-s7-lem-1 .statement tag=02G1}

Soit E un espace de Banach et soit $u$ un endomorphisme de E. Soit $(E_i)_{i\in I}$ une famille finie de sous-espaces fermés de E, stables par $u$, tels que $E =\bigoplus_{i\in I}E_i$. Pour tout $i\in I$, notons $u_i$ l’endomorphisme de $E_i$ déduit de $u$. On a Sp($u$) $=\bigcup_{i\in I}$ Sp($u_i$), et pour tout $f\in \mathscr{O}$(Sp($u$)), l’endomorphisme $f(u)$ stabilise les espaces $E_i$, et $f(u)$ coïncide avec $f(u_i)$ sur $E_i$.

L’endomorphisme $u$ est un isomorphisme si et seulement si $u_i$ est un isomorphisme pour tout $i\in I$. En appliquant cette propriété à $u-\lambda 1_E$, on en déduit que Sp($u$) est la réunion des ensembles Sp($u_i$) pour $i\in I$.

Soit $f\in \mathscr{O}$(Sp($u$)). L’endomorphisme $f(u)$ de E appartient au bicommutant de $u$ dans $\mathscr{L}(E)$ (th. 5 de I, p. 74), donc commute avec les projecteurs $p_i$. Il stabilise alors les espaces $E_i$. Considérons le morphisme unifère continu $\varpi$ de l’algèbre produit $\prod_{i\in I}\mathscr{L}(E_i)$ dans $\mathscr{L}(E)$ défini par $(v_i)_{i\in I}\mapsto \bigoplus_iv_i$. Il applique la famille $(u_i)$ sur $u$. La prop. 7 de I, p. 75 implique alors que Sp($u$)$\subset \bigcup_{i\in I}$ Sp($u_i$) et

$$
f(u) =f(\varpi ((u_i)_{i\in I})) =\varpi ((f(u_i))_{i\in I}) =\bigoplus_{i\in I}f(u_i)
$$

ce qui conclut la preuve du lemme.

#### Proposition 1 {#ts-i-s7-prop-1 .statement tag=02G2}

Soient E un espace de Banach complexe et $u$ un endomorphisme de E. Soient $\lambda \in \mathbf{C}$ et $f\in \mathscr{O}$(Sp($u$)). On a

Ker($u-\lambda 1_E$)$\subset$ Ker($f(u)-f(\lambda )1_E$).

Soit $x\in E$ non nul. L’ensemble A des $v\in \mathscr{L}(E)$ tels que $x$ soit vecteur propre de $v$ est une sous-algèbre unifère de $\mathscr{L}(E)$.

L’algèbre A est pleine : si $v\in A$ est inversible dans $\mathscr{L}(E)$ et si $x$ est vecteur propre de $v$ pour la valeur propre $\lambda$, alors $\lambda \not= 0$ et $v^{-1}(x) =\lambda^{-1}x$, ce qui prouve que $v^{-1}\in A$.

L’algèbre A est fermée dans $\mathscr{L}(E)$. En effet, si $(v_n)_{n\in\mathbf{N}}$ est une suite dans A telle que $v_n$ converge vers $v\in \mathscr{L}(E)$, la suite $(\lambda_n)_{n\in\mathbf{N}}$ telle que $v_n(x) =\lambda_nx$ est bornée, donc admet une sous-suite convergeant vers un nombre complexe $\mu$, de sorte que $v(x) =\mu x$.

Supposons que $x$ soit vecteur propre de $u$ et que $u(x) =\lambda x$. L’algèbre A contient $u$, donc contient la sous-algèbre unifère fermée pleine B engendrée par $u$, qui est commutative. L’application $\chi : B\rightarrow \mathbf{C}$ qui, à $v$, associe la valeur propre de $v$ relative à $x$ est un caractère de B tel que $\chi (u) =\lambda$. Pour tout $f\in \mathscr{O}$(Sp($u$)), on a $f(u)\in B$ et $\chi (f(u)) =f(\chi (u)) =f(\lambda )$ d’après la prop. 7 de I, p. 75, d’où la proposition.

### 2. Projecteurs spectraux

Soit E un espace de Banach. On note A l’algèbre de Banach unifère $\mathscr{L}(E)$ des endomorphismes de E. Soit $u\in A$.

Soit H une partie de Sp($u$) qui est ouverte et fermée dans Sp($u$) ; notons K son complémentaire dans Sp($u$).

L’élément idempotent associé à $u$ et H (n$^o12$ de I, p. 81) est un projecteur continu de E, appelé le projecteur spectral associé à $u$ et H ; on le note $e_H(u)$, ou simplement $e_H$. Son image est appelée le sous-espace spectral de E associé à $u$ et à H, et notée $E_H(u)$, ou simplement $E_H$. Son noyau est $E_K(u)$, et est également noté $\widetilde{E}_H(u)$, ou simplement $\widetilde{E}_H$. L’espace E est somme directe topologique des sous-espaces fermés $E_H$ et $E_K$. Pour que l’on ait $E_H= 0$, il faut et il suffit que l’on ait $e_H= 0$, c’est-à-dire que la fonction indicatrice $f_H$ de H sur Sp($u$) soit la fonction nulle, c’est-à-dire que $H =\emptyset$.

Tout endomorphisme $v$ de E qui commute à $u$ commute aussi à $e_H(u)$ (th. 5 de I, p. 74), donc stabilise $E_H$ et $E_K$. En particulier, l’endomorphisme $u$ laisse stables les sous-espaces $E_H$ et $E_K$. L’espace $E_K$ est le seul supplémentaire topologique de $E_H$ dans E qui soit stable par $u$.

L’algèbre unifère $A_H=e_HAe_H($loc. cit.) est la sous-algèbre de A formée des endomorphismes de E qui laissent stable $E_H$ et qui sont nuls sur $E_K$. Pour tout $v\in A_H$, on note $v|E_H$ l’endomorphisme de $E_H$ déduit de $v$. L’application $v\mapsto v|E_H$ est un isomorphisme de $A_H$ dans $\mathscr{L}(E_H)$. En particulier, on a Sp($u|E_H$) $=$ Sp$_{A_H}(u|E_H) = H$ et Sp$_{A_K}(u|E_K) = K$ d’après la formule (18) de I, p. 82.

#### Proposition 2 {#ts-i-s7-prop-2 .statement tag=02G3}

Soient E un espace de Banach et $u$ un endomorphisme de E. Soient $E_1$ et $E_2$ des sous-espaces fermés de E stables par $u$ tels que $E = E_1\oplus E_2$. On suppose que les endomorphismes $u_1$ et $u_2$ de $E_1$ et $E_2$ déduits de $u$ ont des spectres disjoints $H_1=$ Sp($u_1$) et $H_2$ = Sp($u_2$). Alors Sp($u$) $= H_1\cup H_2$ et $e_{H_1}(u)$ est le projecteur d’image $E_1$ et de noyau $E_2$. En particulier, on a $E_{H_1}= E_1$ et $E_{H_2}= E_2$.

On a Sp($u$) $= H_1\cup H_2($I, p. 128, lemme 1). Comme les ensembles $H_1$ et $H_2$ sont compacts, ils sont ouverts et fermés dans Sp($u$). Pour toute fonction holomorphe $f$ au voisinage de Sp($u$), l’endomorphisme $f(u)$ stabilise $E_1$ et $E_2$ et coïncide dans $E_1$ avec $f(u_1)$ et dans $E_2$ avec $f(u_2)$ (loc. cit.). Prenons en particulier pour $f$ le germe de fonction holomorphe $f_{H_1}$ qui vaut 1 au voisinage de $H_1$ et 0 au voisinage de $H_2$ (cf. numéro 12 de I, p. 81) ; alors $f_{H_1}(u_1)$ est l’application identique de $E_1$ puisque $f_{H_1}$ = 1 au voisinage de $H_1=$ Sp($u_1$), et $f_{H_1}(u_2)$ est nulle puisque $f_{H_1}= 0$ au voisinage de $H_2$. Donc $e_{H_1}(u) =f_{H_1}(u)$ est le projecteur d’image $E_1$ et de noyau $E_2$, et l’on a donc $E_1= E_{H_1}$ et $E_2= E_{H_2}$.

Soient E un espace de Banach et $u$ un endomorphisme de E. Soit $(H_i)_{i\in I}$ une famille finie de parties ouvertes et fermées de Sp($u$), deux à deux disjointes, et soit H sa réunion. Les relations (15) et (16) de I, p. 81 entraînent les assertions suivantes :

a) La famille de projecteurs $(e_{H_i}(u))_{i\in I}$ est orthogonale (c’est-à-dire, que $e_{H_i}(u)e_{H_j}(u) = 0$ pour tous $(i, j)$ dans $I^2$ tels que $i\not=j$, cf. A, II, p. 18, déf. 7) et sa somme est $e_H(u)$ ;

b) L’espace vectoriel $E_H$ est somme directe topologique de la famille $(E_{H_i})_{i\in I}$;

c) Pour tout $j\in I$, on a $E_{Sp(u)-H_j}= E_{Sp(u)-H}\oplus \bigoplus_{i\not=j}E_{H_i}$;

d) L’espace vectoriel $E_{Sp(u)-H}$ est l’intersection de la famille $(E_{Sp(u)-H_i})_{i\in I}$.

Lorsque H = Sp($u$), la décomposition en somme directe topologique $\bigoplus_{i\in I}E_{H_i}$ de E est appelée la décomposition spectrale de E associée à $u$ et à la partition finie $(H_i)_{i\in I}$ de Sp($u$).

Soit $f$ un élément de $\mathscr{O}$(Sp($u$)). Le spectre de l’endomorphisme $f(u)$ de E est l’image par $f$ du spectre de $u($I, p. 75, prop. 8). Soit L une partie ouverte et fermée de Sp($f(u)$). L’ensemble H des éléments $\lambda \in$ Sp($u$) tels que $f(\lambda )$ appartienne à L est ouvert et fermé dans Sp($u$), et on a $e_L(f(u)) =e_H(u)$ puisque $f_L\circ f=f_H$ dans $\mathscr{O}$(Sp($u$)) (loc. cit.).

### 3. Points isolés du spectre

Soit E un espace de Banach et soit $u$ un endomorphisme de E. Soit $\lambda \in \mathbf{C}$ un point isolé de Sp($u$). On note alors $E_{\lambda}(u) = E_{\{\lambda\}}(u)$ et $e_{\lambda}(u)$ le projecteur spectral d’image $E_{\lambda}(u)$ associé à $u$ et à $\{\lambda \}$.

On note aussi $\widetilde{E}_{\lambda}(u) = E_{Sp(u)-\{\lambda\}}(u)$. Le spectre de l’endomorphisme de $\widetilde{E}_{\lambda}(u)$ déduit de $u$ est Sp($u$)$-\{\lambda \}$; en particulier, $u-\lambda 1_E$ induit un automorphisme de $\widetilde{E}_{\lambda}(u)$.

L’espace $E_{\lambda}(u)$ n’est pas nul. Le spectre de l’endomorphisme de $E_{\lambda}(u)$ déduit de $u$ est réduit à $\lambda$, donc $u-\lambda 1_E$ induit un endomorphisme quasi-nilpotent de $E_{\lambda}(u)$. L’endomorphisme $u-\lambda 1_E$ induit un automorphisme de $\widetilde{E}_{\lambda}(u)$, donc Ker($u-\lambda 1_E$)$^n\subset E_{\lambda}(u)$ pour tout $n\in \mathbf{N}$. En particulier, on a Ker($u-\lambda 1_E$)$\subset E_{\lambda}(u)$.

Pour que $\lambda$ soit pôle d’ordre $p >0$ de la résolvante de $u$, il faut et il suffit que $(u-\lambda 1_E)^{p-1}e_{\lambda}(u)\not= 0$ et $(u-\lambda 1_E)^pe_{\lambda}(u) = 0$ (corollaire de la proposition 17 de I, p. 83). Dans ce cas, on a $E_{\lambda}(u) =$ Ker(($u-\lambda 1_E$)$^p)$ et $\widetilde{E}_{\lambda}(u) =$ Im(($u-\lambda 1_E$)$^p)$, puisque $(u-\lambda 1_E)^p$ induit un automorphisme de $\widetilde{E}_{\lambda}(u)$. On a aussi

$(u-\lambda 1_E)^{p-1}e_{\lambda}(u) =$ lim$_{z\rightarrow\lambda}(z-\lambda 1_E)^pR(u, z)$

d’après la proposition 17 de I, p. 83.

On prendra garde qu’en général $E_{\lambda}(u)$ n’est pas la réunion de la famille (Ker(($u-\lambda 1_E$)$^n))_{n\in\mathbf{N}}$, ni même l’adhérence de cette réunion ; en particulier, un point isolé de Sp($u$) n’est pas nécessairement une valeur propre de $u($I, p. 187, exerc. 1). De même, il peut exister des valeurs propres de $u$ qui ne sont pas des points isolés de Sp($u$) (I, p. 188, exerc. 2).

### 4. Spectre de la transposée d’un endomorphisme

#### Proposition 3 {#ts-i-s7-prop-3 .statement tag=02G4}

Soit E un espace de Banach et soit $E'$ son dual. Soit $u$ un endomorphisme de E.

a) On a Sp($u$) $=$ Sp($^tu$) ;

b) Pour tout $f\in \mathscr{O}$(Sp($u$)), on a $f(^tu) =^tf(u)$ ;

c) On a $e_H(^tu) =^te_H(u)$ pour toute partie H de Sp($u$) qui est ouverte et fermée.

Pour qu’un endomorphisme de E soit un automorphisme, il faut et il suffit que sa transposée soit un automorphisme de $E'$ (EVT, IV, p. 30, cor. 5), d’où l’assertion a).

L’application $v\mapsto^tv$ est un homomorphisme unifère et continu de l’algèbre de Banach $\mathscr{L}(E)$ dans l’algèbre de Banach opposée de $\mathscr{L}(E')$ (EVT, IV, p. 7, prop. 8). Comme l’algèbre $\mathscr{O}$(Sp($^tu$)) est commutative, l’application $f\mapsto^tf(u)$ est un homomorphisme unifère et continu de l’algèbre $\mathscr{O}$(Sp($^tu$)) dans l’algèbre $\mathscr{L}(E')$. Cet homomorphisme applique le germe de l’application identique de $\mathbf{C}$ sur $^tu$, donc coïncide avec l’homomorphisme $f\mapsto f(^tu)$ (th. 5 de I, p. 74). Cela prouve b).

L’assertion c) résulte de b), appliquée à la fonction $f_H$ égale à 1 au voisinage de H et à 0 au voisinage de son complémentaire dans Sp($u$).

#### Remarque {#ts-i-s7-n4-rem-1 .statement tag=02G5}

Soit H une partie ouverte et fermée de Sp($u$), dont la décomposition spectrale associée est $E = E_H(u)\oplus \widetilde{E}_H(u)$. Il découle de l’assertion c) que si l’on identifie $E'$ à $E_H(u)'\oplus \widetilde{E}_H(u)'$, alors on a $E'_H(^tu) = E_H(u)'$ et $\widetilde{E}'_H(^tu) =\widetilde{E}_H(u)'$.

### 5. Cas des espaces hilbertiens

Dans ce numéro, on considère des espaces hilbertiens sur $K =\mathbf{R}$ ou $\mathbf{C}$. On notera $\langle x_1|x_2\rangle$ le produit scalaire de deux vecteurs $x_1$ et $x_2$ dans un espace hilbertien E.

Si E est un espace hilbertien complexe, l’algèbre de Banach $\mathscr{L}(E)$ munie de l’involution $u\mapsto u^*$ est une algèbre stellaire (exemple 1 de I, p. 102). En particulier, si $u\in \mathscr{L}(E)$, on a $\varrho (u^*) =\varrho (u)$ et Sp($u^*$) $=$ Sp($u$).

Soit $u\in \mathscr{L}(E)$ un endomorphisme normal et soit $\lambda \in \mathbf{C}$. L’espace propre de $u$ relatif à $\lambda$ coïncide avec l’espace propre de l’adjoint $u^*$ relatif à $\lambda$ (EVT, V, p. 43, cor. de la prop. 8). Cependant, ces espaces ne coïncident pas en général si $u$ n’est pas normal (exercice 3 de I, p. 188).

Soient $\lambda$ et $\mu$ des nombres complexes tels que $\lambda \not=\mu$. Soit $x$ un vecteur propre de $u$ relatif à $\lambda$ et soit $y$ un vecteur propre de $u$ relatif à $\mu$. Alors, $u^*(x) =\lambda x$, donc

$$
\mu\langle x|y\rangle =\langle x|u(y)\rangle =\langle u^*(x)|y\rangle =\langle \lambda x|y\rangle =\lambda \langle x|y\rangle
$$

Par suite, $\langle x|y\rangle = 0$ : les espaces propres de $u$ sont deux à deux orthogonaux. De plus, pour tout $\lambda \in \mathbf{C}$, l’espace propre de $u$ relatif à $\lambda$ coïncide avec le sous-espace primaire de $u$ relatif à $\lambda$, c’est-à-dire (LIE, VII, §1, n$^o1)$ la réunion pour $k\in \mathbf{N}$ des noyaux de $(u-\lambda 1_E)^k$ (EVT, V, p. 43, cor. de la prop. 8).

#### Lemme 2 {#ts-i-s7-lem-2 .statement tag=02G6}

Soit E un espace hilbertien complexe et soit $u$ un endomorphisme normal de E. Soit $(E_i)_{i\in I}$ une famille finie de sous-espaces fermés de E, stables par $u$ et deux à deux orthogonaux, tels que $E =\bigoplus_{i\in I}E_i$. Pour tout $i\in I$, notons $u_i$ l’endomorphisme de $E_i$ déduit de $u$. On a Sp($u$) $=\bigcup_{i\in I}$ Sp($u_i$), et pour tout $f\in \mathscr{C}$(Sp($u$)), l’endomorphisme $f(u)$ stabilise les espaces $E_i$, et $f(u)$ coïncide avec $f(u_i)$ sur $E_i$.

La preuve suit celle du lemme 1 de I, p. 128 en utilisant la remarque de 6 de I, p. 110 et la prop. 8 de I, p. 112.

#### Proposition 4 {#ts-i-s7-prop-4 .statement tag=02G7}

Soit E un espace hilbertien complexe et soit $u$ un endomorphisme normal de E. Pour toute fonction $f\in \mathscr{C}$ (Sp($u$)) et tout $\lambda \in \mathbf{C}$, on a

Ker($u-\lambda 1_E$)$\subset$ Ker($f(u)-f(\lambda )1_E$).

La preuve est analogue à celle de la proposition 1 de I, p. 128 ; reprenons-en les arguments. L’algèbre A introduite dans loc. cit. est ici une sous-algèbre unifère stellaire de $\mathscr{L}(E)$ (EVT, V, p. 43, cor.). Elle contient donc la sous-algèbre unifère stellaire B engendrée par $u$, qui est commutative. L’application $\chi : B\rightarrow \mathbf{C}$ qui, à $v$, associe la valeur propre de $v$ relative à $x$ est un caractère de B tel que $\chi (u) =\lambda$. Pour tout $f\in \mathscr{C}$ (Sp($u$))), on a $f(u)\in B$ et $\chi (f(u)) =f(\chi (u)) =f(\lambda )$ d’après la prop. 8 de I, p. 112, d’où l’assertion.

#### Lemme 3 {#ts-i-s7-lem-3 .statement tag=02G8}

Soient E un espace hilbertien et $p\in \mathscr{L}(E)$ un projecteur. Les assertions suivantes sont équivalentes :

(i) Le projecteur $p$ est un orthoprojecteur, c’est-à-dire que Ker($p$) $=$ Im($p$)$^{\circ}$ (EVT, V, p. 13) ;

(ii) Le projecteur $p$ est hermitien;

(iii) Le projecteur $p$ est normal ;

(iv) On a Ker($p$)$\subset$ Ker($p^*$) ;

(v) On a Im($p$)$\subset$ Im($p^*$) ;

(vi) Le projecteur $p$ est positif;

(vii) On a $\|p\|\leqslant 1$.

Rappelons d’abord que Ker($p^*$) $=$ Im($p$)$^{\circ}$ et Ker($p$) $=$ Im($p^*$)$^{\circ}$ (EVT, V, p. 41, prop. 4). De plus, l’image de $p$ (resp. $p^*)$ est fermée, puisqu’elle coïncide avec le noyau de $1-p$ (resp. $1-p^*)$. Donc on a

(1) Im($p$) $=$ Ker($p^*$)$^{\circ}$, Im($p^*$) $=$ Ker($p$)$^{\circ}$.

(i) $=\Rightarrow$ (ii)$:p^*$ est un projecteur de noyau Im($p$)$^{\circ}=$ Ker($p$) et dont l’image est Im($p^*$)$^{\circ}=$ Ker($p$) $=$ Im($p$)$^{\circ}$; donc $p^*=p$.

(ii) $=\Rightarrow$ (iii) puisque tout endomorphisme hermitien est normal.

(iii) $=\Rightarrow$ (iv) : comme $p$ est normal, on a $\|p(x)\|^2=\|p^*(x)\|^2$ pour tout $x$ dans E (EVT, V, p. 43, prop. 7), d’où l’inclusion demandée.

(iv) $=\Rightarrow$ (v) suit des égalités (1) ci-dessus.

(v) $=\Rightarrow$ (vi) : pour tout $x\in E$, on a $p(x)\in$ Im($p^*$), et par conséquent $\langle p(x)|x\rangle =\langle p^*(p(x))|x\rangle =\|p(x)\|^2\geqslant 0$.

(vi) $=\Rightarrow$ (vii) : soient $x\in E$ et $y=x-p(x)\in$ Ker($p$). Pour tout $t\in \mathbf{R}$, on a par hypothèse

$$
\langle x+ty|p(x)\rangle =\langle x+ty|p(x+ty)\rangle \geqslant 0
$$

ce qui n’est possible que si $\langle y|p(x)\rangle = 0$. Mais alors

$$
\|p(x)\|^2=\langle x|p(x)\rangle \leqslant \|x\|\|p(x)\|
$$

et donc $\|p\|\leqslant 1$.

(vii) $=\Rightarrow$ (i) : soit $y\in$ Im($p$) ; notons $z$ la projection orthogonale de $y$ sur Ker($p$)$^{\circ}$ et posons $x=y-z\in$ Ker($p$). On a $p(z) =p(y) =y$, donc $\|y\|\leqslant \|z\|$ par hypothèse. Mais, comme $x$ et $z$ sont orthogonaux, on a $\|y\|^2=\|x\|^2+\|z\|^2$, d’où $\|x\|= 0$, c’est-à-dire $y=z$. Ainsi, Im($p$)$\subset$ Ker($p$)$^{\circ}$. Comme de plus $\|p^*\|=\|p\|\leqslant 1$, on a de même Im($p^*$)$\subset$ Ker($p^*$)$^{\circ}$, ce qui fournit l’inclusion réciproque par (1).

#### Proposition 5 {#ts-i-s7-prop-5 .statement tag=02G9}

Soient E un espace hilbertien complexe et $u$ un endomorphisme normal de E.

a) Pour toute partie ouverte et fermée H du spectre de $u$, le projecteur spectral $e_H(u)$ est un orthoprojecteur dont le noyau est l’image du projecteur spectral $e_{Sp(u)-H}(u)$ ;

b) Si $H_1$ et $H_2$ sont des parties disjointes, ouvertes et fermées du spectre de $u$, alors les sous-espaces spectraux $E_{H_1}$ et $E_{H_2}$ sont orthogonaux ;

c) Si $\lambda \in \mathbf{C}$ est un point isolé du spectre de $u$, alors $\lambda$ est une valeur propre de $u$ et l’image du projecteur spectral $e_{\lambda}(u)$ est l’espace propre de $u$ relatif à $\lambda$.

Démontrons a). Comme le calcul fonctionnel holomorphe est compatible avec le calcul fonctionnel continu (I, p. 111, cor. 1), on a $e_H(u) =\varphi_H(u)$, où $\varphi_H\in \mathscr{C}$ (Sp($u$)) est la fonction caractéristique de H. Cela implique $e_H(u)^*=\varphi_H(u) =\varphi_H(u) =e_H(u)$, donc $e_H(u)$ est un orthoprojecteur (lemme 3, (ii)). Son noyau est l’image du projecteur $1-e_H(u) =e_{Sp(u)-H}(u)$.

Démontrons b). Les fonctions caractéristiques $\varphi_{H_1}$ et $\varphi_{H_2}$ de $H_1$ et $H_2$ dans Sp($u$) sont continues et leur produit est nul, ce qui implique $e_{H_1}(u)\circ e_{H_2}(u) =e_{H_2}(u)\circ e_{H_1}(u) = 0$. Les inclusions $E_{H_2}(u)\subset E_{H_1}(u)^{\circ}$ et $E_{H_1}(u)\subset E_{H_2}(u)^{\circ}$ en résultent.

Démontrons enfin l’assertion c). La fonction caractéristique $\varphi_{\lambda}$ de $\{\lambda \}$ est continue et non nulle sur Sp($u$) ; elle vérifie $(z-\lambda )\varphi_{\lambda}(z) = 0$ pour tout $z\in$ Sp($u$). On a donc $(u-\lambda 1_E)\varphi_{\lambda}(u) = 0$. L’image de $\varphi_{\lambda}(u)$, qui est non nulle, est donc contenue dans le sous-espace propre de $u$ relatif à $\lambda$. Comme on a $e_{\lambda}(u) =\varphi_{\lambda}(u)$ et que l’image de $e_{\lambda}(u)$ contient le sous-espace propre de $u$ relatif à $\lambda$, l’assertion en résulte.

#### Lemme 4 {#ts-i-s7-lem-4 .statement tag=02GA}

Soit E un espace hilbertien et soit $u$ un endomorphisme normal de E. Soit F un sous-espace fermé de E contenant un ensemble total de vecteurs propres de $u$. Alors $F^{\circ}$ est stable par $u$ et l’endomorphisme $\widetilde{u}$ de $F^{\circ}$ déduit de $u$ est normal.

Puisque $u$ est normal, tout vecteur propre de $u$ est également vecteur propre de $u^*$ (EVT, V, p. 43, cor.). L’hypothèse implique donc que F est stable par $u$ et par $u^*$. D’après EVT, V, p. 41, prop. 4 (ii), on a donc $u(F^{\circ})\subset F^{\circ}$ et $u^*(F^{\circ})\subset F^{\circ}$. Il en découle que l’adjoint de $\widetilde{u}$ est l’endomorphisme de $F^{\circ}$ déduit de $u^*$. Puisque $u$ est normal, l’endomorphisme $\widetilde{u}$ est normal.

### 6. Image numérique

#### Définition 2 {#ts-i-s7-def-2 .statement tag=02GB}

Soit E un espace hilbertien complexe et soit $u$ un endomorphisme de E. On appelle image numérique de $u$ l’ensemble des nombres complexes de la forme $\langle x|u(x)\rangle$, où $x$ parcourt la sphère unité de E. On note $\iota (u)$ l’image numérique de $u$.

L’image numérique de $u^*$ est l’image de $\iota (u)$ par la conjugaison complexe. Pour tous nombres complexes $\lambda$ et $\mu$, l’image numérique de $\lambda u+\mu1_E$ est égale à $\lambda \iota (u) +\mu$.

#### Proposition 6 {#ts-i-s7-prop-6 .statement tag=02GC}

Soit E un espace hilbertien complexe et soit $u$ un endomorphisme de E.

a) L’ensemble des valeurs propres de $u$ est contenu dans $\iota (u)$ ;

b) Le spectre de $u$ est contenu dans l’adhérence de $\iota (u)$ dans $\mathbf{C}$.

Soit $\lambda$ une valeur propre de $u$ et soit $x\in E$ un vecteur non nul tel que $u(x) =\lambda x$. Quitte à remplacer $x$ par $x/\|x\|$, on peut supposer que $\|x\|= 1$. Alors, $\langle x|u(x)\rangle =\lambda$, donc $\lambda \in \iota (u)$.

Démontrons b). En considérant $u-\lambda 1_E$, on se ramène à démontrer que si 0 appartient au spectre de $u$, alors 0 est adhérent à $\iota (u)$.

Supposons d’abord qu’il existe un nombre réel $c >$ 0 tel que $\|u(x)\|\geqslant c$ pour tout $x$ de norme 1 dans E. L’endomorphisme $u$ est alors injectif et fermé (lemme 8 de I, p. 107). Comme il n’est pas inversible par hypothèse, il n’est pas surjectif. Par conséquent, l’orthogonal du noyau de $u^*$ n’est pas égal à E (EVT, V, p. 41, prop. 4), ce qui démontre que le noyau de $u^*$ n’est pas réduit à 0. Ainsi 0 appartient à $\iota (u^*)$, donc à $\iota (u)$.

Si l’hypothèse précédente n’est pas valide, alors pour tout entier $n\geqslant 1$, il existe un vecteur $x_n$ de norme 1 dans E tel que $\|u(x_n)\|\leqslant 1/n$. On a alors $|\langle x_n|u(x_n)\rangle |\leqslant 1/n$, ce qui implique que 0 appartient à l’adhérence de $\iota (u)$.

Proposition 7 (Théorème de Hausdorff–Toeplitz)

Soit E un espace hilbertien complexe et soit $u\in \mathscr{L}(E)$. L’image numérique $\iota (u)$ est une partie convexe de $\mathbf{C}$.

Nous aurons besoin de deux lemmes pour démontrer cette proposition.

#### Lemme 5 {#ts-i-s7-lem-5 .statement tag=02GD}

Soit E un espace hilbertien complexe de dimension 2. Munissons l’espace vectoriel réel $\mathscr{L}(E)_h$ des endomorphismes hermitiens de E de la norme préhilbertienne $u\mapsto$ Tr($u^*u$)$^{1/2}$. L’ensemble des

$$
\surd
$$

orthoprojecteurs de rang 1 de E est la sphère S de rayon $1/$ 2 centrée en $^1_21_E$ dans le sous-espace affine de dimension 3 des endomorphismes de trace 1 dans $\mathscr{L}(E)_h$.

Soit F le sous-espace affine réel de $\mathscr{L}(E)_h$ formé des éléments de trace 1. Les orthoprojecteurs de rang 1 de E appartiennent à F (lemme 3, (ii)).

Soit $u\in F$. On a $\|u-^1_21_E\|^2=$ Tr($u^2-u+^1_4$) $=$ Tr($u^2$)$-^1_2$. Par conséquent, $u\in S$ si et seulement si Tr($u^2$) $= 1$. Puisque 2 det($u$) $=$ Tr($u$)$^2-$ Tr($u^2$) $= 1-$ Tr($u^2$), cette condition équivaut à det($u$) $= 0$. D’après le théorème de Hamilton–Cayley (A, III, p. 107, prop. 20), on a donc $u\in S$ si et seulement si $u^2-u= 0$, ce qui signifie que $u$ est un projecteur hermitien de rang 1 (loc. cit.), d’où le résultat.

#### Lemme 6 {#ts-i-s7-lem-6 .statement tag=02GE}

Soit E un espace vectoriel normé réel, soit F un espace vectoriel réel et soit $u: E\rightarrow F$ une application affine non injective. Soient B une boule de E et S la sphère correspondante. On a $u(S) =$ $u(B)$, et en particulier, $u(S)$ est convexe.

On se ramène au cas où $u$ est linéaire et où B est la boule unité de E. On a $u(S)\subset u(B)$. Inversement, soit $x\in B$ et soit $y$ un élément non nul de Ker($u$). L’image de l’application continue $t\mapsto  \|x+ty\|$ de $\mathbf{R}$ dans $\mathbf{R}_+$ est un intervalle non borné contenant le nombre réel $\|x\|\leqslant 1$. Il existe donc $t\in \mathbf{R}$ tel que $\|x+ty\|= 1$. On a alors $x+ty\in S$ et $u(x+ty) =u(x)$, donc $u(x)\in u(S)$.

Démontrons la prop. 7. Soient $x$ et $y$ des éléments de la sphère unité de E ; démontrons que le segment d’extrémités $\langle x|u(x)\rangle$ et $\langle y|u(y)\rangle$ est contenu dans l’image numérique de $u$.

Soit F le sous-espace de E engendré par $x$ et $y$. Si dim(F) = 1, on a $\langle x|u(x)\rangle =\langle y|u(y)\rangle$, d’où l’assertion. Sinon, on a dim(F) = 2 ; soit alors $p$ l’orthoprojecteur de E d’image F et notons $u_F$ l’endomorphisme de F donné par $x\mapsto p(u(x))$. Puisque $p$ est hermitien (lemme 3 de I, p. 133), on a $\langle z|u_F(z)\rangle =\langle z|u(z)\rangle$ pour tout $z\in F$, de sorte que $\iota (u_F)\subset \iota (u)$. On peut donc supposer que E = F.

Pour tout élément $z$ de E, soit $v_z$ l’endomorphisme hermitien de E défini par $t\mapsto  \langle z|t\rangle z$; on a $\langle z|u(z)\rangle =$ Tr($u\circ v_z$). Lorsque $z$ parcourt la sphère unité de E$,v_z$ décrit l’ensemble des orthoprojecteurs de rang 1 de E, qui est une sphère S dans le sous-espace affine réel V de $\mathscr{L}(E)$ formé des endomorphismes hermitiens de E de trace 1 (lemme 5). L’image numérique de E est donc l’ensemble des Tr($u\circ v$), pour $v\in S$. L’application $v\mapsto$ Tr($u\circ v$) de V dans $\mathbf{C}$ est linéaire. Comme dim$_{\mathbf{R}}(V) = 3>$ dim$_{\mathbf{R}}(\mathbf{C})$, elle n’est pas injective ; il résulte alors du lemme 6 que $\iota (u)$ est convexe.

### 7. Éléments positifs

Soit E un espace hilbertien complexe. Soit $u$ un endomorphisme de E. Rappelons (EVT, V, p. 45, déf. 6) que $u$ est dit positif si l’on a $\langle x|u(x)\rangle \geqslant 0$ pour tout $x\in E$. L’endomorphisme $u$ est alors hermitien (loc. cit.). De plus, si F est un espace hilbertien complexe et si $v\in$ $\mathscr{L}(F; E)$, alors l’endomorphisme $v^*uv$ de F est positif (EVT, V, p. 45, prop. 12).

#### Proposition 8 {#ts-i-s7-prop-8 .statement tag=02GF}

Soit E un espace hilbertien complexe. Soit $u$ un endomorphisme de E. Les conditions suivantes sont équivalentes :

(i) L’endomorphisme $u$ est positif;

(ii) L’image numérique de $u$ est contenue dans $\mathbf{R}_+$;

(iii) L’endomorphisme $u$ est un élément positif de l’algèbre stellaire $\mathscr{L}(E)$ ;

(iv) Il existe un élément hermitien $v$ de $\mathscr{L}(E)$ tel que $u=v^2$;

(v) Il existe une application linéaire continue $v$ de E dans un espace hilbertien complexe F telle que $u=v^*v$.

D’après EVT, V, p. 45, déf. $6,u$ est positif si et seulement s’il est hermitien et si $\langle x|u(x)\rangle \geqslant 0$ pour tout $x\in E$. L’implication (i) $=\Rightarrow$ (ii) résulte donc de la définition de l’image numérique.

(ii) $=\Rightarrow$ (iii) : l’hypothèse implique que $u$ est hermitien (EVT, V, p. 45, et remarque, p. 2) et son spectre est contenu dans $\mathbf{R}_+$ (prop. 6) ; par suite, $u$ est un élément positif de l’algèbre stellaire $\mathscr{L}(E)$.

(iii) $=\Rightarrow$ (iv) : c’est un cas particulier de la prop. 16 de I, p. 118.

(iv) $=\Rightarrow$ (v) est immédiat.

(v) $=\Rightarrow$ (i) : soit F un espace hilbertien complexe et soit $v\in \mathscr{L}(E; F)$ tel que $u=v^*v$. Soit $x\in E$. On a $\langle x|u(x)\rangle =\langle x|(v^*v)(x)\rangle =\|v(x)\|^2$, ce qui prouve que $u$ est positif.

Rappelons (EVT, V, p. 45, remarque 1) que, pour tout élément hermitien $u$ de $\mathscr{L}(E)$, on pose

$$
\langle x|u(x)\rangle
$$

$m(u) =$ inf $\langle x|u(x)\rangle =$ inf $\iota (u) =$ inf,

$$
_{x\in E}x_{\in E-\{0\}}\|x\|^2
$$

$\|x\|=1$

$$
\langle x|u(x)\rangle
$$

$M(u) =$ sup $\langle x|u(x)\rangle =$ sup $\iota (u) =$ sup.

$$
_{x\in E}x_{\in E-\{0\}}\|x\|^2
$$

$\|x\|=1$

Si $E =\{0\}$, on a $M(u) =-\infty ,m(u) = +\infty$ et $\iota (u) =\emptyset$.

Supposons E non nul ; on a alors $m(u)\leqslant M(u)$ et l’image numérique de $u$ est un intervalle d’extrémités $m(u)$ et $M(u)$. D’après la prop. 6, Sp($u$) est contenu dans l’intervalle $[m(u),M(u)]$. Plus précisément :

#### Proposition 9 {#ts-i-s7-prop-9 .statement tag=02GG}

Soit E un espace hilbertien complexe et soit $u$ un élément hermitien de $\mathscr{L}(E)$.

a) On a $m(u) =$ inf Sp($u$) et $M(u) =$ sup Sp($u$) ;

b) Si E n’est pas nul, on a $\|u\|=$ sup($|m(u)|,|M(u)|$).

Soit $\lambda \in \mathbf{R}$. Pour que $\lambda$ soit un minorant du spectre de $u$, il faut et il suffit que $u-\lambda \geqslant 0$. Cela équivaut (prop. 8, (ii)) à la condition $\langle x|u(x)\rangle \geqslant \lambda \|x\|^2$ pour tout $x\in E$, c’est-à-dire, à $m(u)\geqslant \lambda$. Ceci démontre que $m(u)$ est la borne inférieure de Sp($u$). Similairement, on vérifie que $M(u)$ est la borne supérieure de Sp($u$).

Comme $u$ est normal, on a $\varrho (u) =\|u\|$ (cor. 1 de I, p. 108). Comme $E\not=\{0\}$, le spectre de $u$ n’est pas vide (cor. 1 de I, p. 26) et $\varrho (u)$ est le rayon du plus petit disque de centre 0 qui contient Sp($u$) (th. 1 de I, p. 24), donc b) résulte de a).

### 8. Décomposition polaire

Dans ce numéro, on considère des espaces hilbertiens complexes.

Soient $E_1$ et $E_2$ des espaces hilbertiens et $u\in \mathscr{L}(E_1; E_2)$. L’endomorphisme $u^*u$ de $E_1$ est positif (prop. 8), donc on peut former l’élément positif $(u^*u)^{1/2}$ de $\mathscr{L}(E_1)$.

#### Définition 3 {#ts-i-s7-def-3 .statement tag=02GH}

On dit que $(u^*u)^{1/2}$ est la valeur absolue de $u$, et on la note $|u|$.

Dans le cas où $E_1= E_2$, cette définition coïncide avec celle donnée dans la remarque 9 de I, p. 119.

Pour un élément $u$ de $\mathscr{L}(E_1; E_2)$, rappelons (EVT, V, p. 41, déf. 2) que le sous-espace initial de $u$ est le sous-espace fermé Ker($u$)$^{\circ}$ de $E_1$ et le sous-espace final de $u$ est le sous-espace fermé Im($u$) de $E_2$.

#### Proposition 10 {#ts-i-s7-prop-10 .statement tag=02GI}

Soient $E_1$ et $E_2$ des espaces hilbertiens complexes et $u\in \mathscr{L}(E_1; E_2)$.

a) Le sous-espace initial et le sous-espace final de $|u|$ sont tous deux égaux au sous-espace initial de $u$ et on a $\||u|\|=\|u\|$;

b) Il existe une unique application partiellement isométrique $j$ de $E_1$ dans $E_2$ telle que Ker($j$) $=$ Ker($u$) et $u=j|u|$;

c) Le sous-espace initial (resp. final) de $j$ est égal à celui de $u$;

d) Soient $u_1$ un élément positif de $\mathscr{L}(E_1)$ et $j_1$ un élément partiellement isométrique de $\mathscr{L}(E_1; E_2)$ tels que $u=j_1u_1$ et Ker($j_1$) $=$ Ker($u_1$). Alors $u_1=|u|$ et $j_1=j$.

Pour tout $x\in E_1$, on a

$$
\|u(x)\|^2=\langle x|(u^*u)(x)\rangle =\langle x||u|^2(x)\rangle =\||u|(x)\|^2 \tag{2}
$$

Cela démontre que Ker($u$) $=$ Ker($|u|$) et $\||u|\|=\|u\|$. Comme $|u|$ est hermitien, l’adhérence de l’image de $|u|$ est le supplémentaire orthogonal de son noyau (EVT, V, p. 41, prop. 4), c’est-à-dire l’espace initial de $u$, d’où a).

La formule (2) implique qu’il existe une application isométrique $v$ de Im($|u|$) sur Im($u$) telle que $v(|u|(x)) =u(x)$ pour tout $x\in E_1$. Soit $j$ l’unique élément de $\mathscr{L}(E_1; E_2)$ qui prolonge $v$ et s’annule dans Im($|u|$)$^{\circ}=$ Ker($|u|$) $=$ Ker($u$). Alors $j$ possède les propriétés de b). L’unicité de $j$ découle de la décomposition E = Ker($u$)$\oplus$ Im($|u|$).

Le sous-espace initial de $j$ est Ker($j$)$^{\circ}=$ Ker($u$)$^{\circ}$, l’espace initial de $u$. Son sous-espace final est $j$(Ker($u$)$^{\circ}) =j$(Im($|u|$)) $=$ Im($u$), le sous-espace final de $u$. Cela démontre c).

Soient maintenant $u_1$ et $j_1$ comme dans d). On a $u^*u=u_1j_1^*j_1u_1$. L’application $j_1^*j_1$ est l’orthoprojecteur de noyau Ker($j_1$) $=$ Ker($u_1$) (EVT, V, p. 41, prop. 5 (ii)) et donc d’image Im($u_1$). Donc $u^*u=u^2_1$ et par suite $u_1= (u^*u)^{1/2}=|u|($I, p. 118, prop. 16). L’assertion d’unicité de b) implique finalement que $j_1=j$.

#### Définition 4 {#ts-i-s7-def-4 .statement tag=02GJ}

Soient $E_1$ et $E_2$ des espaces hilbertiens complexes et $u\in \mathscr{L}(E_1; E_2)$. Le couple $(j,|u|)$, où $j$ est l’unique application partiellement isométrique de $E_1$ dans $E_2$ telle que $u=j|u|$ et Ker($j$) $=$ Ker($u$), est appelé la décomposition polaire de $u$.

#### Proposition 11 {#ts-i-s7-prop-11 .statement tag=02GK}

Soient $E_1$ et $E_2$ des espaces hilbertiens complexes et $u\in \mathscr{L}(E_1; E_2)$. Soit $(j,|u|)$ la décomposition polaire de $u$.

a) On a $|u|=j^*u=u^*j$;

b) On a $|u^*|=ju^*=uj^*$;

c) La décomposition polaire de $u^*$ est $(j^*,|u^*|)$.

Notons I = Ker($u$)$^{\circ}$ et F = Im($u$) le sous-espace initial et le sous-espace final de $u$; on a de plus I = Ker($|u|$)$^{\circ}=$ Im($|u|$) (prop. 10, a)). L’application $j^*j$ est l’orthoprojecteur de $E_1$ sur I (loc. cit. et EVT, V, p. 41, prop. 5 (ii)). On a donc $j^*u=j^*j|u|=|u|$, puis $u^*j= (j^*u)^*=|u|^*=|u|$, d’où a).

Similairement, on calcule $u^*$ = $|u|j^*= (j^*j|u|)j^*$ = $j^*(j|u|j^*)$. L’endomorphisme $j|u|j^*$ de $E_2$ est positif. L’application linéaire $j^*$ est partiellement isométrique d’espace initial F et d’espace final I (EVT, V, p. 41, prop. 5) et les applications linéaires de I dans F (resp. de F dans I) déduites de $j$ et $j^*$ par passages aux sous-espaces sont des isomorphismes réciproques l’un de l’autre (loc. cit.). On a donc Ker($j|u|j^*$) $=$ Ker($|u|j^*$) $=$ Ker($j^*$), puisque l’image de $j^*$ est contenue dans Ker($u$)$^{\circ}=$ Ker($|u|$)$^{\circ}$. D’après la prop. 10, d), le couple $(j^*, j|u|j^*)$ est la décomposition polaire de $u^*$. Cela prouve c) et l’assertion b) se déduit alors de l’assertion a) appliquée à $u^*$.

#### Corollaire {#ts-i-s7-n8-cor-1 .statement tag=02GL}

Soient $E_1$ et $E_2$ des espaces hilbertiens complexes et soit $u\in \mathscr{L}(E_1; E_2)$. On a Im($u$) $=$ Im($|u^*|$).

Soit $(j,|u|)$ la décomposition polaire de $u$. On a $|u^*|=j|u|j^*=uj^*$ d’après la proposition précédente. D’après EVT, V, p. 41, prop. 5, l’application $j^*$ est partiellement isométrique. Son espace final est Ker($j$)$^{\circ}=$ Ker($u$)$^{\circ}$ (prop. 10, c)). L’assertion en résulte.

#### Proposition 12 {#ts-i-s7-prop-12 .statement tag=02GM}

Soient $E_1$ et $E_2$ des espaces hilbertiens complexes et $u\in \mathscr{L}(E_1; E_2)$. Soit $(j,|u|)$ la décomposition polaire de $u$. Pour que $u$ soit bijectif, il faut et il suffit que $|u|$ soit inversible dans $\mathscr{L}(E_1)$ et que $j$ soit un isomorphisme de $E_1$ sur $E_2$.

La condition est suffisante. Réciproquement, si $u$ est bijectif, alors $u^*u$ est inversible dans $\mathscr{L}(E_1)$, et $|u|= (u^*u)^{1/2}$ l’est également puisque son spectre est contenu dans $\mathbf{R}_+^*$. En outre, Ker($j$) $=$ Ker($u$) $=\{0\}$ et Im($j$) $=$ Im($u$) $= F$, donc $j$ applique isométriquement $E_1$ sur $E_2$.

#### Proposition 13 {#ts-i-s7-prop-13 .statement tag=02GN}

Soient E un espace hilbertien complexe et $u$ un endomorphisme de E. Les conditions suivantes sont équivalentes:

(i) L’endomorphisme $u$ est normal;

(ii) Il existe un élément unitaire $v$ de $\mathscr{L}(E)$, permutable à $|u|$, tel que $u=v|u|$.

Soit $(j,|u|)$ la décomposition polaire de $u$. Supposons que $u$ est normal. On a alors $|u^*|= (uu^*)^{1/2}= (u^*u)^{1/2}=|u|$. La prop. 11 implique alors $|u|j=|u^*|j=ju^*j=j|u|$. De plus, $j$ laisse stables les sous-espaces orthogonaux supplémentaires Ker($|u|$) $=$ Ker($j$) et Im($|u|$) $=$ Im($j$) (prop. 10). Soit $v$ l’élément de $\mathscr{L}(E)$ qui coïncide avec $j$ sur Ker($u$)$^{\circ}$ et avec l’application identique sur Ker($u$). Comme $j$ induit une isométrie de Ker($u$)$^{\circ}$ sur Im($u$) $=$ Ker($u^*$)$^{\circ}=$ Ker($u$)$^{\circ}$ (puisque $u$ est normal), l’endomorphisme $v$ est unitaire ; il est de plus permutable à $|u|$, puisque $j|u|=|u|j$, et l’on a $u=v|u|$.

Inversement, soit $v$ un élément unitaire de $\mathscr{L}(E)$, permutable à $|u|$, tel que $u=v|u|$. On a $uu^*=v|u|^2v^*=|u|^2vv^*=|u|^2=u^*u$, donc $u$ est normal.

Soit E un espace hilbertien complexe et $u\in \mathscr{L}(E)$. Soit $(j,|u|)$ la décomposition polaire de $u$. Il est possible que $j$ soit permutable à $|u|$ sans que $u$ soit normal (exercice 11 de I, p. 189).

## EXERCICES {#ts-i-s7-exercises}

Dans les exercices ci-dessous, tous les espaces de Banach sont sur $\mathbf{C}$.

See the [exercises for § 7](exercises/s7/).
