---
book: alg
book_title: Algebra
chapter: V
chapter_title: Corps commutatifs
section: 11
section_title: EXTENSIONS ABÉLIENNES
lang: fr
source: alg-iv-vii-fr
book_pages: A V.152-A V.156
pdf_pages: 0177-0193, 0256-0260
extraction: ocr
subsections:
    - "no": 1
      title: Extensions abéliennes et clôture abélienne
      page: 0
      pdf_page: 177
    - "no": 2
      title: Racines de l’unité
      page: 74
      pdf_page: 178
    - "no": 3
      title: Racines primitives de l’unité
      page: 76
      pdf_page: 180
    - "no": 4
      title: Extensions cyclotomiques
      page: 0
      pdf_page: 181
    - "no": 5
      title: Irréductibilité des polynômes cyclotomiques
      page: 80
      pdf_page: 184
    - "no": 6
      title: Extensions cycliques
      page: 81
      pdf_page: 185
    - "no": 7
      title: Dualité des $\mathbf{Z}/n\mathbf{Z}$-modules
      page: 82
      pdf_page: 186
    - "no": 8
      title: Théorie de Kummer
      page: 84
      pdf_page: 188
    - "no": 9
      title: Théorie d’Artin-Schreier
      page: 0
      pdf_page: 191
statements: 42
exercises: 23
content_sha256: a7d120eb9909dcf5ef661f53cfcd32f9f607d9ae2ce4cd59743ab6d3a0b09fc9
---

## § 11. EXTENSIONS ABÉLIENNES

Dans tout ce paragraphe, on note $K$ un corps.

### 1. Extensions abéliennes et clôture abélienne

#### Définition 1 {#alg-v-s11-def-1 .statement}

On dit qu’une extension $E$ de $K$ est abélienne si elle est galoisienne et si son groupe de Galois est commutatif.

Comme tout sous-groupe d’un groupe commutatif est distingué, le cor. 4 de V, p. 66, montre que toute sous-extension d’une extension abélienne est abélienne.

#### Proposition 1 {#alg-v-s11-prop-1 .statement}

Soient E une extension galoisienne de K, et Γ son groupe de Galois. Soit Δ le groupe dérivé de Γ (I, p. 67, déf. 4) et soit F le corps des invariants de Δ. Pour qu’une sous-extension L de E soit abélienne sur K, il faut et il suffit qu’elle soit contenue dans F.

Notons d’abord que F est aussi le corps des invariants de l’adhérence $\overline{\Delta}$ de Δ dans Γ, et que $\overline{\Delta}$ est un sous-groupe distingué fermé de Γ. D’après V, p. 66, cor. 4, F est donc une extension galoisienne de K. De plus, le groupe de Galois de F sur K est isomorphe à $\Gamma / \overline{\Delta}$, donc est commutatif. Toute sous-extension de F est donc abélienne. Réciproquement, soit L une extension abélienne de K contenue dans E, et soit Π le groupe de Galois de E sur L. Comme L est galoisienne, Π est un sous-groupe distingué de Γ et le groupe de Galois de L sur K est isomorphe à $\Gamma / \Pi$ (V, p. 66, cor. 4). Par suite, $\Gamma / \Pi$ est commutatif et Π contient Δ ; d’où $L \subset F$.

#### Corollaire {#alg-v-s11-n1-cor-1 .statement}

Soit E une extension de K, et soit $(E_i)_{i \in I}$ une famille de sous-extensions de E, telle que $E = K(\bigcup_{i \in I} E_i)$. On suppose que chacune des extensions $E_i$ est abélienne ; il en est alors de même de E.

Tout d’abord, E est extension galoisienne de K (V, p. 55, prop. 1). Si le corps F est défini comme dans la prop. 1, on a $E_i \subset F$ pour tout $i \in I$, d’où $F = E$.

