---
book: ts
book_title: Théories spectrales
chapter: IV
chapter_title: THÉORIE SPECTRALE HILBERTIENNE
section: 1
section_title: Opérateurs compacts sur un espace hilbertien
lang: fr
source: ts-iii-v-fr
book_pages: TS IV.146-TS IV.179, TS IV.313-TS IV.319
pdf_pages: 0159-0192, 0326-0332
extraction: native
subsections:
    - "no": 1
      title: Endomorphismes diagonaux
      page: 146
      pdf_page: 159
    - "no": 2
      title: Diagonalisation des endomorphismes compacts
      page: 149
      pdf_page: 162
    - "no": 3
      title: Suite décroissante des valeurs propres
      page: 151
      pdf_page: 164
    - "no": 4
      title: Caractérisations variationnelles des valeurs propres
      page: 153
      pdf_page: 166
    - "no": 5
      title: Applications de la caractérisation variationnelle des valeurs propres
      page: 155
      pdf_page: 168
    - "no": 6
      title: Inégalités de Weyl
      page: 157
      pdf_page: 170
    - "no": 7
      title: Endomorphismes de trace finie
      page: 164
      pdf_page: 177
    - "no": 8
      title: Applications nucléaires
      page: 167
      pdf_page: 180
    - "no": 9
      title: Opérateurs intégraux de Hilbert–Schmidt
      page: 172
      pdf_page: 185
    - "no": 10
      title: Trace des opérateurs intégraux à noyau continu
      page: 174
      pdf_page: 187
statements: 66
exercises: 22
content_sha256: 4db5f659f6f30649155bfba69f064247a3715361301acd1965247c33dfa2869f
---

## § 1. OPÉRATEURS COMPACTS SUR UN ESPACE HILBERTIEN

Dans ce paragraphe, K est un corps égal à $\mathbf{R}$ ou $\mathbf{C}$ et E désigne un espace hilbertien sur le corps K.

### 1. Endomorphismes diagonaux

#### Définition 1 {#ts-iv-s1-def-1 .statement tag=02W8}

Soit $B = (e_i)_{i\in I}$ une base orthonormale de E. Un endomorphisme $u$ est dit diagonal dans la base B ou diagonal relativement à B s’il existe une famille $\lambda = (\lambda_i)_{i\in I}$ d’éléments de K tels que $u(e_i) =\lambda_ie_i$ pour tout $i\in I$.

Soit $B = (e_i)_{i\in I}$ une base orthonormale de E. On note $\mathscr{D}_B(E)$ l’ensemble des endomorphismes de E qui sont diagonaux relativement à B. C’est une sous-algèbre commutative unifère fermée de $\mathscr{L}(E)$. Soit $u\in \mathscr{D}_B(E)$. La famille $\lambda = (\lambda_i)_{i\in I}$ telle que $u(e_i) =\lambda_ie_i$ est déterminée de manière unique par $u$ et par la base B, et on dit que c’est la famille des valeurs propres de $u$ relativement à B.

Supposons que $K =\mathbf{R}$ et identifions E à un sous-espace de $E_{(\mathbf{C})}$. Soit $B = (e_i)_{i\in I}$ une base orthonormée de E. Notons $B_{(\mathbf{C})}$ la base orthonormée $(1\otimes e_i)_{i\in I}$ de $E_{(\mathbf{C})}($cf. EVT, V, p. 29, cor. 1). L’application $u\mapsto u_{(\mathbf{C})}$ induit un morphisme injectif d’algèbres de $\mathscr{D}_B(E)$ dans $\mathscr{D}_{B_{(\mathbf{C})}}(E_{(\mathbf{C})})$; son image est l’ensemble des $u\in \mathscr{D}_{B_{(\mathbf{C})}}(E_{(\mathbf{C})})$ tel que $u(E)\subset E$, autrement dit l’ensemble des $u$ diagonaux dans la base $B_{(\mathbf{C})}$ dont les valeurs propres sont réelles.

Pour tout $i\in I$, on note $p_i$ l’orthoprojecteur de E d’image $Ke_i$. On a $\|p_i\|= 1$ pour tout $i\in I$. L’endomorphisme $p_i$ est diagonal dans la base B, la famille de ses valeurs propres est la famille $(\delta_{ij})_{j\in I}$ (symbole de Kronecker, cf. A, II, p. 24).

Soit $B'= (f_i)_{i\in I}$ une base orthonormale de E et $u: E\rightarrow E$ l’isomorphisme isométrique tel que $u(f_i) =e_i$. Alors $\mathscr{D}_{B'}(E) =u^{-1}\mathscr{D}_B(E)u$.

On munit I de la topologie discrète et on note $\mathscr{B}(I) =\mathscr{C}_b(I; K)$ l’algèbre de Banach unifère des fonctions bornées sur I à valeurs dans K (exemple 2 de I, p. 17) ; si $K =\mathbf{C}$, c’est une algèbre stellaire (exemple 2 de I, p. 102).

#### Lemme 1 {#ts-iv-s1-lem-1 .statement tag=02W9}

Soit $u\in \mathscr{D}_B(E)$ et $\lambda = (\lambda_i)_{i\in I}$ la famille de ses valeurs propres. La famille $\lambda$ est bornée et l’on a sup$_i|\lambda_i|=\|u\|$.

On a $|\lambda_i|\leqslant \|u\|$ pour tout $i$, d’où sup$_{i\in I}|\lambda_i|\leqslant \|u\|$. Comme de plus

$\|u(x)\|^2=\sum_{i\in I}|\lambda_i|^2|\langle e_i|x\rangle |^2\leqslant$ sup$_{i\in I}|\lambda_i|^2\|x\|^2$

pour tout $x\in E$ (EVT, V, p. 22, prop. 5), il vient $\|u\|=$ sup$|\lambda_i|$.

#### Proposition 1 {#ts-iv-s1-prop-1 .statement tag=02WA}

a) L’application $\alpha$ de $\mathscr{D}_B(E)$ dans $\mathscr{B}(I)$ qui à un endomorphisme diagonal $u$ associe la famille des valeurs propres de $u$ est un isomorphisme isométrique d’algèbres de Banach sur K. Si $K =\mathbf{C}$, c’est un morphisme d’algèbres involutives ;

b) Pour toute famille bornée $\lambda = (\lambda_i)_{i\in I}$, la famille $(\lambda_ip_i)_{i\in I}$ est sommable dans l’espace $\mathscr{L}(E)$ muni de la topologie de la convergence simple, et la somme de cette famille est l’unique application $u\in \mathscr{D}_B(E)$ telle que $\alpha (u) =\lambda$;

c) Soit $u\in \mathscr{D}_B(E)$ et soit $\lambda$ la famille de ses valeurs propres relativement à B. Le spectre de $u$ est l’adhérence dans K de l’ensemble des valeurs de $\lambda$;

d) Si K = $\mathbf{C}$, alors l’application de calcul fonctionnel continu de $\mathscr{C}$ (Sp($u$)) dans $\mathscr{L}(E)$ associe à une fonction continue $f\in \mathscr{C}$ (Sp($u$)) l’endomorphisme $\alpha (f\circ \lambda )$ dans $\mathscr{D}_B(E)$.

D’après le lemme 1, la famille des valeurs propres d’un endomorphisme diagonal dans B est bornée et l’application de $\mathscr{D}_B(E)$ dans $\mathscr{B}(I)$ ainsi définie est un morphisme continu isométrique d’algèbres de Banach unifères.

Soit $i\in I$. Pour tout $j\in I$, on a $\langle u^*(e_i)|e_j\rangle =\lambda_j\langle e_i|e_j\rangle =\langle \overline{\lambda_j}e_i|e_j\rangle$. Il en résulte que $u^*(e_i) =\overline{\lambda}_ie_i$. L’adjoint de $u$ est donc l’endomorphisme diagonal dans la base B dont $(\lambda_i)_{i\in I}$ est la famille des valeurs propres. L’assertion a) en résulte.

Soit $\lambda = (\lambda_i)_{i\in I}\in \mathscr{B}(I)$. Pour tout $x\in E$, la famille $(|\langle e_i|x\rangle |^2)_{i\in I}$ est sommable, de somme $\|x\|^2$ (EVT, V, p. 22, prop. 5), d’où, pour tout sous-ensemble fini J de I :

$\sum_{i\in J}\lambda_ip_i(x)^2=\sum_{i\in J}|\lambda_i|^2|\langle e_i|x\rangle |^2\leqslant$ sup$_{i\in I}|\lambda_i|^2(\sum_{j\in J}|\langle e_i|x\rangle |^2$

$\leqslant$ sup$_{i\in I}|\lambda_i|^2\|x\|^2$.

Par conséquent, la famille $(\lambda_ip_i)$ est sommable dans $\mathscr{L}(E)$ muni de la topologie de la convergence simple. Sa somme $u_{\lambda}$ vérifie $u_{\lambda}(e_i) =\lambda_ie_i$; c’est donc un endomorphisme diagonal dans la base B, de valeurs propres $\lambda$. L’assertion b) en résulte.

Les dernières assertions résultent de a), de l’exemple 3 de I, p. 17 et de l’exemple 4 de I, p. 111.

#### Remarque {#ts-iv-s1-n1-rem-1 .statement tag=02WB}

L’algèbre de Banach $\mathscr{D}_B(E)$ est une sous-algèbre fermée commutative maximale de $\mathscr{L}(E)$. En effet, soit $u$ un endomorphisme de E qui commute avec $\mathscr{D}_B(E)$. Soit $i\in I$. Comme le projecteur orthogonal $p_i$ est diagonal dans la base B, on a $p_i(u(e_i)) =u(p_i(e_i)) =u(e_i)$, ce qui implique que $u(e_i)$ est proportionnel à $e_i$. Ainsi $u$ est diagonal dans la base B.

Si E est de dimension infinie, il existe des sous-algèbres involutives commutatives maximales de $\mathscr{L}(E)$ qui ne sont pas isomorphes à $\mathscr{D}_B(E)$ (exercice 5 de IV, p. 314).

#### Proposition 2 {#ts-iv-s1-prop-2 .statement tag=02WC}

Soient $u\in \mathscr{D}_B(E)$ et $\lambda = (\lambda_i)_{i\in I}$ la famille de ses valeurs propres.

a) Les conditions suivantes sont équivalentes:

(i) On a $\lambda \in \mathscr{C}_0(I; K)$;

(ii) L’endomorphisme $u$ est compact ;

(iii) La famille $(\lambda_ip_i)_{i\in I}$ est sommable dans l’espace de Banach

$\mathscr{L}(E)$. Sa somme est alors égale à $u$.

b) Supposons que $u$ est compact et notons Λ l’ensemble des valeurs de $\lambda$. L’ensemble des $i\in I$ tels que $\lambda_i\not = 0$ est dénombrable. Si E est de dimension infinie, on a Sp$_s(u) = \Lambda -\{0\}$ et Sp($u$) $= \Lambda \cup  \{0\}$. Si E est de dimension finie, alors Sp$_s(u) =$ Sp($u$) $= \Lambda$.

D’après le lemme 1, on a $\|\sum_{j\in J}\lambda_jp_j\|=$ sup$_{j\in J}|\lambda_j|$ pour toute partie finie J de I. Il en résulte, d’après le critère de Cauchy, que la famille $(\lambda_ip_i)$ est sommable dans $\mathscr{L}(E)$ si et seulement si la famille $\lambda$ tend vers 0 à l’infini, ce qui implique que les conditions (i) et (iii) sont équivalentes.

La condition (iii) implique que $u$ est compact (corollaire de la proposition 2 de III, p. 4). Réciproquement, supposons que l’endomorphisme $u$ est compact. La famille B étant bornée dans E, son image par $u$ dans E est relativement compacte dans E (III, p. 2), donc précompacte. Soit $\varepsilon  >0$ et J un sous-ensemble fini de I tel que l’image de B par $u$ est contenue dans la réunion des boules de rayon $\varepsilon$ et de centre $u(e_j)$ pour $j\in J$. Soit $i\in I$ - J. Il existe $j\in J$ tel que $\|u(e_i)-u(e_j)\|\leqslant \varepsilon$, donc

$$
|\lambda_i|^2\leqslant |\lambda_i|^2+|\lambda_j|^2=\|u(e_i)-u(e_j)\|^2\leqslant \varepsilon^2
$$

Par conséquent, on a $\lambda \in \mathscr{C}_0(I; K)$, c’est-à-dire la condition (i).

Enfin, le spectre de $u$ et son spectre sensible sont calculés en fonction de $\lambda$ en utilisant la prop. 1, c) et la proposition 5 de III, p. 90.

#### Remarque {#ts-iv-s1-n1-rem-2 .statement tag=02WD}

Lorsque I est infini, la condition $\lambda \in \mathscr{C}_0(I; K)$ peut aussi s’énoncer « la famille $\lambda$ tend vers 0 selon le filtre des complémentaires des parties finies de I. »

### 2. Diagonalisation des endomorphismes compacts

#### Théorème 1 {#ts-iv-s1-thm-1 .statement tag=02WE}

Supposons $K =\mathbf{C}$. Soit $u$ un endomorphisme compact et normal de E. Il existe une base orthonormale B de E telle que $u$ est diagonal dans la base B.

L’ensemble Sp$_s(u)$ est dénombrable, et il ne contient pas 0 si E est de dimension infinie (III, p. 90, prop. 5, b)). Pour tout élément $\lambda \in$ Sp$_s(u)$, notons $N_{\lambda}$ le nilespace de $u-\lambda 1_E$. Il est de dimension finie (loc. cit.) et, puisque $u$ est normal, il coïncide avec l’espace propre de $u$ relatif à $\lambda$ (EVT, V, p. 43, cor. de la prop. 8). Les espaces $N_{\lambda}$ sont deux à deux orthogonaux (I, p. 132, n$^o5$).

