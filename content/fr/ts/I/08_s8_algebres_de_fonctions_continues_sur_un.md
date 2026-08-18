---
book: ts
book_title: Théories spectrales
chapter: I
chapter_title: ALGÈBRES NORMÉES
section: 8
section_title: Algèbres de fonctions continues sur un espace compact
lang: fr
source: ts-i-ii-fr
book_pages: TS I.142-TS I.151, TS I.191-TS I.197
pdf_pages: 0155-0164, 0204-0210
extraction: native
subsections:
    - "no": 1
      title: Sous-algèbres de l’algèbre des fonctions continues sur un espace compact
      page: 142
      pdf_page: 155
    - "no": 2
      title: Fonctions continues sur un sous-ensemble compact de $\mathbf{C}^{\Lambda}$
      page: 146
      pdf_page: 159
    - "no": 3
      title: Fonctions continues sur un sous-ensemble compact de C
      page: 148
      pdf_page: 161
statements: 11
exercises: 11
content_sha256: 6719d8fa02b8619f5a4398d148de092ec4a408ad6829aa3e617eaa85aa532216
---

## § 8. ALGÈBRES DE FONCTIONS CONTINUES SUR UN ESPACE COMPACT

Dans ce paragraphe, le corps de base est $\mathbf{C}$.

### 1. Sous-algèbres de l’algèbre des fonctions continues sur un espace compact

Soient X un espace topologique compact et B une sous-algèbre unifère de $\mathscr{C}(X)$. On note ev l’application $x\mapsto$ ev$_x$ de X dans $\mathsf{X}(B)$ telle que ev$_x(f) =f(x)$ pour tout $f\in B$. On désigne par $j$ l’injection de B dans $\mathscr{C}(X)$, ainsi $\mathsf{X}(j) =$ ev.

#### Proposition 1 {#ts-i-s8-prop-1 .statement tag=02H4}

Soit $f\mapsto  \|f\|_B$ une norme munissant B d’une structure d’algèbre de Banach.

a) L’application $j$ est de norme $\leqslant 1$ dans $\mathscr{L}(B;\mathscr{C}(X))$ ;

b) Le radical de l’algèbre B est nul ;

c) L’application ev est continue de X dans $\mathsf{X}(B)$ ;

d) Si B sépare les points de X, alors l’application ev est un homéo-morphisme de X sur une partie fermée de $\mathsf{X}(B)$.

On peut identifier X à $\mathsf{X}(\mathscr{C}(X))$ et $\mathscr{G}_{\mathscr{C}(X)}$ à l’application identique (exemple 1 de I, p. 36). L’application ev s’identifie alors à $\mathsf{X}(j)$, ce qui démontre c).

Pour toute fonction $f\in B$ et tout $x\in X$, on a $\mathscr{G}_B(f$)(ev$_x) =f(x)$, d’où

$\|f\|_{\mathscr{C}(X)}=$ sup$_{x\in X}|\mathscr{G}_B(f$)(ev$_x)|\leqslant \varrho_B(f)\leqslant \|f\|_B$,

(cf. prop. 7 de I, p. 38, a)) ce qui entraîne a). De plus, ceci montre que la transformation de Gelfand de B est injective, d’où b) (prop. 8 de I, p. 38). Si B sépare les points de X, alors l’application ev est injective, d’où d) puisque X est compact.

On s’intéresse maintenant à la surjectivité de l’application ev.

#### Proposition 2 {#ts-i-s8-prop-2 .statement tag=02H5}

Soit $f\mapsto  \|f\|_B$ une norme telle que $(B,\|\cdot \|_B)$ est une algèbre de Banach.

a) Si l’application ev est surjective, alors l’algèbre B est une sous-algèbre pleine de $\mathscr{C}(X)$ ;

b) Supposons que B est une sous-algèbre pleine de $\mathscr{C}(X)$, et qu’il existe un élément $a\in B$ tel que l’ensemble des éléments $f(a)$, où $f$ parcourt l’ensemble des fonctions rationnelles sur $\mathbf{C}$ sans pôle sur Sp$_B(a)$, est dense dans B. Alors l’application ev est surjective ;

c) Si B est une sous-algèbre involutive pleine de $\mathscr{C}(X)$, alors l’application ev est surjective.