On dit qu’une extension E de K est une clôture abélienne de K si c’est une extension abélienne de K, et si toute extension abélienne de K est isomorphe à une sous-extension de E. La prop. 1 entraîne l’existence d’une clôture abélienne de K : en effet, soit $K_s$ une clôture séparable de K, de groupe de Galois Γ et soit $(\overline{\Gamma}, \overline{\Gamma})$ l’adhérence du groupe dérivé de Γ ; notons $K_{ab}$ le corps des invariants de $(\overline{\Gamma}, \overline{\Gamma})$; comme toute extension algébrique séparable de K est isomorphe à une sous-extension de $K_s$ (V, p. 44, cor.), la prop. 1 montre que $K_{ab}$ est une clôture abélienne de K. Le groupe de Galois de $K_{ab}$ sur K est canoniquement isomorphe à $\Gamma / (\overline{\Gamma}, \overline{\Gamma})$. Démontrons maintenant l’unicité des clôtures abéliennes : soient E et E’ deux clôtures abéliennes de K ; il existe par définition des K-homomorphismes $u : E \to E'$ et $v : E' \to E$, et la prop. 1 (V, p. 50) entraîne $v(u(E)) = E$ et $u(v(E')) = E'$, donc $u$ est un K-isomorphisme de E sur E’. Tout autre K-isomorphisme de E sur E’ est de la forme $u_1 = \sigma_0 \circ u$ avec $\sigma_0 \in \mathrm{Gal}(E'/K)$; comme $\mathrm{Gal}(E'/K)$ est commutatif, l’isomorphisme $\sigma \mapsto u \circ \sigma \circ u^{-1}$ de $\mathrm{Gal}(E/K)$ sur $\mathrm{Gal}(E'/K)$ est indépendant de $u$; on l’appelle l’isomorphisme canonique de $\mathrm{Gal}(E/K)$ sur $\mathrm{Gal}(E'/K)$.

### 2. Racines de l’unité

#### Définition 2 {#alg-v-s11-def-2 .statement}

On dit qu’un élément $\zeta$ de K est une racine de l’unité s’il existe un entier $n > 0$ tel que $\zeta^n = 1$; pour tout entier $n > 0$ tel que $\zeta^n = 1$, on dit que $\zeta$ est racine n-ième de l’unité.

Il revient au même de dire que les racines de l’unité sont les éléments d’ordre fini du groupe multiplicatif $K^*$ des éléments $\neq 0$ de $K$ (I, p. 49). Les racines de l’unité forment un sous-groupe $\mu_\infty(K)$ de $K^*$, et les racines $n$-ièmes un sous-groupe $\mu_n(K)$ de $\mu_\infty(K)$. On a $\mu_\infty(K) = \bigcup_{n \geq 1} \mu_n(K)$ et $\mu_n(K) \subset \mu_m(K)$ si $n$ divise $m$. Pour toute racine de l’unité $\zeta$, il existe un plus petit entier $n \geq 1$ tel que $\zeta$ appartienne à $\mu_n(K)$, à savoir l’ordre de $\zeta$ dans le groupe $K^*$.

Le groupe $\mu_n(K)$ étant l’ensemble des racines du polynôme $X^n - 1$ est d’ordre fini $\leq n$. Soit $p$ la caractéristique de $K$. Lorsque l’on a $p = 0$, ou bien que l’on a $p \neq 0$ et $n$ non divisible par $p$, la dérivée $nX^{n-1}$ de $X^n - 1$ est étrangère à $X^n - 1$, et le polynôme $X^n - 1$ est donc séparable ; si, de plus, $K$ est algébriquement clos, $\mu_n(K)$ est donc un groupe à $n$ éléments.

Supposons que $K$ soit de caractéristique non nulle $p$ et soit $r \geq 0$ un entier ; comme l’application $x \mapsto x^{p^r}$ de $K$ dans $K$ est injective, on a $\mu_{npr}(K) = \mu_n(K)$ pour tout entier $n \geq 1$.

On notera qu’un corps peut ne contenir aucune racine $n$-ième de l’unité autre que 1 : c’est le cas par exemple des corps premiers $\mathbf{Q}$ et $\mathbf{F}_2$ pour tout entier $n$ impair.

#### Théorème 1 {#alg-v-s11-thm-1 .statement}

Soit $p$ l’exposant caractéristique de $K$ et soit $n > 0$ un entier. Le groupe $\mu_n(K)$ des racines $n$-ièmes de l’unité dans $K$ est cyclique et son ordre divise $n$. Lorsque $K$ est algébriquement clos et que $n$ est premier à $p$, le groupe $\mu_n(K)$ est cyclique d’ordre $n$.

Il suffit de prouver la première assertion du théorème, qui résulte du lemme plus précis suivant :

#### Lemme 1 {#alg-v-s11-lem-1 .statement}

Soit $G$ un sous-groupe fini de $K^*$, d’ordre $m$. Alors $G$ est cyclique et l’on a $G = \mu_m(K)$.

Considérons $G$ comme un $\mathbf{Z}$-module ; on a $mx = 0$ pour tout $x \in G$, donc l’annulateur de $G$ est un idéal de la forme $r\mathbf{Z}$ où l’entier $r \geq 1$ divise $m$. On a donc $G \subset \mu_r(K)$. D’après le lemme 4 (V, p. 71) appliqué à $A = \mathbf{Z}$ et $M = G$, il existe un élément $x$ de $G$ d’ordre $r$ ; soit $G'$ le sous-groupe cyclique de $G$ engendré par $x$. On a $G' \subset \mu_r(K)$, Card $G' = r$ et Card $\mu_r(K) \leq r$ ; on a, par suite, $G' = \mu_r(K) \supset G$ et $G$ est cyclique d’ordre $r$, égal à $\mu_r(K)$. Comme $G$ est d’ordre $m$, on a $m = r$, d’où le lemme 1.

#### Proposition 2 {#alg-v-s11-prop-2 .statement}

Supposons que $K$ soit algébriquement clos, et soit $p$ son exposant caractéristique. Il existe un isomorphisme de $\mu_\infty(K)$ sur le groupe $\mathbf{Q}/\mathbf{Z}[1/p]$.

On a noté $\mathbf{Z}[1/p]$ le sous-anneau de $\mathbf{Q}$ engendré par $1/p$, c’est-à-dire l’ensemble des nombres rationnels de la forme $a/p^n$ avec $a \in \mathbf{Z}$ et $n \geq 1$ ; on a donc $\mathbf{Z}[1/p] = \mathbf{Z}$ si $K$ est de caractéristique 0.

Soit $(\nu_n)_{n \geq 1}$ la suite strictement croissante formée de tous les entiers qui ne sont pas divisibles par $p$ si $p \neq 1$ ; posons $\lambda_n = \nu_1 \nu_2 \ldots \nu_n$, et désignons par $H_n$ le groupe des racines $\lambda_n$-ièmes de l’unité ; on a $H_{n+1} \supset H_n$ et $\mu_\infty(K) = \bigcup_n H_n$. Comme $H_n$ est cyclique d’ordre $\lambda_n$ (th. 1), il existe une suite $(\alpha_n)_{n \geq 1}$ de racines de l’unité telle que $\alpha_n$ engendre $H_n$ et que $\alpha_n = \alpha_{n+1}^{v_n + 1}$.

Par ailleurs, soit $\beta_n$ la classe modulo $\mathbf{Z}[1/p]$ de $1/\lambda_n$, et soit $H'_n$ le sous-groupe cyclique de $\mathbf{Q}/\mathbf{Z}[1/p]$ engendré par $\beta_n$. Il est immédiat qu’on a $\beta_n = v_{n+1} \beta_{n+1}$ et $H'_n$ est d’ordre $\lambda_n$, car $\lambda_n$ n’est pas divisible par $p$ si $p \neq 1$. Il existe donc pour tout $n \geq 1$ un isomorphisme $\varphi_n : H_n \to H'_n$ tel que $\varphi_n(\alpha_n) = \beta_n$ et les relations $\alpha_n = \alpha_{n+1}^{v_n + 1}$, $\beta_n = v_{n+1} \beta_{n+1}$ montrent que $\varphi_{n+1}$ prolonge $\varphi_n$. Finalement, il existe un unique isomorphisme $\varphi$ de $\mu_\infty(K)$ sur $\mathbf{Q}/\mathbf{Z}[1/p]$ prolongeant les isomorphismes $\varphi_n$, c’est-à-dire tel que $\varphi(\alpha_n) = \beta_n$ pour tout $n \geq 1$.

#### Remarque 1 {#alg-v-s11-n2-rem-1 .statement}

Lorsque K est un corps algébriquement clos de caractéristique 0, le groupe $\mu_\infty(K)$ est donc isomorphe (non canoniquement) à $\mathbf{Q}/\mathbf{Z}$. \* Lorsque K est le corps $\mathbf{C}$ des nombres complexes, on peut expliciter un tel isomorphisme ; en effet, l’application $x \mapsto e^{2\pi i x}$ est un homomorphisme de $\mathbf{Q}$ dans $\mathbf{C}^*$ de noyau $\mathbf{Z}$ et d’image $\mu_\infty(\mathbf{C})$; elle définit donc par passage au quotient un isomorphisme de $\mathbf{Q}/\mathbf{Z}$ sur $\mu_\infty(\mathbf{C})$. \*
2) On peut prouver (cf. V, p. 156, exerc. 21) le résultat suivant : soient G et H deux groupes commutatifs dont tout élément est d’ordre fini. On suppose que, pour tout entier $n \geq 1$, l’équation $nx = 0$ a le même nombre de solutions, supposé fini, dans G que dans H. Les groupes G et H sont alors isomorphes. Ceci fournit une nouvelle démonstration de la prop. 2.
3) Pour tout nombre premier $l$, posons $\mu_{l^\infty}(K) = \bigcup_{n \geq 0} \mu_{l^n}(K)$. Lorsque $l$ est la caractéristique $p$ de K, on a $\mu_{p^\infty}(K) = \{ 1 \}$. On déduit de I, p. 76, théorème 4, que $\mu_\infty(K)$ est somme directe des sous-groupes $\mu_{l^\infty}(K)$ où $l$ parcourt l’ensemble des nombres premiers distincts de $p$. Pour un nombre premier $l$ donné, deux cas seulement sont possibles : ou bien $\mu_{l^\infty}(K)$ est fini et alors $\mu_{l^\infty}(K)$ est isomorphe à $\mathbf{Z}/l^n\mathbf{Z}$ pour un $n$ convenable (th. 1), ou bien $\mu_{l^\infty}(K)$ est infini et alors $\mu_{l^\infty}(K)$ est isomorphe à $\mathbf{Z}[l^{-1}]/\mathbf{Z}$ (cf. remarque 2).

### 3. Racines primitives de l’unité

Soit $n \geq 1$ un entier. On appelle indicateur d’Euler de $n$, et l’on note $\varphi(n)$, le nombre des éléments inversibles de l’anneau $\mathbf{Z}/n\mathbf{Z}$ des entiers modulo $n$. D’après la proposition suivante, $\varphi(n)$ est aussi le nombre des entiers $k$ premiers à $n$ et tels que $0 \leq k < n$.

#### Proposition 3 {#alg-v-s11-prop-3 .statement}

Soient $k$ et $n \geq 1$ deux entiers. Les assertions suivantes sont équivalentes :
a) la classe de $k$ modulo $n$ est inversible dans l’anneau $\mathbf{Z}/n\mathbf{Z}$;
b) la classe de $k$ modulo $n$ engendre le groupe cyclique $\mathbf{Z}/n\mathbf{Z}$;
c) les entiers $k$ et $n$ sont premiers entre eux (I, p. 106).
Chacune des conditions a) et b) signifie qu’il existe un entier $x$ tel que $kx \equiv 1 \mod n$, c’est-à-dire qu’il existe deux entiers $x$ et $y$ tels que $kx + ny = 1$. Cette dernière condition signifie que $k$ et $n$ sont premiers entre eux.

#### Corollaire 1 {#alg-v-s11-prop-3-cor-1 .statement}

Soit $G$ un groupe cyclique d’ordre $n$ et soit $d$ un diviseur de $n$. Le nombre des éléments d’ordre $d$ de $G$ est égal à $\varphi(d)$. En particulier, $\varphi(n)$ est le nombre des générateurs de $G$.
Comme le groupe $G$ est isomorphe à $\mathbf{Z}/n\mathbf{Z}$, le nombre des générateurs de $G$ est égal à $\varphi(n)$ d’après la prop. 3. Soit $g$ un générateur de $G$; alors les éléments $h$ de $G$ tels que $h^d = 1$ constituent le sous-groupe H de G engendré par $g^{n/d}$; ce groupe est cyclique d’ordre $d$, et les éléments d’ordre $d$ de G sont les générateurs de H, donc leur nombre est égal à $\varphi(d)$.

#### Corollaire 2 {#alg-v-s11-prop-3-cor-2 .statement}

Pour tout entier $n \geqslant 1$, on a

$$
\sum_{d|n} \varphi(d) = n,
$$

l’entier $d$ parcourant l’ensemble des diviseurs $> 0$ de $n$¹.

Avec les notations du cor. 1, tout élément de G a un ordre fini qui est un diviseur $d$ de $n$, et il y a $\varphi(d)$ tels éléments pour $d$ fixé.

Le calcul de $\varphi(n)$ repose sur les deux formules :

(2) $\varphi(mn) = \varphi(m)\varphi(n)$ si $m$ et $n$ sont premiers entre eux,

(3) $\varphi(p^a) = p^{a-1}(p-1)$ ($p$ premier, $a \geqslant 1$).