Soit F le sous-espace de E somme hilbertienne des espaces $N_{\lambda}$ pour $\lambda \in$ Sp$_s(u)-\{0\}$. C’est un espace de type dénombrable, stable par $u$ puisque chaque sous-espace $N_{\lambda}$ est stable par $u$. Comme $N_{\lambda}$ est aussi l’espace propre de $u^*$ relatif à $\overline{\lambda}$ (EVT, V, loc. cit.), l’endomorphisme $u$ induit un endomorphisme $\widetilde{u}$ de $F^{\circ}$ par passage aux sous-espaces. L’endomorphisme $\widetilde{u}$ est compact (prop. 3 de III, p. 5) et normal (lemme 4 de I, p. 135). Par construction, le spectre sensible de $\widetilde{u}$ est contenu dans $\{0\}$ (en effet, tout vecteur propre pour $\widetilde{u}$ en serait un pour $u$, donc appartiendrait à l’un des espaces $N_{\lambda}$ si la valeur propre correspondante était non nulle). Ainsi le rayon spectral de $\widetilde{u}$ est nul, d’où $\widetilde{u}= 0$ puisque $\widetilde{u}$ est normal (cor. 1 de I, p. 108). On a donc $F^{\circ}\subset$ Ker($u$).

Pour tout $\lambda \in$ Sp$_s(u)$, soit $B_{\lambda}$ une base orthonormale de $N_{\lambda}$ et $(e_j)_{j\in J}$ la famille réunion des $B_{\lambda}$; c’est une base orthonormale de F. Soit B la réunion de $(e_j)_{j\in J}$ et d’une base orthonormale de $F^{\circ}$. C’est une base orthonormale de E et $u$ est diagonal dans la base B.

#### Corollaire 1 {#ts-iv-s1-thm-1-cor-1 .statement tag=02WF}

Soit $u$ un endomorphisme compact hermitien de E. Il existe une base orthonormale B de E telle que $u$ est diagonal dans la base B et ses valeurs propres sont réelles.

Si $K =\mathbf{C}$, cela résulte aussitôt du théorème. Supposons $K =\mathbf{R}$. L’espace E est une $\mathbf{R}$-structure sur $E_{(\mathbf{C})}($cf. A, II, p. 119). L’endomorphisme $u_{(\mathbf{C})}$ de $E_{(\mathbf{C})}$ est compact (remarque 4 de III, p. 2) et hermitien. Soient $B = (e_j)_{j\in J}$ une base orthonormale de $E_{(\mathbf{C})}$ telle que $u_{(\mathbf{C})}\in \mathscr{D}_B(E_{(\mathbf{C})})$ et $\lambda$ la famille des valeurs propres de $u_{(\mathbf{C})}$ (théorème 1). On a $\lambda \in \mathbf{R}^J($I, p. 106, prop. 4) ; comme l’application linéaire $u_{(\mathbf{C})}$ est $\mathbf{R}$-rationnelle, le sous-espace propre de $u_{(\mathbf{C})}$ relatif à $\lambda_j$ est $\mathbf{R}$-rationnel pour tout $j\in J ($cf. A, V, p. 60, prop. 6). Il en existe donc une base appartenant à E, et a fortiori, il en existe une base orthonormale dans E. La réunion de ces bases est une base orthonormale $B_{\mathbf{R}}$ de E telle que $u\in \mathscr{D}_{B_{\mathbf{R}}}(E)$.

#### Corollaire 2 {#ts-iv-s1-thm-1-cor-2 .statement tag=02WG}

Soit F un espace hilbertien et soit $u$ une application linéaire continue compacte de E dans F. Il existe un ensemble dénombrable I, une base orthonormale $(e_i)_{i\in I}$ de l’espace initial Ker($u$)$^{\circ}$ de $u$, une famille orthonormale $(f_i)_{i\in I}$ de F et une famille $(\alpha_i)_{i\in I}\in (\mathbf{R}^*_+)^I$ telles que $u(e_i) =\alpha_if_i$ pour tout $i\in I$.

Soit $v=u^*\circ u$. C’est un endomorphisme compact (III, p. 5, prop. 3) et positif, donc hermitien, de E. D’après le corollaire 1, il existe une base orthonormale $(e_j)_{j\in J}$ de E telle que $v$ est diagonal dans cette base. La famille $(\lambda_j)_{j\in J}$ de ses valeurs propres est contenue dans $\mathbf{R}_+^J$. Posons $\alpha_j=\lambda_j$ pour tout $j\in J$. Soit I l’ensemble des $j\in J$ tels que $\alpha_j\not = 0$. C’est un ensemble dénombrable puisque $v$ est compact. La famille $(e_i)_{i\in I}$ est une base orthonormale de l’espace initial de $v$, qui est l’espace initial Ker($u$)$^{\circ}$ de $u$ (EVT, V, p. 43, prop. 8). Posons $f_i=\frac{1}{\alpha_i}u(e_i)$ pour $i\in I$. Quels que soient $i$ et $j$ dans I, on a

1 1 $\lambda_i$

$$
\langle f_i|f_j\rangle =\langle u(e_i)|u(e_j)\rangle =\langle v(e_i)|e_j\rangle =\langle e_i|e_j\rangle
$$

$$
\alpha_i\alpha_j\alpha_i\alpha_j\alpha_i\alpha_j
$$

d’où il résulte que la famille $(f_i)_{i\in I}$ est orthonormale dans F. Le corollaire en résulte, puisque $u(e_i) =\alpha_if_i$ pour tout $i\in I$.

#### Définition 2 {#ts-iv-s1-def-2 .statement tag=02WH}

Avec les notations du corollaire, la famille $(\alpha_i)_{i\in I}$ est la famille des valeurs singulières de $u$, relative à la base orthonormale $(e_i)_{i\in I}$ de l’espace initial de $u$.

#### Remarque 1 {#ts-iv-s1-n2-rem-1 .statement tag=02WI}

Ce corollaire généralise le th. 2 de EVT, V, p. 54, qui correspond aux applications de Hilbert–Schmidt.

#### Remarque 2 {#ts-iv-s1-n2-rem-2 .statement tag=02WJ}

Avec les notations du corollaire, on a la formule

$$
u(x) =\sum_{i\in I}\alpha_i\langle e_i|x\rangle f_i \tag{1}
$$

pour tout $x\in E$.

#### Remarque 3 {#ts-iv-s1-n2-rem-3 .statement tag=02WK}

Soit $u$ un endomorphisme compact positif de E. Soit $B = (f_i)_{i\in I}$ une base orthonormale de E telle que $u$ est diagonal dans la base B (théorème 1), et soit $(\lambda_i)_{i\in I}$ la famille des valeurs propres de $u$ dans cette base. Soit J l’ensemble des $i\in I$ tels que $\lambda_i>0$; la famille $(e_i)_{i\in J}$ est une base orthonormale de l’espace Ker($u$)$^{\circ}$. Pour tout $i\in J$, posons $e_i=f_i$ et $\alpha_i=\lambda_i$. Il vient $u(e_i) =\alpha_if_i:$ la famille $(\alpha_i)_{i\in J}$ est la famille des valeurs singulières de $u$ relative à la base $(e_i)_{i\in J}$.

### 3. Suite décroissante des valeurs propres

Dans ce numéro, on suppose que $K =\mathbf{C}$.

On note $\overline{\mathbf{N}}=\mathbf{N}\cup  \{+\infty \} \subset \overline{\mathbf{R}}$. Dans ce numéro, on dira qu’un espace vectoriel E est de dimension $+\infty  \in \overline{\mathbf{N}}$ si E n’est pas de dimension finie.

Soit $I_E\subset \mathbf{N}$ l’ensemble des dimensions des sous-espaces de dimension finie F de E tels que $F\not = E$. On a $I_E=\mathbf{N}$ si E est de dimension infinie, et sinon $I_E=\{0, . . .$, dim(E) $-1\}$. On notera $I = I_E$ lorsqu’aucune confusion ne pourra en résulter.

Soit $u$ un endomorphisme compact et positif (en particulier hermitien) de E. Le spectre sensible de $u$ est l’ensemble des valeurs d’une suite strictement décroissante $(\nu_k)_{0\leqslant k<Card(Sp_s(u))}$ de nombres réels positifs (cf. prop. 5 de III, p. 90). Pour tout entier $k$ tel que $0\leqslant k <$ Card(Sp$_s(u))$, on note $n_k\geqslant 1$ la multiplicité spectrale de $\nu_k$. Soit $M\in \overline{\mathbf{N}}$ la somme des multiplicités spectrales $n_k$; c’est la dimension de l’image de $u$. On a $M\leqslant$ Card(I).

Pour $0\leqslant n <M$, on définit $\lambda_n(u) =\nu_k$, où $k\geqslant 0$ est l’unique entier tel que

$$
n_0+\cdots +n_{k-1}\leqslant n < n_0+\cdots +n_k
$$

On pose $\lambda_n(u) = 0$ si $n\in I$ vérifie $n\geqslant M$. Ce cas ne peut se présenter que si $I =\mathbf{N}$ et si Sp$_s(u)$ est fini (ou, ce qui revient au même, si E est de dimension infinie et $u$ est de rang fini).

La suite $(\lambda_n(u))_{n\in I}$ est décroissante ; pour tout $\lambda \in$ Sp$_s(u)$, le nombre d’entiers $n$ tels que $\lambda_n(u) =\lambda$ est égal à la multiplicité spectrale de la valeur propre $\lambda$ de $u$.

On dit, par abus de langage, que $(\lambda_n(u))_{n\in J}$ est la suite décroissante des valeurs propres de $u$ répétées avec leurs multiplicités.

#### Proposition 3 {#ts-iv-s1-prop-3 .statement tag=02WL}

Soit $u$ un endomorphisme compact positif de E. Il existe une famille orthonormale $(e_n)_{n\in I}$ dans E telle que, pour tout $x\in E$, l’on ait

$$
u(x) =\sum_{n\in I}\lambda_n(u)\langle e_n|x\rangle e_n,\langle x|u(x)\rangle =\sum_{n\in I}\lambda_n(u)|\langle e_n|x\rangle |^2
$$

Soit $B = (f_j)_{j\in J}$ une base orthonormale de E dans laquelle $u$ est diagonal (cor. 1 de IV, p. 150) et $(\lambda_j)_{j\in J}$ la famille des valeurs propres de $u$ dans la base B. Soit $J'$ l’ensemble des $j\in J$ tels que $\lambda_j$ appartient au spectre sensible de $u$.

Pour chaque $\lambda \in$ Sp$_s(u)$, il existe une bijection entre les entiers $n$ tels que $0\leqslant n <M$ et $\lambda_n(u) =\lambda$ et les $j\in J'$ tels que $\lambda_j=\lambda$, car ces deux ensembles ont comme cardinal la multiplicité spectrale de $\lambda$. Un choix de telles bijections pour tout $\lambda$ définit une bijection $\iota$ de l’ensemble des entiers tels que $0\leqslant n <M$ dans l’ensemble $J'$. On définit la suite $(e_n)_{0\leqslant n<M}$ dans E en posant $e_n=f_{\iota(n)}$ pour $0\leqslant n <M$. C’est une famille orthonormale dans E.

Dans le cas où M $<$ Card(I) $= +\infty$, l’espace F engendré par $\{e_0, . . . , e_{M-1}\}$ est de dimension finie et son orthogonal $F^{\circ}$ est de dimension infinie ; on choisit pour $(e_n)_{n\geqslant M}$ une famille orthonormale dans $F^{\circ}$.

Pour tout $x\in E$, on a

$$
u(x) =\sum_{j\in J'}\lambda_j\langle f_j|x\rangle f_j=\sum_{0\leqslant n<M}\lambda_n(u)\langle e_n|x\rangle e_n
$$

puisque $u(f_j) = 0$ lorsque $j\in J$ - $J'$. Si $n\in I$ vérifie $n\geqslant M$, on a $\lambda_n(u) = 0$, et on obtient la première formule de la proposition. La seconde en résulte.

#### Proposition 4 {#ts-iv-s1-prop-4 .statement tag=02WM}

Soit $u$ un endomorphisme compact positif de E. Soit $f\in \mathscr{C}(\mathbf{R}_+)$ une application continue croissante telle que $f(0) = 0$.

L’endomorphisme $f(u)$ est compact et positif et, pour tout $n\in I_E$, on a $\lambda_n(f(u)) =f(\lambda_n(u))$.

L’endomorphisme $f(u)$ est compact et positif d’après la prop. 6, b) de III, p. 91 et la prop. 15, a) de I, p. 117. Le spectre de $f(u)$ est l’image par $f$ du spectre de $u$ (cor. 2 de I, p. 111). Si $\lambda \in$ Sp$_s(f(u))$, la multiplicité spectrale de $\lambda$ est la somme des multiplicités spectrales des $\mu\in$ Sp($u$) tels que $f(\mu) =\lambda$ (cor. 2 de III, p. 84). Comme $f$ est croissante, la suite $(f(\lambda_n(u)))_{n\in I_E}$ est décroissante. L’assertion résulte alors de la définition de la suite $(\lambda_n(f(u)))_{n\in I_E}$.

### 4. Caractérisations variationnelles des valeurs propres

Dans ce numéro, on suppose que $K =\mathbf{C}$.

Soient $u$ un endomorphisme compact et positif de E et $(\lambda_n(u))_{n\in I_E}$ la suite décroissante des valeurs propres de $u$. On pose $I = I_E$.

Pour tout sous-espace fermé F de E, on note

$$
\langle x|u(x)\rangle \langle x|u(x)\rangle
$$

$r_F(u) =$ inf 2 $,R_F(u) =$ sup 2,

$$
_{x\in F-\{0\}}\|x\|x_{\in F^{\circ-}\{0\}}\|x\|
$$

où la borne inférieure (resp. la borne supérieure) est prise dans $[0,+\infty ]$.

Pour tout $n\in \mathbf{N}$, on note $\mathscr{F}_n$ l’ensemble des sous-espaces vectoriels $F\subset E$ de dimension $n$. On dit qu’un sous-espace $F\in \mathscr{F}_n$ est adapté à $u$ s’il admet une base orthonormale $(f_i)_{0\leqslant i\leqslant n-1}$ telle que $u(f_i) =\lambda_i(u)f_i$ pour $0\leqslant i\leqslant n-1$.

#### Proposition 5 {#ts-iv-s1-prop-5 .statement tag=02WN}

Soit $n\in I$.

a) Pour tout sous-espace $F\in \mathscr{F}_{n+1}$ adapté à $u$, on a $\lambda_n(u) =r_F(u)$;

b) Pour tout sous-espace $F\in \mathscr{F}_n$ adapté à $u$, on a $\lambda_n(u) = R_F(u)$.

Soit $F\in \mathscr{F}_{n+1}$ un sous-espace adapté à $u$, et $(f_i)_{0\leqslant i\leqslant n}$ une base orthonormale de F telle que $u(f_i) =\lambda_i(u)f_i$ pour tout $i$. Pour tout $x$ dans F, on a