L’assertion a) résulte de la prop. 10 de I, p. 40, et l’assertion b) de la prop. 11 de I, p. 41, puisque la sous-algèbre pleine de B engendrée par $a$ est l’ensemble des éléments $f(a)$, où $f$ parcourt l’ensemble des fonctions rationnelles sur $\mathbf{C}$ sans pôle sur Sp$_B(a)$ (lemme I, p. 6 et prop. 6 de I, p. 37, b)).

Démontrons c). Supposons donc que B est une sous-algèbre involutive pleine de $\mathscr{C}(X)$. Pour démontrer que ev est surjective, il suffit de démontrer que pour tout $\chi \in \mathsf{X}(B)$, il existe $y\in X$ tel que Ker($\chi$ ) $=$ Ker(ev$_y)$ (th. 2 de I, p. 30). Soit I = Ker($\chi$ ). C’est un idéal maximal de B. Soit Φ l’ensemble des $x\in X$ tels que $f(x) = 0$ pour tout $f\in I$. Montrons que Φ n’est pas vide. Dans le cas contraire, puisque X est compact, il existerait un entier $n\geqslant 1$, un recouvrement ouvert $(V_1, . . . ,V_n)$ de X et, pour tout entier $i$ tel que $1\leqslant i\leqslant n$, une fonction $f_i\in I$ telle que $f_i(x)\not= 0$ pour tout $x\in V_i$. Comme l’algèbre B est une sous-algèbre involutive de $\mathscr{C}(X)$, la fonction

$$
f=\sum_{i=1}^nf_i\overline{f}_i
$$

appartiendrait à I. Or $f(x)>0$ pour tout $x\in X$, et donc $f$ serait inversible dans $\mathscr{C}(X)$. Puisque B est supposée être une sous-algèbre pleine de $\mathscr{C}(X)$, la fonction $f\in$ I serait inversible dans B, ce qui ne peut être. Par conséquent, l’ensemble Φ n’est pas vide. Soit $y$ un élément de Φ; le noyau du caractère ev$_y$ contient I, et est donc égal à I.

#### Exemple {#ts-i-s8-n1-exa-1 .statement tag=02H6}

Soient $X = [0,1]$ et $n\geqslant 0$ un entier. Soit B l’algèbre des fonctions $f: X\rightarrow \mathbf{C}$ admettant des dérivées continues sur $[0,1]$ jusqu’à l’ordre $n$, munie de la norme considérée dans l’exemple 4 de I, p. 18. Alors B est une sous-algèbre involutive pleine de $\mathscr{C}(X)$ séparant les points de X, donc $\mathsf{X}(B)$ s’identifie à X.

On considère la fonction logarithme comme définie sur $\mathbf{R}_+$ et à valeurs dans $\mathbf{R}\cup  \{-\infty \}$ en posant log(0) $=-\infty$.

#### Proposition 3 {#ts-i-s8-prop-3 .statement tag=02H7}

Soit X un espace compact. Soit B une sous-algèbre de Banach unifère de $\mathscr{C}(X)$, munie de la norme induite, séparant les points de X. On identifie X à une partie fermée de $\mathsf{X}(B)$ (prop. 1, d)).

a) Pour tout $f\in B$, la transformée de Gelfand $\mathscr{G}_B(f)$ est une fonction continue dans $\mathsf{X}(B)$ qui prolonge $f$ et vérifie $\|f\|=$ sup$|\mathscr{G}_B(f)|$. En particulier, $\mathscr{G}_B$ est un isomorphisme isométrique de B sur une sous-algèbre de Banach de $\mathscr{C}(\mathsf{X}(B))$ ;

b) Soit $B^*$ l’ensemble des éléments inversibles de B. Pour tout caractère $\chi \in \mathsf{X}(B)$, il existe une mesure positive $\mu$ de masse 1 sur X telle que, pour tout $f\in B^*$, on ait

log($|\chi (f)|$) $=\int_X$ log($|f|$)$d\mu$.

De plus, pour tout $f\in B$, on a

$$
\chi (f) =\int_Xf d\mu
$$

c) On suppose que tout élément de $\mathscr{C}_{\mathbf{R}}(X)$ est limite uniforme de parties réelles de fonctions appartenant à B. Alors, pour tout $\chi \in \mathsf{X}(B)$, il existe une unique mesure $\mu_{\chi}\geqslant 0$ sur X telle que, pour toute fonction $f\in B$, on ait

$$
\chi (f) =\int_Xf d\mu_{\chi}
$$

