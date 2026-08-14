---
book: ts
book_title: Théories spectrales
chapter: I
chapter_title: ALGÈBRES NORMÉES
section: 3
section_title: Algèbres de Banach commutatives
lang: fr
source: ts-i-ii-fr
book_pages: A I.29-A I.49, A I.166-A I.172
pdf_pages: 0042-0062, 0179-0185
extraction: native
subsections:
    - "no": 1
      title: Caractères d’une algèbre de Banach commutative
      page: 29
      pdf_page: 42
    - "no": 2
      title: Fonctions continues nulles à l’infini sur un espace locale- ment compact
      page: 31
      pdf_page: 44
    - "no": 3
      title: Applications partielles propres
      page: 33
      pdf_page: 46
    - "no": 4
      title: Transformation de Gelfand
      page: 36
      pdf_page: 49
    - "no": 5
      title: Morphismes d’algèbres de Banach commutatives
      page: 40
      pdf_page: 53
    - "no": 6
      title: Spectre simultané
      page: 41
      pdf_page: 54
    - "no": 7
      title: Ensembles polynomialement convexes
      page: 44
      pdf_page: 57
statements: 48
exercises: 29
content_sha256: f6ce510d33b48cb7d981701098ef96e8029d1308ef57b9c441604229ff35a6a2
---

## § 3. ALGÈBRES DE BANACH COMMUTATIVES

Dans cette section, le corps de base est $\mathbf{C}$.

### 1. Caractères d’une algèbre de Banach commutative

#### Théorème 1 {#ts-i-s3-thm-1 .statement tag=027P}

Soit A une algèbre de Banach et soit $\chi : A\rightarrow \mathbf{C}$ un morphisme d’algèbres (cf. I, p. 9). Alors $\chi$ est continu, de norme au plus 1. Si A est unifère et si $\chi$ est un morphisme unifère, alors $\chi$ est de norme 1.

Démontrons que $|\chi (x)|\leqslant \|x\|$ pour tout $x\in$ A. Quitte à remplacer A par l’algèbre de Banach engendrée par $x$, on peut supposer que A est commutative ; alors, $\chi \in \mathsf{X}'(A)$. Pour tout $x\in A$, on a $\chi (x)\in$ Sp$'_A(x)$ (I, p. 9, n$^o7$), donc $|\chi (x)|\leqslant \varrho (x)\leqslant \|x\|($I, p. 28, cor. 5), d’où la première assertion.

Si, de plus, A est unifère, l’égalité $\chi (1) = 1$ entraîne que $\|\chi \|\geqslant 1$, d’où l’égalité voulue.

#### Remarque {#ts-i-s3-n1-rem-1 .statement tag=027Q}