$$
\langle x|u(x)\rangle =\sum_{0\leqslant i\leqslant n}\lambda_i(u)|\langle f_i|x\rangle |^2\geqslant \lambda_n(u)\sum_{0\leqslant i\leqslant n}|\langle f_i|x\rangle |^2=\lambda_n(u)\|x\|^2
$$

avec égalité si $x=f_n$. Cela implique que $r_F(u) =\lambda_n(u)$, d’où l’assertion a).

Soit $F\in \mathscr{F}_n$ un sous-espace adapté à $u$. Le sous-espace fermé $F^{\circ}$ est non nul (car $n=$ dim(F) $<$ dim(E)) et stable par $u$; l’endomorphisme $\widetilde{u}$ de $F^{\circ}$ déduit de $u$ par passage aux sous-espaces est compact et positif.

On a Sp($\widetilde{u}$)$\subset$ Sp($u$). On a de plus Sp($\widetilde{u}$)$\subset [0, \lambda_n(u)]$. En effet, il suffit de vérifier que $\lambda \leqslant \lambda_n(u)$ pour tout $\lambda \in$ Sp$_s(\widetilde{u})$. Le nombre $\lambda$ est alors une valeur propre de $u$, donc il existe $j\in I$ tel que $\lambda =\lambda_j(u)$. L’espace propre de $u$ relatif à $\lambda_j(u)$ n’est donc pas contenu dans F, ce qui implique que $\lambda_j(u)\leqslant \lambda_n(u)$.

Supposons que $\lambda_n(u)>0$. L’espace propre de $u$ relatif à $\lambda_n(u)$ n’est alors pas contenu dans F, et $\lambda_n(u)$ appartient donc au spectre sensible de $\widetilde{u}$. On en déduit que sup(Sp($\widetilde{u}$)) $=\lambda_n(u)$. Si $\lambda_n(u) = 0$, on a le même résultat puisque le spectre de $\widetilde{u}$ est alors réduit à $\{0\}$.

Par ailleurs, on a par définition $R_F(u) = R_{\{0\}}(\widetilde{u})$, et finalement $R_{\{0\}}(\widetilde{u}) =$ sup(Sp($\widetilde{u}$)) d’après la prop. 9 de I, p. 139, a). L’assertion b) est démontrée.

#### Proposition 6 {#ts-iv-s1-prop-6 .statement tag=02WO}

Pour tout $n\in I$, on a

$\lambda_n(u) =_{F\in}$sup$_{\mathscr{F}_{n+1}}r_F(u) =$ inf$_{F\in\mathscr{F}_n}R_F(u)$.

Soit $(e_n)_{n\in I}$ une famille orthonormale ayant la propriété de la prop. 3 de IV, p. 152. Pour tout entier tel que $1\leqslant n <M + 1$, soit $F_n\in \mathscr{F}_n$ le sous-espace de dimension $n$ de E engendré par $(e_0, . . . , e_{n-1})$; par construction, l’espace $F_n$ est adapté à $u$. D’après la prop. 5, on a donc

$$
\lambda_n(u) =r_{F_{n+1}}(u) = R_{F_n}(u) \tag{2}
$$

Soit $n\in I$. Soit $F\in \mathscr{F}_{n+1}$. La restriction à F de l’orthoprojecteur sur $F_n$ n’est pas injective, donc il existe $x\not = 0$ dans F orthogonal à $F_n$. Comme $x\in F^{\circ}_n$, on a alors (prop. 3 de IV, p. 152)

$$
\langle x|u(x)\rangle =\sum_{m\in I}\lambda_m(u)|\langle e_m|x\rangle |^2
$$

$m\geqslant n$

$$
\leqslant \lambda_n(u)\sum_{mm\geqslant\in nI}|\langle e_m|x\rangle |^2=\lambda_n(u)\|x\|^2
$$

Cela démontre que $r_F(u)\leqslant \lambda_n(u)$, d’où en particulier l’inégalité

(3) $F_{\in}$sup$_{\mathscr{F}_{n+1}}r_F(u)\leqslant \lambda_n(u)$.

Soit $F\in \mathscr{F}_n$. La restriction à $F_{n+1}$ de l’orthoprojecteur sur F n’est pas injective, donc il existe un vecteur $x\not = 0$ dans $F_{n+1}$ orthogonal à F. Comme $x\in F_{n+1}$, on a (loc. cit.)

$$
\langle x|u(x)\rangle =\sum_{0\leqslant m\leqslant n}\lambda_m(u)|\langle e_m|x\rangle |^2
$$

$$
\geqslant \lambda_n(u)\sum_{0\leqslant m\leqslant n}|\langle e_m|x\rangle |^2=\lambda_n(u)\|x\|^2
$$

et donc $R_F(u)\geqslant \lambda_n(u)$. En particulier, il vient

(4) Finf$_{\in\mathscr{F}_n}R_F(u)\geqslant \lambda_n(u)$.

Au vu des formules (2), (3) et (4), la proposition est démontrée.

### 5. Applications de la caractérisation variationnelle des valeurs propres

Dans ce numéro, on considère des espaces hilbertiens sur $\mathbf{C}$.

#### Proposition 7 {#ts-iv-s1-prop-7 .statement tag=02WP}

Soient $u$ et $v$ des endomorphismes compacts positifs de E.

a) On a $|\lambda_n(u)-\lambda_n(v)|\leqslant \|u-v\|$ pour tout $n\in I$;

b) Si $u\leqslant v$, alors $\lambda_n(u)\leqslant \lambda_n(v)$ pour tout $n\in I$.

Soit $n\in I$ et soit F un sous-espace vectoriel de dimension $n$ de E. Pour tout $x\in F$, on a

$$
|\langle x|v(x)\rangle  - \langle x|u(x)\rangle |\leqslant \|u-v\| \|x\|^2
$$

donc les inégalités

$$
R_F(v)- \|u-v\|\leqslant R_F(u)\leqslant R_F(v) +\|u-v\|
$$

L’assertion a) en découle d’après la proposition 6 de IV, p. 154.

Si $u\leqslant v$, on a $\langle x|u(x)\rangle \leqslant \langle x|v(x)\rangle$ pour tout $x\in E$. Pour tout $n\in I$ et tout sous-espace F de dimension $n$, on a donc $R_F(u)\leqslant R_F(v)$, d’où $\lambda_n(u)\leqslant \lambda_n(v) ($loc. cit.).

#### Proposition 8 {#ts-iv-s1-prop-8 .statement tag=02WQ}

Soit $u$ un endomorphisme compact positif de E. Soient H un sous-espace fermé de E et $i_H: H\rightarrow E$ l’injection canonique. Notons $u_H$ l’endomorphisme $i^*_Hui_H$ de H. Il est compact et positif.

a) On a $I_H\subset I_E$ et $\lambda_n(u_H)\leqslant \lambda_n(u)$ pour tout $n\in I_H$;

b) Si H est de codimension finie $k\in \mathbf{N}$ dans E, alors on a $I_H+k\subset I_E$ et $\lambda_{n+k}(u)\leqslant \lambda_n(u_H)$ pour tout $n\in I_H$.

L’endomorphisme $u_H$ est compact (prop. 3 de III, p. 5). Il est positif car $\langle x|u_H(x)\rangle =\langle i_H(x)|u(i_H(x))\rangle \geqslant 0$ pour tout $x\in H$.

Soit $n\in I_H\subset I_E$. Soit F un sous-espace de dimension $n+ 1$ de H adapté à $u_H$. On a donc $\lambda_n(u_H) =r_F(u_H)$ (prop 5 de IV, p. 153, a)), et comme de plus $r_F(u_H) =r_F(u)\leqslant \lambda_n(u)$ (prop. 6 de IV, p. 154), on obtient l’assertion a).

Supposons que H est de codimension $k\in \mathbf{N}$ dans E et que $n\in I_H$. Soit F un sous-espace de H de dimension $n$ adapté à $u_H$. Son orthogonal dans H est égal à $H\cap F^{\circ}$, et c’est l’orthogonal dans E du sous-espace $F + H^{\circ}$ de dimension $n+k$. Donc $n+k\in I_E$ et (prop 5 de IV, p. 153, b))

$$
\langle x|u_H(x)\rangle
$$

$\lambda_n(u_H) =$ sup 2 $= R_{F+H^{\circ}}(u)$

$$
_{x\in H\cap F^{\circ}}\|x\|
$$

$x\not =0$

d’où $\lambda_n(u_H)\leqslant \lambda_{n+k}(u)$ (prop. 6 de IV, p. 154).

#### Définition 3 {#ts-iv-s1-def-3 .statement tag=02WR}

Soit F un espace hilbertien et soit $u$ une application linéaire compacte de E dans F.

Pour tout entier $n\in I_E$ on note $\alpha_n(u) =\lambda_n(u^*\circ u)$. Soit J l’ensemble des $n\in I_E$ tels que $\alpha_n(u)>0$. La famille $(\alpha_n(u))_{n\in J}$ est appelée la suite des valeurs singulières de $u$ répétées avec multiplicité.

On dit que la suite $(\alpha_n(u))_{n\in I_E}$ est la suite élargie des valeurs singulières de $u$.

La suite $(\alpha_n(u))_{n\in I_E}$ est bien définie puisque l’endomorphisme $u^*\circ u$ de E est compact (III, p. 5, prop. 3) ; c’est une famille décroissante de nombres réels positifs puisque $u^*\circ u$ est positif.

#### Proposition 9 {#ts-iv-s1-prop-9 .statement tag=02WS}

Soit F un espace hilbertien et soit $u$ une application linéaire compacte de E dans F.

a) Pour $n\in I_E$, on a

$$
\|u(x)\|\|u(x)\|
$$

$\alpha_n(u) =$ sup inf = inf sup.

$$
_{F\in\mathscr{F}_{n+1}x\in F-\{0\}}\|x\|_{F\in\mathscr{F}_nx\in F^{\circ-}\{0\}}\|x\|
$$

b) Soit J l’ensemble des $n\in I_E$ tels que $\alpha_n(u)\not = 0$. Il existe des familles orthonormales $(e_n)_{n\in J}$ dans E et $(f_n)_{n\in J}$ dans F telles que pour tout $x\in E$, on a

$$
u(x) =\sum_{n\in J}\alpha_n(u)\langle e_n|x\rangle f_n
$$

Comme $\langle x|u^*u(x)\rangle =\|u(x)\|^2$ pour tout $x\in E$, les définitions et la prop. 6 de IV, p. 154, a), impliquent l’égalité de la première assertion.

Soit $(e_n)_{n\in I_E}$ une famille orthonormale de E vérifiant les conclusions de la prop. 3 de IV, p. 152 appliquée à l’endomorphisme compact positif $u^*\circ u$ de E. Posons $f_n=\alpha^{-1}_nu(e_n)$ pour $n\in J$. En raisonnant comme dans la preuve du corollaire 2 de IV, p. 150, on obtient l’assertion c).

#### Corollaire {#ts-iv-s1-n5-cor-1 .statement tag=02WT}

Soient F un espace hilbertien et $u$ une application linéaire compacte de E dans F. Soient $w\in \mathscr{L}(E)$ et $v\in \mathscr{L}(F)$. Pour tout $n\in I_E$, on a $\alpha_n(w\circ u\circ v)\leqslant \|v\| \|w\|\alpha_n(u)$.

C’est une conséquence de l’assertion a) de la proposition précédente.

#### Remarque 1 {#ts-iv-s1-n5-rem-1 .statement tag=02WU}

La suite $(\alpha_n(u))_{n\in I_E}$ étant décroissante, l’ensemble J est, soit égal à $I_E$, soit égal à un segment $\{0, . . . , m\}$ dans $I_E$ où $m\in \mathbf{N}$. Ce dernier cas vaut si et seulement si $u$ est de rang fini.

#### Remarque 2 {#ts-iv-s1-n5-rem-2 .statement tag=02WV}

Comme $\|u(x)\|=\||u|(x)\|$ pour tout $x\in E ($I, p. 139, prop. 10), on a $\alpha_n(u) =\alpha_n(|u|)$ pour tout $n\in I_E$.

#### Remarque 3 {#ts-iv-s1-n5-rem-3 .statement tag=02WW}

Si $u$ est positif, alors $\alpha_n(u) =\lambda_n(u)$ pour tout $n\in I_E$ (en effet, on a alors $\alpha_n(u)^2=\lambda_n(u^*u) =\lambda_n(u^2) =\lambda_n(u)^2$ d’après la prop. 4 de IV, p. 153).

#### Remarque 4 {#ts-iv-s1-n5-rem-4 .statement tag=02WX}

Il est possible que $\alpha_n(v\circ u\circ w) = 0$ même si $\alpha_n(u)$ est non nul ; dans ce cas, $\alpha_n(v\circ u\circ w)$ n’est pas une valeur singulière de $v\circ u\circ w$.

### 6. Inégalités de Weyl

Dans ce numéro, on considère des espaces hilbertiens sur $K =\mathbf{C}$.

Soit E un espace hilbertien. Pour tout $n\in \mathbf{N}$, on rappelle qu’on a défini la puissance extérieure hilbertienne $\widehat{\wedge}^nE$ dans EVT, V, p. 34. Pour tout espace hilbertien F et pour $u\in \mathscr{L}(E; F)$, on a également défini l’application linéaire $\widehat{\wedge}^nu\in \mathscr{L}(\widehat{\wedge}^nE;\widehat{\wedge}^nF) ($loc. cit.). Ces constructions sont fonctorielles : pour tout espace hilbertien G et pour toute application linéaire $v\in \mathscr{L}(F; G)$, la formule

$$
\widehat{\wedge}^nv\circ \widehat{\wedge}^nu=\widehat{\wedge}^n(v\circ u)
$$

est valide (loc. cit., formule (28)).

Soient H un sous-espace fermé de E et $i_H$ l’injection canonique de H dans E. Pour tout endomorphisme $u$ de E, on note $u_H$ l’endomorphisme $i^*_Hui_H$ de H.

#### Lemme 2 {#ts-iv-s1-lem-2 .statement tag=02WY}

Soit $n\in \mathbf{N}$. L’application $\widehat{\wedge}^ni_H$ est une application linéaire isométrique de $\widehat{\wedge}^nH$ dans $\widehat{\wedge}^nE$.