En outre, pour toute fonction $f\in B$, on a

log($|\chi (f)|$)$\leqslant \int_X$ log($|f|$)$d\mu_{\chi}$; la fonction log$|f|$ étant bornée supérieurement, l’intégrale existe dans $\mathbf{R}\cup  \{-\infty \}$.

L’assertion a) résulte de l’identification de X avec un sous-espace fermé de $\mathsf{X}(B)$ et des inégalités

$\|f\|=$ sup$_{x\in X}|f(x)|\leqslant$ sup$_{\chi\in\mathsf{X}(B)}|\chi (f)|=$ sup$|\mathscr{G}_B(f)|=\varrho_B(f)\leqslant \|f\|$

pour tout $f\in B$.

Soient $\chi \in \mathsf{X}(B)$ et $n$ un entier positif. Soient $\lambda_1, . . . , \lambda_n\in \mathbf{R}$ et $f_1, . . . , f_n\in B^*$. On a alors

(1) $\sum_{i=1}^n\lambda_i$ log($|\chi (f_i)|$)$\leqslant$ sup$_{x\in X}(\sum_{i=1}^n\lambda_i$ log($|f_i(x)|$)).

En effet, par continuité, il suffit de prouver cette inégalité quand les nombres réels $\lambda_i$ sont rationnels. Par réduction au même dénominateur, on se ramène au cas où $\lambda_i\in \mathbf{Z}$ pour tout $i$. L’inégalité s’écrit alors

log($|\chi (f_1^{\lambda_1}\cdots f_n^{\lambda_n})|$)$\leqslant$ sup$_{x\in X}$ log($|(f_1^{\lambda_1}\cdots f_n^{\lambda_n})(x)|$),

et résulte du fait que $\|\chi \|= 1$ (th. 1 de I, p. 29).

Soit $B'$ le sous-espace vectoriel de $\mathscr{C}_{\mathbf{R}}(X)$ engendré par les fonctions log($|f|$) pour $f\in B^*$. La majoration (1) prouve qu’il existe une forme linéaire $h$ de norme $\leqslant$ 1 sur $B'$ telle que log($|\chi (f)|$) $=h$(log($|f|$)) pour tout $f\in B^*$. D’après le théorème de Hahn–Banach (EVT, II, p. 24, cor. 2), la forme linéaire $h$ se prolonge en une forme linéaire $\mu$ de norme $\leqslant 1$ sur $\mathscr{C}_{\mathbf{R}}(X)$, c’est–à–dire en une mesure réelle $\mu$ sur X telle que $\|\mu\|\leqslant 1$ (INT, III, §1, n$^o5)$. En prenant pour élément $f$ de $B^*$ la constante $e=$ exp(1), on voit que $1 =\mu(1)$. Donc, en écrivant $\mu=\mu^+-\mu^-$ comme la différence de deux mesures positives étrangères (INT, III, §1, n$^o6$, th. 3), il vient

$$
1 =\mu^+(1)-\mu^-(1)\leqslant \mu^+(1) +\mu^-(1) =\|\mu\|\leqslant 1
$$

d’où $\mu=\mu^+\geqslant 0$ et $\|\mu\|= 1$.

Pour tout $f\in B$, on a exp($f$)$\in B^*$, donc

$\int_X\mathscr{R}(f)d\mu=\int_X$ log($|$exp($f$)$|)d\mu=$ log($|\chi$(exp($f$))$|)$

= log($|$exp($\chi (f)$)$|) =\mathscr{R}(\chi (f))$,

où on a utilisé le cor. 1 de I, p. 66. En appliquant cette égalité à $if$, on en conclut que $\int_Xf d\mu=\chi (f)$. Ceci établit b).

Plaçons-nous dans les hypothèses de c). L’existence de $\mu_{\chi}$ résulte de b). D’autre part, on a $\mu_{\chi}(\mathscr{R}(f)) =\mathscr{R}(\chi (f))$ pour tout $f\in B$. Puisque les parties réelles de fonctions $f\in B$ sont denses dans $\mathscr{C}_{\mathbf{R}}(X)$ par hypothèse, la mesure $\mu_{\chi}$ est déterminée de manière unique par $\chi$.

Soit $f\in B$. Soit $\varepsilon  >0$ un nombre réel. Il existe, par hypothèse, une fonction $g\in B$ telle que