La première résulte immédiatement de ce que les anneaux $\mathbf{Z}/mn\mathbf{Z}$ et $(\mathbf{Z}/m\mathbf{Z}) \times (\mathbf{Z}/n\mathbf{Z})$ sont isomorphes (I, p. 107), et que l’on a $(\mathbf{A} \times \mathbf{B})^* = \mathbf{A}^* \times \mathbf{B}^*$ pour deux anneaux $\mathbf{A}$ et $\mathbf{B}$. Pour prouver (3), remarquons que les diviseurs positifs de $p^a$ sont $1, p, p^2, \ldots, p^a$; par conséquent, l’entier $k$ n’a pas d’autre diviseur commun avec $p^a$ que 1 si et seulement s’il n’est pas divisible par $p$; comme il y a $p^{a-1}$ multiples de $p$ compris entre 0 et $p^a - 1$, on a bien (3).

Les formules (2) et (3) entraînent aussitôt

$$
\varphi(n) = n \prod_p (1 - 1/p),
$$

où $p$ parcourt l’ensemble des diviseurs premiers de $n$.

On dit qu’une racine $n$-ième de l’unité est primitive si elle est d’ordre $n$; s’il existe une telle racine $\zeta$, le groupe $\mu_n(\mathbf{K})$ est d’ordre $n$ et il est engendré par $\zeta$. \* Par exemple, les racines primitives $n$-ièmes de l’unité dans $\mathbf{C}$ sont les nombres $e^{2\pi i k/n}$ avec $0 \leqslant k < n$ et $k$ premier à $n$. \* Le cor. 1 de la prop. 3 entraîne le résultat suivant.

#### Proposition 4 {#alg-v-s11-prop-4 .statement}

Soit $n \geqslant 1$ un entier ; on suppose qu’il existe $n$ racines $n$-ièmes de l’unité dans $\mathbf{K}$ (ce qui a lieu par exemple si $\mathbf{K}$ est séparablement clos et $n.1_\mathbf{K} \neq 0$). Le nombre des racines primitives $n$-ièmes de l’unité dans $\mathbf{K}$ est égal à $\varphi(n)$.

### 4. Extensions cyclotomiques

Soit $p$ l’exposant caractéristique de $\mathbf{K}$, et soit $n \geqslant 1$ un entier premier à $p$; on appelle extension cyclotomique de niveau $n$ sur $\mathbf{K}$ toute extension de décomposition E du polynôme $X^n - 1$ sur $\mathbf{K}$ (V, p. 20). Comme ce polynôme est séparable, E

¹ La relation $d|n$ entre entiers $> 0$ signifie « $d$ divise $n$ » (cf. VI, p. 5).

est une extension galoisienne de K, de degré fini (V, p. 55). Il existe une racine primitive n-ième de l’unité dans E ; si $\zeta$ est une telle racine, toute racine n-ième de l’unité est une puissance de $\zeta$, donc $E = K(\zeta)$.

Dans la suite de ce numéro, on choisit une clôture séparable $K_s$ de K. Pour tout entier $n \geq 1$ premier à $p$, le groupe $\mu_n(K_s)$ est cyclique d’ordre $n$, et le corps
$$
R_n(K) = K(\mu_n(K_s))
$$
est une extension cyclotomique de niveau $n$ de K. On peut considérer $\mu_n(K_s)$ comme un module libre de rang 1 sur l’anneau $\mathbf{Z}/n\mathbf{Z}$, et tout élément $\sigma$ de Gal$(K_s/K)$ induit un automorphisme de $\mu_n(K_s)$; il existe par suite un homomorphisme $\chi_n : \mathrm{Gal}(K_s/K) \to (\mathbf{Z}/n\mathbf{Z})^*$ caractérisé par la formule $u(\zeta) = \zeta^j$ pour toute racine n-ième de l’unité $\zeta$ dans $K_s$, tout $u$ dans Gal$(K_s/K)$ et tout entier $j$ dans la classe $\chi_n(u)$ modulo $n$. Comme on a $R_n(K) = K(\mu_n(K_s))$, le noyau de $\chi_n$ est le sous-groupe Gal$(K_s/R_n(K))$ de Gal$(K_s/K)$; par suite, on a $\chi_n = \varphi_n \circ \psi_n$ où $\psi_n$ est l’homomorphisme de restriction de Gal$(K_s/K)$ sur Gal$(R_n(K)/K)$ et $\varphi_n$ un homomorphisme injectif de Gal$(R_n(K)/K)$ dans $(\mathbf{Z}/n\mathbf{Z})^*$. En particulier, on a le résultat suivant :

#### Proposition 5 {#alg-v-s11-prop-5 .statement}

*Pour tout entier $n \geq 1$ premier à $p$, l’extension $R_n(K)$ de $K$ est abélienne de degré fini, son groupe de Galois est isomorphe à un sous-groupe de $(\mathbf{Z}/n\mathbf{Z})^*$ et son degré divise l’ordre $\varphi(n)$ de $(\mathbf{Z}/n\mathbf{Z})^*$*.

Soit $\overline{\mathbf{Q}}$ une clôture algébrique du corps $\mathbf{Q}$ des nombres rationnels. Soit $n \geq 1$ un entier. On définit le *polynôme cyclotomique $\Phi_n$ de niveau $n$* par
$$
\Phi_n(X) = \prod_{\zeta \in S_n} (X - \zeta),
$$
où $S_n$ est l’ensemble des racines primitives $n$-ièmes de l’unité dans $\overline{\mathbf{Q}}$. Le polynôme $\Phi_n$ est de degré $\varphi(n)$ (prop. 4). Il est clair que $\Phi_n(X)$ est invariant par tout automorphisme de $\overline{\mathbf{Q}}$, donc appartient à $\mathbf{Q}[X]$. Comme tout élément $\zeta$ de $S_n$ est racine du polynôme $X^n - 1$, le polynôme $\Phi_n(X)$ divise $X^n - 1$, et le lemme suivant montre que $\Phi_n(X)$ est un polynôme unitaire à coefficients *entiers*.

#### Lemme 2 {#alg-v-s11-lem-2 .statement}

*Soient $f, g$ et $h$ des polynômes unitaires de $\mathbf{Q}[X]$ tels que $f = gh$. Si $f$ est à coefficients entiers, il en est de même de $g$ et $h$*.

Soit $a$ (resp. $b$) le plus petit des entiers $\alpha \geq 1$ (resp. $\beta \geq 1$) tels que $\alpha g$ (resp. $\beta h$) ait tous ses coefficients entiers ; posons $g' = ag$ et $h' = bh$ et montrons par l’absurde que l’on a $a = b = 1$. Sinon, il existerait un diviseur premier $p$ de $ab$. Si $u \in \mathbf{Z}[X]$, notons $\bar{u}$ le polynôme à coefficients dans le corps $F_p$ obtenu par réduction modulo $p$ des coefficients de $u$. On a $g'h' = abf$, d’où $\bar{g}'\bar{h}' = 0$; comme l’anneau $F_p[X]$ est intègre (IV, p. 9, prop. 8), on a donc $\bar{g}' = 0$ ou $\bar{h}' = 0$. Autrement dit, $p$ divise tous les coefficients de $g'$ ou tous ceux de $h'$ et ceci contredit les hypothèses faites.

On a la relation
$$
X^n - 1 = \prod_{d|n} \Phi_d(X).
$$

En effet, on a $X^n - 1 = \prod_{\zeta \in \mu_n(\mathbf{Q})} (X - \zeta)$ et les ensembles $S_d$ pour $d$ divisant $n$ forment une partition de $\mu_n(\mathbf{Q})$.

La formule (6) détermine $\Phi_n(X)$ lorsqu’on connaît les $\Phi_d(X)$ pour tous les diviseurs $d < n$ de $n$; comme $\Phi_1(X) = X - 1$, on a ainsi un procédé de récurrence pour calculer $\Phi_n$. Par exemple pour $p$ premier, on a

$$
X^p - 1 = (X - 1)\, \Phi_p(X),
$$

d’où

$$
\Phi_p(X) = X^{p-1} + X^{p-2} + \cdots + X + 1,
$$

et

$$
\Phi_{pr+1}(X) = \Phi_p(X^{pr}) \quad \text{pour } r \geqslant 0.
$$

Donnons les valeurs des polynômes $\Phi_n(X)$ pour $1 \leqslant n \leqslant 12$:

$$
\begin{align*}
\Phi_1(X) &= X - 1 \\
\Phi_2(X) &= X + 1 \\
\Phi_3(X) &= X^2 + X + 1 \\
\Phi_4(X) &= X^2 + 1 \\
\Phi_5(X) &= X^4 + X^3 + X^2 + X + 1 \\
\Phi_6(X) &= X^2 - X + 1 \\
\Phi_7(X) &= X^6 + X^5 + X^4 + X^3 + X^2 + X + 1 \\
\Phi_8(X) &= X^4 + 1 \\
\Phi_9(X) &= X^6 + X^3 + 1 \\
\Phi_{10}(X) &= X^4 - X^3 + X^2 - X + 1 \\
\Phi_{11}(X) &= X^{10} + X^9 + X^8 + X^7 + X^6 + X^5 + X^4 + X^3 + X^2 + X + 1 \\
\Phi_{12}(X) &= X^4 - X^2 + 1
\end{align*}
$$