Soit A une algèbre de Banach commutative. Il découle de ce théorème que la topologie de la convergence simple sur $\mathsf{X}'(A)$ coïncide avec la restriction à $\mathsf{X}'(A)$ de la topologie faible $\sigma (A',A)$ du dual $A'$ de A.

#### Corollaire {#ts-i-s3-n1-cor-1 .statement tag=027R}

Soit A une algèbre de Banach commutative. L’espace $\mathsf{X}'(A)$ est compact. L’espace $\mathsf{X}(A)$ est localement compact, et est compact si A admet un élément unité.

Soit $A'$ le dual de l’espace de Banach A. Sa boule unité $A'_1$ est faiblement compacte (EVT, III, p. 17, cor. 2). D’après le th. 1, on a $\mathsf{X}'(A)\subset A'_1$. De plus, $\mathsf{X}'(A)$ est fermé dans $A'$ pour la topologie faible, car il est l’intersection des ensembles faiblement fermés

$X_{x,y}=\{f\in A'|f(xy)-f(x)f(y) = 0\}$ (pour $x,y\in A)$.

Il en résulte que $\mathsf{X}'(A)$ est compact et que $\mathsf{X}(A) =\mathsf{X}'(A)-\{0\}$ est localement compact.

Si A admet un élément unité 1, alors $\mathsf{X}(A)$ est l’ensemble des $\chi \in$ $\mathsf{X}'(A)$ tels que $\chi (1) = 1$, et est donc une partie fermée, et par suite compacte, de $\mathsf{X}'(A)$.

Tout espace compact est homéomorphe à $\mathsf{X}(A)$ pour une algèbre de Banach unifère commutative A convenable (cf. I, p. 32, cor. 2).

#### Théorème 2 {#ts-i-s3-thm-2 .statement tag=027S}

Soit A une algèbre de Banach commutative. L’application $\chi \mapsto$ Ker($\chi$ ) est une bijection de $\mathsf{X}(A)$ sur l’ensemble J(A) des idéaux maximaux réguliers de A.

Soit I un idéal maximal régulier de A. Il est fermé (I, p. 22, cor. 2), donc $A/I$ est une algèbre de Banach. Comme c’est un corps (A, VIII, p. 426, prop. 2), le théorème de Gelfand–Mazur (I, p. 26, cor. 2), implique que $A/I$ est de dimension 1 sur $\mathbf{C}$. Donc I est de codimension 1 dans A. Le théorème résulte alors du lemme 3 de I, p. 10.

Il peut arriver qu’une algèbre de Banach commutative non nulle A, sans élément unité, n’ait aucun idéal maximal ; alors $\mathsf{X}'(A)$ est réduit à $\{0\}($cf. I, p. 186, exercice 31).

Ce théorème montre que les ensembles J(A) et $\widehat{A}$ de I, p. 11, qui s’identifient puisque A est commutative, peuvent aussi s’identifier à l’ensemble $\mathsf{X}(A)$. Il y a donc lieu de considérer sur $\mathsf{X}(A)$ la topologie faible, et la topologie de Jacobson qui est moins fine (I, p. 15, prop. 5). Les ensembles fermés V(M) de la topologie de Jacobson, pour $M\subset A$, sont les ensembles

$$
\{\chi \in \mathsf{X}(A)|\chi (M) = 0\}
$$

de $\mathsf{X}(A)$, qu’on notera parfois encore V(M). Similairement, pour toute partie M de $\mathsf{X}(A)$, on notera Υ(M) l’idéal intersection des noyaux des $\chi \in M$ ; il est égal à l’ensemble $\Upsilon (M')$ défini dans I, p. 13 pour la partie $M'\subset J(A)$ correspondant à M lorsqu’on identifie J(A) et $\mathsf{X}(A)$.

Quand on utilisera une notion topologique dans $\mathsf{X}(A)$ sans préciser de quelle topologie il s’agit, il s’agira toujours de la topologie faible.

### 2. Fonctions continues nulles à l’infini sur un espace locale- ment compact

Dans ce numéro, X est un espace localement compact. On note $\mathscr{C}_0(X)$ l’algèbre de Banach commutative des fonctions complexes continues tendant vers 0 à l’infini sur X, munie de la norme $\|f\|=$ sup$|f(x)|$

$x\in X$

(exemple 3 de I, p. 17).

#### Proposition 1 {#ts-i-s3-prop-1 .statement tag=027T}

Pour toute partie fermée Φ de X, soit $I_{\Phi}$ l’ensemble des $f\in \mathscr{C}_0(X)$ nulles sur Φ. Alors $\Phi \mapsto I_{\Phi}$ est une bijection de l’ensemble des parties fermées de X sur l’ensemble des idéaux fermés de $\mathscr{C}_0(X)$.

L’ensemble $I_{\Phi}$ est un idéal fermé de $\mathscr{C}_0(X)$.

Soient $\Phi \not= \Phi '$ des parties fermées de X. Quitte à échanger Φ et $\Phi '$, on peut supposer qu’il existe $x\in \Phi '$ tel que $x\notin \Phi$, et il existe alors une fonction $f\in \mathscr{C}_0(X)$ nulle sur Φ et non nulle en $x$ (TG, IX, p. 43, prop. 1). On a $f\in I_{\Phi}$ et $f\notin I_{\Phi'}$, de sorte que l’application $\Phi \mapsto I_{\Phi}$ est injective.

Soit I un idéal fermé de $\mathscr{C}_0(X)$. Soit Φ l’ensemble des $x\in X$ tels que $f(x) = 0$ pour tout $f\in I$ ; c’est une partie fermée de X, et on a $I\subset I_{\Phi}$. Démontrons que $I_{\Phi}\subset I$, ce qui impliquera que $I = I_{\Phi}$ et terminera la preuve de la proposition.

Soit $f\in I_{\Phi}$. Pour tout nombre réel $\varepsilon  >0$, notons $C_{\varepsilon}$ l’ensemble des $x\in X$ tels que $|f(x)|\geqslant \varepsilon$. Puisque $f$ tend vers 0 à l’infini, l’ensemble $C_{\varepsilon}$ est compact. Soit $x\in C_{\varepsilon}$; comme $f(x)\not= 0$ et $f\in I_{\Phi}$, on a $x\notin \Phi$ ; par définition de Φ, il existe alors une fonction $\varphi_x\in I$ telle que $|\varphi_x(x)|>1$, donc telle que $|\varphi_x(y)|>1$ pour tout $y$ appartenant à un voisinage $V_x$ de $x$. Les ouverts $V_x\cap C_{\varepsilon}$ recouvrent $C_{\varepsilon}$. Puisque l’ensemble $C_{\varepsilon}$ est compact, il existe un sous-ensemble fini $T_{\varepsilon}\subset X$ tel que

$$
C_{\varepsilon}\subset \bigcup_{x\in T_{\varepsilon}}V_x
$$

Alors l’élément

1

$$
g_{\varepsilon}=\sum\varphi_x\overline{\varphi_x}\geqslant 0
$$

$$
\varepsilon
$$

$x\in T_{\varepsilon}$

de $\mathscr{C}_0(X)$ appartient à I, et on a $g_{\varepsilon}\geqslant \varepsilon^{-1}$ sur $C_{\varepsilon}$. La fonction

$$
f g_{\varepsilon}
$$

$$
f_{\varepsilon}=
$$

$$
1 +g_{\varepsilon}
$$

appartient à I. Pour $x /\in C_{\varepsilon}$, on a

$$
|f(x)-f_{\varepsilon}(x)|\leqslant 2\varepsilon
$$

et pour $x\in C_{\varepsilon}$, on a

$$
|f(x)|
$$

$$
|f(x)-f_{\varepsilon}(x)|=\leqslant \varepsilon |f(x)|
$$

$$
1 +g_{\varepsilon}(x)
$$

Ainsi $f_{\varepsilon}$ converge uniformément vers $f$ sur X quand $\varepsilon$ tend vers 0. On a donc $f\in I$, d’où $f\in I$ puisque I est fermé.

#### Corollaire 1 {#ts-i-s3-prop-1-cor-1 .statement tag=027U}

Pour tout $x\in X$, soit $I_x$ l’ensemble des $f\in \mathscr{C}_0(X)$ nulles en $x$. Alors $x\mapsto I_x$ est une bijection de X sur l’ensemble des idéaux fermés maximaux de $\mathscr{C}_0(X)$. Ces idéaux sont réguliers.

Ceci résulte aussitôt de la prop. 1.

Notons $X'$ le compactifié d’Alexandroff de X, c’est-à-dire l’espace compact déduit de X par adjonction d’un point à l’infini $\omega_X$ (TG, I, p. 67 et 68). L’algèbre $\mathscr{C}_0(X)$ s’identifie à l’algèbre de Banach des fonctions complexes continues sur $X'$ nulles en $\omega_X$.

Pour tout $x\in X'$, on note ev$_x$ le caractère de $\mathscr{C}_0(X)$ défini par ev$_x(f) =f(x)$ pour tout $f\in \mathscr{C}_0(X)$.

#### Corollaire 2 {#ts-i-s3-prop-1-cor-2 .statement tag=027V}

L’application $x\mapsto$ ev$_x$ est un homéomorphisme de $X'$ sur $\mathsf{X}'(\mathscr{C}_0(X))$, et sa restriction à X est un homémorphisme de X sur $\mathsf{X}(\mathscr{C}_0(X))$. De plus, la topologie faible et la topologie de Jacobson coïncident sur $\mathsf{X}(\mathscr{C}_0(X))$.

L’application ev$:x\mapsto$ ev$_x$ de $X'$ dans $\mathsf{X}'(\mathscr{C}_0(X))$ est injective. Elle est surjective d’après le cor. 1 et le th. 2 de I, p. 30. Elle est continue, car pour toute fonction $f\in \mathscr{C}_0(X)$ et tout ouvert U de $\mathbf{R}$, on a

ev$^{-1}(\{\chi \in \mathsf{X}'(\mathscr{C}_0(X))|\chi (f)\in U\}) =\overset{-1}{f}(U)$

qui est ouvert dans X. L’application ev est donc un homéomorphisme puisque $X'$ est compact. La restriction de ev à X est alors un homéo-morphisme sur $\mathsf{X}(\mathscr{C}_0(X))$.

Si F est une partie faiblement fermée de $\mathsf{X}(\mathscr{C}_0(X))$, elle correspond par l’homéomorphisme ev à une partie fermée Φ de X ; précisément, d’après la prop. 1, on a $F =\{\chi \in \mathsf{X}(\mathscr{C}_0(X))|I_{\Phi}\subset$ Ker $\chi \}$ qui est fermé pour la topologie de Jacobson.

#### Corollaire 3 {#ts-i-s3-prop-1-cor-3 .statement tag=027W}

Supposons X compact. Alors l’application $x\mapsto$ ev$_x$ est un homéomorphisme de X sur $\mathsf{X}(\mathscr{C}(X))$. La topologie faible et la topologie de Jacobson coïncident sur $\mathsf{X}(\mathscr{C}(X))$.

### 3. Applications partielles propres

Dans ce numéro, X et Y sont des espaces topologiques localement compacts. On note $X'$ (resp. $Y')$ l’espace compact obtenu à partir de X (resp. Y) par adjonction d’un point à l’infini $\omega_X$ (resp. $\omega_Y)$ (TG, I, p. 67–68). On identifie $X'$ et $Y'$ à $\mathsf{X}'(\mathscr{C}_0(X))$ et $\mathsf{X}'(\mathscr{C}_0(Y))$, respectivement (corollaire 2 de I, p. 32).

#### Définition 1 {#ts-i-s3-def-1 .statement tag=027X}

Une application partielle propre de X dans Y est une correspondance $f= (\Gamma ,X,Y)$ (E, II, p. 10, déf. 2) entre X et Y telle que

(i) Le graphe Γ est fonctionnel;

(ii) Le domaine de définition de $f$ est un ouvert U de X ;

(iii) L’application $x\mapsto f(x)$ de U dans Y est propre.

L’application identique de X est une application partielle propre de X dans X. Soient Z un espace topologique localement compact et $f$ (resp. $g)$ une application partielle propre de X dans Y (resp. de Y dans Z). Alors la correspondance composée $g\circ f$ (E, II, p. 11, déf. 6) est une application partielle propre de X dans Z (TG, I, p. 72, prop. 3, et p. 73, prop. 5).

#### Lemme 1 {#ts-i-s3-lem-1 .statement tag=027Y}

Pour toute application partielle propre $f$ de X dans Y, de domaine de définition U, notons $\widetilde{f}$ l’application de $X'$ dans $Y'$ définie par $\widetilde{f}(x) =f(x)$ si $x\in U$ et $\widetilde{f}(x) =\omega_Y$ si $x /\in U$ ; elle est continue.

L’application $f\mapsto \widetilde{f}$ est une bijection entre l’ensemble des applications partielles propres $f$ de X dans Y et l’ensemble des applications continues $g$ de $X'$ dans $Y'$ telles que $g(\omega_X) =\omega_Y$.

Soit $f$ une application partielle propre de X dans Y et soit U son domaine. Démontrons que l’application $\widetilde{f}$ est continue. Elle est continue en tout point de U, car U est ouvert dans $X'$. Démontrons qu’elle est également continue en tout point $x$ de $X'-$ U ; on a alors $\widetilde{f}(x) =\omega_Y$. Soit V un voisinage ouvert de $\omega_Y$ dans $Y'$; démontrons que $\widetilde{f}^{-1}(V)$ est un voisinage de $x$. Par définition de l’espace topologique $Y'$, on peut supposer que V est de la forme $Y'-$ K, où K est une partie compacte de Y. Puisque $f$ définit une application propre de U dans Y, l’ensemble $f^{-1}(K)$ est compact dans U (TG, I, p. 77, prop. 6), donc dans $X'$. C’est en particulier une partie fermée de $X'$ et $\widetilde{f}^{-1}(V) =$ $X'-f^{-1}(K)$ est une partie ouverte de $X'$, et est donc un voisinage de $x$.

Inversement, soient $g: X'\rightarrow Y'$ une application continue telle que $g(\omega_X) =\omega_Y$ et $\Gamma_g\subset X'\times Y'$ son graphe. L’ensemble U = X $-\overset{-1}{g}(\omega_Y)$ est ouvert dans X. La correspondance $f= (\Gamma_g\cap (U\times Y),X,Y)$ est une application partielle propre de X dans Y (TG, I, p. 77, prop. 7) telle que $\widetilde{f}=g$, et c’est la seule.

Nous identifierons les applications partielles propres de X dans Y aux applications continues de $X'$ dans $Y'$ qui appliquent $\omega_X$ sur $\omega_Y$. En particulier, les applications propres de X dans Y sont les applications partielles propres de domaine X ; elles s’identifient aux applica-

$-1$

tions continues $f$ de $X'$ dans $Y'$ telles que que $f(\omega_Y) =\{\omega_X\}$. Si X est compact, ce sont tout simplement les applications continues de X dans Y.

Soit A une algèbre de Banach complexe commutative. Rappelons que $\mathsf{X}'(A)$ s’identifie à l’espace compact obtenu à partir de $\mathsf{X}(A)$ par adjonction d’un point à l’infini (I, p. 29, corollaire).

#### Proposition 2 {#ts-i-s3-prop-2 .statement tag=027Z}

Soient A et B des algèbres de Banach complexes commutatives. Pour tout morphisme d’algèbres $\pi : A\rightarrow B$, l’application $\mathsf{X}'(\pi )$ est une application partielle propre de $\mathsf{X}(B)$ dans $\mathsf{X}(A)$.

En effet, $\mathsf{X}'(\pi )$ est une application continue de $\mathsf{X}'(B)$ dans $\mathsf{X}'(A)$ (I, p. 10). Le point à l’infini de $\mathsf{X}'(B)$ (resp. de $\mathsf{X}'(A)$) est le caractère nul, et on a $\mathsf{X}'(\pi )(0) = 0$.

#### Proposition 3 {#ts-i-s3-prop-3 .statement tag=0280}

a) Pour toute application partielle propre $\varphi$ de X dans Y, l’application $f\mapsto f\circ \varphi$ de $\mathscr{C}(Y')$ dans $\mathscr{C}(X')$ induit un morphisme d’algèbres $\varphi^*$ de $\mathscr{C}_0(Y)$ dans $\mathscr{C}_0(X)$ ;

b) L’application $\varphi \mapsto \varphi^*$ est une bijection de l’ensemble des applications partielles propres de X dans Y sur l’ensemble des morphismes d’algèbres de $\mathscr{C}_0(Y)$ dans $\mathscr{C}_0(X)$. Sa bijection réciproque est l’application $\pi \mapsto \mathsf{X}'(\pi )$.

Démontrons a). Soit $\varphi$ une application partielle propre de X dans Y, identifiée à une application continue de $X'$ dans $Y'$ telle que $\varphi (\omega_X) =\omega_Y$. Pour $f\in \mathscr{C}_0(Y)$, on a $(f\circ \varphi )(\omega_X) =f(\omega_Y) = 0$, donc l’application $\varphi^*$ est bien définie. C’est un morphisme d’algèbres.

Démontrons que $\mathsf{X}'(\varphi^*)$ s’identifie à $\varphi$. Soit $x\in X$. Pour toute fonction $f\in \mathscr{C}_0(Y)$, le caractère $\mathsf{X}'(\varphi^*$)(ev$_x)$ associe à $f$ le nombre complexe

(ev$_x\circ \varphi^*)(f) =$ ev$_x(f\circ \varphi ) =f(\varphi (x))$,

donc $\mathsf{X}'(\varphi^*$)(ev$_x) =$ ev$_{\varphi(x)}$. Cela démontre l’assertion.

Inversement, soit $\pi :\mathscr{C}_0(Y)\rightarrow \mathscr{C}_0(X)$ un morphisme d’algèbres. Démontrons que $\mathsf{X}'(\pi )^*=\pi$. Soit $f\in \mathscr{C}_0(Y)$, et notons $g=\mathsf{X}'(\pi )^*(f)\in$ $\mathscr{C}_0(X)$. Pour tout $x\in X$, on a

$g(x) = (f\circ \mathsf{X}'(\pi ))(x) =$ ev$_{\mathsf{X}'(\pi)(x)}(f) =$ (ev$_x\circ \pi )(f) =\pi (f)(x)$,

puisque $\mathsf{X}'(\pi )$ vérifie ev$_{\mathsf{X}'(\pi)(x)}=$ ev$_x\circ \pi$. On a donc $g=\pi (f)$, ce qui permet de conclure que $\mathsf{X}'(\pi )^*=\pi$.