(2) $\mathscr{R}(g)-\varepsilon \leqslant$ log($|f|+\varepsilon$ )$\leqslant \mathscr{R}(g) +\varepsilon$.

Soit $h=$ exp($g$)$\in B^*$. D’après (2), on a

$$
|h|e^{-\varepsilon}\leqslant |f|+\varepsilon \leqslant |h|e^{\varepsilon} \tag{3}
$$

La majoration implique $|f h^{-1}|\leqslant e^{\varepsilon}$, d’où $|\chi (f h^{-1})|\leqslant e^{\varepsilon}$, et par suite

(4) log($|\chi (f)|$)$\leqslant$ log($|\chi (h)|$) $+\varepsilon =\int_X$ log($|h|$)$d\mu_{\chi}+\varepsilon$.

La minoration dans (3) implique alors

log($|\chi (f)|$)$\leqslant \int_X$ log $(|f|+\varepsilon )d\mu_{\chi}+ 2\varepsilon$.

En faisant tendre $\varepsilon$ vers 0, on en déduit que

log($|\chi (f)|$)$\leqslant \int_X$ log($|f|$)$d\mu_{\chi}$.

Ceci finit la démonstration.

### 2. Fonctions continues sur un sous-ensemble compact de $\mathbf{C}^{\Lambda}$

Soient Λ un ensemble et X une partie compacte de $\mathbf{C}^{\Lambda}$. On note P(X) la sous-algèbre de Banach unifère de $\mathscr{C}(X)$ formée des fonctions sur X qui sont limites uniformes sur X de fonctions polynômes sur $\mathbf{C}^{\Lambda}$. Les fonctions coordonnées $z_{\lambda}|X$ engendrent topologiquement P(X), et P(X) sépare les points de X. Soit Y l’enveloppe polynomialement convexe de X (déf. 4 de I, p. 45). Comme

sup$_{z\in Y}|p(z)|=$ sup$_{z\in X}|p(z)|$

(cf. n$^o7$ de I, p. 44) pour tout $p\in \mathbf{C}[(X_{\lambda})_{\lambda\in\Lambda}]$, les suites de polynômes uniformément convergentes dans X se prolongent de manière unique en suites de polynômes uniformément convergentes dans Y. Il existe donc un unique isomorphisme isométrique de P(X) sur P(Y) qui, pour toute fonction coordonnée $z_{\lambda}$ sur $\mathbf{C}^{\Lambda}$, transforme $z_{\lambda}|X$ en $z_{\lambda}|Y$. Cet isomorphisme sera dit canonique.

#### Proposition 4 {#ts-i-s8-prop-4 .statement tag=02H8}

Soit X un espace compact. Soit B une sous-algèbre de Banach unifère de $\mathscr{C}(X)$, munie de la norme induite, séparant les points de X. On identifie X à une partie fermée de $\mathsf{X}(B)$ (prop. 1 de I, p. 142, d)). Soit $(x_{\lambda})_{\lambda\in\Lambda}$ une famille d’éléments de B engendrant topologiquement l’algèbre unifère B. On considère le diagramme commutatif

$$
\leftarrow_i
$$

X $\rightarrow \mathsf{X}(B)$

$$
\rightarrow \leftarrow_{\varphi}\rightarrow \leftarrow_{\varphi'}
$$

$$
_{\Lambda}\leftarrow_{j\Lambda}
$$

Sp$_{\mathscr{C}(X)}((x_{\lambda}))\rightarrow$ Sp$_B((x_{\lambda}))$

où $\varphi$ et $\varphi '$ sont les applications définies par la famille $(x_{\lambda})_{\lambda\in\Lambda}($cf. n$^o6$ de I, p. 41), et $i$ et $j$ sont les injections canoniques. Alors :

a) Les applications $\varphi$ et $\varphi '$ sont des homéomorphismes ;

b) Le spectre simultané Sp$^{\Lambda}_B((x_{\lambda}))$ est l’enveloppe polynomialement convexe de Sp$^{\Lambda}_{\mathscr{C}(X)}((x_{\lambda}))$ ;

c) L’application $\varphi$ transforme $\mathscr{C}(X)$ en $\mathscr{C}$(Sp$^{\Lambda}_{\mathscr{C}(X)}((x_{\lambda})))$ et B en P(Sp$^{\Lambda}_{\mathscr{C}(X)}((x_{\lambda})))$ ;

d) L’application $\varphi '$ transforme $\mathscr{G}_B(B)$ en P(Sp$^{\Lambda}_B((x_{\lambda})))$ ;