Soit $(e_j)_{j\in J}$ une base orthonormée de H et $(e_j)_{j\in J'}$ une base orthonormale de E, où $J\subset J'$. Munissons $J'$ d’une structure d’ordre total. Les éléments $e_{j_1}\wedge  \cdots  \wedge e_{j_n}$ pour $j_1<\cdots < j_n$ dans $J'$ (resp. dans J) forment une base orthonormale de $\widehat{\wedge}^nE$ (resp. de $\widehat{\wedge}^nH)$ d’après la prop. 5 de EVT, V, p. 34, prop. 5. Le lemme en résulte.

Dans la suite, on identifiera $\widehat{\wedge}^nH$ à un sous-espace fermé de $\widehat{\wedge}^nE$ par le truchement de l’application $\widehat{\wedge}^ni_H$.

#### Lemme 3 {#ts-iv-s1-lem-3 .statement tag=02WZ}

Soient F un espace hilbertien et $u\in \mathscr{L}(E; F)$. Soit $n\in \mathbf{N}$.

a) On a $\widehat{\wedge}^nu^*=\widehat{\wedge}^n(u^*)$;

b) Si F = E et $u$ est hermitien (resp. positif, normal, unitaire), alors $\widehat{\wedge}^nu$ est hermitien (resp. positif, normal, unitaire) ;

c) On a $|\widehat{\wedge}^nu|=\widehat{\wedge}^n|u|$;

d) Soit H un sous-espace fermé de E. La restriction $(\widehat{\wedge}^nu)|\widehat{\wedge}^nH$ de $\widehat{\wedge}^nu$ à $\widehat{\wedge}^nH$ est égale à $\widehat{\wedge}^n(u|H) ($égalité dans $\mathscr{L}(\widehat{\wedge}^nH;\widehat{\wedge}^nF))$;

e) Supposons F = E. Soit H un sous-espace fermé de E. On a $\widehat{\wedge}^nu_{\widehat{\wedge}^nH}=\widehat{\wedge}^n(u_H)$ dans $\mathscr{L}(\widehat{\wedge}^nH)$.

L’assertion a) résulte de EVT, V, p. 39, formule (13). Elle implique aussitôt que $\widehat{\wedge}^nu$ est hermitien (resp. unitaire) lorsque $u$ est hermitien (resp. unitaire). Si $u$ est positif, alors $u^{1/2}$ est hermitien, donc aussi $\widehat{\wedge}^n(u^{1/2})$; la relation $\widehat{\wedge}^nu=\widehat{\wedge}^nu^{1/22}$ implique que $\widehat{\wedge}^nu$ est positif (I, p. 138, prop. 8). Cela démontre b).

Ce qui précède permet de calculer que

$$
\widehat{\wedge}^n|u|^2=\widehat{\wedge}^n(|u|^2) =\widehat{\wedge}^n(u^*u)
$$

$$
=\widehat{\wedge}^nu^*\widehat{\wedge}^nu=\widehat{\wedge}^nu^*(\widehat{\wedge}^nu) =|\widehat{\wedge}^nu|^2
$$

Comme $\widehat{\wedge}^n|u|$ est positif d’après b), il résulte de la prop. 16 de I, p. 118 que $\widehat{\wedge}^n|u|=|\widehat{\wedge}^nu|$, d’où c).

Soit $i_H$ l’injection canonique de H dans E. L’espace $\widehat{\wedge}^nH$ est identifié à un sous-espace fermé de $\widehat{\wedge}^nE$ par l’application $\widehat{\wedge}^ni_H$, d’où

$$
(\widehat{\wedge}^nu)|\widehat{\wedge}^nH =\widehat{\wedge}^nu\circ \widehat{\wedge}^ni_H=\widehat{\wedge}^n(u\circ i_H) =\widehat{\wedge}^n(u|H)
$$

et

$$
(\widehat{\wedge}^nu)_{\widehat{\wedge}^nH}= (\widehat{\wedge}^ni_H)^*\circ \widehat{\wedge}^nu\circ \widehat{\wedge}^ni_H=\widehat{\wedge}^n(i^*_Hui_H) =\widehat{\wedge}^n(u_H)
$$

ce qui démontre d) et e).

Soit F un espace hilbertien, et soit $u\in \mathscr{L}^c(E; F)$. Comme dans le numéro 3 de IV, p. 151, on note $I_E$ l’ensemble des dimensions des sous-espaces de dimension finie F de E tels que $F\not = E$. On rappelle que $(\alpha_n(u))_{n\in I_E}$ désigne la suite élargie des valeurs singulières de $u$ (déf. 3 de IV, p. 156).

#### Proposition 10 {#ts-iv-s1-prop-10 .statement tag=02X0}

On a l’égalité

$$
\prod_{i=0}^n\alpha_i(u) =(\wedge^{n+1}u
$$

pour tout $n\in I_E$.

Le lemme 3, c) démontre que $\|\widehat{\wedge}^{n+1}u\|=\|\widehat{\wedge}^{n+1}|u|\|$; comme de plus $\alpha_i(u) =\alpha_i(|u|)$ pour tout $i\in I_E$ (remarque 5 de IV, p. 157, (2)), il suffit de démontrer l’assertion pour $|u|$. Cela permet de supposer que F = E et que $u$ est positif.

Soit alors $B = (e_j)_{j\in J}$ une base orthonormale de E telle que $u$ est diagonalisable dans la base B (théorème 1 de IV, p. 149), et soit $(\lambda_j)_{j\in J}$ la famille des valeurs propres de $u$ dans la base B. Munissons J d’un ordre total, et notons $J_n$ l’ensemble des familles strictement croissantes $(j_0, . . . , j_n)\in J^{n+1}$ d’éléments de J. Les vecteurs

$$
e_{\iota}=e_{j_0}\wedge  \cdots  \wedge e_{j_n}
$$

pour $\iota = (j_0, . . . , j_n)\in J_n$ forment une base orthonormale $B_n$ de $\widehat{\wedge}^{n+1}E$ (EVT, V, p. 34, prop. 5). Pour tout $\iota = (j_0, . . . , j_n)\in J_n$, notons

$$
\lambda_{\iota}=\prod_{j=0}^n\lambda_{i_j}
$$

Il vient $\widehat{\wedge}^{n+1}ue_{\iota}=\lambda_{\iota}e_{\iota}$, donc $\widehat{\wedge}^{n+1}u$ est diagonal dans la base $B_n$. Par conséquent, on a

$\|\widehat{\wedge}^{n+1}u\|=$ sup $\lambda_{\iota}$

$\iota \in I_n$

(lemme 1 de IV, p. 147), qui est égal au produit $\lambda_0(u)\cdots \lambda_n(u)$ des $n+ 1$ plus grandes valeurs propres de $u$. La formule désirée en résulte puisque $\lambda_i(u) =\alpha_i(u)$ pour tout $i\in I_E$ lorsque $u$ est positif (remarque 5 de IV, p. 157, (3)).

En particulier, si $\alpha_1(u)< \alpha_0(u) =\|u\|$, on voit que l’inégalité $\|\widehat{\wedge}^n(u)\|\leqslant \|u\|^n$ (EVT, V, p. 34, formule (29)) n’est pas une égalité en général si $n\geqslant 2$.

#### Corollaire {#ts-iv-s1-n6-cor-1 .statement tag=02X1}

Soit G un espace hilbertien et $v\in \mathscr{L}^c(F; G)$. On a

$$
\prod_{i=0}^n\alpha_i(v\circ u)\leqslant \prod_{i=0}^n\alpha_i(u)\alpha_i(v)
$$

pour tout $n\in I_E$.

Il suffit de remarquer que

$$
\|\widehat{\wedge}^{n+1}(vu)\|=\|\widehat{\wedge}^{n+1}v\circ \widehat{\wedge}^{n+1}u\|\leqslant \|\widehat{\wedge}^{n+1}v\| \|\widehat{\wedge}^{n+1}u\|
$$

et d’appliquer la proposition 10.

#### Lemme 4 {#ts-iv-s1-lem-4 .statement tag=02X2}

Soit A un anneau. Soient $n\in \mathbf{N}$ et $(a_i)_{0\leqslant i\leqslant n}$ et $(b_i)_{0\leqslant i\leqslant n}$ des familles d’éléments de A. Pour $0\leqslant j\leqslant n$, posons

$$
A_j=\sum_{i=0}^ja_i
$$

On a

$$
\sum_{i=0}^na_ib_i= A_nb_n-\sum^{n-1}_{i=0}A_i(b_{i+1}-b_i)
$$

Posons $A_{-1}= 0$. On a $a_i= A_i-A_{i-1}$ pour $0\leqslant i\leqslant n$, donc

$$
\sum_{i=0}^na_ib_i=\sum_{i=0}^n(A_i-A_{i-1})b_i=\sum^{n-1}_{i=0}A_i(b_i-b_{i+1}) + A_nb_n
$$

comme désiré.

Soit I un intervalle de $\overline{\mathbf{R}}$ ne contenant pas $+\infty$. Rappelons (FVR, I, p. 38, remarque) qu’une fonction continue $f: I\rightarrow [-\infty ,+\infty [$ est dite convexe si sa restriction à l’intérieur de I est une fonction convexe à valeurs dans $\mathbf{R}$; elle a alors une limite (finie ou infinie) à droite en inf I. Dans les énoncés ci-dessous, le produit de 0 et d’un élément de $\{-\infty ,+\infty \}$ est par convention égal à 0.

#### Lemme 5 {#ts-iv-s1-lem-5 .statement tag=02X3}

Soient $I\subset \overline{\mathbf{R}}$ un intervalle ne contenant pas $+\infty$ et $f$ une fonction convexe croissante de I dans $[-\infty ,+\infty [$.

Soient $n$ un entier naturel et

$$
a_0\geqslant a_1\geqslant \cdots \geqslant a_n,b_0\geqslant b_1\geqslant \cdots \geqslant b_n
$$

des éléments de I.

Soient $\varrho_0\geqslant \varrho_1\geqslant \cdots \geqslant \varrho_n$ des nombres réels positifs. Supposons que

$$
\sum_{i=0}^ja_i\leqslant \sum_{i=0}^jb_i \tag{5}
$$

pour tout entier $j$ tel que $0\leqslant j\leqslant n$. On a alors

$$
\sum_{i=0}^n\varrho_if(a_i)\leqslant \sum_{i=0}^n\varrho_if(b_i) \tag{6}
$$

Supposons d’abord que $a_i\in \mathring{I}$, et donc $f(a_i)\in \mathbf{R}$, pour tout $i$. Soit $i$ tel que $0\leqslant i\leqslant n$, et soient $(\alpha_i, \beta_i)$ des nombres réels tels que la droite d’équation $y=\alpha_ix+\beta_i$ est une droite d’appui du graphe de $f$ au point $(a_i, f(a_i))$ (FVR, I, p. 37). On a par conséquent $f(a_i) =\alpha_ia_i+\beta_i$ et $f(b_i)\geqslant \alpha_ib_i+\beta_i$ puisque le graphe de $f$ est au dessus de la droite d’appui, d’où

$$
f(b_i)-f(a_i)\geqslant \alpha_i(b_i-a_i) \tag{7}
$$

Par ailleurs, si $i < n$, on a

$$
\alpha_i\geqslant f'_g(a_i)\geqslant f'_d(a_{i+1})\geqslant \alpha_{i+1}
$$

(loc. cit. et FVR, I, p. 36, cor. 1) ; de plus $\alpha_i\geqslant 0$ puisque $f$ est croissante (FVR, I, p. 22, corollaire), d’où $\varrho_i\alpha_i\geqslant \varrho_{i+1}\alpha_{i+1}\geqslant 0$ pour $0\leqslant i < n$.

Soit $j$ un entier tel que $0\leqslant j\leqslant n$. Posons

$$
A_j=\sum_{i=0}^j(b_i-a_i)
$$

de sorte que $A_j\geqslant 0$ par l’hypothèse (5). En appliquant l’inégalité (7) puis le lemme 4, on en déduit

$$
\sum_{i=0}^n\varrho_i(f(b_i)-f(a_i))\geqslant \sum_{i=0}^n\varrho_i\alpha_i(b_i-a_i)
$$

$$
=\varrho_n\alpha_nA_n+\sum^{n-1}_{j=0}(\varrho_j\alpha_j-\varrho_{j+1}\alpha_{j+1})A_j\geqslant 0
$$

Considérons le cas cas général, et raisonnons par récurrence sur $n$. Si l’un des $a_i$ n’appartient pas à l’intérieur de I, on a nécessairement $a_0=$ sup I ou $a_n=$ inf I.

Supposons d’abord que $a_n$ = inf I. On a alors $a_n\leqslant b_n$ et donc $\varrho_nf(a_n)\leqslant \varrho_nf(b_n)$. L’hypothèse de récurrence, appliquée aux familles $(a_0, . . . , a_{n-1}), (b_0, . . . , b_{n-1})$ et $(\varrho_0, . . . , \varrho_{n-1})$, implique

$$
\sum^{n-1}_{i=0}\varrho_if(a_i)\leqslant \sum^{n-1}_{i=0}\varrho_if(b_i)
$$

d’où l’inégalité désirée en ajoutant $\varrho_nf(a_n)$. Le cas où $a_0=$ sup I est traité de manière similaire.

#### Proposition 11 (Inégalités de Weyl) {#ts-iv-s1-prop-11 .statement tag=02X4}

Soient G un espace hilbertien et $v\in \mathscr{L}^c(F; G)$. Soit $g:\mathbf{R}_+\rightarrow [-\infty ,+\infty [$ une fonction croissante telle que la fonction $g\circ$ exp est convexe. On a

$$
\sum_{i=0}^ng(\alpha_i(v\circ u))\leqslant \sum_{i=0}^ng(\alpha_i(v)\alpha_i(u))
$$

pour tout $n\in I_E\cap I_F$.

Posons $I = [-\infty ,+\infty [$ et $f=g\circ$ exp. Il est loisible d’appliquer le lemme 5 avec

$a_i=$ log($\alpha_i(v\circ u)$)$\in I,b_i=$ log($\alpha_i(v)\alpha_i(u)$)$\in I$

et $\varrho_i= 1$ pour $0\leqslant i\leqslant n$, puisque

$\sum_{i=0}^ja_i=$ log $\prod_{i=0}^j\alpha_i(v\circ u)\leqslant$ log $\prod_{i=0}^j\alpha_i(v)\alpha_i(u)=\sum_{i=0}^jb_i$

pour $0\leqslant j\leqslant n$ d’après le cor. de la prop. 10. L’inégalité (6) est alors la conclusion recherchée.

#### Lemme 6 {#ts-iv-s1-lem-6 .statement tag=02X5}

Soient $g$ et $h$ des fonctions convexes définies sur des intervalles I et J de $\mathbf{R}$, respectivement. Si $g$ est croissante et définie sur l’image de $h$, alors la fonction $g\circ h$ est convexe sur J.

En effet, pour $t\in [0,1]$ et $(x, y)\in J\times J$, on a

$$
g(h(tx+ (1-t)y))\leqslant g(th(x) + (1-t)h(y))
$$

$$
\leqslant tg(h(x)) + (1-t)g(h(y))
$$

#### Corollaire {#ts-iv-s1-n6-cor-2 .statement tag=02X6}

Soient G un espace hilbertien et $v\in \mathscr{L}^c(F; G)$. Soit $n\in I_E\cap I_F$.

a) Soit $r\in \mathbf{R}^*_+$. On a

$$
\sum_{i=0}^n\alpha_i(v\circ u)^r\leqslant \sum_{i=0}^n\alpha_i(v)^r\alpha_i(u)^r
$$

b) Soient $p, q, r\in \mathbf{R}_+^*$ tels que $\frac{1}{p}+\frac{1}{q}=\frac{1}{r}$. Alors

$n1/rn1/pn1/q$

$$
\sum_{i=0}\alpha_i(v\circ u)^r\leqslant \sum_{i=0}\alpha_i(v)^p\sum_{i=0}\alpha_i(u)^q
$$

c) Supposons que F = E. Pour tout entier $m\geqslant 2$, on a

$nnm/2$

$$
\sum_{i=0}\alpha_i(u^m)\leqslant \sum_{i=0}\alpha_i(u)^2
$$

Soit $r\in \mathbf{R}^*_+$ et soit $g$ la fonction définie sur $\mathbf{R}_+$ par $g(x) =x^r$. La fonction $g\circ$ exp est convexe (lemme 6), donc l’assertion a) résulte de la prop. 11 appliquée à la fonction $g$.

L’assertion b) résulte de a) et de l’inégalité de Hölder (INT, I, prop. 4).

Soit $m\geqslant 2$ un entier. Appliquons b) avec $r= 1,p=q= 2$ et $v=u^{m-1}$. On trouve

$nn1/2n1/2$

$$
\sum_{i=0}\alpha_i(u^m)\leqslant \sum_{i=0}\alpha_i(u^{m-1})^2\sum_{i=0}\alpha_i(u)^2
$$

Démontrons c) par récurrence sur $m\geqslant 2$. L’inégalité précédente établit l’assertion lorsque $m= 2$. Supposons que $m\geqslant 3$ et que l’assertion est valide pour $m-1$; puisque on a

