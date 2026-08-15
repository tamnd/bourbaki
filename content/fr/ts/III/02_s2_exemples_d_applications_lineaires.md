---
book: ts
book_title: Théories spectrales
chapter: III
chapter_title: APPLICATIONS LINÉAIRES COMPACTES ET PERTURBATIONS
section: 2
section_title: Exemples d’applications linéaires compactes
lang: fr
source: ts-iii-v-fr
book_pages: A III.23-A III.39, A III.118-A III.120
pdf_pages: 0037-0053, 0132-0134
extraction: native
subsections:
    - "no": 1
      title: Endomorphismes de trace finie, de Hilbert–Schmidt et de puissance $p^{\mathbf{e}}$ nucléaire
      page: 23
      pdf_page: 37
    - "no": 2
      title: Opérateurs diagonaux dans des espaces de suites
      page: 23
      pdf_page: 37
    - "no": 3
      title: Applications linéaires à valeurs dans un espace de fonctions continues définies par un noyau
      page: 25
      pdf_page: 39
    - "no": 4
      title: Applications linéaires entre espaces de Lebesgue définies par un noyau
      page: 26
      pdf_page: 40
    - "no": 5
      title: Restriction d’applications différentiables
      page: 34
      pdf_page: 48
    - "no": 6
      title: Restriction de sections différentiables d’un fibré vectoriel
      page: 35
      pdf_page: 49
    - "no": 7
      title: Restriction de sections analytiques d’un fibré vectoriel
      page: 37
      pdf_page: 51
statements: 26
exercises: 4
content_sha256: eeceaf124b8ad7a5a37337636b826e56e9b84dee69cfb838fb81dd9021a4c1ed
---

## § 2. EXEMPLES D’APPLICATIONS LINÉAIRES COMPACTES

### 1. Endomorphismes de trace finie, de Hilbert–Schmidt et de puissance $p^{\mathbf{e}}$ nucléaire

*Soient E et F des espaces hilbertiens. Tout endomorphisme de E de trace finie (EVT, V, p. 49, déf. 7 et p. 50, déf. 8) est compact (IV, p. 165, cor. 1) ; toute application de Hilbert–Schmidt de E dans F (EVT, V, p. 51, déf. 9) est compacte (IV, p. 165, cor. 2).

Pour tout nombre réel $p\geqslant 1$, l’espace vectoriel $\mathscr{L}_p(E; F)$ des applications linéaires de E dans F de puissance $p^e$ nucléaire est contenu dans $\mathscr{L}^c(E; F) ($cf. IV, p. 169, remarque 2 pour $p= 1).*$

### 2. Opérateurs diagonaux dans des espaces de suites

Soit I un ensemble non vide. Rappelons (EVT, I, p. 4 et p. 5) que l’espace vectoriel des familles bornées $x= (x_i)_{i\in I}$ d’éléments de $\mathbf{C}$, muni de la norme $\|x\|=$ sup$_i|x_i|$, est un espace de Banach que l’on note $\ell^{\infty}_{\mathbf{C}}(I)$.

Soit $p$ un élément de $[1,+\infty [$. L’espace $\ell^p_{\mathbf{C}}(I)$ des familles $x= (x_i)_{i\in I}$ d’éléments de $\mathbf{C}$ telles que la famille $(|x_i|^p)$ soit sommable est un espace vectoriel sur lequel l’application $x\mapsto  \|x\|= (\sum_i|x_i|^p)^{1/p}$ est une norme qui en fait un espace de Banach. Si l’on munit l’espace I de la topologie discrète et de la mesure pour laquelle $\mu(\{x\}) = 1$ pour tout $x\in I$, cet espace n’est autre que l’espace de Banach $L^p_{\mathbf{C}}(I, \mu)$. Lorsque $p= 1$ ou $p= 2$, cette notation coïncide ainsi avec celle de EVT, I, p. 4 et EVT, V, p. 18 (cf. INT, IV, p. 141, §4, n$^o1$, exemple).

Pour des familles $x= (x_i)_{i\in I}$ et $y= (y_i)_{i\in I}$ de nombres complexes, on note $xy$ la famille $(x_iy_i)_{i\in I}$.

#### Proposition 1 {#ts-iii-s2-prop-1 .statement tag=02QK}

Soit $\lambda = (\lambda_i)_{i\in I}$ une famille bornée d’éléments de $\mathbf{C}$. Soit $p$ un élément de $[1,+\infty ]$. Soit E l’espace de Banach $\ell^p_{\mathbf{C}}(I)$.

a) Pour tout $x\in E$, on a $\lambda x\in E$ et l’application $u:x\mapsto \lambda x$ est un endomorphisme continu de E, dont le spectre dans l’algèbre de Banach $\mathscr{L}(E)$ est égal à l’adhérence dans $\mathbf{C}$ de l’ensemble des $\lambda_i$, et dont la norme est égale à sup$_i|\lambda_i|$;

b) L’endomorphisme $u$ est compact si et seulement si pour tout nombre réel $\varepsilon  >0$, l’ensemble des éléments $i\in I$ tels que $|\lambda_i|\geqslant \varepsilon$ est fini.

Avec les notations de la proposition, l’endomorphisme $x\mapsto \lambda x$ est appelé un endomorphisme diagonal de $\ell^p_{\mathbf{C}}(I)$.

Démontrons la proposition. Soit C = sup$_i|\lambda_i|$. Soit $x\in E$. On a les inégalités

$\sum_{i\in I}|\lambda_ix_i|^p\leqslant C^p\|x\|^p$, si $p\not = +\infty$

sup$|\lambda_ix_i|\leqslant C\|x\|$, si $p= +\infty$.

$i\in I$

Cela prouve que $\lambda x\in E$. L’application $x\mapsto \lambda x$ est donc un endomorphisme de E, et ces inégalités prouvent qu’il est de norme $\leqslant C$.

Pour $j\in I$, notons $e_j$ l’élément $(x_i)_{i\in I}$ de $\ell^p_{\mathbf{C}}(I)$ tel que $x_j= 1$ et $x_i= 0$ si $i\not =j$. On a alors $u(e_j) =\lambda_je_j$ pour tout $j\in I$, ce qui montre que $\lambda_j$ appartient au spectre de $u$. Comme le spectre de $u$ est fermé, l’adhérence dans $\mathbf{C}$ de l’ensemble des $\lambda_i$ est inclus dans le spectre de $u$. Puisque le spectre de $u$ est contenu dans le disque centré en 0 et de rayon $\|u\|($I, p. 24, th. 1 et formule (3) de I, p. 21), on en déduit l’inégalité $C\leqslant \|u\|$, d’où $\|u\|= C$.

Réciproquement, si $\lambda \in \mathbf{C}$ n’est pas adhérent à l’ensemble des $\lambda_i$, alors la famille $((\lambda_i-\lambda )^{-1})_{i\in I}$ est bornée. Ce qui précède montre donc que l’application linéaire $x\mapsto ((\lambda -\lambda_i)^{-1}x_i)_{i\in I}$ est un endomorphisme de E. Il est inverse de $u-\lambda 1_E$, et donc $\lambda$ n’appartient pas au spectre de $u$. Cela démontre a).