e) Les applications $\varphi$ et $\varphi '$ transforment $\mathscr{G}_B$ en l’isomorphisme canonique de P(Sp$^{\Lambda}_{\mathscr{C}(X)}((x_{\lambda})))$ sur P(Sp$^{\Lambda}_B((x_{\lambda})))$.

Les applications $\varphi$ et $\varphi '$ sont continues et surjectives (n$^o6$ de I, p. 41). L’application $\varphi '$ est un homéomorphisme d’après l’assertion a) de la prop. 12 de I, p. 43, et $i$ est injective, donc $\varphi$ est injective. Donc $\varphi$ et $\varphi '$ sont des homéomorphismes.

Soit $X_1$ = Sp$^{\Lambda}_{\mathscr{C}(X)}((x_{\lambda}))$. L’enveloppe polynomialement convexe de $X_1$ est $Y_1=$ Sp$^{\Lambda}_B((x_{\lambda}))$ d’après la prop. 14 de I, p. 46.

Pour tout $\lambda \in \Lambda$, notons $z_{\lambda}$ la fonction coordonnée correspondante sur $\mathbf{C}^{\Lambda}$. L’application $\varphi$ transforme $x_{\lambda}$ en $z_{\lambda}|X_1$, et $\varphi '$ transforme $\mathscr{G}_B(x_{\lambda})$ en $z_{\lambda}|Y_1$. Donc $\varphi$ transforme B en $P(X_1)$, et $\varphi '$ transforme $\mathscr{G}_B(B)$ en $P(Y_1)$. Finalement, $\varphi$ et $\varphi '$ transforment $\mathscr{G}_B$ en l’isomorphisme canonique de $P(X_1)$ sur $P(Y_1)$.

#### Corollaire 1 {#ts-i-s8-prop-4-cor-1 .statement tag=02H9}

Soient Λ un ensemble et X une partie compacte de $\mathbf{C}^{\Lambda}$. On identifie X à une partie de $\mathsf{X}(P(X))$ (prop. 1 de I, p. 142, d)). Soit $(z_{\lambda})_{\lambda\in\Lambda}$ la famille des fonctions coordonnées sur $\mathbf{C}^{\Lambda}$.

a) L’application $\theta$ de $\mathsf{X}(P(X))$ sur Sp$^{\Lambda}_{P(X)}((z_{\lambda}))$ définie par la famille $(z_{\lambda})$ est un homéomorphisme de $\mathsf{X}(P(X))$ sur l’enveloppe polynomialement convexe Y de X. Sa restriction à X est l’application identique de X ;

b) Pour toute fonction $f\in P(X)$, l’homéomorphisme $\theta$ transforme le prolongement $\mathscr{G}_{P(X)}(f)$ de $f$ à $\mathsf{X}(P(X))$ en un prolongement $\widetilde{f}$ de $f$ à Y. L’application $f\mapsto \widetilde{f}$ est l’isomorphisme canonique de P(X) sur P(Y).

Dans la prop. 4, prenons B = P(X) et $x_{\lambda}=z_{\lambda}$. Alors $\varphi$ devient l’application identique et $\varphi '$ devient l’application $\theta$. Les assertions du corollaire se réduisent alors à celles de loc. cit.

#### Corollaire 2 {#ts-i-s8-prop-4-cor-2 .statement tag=02HA}

Soit Λ un ensemble et soit $X\subset \mathbf{C}^{\Lambda}$ un ensemble compact. Si X est connexe, alors son enveloppe polynomialement convexe est connexe.

Si X est connexe, les seuls idempotents de $\mathscr{C}(X)$, donc de P(X), sont 0 et 1 (cor. de la prop. I, p. 79). Par conséquent, l’espace $\mathsf{X}(P(X))$ est connexe (loc. cit.) ; or cet ensemble est homémorphe à l’enveloppe polynomialement convexe de X (cor. 1, a)).

### 3. Fonctions continues sur un sous-ensemble compact de C

#### Lemme 1 {#ts-i-s8-lem-1 .statement tag=02HB}

Soit X un sous-ensemble compact du plan et soit O une composante connexe bornée de $\mathbf{C}-$ X. La frontière de O est contenue dans X.