De manière tout à fait similaire, on a :

#### Proposition 4 {#ts-i-s3-prop-4 .statement tag=0281}

Supposons que X et Y sont compacts. Identifions l’espace X (resp. l’espace Y) à $\mathsf{X}(\mathscr{C}(X))$ (resp. $\mathsf{X}(\mathscr{C}(Y))$) (corollaire 3 de I, p. 33).

a) Pour toute application continue $\varphi : X\rightarrow$ Y, l’application $\varphi^*:f\mapsto f\circ \varphi$ est un morphisme d’algèbres de $\mathscr{C}(Y)$ dans $\mathscr{C}(X)$;

b) Les applications $\varphi \mapsto \varphi^*$ et $\pi \mapsto \mathsf{X}(\pi )$ sont des bijections réciproques entre l’ensemble des applications continues de X dans Y et l’ensemble des morphismes d’algèbres de $\mathscr{C}(Y)$ dans $\mathscr{C}(X)$.

#### Remarque {#ts-i-s3-n3-rem-1 .statement tag=0282}

*Dans le langage de la théorie des catégories, les résultats qui précèdent s’interprètent de la manière suivante. Soit $\mathbf{G}$ la catégorie dont les objets sont les espaces topologiques localement compacts et les morphismes les applications partielles propres. Le foncteur X $\mapsto \mathscr{C}_0(X)$ est un foncteur contravariant, pleinement fidèle, de la catégorie $\mathbf{G}$ dans la catégorie des algèbres de Banach commutatives complexes. De plus, $A\mapsto \mathsf{X}(A)$ est un foncteur contravariant de la catégorie des algèbres de Banach commutatives complexes dans la catégorie $\mathbf{G}$. Si l’on associe à un espace topologique localement compact X l’homéomorphisme

ev$: X\rightarrow \mathsf{X}(\mathscr{C}_0(X))$,

on obtient un isomorphisme du foncteur identique de la catégorie $\mathbf{G}$ vers le foncteur composé $X\mapsto \mathsf{X}(\mathscr{C}_0(X))$.

Il n’est pas vrai que le foncteur composé $A\mapsto \mathscr{C}_0(\mathsf{X}(A))$ soit isomorphe au foncteur identique de la catégorie des algèbres de Banach commutatives complexes (cf. exemple 2 de I, p. 36 et exercice 2 de I, p. 155). On verra cependant un énoncé de ce type pour les algèbres stellaires commutatives (numéro 5 de I, p. 107).*

### 4. Transformation de Gelfand

Soit A une algèbre de Banach commutative. Rappelons que, pour tout $x\in A$, on note $\mathscr{G}_A(x)$, ou $\mathscr{G}(x)$, la fonction $\chi \mapsto \chi (x)$ sur $\mathsf{X}(A)$, que $\mathscr{G}(x)$ s’appelle la transformée de Gelfand de $x$, et que l’application $x\mapsto \mathscr{G}(x)$ s’appelle transformation de Gelfand (cf. déf. 5 de I, p. 7). On a donc par définition :

$$
\mathscr{G}(x)(\chi ) =\chi (x)
$$

#### Exemple 1 {#ts-i-s3-n4-exa-1 .statement tag=0283}

Soit X un espace topologique localement compact et considérons l’algèbre de Banach commutative $\mathscr{C}_0(X)$ (exemple 3 de I, p. 17 et numéro 2 de I, p. 31). D’après le cor. 1 de I, p. 32, l’espace des caractères $\mathsf{X}(\mathscr{C}_0(X))$ s’identifie à X par le biais de l’application associant à un élément $x\in X$ le caractère $f\mapsto f(x)$ de $\mathscr{C}_0(X)$, et la transformation de Gelfand de $\mathscr{C}_0(X)$ s’identifie alors à l’application identique.

#### Exemple 2 {#ts-i-s3-n4-exa-2 .statement tag=0284}

Soit $n\geqslant 0$ un entier. Soit $A_n$ l’algèbre des fonctions $f: [0,1]\rightarrow K$ admettant des dérivées continues dans $[0,1]$ jusqu’à l’ordre $n$. Munie de la norme

$^n$ 1 $(_{k)}$

$\|f\|=\sum$ sup $|f(t)|$,

$k$! $_{0\leqslant t\leqslant 1}$

$k=0$

c’est une algèbre de Banach (exemple 4 de I, p. 18). Pour tout $n$, l’espace des caractères $\mathsf{X}(A_n)$ s’identifie à $[0,1]$ et $\mathscr{G}$ à l’inclusion de $A_n$ dans $\mathscr{C}([0,1])$ (cf. exemple 1 de I, p. 144).

#### Exemple 3 {#ts-i-s3-n4-exa-3 .statement tag=0285}

Soit Δ le disque des nombres complexes $z$ vérifiant $|z|\leqslant 1$ et soit A l’algèbre de Banach complexe des fonctions continues sur Δ analytiques dans l’intérieur de Δ, munie de la norme $\|f\|=$ sup$_{z\in\Delta}|f(z)|$ (exemple 9 de I, p. 20). Alors $\mathsf{X}(A)$ s’identifie à Δ et $\mathscr{G}$ à l’inclusion de A dans $\mathscr{C}(\Delta )$ (cf. exerc. 6 de I, p. 193).

#### Exemple 4 {#ts-i-s3-n4-exa-4 .statement tag=0286}