Les valeurs de $\Phi_1, \Phi_2, \Phi_3, \Phi_4, \Phi_5, \Phi_7, \Phi_8, \Phi_9$ et $\Phi_{11}$ résultent directement des formules (7); on a $\Phi_1 \Phi_2 \Phi_3 \Phi_6 = X^6 - 1$ et $\Phi_1 \Phi_2 \Phi_3 \Phi_4 \Phi_6 \Phi_{12} = X^{12} - 1$, d’où

$$
\Phi_4 \Phi_{12} = \frac{X^{12} - 1}{X^6 - 1} = X^6 + 1 \quad \text{et finalement} \quad \Phi_{12} = \frac{X^6 + 1}{X^2 + 1} = X^4 - X^2 + 1.
$$

Les cas $n = 6$ et $n = 10$ se traitent de manière analogue.

#### Remarque {#alg-v-s11-n4-rem-1 .statement}

\* Pour tout entier $n > 0$, on définit $\mu(n)$ de la façon suivante : si $n$ est divisible par le carré d’un nombre premier, on a $\mu(n) = 0$; sinon, on a $\mu(n) = (-1)^h$ si $n$ est le produit de $h$ nombres premiers distincts (« fonction de Möbius »). On peut montrer qu’on a

$$
\Phi_n(X) = \prod_{d|n} (X^{n/d} - 1)^{\mu(d)},
$$

c’est-à-dire plus explicitement

(9) $$
\Phi_n(X) = \prod_{p_1 < \ldots < p_h} (X^{n/p_1 \ldots p_h} - 1)^{(-1)^h}
$$

où $(p_1, \ldots, p_h)$ parcourt l’ensemble des suites strictement croissantes de diviseurs premiers de $n$ (*cf. LIE, II, p. 94, exerc. 1). \*

### 5. Irréductibilité des polynômes cyclotomiques

Soit $p$ l’exposant caractéristique de $K$ et soit $n \geq 1$ un entier premier à $p$. Notons $\Phi_n \in K[X]$ l’image du polynôme à coefficients entiers $\Phi_n$ par l’unique homomorphisme de $\mathbf{Z}[X]$ dans $K[X]$ qui applique $X$ sur $X$.

#### Lemme 3 {#alg-v-s11-lem-3 .statement}

*Les racines de $\Phi_n$ dans $K_s$ sont les racines primitives $n$-ièmes de l’unité.*

Notons $S_n$ l’ensemble des racines de $\Phi_n$ dans $K_s$. D’après la formule (6), l’ensemble $\mu_n(K_s)$ est réunion des $S_d$ pour $d$ divisant $n$. Toute racine primitive $n$-ième de l’unité appartient donc à $S_n$, et le lemme résulte de la prop. 4 (V, p. 77).

#### Proposition 6 {#alg-v-s11-prop-6 .statement}

*Soit $p$ l’exposant caractéristique de $K$ et soit $n \geq 1$ un entier premier à $p$. Pour que le polynôme $\Phi_n(X)$ soit irréductible dans $K[X]$, il faut et il suffit que l’homomorphisme $\chi_n : \mathrm{Gal}(K_s/K) \to (\mathbf{Z}/n\mathbf{Z})^*$ soit surjectif.*

D’après le lemme 3, on a $R_n(K) = K(\zeta)$ pour toute racine $\zeta$ de $\Phi_n(X)$ et par suite $\Phi_n(X)$ est irréductible dans $K[X]$ si et seulement si le degré $\varphi(n)$ de $\Phi_n(X)$ est égal à $[R_n(K) : K]$. Par ailleurs, le groupe de Galois de $R_n(K)$ sur $K$ est d’ordre $[R_n(K) : K]$ et il est isomorphe au sous-groupe de $(\mathbf{Z}/n\mathbf{Z})^*$ image de $\chi_n$. La prop. 6 résulte alors de ce que $(\mathbf{Z}/n\mathbf{Z})^*$ est d’ordre $\varphi(n)$.

*Théorème 2 (Gauss).* — *Soient $\overline{\mathbf{Q}}$ une clôture algébrique de $\mathbf{Q}$ et $n \geq 1$ un entier.*
  a) *Le polynôme cyclotomique $\Phi_n(X)$ est irréductible dans $\mathbf{Q}[X]$.*
  b) *Le degré de $R_n(\mathbf{Q})$ sur $\mathbf{Q}$ est égal à $\varphi(n)$.*
  c) *L’homomorphisme $\chi_n$ de $\mathrm{Gal}(\overline{\mathbf{Q}}/\mathbf{Q})$ dans $(\mathbf{Z}/n\mathbf{Z})^*$ est surjectif, et définit par passage au quotient un isomorphisme de $\mathrm{Gal}(R_n(\mathbf{Q})/\mathbf{Q})$ sur $(\mathbf{Z}/n\mathbf{Z})^*$.*

Compte tenu de la prop. 6, il suffit de prouver l’assertion c). Tout entier $r$ premier à $n$ est le produit de nombres premiers $p_1, \ldots, p_s$ ne divisant pas $n$ ; il suffit donc de prouver que pour tout nombre premier $p$ ne divisant pas $n$, l’application $x \mapsto x^p$ de $\mu_n(\mathbf{Q})$ dans lui-même se prolonge en un automorphisme de $R_n(\mathbf{Q})$. Il suffira de prouver que, si $\zeta$ est une racine primitive $n$-ième de l’unité, le polynôme minimal $f$ de $\zeta$ sur $\mathbf{Q}$ est égal au polynôme minimal $g$ de $\zeta^p$ sur $\mathbf{Q}$.

Raisonnons par l’absurde en supposant $f \neq g$. Les polynômes $f$ et $g$ sont unitaires et irréductibles dans $\mathbf{Q}[X]$ et divisent $X^n - 1$, et il existe donc $u \in \mathbf{Q}[X]$ tel que $X^n - 1 = fgu$ (IV, p. 13, prop. 13). Le lemme 2 (V, p. 78) montre que $f, g$ et $u$ sont à coefficients entiers. Notons $\bar{v}$ le polynôme à coefficients dans $\mathbf{F}_p$ déduit d’un polynôme $v \in \mathbf{Z}[X]$ par réduction modulo $p$. On a donc $X^n - 1 = \bar{f} \bar{g} \bar{u}$ dans $\mathbf{F}_p[X]$.

Par ailleurs, on a $g(\zeta^p) = 0$ et $g(X^p)$ est donc multiple de $f(X)$ dans $\mathbf{Q}[X]$. D’après le lemme 2, il existe $h \in \mathbf{Z}[X]$ tel que $g(X^p) = f(X).h(X)$. Or on a $v(X^p) = v(X)^p$ pour tout polynôme $v \in \mathbf{F}_p[X]$. Par réduction modulo $p$, on obtient donc $\bar{g}^p = \bar{f}\bar{h}$. Si $v$ est un polynôme unitaire irréductible dans $\mathbf{F}_p[X]$ divisant $\bar{f}$, il divise donc $\bar{g}$. Comme $\bar{f}\bar{g}$ divise $X^n - 1$, on voit que $v^2$ divise $X^n - 1$ dans $\mathbf{F}_p[X]$. Ceci est absurde car le polynôme $X^n - 1$ est séparable dans $\mathbf{F}_p[X]$.

On peut montrer que, pour toute extension abélienne E de degré fini sur $\mathbf{Q}$, il existe un entier $n \geqslant 1$ tel que E soit isomorphe à une sous-extension de $R_n(\mathbf{Q})$. \* Autrement dit, le corps $\mathbf{Q}(\mu_\infty(\mathbf{C}))$ est une clôture abélienne de $\mathbf{Q}$. \* (« Théorème de Kronecker-Weber ».)

### 6. Extensions cycliques

#### Définition 3 {#alg-v-s11-def-3 .statement}

On dit qu’une extension E de K est cyclique, si elle est galoisienne et si son groupe de Galois est cyclique.

#### Exemple 1 {#alg-v-s11-n6-exa-1 .statement}