$nm$ 2

$$
\sum_{i=0}\alpha_i(u^{m-1})^2\leqslant \sum_{i=0}\alpha_i(u^{m-1})
$$

l’inégalité ci-dessus implique

$nn1/2n1/2nm/2$

$$
\sum_{i=0}\alpha_i(u^m)\leqslant \sum_{i=0}\alpha_i(u^{m-1})\sum_{i=0}\alpha_i(u)^2\leqslant \sum_{i=0}\alpha_i(u)^2
$$

en appliquant l’hypothèse de récurrence.

### 7. Endomorphismes de trace finie

On rappelle qu’un endomorphisme positif $u$ de E est de trace finie si et seulement s’il existe une base orthonormale $(e_i)_{i\in I}$ de E telle que

$$
\sum_{i\in I}\langle e_i|u(e_i)\rangle <+\infty
$$

(EVT, V, p. 48, lemme 3 et p. 49, déf. 7). Si $K =\mathbf{C}$, l’espace $\mathscr{L}_1(E)$ des endomorphismes de trace finie de E est l’espace vectoriel engendré par l’ensemble des endomorphismes positifs de trace finie (EVT, V, p. 50, déf. 8) ; si $K =\mathbf{R}$, l’espace $\mathscr{L}_1(E)$ est défini comme l’intersection $\mathscr{L}(E)\cap \mathscr{L}_1(E_{(\mathbf{C})})$ (EVT, V, p. 50).

Si $u\in \mathscr{L}_1$(E), alors la série

$$
\sum_{i\in I}\langle e_i|u(e_i)\rangle
$$

converge pour toute base orthonormale $(e_i)_{i\in I}$ de E et sa somme est indépendante de la base orthonormale ; on dit que c’est la trace Tr($u$) de $u$ (EVT, V, p. 50). Si $K =\mathbf{R}$, on a Tr($u$) $=$ Tr($u_{(\mathbf{C})}$).

Soit $u\in \mathscr{L}_1(E)$. On a $u^*\in \mathscr{L}_1(E)$ et Tr($u^*$) $=$ Tr($u$) $($loc. cit.).

#### Proposition 12 {#ts-iv-s1-prop-12 .statement tag=02X7}

Soit $B = (e_i)_{i\in I}$ une base orthonormale de E. Soit $u\in \mathscr{D}_B(E)$ et notons $\lambda = (\lambda_i)_{i\in I}$ la famille de ses valeurs propres. L’endomorphisme $u$ est de trace finie si et seulement si la famille $\lambda$ est sommable dans K. On a alors Tr($u$) $=\sum\lambda_i$.

Quitte à remplacer $u$ par $u_{(\mathbf{C})}$, on peut supposer que $K =\mathbf{C}$.

Supposons d’abord que $u$ est de trace finie. D’après EVT, V, p. 50 et p. 49, formule (25), la famille $(\langle e_i|u(e_i)\rangle )_{i\in I}= (\lambda_i)_{i\in I}$ est sommable.

Réciproquement, supposons que la famille $\lambda$ est sommable.

Chacune des familles $(\mathscr{R}(\lambda_i)^+), (\mathscr{R}(\lambda_i)^-), (\mathscr{I}(\lambda_i)^+), (\mathscr{I}(\lambda_i)^-)$ est alors sommable. L’endomorphisme $u$ est combinaison linéaire des éléments de $\mathscr{D}_B(E)$ dont ces familles sont les valeurs propres. Ces éléments de $\mathscr{D}_B(E)$ sont positifs. Puisque, par définition, l’espace des endomorphismes de trace finie est engendré par les endomorphismes positifs de trace fini, on peut donc supposer que $\lambda_i\geqslant 0$ pour tout $i$. Comme $\langle e_i|u(e_i)\rangle =\lambda_i$, la famille $(\langle e_i|u(e_i)\rangle )_{i\in I}$ est sommable, donc $u$ est de trace finie (EVT, V, p. 48, lemme 3).

Enfin, si $u$ est de trace finie, alors d’après EVT, V, p. 50, on a

Tr($u$) $=\sum_{i\in I}\langle e_i|u(e_i)\rangle =\sum_{i\in I}\lambda_i$.

#### Corollaire 1 {#ts-iv-s1-prop-12-cor-1 .statement tag=02X8}

Soit $u$ un endomorphisme de trace finie de E.

a) L’endomorphisme $u$ est compact;

b) Soient $B = (e_i)_{i\in I}$ une base orthonormale de l’espace initial Ker($u$)$^{\circ}$ de $u,C = (f_i)_{i\in I}$ une famille orthonormale de E et $(\alpha_i)_{i\in I}$ une famille dans $(\mathbf{R}^*_+)^I$ telles que $u(e_i) =\alpha_if_i$ pour tout $i\in I$ (cor. 2 de IV, p. 150). On a

Tr($u$) $=\sum_{i\in I}\alpha_i\langle e_i|f_i\rangle$.

Pour démontrer a), on peut supposer que $K =\mathbf{C}$ (EVT, V, p. 50 et remarque 4 de III, p. 2) et que $u$ est positif (EVT, V, p. 50, déf. 8).

D’après EVT, V, p. 56, cor. 1, il existe une base orthonormale $B = (e_i)_{i\in I}$ de E tel que $u$ est diagonal dans la base B et de plus la famille $\lambda$ des valeurs propres de $u$ appartient à $\mathbf{R}^I_+$ et est sommable. La famille $\lambda$ appartient donc à $\mathscr{C}_0(I; K)$ (TG, III, p. 38, prop. 1), et par conséquent l’endomorphisme $u$ est compact (prop. 2 de IV, p. 148).

Démontrons b). Soit $(e_i)_{i\in J}$ une base orthonormale de E prolongeant la famille B, de sorte que $u(e_i) = 0$ si $i\in J$ - I. Il vient

Tr($u$) $=\sum_{i\in J}\langle e_i|u(e_i)\rangle =\sum_{i\in I}\langle e_i|u(e_i)\rangle =\sum_{i\in I}\alpha_i\langle e_i|f_i\rangle$.

#### Corollaire 2 {#ts-iv-s1-prop-12-cor-2 .statement tag=02X9}

Soit F un espace hilbertien. Soit $u\in \mathscr{L}(E; F)$ une application de Hilbert–Schmidt. Alors $u$ est une application linéaire compacte.

Soit $(j,|u|)$ la décomposition polaire de $u($I, p. 140, déf. 4). Par définition (EVT, V, p. 50, déf. 9) l’endomorphisme $u^*u$ est de trace finie,$\surd$ donc est compact (corollaire 1, a)) ; il en est de même de $|u|=u^*u$ (prop. 6 de III, p. 91, b)) et de $u=j|u|$ (prop. 3 de III, p. 5).

#### Corollaire 3 {#ts-iv-s1-prop-12-cor-3 .statement tag=02XA}

Supposons que $K =\mathbf{C}$. Soit $u$ un endomorphisme compact positif de E. L’endomorphisme $u$ est de trace finie si et seulement si la famille décroissante de ses valeurs propres $(\lambda_n(u))_{n\in I_E}$ est sommable ; la trace de $u$ est alors la somme de cette famille.

D’après le th. 1 de IV, p. 149, cela résulte de la proposition précédente et de la définition de la suite $(\lambda_n(u))_{n\in I_E}$ (n$^o3$ de IV, p. 151), compte tenu de la formule (28) de EVT, V, p. 49.

#### Corollaire 4 {#ts-iv-s1-prop-12-cor-4 .statement tag=02XB}

Soit F un espace hilbertien. Soit $u\in \mathscr{L}(E; F)$ une application linéaire compacte. Soient $B = (e_i)_{i\in I}$ une base orthonormale de l’espace initial Ker($u$)$^{\circ}$ de $u,C = (f_i)_{i\in I}$ une famille orthonormale de F et $(\alpha_i)_{i\in I}$ une famille dans $(\mathbf{R}^*_+)^I$ telles que $u(e_i) =\alpha_if_i$ pour tout $i\in I$ (cor. 2 de IV, p. 150).

L’endomorphisme $|u|$ de E est de trace finie si et seulement si la famille $(\alpha_i)_{i\in I}$ est sommable. On a alors $u\in \mathscr{L}_2(E; F)$ et

(8) Tr($|u|$) $=\sum_{i\in I}\alpha_i,\|u\|^2_2=$ Tr($u^*u$) $=\sum_{i\in I}\alpha^2_i$,

et en particulier $\|u\|_2\leqslant$ Tr($|u|$).

La famille des valeurs propres non nulles de $|u|$ est $(\alpha_i)_{i\in I}$, donc $|u|$ est de trace finie si et seulement si la famille $(\alpha_i)_{i\in I}$ est sommable (prop. 12). Si c’est le cas, la famille $(\alpha^2_i)$ des valeurs propres non nulles de $u^*u=|u|^2$ est sommable, et les formules (8) résultent de loc. cit.

#### Lemme 7 {#ts-iv-s1-lem-7 .statement tag=02XC}

Soit $\lambda = (\lambda_i)_{i\in I}$ une famille de nombres complexes. Pour tout $t\in \mathbf{C}^*$, soit $n_t$ le cardinal de l’ensemble des $i\in I$ tels que $\lambda_i=t$. La famille $(\lambda_i)_{i\in I}$ est sommable si et seulement si $n_t$ est fini pour tout $t\in \mathbf{C}^*$ et si la famille $(n_tt)_{t\in\mathbf{C}^*}$ est sommable. Dans ce cas, les sommes de ces deux familles sont égales.

Supposons que la famille $(\lambda_i)_{i\in I}$ est sommable. Pour tout $t\in \mathbf{C}$, soit $I_t$ l’ensemble des $i\in I$ tels que $\lambda_i=t$. D’après TG, III, p. 39, th. 2, appliqué à la partition de I par les ensembles $I_t$, l’ensemble $I_t$ est fini pour tout $t\in \mathbf{C}^*$, et de plus la famille $(n_tt)_{t\in\mathbf{C}^*}$ est sommable de somme égale à celle de la famille $(\lambda_i)_{i\in I}$.

Réciproquement, supposons que $n_t$ est fini pour tout $t\in \mathbf{C}^*$ et que la famille $(n_tt)_{t\in\mathbf{C}^*}$ est sommable. Soient J une partie finie de I et Λ l’ensemble des $\lambda_i$ pour $i\in J$. On a

$$
\sum_{i\in J}\lambda_i\leqslant \sum_{t\in\Lambda-\{0\}}n_t|t|\leqslant \sum_{t\in\mathbf{C}^*}n_t|t|
$$

donc la famille $(\lambda_i)_{i\in I}$ est sommable (TG, VII, p. 17, corollaire).

#### Proposition 13 {#ts-iv-s1-prop-13 .statement tag=02XD}

Supposons que $K =\mathbf{C}$. Soit $u$ un endomorphisme normal compact de E. Pour $t\in$ Sp$_s(u)$, soit $n_t\geqslant 1$ la multiplicité spectrale de la valeur propre $t$ de $u$. Pour que $u$ soit de trace finie, il faut et il suffit que la famille $(n_tt)_{t\in Sp_s(u)}$ soit sommable. La trace de $u$ est alors la somme de cette famille.