Considérons l’algèbre de Banach complexe A des séries de Fourier absolument convergentes (exemple 8 de I, p. 19). Pour tout élément $u$ du cercle unité $\mathbf{U}$, l’application $f\mapsto f(u)$ est un caractère ev$_u$ de A. Si $f_0\in A$ est l’application identique de $\mathbf{U}$, on a ev$_u(f_0) =u$, donc l’application ev$:u\mapsto$ ev$_u$ de $\mathbf{U}$ dans $\mathsf{X}(A)$ est injective ; elle est continue.

Soit $\chi \in \mathsf{X}(A)$. On a $\|f_0\|$ = $\|f_0^{-1}\|$ = 1, donc $|\chi (f_0)|\leqslant$ 1 et $|\chi (f_0)^{-1}|\leqslant 1$. Cela montre que $\chi (f_0)\in \mathbf{U}$ et il existe $u\in \mathbf{U}$ tel que $\chi (f_0) =$ ev$_u(f_0)$. Comme $\{f_0, f_0^{-1}\}$ engendre topologiquement l’algèbre unifère A, on a $\chi =$ ev$_u$. Ainsi, l’application ev est un homéomorphisme de $\mathbf{U}$ sur $\mathsf{X}(A)$, par lequel on identifie ces espaces. La transformation de Gelfand de A s’identifie alors à l’inclusion de A dans $\mathscr{C}(\mathbf{U})$.

Puisque A est isomorphe à l’algèbre de Banach $L^1(\mathbf{Z})$ (exemple 8 de I, p. 19), l’espace $\mathsf{X}(L^1(\mathbf{Z}))$ s’identifie à $\mathbf{U}$ et, pour tout élément $(c_n)\in L^1(\mathbf{Z})$, la transformée de Gelfand $\mathscr{G}_{L^1(\mathbf{Z})}((c_n))$ s’identifie à la fonction $u\mapsto \sum_{n\in\mathbf{Z}}c_nu^n$ sur $\mathbf{U}$.

#### Exemple 5 {#ts-i-s3-n4-exa-5 .statement tag=0287}

Soit Δ le disque unité des nombres complexes $z$ tels que $|z|\leqslant 1$. Sa frontière dans $\mathbf{C}$ est $\mathbf{U}$. Soit A l’algèbre de Banach des fonctions complexes $f$ sur $\mathbf{U}$ telles qu’il existe une fonction continue $\widetilde{f}\in \mathscr{C}(\Delta )$ prolongeant $f$ qui est analytique dans $\mathring{\Delta}$, munie de la norme $\|f\|=$ sup$_{z\in\mathbf{U}}|f(z)|$. En vertu du principe du maximum (VAR, R1, p. 30, 3.3.7), on a alors $\|f\|=$ sup$_{z\in\Delta}|\widetilde{f}(z)|$, et donc A coïncide avec l’algèbre de l’exemple 9 de I, p. 20. L’ensemble $\mathsf{X}(A)$ s’identifie à Δ et, si $f\in A$, l’application $\mathscr{G}(f)$ s’identifie avec le prolongement continu de $f$ dans Δ qui est analytique dans $\mathring{\Delta}($cf. exerc. 6 de I, p. 193).

#### Proposition 5 {#ts-i-s3-prop-5 .statement tag=0288}

Soit A une algèbre de Banach commutative. Pour tout $x\in A$, la fonction $\mathscr{G}(x)$ appartient à l’algèbre de Banach commutative $\mathscr{C}_0(\mathsf{X}(A))$ des fonctions continues sur $\mathsf{X}(A)$ tendant vers 0 à l’infini.

Par définition (cf. n$^o7$ de I, p. 9), la fonction $\mathscr{G}_A'(x) :\chi \mapsto \chi (x)$ est continue sur $\mathsf{X}'(A)$ et nulle en 0. Comme $\mathsf{X}'(A)$ s’identifie au compactifié d’Alexandroff de $\mathsf{X}(A)$ d’après le cor. 1 de I, p. 29, la proposition en résulte.

#### Proposition 6 {#ts-i-s3-prop-6 .statement tag=0289}

Soit A une algèbre de Banach commutative et soit $x\in A$.

a) La réunion de l’ensemble des valeurs de $\mathscr{G}(x)$ et de $\{0\}$ est égale à Sp$'_A(x)$ ;

b) Si A admet un élément unité, l’ensemble des valeurs de $\mathscr{G}(x)$ est Sp$_A(x)$. En particulier, pour que $x$ soit inversible, il faut et il suffit que $\mathscr{G}(x)$ ne s’annule pas.

Supposons que A admette un élément unité. On sait que, pour tout $\chi \in \mathsf{X}(A)$, on a $\chi (x)\in$ Sp$_A(x)$. Réciproquement, soit $\lambda \in$ Sp$_A(x)$. Alors $x-\lambda$ n’est pas inversible, donc appartient à un idéal maximal de A. Il existe alors $\chi \in \mathsf{X}(A)$ tel que $\chi (x-\lambda ) = 0$ (th. 2 de I, p. 30), d’où b).

Passons au cas général. Soit $\widetilde{A}$ l’algèbre de Banach obtenue à partir de A par adjonction d’un élément unité ; elle est commutative. L’ensemble Sp$'_A(x)$ est égal à Sp$_{\widetilde{A}}(x)$, c’est-à-dire à l’ensemble des valeurs de $\mathscr{G}_{\widetilde{A}}(x)$ sur $\mathsf{X}(\widetilde{A}) =\mathsf{X}'(A)$. D’où a).

#### Exemple {#ts-i-s3-n4-exa-6 .statement tag=028A}

Considérons l’algèbre de Banach A des séries de Fourier absolument convergentes (exemple 4). La prop. 6, b) implique que si $\varphi$ est une fonction sur le cercle unité $\mathbf{U}$ admettant une série de Fourier absolument convergente, et si $\varphi$ ne s’annule pas, la fonction $1/\varphi$ admet également une série de Fourier absolument convergente (« théorème de Wiener »).

#### Proposition 7 {#ts-i-s3-prop-7 .statement tag=028B}

Soit A une algèbre de Banach commutative.

a) La transformation de Gelfand $\mathscr{G}$ définit un morphisme de A dans $\mathscr{C}_0(\mathsf{X}(A))$ tel que $\|\mathscr{G}(x)\|=\varrho (x)\leqslant \|x\|$ pour tout $x\in A$ ;

b) Pour que la transformation de Gelfand $\mathscr{G}$ soit isométrique, il faut et il suffit que $\|x^2\|=\|x\|^2$ pour tout $x\in A$.

L’application $\mathscr{G}$ est un morphisme de A dans $\mathscr{C}_0(\mathsf{X}(A))$ d’après le n$^o7$ de I, p. 9 et la prop. 5 de I, p. 37, et vérifie $\|\mathscr{G}(x)\|=\varrho (x)$ d’après la prop. 6 et le cor. 5 de I, p. 28. L’assertion b) résulte de a) et de la remarque 1 de I, p. 21.

#### Corollaire {#ts-i-s3-n4-cor-1 .statement tag=028C}

Soient A une algèbre de Banach, $x$ et $y$ des éléments permutables de A.

a) On a $\varrho (xy)\leqslant \varrho (x)\varrho (y)$ et $\varrho (x+y)\leqslant \varrho (x) +\varrho (y)$ ;

b) Si $y$ est quasi-nilpotent, alors Sp$'_A(x) =$ Sp$'_A(x+y)$ ; si de plus A est unifère, alors Sp$_A(x) =$ Sp$_A(x+y)$.

En considérant l’algèbre de Banach déduite de A par adjonction d’un élément unité, on se ramène d’abord au cas où l’algèbre A est unifère. Puis en considérant la sous-algèbre pleine fermée de A engendrée par $x$ et $y$, on se ramène au cas où A est commutative et unifère. L’assertion a) est alors une conséquence de la prop. 7, a), et l’assertion b) découle de la prop. 6 de I, p. 37 et du cor. 5 de I, p. 28.

#### Proposition 8 {#ts-i-s3-prop-8 .statement tag=028D}

Soit A une algèbre de Banach commutative. Les quatre ensembles suivants sont égaux:

(i) Le noyau de la transformation de Gelfand ;

(ii) L’ensemble des éléments $x$ de A tels que Sp$'_A(x) =\{0\}$;

(iii) L’ensemble des éléments quasi-nilpotents de A ;

(iv) Le radical de A.

Notons $N_1,N_2,N_3,N_4$, respectivement, ces ensembles. On a $N_1=$ $N_2$ (prop. 6, a)), et $N_2= N_3($I, p. 28, cor. 5). Par définition, l’ensemble $N_4$ est l’intersection des idéaux maximaux réguliers de A ; c’est donc l’intersection des noyaux des caractères de A (th. 2 de I, p. 30), qui est égal à $N_1$.

#### Remarque 1 {#ts-i-s3-n4-rem-1 .statement tag=028E}

En général, l’image de la transformation de Gelfand n’est ni fermée dans $\mathscr{C}_0(\mathsf{X}(A))$, ni dense dans $\mathscr{C}_0(\mathsf{X}(A))$ (exerc. 7 de I, p. 193).