Toute extension galoisienne de degré premier est cyclique, car tout groupe fini G d’ordre premier $p$ est cyclique (en effet, tout élément $x \neq 1$ de G est d’ordre $p$, donc engendre G).
2) Soit $F(X) = X^2 + aX + b$ un polynôme irréductible dans $K[X]$. Le seul cas où $F(X)$ n’est pas séparable est celui où K est de caractéristique 2 et $a = 0$. On écarte désormais ce cas ; soit E une extension de K engendrée par une racine $x$ de $F(X)$. On a $[E : K] = 2$, et $F(X) = (X - x)(X + a + x)$, donc E est une extension galoisienne de K. Le groupe de Galois de E par rapport à K est d’ordre 2, donc cyclique.
3) Soient F un corps et $\sigma$ un automorphisme d’ordre fini $n$. Le corps E des invariants de $\sigma$ est aussi le corps des invariants du groupe cyclique d’ordre $n$ engendré par $\sigma$, et par suite (V, p. 64, th. 3), F est une extension cyclique de degré $n$ de E.

On sait (I, p. 48) que tout sous-groupe et tout groupe quotient d’un groupe cyclique est cyclique. Par suite (V, p. 66, cor. 4), si E est une extension cyclique d’un corps K, de degré $n$, toute sous-extension F de E est cyclique sur K, et E est cyclique sur F. Pour tout diviseur $d$ de $n$, il existe un unique sous-corps F de degré $d$ sur K contenu dans E : en effet, dans un groupe cyclique d’ordre $n$, il existe un unique sous-groupe d’indice $d$.

#### Théorème 3 (Hilbert) {#alg-v-s11-thm-3 .statement}

Soit E une extension cyclique de K, et soit $\sigma$ un générateur du groupe de Galois $\Gamma$ de E sur K.
a) Pour qu’un élément $x \in E$ soit tel que $N_{E/K}(x) = 1$, il faut et il suffit qu’il existe $y \in E^*$ tel que $x = y/\sigma(y)$; tout $y_1 \in E^*$ tel que $x = y_1/\sigma(y_1)$ est alors de la forme $\lambda y$, avec $\lambda \in K^*$.
b) Pour qu’un élément $x \in E$ soit tel que $\mathrm{Tr}_{E/K}(x) = 0$, il faut et il suffit qu’il existe $z \in E$ tel que $x = z - \sigma(z)$; tout $z_1 \in E$ tel que $x = z_1 - \sigma(z_1)$ est alors de la forme $z + \mu$, avec $\mu \in K$.

Prouvons d’abord un lemme.
Lemme 4. — Soient $\Gamma$ un groupe cyclique d’ordre $n$, $\sigma$ un générateur de $\Gamma$ et M un groupe commutatif sur lequel opère $\Gamma$ de façon que $\gamma.(m + m') = \gamma.m + \gamma.m'$ pour tous $\gamma \in \Gamma, m, m' \in M$. Soit $Z$ l’ensemble des applications $f$ de $\Gamma$ dans $M$ satisfaisant à la relation

$$(10)$$
$$ f(\tau \tau') = f(\tau) + \tau . f(\tau') \quad \text{pour } \tau, \tau' \text{ dans } \Gamma . $$

Posons $u(f) = f(\sigma)$ pour $f \in Z$ et $t(m) = \sum_{\tau \in \Gamma} \tau . m$ pour $m \in M$. Alors la suite
$$ 0 \to Z \xrightarrow{u} M \xrightarrow{t} M $$
est exacte.

Soit $f \in Z$; faisant $\tau = \tau' = 1$ dans (10), on obtient $f(1) = 0$. De plus, on déduit par récurrence sur $m \geqslant 0$ la relation
$$(11)$$
$$ f(\sigma^m) = f(\sigma) + \sigma . f(\sigma) + \cdots + \sigma^{m-2} . f(\sigma) + \sigma^{m-1} . f(\sigma) . $$

On a $\sigma^n = 1$, d’où $f(\sigma^n) = 0$; la relation précédente avec $m = n$ équivaut à l’égalité $t(u(f)) = 0$, d’où $\operatorname{Im} u \subset \operatorname{Ker} t$. En outre, il résulte de (11) que $\operatorname{Ker} u = 0$.

Soit $m \in M$ tel que $t(m) = 0$, c’est-à-dire $m + \sigma . m + \cdots + \sigma^{n-1} . m = 0$. Définissons l’application $f$ de $\Gamma$ dans $M$ par
$$(12)$$
$$ f(\sigma^j) = m + \sigma . m + \cdots + \sigma^{j-2} . m + \sigma^{j-1} . m $$
pour $0 \leqslant j \leqslant n - 1$. On laisse au lecteur le soin d’établir la relation (10). On a évidemment $m = f(\sigma)$, d’où $\operatorname{Im} u \supset \operatorname{Ker} t$.

Le lemme étant prouvé, soient $y \in E^*$ et $x = y / \sigma(y)$; on a $N_{E/K}(\sigma(y)) = N_{E/K}(y)$, d’où $N_{E/K}(x) = 1$. Réciproquement, soit $x$ dans $E^*$ tel que $N_{E/K}(x) = 1$; d’après le lemme 4 appliqué à $M = E^*$, il existe une famille d’éléments $(c_\tau)_{\tau \in \Gamma}$ de $E^*$ satisfaisant à la relation $c_{\tau \tau'} = c_\tau . \tau(c_{\tau'})$ pour $\tau, \tau'$ dans $\Gamma$, et $c_\sigma = x$. D’après le cor. 1 de la prop. 9 (V, p. 63), il existe $y \in E^*$ avec $c_\tau = y / \tau(y)$ pour tout $\tau \in \Gamma$, d’où en particulier $x = c_\sigma = y / \sigma(y)$. Si $y_1 \in E^*$ vérifie la relation $x = y_1 / \sigma(y_1)$, on a
$$ \sigma(y_1 y^{-1}) = y_1 y^{-1} , $$
donc $y_1 y^{-1}$ appartient à $K^*$ puisque $\sigma$ engendre le groupe de Galois de $E$ sur $K$. Ceci prouve a).

L’assertion b) se déduit de manière analogue du cor. 2 de la prop. 9 (V, p. 63).

### 7. Dualité des $\mathbf{Z}/n\mathbf{Z}$-modules

Dans ce numéro, on note $n$ un entier $> 0$ et $T$ un groupe cyclique d’ordre $n$. On dit qu’un groupe $G$ est annulé par $n$ si $g^n = 1$ pour tout $g \in G$; si de plus $G$ est commutatif, la structure de groupe de $G$ est sous-jacente à une unique structure de $\mathbf{Z}/n\mathbf{Z}$-module.

Pour tout groupe $G$, notons $\operatorname{Hom}(G, T)$ le groupe des homomorphismes de $G$ dans $T$; c’est un groupe commutatif annulé par $n$.

#### Proposition 7 {#alg-v-s11-prop-7 .statement}

*Soient $G$ un groupe commutatif annulé par $n$ et $H$ un sous-groupe de $G$. L’homomorphisme de restriction $\operatorname{Hom}(G, T) \to \operatorname{Hom}(H, T)$ est surjectif.*

Soit en effet $f : H \to T$ un homomorphisme et prouvons qu’il existe un homomorphisme de $G$ dans $T$ prolongeant $f$. Supposons d’abord $G$ cyclique, engendré par un élément $g$ d’ordre $r$ divisant $n$; notons $t$ un générateur de $T$. Il existe un diviseur $s$ de $r$ tel que $H$ soit engendré par $g^s$ (I, p. 48, prop. 19), et l’on a, pour tout $x \in \mathbf{Z}, f(g^{sx}) = t^{ax}$, où $a$ est un entier tel que $n$ divise $ar/s$. Alors $a/s = (ar/ns)(n/r)$ est entier et l’homomorphisme $g^x \mapsto t^{(a/s)x},\ x \in \mathbf{Z}$, de $G$ dans $T$ prolonge $f$. Dans le cas général, considérons l’ensemble des couples $(H', f')$, où $H'$ est un sous-groupe de $G$ contenant $H$ et $f'$ un homomorphisme de $H'$ dans $T$ prolongeant $f$, et ordonnons-le par la relation $(H', f') \leq (H'', f'')$ si $H' \subset H''$ et si la restriction de $f''$ à $H'$ est $f'$. D’après E, III, p. 20, déf. 3 et th. 2, cet ensemble possède un élément maximal $(H_1, f_1)$, et il suffit de prouver que $H_1 = G$; dans le cas contraire, il existe $g \in G,\ g \notin H_1$, et il suffit de prouver que $f_1$ peut se prolonger en un homomorphisme dans $T$ du sous-groupe de $G$ engendré par $H_1$ et $g$. Or, si $C$ désigne le groupe cyclique engendré par $g$, la restriction de $f_1$ à $C \cap H_1$ se prolonge en un homomorphisme $f_2$ de $C$ dans $T$ et l’homomorphisme $xy \mapsto f_1(x)f_2(y),\ x \in H_1,\ y \in C$, de $H_1C$ dans $T$ répond à la question.