Soit $B = (e_i)_{i\in I}$ une base orthonormale de E telle que $u$ soit diagonal dans la base B (th. 1 de IV, p. 149), et soit $\lambda = (\lambda_i)_{i\in I}$ la famille de ses valeurs propres. Puisque, pour $t\in$ Sp$_s(u)$, la multiplicité $n_t$ est égale au nombre d’éléments $i\in I$ tels que $\lambda_i=t$ et que les éléments non nuls de $\lambda$ appartiennent à Sp$_s(u)$, l’assertion résulte alors de la prop. 12 et du lemme précédent.

### 8. Applications nucléaires

Dans ce numéro, F désigne un espace hilbertien sur K. Lorsque $K =\mathbf{C}$, on rappelle (I, p. $139\surd$,déf. 3) que pour $u\in \mathscr{L}(E; F)$, on note $|u|$ l’endomorphisme positif $u^*\circ u$ de E. Lorsque $K =\mathbf{R}$, l’élément $|u_{(\mathbf{C})}|$ de $\mathscr{L}(E_{(\mathbf{C})})$ est de la forme $v_{(\mathbf{C})}$ pour un unique endomorphisme $v\in \mathscr{L}$ (E), qui est encore noté $|u|($cf. I, p. 87).

On note $(u, v)\mapsto  \langle u|v\rangle =$ Tr($u^*v$) le produit scalaire dans l’espace hilbertien $\mathscr{L}_2(E; F)$ (EVT, V, p. 53, remarques 1 et 2).

Pour tout $u\in \mathscr{L}(E; F)$, on note $\|u\|_1=$ Tr($|u|$) si $|u|$ est de trace finie et $\|u\|_1= +\infty$ si ce n’est pas le cas. On a donc $\|u\|_1\in \mathbf{R}_+\cup \{+\infty \}$. Puisque $\|u\|=\| |u| \|$ (prop. 10, a) de I, p. 139) et que, si $v$ est positif et de trace finie, alors Tr($v$)$\geqslant \|v\|$ (EVT, V, p. 49, formule (24bis) et p. 44, prop. 9), il vient

$$
\|u\|\leqslant \|u\|_1 \tag{9}
$$

Si $\|u\|_1$ est fini, alors $u$ est une application de Hilbert–Schmidt et $\|u\|_2\leqslant \|u\|_1$ (cor. 4 de IV, p. 165).

#### Proposition 14 {#ts-iv-s1-prop-14 .statement tag=02XE}

Soit $u\in \mathscr{L}_2(E; F)$. On a

$\|u\|_1=_{v\in\mathscr{L}}$sup$_{_2(E;F)}|\langle v|u\rangle |$,

$\|v\|\leqslant 1$

la borne supérieure étant calculée dans $\mathbf{R}_+\cup  \{+\infty \}$.

Soient $B = (e_i)_{i\in I}$ une base orthonormale de l’espace initial Ker($u$)$^{\circ}$ de $u, C = (f_i)_{i\in I}$ une famille orthonormale de F et $(\alpha_i)_{i\in I}$ une famille dans $(\mathbf{R}^*_+)^I$ telles que $u(e_i) =\alpha_if_i$ pour tout $i\in I$ (cor. 2 de IV, p. 150). La famille $(\alpha_i)_{i\in I}$ est de carré sommable puisque $u$ appartient à $\mathscr{L}_2(E; F)$ (cor. 4 de IV, p. 165). Soit $(e_j)_{j\in J}$ une base orthonormale de E qui prolonge $(e_i)_{i\in I}$.

Soit L une partie finie de I. Soit $v_L$ l’application linéaire continue de rang fini de E dans F définie par

$$
v_L(x) =\sum_{i\in L}\langle e_i|x\rangle f_i
$$

pour tout $x$ dans E. On a $\|v_L\|\leqslant 1$ et $v_L\in \mathscr{L}_2(E; F)$. De plus, pour tout $j\in J$, on a $v_L(e_j) = 0$ si $j /\in L$ et $v_L(e_j) =f_j$ si $j\in L$. Ainsi

$|\langle v_L|u\rangle |=|$Tr($v^*_Lu$)$|=\sum_{j\in J}\langle v_L(e_j)|u(e_j)\rangle =\sum_{j\in L}\alpha_j$.

D’après loc. cit., on en déduit que

(10) $\|u\|_1=$ sup$_L\sum_{j\in L}\alpha_j\leqslant_{v\in\mathscr{L}}$sup$_{_2(E;F)}|\langle v|u\rangle |$

$\|v\|\leqslant 1$

dans $\mathbf{R}_+\cup  \{+\infty \}$.

Cela implique l’égalité de la proposition lorsque $\|u\|_1= +\infty$.

Supposons que $\|u\|_1$ est fini. Pour tout $i\in I$, soit $p_i$ l’application linéaire de E dans F telle que $p_i(e_i) =f_i$ et $p_i(x) = 0$ pour tout $x\in e^{\circ}_i$. Pour tous $j$ et $k$ dans I, on a

$\langle p_j|p_k\rangle =$ Tr($p^*_jp_k$) $=\sum_{i\in J}\langle p_j(e_i)|p_k(e_i)\rangle$,

qui est nul sauf si $j=k$, auquel cas cette quantité vaut $\|f_k\|^2= 1$. La famille $(p_i)_{i\in I}$ est donc orthonormale dans $\mathscr{L}_2(E; F)$. Par conséquent, la famille $(\alpha_ip_i)_{i\in I}$ est sommable dans $\mathscr{L}_2(E; F)$; sa somme est égale à $u$ puisque ces deux applications linéaires continues coïncident sur les éléments $e_i$ pour tout $i\in J$.

Soit $v\in \mathscr{L}_2(E; F)$. Pour tout $i\in I$, il vient

$\langle v|p_i\rangle =$ Tr($v^*p_i$) $=\sum_{j\in J}\langle v(e_j)|p_i(e_j)\rangle =\langle v(e_i)|f_i\rangle$.

Si $\|v\|\leqslant 1$, on majore alors

$$
|\langle v|u\rangle |=\langle v|\sum_{i\in I}\alpha_ip_i\rangle \leqslant \sum_{i\in I}\alpha_i|\langle v|p_i\rangle |
$$

$=\sum_{i\in I}\alpha_i|\langle v(e_i)|f_i\rangle |\leqslant \sum_{i\in I}\alpha_i=$ Tr($|u|$),

d’où l’inégalité

sup $|\langle v|u\rangle |\leqslant \|u\|_1$,

$v\in \mathscr{L}_2(E;F)$

$$
\|v\|\leqslant 1
$$

ce qui, combiné avec la formule (10), conclut la preuve de la proposition.

Il résulte de cette proposition que l’ensemble $\mathscr{L}_1(E; F)$ des applications linéaires continues $u$ de E dans F telles que $\|u\|_1$ est fini est un sous-espace vectoriel de $\mathscr{L}_2(E; F)$ et que l’application $u\mapsto  \|u\|_1$ est une semi-norme sur $\mathscr{L}_1(E; F)$; l’inégalité (9) démontre que c’est une norme.

#### Définition 4 {#ts-iv-s1-def-4 .statement tag=02XF}

On dit que l’espace vectoriel $\mathscr{L}_1(E; F)$ muni de la norme $u\mapsto  \|u\|_1$ est l’espace des applications nucléaires de E dans F. Si $u\in \mathscr{L}_1(E; F)$, on dit que $u$ est nucléaire.

#### Remarque 1 {#ts-iv-s1-n8-rem-1 .statement tag=02XG}

Supposons que $K =\mathbf{R}$. Soit $u\in \mathscr{L}(E; F)$. On a $u\in \mathscr{L}_1(E; F)$ si et seulement si $u_{(\mathbf{C})}\in \mathscr{L}_1(E_{(\mathbf{C})}; F_{(\mathbf{C})})$; dans ce cas, on a $\|u\|_1=\|u_{(\mathbf{C})}\|_1$.

#### Remarque 2 {#ts-iv-s1-n8-rem-2 .statement tag=02XH}

Soit $u$ une application nucléaire de E dans F. L’application $u$ étant de Hilbert–Schmidt, elle est compacte (cor. 2 de IV, p. 165). De plus, la proposition 14 implique que pour tout $v\in \mathscr{L}_2(E; F)$, on a

$$
|\langle v|u\rangle |\leqslant \|v\| \|u\|_1 \tag{11}
$$

#### Remarque 3 {#ts-iv-s1-n8-rem-3 .statement tag=02XI}

Supposons que $K =\mathbf{C}$. Soit $u\in \mathscr{L}_1(E; E)$ tel que $u$ est positif. La norme $\|u\|_1$ de $u$ est la somme de la suite $(\lambda_n(u))_{n\in I_E}$ (cor. 3 de IV, p. 165).

#### Remarque 4 {#ts-iv-s1-n8-rem-4 .statement tag=02XJ}

L’inclusion canonique de $\mathscr{L}_1(E; F)$ dans $\mathscr{L}(E; F)$ est de norme $\leqslant 1$ (inégalité (9), p. 167).

#### Proposition 15 {#ts-iv-s1-prop-15 .statement tag=02XK}

Soit G un espace hilbertien sur K. L’application $(u, v)\mapsto v\circ u$ de $\mathscr{L}(E; F)\times \mathscr{L}(F; G)$ dans $\mathscr{L}(E; G)$ définit par passage aux sous-espaces une application bilinéaire continue de norme $\leqslant 1$ de $\mathscr{L}_2(E; F)\times \mathscr{L}_2(F; G)$ dans $\mathscr{L}_1(E; G)$.

Soient $u\in \mathscr{L}_2(E; F)$ et $v\in \mathscr{L}_2(F; G)$. Soit $w\in \mathscr{L}_2(E; G)$. Il vient $\langle uv|w\rangle =$ Tr($v^*u^*w$) $=\langle v|u^*w\rangle$ d’où

$$
|\langle uv|w\rangle |\leqslant \|v\|_2\|u^*w\|_2\leqslant \|v\|_2\|u\|_2\|w\|
$$

d’après l’inégalité de Cauchy–Schwarz et la formule (37) de EVT, V, p 52. Le résultat découle donc de la prop. 14.

#### Lemme 8 {#ts-iv-s1-lem-8 .statement tag=02XL}

L’application $u\mapsto u^*$ de $\mathscr{L}(E; F)$ dans $\mathscr{L}(F; E)$ définit par passage aux sous-espaces une application linéaire isométrique de $\mathscr{L}_1(E; F)$ dans $\mathscr{L}_1(F; E)$.

Soit $u\in \mathscr{L}_1(E; F)$. Comme $u$ est une application de Hilbert–Schmidt, il en est de même de $u^*$ (EVT, V, p. 54). L’application $v\mapsto v^*$ est une bijection de l’ensemble des $v\in \mathscr{L}_2(E; F)$ tels que $\|v\|\leqslant 1$ dans l’ensemble des $w\in \mathscr{L}_2(F; E)$ tels que $\|w\|\leqslant 1$; pour tout $v\in \mathscr{L}_2(E; F)$ avec $\|v\|\leqslant 1$, on a $\langle v|u\rangle =\langle u^*|v^*\rangle$ (EVT, V, p. 54, formule (42)), d’où le résultat d’après la prop. 14.

#### Proposition 16 {#ts-iv-s1-prop-16 .statement tag=02XM}

Soient $E_1$ et $F_1$ des espaces hilbertiens. Soient $u$ dans $\mathscr{L}_1(E; F),v$ dans $\mathscr{L}(E_1; E)$ et $v_2$ dans $\mathscr{L}(F; F_1)$. On a alors $v_2uv_1\in \mathscr{L}_1(E_1; F_1)$ et $\|v_2uv_1\|_1\leqslant \|v_2\| \|v_1\| \|u\|_1$.

Soit $w\in \mathscr{L}_2(E; F_1)$ tel que $\|w\|\leqslant 1$. On a $v_2u\in \mathscr{L}_2(E; F_1)$ (EVT, V, p. 52, formule (36)). Comme $v^*_2w\in \mathscr{L}_2(E; F) ($loc. cit.), il vient

$$
|\langle w|v_2u\rangle |=|\langle v^*_2w|u\rangle |\leqslant \|v_2\| \|u\|_1
$$

(formule (11)), d’où $v_2u\in \mathscr{L}_1(E; F_1)$ et $\|v_2u\|_1\leqslant \|v_2\|\|u\|_1$ (prop. 14).

Soit $v_1\in \mathscr{L}(E_1; E)$; puisque $uv_1= (v^*_1u^*)^*$, on a $uv_1\in \mathscr{L}_1(E_1; F)$ et $\|uv_1\|_1\leqslant \|v^*_1\| \|u^*\|_1=\|v_1\| \|u\|_1$ (lemme 8).

La proposition résulte aussitôt de ces inégalités.

#### Proposition 17 {#ts-iv-s1-prop-17 .statement tag=02XN}

L’espace $\mathscr{L}_1(E; E)$ coïncide avec l’espace $\mathscr{L}_1(E)$ des endomorphismes de trace finie de E, et on a $|$Tr($u$)$|\leqslant \|u\|_1$ pour tout endomorphisme $u$ de E de trace finie.

On peut supposer que $K =\mathbf{C}$. L’espace $\mathscr{L}_1(E; E)$ contient par définition l’ensemble des endomorphismes positifs de trace finie, et donc $\mathscr{L}_1(E)\subset \mathscr{L}_1(E; E)$ (EVT, p. 50, déf. 8). Réciproquement, démontrons que $\mathscr{L}_1(E; E)$ est contenu dans $\mathscr{L}_1(E)$.

Soit $u\in \mathscr{L}_1(E; E)$. On a $u^*\in \mathscr{L}_1(E; E)$ (lemme 8) ; il suffit donc de démontrer que les éléments hermitiens de $\mathscr{L}_1(E; E)$ sont de trace finie (lemme 2 de I, p. 96).

Soit $u$ un tel endomorphisme. Il est compact (remarque 2, p. 169). Soit B une base orthonormale de E telle que $u$ soit diagonal dans la base B (th. 1 de IV, p. 149) et soit $\lambda$ la famille des valeurs propres de $u$ relativement à B. L’endomorphisme $|u|$ est diagonalisable dans la base B et la famille de ses valeurs propres est $|\lambda |$ (prop. 1, d) de IV, p. 147). Puisque $|u|$ est de trace finie, cette dernière famille est sommable (prop. 12 de IV, p. 164), donc la famille $\lambda$ est sommable. Par conséquent, $u$ est de trace finie (loc. cit.), et on a $|$Tr($u$)$|\leqslant$ Tr($|u|$) $=\|u\|_1$.