L’adhérence de l’ensemble O dans $\mathbf{C}-$ X est égale à $\overline{O}\cap (\mathbf{C}-$ X) où $\overline{O}$ est son adhérence dans $\mathbf{C}$. Comme O est une composante connexe de $\mathbf{C}-$ X, on a donc $\overline{O}\cap (\mathbf{C}-$ X) = O, ce qui démontre bien que $\overline{O}-O\subset X$.

Soit X une partie compacte de $\mathbf{C}$. Soit $O_{\infty}$ la composante connexe non bornée de $\mathbf{C}-$X, et soit $(O_i)_{i\in I}$ la famille des composantes connexes bornées de $\mathbf{C}-$ X, les parties $O_i$ étant deux à deux distinctes.

Soit E une partie de $\mathbf{C}-$ X. On note $R_E(X)$ l’adhérence dans $\mathscr{C}(X)$ de l’ensemble des fonctions $f|X$, où $f$ est une fonction rationnelle sur $\mathbf{C}$ dont tous les pôles appartiennent à E. L’algèbre $R_E(X)$ est une sous-algèbre de Banach unifère de $\mathscr{C}(X)$ qui sépare les points de X. Soit $z$ la fonction identique sur X. La sous-algèbre fermée pleine de $R_E(X)$ engendrée par $z$ est égale à $R_E(X)$ (lemme 2 de I, p. 6). Les éléments de $R_E(X)$ sont holomorphes dans l’intérieur de X.

On a en particulier $R_{\emptyset}(X) = P(X)$. On note $R(X) = R_{\mathbf{C}-X}(X)$. On note I(E) l’ensemble des éléments $i\in I$ tels que $E\cap O_i=\emptyset$, et

$$
X_E= X\cup (\bigcup_{i\in I(E)}O_i)
$$

L’ensemble $X_E$ est compact, car borné et fermé, son complémentaire dans $\mathbf{C}$ étant la réunion de l’ouvert $O_{\infty}$ et des ouverts $O_i$ qui rencontrent E.

#### Proposition 5 {#ts-i-s8-prop-5 .statement tag=02HC}

Avec les notations ci-dessus :

a) L’application de restriction $h$ de $R_E(X_E)$ dans $R_E(X)$ est un isomorphisme isométrique ;

b) L’algèbre $R_E(X_E)$ est une sous-algèbre pleine de $\mathscr{C}(X_E)$ ;

c) Tout caractère de $R_E(X_E)$ est de la forme $f\mapsto f(w)$, où $w$ est un élément de $X_E$;

d) L’application $\chi \mapsto \chi (z)$ est un homéomorphisme de $\mathsf{X}(R_E(X))$ sur $X_E$;

e) Si $E'$ est une partie de $\mathbf{C}-$ X, on a $R_E(X) = R_{E'}(X)$ si et seulement si $X_E= X_{E'}$, ce qui équivaut aussi à $I(E) = I(E')$.

L’application de restriction $h$ de $R_E(X_E)$ dans $R_E(X)$ est un morphisme d’algèbres de Banach tel que $\|h(f)\|\leqslant \|f\|$ pour toute fonction $f\in R_E(X_E)$. Soit $f\in R_E(X_E)$. Soit $i\in I(E)$. Puisque $f$ est holomorphe au voisinage de l’ouvert borné $O_i$, le principe du maximum (VAR, I, p. 29) implique qu’il existe un élément $z_0$ dans la frontière de $O_i$ tel que $|f(z_0)|=$ sup$_{z\in O_i}|f(z)|$. Comme la frontière de $O_i$ est contenue dans X (lemme 1), on en déduit que sup$_{z\in O_i}|f(z)|\leqslant \|h(f)\|$. Puisque cette inégalité vaut pour tout $i\in I(E)$, il en résulte que $\|f\|\leqslant \|h(f)\|$. Le morphisme $h$ est donc isométrique, et en particulier injectif. Démontrons maintenant qu’il est surjectif. Soit $g\in R_E(X)$. Il existe une suite $(f_n)$ de fonctions rationnelles dont les pôles appartiennent à E qui converge uniformément vers $g$ sur X. Les $f_n|X_E$ sont des éléments de $R_E(X_E)$. Puisque $h$ est isométrique, la suite $(f_n|X_E)$ converge dans $\mathscr{C}(X_E)$. Si $f$ est sa limite, on a $f\in R_E(X_E)$ et $g=f|X =h(f)$. D’où a).