#### Corollaire 1 {#alg-v-s11-prop-7-cor-1 .statement}

*Si $G$ est un groupe commutatif annulé par $n$, et si $G \neq \{1\}$, alors $\mathrm{Hom}(G, T) \neq \{1\}$*.

En effet, il suffit de remarquer que si $H$ est un sous-groupe cyclique de $G$ distinct de $\{1\}$, on a $\mathrm{Hom}(H, T) \neq \{1\}$, et d’appliquer la prop. 7.

#### Corollaire 2 {#alg-v-s11-prop-7-cor-2 .statement}

*Si $G$ est un groupe commutatif fini annulé par $n$, les groupes $G$ et $\mathrm{Hom}(G, T)$ ont même ordre*.

Si $G$ est cyclique d’ordre $r$, de générateur $g$, l’application $f \mapsto f(g)$ est une bijection de $\mathrm{Hom}(G, T)$ sur l’ensemble des éléments $t$ de $T$ tels que $t^r = 1$, d’où l’assertion dans ce cas. D’autre part, si $H$ est un sous-groupe cyclique de $G$, on a $\mathrm{Card}(G) = \mathrm{Card}(H).\mathrm{Card}(G/H)$; par ailleurs, on a une suite exacte

$$
\{1\} \to \mathrm{Hom}(G/H, T) \to \mathrm{Hom}(G, T) \to \mathrm{Hom}(H, T) \to \{1\}
$$

(II, p. 36, th. 1 et prop. 7 ci-dessus), donc

$$
\mathrm{Card}(\mathrm{Hom}(G, T)) = \mathrm{Card}(\mathrm{Hom}(H, T)).\mathrm{Card}(\mathrm{Hom}(G/H, T)).
$$

Comme on a $\mathrm{Card}(\mathrm{Hom}(H, T)) = \mathrm{Card}(H)$, il est équivalent de démontrer le corollaire pour $G$ ou pour $G/H$. On conclut alors par récurrence sur $\mathrm{Card}(G)$.

Soient maintenant $G$ et $H$ deux groupes et $f : G \times H \to T$ une application *bimultiplicative*, c’est-à-dire telle que pour tous $g,\ g' \in G,\ h,\ h' \in H$, on ait

$$
f(gg', h) = f(g, h)f(g', h),\quad f(g, hh') = f(g, h)f(g, h').
$$

On définit des homomorphismes de groupes

$$
s_f : G \to \mathrm{Hom}(H, T),\quad d_f : H \to \mathrm{Hom}(G, T),
$$

par $s_f(g)(h) = d_f(h)(g) = f(g, h)$ (cf. II, p. 74, cor. à la prop. 1, lorsque G et H sont commutatifs).

#### Proposition 8 {#alg-v-s11-prop-8 .statement}

*Supposons G et H commutatifs et annulés par n. Si $s_f$ est bijectif et H fini, alors $d_f$ est bijectif et l’on a $\mathrm{Card}(G) = \mathrm{Card}(H)$.*

Si $s_f$ est bijectif et H fini, on a d’après le corollaire 2 à la prop. 7, la relation $\mathrm{Card}(G) = \mathrm{Card}(\mathrm{Hom}(H, T)) = \mathrm{Card}(H)$, donc $\mathrm{Card}(G)$ est fini et par une nouvelle application du corollaire $\mathrm{Card}(\mathrm{Hom}(G, T)) = \mathrm{Card}(H)$. Il suffit donc de prouver que $d_f$ est injectif. Or, si $h \in \mathrm{Ker}(d_f)$, on a $f(g, h) = 1$ pour tout $g \in G$, donc puisque $s_f$ est bijectif, $\varphi(h) = 1$ pour tout $\varphi \in \mathrm{Hom}(H, T)$; d’après la prop. 7, cela implique $\mathrm{Hom}(\mathrm{Ker}(d_f), T) = \{ 1 \}$, donc $\mathrm{Ker}(d_f) = \{ 1 \}$ d’après le cor. 1 à la prop. 7.

### 8. Théorie de Kummer

Dans ce numéro, on note $n$ un entier $> 0$, et on suppose que $\mu_n(K)$ a $n$ éléments ; d’après V, p. 75, cela signifie aussi que $n$ est premier à l’exposant caractéristique de K et que toutes les racines $n$-ièmes de l’unité dans une clôture algébrique $\Omega$ de K appartiennent à K.

On dit qu’une extension L de K est *abélienne d’exposant divisant n* si elle est abélienne (V, p. 73, déf. 1) et si son groupe de Galois $\mathrm{Gal}(L/K)$ est annulé par $n$ (V, p. 82).

Soit A une partie de $K^*$ ; on note $K(A^{1/n})$ la sous-extension de $\Omega$ engendrée par les $\theta \in \Omega$ tels que $\theta^n \in A$.

#### Lemme 5 {#alg-v-s11-lem-5 .statement}

*$K(A^{1/n})$ est une extension abélienne de K d’exposant divisant n.*

Comme les polynômes $X^n - a, a \in A$, sont séparables sur K, $L = K(A^{1/n})$ est une extension séparable, donc galoisienne, de K. Soit $\sigma \in \mathrm{Gal}(L/K)$ et soit $\theta \in \Omega$ tel que $\theta^n \in A$. On a $\sigma(\theta)^n = \theta^n$ ; il existe donc $\zeta \in \mu_n(\Omega) = \mu_n(K)$ tel que $\sigma(\theta) = \zeta \theta$ : cela implique $\sigma^n(\theta) = \zeta^n \theta = \theta$, d’où $\sigma^n = 1$. Si $\sigma'$ est un autre élément de $\mathrm{Gal}(L/K)$, il existe $\zeta' \in \mu_n(K)$ tel que $\sigma'(\theta) = \zeta' \theta$, d’où $\sigma' \sigma(\theta) = \zeta \zeta' \theta = \sigma \sigma'(\theta)$, et $\sigma' \sigma = \sigma \sigma'$.

#### Lemme 6 {#alg-v-s11-lem-6 .statement}

*Soit L une extension galoisienne de K. Il existe une unique application $(\sigma, a) \mapsto \langle \sigma, a \rangle$ de $\mathrm{Gal}(L/K) \times ((L^n \cap K^*)/K^{*n})$ dans $\mu_n(K)$ telle que pour tout $\sigma \in \mathrm{Gal}(L/K)$ et tout élément $\theta \in L^*$ tel que $\theta^n \in K$, on ait, notant $\overline{\theta}^n$ la classe de $\theta^n$ mod. $K^{*n}$ :

$$
\langle \sigma, \overline{\theta}^n \rangle = \sigma(\theta)/\theta .
$$

Cette application est bimultiplicative.

En effet, le membre de droite de (13) est une racine $n$-ième de l’unité qui ne dépend que de la classe mod. $K^{*n}$ de $\theta^n$ ; cela démontre la première assertion. La seconde se vérifie sans difficultés.

Pour toute extension galoisienne L de K, notons

$$
k_L : (L^n \cap K^*)/K^{*n} \to \operatorname{Hom}(\operatorname{Gal}(L/K), \mu_n(K)) ,
$$
$$
k'_L : \operatorname{Gal}(L/K) \to \operatorname{Hom}((L^n \cap K^*)/K^{*n}, \mu_n(K)) ,
$$

les homomorphismes déduits de l’application bimultiplicative précédente (V, p. 83).

#### Proposition 9 {#alg-v-s11-prop-9 .statement}

*Pour toute extension galoisienne de degré fini L de K, l’homomorphisme k_L est bijectif.*

Soit $\theta \in L^*$ tel que $\theta^n \in K$ et que la classe de $\theta^n$ mod. $K^{*n}$ appartienne au noyau de $k_L$. Pour tout $\sigma \in \operatorname{Gal}(L/K)$, on a par définition $\sigma(\theta) = \theta$; donc $\theta \in K^*$ et $\theta^n \in K^{*n}$. Cela démontre l’injectivité de $k_L$. Soit maintenant $f : \operatorname{Gal}(L/K) \to \mu_n(K)$ un homomorphisme ; pour tous $\sigma, \tau \in \operatorname{Gal}(L/K)$, on a
$$
f(\sigma \tau) = f(\sigma) f(\tau) = f(\sigma) \cdot \sigma f(\tau) , \quad f(\sigma)^n = 1 .
$$
D’après V, p. 63, cor. 1, il existe $\theta \in L^*$ tel que $f(\sigma) = \sigma(\theta)/\theta$ pour tout $\sigma \in \operatorname{Gal}(L/K)$; comme $f(\sigma)^n = 1$, on a $\sigma(\theta^n) = \theta^n$ pour tout $\sigma \in \operatorname{Gal}(L/K)$, donc $\theta^n \in K^*$; si $a$ est la classe de $\theta^n$ mod. $K^{*n}$, on a par définition $f(\sigma) = \langle \sigma, a \rangle$ pour $\sigma \in \operatorname{Gal}(L/K)$, donc $f = k_L(a)$.