#### Remarque 2 {#ts-i-s3-n4-rem-2 .statement tag=028F}

L’image de la transformation de Gelfand sépare les points de $\mathsf{X}(A)$, puisque si $\chi_1\not=\chi_2$ sont des éléments de $\mathsf{X}(A)$, il existe $x\in A$ tel que $\chi_1(x)\not=\chi_2(x)$.

#### Remarque 3 {#ts-i-s3-n4-rem-3 .statement tag=028G}

Si $\chi \in \mathsf{X}(A)$, il existe un élément de l’image de la transformation de Gelfand qui ne s’annule pas en $\chi$.

#### Remarque 4 {#ts-i-s3-n4-rem-4 .statement tag=028H}

Si A possède un élément unité, l’image de la transformation de Gelfand est une sous-algèbre pleine de l’algèbre des fonctions continues sur $\mathsf{X}(A)$ (prop. 6, b)).

#### Lemme 2 {#ts-i-s3-lem-2 .statement tag=028I}

Soit A une algèbre de Banach commutative. Soit M une partie de $\mathsf{X}(A)$. Alors M est fermée pour la topologie de Jacobson si et seulement si, pour tout caractère $\chi \in \mathsf{X}(A)$ - M, il existe un élément $x$ de A tel que $\mathscr{G}(x)$ soit nul sur M et non nul en $\chi$.

Soit Υ(M) l’intersection des noyaux des éléments de M. L’ensemble M est fermé pour la topologie de Jacobson si et seulement si M = V(Υ(M)) (cf. I, p. 13 et I, p. 30). Cette condition équivaut à dire que les éléments $\chi$ de M sont précisément les caractères qui s’annulent sur Υ(M). Par conséquent M est fermé si et seulement si pour tout caractère $\chi  /\in M$, il existe $x\in \Upsilon (M)$ tel que $\chi (x)\not= 0$. Cela se traduit en $\mathscr{G}(x)(\chi )\not= 0$ et $\mathscr{G}(x)|M = 0$.

### 5. Morphismes d’algèbres de Banach commutatives

#### Proposition 9 {#ts-i-s3-prop-9 .statement tag=028J}

Soit A une algèbre de Banach, soit B une algèbre de Banach commutative et sans radical, Tout morphisme de l’algèbre sous-jacente à A dans l’algèbre sous-jacente à B est continu.

Soit $h: A\rightarrow B$ un morphisme d’algèbres et soit $(a, b)\in A\times B$ un point adhérent au graphe Γ de $h$. Soit $\chi \in \mathsf{X}'(B)$. La fonction $x\mapsto \chi (h(x))$ de A dans $\mathbf{C}$ est un homomorphisme d’algèbres, donc est continu (I, p. 29, th. 1). L’application de $A\times B$ dans $\mathbf{C}$ donnée par $(x, y)\mapsto \chi (h(x))-\chi (y)$ est alors continue, elle est nulle sur Γ, donc nulle en $(a, b)$. On a ainsi $\chi (h(a)) =\chi (b)$ pour tout $\chi \in \mathsf{X}'(B)$. Comme B est sans radical, on a $h(a) =b$. Ainsi le graphe de $h$ est fermé et donc $h$ est continu (EVT, I, p. 19, cor. 5).

#### Corollaire {#ts-i-s3-n5-cor-1 .statement tag=028K}

Sur une algèbre complexe commutative sans radical, deux normes définissant des structures d’algèbre de Banach sont équivalentes.

Il suffit d’appliquer la prop. 9 à l’application identique de l’algèbre.

Soient A et B des algèbres de Banach commutatives. D’après le n$^o7$ de I, p. 9, si $h: A\rightarrow B$ est un morphisme surjectif, $\mathsf{X}'(h)$ est un homéo-morphisme de $\mathsf{X}'(B)$ sur un sous-espace fermé de $\mathsf{X}'(A)$ qui transforme 0 en 0. (Dans le cas où $h$ est l’injection d’une sous-algèbre dans $\mathscr{C}(X)$, l’application $\mathsf{X}'(h)$ est injective sous des hypothèses beaucoup plus faibles, cf. I, p. 142, prop. 1, d).)

Soit maintenant $h: A\rightarrow B$ un morphisme injectif. En général, $\mathsf{X}'(h)$ n’est pas surjectif, mais la proposition suivante fournit une condition nécessaire pour que ce soit le cas.

#### Proposition 10 {#ts-i-s3-prop-10 .statement tag=028L}

Soient A et B des algèbres de Banach unifères commutatives, $h: A\rightarrow B$ un morphisme d’algèbres unifère, non nécessairement continu. Si $\mathsf{X}(h)$ est surjectif, alors $h(A)$ est une sous-algèbre pleine de B.

Soit $x\in A$ tel que $h(x)$ soit inversible dans B. Pour tout $\chi \in \mathsf{X}(A)$, il existe $\xi \in \mathsf{X}(B)$ tel que $\chi =\mathsf{X}(h)(\xi )$, donc $\chi (x) =\xi (h(x))\not= 0$. La prop. 6 de I, p. 37 montre alors que $x$ est inversible dans A, et donc que $h(x)$ est inversible dans $h(A)$.

La condition nécessaire de la proposition n’est pas suffisante, même si $h$ est isométrique (I, p. 168, exerc. 14). On a toutefois le résultat suivant :

#### Proposition 11 {#ts-i-s3-prop-11 .statement tag=028M}

Soient A et B des algèbres de Banach unifères commutatives, soit $a$ un élément de A et soit $h: A\rightarrow B$ un morphisme injectif unifère (non nécessairement continu). On suppose que la sous-algèbre fermée pleine de A engendrée par $a$ est égale à A. Les conditions suivantes sont équivalentes :

(i) $\mathsf{X}(h)$ est surjectif;

(ii) $h(A)$ est une sous-algèbre pleine de B;

(iii) Sp$_A(a) =$ Sp$_B(h(a))$.

(i) $=\Rightarrow$ (ii) résulte de la prop. 10.

(ii) $=\Rightarrow$ (iii) résulte de la formule Sp$_A(a) =$ Sp$_{h(A)}(h(a)) =$ Sp$_B(h(a))$, valide puisque $h(A)$ est une sous-algèbre pleine de B.

(iii) $=\Rightarrow$ (i) d’après la formule (4) du n$^o6$ de I, p. 6, on a le diagramme commutatif

$$
\leftarrow^{\mathsf{X}(h)}
$$

$$
\mathsf{X}(B)\rightarrow \mathsf{X}(A)
$$

$$
\rightarrow \leftarrow_{\mathscr{G}_B(h(a))}\rightarrow \leftarrow_{\mathscr{G}_A(a)}
$$

$$
\leftarrow_i
$$

Sp$_B(h(a))\rightarrow$ Sp$_A(a)$

où les flèches verticales désignent des applications surjectives (I, p. 37, prop. 6) et $i$ est l’inclusion canonique. L’hypothèse (iii) signifie que $i$ est bijective. De plus l’application surjective $\mathscr{G}_A(a) :\mathsf{X}(A)\rightarrow$ Sp$_A(a)$ est bijective : en effet, pour tout caractères $\chi_1$ et $\chi_2$ de A, l’ensemble $A_{\chi_1,\chi_2}=\{x\in A|\chi_1(x) =\chi_2(x)\}$ est une sous-algèbre fermée pleine de A. Par hypothèse, on a donc $A_{\chi_1,\chi_2}$ = A si $a\in A_{\chi_1,\chi_2}$, c’est-àdire $\chi_1=\chi_2$ si $\mathscr{G}_A(a)\chi_1=\mathscr{G}_A(a)\chi_2$. Le diagramme implique alors que l’application $\mathsf{X}(h)$ est surjective.

### 6. Spectre simultané

Soit Λ un ensemble. Soit $C_{\Lambda}=\mathbf{C}[(X_{\lambda})_{\lambda\in\Lambda}]$ l’algèbre unifère des polynômes complexes par rapport à une famille d’indéterminées $(X_{\lambda})_{\lambda\in\Lambda}$. Pour tout $\chi \in \mathsf{X}(C_{\Lambda})$, on a $(\chi (X_{\lambda}))_{\lambda\in\Lambda}\in \mathbf{C}^{\Lambda}$; l’application $\chi \mapsto$ $(\chi (X_{\lambda}))_{\lambda\in\Lambda}$ est un homéomorphisme de $\mathsf{X}(C_{\Lambda})$ sur l’espace produit $\mathbf{C}^{\Lambda}$, par lequel on identifie ces espaces.

Soient d’autre part A une algèbre de Banach commutative unifère et $x= (x_{\lambda})_{\lambda\in\Lambda}$ une famille d’éléments de A. Il existe un morphisme unifère $h$ et un seul de $C_{\Lambda}$ dans A tel que $h(X_{\lambda}) =x_{\lambda}$ pour tout $\lambda$. L’application continue $\mathsf{X}(h)$ de $\mathsf{X}(A)$ dans $\mathbf{C}^{\Lambda}$ est l’application qui à $\chi$ associe la famille $(\chi (x_{\lambda}))_{\lambda\in\Lambda}$. On l’appelle l’application de $\mathsf{X}(A)$ dans $\mathbf{C}^{\Lambda}$ définie par $x$.