En conséquence, l’espace $\mathscr{L}_1(E)$ est un idéal bilatère auto-adjoint de l’algèbre stellaire $\mathscr{L}(E)$. Si E est de dimension infinie, cet idéal n’est pas fermé dans $\mathscr{L}(E)$.

Les propositions 17 et 16 démontrent que l’application $b$ de $\mathscr{L}_1(E; F)\times \mathscr{L}(F; E)$ dans $\mathbf{C}$ définie par $b(u, v) =$ Tr($vu$) est une forme bilinéaire continue qui met les espaces $\mathscr{L}_1(E; F)$ et $\mathscr{L}(F; E)$ en dualité.

#### Lemme 9 {#ts-iv-s1-lem-9 .statement tag=02XO}

Soit $u\in \mathscr{L}_1(E; F)$. On a

$\|u\|_1=$ sup $|b(u, v)|$.

$v\in \mathscr{L}^c(F;E)$

$$
\|v\|\leqslant 1
$$

Puisque toute application de Hilbert–Schmidt est compacte (cor. 2 de IV, p. 165), on a

$\|u\|_1\leqslant_{v\in\mathscr{L}}$sup$_{_c(E;F)}|$Tr($vu$)$|=_{v\in\mathscr{L}}$sup$_{_c(F;E)}|b(u, v)|$

$\|v\|\leqslant 1\|v\|\leqslant 1$

d’après la prop. 14.

Soit $v\in \mathscr{L}^c(E; F)$ de norme $\leqslant$ 1. Comme $\mathscr{L}_2(E; F)$ est dense dans $\mathscr{L}^c(E; F)$, il existe une suite $(v_n)_{n\in\mathbf{N}}$ dans $\mathscr{L}_2(E; F)$ qui converge vers $v$ dans $\mathscr{L}(E; F)$. La suite $(b(u, v_n))_{n\in\mathbf{N}}$ converge vers $b(u, v)$; comme $|b(u, v_n)|$ = $|$Tr($v_nu$)$|$ = $|\langle v_n^*|u\rangle |\leqslant \|u\|_1$ (prop. 14) pour tout $n\in \mathbf{N}$, il en résulte que $|b(u, v)|\leqslant \|u\|_1$.

Notons $\theta$ l’application linéaire continue

$$
\theta :\mathscr{L}_1(E; F)\rightarrow \mathscr{L}^c(F; E)'
$$

telle que $\theta (u)(v) =b(u, v)$.

#### Proposition 18 {#ts-iv-s1-prop-18 .statement tag=02XP}

L’application $\theta$ est un isomorphisme isométrique.

D’après le lemme 9, l’application $\theta$ est isométrique, et il suffit de démontrer que $\theta$ est surjective.

Soit $\lambda \in \mathscr{L}^c(F; E)'$. Puisque $\|v\|\leqslant \|v\|_2$ pour tout $v\in \mathscr{L}_2(F; E)$ (EVT, V, p. 52, formule (33)), la restriction de $\lambda$ au sous-espace $\mathscr{L}_2(F; E)$ est une forme linéaire continue sur l’espace hilbertien $\mathscr{L}_2(F; E)$. Il existe donc un élément $u$ de $\mathscr{L}_2(F; E)$ tel que $\lambda (v) =\langle u|v\rangle$ pour tout $v\in \mathscr{L}_2(F; E)$ (EVT, V, p. 15, th. 3).

Pour tout $w\in \mathscr{L}_2(E; F)$ de norme $\leqslant 1$, on a $|\langle w|u\rangle |=|\lambda (w)|\leqslant \|\lambda \|$. Par conséquent, $u$ est une application nucléaire de E dans F (prop. 14).

Les formes linéaires continues $\lambda$ et $\theta (u)$ sont égales sur le sous-espace dense $\mathscr{L}_2(F,E)$ de $\mathscr{L}^c(F; E)$. Il en résulte que $\lambda =\theta (u)$, ce qui conclut la démonstration.

#### Corollaire {#ts-iv-s1-n8-cor-1 .statement tag=02XQ}

L’espace normé $\mathscr{L}_1(E; F)$ est un espace de Banach.

L’assertion résulte de la proposition et de EVT, III, p. 24, cor. 2 puisque l’espace $\mathscr{L}^c(F; E)$ est un espace normé.

### 9. Opérateurs intégraux de Hilbert–Schmidt

Dans ce numéro, X et Y sont des espaces topologiques localement compacts. Soient $\mu$ une mesure positive sur X et $\nu$ une mesure positive sur Y. On note $L^2$(X), $L^2(Y)$ et $L^2(X\times Y)$ les espaces $L^2(X, \mu), L^2(Y, \nu )$ et $L^2(X\times Y, \mu\otimes \nu )$ respectivement, et de même pour $\mathscr{L}^2$(X), $\mathscr{L}^2(Y)$ et $\mathscr{L}^2(X\times Y)$.

On rappelle (cf. n$^o4$ de III, p. 26) que pour tout $N\in \mathscr{L}^2(X\times Y)$, il existe une unique application linéaire continue $u_N$ de $L^2(X)$ dans $L^2(Y)$ telle que

$$
\langle g|u_N(f)\rangle =\int_{X\times Y}g(y)N(x, y)f(x)d(\mu\otimes \nu )(x, y) \tag{12}
$$

pour tout $f\in L^2(X)$ et tout $g\in L^2(Y)$. L’application $u_N$ est compacte (cor. 1 de III, p. 33). L’application $N\mapsto u_N$ induit par passage aux quotients une application linéaire continue et injective de $L^2(X\times Y)$ dans $\mathscr{L}(L^2(X); L^2(Y))$ (prop. 5 de III, p. 30).

On note $\theta$ l’unique application linéaire de $\mathscr{L}^2(X)\otimes \mathscr{L}^2(Y)$ dans $\mathscr{L}^2(X\times Y)$ qui pour tous $f\in \mathscr{L}^2(X)$ et $g\in \mathscr{L}^2(Y)$ associe à $f\otimes g$ la fonction définie par $(x, y)\mapsto f(x)g(y)$.

#### Lemme 10 {#ts-iv-s1-lem-10 .statement tag=02XR}

L’application $\theta$ définit par passage aux quotients une application linéaire $\widetilde{\theta}$ de $L^2(X)\otimes L^2(Y)$ dans $L^2(X\times Y)$, et il existe un unique isomorphisme isométrique de $L^2(X)\widehat{\otimes}_2L^2(Y)$ sur $L^2(X\times Y)$ qui coïncide avec celle-ci sur $L^2(X)\otimes L^2(Y)$.

La première assertion est élémentaire. Démontrons la seconde.

Soient $(f_i)_{i\in I}$ et $(g_j)_{j\in J}$ des bases orthonormales de $L^2(X)$ et $L^2$(Y), respectivement. La famille $(f_i\otimes g_j)_{(i,j)\in I\times J}$ est une base orthonormale de $L^2(X)\widehat{\otimes}_2L^2(Y)$ (EVT, V, p. 29, cor. 1) et la famille $(\widetilde{\theta}(\overline{f}_i\otimes g_j))_{(i,j)\in I\times J}$ est orthonormale dans $L^2(X\times Y)$ (INT, V, p. 95, § 8, n$^o3$, cor. 2). L’application $\widetilde{\theta}$ s’étend donc par continuité en une application linéaire isométrique de $L^2(X)\widehat{\otimes}_2L^2(Y)$ dans $L^2(X\times Y)$. Il reste à démontrer que cette extension est surjective.

Pour cela il suffit de prouver que l’image de $\widetilde{\theta}$ est dense dans $L^2(X\times Y)$. Soit N un élément de $L^2(X\times Y)$ orthogonal à l’image de $\widetilde{\theta}$. Pour tous $i\in I$ et $j\in J$, on a $\langle g_j|u_N(f_i)\rangle =\langle \widetilde{\theta}(f_i\otimes g_j)|N\rangle = 0$ (formule (12)), d’où $u_N= 0$, et donc N = 0.

Le lemme précédent établit l’assertion énoncée dans EVT, V, p. 29, exemple 2.

On identifiera dans la suite $L^2(X)\widehat{\otimes}_2L^2(Y)$ et $L^2(X\times Y)$ par l’isomorphisme isométrique du lemme 10.

#### Proposition 19 {#ts-iv-s1-prop-19 .statement tag=02XS}

L’application $N\mapsto u_N$ est un isomorphisme isométrique de $L^2(X\times Y)$ sur l’espace $\mathscr{L}_2(L^2(X); L^2(Y))$ des applications de Hilbert–Schmidt de $L^2(X)$ dans $L^2(Y)$.

L’application linéaire de $L^2(Y)\otimes L^2(X)$ dans $\mathscr{L}_2(L^2(X); L^2(Y))$ qui associe à $g\otimes f$ l’application de Hilbert–Schmidt $h\mapsto  \langle f|h\rangle g$ se prolonge en un isomorphisme isométrique $\theta_1$ de $L^2(Y)\widehat{\otimes}_2L^2(X)$ sur $\mathscr{L}_2(L^2(X); L^2(Y))$ (EVT, V, p. 52, th. 1).

Notons par ailleurs $\theta_2$ l’isomorphisme isométrique de $L^2(X)\widehat{\otimes}_2L^2(Y)$ sur $L^2(Y)\widehat{\otimes}_2L^2(X)$ qui à $f\otimes g$ associe $g\otimes \overline{f}$ pour tout $f\in L^2(X)$ et tout $g\in L^2(Y)$.

L’application linéaire $\theta_3=\theta_1\circ \theta_2$ s’identifie à un isomorphisme isométrique de $L^2(X\times Y)$ sur $\mathscr{L}_2(L^2(X); L^2(Y))$.

Soient $f\in L^2(X)$ et $g\in L^2$(Y), et soit N l’élément de $L^2(X\times Y)$ identifié à $f\otimes g$. D’après INT, V, p. 95, § 8, n$^o3$, cor. 2 et la formule (12) on a

$$
\langle g_1|u_N(f_1)\rangle =\langle \overline{f}|f_1\rangle  \langle g_1|g\rangle
$$

pour tous $f_1\in L^2(X)$ et $g_1\in L^2(Y)$. L’application $u=\theta_3(N)$ est l’application linéaire $\theta_1(g\otimes f)$; elle vérifie donc $u(h) =\langle f|h\rangle g$ pour tout $h\in L^2(X)$. Par conséquent, quels que soient $f_1\in L^2(X)$ et $g_1\in L^2$(Y), il vient

$$
\langle g_1|u(h_1)\rangle =\langle \overline{f}|h_1\rangle  \langle g_1|g\rangle =\langle g_1|u_N(h_1)\rangle
$$

d’où $\theta_3(N) =u_N$. Puisque $\theta_3$ et $N\mapsto u_N$ sont continues, on conclut que $\theta_3(N) =u_N$ pour tout $N\in L^2(X\times Y)$, ce qui conclut la preuve.

#### Corollaire {#ts-iv-s1-n9-cor-1 .statement tag=02XT}

Pour tout $N\in L^2(X\times Y)$, l’application linéaire $u_N$ est une application de Hilbert–Schmidt et on a Tr($u^*_Nu_N$) $=\|N\|^2$.

En effet, on a $\|u\|_2=$ Tr($u^*u$) pour tout $u\in \mathscr{L}_2(L^2(X); L^2(Y))$.

#### Remarque {#ts-iv-s1-n9-rem-1 .statement tag=02XU}

Soit $N\in L^2(X\times Y)$. D’après le corollaire 2 de IV, p. 150, il existe un ensemble dénombrable I, des familles orthonormales $(f_i)_{i\in I}$ dans $L^2(X)$ et $(g_i)_{i\in I}$ dans $L^2$(Y), ainsi qu’une famille $(\alpha_i)_{i\in I}$ dans $\mathbf{R}^*_+$, tels que

$$
u_N(f) =\sum_{i\in I}\alpha_i\langle f_i|f\rangle g_i
$$

pour tout $f\in L^2$(X), où la série converge dans $L^2(Y)$. D’après le cor. 4 de IV, p. 165 et le corollaire ci-dessus, on a

$\sum_{i\in I}\alpha^2_i=$ Tr($u^*_Nu_N$) $=\|u_N\|^2_2=\int_{X\times Y}|N(x, y)|^2d(\mu\otimes \nu )(x, y)$.

Notons de plus $h_{i,j}=\overline{f}_i\otimes g_j\in L^2(X\times Y)$ pour tout $(i, j)\in I\times I$. On a alors

$$
N =\sum_{i\in I}\alpha_ih_{i,i}
$$

dans $L^2(X\times Y)$.

En effet, soient $(f_j)_{j\in J}$ et $(g_k)_{k\in K}$ des bases orthonormales de $L^2(X)$ et $L^2$(Y), respectivement, prolongeant les familles $(f_i)_{i\in I}$ et $(g_i)_{i\in I}$. Posons $h_{j,k}=f_j\otimes g_k$ pour tout $(j, k)\in J\times K$. D’après le lemme 10, la famille $(h_{j,k})_{(j,k)\in J\times K}$ est une base orthonormale de $L^2(X\times Y)$. On a $\langle h_{j,k}|N\rangle =\langle g_k|u_N(f_j)\rangle$ pour tout $(j, k)\in J\times K$. Si $j /\in I$, cette quantité est nulle. Si $j\in I$, elle est égale à $\alpha_j\langle g_k|g_j\rangle$, donc est nulle sauf si $k=j$, auquel cas $\langle h_{j,j}|N\rangle =\alpha_j$. Par conséquent

$$
N =\sum_{(j,k)\in J\times K}\langle h_{j,k}|N\rangle h_{j,k}=\sum_{i\in I}\alpha_ih_{i,i}
$$

### 10. Trace des opérateurs intégraux à noyau continu

Dans ce numéro, on garde les conventions du numéro précédent avec Y = X et $\nu =\mu$. On suppose que X est un espace topologique localement compact dénombrable à l’infini (TG, I, p. 68, déf. 5).

En particulier, on identifie les espaces $L^2(X\times X)$ et $L^2(X)\widehat{\otimes}_2L^2(X)$ (lemme 10 de IV, p. 172). On notera $\widetilde{f}$ la classe dans $L^2(X)$ (resp. dans $L^2(X\times X))$ d’une fonction $f\in \mathscr{L}^2(X)$ (resp. dans $\mathscr{L}^2(X\times X))$.