#### Corollaire {#alg-v-s11-n8-cor-1 .statement}

*Si L est une extension galoisienne de K, l’homomorphisme k_L est injectif et son image est le groupe $\operatorname{Hom}_c(\operatorname{Gal}(L/K), \mu_n(K))$ des homomorphismes continus du groupe topologique $\operatorname{Gal}(L/K)$ dans le groupe discret $\mu_n(K)$.

Cela résulte aussitôt de ce qui précède, du fait que L est réunion filtrante croissante de sous-extensions galoisiennes $L_i$ de degré fini, et de ce qu’un homomorphisme de $\operatorname{Gal}(L/K)$ dans $\mu_n(K)$ est continu si et seulement s’il se factorise par un des quotients $\operatorname{Gal}(L_i/K)$ de $\operatorname{Gal}(L/K)$.

#### Théorème 4 {#alg-v-s11-thm-4 .statement}

*a) L’application $H \mapsto K(H^{1/n})$ est une bijection croissante de l’ensemble des sous-groupes de $K^*$ contenant $K^{*n}$ sur l’ensemble des sous-extensions abéliennes d’exposant divisant n de $\Omega$. L’application réciproque est $L \mapsto L^n \cap K^*$.
b) Pour tout sous-groupe H de $K^*$ contenant $K^{*n}$, l’homomorphisme
$$
k' : \operatorname{Gal}(K(H^{1/n})/K) \to \operatorname{Hom}(H/K^{*n}, \mu_n(K))
$$
est bijectif. Lorsqu’on munit le groupe $\operatorname{Hom}(H/K^{*n}, \mu_n(K))$ de la topologie de la convergence simple, c’est un homéomorphisme.
c) Soit H un sous-groupe de $K^*$ contenant $K^{*n}$. Pour chaque $a \in H/K^{*n}$, soit $\theta_a$ un élément de $\Omega$ tel que $\theta_a^n$ soit un représentant de a dans H. Alors les $\theta_a, a \in H/K^{*n}$ forment une base du K-espace vectoriel $K(H^{1/n})$. En particulier
$$
[K(H^{1/n}) : K] = (H : K^{*n}) .
$$

A) Pour toute extension abélienne L de K d’exposant divisant n, posons $H_L = L^n \cap K^*$. Si $[L : K]$ est fini, l’homomorphisme $k'_L$ de $\operatorname{Gal}(L/K)$ dans $\operatorname{Hom}(H_L, \mu_n(K))$ est bijectif d’après la prop. 9 et V, p. 84, prop. 8.

Comme toute extension abélienne de K d’exposant divisant n est réunion filtrante croissante de sous-extensions abéliennes de degré fini d’exposant divisant n, on en déduit par passage à la limite projective que $k'_L$ est un homéomorphisme de groupes topologiques pour toute extension abélienne L de K d’exposant divisant n.

B) Soit L une extension abélienne de degré fini, d’exposant divisant n, de K, et soit $L' = K(H_L^{1/n})$; c’est une sous-extension de L ; de plus, $H_{L'}$ contient $H_L$ donc lui est égal. Puisque les homomorphismes $k'_L$ et $k'_{L'}$ sont bijectifs d’après A), et que $H_L = H_{L'}$, les groupes Gal(L/K) et Gal(L'/K) ont même ordre, donc sont égaux. Cela prouve que $L' = L$, donc que $L = K(H_L^{1/n})$. Si L est une extension abélienne d’exposant divisant n de K, on a $K(H_L^{1/n}) = L$, puisque $K(H_L^{1/n})$ est une sous-extension de L qui contient toute sous-extension de degré fini de L.

C) Soit H un sous-groupe de $K^*$ contenant $K^{*n}$; posons $L = K(H^{1/n})$, c’est une extension abélienne de K d’exposant divisant n (V, p. 84, lemme 5). On a $H \subset H_L$, d’où une suite exacte de groupes commutatifs annulés par n
$$
\{1\} \to H/K^{*n} \to H_L/K^{*n} \to H_L/H \to \{1\}.
$$
On en déduit une suite exacte
$$
\{1\} \to \operatorname{Hom}(H_L/H, \mu_n(K)) \to \operatorname{Hom}(H_L/K^{*n}, \mu_n(K)) \xrightarrow{u} \operatorname{Hom}(H/K^{*n}, \mu_n(K)),
$$
où u est l’homomorphisme de restriction.

Si l’on identifie $\operatorname{Hom}(H_L/K^{*n}, \mu_n(K))$ à Gal(L/K) grâce à l’isomorphisme $k'_L$, le noyau de u s’identifie à l’ensemble des $\sigma \in \operatorname{Gal}(L/K)$ tels que $\sigma(\theta) = \theta$ pour tout $\theta \in H^{1/n}$. Il s’ensuit que u est injectif, donc que $\operatorname{Hom}(H_L/H, \mu_n(K))$ est réduit à $\{1\}$; d’après le cor. 1 de V, p. 83, on a donc $H = H_L$. Cela achève de démontrer a) et b).

D) Démontrons c). Si $a, b \in H$, on a $\theta_a \theta_b / \theta_{ab} \in K$. Il en résulte que le sous-espace vectoriel de $K(H^{1/n})$ engendré par les $\theta_a$ est stable par multiplication, donc coïncide avec $K(H^{1/n})$. Il nous reste donc à démontrer que les $\theta_a$ sont linéairement indépendants ; pour ce faire, on peut évidemment supposer que $H/K^{*n}$ est fini ; alors $[K(H^{1/n}) : K] = (\operatorname{Gal}(K(H^{1/n})/K) : \{1\}) = (H : K^{*n})$ d’après b) et le cor. 2 de V, p. 83 ; comme les $\theta_a$ sont au nombre de $(H : K^{*n})$ et engendrent le K-espace vectoriel $K(H^{1/n})$, ils sont linéairement indépendants.

#### Exemple 1 {#alg-v-s11-n8-exa-1 .statement}

Il existe une plus grande extension abélienne d’exposant divisant n de K contenue dans $\Omega$; elle s’obtient en adjoignant à K les racines n-ièmes de tous ses éléments ; son groupe de Galois s’identifie à $\operatorname{Hom}(K^*/K^{*n}, \mu_n(K))$, donc aussi à $\operatorname{Hom}(K^*, \mu_n(K))$.

#### Exemple 2 {#alg-v-s11-n8-exa-2 .statement}

Prenons $K = \mathbf{Q}$ et $n = 2$. Alors $\mathbf{Q}^*/\mathbf{Q}^{*2}$ est un $\mathbf{F}_2$-espace vectoriel admettant pour base la réunion de $\{-1\}$ et de l’ensemble des nombres premiers. La plus grande extension abélienne d’exposant 2 de $\mathbf{Q}$ contenue dans $\mathbf{C}$ est donc le sous-corps $\mathbf{Q}(i, \sqrt{2}, \sqrt{3}, \sqrt{5}, ...)$ de $\mathbf{C}$. Son groupe de Galois est formé de tous les automorphismes obtenus en multipliant de façon indépendante chacun des éléments $i, \sqrt{2}, \sqrt{3}, \sqrt{5}$, etc., par $\pm 1$.

#### Exemple 3 {#alg-v-s11-n8-exa-3 .statement}

Soit L une extension cyclique de K de degré n ; alors le groupe $(L^n \cap K^*)/K^{*n}$ est cyclique d’ordre n. Si $a \in K^*$ est tel que la classe de $a$ mod. $K^{*n}$ est un générateur de ce groupe, alors L est K-isomorphe à K[X]/(X^n - a), et le groupe Gal(L/K) est formé des n automorphismes transformant X en les $\zeta X$, $\zeta \in \mu_n(K)$.

#### Exemple 4 {#alg-v-s11-n8-exa-4 .statement}

Inversement, soit $a \in K^*$, et soit r le plus petit entier > 0 tel que $a^r \in K^{*n}$; alors le sous-corps L de $\Omega$ engendré par les racines du polynôme $X^n - a$ est une extension cyclique de K de degré r. En particulier, $X^n - a$ est irréductible si et seulement si $r = n$.

#### Remarque {#alg-v-s11-n8-rem-1 .statement}

Soit $a \in K^*$ et soit r le plus petit entier > 0 tel que $a^r \in K^n$. Soit B l’ensemble des racines dans K du polynôme $X^{n/r} - a$; alors on a

$$
X^n - a = \prod_{b \in B} (X^r - b),
$$

par substitution de $X^r$ à T dans la relation $T^{n/r} - a = \prod (T - b)$. D’après l’exemple 4, chacun des polynômes $X^r - b$ est irréductible, de sorte que (14) est la décomposition de $X^n - a$ en polynômes irréductibles dans K[X].