Prouvons l’assertion d). Appliquons la prop. 3 de I, p. 144 à l’algèbre $B = R_E(X)$. L’assertion b) de loc. cit. implique que l’application qui à $\chi$ associe $\chi (z)$ est un homéomorphisme de $\mathsf{X}(R_E(X))$ dans Sp$_{R_E(X)}(z)$. Soit $z_E$ l’application identique de $X_E$. D’après loc. cit., a), on a Sp$_{R_E(X)}(z) =$ Sp$_{R_E(X_E)}(z_E)$. Il suffit donc de montrer que Sp$_{R_E(X_E)}(z_E) = X_E$. Le cor. de la prop. 6 de I, p. 28 démontre que Sp$_{R_E(X_E)}(z_E)$ est la réunion de Sp$_{\mathscr{C}(X_E)}(z_E) = X_E$ et de certaines composantes connexes bornées du complémentaire de $X_E$. Soit $O_i$ l’une des composantes connexes bornées du complémentaire de $X_E$. L’intersection $E\cap O_i$ est donc non vide. Soit $\lambda \in E\cap O_i$; puisque $(\lambda -z_E)^{-1}\in R_E(X_E)$, on a $\lambda \notin$ Sp$_{R_E(X_E)}(z_E)$. Ainsi, $O_i$ n’est pas contenu dans Sp$_{R_E(X_E)}(z_E)$. Cela montre que Sp$_{R_E(X_E)}(z_E) = X_E$.

Cette égalité implique par ailleurs que Sp$_{R_E(X_E)}(z_E) =$ Sp$_{\mathscr{C}(X_E)}(z_E)$. Cela établit la condition (iii) de la prop. 11 de I, p. 41, appliquée à l’injection canonique de $R_E(X_E)$ dans $\mathscr{C}(X_E)$ et à l’élément $z_E$. Les assertions b) et c) sont les conditions équivalentes (i) et (ii) de loc. cit.

L’assertion d) démontre que $X_E= X_{E'}$ si $R_E(X) = R_{E'}(X)$. Réciproquement, supposons que $X_E= X_{E'}$. En remplaçant $E'$ par $E\cup E'$, on peut supposer que $E\subset E'$. D’après b), l’algèbre $R_E(X_E)$ est une sous-algèbre fermée pleine de $\mathscr{C}(X_E)$, et donc aussi de $R_{E'}(X_E)$. Elle contient $z_E$, et donc $R_E(X_E) = R_{E'}(X_E)$. Appliquant a), on en déduit que $R_E(X) = R_{E'}(X)$. Finalement l’équivalence de $X_E= X_{E'}$ et $I(E) = I(E')$ est une conséquence des définitions.

#### Corollaire 1 {#ts-i-s8-prop-5-cor-1 .statement tag=02HD}

Les conditions suivantes sont équivalentes :

(i) L’ensemble E rencontre toutes les composantes connexes bornées de $\mathbf{C}-$ X ;

(ii) L’application $\chi \mapsto \chi (z)$ est un homéomorphisme de $\mathsf{X}(R_E(X))$ sur X ;

(iii) On a $R_E(X) = R(X)$.

Soit $E'=\mathbf{C}-$ X. Les conditions (i), (ii) et (iii) sont respectivement équivalentes à $I(E) = I(E')$, à $X_E= X_{E'}$ (d’après la prop. 5, d)) et à $R_E(X) = R_{E'}(X)$. Elles sont donc équivalentes entre elles d’après la prop. 5, e).

Le corollaire suivant précise le théorème de Runge (th. 3 de I, p. 69).

#### Corollaire 2 (Théorème de Runge) {#ts-i-s8-prop-5-cor-2 .statement tag=02HE}

Pour tout $i\in I$, soit $\lambda_i$ un point de $O_i$. Soit $f$ une fonction complexe holomorphe dans un voisinage ouvert de X. Alors $f|X$ est limite uniforme de restrictions à X de fractions rationnelles dont les pôles sont certains des $\lambda_i$.

Avec $E =\{\lambda_i\}_{i\in I}$, l’hypothèse est la condition (i) du cor. 1. On a donc $R_E(X) = R(X)$, et le th. 3 de I, p. 69 montre que $R(X) =\mathscr{O}(X)$.

## EXERCICES {#ts-i-s8-exercises}

Tous les espaces de Banach et toutes les algèbres de Banach ci-dessous sont complexes.

See the [exercises for § 8](exercises/s8/).