#### Définition 2 {#ts-i-s3-def-2 .statement tag=028N}

L’image de l’application $\mathsf{X}(h)$ est appelée le spectre simultané de $x$, et notée Sp$^{\Lambda}_A(x)$ ou Sp$^{\Lambda}(x)$.

Le spectre simultané de $x$ est une partie compacte de $\mathbf{C}^{\Lambda}$. Un élément $c= (c_{\lambda})\in \mathbf{C}^{\Lambda}$ appartient à Sp$^{\Lambda}_A(x)$ si et seulement si les éléments $x_{\lambda}-c_{\lambda}$ appartiennent à un même idéal maximal de A, autrement dit si la famille $(x_{\lambda}-c_{\lambda})_{\lambda\in\Lambda}$ n’engendre pas l’algèbre A.

Si Λ contient un seul élément, de sorte que la famille $x$ se réduit à un seul élément $x\in A$, on a Sp$^{\Lambda}_A(x) =$ Sp$_A(x)$ (I, p. 37, prop. 6, b)). Si $\Lambda '\subset \Lambda$, alors Sp$^{\Lambda}_{A'}((x_{\lambda})_{\lambda\in\Lambda'})$ est l’image de Sp$^{\Lambda}_A((x_{\lambda})_{\lambda\in\Lambda})$ par l’application canonique de projection de $\mathbf{C}^{\Lambda}$ sur $\mathbf{C}^{\Lambda'}$. En particulier, on a

Sp$^{\Lambda}_A(x)\subset \prod_{\lambda\in\Lambda}$ Sp$_A(x_{\lambda})$.

Notons $z_{\lambda}$, pour $\lambda \in \Lambda$, les fonctions coordonnées sur $\mathbf{C}^{\Lambda}$. Si $\chi \in$ $\mathsf{X}(A)$, la valeur en $\chi$ de $z_{\lambda}\circ \mathsf{X}(h)$ est $\chi (x_{\lambda})$, donc $z_{\lambda}\circ \mathsf{X}(h) =\mathscr{G}(x_{\lambda})$.

Soient A et B des algèbres de Banach commutatives unifères, $\varphi$ un morphisme unifère de A dans B, et $x= (x_{\lambda})_{\lambda\in\Lambda}$ une famille d’éléments de A. Notons $\varphi (x)$ la famille $(\varphi (x_{\lambda}))_{\lambda\in\Lambda}$ d’éléments de B. On a, pour tout $\chi \in \mathsf{X}(B)$, et tout $\lambda \in \Lambda$

$$
\chi (\varphi (x_{\lambda})) = (\mathsf{X}(\varphi )(\chi ))(x_{\lambda})
$$

donc Sp$^{\Lambda}_B(\varphi (x))\subset$ Sp$^{\Lambda}_A(x)$. Le diagramme

$$
\leftarrow^{\mathsf{X}(\varphi)}
$$

$$
\mathsf{X}(B)\rightarrow \mathsf{X}(A)
$$

$$
\rightarrow \leftarrow \rightarrow \leftarrow \tag{1}
$$

$$
_{\Lambda}\leftarrow_{i\Lambda}
$$

Sp$_B(\varphi (x))\rightarrow$ Sp$_A(x)$

où $i$ désigne l’inclusion, et où les flèches verticales désignent les applications définies par les familles $\varphi (x)$ et $x$, est donc commutatif.

#### Exemple {#ts-i-s3-n6-exa-1 .statement tag=028O}

Soit K $\subset \mathbf{C}^{\Lambda}$ une partie compacte. Soit $z= (z_{\lambda})_{\lambda\in\Lambda}$ la famille dans $\mathscr{C}(K)$ des restrictions à K des fonctions coordonnées de $\mathbf{C}^{\Lambda}$. Alors le spectre simultané Sp$^{\Lambda}_{\mathscr{C}(K)}(z)$ est égal à K. En effet, d’après le cor. 2 de I, p. 32, tout caractère $\chi$ de $\mathscr{C}(K)$ est de la forme $f\mapsto f(x)$ pour un élément $x\in K$, et on a alors $(\chi (z_{\lambda}))_{\lambda\in\Lambda}=x$.

#### Proposition 12 {#ts-i-s3-prop-12 .statement tag=028P}

Soient Λ un ensemble et A une algèbre de Banach unifère commutative. Soit $x= (x_{\lambda})_{\lambda\in\Lambda}$ une famille d’éléments de A.

a) On suppose que la sous-algèbre pleine de A engendrée par la famille $x$ est dense dans A. L’application de $\mathsf{X}(A)$ dans $\mathbf{C}^{\Lambda}$ définie par $x$ est un homéomorphisme de $\mathsf{X}(A)$ sur le spectre simultané Sp$^{\Lambda}_A(x)$ ;

b) On suppose que la sous-algèbre unifère de A engendrée par la famille $x$ est dense dans A. Pour tout $c\in \mathbf{C}^{\Lambda}$, les conditions suivantes sont équivalentes :

(i) $c\in$ Sp$^{\Lambda}_A(x)$ ;

(ii) $|P(c)|\leqslant \varrho (P(x))$ pour tout polynôme $P\in \mathbf{C}[(X_{\lambda})_{\lambda\in\Lambda}]$;

(iii) $|P(c)|\leqslant \|P(x)\|$ pour tout polynôme $P\in \mathbf{C}[(X_{\lambda})_{\lambda\in\Lambda}]$.

a) L’application de $\mathsf{X}(A)$ dans Sp$^{\Lambda}_A(x)$ définie par la famille $x$ est continue et surjective. Soient $\chi ,\chi '\in \mathsf{X}(A)$ des caractères ayant la même image, c’est-à-dire tels que $\chi (x_{\lambda}) =\chi '(x_{\lambda})$ pour tout $\lambda \in \Lambda$. Les caractères $\chi$ et $\chi '$ coïncident sur les éléments de la forme $P(x)Q(x)^{-1}$, où $P\in \mathbf{C}[(X_{\lambda})]$, $Q\in \mathbf{C}[(X_{\lambda})]$ et $Q(x)$ est inversible dans A, c’est-à-dire sur la sous-algèbre pleine de A engendrée par les éléments $x_{\lambda}$ (lemme 2 de I, p. 6). Puisque $\chi$ et $\chi '$ sont continus (th. 1 de I, p. 29), ils sont donc égaux sur A. Cela démontre que $\mathsf{X}(h)$ est une bijection continue de $\mathsf{X}(A)$ sur Sp$^{\Lambda}_A(x)$, et par suite c’est un homéomorphisme puisque $\mathsf{X}(A)$ est compact.

b) Montrons que (i) implique (ii) : si $c= (c_{\lambda})_{\lambda\in\Lambda}\in$ Sp$^{\Lambda}_A(x)$, il existe $\chi \in \mathsf{X}(A)$ tel que $c_{\lambda}=\chi (x_{\lambda})$ pour tout $\lambda$. Pour tout $P\in \mathbf{C}[(X_{\lambda})]$, on a donc $|P(c)|=|P((\chi (x_{\lambda}))_{\lambda\in\Lambda})|=|\chi (P(x))|\leqslant \varrho (P(x))$.

L’assertion (ii) implique (iii) en raison de l’inégalité $\varrho (x)\leqslant \|x\|$, valide pour tout $x\in A$ par définition du rayon spectral.

Montrons finalement que (iii) implique (i). Soit $c= (c_{\lambda})_{\lambda\in\Lambda}\in \mathbf{C}^{\Lambda}$ tel que

$$
|P(c)|\leqslant \|P(x)\| \tag{2}
$$