### 9. Théorie d’Artin-Schreier

Dans ce numéro, on note p un nombre premier et on suppose que K est de caractéristique p. On note $\Omega$ une clôture algébrique de K et $\rho$ l’endomorphisme du groupe additif de $\Omega$ défini par

$$
\rho(x) = x^p - x .
$$

D’après V, p. 89, le noyau de $\rho$ est le sous-corps premier $F_p$ de K. Pour toute partie A de K, notons $K(\rho^{-1}(A))$ la sous-extension de $\Omega$ engendrée par les $x \in \Omega$ tels que $\rho(x) \in A$.

#### Lemme 7 {#alg-v-s11-lem-7 .statement}

$K(\rho^{-1}(A))$ est une extension abélienne de K d’exposant divisant p.

Comme les polynômes $\rho - a = X^p - X - a, \ a \in A,$ sont séparables sur K, l’extension $L = K(\rho^{-1}(A))$ est galoisienne. Soit $\sigma \in \mathrm{Gal}(L/K)$ et soit $x \in \rho^{-1}(A)$; on a $\rho(\sigma(x)) = \rho(x)$, donc $\sigma(x) - x \in F_p$, c’est-à-dire $\sigma(x) = x + i, \ i \in F_p$. Cela implique $\sigma^p(x) = x + pi = x$, donc $\sigma^p = 1$; de même, si $\sigma' \in \mathrm{Gal}(L/K)$ et si $\sigma'(x) = x + j$, on a $\sigma \circ \sigma'(x) = x + i + j = \sigma' \circ \sigma(x)$, donc $\sigma \circ \sigma' = \sigma' \circ \sigma$.

#### Lemme 8 {#alg-v-s11-lem-8 .statement}

Soit L une extension galoisienne de K. Il existe une unique application $(\sigma, a) \mapsto [\sigma, a]$ de $\mathrm{Gal}(L/K) \times ((\rho(L) \cap K)/\rho(K))$ dans $F_p$ telle que, pour tout $\sigma \in \mathrm{Gal}(L/K)$ et tout élément x de L tel que $\rho(x) \in K$, on ait, notant $\overline{\rho(x)}$ la classe de $\rho(x)$ mod. $\rho(K)$

$$
[\sigma, \overline{\rho(x)}] = \sigma(x) - x .
$$

Cette application est $\mathbf{Z}$-bilinéaire (pour $\sigma, \tau \in \mathrm{Gal}(L/K), \ a, \ b \in (\rho(L) \cap K)/\rho(K)$, on a $[\sigma \tau, a] = [\sigma, a] + [\tau, a], \ [\sigma, a + b] = [\sigma, a] + [\sigma, b]$).

En effet, le second membre de (15) est un élément de $F_p$ qui ne dépend que de la classe de $p(x)$ mod. $p(K)$; cela démontre la première assertion. La seconde se vérifie sans difficultés.

Pour toute extension galoisienne $L$ de $K$, notons
$$
a_L : (\mathfrak{p}(L) \cap K)/\mathfrak{p}(K) \to \mathrm{Hom}(\mathrm{Gal}(L/K), \mathbf{F}_p)
$$
$$
a'_L : \mathrm{Gal}(L/K) \to \mathrm{Hom}((\mathfrak{p}(L) \cap K)/\mathfrak{p}(K), \mathbf{F}_p)
$$
les homomorphismes déduits de l’application $\mathbf{Z}$-bilinéaire précédente (V, p. 83).

#### Proposition 10 {#alg-v-s11-prop-10 .statement}

*Pour toute extension galoisienne de degré fini $L$ de $K$, l’homomorphisme $a_L$ est bijectif.*

Soit $x \in L$ tel que $p(x) \in K$ et que la classe de $p(x)$ mod. $p(K)$ appartienne au noyau de $a_L$. Pour tout $\sigma \in \mathrm{Gal}(L/K)$, on a par définition $\sigma(x) = x$; donc $x \in K$ et $p(x) \in p(K)$. Cela démontre l’injectivité de $a_L$. Soit maintenant $f : \mathrm{Gal}(L/K) \to \mathbf{F}_p$ un homomorphisme ; pour tous $\sigma, \tau \in \mathrm{Gal}(L/K)$, on a
$$
f(\sigma \tau) = f(\sigma) + \sigma(f(\tau)) , \quad f(\sigma) \in \mathbf{F}_p .
$$
D’après V, p. 63, cor. 2, il existe $x \in L$ tel que $f(\sigma) = \sigma(x) - x$ pour tout $\sigma \in \mathrm{Gal}(L/K)$. Comme $f(\sigma) \in \mathbf{F}_p$, on a $p(\sigma(x)) = p(x)$, donc $\sigma(p(x)) = p(x)$ pour tout $\sigma \in \mathrm{Gal}(L/K)$ et $p(x) \in K$. Si $a$ est la classe de $p(x)$ mod. $p(K)$, on a $f(\sigma) = [\sigma, a]$, donc $f = a_L(a)$.

#### Corollaire {#alg-v-s11-n9-cor-1 .statement}

*Si $L$ est une extension galoisienne de $K$, l’homomorphisme $a_L$ est injectif et son image est le groupe $\mathrm{Hom}_c(\mathrm{Gal}(L/K), \mathbf{F}_p)$ des homomorphismes continus du groupe topologique $\mathrm{Gal}(L/K)$ dans le groupe discret $\mathbf{F}_p$.*
Cela se démontre comme le cor. de la prop. 9 de V, p. 85.

#### Théorème 5 {#alg-v-s11-thm-5 .statement}

*a) L’application $A \mapsto K(p^{-1}(A))$ est une bijection de l’ensemble des sous-groupes de $K$ contenant $p(K)$ sur l’ensemble des sous-extensions abéliennes d’exposant divisant $p$ de $\Omega$. L’application réciproque est $L \mapsto \mathfrak{p}(L) \cap K$.
b) Pour tout sous-groupe $A$ de $K$ contenant $p(K)$, l’homomorphisme
$$
a' : \mathrm{Gal}(K(p^{-1}(A))/K) \to \mathrm{Hom}(A/p(K), \mathbf{F}_p)
$$
est bijectif. Lorsqu’on munit $\mathrm{Hom}(A/p(K), \mathbf{F}_p)$ de la topologie de la convergence simple, c’est un homéomorphisme.
c) Soit $A$ un sous-groupe de $K$ contenant $p(K)$ et soit $B$ une base du $\mathbf{F}_p$-espace vectoriel $A/p(K)$. Pour chaque $a \in B$ soit $x_a$ un élément de $\Omega$ tel que $p(x_a)$ soit un représentant de $a$ dans $A$. Alors les monômes $x^\alpha = \prod_{a \in B} x_a^{\alpha(a)}$ avec $\alpha = (\alpha(a))$ dans $\mathbf{N}^{(B)}$ tel que $0 \leq \alpha(a) < p$ pour tout $a \in B$ forment une base du $K$-espace vectoriel $K(p^{-1}(A))$.
En particulier, on a
$$
[K(p^{-1}(A)) : K] = (A : p(K)) .
$$
Le th. 5 se démontre comme le th. 4 (V, p. 85), *mutatis mutandis*.

#### Exemple 1 {#alg-v-s11-n9-exa-1 .statement}

Il existe une plus grande extension abélienne de $K$ d’exposant divisant $p$ contenue dans $\Omega$; c’est $K(p^{-1}(K))$; son groupe de Galois s’identifie à $\mathrm{Hom}(K/p(K), \mathbf{F}_p)$.

#### Exemple 2 {#alg-v-s11-n9-exa-2 .statement}

Soit L une extension cyclique de K de degré $p$; alors le groupe $(\mathfrak{p}(L) \cap K)/\mathfrak{p}(K)$ est cyclique d’ordre $p$. Si $a \in K$ est tel que la classe de $a$ mod. $\mathfrak{p}(K)$ est un générateur de ce groupe, alors L est K-isomorphe à $K[X]/(X^p - X - a)$, et le groupe de Galois $\mathrm{Gal}(L/K)$ est formé des $p$ automorphismes transformant $X$ en $X + i, i \in \mathbf{F}_p$.

#### Exemple 3 {#alg-v-s11-n9-exa-3 .statement}

Inversement, si $a \in K - \mathfrak{p}(K)$, alors le polynôme $X^p - X - a$ est irréductible et le sous-corps L de $\Omega$ engendré par ses racines est une extension cyclique de K de degré $p$. Si $a \in \mathfrak{p}(K)$, alors $X^p - X - a = \prod_{\alpha \in \mathfrak{p}^{-1}(a)} (X - \alpha)$.

## EXERCICES {#alg-v-s11-exercises}

See the [exercises for § 11](exercises/s11/).