Démontrons maintenant b). Supposons que l’endomorphisme $u$ est compact. Soit $\varepsilon  >0$. Notons J l’ensemble des $i\in I$ tels que $|\lambda_i|\geqslant \varepsilon$. L’ensemble des éléments $e_i$ pour $i\in J$ est borné dans E. Son image par $u$, formée des éléments $\lambda_ie_i$ pour $i\in J$, est donc relativement compacte dans E (remarque 1 de III, p. 2). Comme $\|\lambda_ie_i-\lambda_je_j\|\geqslant \varepsilon$ pour tout couple d’éléments $i\not =j$ dans J, cela n’est possible que si l’ensemble J est fini.

Démontrons l’assertion réciproque. Soit J une partie finie de I et notons $z_J= (z_{J,i})_{i\in I}$, où $z_{J,i}=\lambda_i$ pour $i\in J$ et $z_{J,i}= 0$ pour $i\in I$- J ; la famille $z_J$ définit un endomorphisme de rang fini $u_J:x\mapsto z_Jx$ de E. D’après ce qui précède, la norme de l’application linéaire $u-u_J$ est majorée par la borne supérieure dans $\mathbf{R}_+$ de la famille $(|\lambda_i|)_{i\in I-J}$. L’hypothèse implique que pour tout $\varepsilon  >0$, il existe une partie finie $J\subset I$ telle que cette borne supérieure soit $\leqslant \varepsilon$. Il en résulte que l’application $u$ est adhérente à $\mathscr{L}^f$(E), et donc qu’elle est compacte (III, p. 4, cor. de la prop. 2).

#### Remarque 1 {#ts-iii-s2-n2-rem-1 .statement tag=02QL}

L’hypothèse de l’assertion b) est toujours valide si I est fini. Lorsque l’ensemble I est infini, elle signifie que la famille $(\lambda_i)_{i\in I}$ tend vers 0 suivant le filtre des complémentaires de parties finies de I ; en particulier, l’ensemble des $i\in I$ tels que $\lambda_i\not = 0$ est alors dénombrable.

#### Remarque 2 {#ts-iii-s2-n2-rem-2 .statement tag=02QM}

*On verra ultérieurement (cf. IV, p. 149, théorème 1) que lorsque $p= 2$, tout endomorphisme compact normal de l’espace hilbertien $\ell^2_{\mathbf{C}}(I)$ est de la forme $u=w\circ v\circ w^{-1}$ où $v$ est un endomorphisme compact diagonal et $w$ est un endomorphisme unitaire (EVT, V, p. 40) de l’espace hilbertien $\ell^2_{\mathbf{C}}(I).*$

### 3. Applications linéaires à valeurs dans un espace de fonctions continues définies par un noyau

On prend ici $K =\mathbf{C}$. Soient X et Y des espaces topologiques localement compacts. Soient $\mu$ une mesure complexe sur X et $k$ une application de $X\times Y$ dans $\mathbf{C}$ possédant les deux propriétés suivantes :

(i) Pour tout $y\in Y$, la fonction $k_y:x\mapsto k(x, y)$ de X dans $\mathbf{C}$ est $\mu$-intégrable ;

(ii) L’application $y\mapsto k_y$ de Y dans $\mathscr{L}_{\mathbf{C}}^1(X, \mu)$ est continue.

Munissons l’espace $\mathscr{C}(Y)$ des fonctions continues sur Y à valeurs complexes de la topologie de la convergence compacte. Pour $f$ dans $\mathscr{L}_{\mathbf{C}}^{\infty}(X, \mu)$, on définit $\widetilde{k}(f) : Y\rightarrow \mathbf{C}$ par

$$
\widetilde{k}(f)(y) =\int_Xk(x, y)f(x)d\mu(x) =\int_Xk_yf d\mu \tag{1}
$$

L’application $h\mapsto \int_Xhf d\mu$ est une forme linéaire continue sur $\mathscr{L}_{\mathbf{C}}^1(X, \mu)$, donc la condition (ii) montre que la fonction $\widetilde{k}(f)$ est continue.

#### Proposition 2 {#ts-iii-s2-prop-2 .statement tag=02QN}

L’application $\widetilde{k}$ de $\mathscr{L}_{\mathbf{C}}^{\infty}(X, \mu)$ dans $\mathscr{C}(Y)$ est compacte.

Quels que soient $y$ et $y'$ dans Y, on a

$$
|\widetilde{k}(f)(y)|\leqslant \|k_y\|_1\|f\|_{\infty},|\widetilde{k}(f)(y)-\widetilde{k}(f)(y')|\leqslant \|k_y-k_{y'}\|_1\|f\|_{\infty}
$$

D’après le théorème d’Ascoli (TG, X, p. 18, cor. 2), il en résulte que l’image par $\widetilde{k}$ de la boule unité de $\mathscr{L}_{\mathbf{C}}^{\infty}(X;\mu)$ est relativement compacte dans $\mathscr{C}(Y)$.

#### Corollaire {#ts-iii-s2-n3-cor-1 .statement tag=02QO}

Soient X un espace topologique compact, Y un espace topologique localement compact, $\mu$ une mesure complexe sur X et $k$ une application continue de $X\times Y$ dans $\mathbf{C}$. Alors la formule (1) définit une application linéaire compacte, encore notée $\widetilde{k}$, de $\mathscr{C}(X)$ muni de la topologie de la convergence uniforme dans $\mathscr{C}(Y)$ muni de la topologie de la convergence compacte.