pour tout P $\in \mathbf{C}[(X_{\lambda})]$. Soit $A'$ la sous-algèbre unifère de A engendrée par la famille $x$; ses éléments sont de la forme $P(x)$ pour $P\in \mathbf{C}[(X_{\lambda})]$. La majoration (2) implique que la condition $P(x) = 0$ entraîne $P(c) = 0$. Il existe donc un morphisme d’algèbres unifères $\xi$ de $A'$ dans $\mathbf{C}$ tel que $\xi (x_{\lambda}) =c_{\lambda}$ pour tout $\lambda \in \Lambda$. D’après (2), le morphisme $\xi$ est continu. Il se prolonge donc par continuité en un caractère $\chi$ de $\overline{A'}= A$, qui vérifie $c= (\chi (x_{\lambda}))_{\lambda\in\Lambda}\in$ Sp$^{\Lambda}_A(x)$. Cela termine la démonstration.

### 7. Ensembles polynomialement convexes

#### Définition 3 {#ts-i-s3-def-3 .statement tag=028Q}

Soient Λ un ensemble et V une partie de $\mathbf{C}^{\Lambda}$. On dit que V est polynomialement convexe si V est l’ensemble des points $(c_{\lambda})_{\lambda\in\Lambda}$ de $\mathbf{C}^{\Lambda}$ tel que

$|P((c_{\lambda}))|\leqslant$ sup$_{c\in V}|P(c)|$

pour tout $P\in \mathbf{C}[(X_{\lambda})]$.

#### Lemme 3 {#ts-i-s3-lem-3 .statement tag=028R}

Soit Λ un ensemble. Une partie V de $\mathbf{C}^{\Lambda}$ est polynomialement convexe si et seulement s’il existe une famille $(P_i)_{i\in I}$ d’éléments de $\mathbf{C}[(X_{\lambda})_{\lambda\in\Lambda}]$ et une famille $(M_i)_{i\in I}$ d’éléments de $[0,+\infty ]$ tels que V soit l’ensemble des $c\in \mathbf{C}^{\Lambda}$ vérifiant

$$
|P_i(c)|\leqslant M_i
$$

pour tout $i\in I$.

Si la partie V de $\mathbf{C}^{\Lambda}$ est polynomialement convexe, elle vérifie la condition ci-dessus pour la famille formée des éléments P de $\mathbf{C}[(X_{\lambda})_{\lambda\in\Lambda}]$ en posant $M_P=$ sup$_{c\in V}|P(c)|$.

Réciproquement, soient $(P_i)_{i\in I}$ une famille d’éléments de $\mathbf{C}[(X_{\lambda})_{\lambda\in\Lambda}]$ et $(M_i)_{i\in I}$ une famille d’éléments de $[0,+\infty ]$. Soit V l’ensemble des $c$ dans $\mathbf{C}^{\Lambda}$ tels que $|P_i(c)|\leqslant M_i$ pour tout $i\in I$. On a alors sup$_{c\in V}|P_i(c)|\leqslant M_i$ pour $i\in I$. Supposons que $x\in \mathbf{C}^{\Lambda}$ vérifie

$|P(x)|\leqslant$ sup$_{c\in V}|P(c)|$

pour tout $P\in \mathbf{C}[(X_{\lambda})]$. Pour $i\in I$, on a en particulier $|P_i(x)|\leqslant M_i$, donc $x\in V$. Inversement, pour tout élément $x\in V$ et tout polynôme $P\in \mathbf{C}[(X_{\lambda})]$, on a $|P(x)|\leqslant$ sup$_{c\in V}|P(c)|$. Par conséquent, l’ensemble V est polynomialement convexe.

#### Lemme 4 {#ts-i-s3-lem-4 .statement tag=028S}

Soit A une algèbre de Banach commutative unifère. Soient Λ un ensemble et $x= (x_{\lambda})_{\lambda\in\Lambda}$ une famille d’éléments de A. Si la sous-algèbre unifère engendrée par la famille $x$ est dense dans A, alors le spectre simultané Sp$^{\Lambda}_A(x)$ est polynomialement convexe.

Cela résulte de l’assertion b) de la prop. 12 de I, p. 43 et de la définition 3.

Toute intersection de parties polynomialement convexes de $\mathbf{C}^{\Lambda}$ est polynomialement convexe (lemme 3). Cela justifie la définition suivante :

#### Définition 4 {#ts-i-s3-def-4 .statement tag=028T}

Soient Λ un ensemble et V une partie de $\mathbf{C}^{\Lambda}$. L’enveloppe polynomialement convexe de V est le plus petit sous-ensemble polynomialement convexe de $\mathbf{C}^{\Lambda}$ contenant V.

L’enveloppe polynomialement convexe de V est l’ensemble des $c$ appartenant à $\mathbf{C}^{\Lambda}$ tels que $|P(c)|\leqslant$ sup$_W|P|$ pour tout $P\in \mathbf{C}[(X_{\lambda})]$. En effet, cet ensemble est polynomialement convexe par le lemme 3, et est contenu dans tout ensemble polynomialement convexe contenant V par définition.

#### Exemple {#ts-i-s3-n7-exa-1 .statement tag=028U}

Soient Λ un ensemble fini et $V\subset \mathbf{C}^{\Lambda}$ une partie convexe compacte. Alors V est polynomialement convexe. En effet, soit W l’enveloppe polynomialement convexe de V. Démontrons que $W\subset V$, ce qui entraînera l’assertion. Soit $x\in \mathbf{C}^{\Lambda}-$V. Il existe un hyperplan réel H dans $\mathbf{C}^{\Lambda}$ qui sépare strictement $x$ et V (EVT, II, p. 41, prop. 4). Soient $f_{\mathbf{R}}$ une forme $\mathbf{R}$-linéaire sur $\mathbf{C}^{\Lambda}$ et $\alpha \in \mathbf{R}$ tels que H est l’ensemble des $y\in \mathbf{C}^{\Lambda}$ vérifiant $f_{\mathbf{R}}(y) =\alpha$. Soit $f$ une forme linéaire sur $\mathbf{C}^{\Lambda}$ telle que $f_{\mathbf{R}}=\mathscr{R}(f)$. On a donc

$\mathscr{R}(f(x))>$ sup$\mathscr{R}(f(y))$.

$y\in V$

Pour tout $t\in \mathbf{R}$ et $y\in V$, posons $f_t(y) =t+f(y)$. On a $|f_t|-\mathscr{R}(f_t)\rightarrow 0$ dans $\mathscr{C}(\mathbf{C}^{\Lambda},\mathbf{R})$ muni de la topologie de la convergence compacte quand $t\rightarrow +\infty$. Pour $t$ suffisamment grand, il vient $|f_t(x)|>$ sup$_{y\in V}|f_t(y)|$ puisque V est compacte. Ainsi $x\in \mathbf{C}^{\Lambda}-$ W puisque $f_t$ est une fonction polynomiale.

#### Lemme 5 {#ts-i-s3-lem-5 .statement tag=028V}

Soit K une partie compacte de $\mathbf{C}$. On note $\widehat{K}$ la réunion de K et des composantes connexes de $\mathbf{C}-$ K qui sont relativement compactes. Alors l’ensemble $\widehat{K}$ est compact.

Comme K est compact, il existe un nombre réel $r >0$ tel que K est contenu dans le disque ouvert D de centre 0 et de rayon $r$. Alors $\mathbf{C}-$ K contient $\mathbf{C}-$D. Comme l’espace $\mathbf{C}-$ D est connexe (étant homéomorphe à $[r,+\infty [\times \mathbf{S}^1)$, il est contenu dans une composante connexe U de $\mathbf{C}-$K. Toute autre composante connexe de $\mathbf{C}-$ K est contenue dans D, donc est bornée. La composante connexe U est alors l’unique composante connexe non bornée de $\mathbf{C}-$ K, c’est-à-dire $U =\mathbf{C}-\widehat{K}$. Puisque U est ouvert et contient le complémentaire du disque D, l’ensemble $\widehat{K}$ est compact.

#### Proposition 13 {#ts-i-s3-prop-13 .statement tag=028W}

Soit $n\geqslant 1$ un entier. Soit $K\subset \mathbf{C}^n$ une partie fermée et V son enveloppe polynomialement convexe.

a) Toute composante connexe bornée de $\mathbf{C}^n-$ K est contenue dans V ;

b) Si $n= 1$, et si K est compact, alors V est la réunion $\widehat{K}$ de K et des composantes connexes bornées de $\mathbf{C}-$ K.

Comme $K\subset \mathbf{C}^n$ est fermé, son complémentaire $\mathbf{C}^n-$ K est ouvert, donc localement connexe, de sorte que chaque composante connexe de $\mathbf{C}^n-$ K est ouverte. Le principe du maximum (VAR, R1, p. 29, 3.3.7) montre alors que toute composante connexe bornée de $\mathbf{C}^n-$ K est contenue dans V, ce qui montre l’assertion a).

Supposons maintenant $n= 1$ et K compact. Notons $\widehat{K}$ la réunion de K et des composantes connexes bornées de $\mathbf{C}-$ K, de sorte que $\widehat{K}\subset$ V par ce qui précède. L’ensemble $\widehat{K}$ est compact (lemme 5). Soit A l’algèbre de Banach unifère commutative $\mathscr{C}(\widehat{K})$. Soient $x\in A$ la fonction identique de $\widehat{K}$ et B la sous-algèbre unifère fermée de A engendrée par $x$. On a Sp$_A(x) =\widehat{K}$ (exemple 3 de I, p. 17), donc $\mathbf{C}-$ Sp$_A(x)$ est connexe. Par suite on a Sp$_B(x) =$ Sp$_A(x)$ (cor. de la prop. 6 de I, p. 28). Comme Sp$_B(x)$ est polynomialement convexe d’après le lemme 4, cela montre que $\widehat{K}$ est polynomialement convexe et donc que $V\subset \widehat{K}$.

La seconde partie de la proposition ne s’étend pas au cas $n\geqslant 2$ (cf. exerc. 23 de I, p. 170).

#### Proposition 14 {#ts-i-s3-prop-14 .statement tag=028X}