#### Proposition 20 {#ts-iv-s1-prop-20 .statement tag=02XV}

Soit $(f_n)_{n\in\mathbf{N}}$ une suite d’applications mesurables de X dans un espace métrisable F. On suppose que la limite de $f_n(x)$ existe dans le complémentaire d’une partie $\mu$-négligeable de X. Il existe une suite $(C_m)_{m\in\mathbf{N}}$ de parties compactes de X dont la réunion $\widetilde{X}$ vérifie $|\mu|(X-\widetilde{X}) = 0$, telle que les fonctions $f_n$ sont continues dans $C_m$ pour tout $n\in \mathbf{N}$ et tout $m\in \mathbf{N}$, et la suite $(f_n)_{n\in\mathbf{N}}$ converge uniformément vers $f$ dans $C_m$ pour tout $m\in \mathbf{N}$.

Il résulte du th. 2 de INT, IV, p. 175, § 5, n$^o4$ et de la prop. 12, b) de INT, IV, p. 188, § 5, n$^o8$, que l’ensemble des parties compactes C de X telles que les fonctions $f_n$ sont continues dans C pour tout $n$, et que $(f_n)$ converge uniformément vers $f$ dans C, est $\mu$-dense dans X (INT, IV, p. 189, § 5, n$^o8$, déf. 6). L’assertion résulte alors de la remarque de INT, IV, p. 189, §5, n$^o8$.

Soit N une fonction appartenant à $\mathscr{L}^2(X\times X)$ et $u_N$ l’application de Hilbert–Schmidt de $L^2(X)$ dans $L^2(X)$ de noyau N (prop. 19 de IV, p. 173). Puisque l’application $u_N$ est compacte, il existe d’après la prop. 9 de IV, p. 156 un élément M de $\mathbf{N}$ et, en notant I l’ensemble des entiers $n\in \mathbf{N}$ tels que $n\leqslant M$, des familles orthonormales $(f_i)_{i\in I}$ et $(g_i)_{i\in I}$ dans $\mathscr{L}^2(X)$ et une famille $(\alpha_i)_{i\in I}$ dans $\mathbf{R}^*_+$ telles que

$$
u_N(f) =\sum_{i\in I}\alpha_i\langle \widetilde{f}_i|f\rangle \widetilde{g}_i \tag{13}
$$

pour tout $f\in L^2$(X), où la série converge dans $L^2(X)$.

Pour tout $i\in I$, on note $h_i\in \mathscr{L}^2(X\times X)$ la fonction définie par $h_i(x, y) =f_i(x)g_i(y)$, de sorte que $\widetilde{h}_i$ est la classe de $f_i\otimes g_i$. D’après la remarque 9 de IV, p. 173, la série de terme général $\alpha_ih_i$ converge vers N dans $L^2(X\times X)$.

Dans la suite de ce numéro, on suppose que N est une fonction continue.

#### Proposition 21 {#ts-iv-s1-prop-21 .statement tag=02XW}

Supposons que $u_N$ est de trace finie. Il existe alors un ensemble $\widetilde{X}\subset X$ dont le complémentaire X $-\widetilde{X}$ est $\mu$-négligeable et une fonction $H\in \mathscr{L}^2(X\times X)$ vérifiant les conditions suivantes :

(i) Pour tout $(x, y)\in \widetilde{X}\times \widetilde{X}$, la famille $(\alpha_if_i(x)g_i(y))_{i\in I}$ est sommable dans $\mathbf{C}$ et sa somme est $N(x, y)$;

(ii) Pour toute partie finie J de I et tout $(x, y)\in \widetilde{X}\times \widetilde{X}$, on a

$$
\sum_{i\in J}\alpha_ih_i(x, y)\leqslant H(x, y) \tag{14}
$$

(iii) La fonction $x\mapsto H(x, x)$ appartient à $\mathscr{L}^1(X)$.

Puisque $u_N$ est de trace finie, la famille $(\alpha_i)$ est sommable (cor. 4 de IV, p. 165). Les séries

$$
\sum_{i\in I}\alpha_i|f_i|^2,\sum_{i\in I}\alpha_i|g_i|^2
$$

convergent donc dans $\mathscr{L}^1(X)$ et par suite $\mu$-presque partout (INT, IV, p. 128, § 3, n$^o3$, prop. 6). Notons F et G, respectivement, les fonctions définies $\mu$-presque partout par la somme de ces séries, en posant $F(x) = 0$ et $G(x) = 0$ pour tout $x$ tel que la série correspondante ne converge pas. Comme F et G appartiennent à $\mathscr{L}^1$(X), la fonction H définie par $H(x, y) =F(x)G(y)$ appartient à $\mathscr{L}^2(X\times X)$ (INT, V, p. 95, § 8, n$^o3$, cor. 2).

Appliquons la prop. 20 à l’espace X, à $F =\mathbf{C}^2$, et aux applications mesurables

$$
s_n:x\mapsto \sum_{i\in I}\alpha_i|f_i(x)|^2,\sum_{i\in I}\alpha_i|g_i(x)|^2
$$

$i\leqslant ni\leqslant n$

définies sur X. Il existe donc une suite $(C_m)_{m\in\mathbf{N}}$ de parties compactes de X vérifiant les conditions suivantes :

(1) la réunion $\widetilde{X}$ vérifie $\mu(X-\widetilde{X}) = 0$;

(2) pour tout $m\in \mathbf{N}$ et tout $n\in \mathbf{N}$, les fonctions $s_n$ sont continues dans $C_m$;

(3) pour tout $m\in \mathbf{N}$, les séries $\sum\alpha_i|f_i|^2$ et $\sum\alpha_i|g_i|^2$ convergent uniformément sur $C_m$ vers F et G, respectivement ;

(4) le support de la mesure induite par $\mu$ sur $C_m$ est égal à $C_m$ (quitte à remplacer $C_m$ par le support de cette mesure).

Démontrons que l’ensemble $\widetilde{X}$ et la fonction H vérifient les conditions (i), (ii) et (iii).

Soit $(x, y)\in \widetilde{X}\times \widetilde{X}$. Pour tout sous-ensemble fini $J\subset I$, on a

$1/21/2$

(15) $\sum_{i\in J}\alpha_i\overline{f_i(x)}g_i(y)\leqslant \sum_{i\in J}\alpha_i|f_i(x)|^2\sum_{i\in J}\alpha_i|g_i(y)|^2$

d’où également

$$
\sum_{i\in J}\alpha_i\overline{f_i(x)}g_i(y)\leqslant H(x, y) \tag{16}
$$

ce qui établit dores et déjà la propriété (ii).

D’après l’inégalité (15), la série $\sum_i\alpha_ih_i$ converge uniformément sur $K_m\times K_n$ pour tout $(m, n)\in \mathbf{N}^2$. Soit $\widetilde{N}$ la fonction sur $X\times X$ définie par

$$
\widetilde{N}(x, y) =\sum_{i\in I}\alpha_ih_i(x, y) =\sum_{i\in I}\alpha_i\overline{f_i(x)}g_i(y)
$$

pour tout $(x, y)\in \widetilde{X}\times \widetilde{X}$ et par $\widetilde{N}(x, y) = 0$ sinon. La fonction $\widetilde{N}$ est mesurable (INT, IV, p. 175, § 5, n$^o4$, th. 2), et elle est continue sur $K_m\times K_n$ pour tout $(m, n)\in \mathbf{N}^2$.

D’après (16), on a $|\widetilde{N}(x, y)|\leqslant H(x, y)$ pour tout $(x, y)\in X\times X$, et en particulier $\widetilde{N}$ appartient à $\mathscr{L}^2(X\times X)$ (INT, IV, p. 84, § 5, n$^o6$, th. 5).

Démontrons que $N =\widetilde{N}$ sur $\widetilde{X}\times \widetilde{X}$, ce qui établira la propriété (i). Soient $f$ et $g$ des éléments de $\mathscr{L}^2(X)$. On a

$$
\langle g|u_{\widetilde{N}}(f)\rangle =\int_{X\times X}\widetilde{N}(x, y)f(x)\overline{g(y)}d(\mu\otimes \mu)(x, y)
$$

(formule (12) de IV, p. 172). Pour tout $(x, y)\in \widetilde{X}\times \widetilde{X}$ et toute partie finie J de I, on a

$$
\sum_{i\in J}\alpha_i\overline{f_i(x)}g_i(y)f(x)\overline{g(y)}\leqslant |f(x)g(y)|H(x, y)
$$

par la formule (16). Comme le membre de droite de cette inégalité est intégrable sur $X\times X$ (INT, V, p. 95, § 8, n$^o3$, cor. 2), on peut appliquer le théorème de Lebesgue (INT, IV, p. 137, § 3, n$^o7$, th. 6) et la formule (13) pour en déduire que

$$
\langle g|u_{\widetilde{N}}(f)\rangle =\sum_{i\in I}\alpha_i\int_{X\times X}\overline{f_i(x)}g_i(y)f(x)\overline{g(y)}d(\mu\otimes \mu)(x, y)
$$

$$
=\sum_{i\in I}\alpha_i\langle f_i|f\rangle \langle g|g_i\rangle =\langle g|u_N(f)\rangle
$$

Par conséquent, il vient $u_{\widetilde{N}}=u_N$, d’où $N =\widetilde{N}$ dans $L^2(X\times X)$ (prop. 3 de III, p. 28, b)).

Pour tout $(m, n)\in \mathbf{N}^2$, les fonctions N et $\widetilde{N}$ sont continues dans $K_m\times K_n$ donc sont égales sur $K_m\times K_n$ (prop. 9 de INT, III, p. 69, § 2, n$^o2)$ puisque le support de la mesure induite par $\mu\otimes \mu$ sur $K_m\times K_n$ est égal à $K_m\times K_n$. Donc N coïncide avec $\widetilde{N}$ sur $\widetilde{X}\times \widetilde{X}$.

$$
\surd
$$

Finalement, la majoration FG $\leqslant (F + G)/2$ entraîne que la fonction $x\mapsto F(x)G(x) = H(x, x)$ est intégrable sur X, d’où la propriété (iii).

Dans la suite de ce numéro, on garde les notations de la proposition.

#### Théorème 2 {#ts-iv-s1-thm-2 .statement tag=02XX}

Supposons que $u_N$ est de trace finie. Alors la fonction $x\mapsto N(x, x)$ appartient à $\mathscr{L}^1(X)$ et l’on a

Tr($u_N$) $=\int_XN(x, x)d\mu(x)$.

D’après les conditions (i) et (ii), on a $|N(x, x)|\leqslant H(x, x)$ pour $x\in \widetilde{X}$, donc la fonction $x\mapsto N(x, x)$ appartient à $\mathscr{L}^1(X)$ d’après la condition (iii).

La condition (i) démontre l’égalité

$$
N(x, x) =\sum_{i\in I}\alpha_i\overline{f_i(x)}g_i(x)
$$

pour tout $x\in \widetilde{X}$. D’après les conditions (ii) et (iii), on peut appliquer le théorème de Lebesgue (INT, IV, p. 137, § 3, n$^o7$, th. 6), dont il résulte que

$$
\int_XN(x, x)d\mu(x) =\sum_{i\in I}\alpha_i\int_X\overline{f_i(x)}g_i(x)d\mu(x)
$$

$=\sum_{i\in I}\alpha_i\langle f_i|g_i\rangle =$ Tr($u_N$),

la dernière égalité résultant du cor. de la prop. 17 de IV, p. 170.

#### Lemme 11 {#ts-iv-s1-lem-11 .statement tag=02XY}

Si l’endomorphisme $u_N$ de $L^2(X)$ est positif, alors $N(x, x)\geqslant 0$ pour tout $x$ dans le support de $\mu$.

Puisque $u_N$ est positif, les familles $(f_i)$ et $(g_i)$ peuvent être choisies de sorte que $f_i=g_i$ pour tout $i\in I$ (remarque 3 de IV, p. 151). Pour tout $x\in \widetilde{X}$, on a alors

$$
N(x, x) =\sum_{i\in I}\alpha_i|f_i(x)|^2\geqslant 0
$$

Puisque N est continue, et que $\mu(X-\widetilde{X}) = 0$, la fonction N est positive sur le support de $\mu$.

#### Remarque {#ts-iv-s1-n10-rem-1 .statement tag=02XZ}

L’assertion réciproque du lemme n’est pas valide (exercice 14 de IV, p. 316).

#### Proposition 22 {#ts-iv-s1-prop-22 .statement tag=02Y0}

On suppose que $u_N$ est un endomorphisme positif de $L^2(X)$. Alors l’endomorphisme $u_N$ est de trace finie si et seulement si la fonction $x\mapsto N(x, x)$ est $\mu$-intégrable. Dans ce cas, on a

Tr($u_N$) $=\int_XN(x, x)d\mu(x)$.

Si $u_N$ est de trace finie, le théorème 2 implique que $x\mapsto N(x, x)$ est intégrable sur X et que son intégrale est la trace de $u_N$.

Réciproquement, supposons que la fonction $x\mapsto N(x, x)$ est intégrable. Puisque $u_N$ est positif, les familles orthonormales $(f_i)_{i\in I}$ et $(g_i)_{i\in I}$ peuvent être choisies de sorte que $f_i=g_i$ pour tout $i\in I$ (remarque 3 de IV, p. 151). Pour tout $x\in \widetilde{X}$, on a

$$
N(x, x) =\sum_{i\in I}\alpha_i|f_i(x)|^2
$$

d’où, pour toute partie finie J de I, on déduit

$$
\sum_{i\in J}\alpha_i=\sum_{i\in J}\alpha_i\int_X|f_i(x)|^2d\mu(x)
$$

$$
=\int_X\sum_{i\in J}\alpha_i|f_i(x)|^2d\mu(x)\leqslant \int_XN(x, x)d\mu(x)
$$

La famille $(\alpha_i)_{i\in I}$ est donc sommable, ce qui implique que l’endomorphisme $u_N$ est de trace finie (prop. 12 de IV, p. 164).

#### Remarque {#ts-iv-s1-n10-rem-2 .statement tag=02Y1}

Même lorsque X est compact et N continu, l’endomorphisme $u_N$ de $L^2(X)$ n’est pas toujours de trace finie (cf. exercice 8 de IV, p. 314).

## EXERCICES {#ts-iv-s1-exercises}

See the [exercises for § 1](exercises/s1/).