Vérifions les conditions (i) et (ii) pour $k$. Pour tout $y\in Y$, l’application $k_y$ est continue sur l’espace compact X, donc $\mu$-intégrable. De plus, l’application $y\mapsto k_y$ est continue de Y dans $\mathscr{C}(X)$ puisque X est compact (TG, X, p. 28, th. 3). Comme $\|k_y-k_{y'}\|_1\leqslant \|\mu\| \|k_y-k_{y'}\|$ pour tout $(y, y')\in Y^2$, cette application de Y dans $\mathscr{L}_{\mathbf{C}}^1(X, \mu)$ est continue. D’après la prop. 2, l’application $\widetilde{k}$ de $\mathscr{L}_{\mathbf{C}}^{\infty}(X, \mu)$ dans $\mathscr{C}(Y)$ est compacte. Par composition avec l’application canonique $\mathscr{C}(X)\rightarrow \mathscr{L}_{\mathbf{C}}^{\infty}(X, \mu)$, on obtient une application linéaire compacte de $\mathscr{C}(X)$ dans $\mathscr{C}(Y)$.

### 4. Applications linéaires entre espaces de Lebesgue définies par un noyau

On prend ici $K =\mathbf{C}$. Soit X un espace topologique localement compact muni d’une mesure positive $\mu$. Pour tout $r\in [1,+\infty ]$, on note $\mathscr{L}^r(X) =\mathscr{L}_{\mathbf{C}}^r(X, \mu)$ et $L^r(X) = L^r_{\mathbf{C}}(X, \mu)$. Lorsque $r\in [1,+\infty [$, on identifie le dual de $L^r(X)$ avec $L^{r'}(X)$ où $r'$ est l’exposant conjugué de $r$, tel que $1/r+ 1/r'= 1$ (INT, V, p. 61, § 5, n$^o8$, th. 4). On note $\|f\|_r$ la norme (ou semi-norme) de $f\in L^r(X)$ (ou $f\in \mathscr{L}^r(X))$.

On rappelle qu’une partie A de X est dite $\mu$-modérée (INT, V, p. 4, § 1, n$^o2)$ si elle est contenue dans la réunion d’une suite d’ensembles $\mu$-intégrables, et qu’une fonction $f$ définie sur X à valeurs dans un espace vectoriel ou dans $\overline{\mathbf{R}}$ est $\mu$-modérée si elle est nulle dans le complémentaire d’une partie $\mu$-modérée de X. Si 1 $\leqslant p <+\infty$ et $f\in \mathscr{L}^p$(X), alors $f$ est modérée (INT, V, p. 9, § 1, n$^o3$, cor.). Si $f$ est $\mu$-modérée, alors $f g$ est $\mu$-modérée pour toute fonction $g$.

Soient $p$ et $q$ des éléments de$]1,+\infty [$. Soient X et Y des espaces topologiques localement compacts, munis de mesures positives $\mu$ et $\nu$, respectivement. On munit l’espace $X\times Y$ (resp. $Y\times X)$ de la mesure produit $\mu\otimes \nu$ (resp. $\nu \otimes \mu)$.

On note $\mathscr{N}^{p,q}(X\times Y, \mu\otimes \nu )$, ou simplement $\mathscr{N}^{p,q}(X\times Y)$, l’ensemble des applications $(\mu\otimes \nu$)-mesurables $k$ de $X\times Y$ dans $\mathbf{C}$ telles qu’il existe un nombre réel $C\geqslant 0$ vérifiant

$$
\int_{X\times Y}^*|k(x, y)f(x)g(y)|d(\mu\otimes \nu )(x, y)\leqslant C\|f\|_p\|g\|_q \tag{2}
$$

pour toutes fonctions $f\in \mathscr{L}^p(X)$ et $g\in \mathscr{L}^q(Y)$. On note alors $\|k\|_{p,q}$ la borne inférieure de l’ensemble des nombres réels C ayant cette propriété.

#### Remarque {#ts-iii-s2-n4-rem-1 .statement tag=02QP}

Soient $f\in \mathscr{L}^p(X)$ et $g\in \mathscr{L}^q(Y)$. Puisque $p <+\infty$ et $q <+\infty$, les fonctions $f$ et $g$ sont modérées, et la fonction définie par $(x, y)\mapsto f(x)g(y)$ est $(\mu\otimes \nu$)-modérée (cf. INT, V, p. 92, § 8, n$^o3$, cor. 2). Par conséquent, la fonction $(x, y)\mapsto k(x, y)f(x)g(y)$ est $(\mu\otimes \nu$)-modérée, et en particulier l’intégrale supérieure de sa valeur absolue coïncide avec l’intégrale supérieure essentielle (INT, V, p. 6, § 1, n$^o3$, prop. 7).

L’ensemble $\mathscr{N}^{p,q}(X\times Y)$ est un sous-espace vectoriel de l’espace des fonctions de $X\times Y$ dans $\mathbf{C}$ et l’application définie par $k\mapsto  \|k\|_{p,q}$ est une semi-norme sur $\mathscr{N}^{p,q}(X\times Y)$.

#### Lemme 1 {#ts-iii-s2-lem-1 .statement tag=02QQ}

Soit $k\in \mathscr{N}^{p,q}(X\times Y)$. La fonction $k$ est localement $(\mu\otimes \nu )$-intégrable.

L’application $k$ est $(\mu\otimes \nu$)-mesurable par hypothèse. Soit A une partie compacte de $X\times Y$. Il existe des parties compactes $B\subset X$ et $C\subset Y$ telles que $A\subset B\times C$. En appliquant (2) aux fonctions caractéristiques $\varphi_B$ de B et $\varphi_C$ de C, on obtient

$$
\int_{X\times Y}^*|k(x, y)|\varphi_A(x, y)d(\mu\otimes \nu )(x, y)
$$

$$
\leqslant \int_{X\times Y}^*|k(x, y)|\varphi_B(x)\varphi_C(y)d(\mu\otimes \nu )(x, y)<+\infty
$$

d’où le résultat (INT, V, p. 41, §5, n$^o1$, prop. 1 et déf. 1).

#### Proposition 3 {#ts-iii-s2-prop-3 .statement tag=02QR}

a) Soit $k\in \mathscr{N}^{p,q}(X\times Y)$. Pour $f\in \mathscr{L}^p(X)$ et $g\in \mathscr{L}^q(Y)$, la fonction

$$
(x, y)\mapsto k(x, y)f(x)g(y)
$$

est $(\mu\otimes \nu )$-intégrable et il existe une unique application $u_k$ de $L^p(X)$ dans $L^{q'}(Y)$ telle que

$$
\langle g, u_k(f)\rangle =\int_{X\times Y}k(x, y)f(x)g(y)d(\mu\otimes \nu )(x, y)
$$

pour tous $f\in L^p(X)$ et $g\in L^q(Y)$. L’application $u_k$ est linéaire et continue, sa norme est $\leqslant \|k\|_{p,q}$;

b) Soit $k\in \mathscr{N}^{p,q}(X\times Y)$. On a $u_k= 0$ si et seulement si $k$ est localement $(\mu\otimes \nu )$-négligeable ;

c) L’application qui à $k$ associe $u_k$ est une application linéaire continue de l’espace semi-normé $\mathscr{N}^{p,q}(X\times Y)$ dans l’espace de Banach $\mathscr{L}(L^p(X); L^{q'}(Y))$, telle que $\|u_k\|\leqslant \|k\|_{p,q}$ pour tout $k\in \mathscr{N}^{p,q}(X\times Y)$.

Soit $k\in \mathscr{N}^{p,q}(X\times X)$. Par définition, la fonction de $X\times Y$ dans $\mathbf{C}$ définie par $(x, y)\mapsto k(x, y)f(x)g(y)$ est $(\mu\otimes \nu$)-intégrable lorsque $f\in \mathscr{L}^p(X)$ et $g\in \mathscr{L}^q$(Y), et l’application

$$
b_k: (f, g)\mapsto \int_{X\times Y}k(x, y)f(x)g(y)d(\mu\otimes \nu )(x, y)
$$

est une application bilinéaire continue de $L^p(X)\times L^q(Y)$ dans $\mathbf{C}$. Pour tout $f\in L^p$(X), il existe donc un unique $h\in L^{q'}(Y)$ tel que $b_k(f, g) =$ $\langle g, h\rangle$ pour tout $g\in L^q(Y)$; notons $u_k(f) =h$. D’après (2), on a $\|u_k(f)\|_{q'}\leqslant \|k\|_{p,q}\|f\|_p$; l’application $u_k$ est linéaire et continue de norme $\leqslant \|k\|_{p,q}$. De plus, l’application $k\mapsto u_k$ est linéaire, et les assertions a) et c) en découlent.

Démontrons b). Supposons que $k$ est localement $(\mu\otimes \nu$)-négligeable. Soient $f\in \mathscr{L}^p(X)$ et $g\in \mathscr{L}^q(Y)$; la fonction définie sur $X\times Y$ par $(x, y)\mapsto k(x, y)f(x)g(y)$ est $(\mu\otimes \nu$)-modérée. Comme elle est localement $(\mu\otimes \nu$)-négligeable, elle est négligeable (INT, V, p. 7, § 1, n$^o2$, cor. 1). Ainsi, on a $\langle u_k(f), g\rangle =b_k(f, g) = 0$. Il en résulte que $u_k= 0$.

Réciproquement, soit $k\in \mathscr{N}^{p,q}(X\times Y)$ tel que $u_k= 0$. La fonction $k$ est localement $(\mu\otimes \nu$)-intégrable (lemme 1). Pour toutes fonctions $f\in \mathscr{K}(X)$ et $g\in \mathscr{K}$ (Y), on a

$$
\langle g, u_k(f)\rangle =\int_{X\times Y}f(x)g(y)k(x, y)d(\mu\otimes \nu )(x, y)
$$

donc la mesure $k\cdot (\mu\otimes \nu )$ sur $X\times Y$ est nulle (cf. INT, III, p. 82, § 4, n$^o1$, th. 1). Cela signifie que $k$ est localement $(\mu\otimes \nu$)-négligeable (INT, V, p. 46, §5, n$^o3$, cor. 2).

#### Définition 1 {#ts-iii-s2-def-1 .statement tag=02QS}

Soit $k\in \mathscr{N}^{p,q}(X\times Y)$. On dit que l’application $u_k$ est l’opérateur intégral à noyau $k$ de $L^p(X)$ dans $L^{q'}(Y)$.

Pour $k\in \mathscr{N}^{p,q}(X\times Y)$ et $f\in \mathscr{L}^p$(X), on notera parfois aussi $u_k(f)$ l’image par $u_k$ de la classe de $f$ dans $L^p(X)$.

#### Proposition 4 {#ts-iii-s2-prop-4 .statement tag=02QT}

Soient $k\in \mathscr{N}^{p,q}(X\times Y)$ et $f\in \mathscr{L}^p(X)$. L’application définie sur X par $x\mapsto k(x, y)f(x)$ est $\mu$-intégrable pour tout $y$ en dehors d’un ensemble localement $\nu$-négligeable, et $u_k(f)$ coïncide avec la classe de la fonction

$$
y\mapsto \int_Xk(x, y)f(x)d\mu(x)
$$

définie localement $\nu$-presque partout.

Notons $Y'$ l’ensemble des $y\in Y$ tels que l’application $x\mapsto k(x, y)f(x)$ n’est pas $\mu$-intégrable. Soit $y\in Y$ et soit C un voisinage compact de $y$, dont on note $\varphi$ la fonction caractéristique. D’après la condition (2) appliquée à $f$ et $\varphi$, la fonction $(x, y)\mapsto k(x, y)f(x)\varphi (y)$ est intégrable sur $X\times Y$ par rapport à la mesure $\mu\otimes \nu$. D’après le théorème de Lebesgue–Fubini (INT, V, p. 96, § 8, n$^o4$, th. 1, a)), la fonction $x\mapsto k(x, y)f(x)\varphi (y)$ est $\mu$-intégrable pour $y$ en dehors d’un ensemble $\nu$-négligeable $Y_C$. Comme $Y'\cap C\subset Y_C$, on en déduit que $Y'$ est localement $\nu$-négligeable dans Y (INT, IV, p. 172, § 5, n$^o2$, déf. 3).

Notons $h$ l’application définie localement $\nu$-presque partout sur Y par $y\mapsto \int k(x, y)f(x)d\mu$. Elle est localement $\nu$-intégrable (INT, V, loc. cit.). Soit $g\in \mathscr{K}(Y)$. On a

$$
\langle g, u_k(f)\rangle =\int_{X\times Y}k(x, y)f(x)g(y)d(\mu\otimes \nu )(x, y)
$$

$$
=\int_Y\int_Xk(x, y)f(x)g(y)d\mu(x)d\nu (y)
$$

$$
=\int_Yg(y)h(y)d\nu (y)
$$

(INT, V, loc. cit.). On a donc $u_k(f) =h$ localement $\nu$-presque partout (cf. INT, V, p. 46, § 5, n$^o3$, cor. 2).

#### Proposition 5 {#ts-iii-s2-prop-5 .statement tag=02QU}

L’espace $\mathscr{L}^{p'}(X\times Y)$ est contenu dans $\mathscr{N}^{p,p}(X\times Y)$. L’application linéaire de $\mathscr{L}^{p'}(X\times Y)$ dans $\mathscr{L}(L^p(X); L^{p'}(Y))$ définie par $k\mapsto u_k$ induit par passage au quotient une application linéaire continue injective de $L^{p'}(X\times Y)$ dans $\mathscr{L}(L^p(X); L^{p'}(Y))$.

Soit $k\in \mathscr{L}^{p'}(X\times Y)$. L’application $k$ est mesurable (INT, IV, p. 84, § 5, n$^o6$, th. 5). Soient $f\in \mathscr{L}^p(X)$ et $g\in \mathscr{L}^p(Y)$. La fonction $h: (x, y)\mapsto f(x)g(y)$ appartient à $\mathscr{L}^p(X\times Y)$ et $\|h\|_p=\|f\|_p\|g\|_p$ (INT, V, p. 95, § 8, n$^o3$, cor. 2). La fonction $hk$ est donc intégrable sur $X\times Y$ et on a

$$
(\mu\otimes \nu )^*(|hk|)\leqslant \|k\|_{p'}\|h\|_p=\|k\|_{p'}\|f\|_p\|g\|_p
$$

d’après l’inégalité de Hölder (INT, IV, p. 208, § 6, n$^o4$, th. 2) ce qui démontre que $k\in \mathscr{N}^{p,p}(X\times Y)$ avec $\|k\|_{p,p}\leqslant \|k\|_{p'}$.

Puisque $p'\not = +\infty$, toute fonction $k\in \mathscr{L}^{p'}(X\times Y)$ est modérée (INT, V, p. 9, § 1, n$^o3$, cor.), et la dernière assertion résulte alors de la prop. 3, b) et c).

Pour toute fonction $k: X\times Y\rightarrow \mathbf{C}$ et pour tout $y\in Y$, on note $k_y$ l’application de X dans $\mathbf{C}$ donnée par $k_y(x) =k(x, y)$, et on note $k_{\circ}$ l’application de Y dans $\mathscr{F}(X;\mathbf{C})$ définie par $y\mapsto k_y$. On notera de même l’application de Y dans l’espace des fonctions définies $\mu$-presque partout sur X qui à $y$ associe la classe de $k_y$.

Pour toute fonction $k$ de $X\times Y$ dans $\mathbf{C}$, on note

$$
N_{p',q'}(k)=\left(\int_Y^\bullet N_{p'}(k_y)^{q'}d\nu(y)\right)^{1/q'}.
$$

C’est un élément de $[0,+\infty ]$.

#### Lemme 2 {#ts-iii-s2-lem-2 .statement tag=02QV}

Pour tout $k\in \mathscr{L}^{p'}(X\times Y)$, on a $N_{p', p'}(k) =\|k\|_{p'}$.

Soit $k\in \mathscr{L}^{p'}(X\times Y)$. D’après INT, V, p. 96, § 8, n$^o4$, th. 1, a), l’ensemble $Y'$ des éléments $y\in Y$ tels que la fonction $|k_y|^{p'}$ ne soit pas $\mu$-intégrable est $\nu$-négligeable ; de plus, la fonction définie par $y\mapsto \mu(|k_y|^{p'})$ sur Y - $Y'$ et nulle sur $Y'$ est $\nu$-intégrable et vérifie

$$
\|k\|^p_{p''}=\int_{X\times Y}|k(x, y)|^{p'}d(\mu\otimes \nu )(x, y) =\int_Y\mu(|k_y|^{p'})d\nu = N_{p', p'}(k)^{p'}
$$

On note $\mathscr{L}^{p',q'}(X,Y, \mu, \nu )$, ou simplement $\mathscr{L}^{p',q'}(X,Y)$, l’espace vectoriel complexe des fonctions $(\mu\otimes \nu$)-mesurables $k$ de $X\times Y$ dans $\mathbf{C}$ telles que, pour $\nu$-presque tout $y\in Y$, l’application $k_y$ appartient à $\mathscr{L}^{p'}$(X), et telles que l’application $k_{\circ}$ appartient à $\mathscr{L}_L^{q'_{p'}}_{(X)}(Y, \nu )$ (INT, IV, p. 129, § 3, n$^o4$, déf. 2). On munit $\mathscr{L}^{p',q'}(X,Y)$ de la semi-norme $k\mapsto N_{p',q'}(k)$; notons que celle-ci vérifie alors $N_{p',q'}(k) =\|k_{\circ}\|_{q'}$, où $k_{\circ}$ est vue comme application à valeurs dans l’espace de Banach $L^{p'}(X)$.

#### Proposition 6 {#ts-iii-s2-prop-6 .statement tag=02QW}

a) L’espace $\mathscr{L}^{p'}(X\times Y)$ est contenu dans $\mathscr{L}^{p',p'}(X,Y)$ et pour $k\in \mathscr{L}^{p'}(X\times Y)$, on a $N_{p', p'}(k) =\|k\|_{p'}$;

b) L’espace $\mathscr{L}^{p',q'}(X,Y)$ est contenu dans $\mathscr{N}^{p,q}(X\times Y)$ et pour $k\in \mathscr{L}^{p',q'}(X,Y)$, on a $\|k\|_{p,q}\leqslant N_{p',q'}(k)$.

Démontrons l’assertion a). Soit $k\in \mathscr{L}^{p'}(X\times Y)$. D’après INT, V, p. 96, § 8, n$^o4$, th. 1, a), la fonction $k_y$ appartient à $\mathscr{L}^{p'}(X)$ pour $\nu$-presque tout $y\in Y$.

Soit $\varepsilon  >0$. Il existe $h\in \mathscr{K}(X\times Y)$ telle que $\|k-h\|_{p'}< \varepsilon$. La fonction $h_{\circ}$ est une fonction continue à support compact de Y dans $L^{p'}(X)$ qui vérifie

$$
\|k_{\circ}-h_{\circ}\|_{p'}= N_{p',p'}(k-h) =\|k-h\|_{p'}< \varepsilon
$$

d’après le lemme 2. Il en résulte que $k_{\circ}$ appartient à $\mathscr{L}_L^{p'_{p'}}_{(X)}(Y, \nu )$, c’est-à-dire que $k$ appartient à $\mathscr{L}^{p',p}(X,Y)$. Le lemme 2 démontre alors que $N_{p', p'}(k) =\|k\|_{p'}$.

Démontrons l’assertion b). Soit $k\in \mathscr{L}^{p',q'}(X,Y)$ et soit $f\in \mathscr{L}^p(X)$. Pour tout $y\in Y$, l’inégalité de Hölder (INT, IV, p. 208, § 6, n$^o4$, th. 2) appliquée à $k_y$ implique

$$
\int_X^*|k(x, y)f(x)|d\mu(x)\leqslant \|k_y\|_{p'}\|f\|_p
$$

Soit $g\in \mathscr{L}^{q'}(Y)$. Les applications $f$ et $g$ sont modérées, puisque $p$ et $q'$ sont finis. Par conséquent, l’application $(x, y)\mapsto f(x)g(y)$ est $(\mu\otimes \nu )$-modérée (cf. INT, V, p. 92, § 8, n$^o3$, cor. 2), et donc l’application $(x, y)\mapsto k(x, y)f(x)g(y)$ est $(\mu\otimes \nu$)-modérée. D’après INT, V, p. 93, § 8, n$^o3$, prop. 7, a), il vient alors

$$
\int_{X\times Y}^*|k(x, y)f(x)g(y)|d(\mu\otimes \nu )
$$

$$
=\int_Y^*|g(y)|\int_X^*|k(x, y)f(x)|d\mu(x)d\nu (y)
$$

$$
\leqslant \|f\|_p\int_Y^*\|k_y\|_{p'}|g(y)|d\nu (y)\leqslant N_{p',q'}(k)\|f\|_p\|g\|_q
$$

en utilisant de nouveau l’inégalité de Hölder. Cela conclut la démonstration.

#### Proposition 7 {#ts-iii-s2-prop-7 .statement tag=02QX}

Soit $k\in \mathscr{L}^{p',q'}(X,Y)$. L’application linéaire $u_k$ de $L^p(X)$ dans $L^{q'}(Y)$ est compacte.

Supposons d’abord que $k$ est tel que $k_{\circ}\in \mathscr{K}(Y;\mathscr{L}^{p'}$(X)), et notons A le support de $k_{\circ}$. Soit F le sous-espace de $\mathscr{K}(Y,A;\mathscr{L}^{p'}(X, \mu))$ engendré par les fonctions $y\mapsto f_2(y)f_1$, où $f_2\in \mathscr{K}(Y,A)$ et $f_1\in \mathscr{L}^{p'}(X)$. Lorsque $m\in \mathscr{K}(Y;\mathscr{L}^{p'}(X))$ vérifie $m_{\circ}\in F$, l’application linéaire $u_m$ est de rang fini, donc compacte. Pour $m_1$ et $m_2$ dans $\mathscr{K}(Y,A;\mathscr{L}^{p'}$(X)), on a de plus

$\int'1/q'$

$$
\|u_{m_1}-u_{m_2}\|\leqslant \|m_1-m_2\|_{p',q'}=_Y\|m_{1,y}-m_{2,y}\|^q_{p'}d\nu (y)
$$

$\leqslant \nu (A)^{1/q'}$ sup$_{y\in Y}N_{p'}(m_{1,y}-m_{2,y})$.

Comme l’espace F est dense dans $\mathscr{K}(Y,A; L^{p'}(X))$ pour la topologie de la convergence uniforme dans A (INT, III, p. 41, § 1, n$^o1$, prop. 1 et INT, III, p. 46, § 1, n$^o2$, prop. 5), on conclut que l’application linéaire $u_k$ est limite d’une suite d’applications linéaires de rang fini. Elle est donc compacte (cor. 1 de III, p. 4).

Considérons le cas général. Soit $k\in \mathscr{L}^{p',q'}(X,Y)$. Pour tout $\varepsilon  >0$, il existe une application $k_{\varepsilon ,\circ}\in \mathscr{K}(Y;\mathscr{L}^{p'}(X))$ telle que

$$
\|k_{\circ}-k_{\varepsilon ,\circ}\|_{q'}< \varepsilon
$$

La fonction $k_{\varepsilon}: X\times Y\rightarrow \mathbf{C}$ correspondante vérifie alors

$$
\|u_k-u_{k_{\varepsilon}}\|\leqslant \|k-k_{\varepsilon}\|_{p,q}\leqslant N_{p',q'}(k-k_{\varepsilon}) =\|k_{\circ}-k_{\varepsilon ,\circ}\|_{q'}< \varepsilon
$$

Puisque $u_{k_{\varepsilon}}$ est compacte d’après ce qui précède, l’application $u_k$ est également compacte (prop. 2 de III, p. 4).

Posons $p= 1$ et supposons $q >1$. Il peut exister des applications $k: X\times Y\rightarrow \mathbf{C}$ telles que $k_y\in \mathscr{L}^{\infty}(X)$ pour tout $y\in Y$, et telles que l’intégrale

$$
\int_Y^*\|k_y\|^q_{\infty'}d\nu (y)
$$

soit finie (en particulier, la condition (2) de III, p. 27 est valide), mais telles que l’application linéaire $u_k$ de $L^1(X)$ dans $L^{q'}(X)$ ne soit pas compacte (exercice 2 de III, p. 119).

En particulier, on déduit de la proposition le corollaire suivant :

#### Corollaire 1 (Hilbert–Schmidt) {#ts-iii-s2-prop-7-cor-1 .statement tag=02QY}

Soit $k\in \mathscr{L}^2(X\times Y)$. L’application linéaire $u_k$ est compacte de $L^2(X)$ dans $L^2(Y)$.

D’après la prop. 5, on a $k\in \mathscr{N}^{2,2}(X\times Y)$, donc l’application linéaire $u_k$ est définie (prop. 3). On a $k\in \mathscr{L}^{2,2}(X\times Y)$ (prop. 6, a)), donc $u_k$ est compacte (prop. 7).

#### Remarque {#ts-iii-s2-n4-rem-2 .statement tag=02QZ}

Dans le cas $p=q= 2$, il est généralement plus commode d’exprimer la caractérisation de l’opérateur intégral $u_k$ à l’aide du produit scalaire : il s’agit de l’unique application de $L^2(X)$ dans $L^2(Y)$ telle que

$$
\langle g|u_k(f)\rangle =\int_{X\times Y}k(x, y)f(x)\overline{g(y)}d(\mu\otimes \nu )(x, y)
$$

pour tous $f\in L^2(X)$ et $g\in L^2(Y)$. De plus, l’adjoint de $u_k$ est l’application linéaire $u_{k^*}$, où $k^*\in L^2(Y\times X)$ vérifie $k^*(y, x) =k(x, y)$ pour presque tout $(y, x)\in Y\times X$. En effet, pour tous $f\in L^2(X)$ et $g\in L^2$(Y), on a

$$
\langle g|u_k(f)\rangle =\int_{X\times Y}k(x, y)\overline{g(y)}f(x)d(\mu\otimes \nu )(x, y) =\langle u_{k^*}(g)|f\rangle
$$

#### Corollaire 2 {#ts-iii-s2-prop-7-cor-2 .statement tag=02R0}

Soit G un groupe topologique compact muni d’une mesure de Haar $\mu$. Soit $p$ un nombre réel tel que $1< p <+\infty$ et $q$ l’exposant conjugué de $p$. Soit $f\in \mathscr{L}^q(G)$. Posons $k(x, y) =f(x^{-1}y)$ pour tous $(x, y)\in G\times G$.

a) On a $k\in \mathscr{L}^{q,p}(G,G)$;

b) Pour $\varphi \in L^p(G)$, la convolution $\varphi *f$ appartient à $L^p(G)$ et l’application linéaire $v_f:\varphi \mapsto \varphi *f$ de $L^p(G)$ dans lui-même est continue. Elle coïncide avec l’endomorphisme $u_k$. En particulier, l’application linéaire $v_f$ est compacte.

Puisque G est compact, la fonction $f$ appartient à $\mathscr{L}^1(G)$. L’application linéaire $v_f$ est donc définie et continue d’après INT, VIII, p. 167, § 4, n$^o5$, prop. 13.

L’application $k$ est $(\mu\otimes \mu$)-mesurable, et on a $\|k_y\|_q=\|f\|_q$ pour tout $y\in G$. Comme la mesure $\mu$ est bornée, il vient

$$
\int_G\|k_y\|^p_qd\mu(y) =\mu(G)\|f\|^p_q
$$

donc $k\in \mathscr{L}^{q,p}(G,G)$. L’application linéaire $u_k$ est donc une application linéaire compacte de $L^p(G)$ dans $L^p(G)$ (prop. 7).

Soit $\varphi \in \mathscr{K}(G)$. D’après INT, VIII, p. 166, § 4, n$^o5$, prop. 11 et la prop. 4 de III, p. 29, on a alors

$$
v_f(\varphi )(y) =\int_G\varphi (x)f(x^{-1}y)d\mu(x)
$$

$$
=\int_G\varphi (x)k(x, y)d\mu(x) =u_k(\varphi )(y)
$$

pour presque tout $y\in G$. Cela implique que $v_f=u_k$.

### 5. Restriction d’applications différentiables

Soient $n$ et $r$ des entiers positifs, U une partie ouverte de $\mathbf{R}^n$ et F un espace de Banach. Notons $\mathscr{C}^r(U; F)$ l’espace vectoriel des applications de classe $C^r$ de U dans F, muni de la topologie de la $C^r$-convergence compacte. Rappelons que celle-ci est la borne supérieure des topologies de la $C^r$-convergence uniforme sur K (VAR, R2, 12.3.10, p. 56), lorsque K décrit l’ensemble des parties compactes de U. L’espace $\mathscr{C}^0(U; F)$ n’est autre que l’espace $\mathscr{C}(U; F)$ des applications continues de U dans F, muni de la topologie de la convergence compacte.

#### Lemme 3 {#ts-iii-s2-lem-3 .statement tag=02R1}

Soit A l’ensemble des multi-indices $\alpha \in \mathbf{N}^n$ tels que $|\alpha |\leqslant r$ et soit $u$ l’application linéaire $f\mapsto (\partial^{\alpha}f)_{\alpha\in A}$ de $\mathscr{C}^r(U; F)$ dans $\mathscr{C}(U; F)^A$.

a) L’application $u$ est injective, continue, stricte et son image est fermée.

b) L’espace vectoriel topologique $\mathscr{C}^r(U; F)$ est complet.

L’application $u$ est linéaire et injective. Elle est continue et stricte par définition de la topologie de $\mathscr{C}^r(U; F)$.

Soit $(g_{\alpha})_{\alpha\in A}$ un point de $\mathscr{C}(U; F)^A$ adhérent à l’image de $u$. Il existe un filtre $\mathfrak{F}$ sur $\mathscr{C}^r(U; F)$ tel que l’on ait $g_{\alpha}=$ lim$_{f,\mathscr{F}}\partial^{\alpha}f$ dans $\mathscr{C}(U; F)$ pour tout $\alpha \in A$. Soit $m$ un entier tel que $0\leqslant m\leqslant r$. En raisonnant par récurrence sur $m$, on déduit du th. 1 de FVR, II, p. 2, que l’application $g_0$ est de classe $C^m$ et que l’on a $g_{\alpha}=\partial^{\alpha}g_0$ pour tout $\alpha \in \mathbf{N}^n$ avec $|\alpha |\leqslant m$. Ainsi $g_0$ appartient à l’espace $\mathscr{C}^r(U; F)$ et son image par $u$ est $(g_{\alpha})_{\alpha\in A}$. Cela démontre que l’image de $u$ est fermée, et établit donc l’assertion a).

L’assertion a) implique que l’espace $\mathscr{C}^r(U; F)$ est isomorphe à son image dans $\mathscr{C}(U; F)^A$; puisque cette image est fermée et que l’espace $\mathscr{C}(U; F)^A$ est complet (TG, X, p. 9, cor. 3 du th. 2 et TG, II, p. 17, prop. 10), l’espace $\mathscr{C}^r(U; F)$ est complet.

#### Proposition 8 {#ts-iii-s2-prop-8 .statement tag=02R2}

Supposons que F est de dimension finie. Soient $s$ un entier tel que $0\leqslant s < r$ et V une partie ouverte relativement compacte de U. L’application linéaire $f\mapsto f|V$ de $\mathscr{C}^r(U; F)$ dans $\mathscr{C}^s(V; F)$ est compacte.

Soit W l’ensemble des fonctions $f\in \mathscr{C}^r(U; F)$ dont les dérivées partielles d’ordre $\leqslant r$ prennent en tout point de V une valeur de norme inférieure à 1. L’ensemble W est un voisinage de 0 dans l’espace $\mathscr{C}^r(U; F)$. Soit $\alpha$ un multi-indice tel que $|\alpha |\leqslant s$. Considérons l’ensemble H des fonctions de la forme $(\partial^{\alpha}f)|V$ pour $f$ dans W. L’ensemble H est une partie équicontinue de $\mathscr{C}(V; F)$ (TG, X, p. 10) d’après le théorème des accroissements finis (VAR, R, 2.2.3). Par ailleurs, pour tout $x\in V$, l’image de H par l’application $g\mapsto g(x)$ est une partie bornée, donc relativement compacte, de F. D’après le théorème d’Ascoli (TG, X, p. 18, cor. 2), l’ensemble H est relativement compact dans $\mathscr{C}(V; F)$. Cela démontre que l’application linéaire $f\mapsto (\partial^{\alpha}f)|V$ de $\mathscr{C}^r(U; F)$ dans $\mathscr{C}(V; F)$ est compacte. La proposition résulte alors du lemme 3 et des remarques 5 et 6 de III, p. 3.

### 6. Restriction de sections différentiables d’un fibré vectoriel

Soient $r$ un entier positif, X une variété différentielle de classe $C^r$ localement de dimension finie et E un fibré vectoriel (réel ou complexe) de base X et de classe $C^r$. Pour tout ouvert U de X, notons $\mathscr{S}^r(U; E)$ l’espace vectoriel (noté $\mathscr{S}_E^r(U)$ dans VAR, R1, 7.4, p. 74) des sections de classe $C^r$ de E au-dessus de U, muni de la topologie de la $C^r$-convergence compacte.

#### Lemme 4 {#ts-iii-s2-lem-4 .statement tag=02R3}

Soit $\mathscr{U}$ un recouvrement ouvert de X. L’application $u:f\mapsto (f|U)_{U\in\mathscr{U}}$ de $\mathscr{S}^r(X; E)$ dans $\prod_{U\in\mathscr{U}}\mathscr{S}^r(U; E)$ est linéaire, injective, continue et stricte. Son image est fermée.

L’application $u$ est linéaire, injective et continue. En vertu de TG, IX, p. 43, prop. 1 et p. 48, cor. 1, toute partie compacte de X possède un recouvrement fini $(C_i)_{i\in I}$ où, pour chaque $i\in I$, l’ensemble $C_i$ est une partie compacte de l’un des ouverts du recouvrement $\mathscr{U}$. Il en résulte que l’application linéaire $u$ est stricte. Enfin, son image est fermée, puisque elle est constituée des familles $(f_U)_{U\in\mathscr{U}}$ telles que $f_U$ et $f_V$ coïncident dans $U\cap V$ pour tous U et V dans $\mathscr{U}$.

#### Proposition 9 {#ts-iii-s2-prop-9 .statement tag=02R4}

L’espace $\mathscr{S}^r(X; E)$ est complet.

Supposons d’abord qu’il existe un entier $n\geqslant 0$ et un espace de Banach F tels que X soit une partie ouverte de $\mathbf{R}^n$ et E le fibré vectoriel trivial $X\times F$ de base X et de fibre F. Dans ce cas, l’espace vectoriel topologique $\mathscr{S}^r(X; E)$ est isomorphe à $\mathscr{C}^r(X; F)$, et le résultat découle du lemme 3 de III, p. 34.

Dans le cas général, soit $\mathscr{U}$ un recouvrement ouvert de X par des domaines de cartes tel que pour tout $U\in \mathscr{U}$, la restriction de E à U est trivialisable. D’après le lemme ci-dessus, l’espace $\mathscr{S}^r(X; E)$ est isomorphe à l’image de l’application linéaire $f\mapsto (f|U)_{U\in\mathscr{U}}$, qui est fermée dans le produit des espaces $\mathscr{S}^r(U; E)$ pour U dans $\mathscr{U}$. D’après le cas précédent, chacun des espaces $\mathscr{S}^r(U; E)$ est complet, donc leur produit est complet (TG, II, p. 17, prop. 10). Par conséquent $\mathscr{S}^r(X; E)$ est complet.

#### Remarque {#ts-iii-s2-n6-rem-1 .statement tag=02R5}

Soit $\mathscr{U}$ un recouvrement ouvert de X par des domaines de cartes $c_U= (U, \varphi_U,\mathbf{R}^{n_U})$ tel que pour tout $U\in \mathscr{U}$, la restriction de E à U est trivialisable de type $F_U$, où $F_U$ est un espace de Banach. Pour tout $U\in \mathscr{U}$, on identifie une section $f$ de E sur U à une application $f_U$ de $\varphi_U(U)$ dans $F_U$. Il résulte de la preuve de la prop. 9 que la topologie de l’espace $\mathscr{S}^r(X; E)$ est définie par la famille des semi-normes $p_{U,C,\alpha}$ telles que

$p_{U,C,\alpha}(f) =$ sup $\|(\partial^{\alpha}f_U)(x)\|$,

$x\in C$ où U parcourt $\mathscr{U}, C$ parcourt l’ensemble des parties compactes de $\varphi_U(U)$ et $\alpha \in \mathbf{N}^{n_U}$ l’ensemble des multi-indices tels que $|\alpha |\leqslant r$.

#### Proposition 10 {#ts-iii-s2-prop-10 .statement tag=02R6}

Supposons que le fibré vectoriel E soit localement de rang fini. Soient $s$ un entier tel que $0\leqslant s < r$ et Y une partie ouverte relativement compacte de X. L’application linéaire $f\mapsto f|Y$ de $\mathscr{S}^r(X; E)$ dans $\mathscr{S}^s(Y; E)$ est compacte.

Supposons d’abord qu’il existe un entier $n\geqslant 0$ et un espace de Banach F de dimension finie tels que X soit une partie ouverte de $\mathbf{R}^n$ et E le fibré vectoriel trivial $X\times F$ de base X et de fibre F. Dans ce cas, les espaces vectoriels topologiques $\mathscr{S}^r(X; E)$ et $\mathscr{S}^s(Y; E)$ sont isomorphes à $\mathscr{C}^r(X; F)$ et $\mathscr{C}^s(Y; F)$, respectivement, et la prop. 10 est conséquence de la prop. 8.

Passons au cas général. Soit C une partie compacte de X contenant Y. Pour tout point $x$ de C, choisissons un voisinage ouvert $U(x)$ de $x$ dans X qui soit un domaine de carte au-dessus duquel le fibré vectoriel E est trivialisable. Choisissons par ailleurs un voisinage ouvert relativement compact $V(x)$ de $x$ dans $U(x)$. Comme l’ensemble C est compact, il est recouvert par une famille finie $(V(x_1), . . . ,V(x_m))$ de tels ouverts. Pour tout $i$, posons $U_i= U(x_i)$ et $Y_i= V(x_i)\cap Y$. Alors $Y_i$ est une partie ouverte relativement compacte de $U_i$ et l’on a $Y = Y_1\cup  \cdots  \cup Y_m$. Les applications linéaires $f\mapsto f|U_i$ de $\mathscr{S}^r(X; E)$ dans $\mathscr{S}^r(U_i; E)$ sont continues et les applications linéaires $g\mapsto g|Y_i$ de $\mathscr{S}^r(U_i; E)$ dans $\mathscr{S}^s(Y_i; E)$ sont compactes d’après la première partie de la démonstration. Les applications linéaires $f\mapsto f|Y_i$ de $\mathscr{S}^r(X; E)$ dans $\mathscr{S}^s(Y_i; E)$ sont donc compactes (prop. 3 de III, p. 5). Compte tenu du lemme 4, appliqué au recouvrement de Y par les ouverts $Y_i$, et des remarques 5 et 6 de III, p. 3, l’application linéaire $f\mapsto f|Y$ de $\mathscr{S}^r(X; E)$ dans $\mathscr{S}^s(Y; E)$ est compacte, ce qui termine la démonstration.

### 7. Restriction de sections analytiques d’un fibré vectoriel

Soient X une variété analytique complexe localement de dimension finie et E un fibré vectoriel analytique de base X (VAR, p. 35 et VAR, p. 70). Notons $\mathscr{S}^{\omega}(X; E)$ l’espace vectoriel des sections analytiques de E sur X, muni de la topologie de la convergence compacte.

#### Lemme 5 {#ts-iii-s2-lem-5 .statement tag=02R7}

Soient $X_0$ la variété analytique réelle sous-jacente à X et $E_0$ le fibré vectoriel complexe sur $X_0$ sous-jacent à E.

a) Le sous-espace vectoriel $\mathscr{S}^{\omega}(X; E)$ de $\mathscr{S}^0(X_0; E_0)$ est fermé, et l’injection de $\mathscr{S}^{\omega}(X; E)$ dans $\mathscr{S}^0(X_0; E_0)$ est continue et stricte ;

b) L’injection canonique de $\mathscr{S}^{\omega}(X; E)$ dans $\mathscr{S}^1(X_0; E_0)$ est continue.

Supposons d’abord qu’il existe un entier $n\geqslant 0$ et un espace de Banach F tels que X soit un ouvert de $\mathbf{C}^n$ et E le fibré vectoriel trivial $X\times F$. Dans ce cas, les espaces vectoriels topologiques $\mathscr{S}^{\omega}(X; E)$, $\mathscr{S}^0(X_0; E_0)$ et $\mathscr{S}^1(X_0; E_0)$ sont isomorphes à $\mathscr{C}^{\omega}(X; F),\mathscr{C}^0(X_0; F)$ et $\mathscr{C}^1(X_0; F)$ respectivement, et l’espace $\mathscr{S}^0(X_0; E_0)$ est métrisable (TG, X, p. 20, cor. de la prop. 1). Le lemme résulte alors de VAR, 3.3.2, p. 28.

Passons au cas général. Soit $\mathfrak{F}$ un filtre sur $\mathscr{S}^{\omega}(X; E)$ qui converge dans l’espace $\mathscr{S}^0(X_0; E_0)$ vers une limite $f$. Il s’agit de démontrer que $f$ appartient à $\mathscr{S}^{\omega}(X; E)$ et que le filtre $\mathfrak{F}$ converge vers $f$ dans l’espace $\mathscr{S}^1(X_0; E_0)$. Cet énoncé est de nature locale, donc résulte de la première partie de la démonstration.

#### Proposition 11 {#ts-iii-s2-prop-11 .statement tag=02R8}

Supposons que le fibré vectoriel E soit localement de rang fini. Soit Y une partie ouverte relativement compacte de X. L’application de restriction $f\mapsto f|Y$ de $\mathscr{S}^{\omega}(X; E)$ dans $\mathscr{S}^{\omega}(Y; E)$ est compacte.

Avec les notations du lemme 5, on a un diagramme commutatif

$$
\mathscr{S}^{\omega}(X; E)\leftarrow^i\rightarrow \mathscr{S}^1(X_0; E_0)
$$

$$
\rightarrow \leftarrow_u\rightarrow \leftarrow_v \tag{3}
$$

$$
\mathscr{S}^{\omega}(Y; E)\leftarrow^j\rightarrow \mathscr{S}^0(Y_0; E_0)
$$

où $i$ et $j$ sont les injections canoniques et $u,v$ les applications de restriction. L’application $i$ est continue (lemme 5, b)), et l’application $u$ est compacte (prop. 10). Comme l’injection canonique $j$ est continue, stricte et d’image fermée (lemme 5, a)), l’application $u$ est compacte (remarque 5 de III, p. 3).

#### Corollaire {#ts-iii-s2-n7-cor-1 .statement tag=02R9}

Soient X une variété analytique complexe compacte et E un fibré vectoriel analytique de base X, localement de rang fini. L’espace vectoriel $\mathscr{S}^{\omega}(X; E)$ est de dimension finie.

Étant compacte, la variété analytique X est localement de dimension finie. D’après la prop. 11, l’application identique de $\mathscr{S}^{\omega}(X; E)$ est une application linéaire compacte. Cela implique que l’espace $\mathscr{S}^{\omega}(X; E)$ est de dimension finie (remarque 3 de III, p. 2).

## EXERCICES {#ts-iii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