Soit Λ un ensemble. Soient A une algèbre de Banach unifère commutative, $x= (x_{\lambda})_{\lambda\in\Lambda}$ une famille d’éléments de A et $A'$ la sous-algèbre de Banach unifère engendrée par $x$. Alors le spectre simultané Sp$^{\Lambda}_{A'}(x)$ est l’enveloppe polynomialement convexe de Sp$^{\Lambda}_A(x)$.

En effet, la prop. 12 de I, p. 43, b) démontre que Sp$^{\Lambda}_{A'}(x)$ est l’ensemble des $c\in \mathbf{C}^{\Lambda}$ tels que $|P(c)|\leqslant \varrho (P(x))$ pour tout $P\in \mathbf{C}[(X_{\lambda})]$. Or on a $\varrho (P(x)) =$ sup $|\chi (P(x))|=$ sup $|P((\chi (x_{\lambda}))_{\lambda\in\Lambda})|=$ sup $|P(c)|$,

$\chi \in \mathsf{X}(A)\chi \in \mathsf{X}(A)c\in$Sp$^{\Lambda}_A(x)$

d’après la prop. 7 de I, p. 38, a) et la prop. 12 de I, p. 43, a). Le résultat découle alors du lemme 3.

#### Proposition 15 {#ts-i-s3-prop-15 .statement tag=028Y}

Soit Λ un ensemble. Soit K une partie compacte polynomialement convexe de $\mathbf{C}^{\Lambda}$. Soit $A_0$ l’ensemble des restrictions à K des fonctions polynômes sur $\mathbf{C}^{\Lambda}$, et soit A l’adhérence de $A_0$ dans l’algèbre $\mathscr{C}(K)$.

Soit ev$: K\rightarrow \mathsf{X}(A)$ l’application définie par $x\mapsto$ ev$_x$, où ev$_x$ est le caractère $f\mapsto f(x)$ de A. Soit $z= (z_{\lambda})_{\lambda\in\Lambda}$ la famille dans A des restrictions à K des fonctions coordonnées sur $\mathbf{C}^{\Lambda}$, et soit $\varphi$ l’application surjective de $\mathsf{X}(A)$ dans Sp$^{\Lambda}_A(z)$ définie par la famille $z$.

Alors on a K = Sp$^{\Lambda}_A(z)$, et les applications ev : K $\rightarrow \mathsf{X}(A)$ et $\varphi :\mathsf{X}(A)\rightarrow K$ sont des homéomorphismes réciproques.

L’application $\varphi \circ$ ev est l’application identique de K. En particulier, K est contenu dans l’image Sp$^{\Lambda}_A(z)$ de $\varphi$.

La prop. 14 implique que Sp$^{\Lambda}_A(z)$ est l’enveloppe polynomialement convexe de Sp$^{\Lambda}_{\mathscr{C}(K)}(z)$. Puisque, d’autre part, on a Sp$^{\Lambda}_{\mathscr{C}(K)}(z) = K$ (I, p. 42, exemple), qui est polynomialement convexe par hypothèse, on en déduit que Sp$^{\Lambda}_A(z) = K$.

Puisque la sous-algèbre unifère engendrée par la famille des éléments $z_{\lambda}$ est dense dans A, l’application $\varphi$ est un homéomorphisme de $\mathsf{X}(A)$ sur Sp$^{\Lambda}_A(z) = K$ (prop. 12 de I, p. 43, a)). L’identité $\varphi \circ$ ev = Id$_K$ démontre alors que ev est l’homéomorphisme réciproque de $\varphi$.

Pour toute partie $\Lambda '$ de Λ, on note pr$_{\Lambda'}$ la projection canonique $\mathbf{C}^{\Lambda}\rightarrow \mathbf{C}^{\Lambda'}$. Soient W une partie de $\mathbf{C}^{\Lambda}$ et V son enveloppe polynomialement convexe. Posons $W'=$ pr$_{\Lambda'}W$. Comme tout élément de $\mathbf{C}[(X_{\lambda})_{\lambda\in\Lambda'}]$ s’identifie à un élément de $\mathbf{C}[(X_{\lambda})_{\lambda\in\Lambda}]$, l’enveloppe polynomialement convexe de $W'$ est contenue dans pr$_{\Lambda'}V$.

#### Lemme 6 {#ts-i-s3-lem-6 .statement tag=028Z}

Soient $K\subset \mathbf{C}^{\Lambda}$ une partie compacte polynomialement convexe et U un voisinage de K. Il existe une partie finie $\Lambda_0$ de Λ telle que, pour toute partie $\Lambda '$ de Λ contenant $\Lambda_0$, l’ensemble pr$_{\Lambda'}(U)$ contienne l’enveloppe polynomialement convexe de pr$_{\Lambda'}(K)$.

Puisque K est compact, il existe une famille de disques compacts $D_{\lambda}$ dans $\mathbf{C}$ de centre 0 et de rayons $R_{\lambda}$ tels que K est contenu dans le produit $D =\prod_{\lambda}D_{\lambda}$. Pour tout $P\in \mathbf{C}[(X_{\lambda})]$, soit $K_P$ l’ensemble des $x\in \mathbf{C}^{\Lambda}$ tels que

$|P(x)|\leqslant$ sup$|P(c)|$.

$c\in K$

On a

$$
D\cap \bigcap_PK_P= K \tag{3}
$$

qui est contenu dans U. Ainsi, l’espace D est la réunion de l’ensemble ouvert $D\cap U$ et de la famille des ensembles ouverts D - $K_P$ pour $P\in \mathbf{C}[(X_{\lambda})]$. Comme D est compact, il existe un entier $q\geqslant 1$ et des polynômes $P_1, . . . ,P_q\in \mathbf{C}[(X_{\lambda})]$ tels que :

$$
D\cap K_{P_1}\cap  \cdots  \cap K_{P_q}\subset U \tag{4}
$$

Il existe un ensemble fini $\Lambda_0\subset$ Λ tel que $P_i\in \mathbf{C}[(X_{\lambda})_{\lambda\in\Lambda_0}]$ pour $1\leqslant i\leqslant q$. Démontrons que $\Lambda_0$ vérifie l’assertion du lemme.

Soit $\Lambda '$ une partie de Λ contenant $\Lambda_0$. Soit E la partie de $\mathbf{C}^{\Lambda'}$ formée des éléments $c= (c_{\lambda})_{\lambda\in\Lambda'}$ définie par les inégalités $|c_{\lambda}|\leqslant R_{\lambda}$ pour $\lambda \in \Lambda '$, et

$|P_i(c)|\leqslant$ sup$_{c\in K}|P_i(c)|$

pour $i= 1, . . . ,q$. La partie E est polynomialement convexe (lemme 3) et la formule (3) démontre que pr$_{\Lambda'}(K)\subset E$.

D’autre part, soit $c= (c_{\lambda})_{\lambda\in\Lambda'}\in E$ ; soit $d= (d_{\lambda})_{\lambda\in\Lambda}$ l’élément de $\mathbf{C}^{\Lambda}$ défini par $d_{\lambda}=c_{\lambda}$ pour $\lambda \in \Lambda '$ et $d_{\lambda}= 0$ pour $\lambda \in \Lambda$- $\Lambda '$. Alors (4) implique que $d\in U$, et donc que $c\in$ pr$_{\Lambda'}(U)$. Ainsi, $E\subset$ pr$_{\Lambda'}(U)$, ce qui achève la démonstration.

#### Lemme 7 {#ts-i-s3-lem-7 .statement tag=0290}

Soient $n\geqslant 1$ un entier et K une partie compacte polynomialement convexe de $\mathbf{C}^n$. Alors K admet un système fondamental de voisinages compacts polynomialement convexes.

Il existe un polydisque (cf. VAR, R1, p. 24) compact Δ de $\mathbf{C}^n$ qui est un voisinage de K. Puisque K est polynomialement convexe, il existe une famille $(P_i)_{i\in I}$ d’éléments de $\mathbf{C}[X_1, . . . ,X_n]$, et une famille $(M_i)_{i\in I}$ de nombres réels positifs tels que K est l’ensemble des $z\in$ Δ vérifiant $|P_i(z)|\leqslant M_i$ pour tout $i$ (lemme 3). Pour toute partie finie J de I et tout $\varepsilon  >0$, soit $K_{J,\varepsilon}$ l’ensemble des $z\in \Delta$ tels que $|P_i(z)|\leqslant M_i+\varepsilon$ pour $i\in J$. Alors chaque ensemble $K_{J,\varepsilon}$ est un voisinage compact polynomialement convexe de K (loc. cit.), et l’intersection des ensembles $K_{J,\varepsilon}$ est K. Les ensembles $K_{J,\varepsilon}$ forment donc un système fondamental de voisinages polynomialement convexes de K (TG, I, p. 60, th. 1).

## EXERCICES {#ts-i-s3-exercises}

Dans les exercices ci-dessous, toutes les algèbres considérées sont sur $\mathbf{C}$, sauf mention explicite du contraire.

See the [exercises for § 3](exercises/s3/).
