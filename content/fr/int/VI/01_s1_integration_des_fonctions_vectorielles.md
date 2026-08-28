---
book: int
book_title: Integration
chapter: VI
chapter_title: Intégration vectorielle
section: 1
section_title: Intégration des fonctions vectorielles
lang: fr
source: int-vi-fr
pdf_pages: 0008-0029, 0078-0087
extraction: ocr
subsections:
    - "no": 1
      title: Fonctions scalairement essentiellement intégrables.
      page: 0
      pdf_page: 8
    - "no": 2
      title: Propriétés de l’intégrale d’une fonction scalairement essentiellement intégrable.
      page: 0
      pdf_page: 11
    - "no": 3
      title: Intégrales d’opérateurs.
      page: 0
      pdf_page: 14
    - "no": 4
      title: La propriété (GDF).
      page: 0
      pdf_page: 17
    - "no": 5
      title: Applications mesurables et applications scalairement mesurables.
      page: 0
      pdf_page: 21
    - "no": 6
      title: 'Applications : I. Extension d’une fonction continue à un espace de mesures.'
      page: 0
      pdf_page: 22
    - "no": 7
      title: '*Applications : II. Extension à un espace de mesures d’une fonction continue à valeurs dans un espace d’opérateurs.*'
      page: 0
      pdf_page: 25
statements: 35
exercises: 27
content_sha256: 17cf0ae507efd8b0c82660237a41bd845fa95e0499b25b224e7c703269e142ee
---

## § 1. Intégration des fonctions vectorielles

Dans ce paragraphe, $\mu$ désigne une mesure positive sur $T$ et $F$ un espace vectoriel localement convexe séparé sur $\mathbf{R}$. Pour toute application $f$ de $T$ dans $F$, et tout élément $z'$ du dual $F'$ de $F$, on désignera par $\langle f, z' \rangle$ ou $\langle z', f \rangle$ la fonction numérique $z' \circ f$ sur $T$. Nous dirons que $f$ possède scalairement une propriété $P$ si, pour tout $z' \in F'$, $\langle z', f \rangle$ possède la propriété $P$. Par exemple, on dira que $f$ est scalairement essentiellement $\mu$-intégrable si, pour tout $z' \in F'$, $\langle z', f \rangle$ est essentiellement $\mu$-intégrable.

On notera que dans cette définition, la topologie de $F$ n'intervient que par l'intermédiaire du dual $F'$ de $F$. Si une fonction $f$ possède scalairement la propriété $P$, elle possède encore scalairement la propriété $P$ quand on remplace la topologie de $F$ par toute topologie localement convexe séparée compatible avec la dualité entre $F$ et $F'$.

### 1. Fonctions scalairement essentiellement intégrables.

Si $f$ est une application scalairement essentiellement $\mu$-intégrable de $T$ dans $F$, l'application $z' \to \int \langle f(t), z' \rangle d\mu(t)$ est une forme linéaire sur $F'$, c'est-à-dire un élément du dual algébrique ${F'}^*$.

#### Définition 1 {#int-vi-s1-def-1 .statement}

On appelle intégrale de $f$ par rapport à $\mu$ et on note $\int f d\mu$, ou $\int f(t) d\mu(t)$, l'élément de ${F'}^*$ défini par
$$
\langle z', \int f d\mu \rangle = \int \langle z', f \rangle d\mu
$$
pour tout $z' \in F'$.

Si $f$ est continue à support compact, elle est scalairement intégrable et la déf. 1 coïncide avec la définition de l'intégrale de $f$ donnée au chap. III, § 4, no 1. D'autre part, si $F$ est un espace de Banach et si $f$ est essentiellement intégrable (chap. V, § 2, no 2, déf. 2), alors $f$ est scalairement essentiellement intégrable et la déf. 1 coïncide avec la définition de l'intégrale de $f$ donnée au chap. V, § 2, no 2 (chap. V, § 2, no 2, prop. 6 et chap. IV, § 4, no 2, cor. 1 du th. 1).

#### Exemple {#int-vi-s1-n1-exa-1 .statement}

Soient X un espace localement compact, $t \to \lambda_t$ une application de T dans l'espace $\mathcal{M}(X)$ des mesures sur X. Dire que la famille $t \to \lambda_t$ est $\mu$-adéquate (chap. V, § 3, no 1, déf. 1) signifie qu'elle est formée de mesures positives et que l'application $t \to \lambda_t$ est scalairement essentiellement $\mu$-intégrable et $\mu$-mesurable pour la topologie $\sigma(\mathcal{M}(X), \mathcal{K}(X))$. Son intégrale par rapport à $\mu$ est la mesure qui a été notée $\int \lambda_t d\mu(t)$ au chap. V, § 3, no 1.

#### Remarque 1 {#int-vi-s1-n1-rem-1 .statement}

Si F est de dimension finie, toute application scalairement essentiellement intégrable de T dans F est essentiellement intégrable (chap. V, § 2, no 2). Par contre, dans le cas général, une fonction scalairement négligeable sur un espace T compact peut ne pas même être $\mu$-mesurable (exerc. 12).

#### Remarque 2 {#int-vi-s1-n1-rem-2 .statement}

Il est clair que l'intégrale de $f$ ne dépend que de la classe de $f$ modulo l'espace des applications de T dans F qui sont scalairement localement $\mu$-négligeables. On notera qu'une fonction g scalairement localement négligeable n'est pas nécessairement nulle localement presque partout (exerc. 12). Toutefois, il en est bien ainsi lorsqu'il existe dans $F'$ une suite $(z'_n)$ partout dense pour la topologie $\sigma(F', F)$ : en effet, si $H_n$ est l'ensemble localement négligeable des points $t \in T$ tels que $\langle g(t), z'_n \rangle \neq 0$, la réunion H des $H_n$ est localement négligeable, et pour tout $t \in H$, on a $\langle g(t), z'_n \rangle = 0$ pour tout $n$, d'où $g(t) = 0$.

Soit $u$ une application linéaire continue de F dans un espace localement convexe séparé G ; sa transposée $^t u$ est une application linéaire de $G'$ dans $F'$, et la transposée (algébrique) $' (t u)$ est une application linéaire de ${F'}^*$ dans ${G'}^*$ qui prolonge $u$, et que nous noterons encore $u$. Avec cette convention :

#### Proposition 1 {#int-vi-s1-prop-1 .statement}

Si $f$ est une application de T dans F, scalairement essentiellement $\mu$-intégrable, l'application $u \circ f$ est scalairement essentiellement $\mu$-intégrable et on a
$$
\int (u \circ f) d\mu = u \left( \int f d\mu \right).
$$

En effet, pour tout $z' \in G'$, on a $\langle z', u \circ f \rangle = \langle 'u(z'), f \rangle$, d’où la première assertion ; la seconde résulte de la formule

$$
z', \int (u \circ f) d\mu \rangle = \int \langle z', u \circ f \rangle d\mu = \langle 'u(z'), \int f d\mu \rangle = \left\langle z', u \left( \int f d\mu \right) \right\rangle.
$$

En particulier si $f$ est scalairement essentiellement $\mu$-intégrable elle reste scalairement essentiellement $\mu$-intégrable lorsqu’on remplace la topologie de $F$ par une topologie moins fine.

#### Proposition 2 {#int-vi-s1-prop-2 .statement}

*Soit $f$ une application scalairement essentiellement $\mu$-intégrable de $T$ dans $F$. Pour toute fonction numérique $g \geqslant 0$, $\mu$-mesurable et bornée, l’application $t \to g(t)f(t)$ (notée $gf$ ou $fg$) de $T$ dans $F$ est scalairement essentiellement $\mu$-intégrable, $f$ est scalairement essentiellement $(g.\mu)$-intégrable, et l’on a*

$$
\int f d(g.\mu) = \int fg d\mu.
$$

C’est une conséquence immédiate de la formule $\langle z', gf \rangle = g \langle z', f \rangle$ pour tout $z' \in F'$ et de la formule $\int h d(g.\mu) = \int hg d\mu$ pour toute fonction scalaire $h$ essentiellement $\mu$-intégrable (chap. V, § 5, no 3, th. 1).

Un grand nombre de propositions sur les fonctions numériques essentiellement intégrables se transposent mot pour mot en propositions sur les fonctions vectorielles scalairement essentiellement intégrables. Signalons parmi les plus importantes les conditions pour qu’une fonction soit essentiellement intégrable par rapport à une mesure définie par une densité (chap. V, § 5, no 3, th. 1), ou par rapport à l’image d’une mesure (chap. V, § 6; no 2, th. 1), ou par rapport à une mesure induite (chap. V, § 7, no 1, th. 1), ou par rapport à la somme d’une famille sommable de mesures positives (chap. V, § 3, no 5, prop. 5). Nous laissons ces transcriptions au lecteur.

Par contre, pour obtenir des énoncés correspondant aux théorèmes sur les intégrales « doubles » (chap. V, § 3, no 4, th. 1 et § 8, no 1, th. 1 (th. de Lebesgue-Fubini)), il est nécessaire d’en renforcer les hypothèses (cf. exerc. 1) ; en appliquant les théorèmes précités à chacune des fonctions $\langle z', f \rangle$, où $z' \in F'$, on obtient ainsi les deux propositions suivantes :

#### Proposition 3 {#int-vi-s1-prop-3 .statement}

*Soient X un espace localement compact, $t \to \lambda_t$ une famille $\mu$-adéquate (chap. V, § 3, no 1, déf. 1) de mesures positives sur X, et soit $\nu = \int \lambda_t d\mu(t)$. Soit f une application de X dans F ; on suppose que : 1° f est scalairement $\nu$-intégrable ; 2° il existe un ensemble $N \subset T$, localement $\mu$-négligeable, tel que, pour tout $t \notin N$, f soit scalairement $\lambda_t$-intégrable et que $\int f d\lambda_t \in F$. Alors la fonction $t \to \int f d\lambda_t$, définie pour $t \notin N$, est scalairement essentiellement $\mu$-intégrable, et on a*

$$
\int f(x) d\nu(x) = \int d\mu(t) \int f(x) d\lambda_t(x).
$$

#### Proposition 4 {#int-vi-s1-prop-4 .statement}

*Soient T, T' deux espaces localement compacts, $\mu$ (resp. $\mu'$) une mesure positive sur T (resp. T'), $\nu = \mu \otimes \mu'$ la mesure produit sur $X = T \times T'$. Soit f une application de X dans F. On suppose que : 1° f est scalairement $\nu$-intégrable ; 2° il existe un ensemble $N \subset T$, localement $\mu$-négligeable, tel que pour tout $t \notin N$, l’application $t' \to f(t, t')$ soit scalairement $\mu$-intégrable, et que $\int f(t, t') d\mu'(t') \in F$. Alors la fonction $t \to \int f(t, t') d\mu'(t')$, définie pour $t \notin N$, est scalairement essentiellement $\mu$-intégrable, et on a*

$$
\iint f(t, t') d\mu(t) d\mu'(t') = \int d\mu(t) \int f(t, t') d\mu'(t').
$$

### 2. Propriétés de l’intégrale d’une fonction scalairement essentiellement intégrable.

#### Proposition 5 {#int-vi-s1-prop-5 .statement}

*Soient $\mu$ une mesure positive bornée sur T, S un ensemble $\mu$-mesurable portant $\mu$ (chap. V, § 5, no 7), f une fonction scalairement $\mu$-intégrable (*) à valeurs dans F. Soit D l’enve-

(*) On rappelle que pour une mesure positive bornée $\mu$, les notions de fonction $\mu$-intégrable et de fonction essentiellement $\mu$-intégrable sont les mêmes (chap. V, § 2, no 1, cor. de la prop. 3).

loppe convexe fermée de $f(S)$ dans l’espace $F'$* muni de la topologie $\sigma(F', F')$. On a alors $\int f d\mu \in \mu(T)D$.

Comme D est l’intersection des demi-espaces fermés contenant $f(S)$ (*Esp. vect. top.*, chap. II, § 3, n° 3, cor. 1 de la prop. 4), il suffit de démontrer que la relation $\langle f(t), z' \rangle \leq a$ pour tout $t \in S$ (où $z' \in F', a \in \mathbf{R}$) entraîne $\langle z', \int f d\mu \rangle \leq a . \mu(T)$; mais comme $\int f d\mu = \int_S f d\mu$, cela résulte de la prop. 1 du chap. IV, § 4, n° 2.

#### Corollaire {#int-vi-s1-n2-cor-1 .statement}

Soient $\mu$ une mesure positive bornée sur T, S un ensemble $\mu$-mesurable portant $\mu$, f une application de T dans F, scalairement $\mu$-mesurable et telle que $f(S)$ soit contenu dans une partie convexe faiblement compacte A de F. Alors f est scalairement $\mu$-intégrable, et l’on a $\int f d\mu \in \mu(T)A \subset F$.

En effet, pour tout $z' \in F'$, $\langle z', f \rangle$ est $\mu$-mesurable et bornée dans S, donc intégrable, ce qui prouve que f est scalairement intégrable. En outre, comme A est compact dans $F_\tau$, il est fermé dans $F'$*, et l’enveloppe convexe fermée de $f(S)$ dans $F'$* est contenue dans A, d’où le corollaire.

#### Proposition 6 {#int-vi-s1-prop-6 .statement}

Soit f une fonction scalairement essentiellement $\mu$-intégrable à valeurs dans F, telle que $\int f d\mu \in F$. Pour toute semi-norme q sur F, semi-continue inférieurement dans F, on a

$$
q\left( \int f d\mu \right) \leq \int^{*} (q \circ f) d\mu.
$$

Soit D l’ensemble des $z \in F$ tels que $q(z) \leq 1$; D est fermé et convexe et contient 0, donc on a $D = D^{00}$ (*Esp. vect. top.*, chap. IV, § 2, n° 3, cor. 2 de la prop. 4). Il suffit donc de prouver que pour tout $z' \in D^0$ on a $|\langle z', \int f d\mu \rangle| \leq \int^{*} (q \circ f) d\mu$; mais cela résulte aussitôt de ce que l’on a, pour tout $t \in T$, $|\langle z', f(t) \rangle| \leq q(f(t))$.

On notera que la fonction numérique $q \circ f$ n’est pas nécessairement $\mu$-mesurable (exerc. 12).

#### Proposition 7 {#int-vi-s1-prop-7 .statement}

Soit $f$ une application de $T$ dans $F$, scalairement essentiellement $\mu$-intégrable et telle que, pour toute partie compacte $K$ de $T$, $f(K)$ soit contenue dans une partie convexe équilibrée faiblement compacte de $F$. Alors $\int f d\mu$ appartient au bidual $F''$ de $F$.

Pour toute partie compacte $K$ de $T$, on a
$$
\int f_{\varphi_K} d\mu = \int (f_{\varphi_K}) d(\varphi_K \cdot \mu);
$$
on peut appliquer à la mesure bornée $\varphi_K \cdot \mu$ et à la fonction $f_{\varphi_K}$ le cor. de la prop. 5, et on a par suite $\int f_{\varphi_K} d\mu \in F$. Pour tout $z' \in F'$, $\langle z', f \rangle$ est essentiellement $\mu$-intégrable, et par suite (chap. V, § 2, no 2, prop. 8) on a $\int \langle z', f \rangle d\mu = \lim_K \int \langle z', f \rangle_{\varphi_K} d\mu$, la limite étant prise suivant l’ensemble filtrant croissant des parties compactes de $T$. On en conclut que, suivant cet ensemble,
$$
\int f_{\varphi_K} d\mu \text{ converge vers } \int f d\mu \text{ pour la topologie } \sigma({F'}^*, F').
$$
Or, on a
$$
|\langle z', \int f_{\varphi_K} d\mu \rangle| = \left| \int \langle z', f \rangle_{\varphi_K} d\mu \right| \leq \int |\langle z', f \rangle| d\mu
$$
ce qui prouve que l’ensemble des éléments $\int f_{\varphi_K} d\mu$ est une partie bornée de $F_\sigma$, donc aussi de $F$ (*Esp. vect. top.*, chap. IV, § 2, no 4, th. 3). La prop. 7 est donc conséquence du lemme suivant :

#### Lemme 1 {#int-vi-s1-lem-1 .statement}

L’adhérence dans ${F'}^*$ (pour la topologie $\sigma({F'}^*, F')$) de toute partie bornée de $F$ est contenue dans le bidual $F''$.

En effet, une partie bornée de $F$ est contenue dans le polaire (dans $F''$) d’un voisinage de 0 dans le dual fort $F'$ de $F$, donc est relativement compacte dans $F''$ pour $\sigma(F'', F')$ (*Esp. vect. top.*, chap. IV, § 2, no 2, prop. 1 et 2); comme $\sigma(F'', F')$ est induite par $\sigma({F'}^*, F')$ le lemme est démontré.

#### Corollaire {#int-vi-s1-n2-cor-2 .statement}

Supposons F semi-réflexif, et soit f une application scalairement essentiellement µ-intégrable de T dans F telle que, pour toute partie compacte K de T, f(K) soit bornée. Alors $\int f d\mu$ appartient à F.

Toute partie bornée de F est en effet relativement faiblement compacte (Esp. vect. top., chap. IV, § 3, n° 3, th. 1), et on a $F = F''$.

#### Proposition 8 {#int-vi-s1-prop-8 .statement}

Soient µ une mesure positive bornée sur T, S un ensemble µ-mesurable portant µ, f une application µ-mesurable de T dans F, telle que f(S) soit contenu dans une partie convexe équilibrée bornée et complète B de F. Alors f est scalairement µ-intégrable et on a $\int f d\mu \in \mu(T)B \subset F$.

Comme S est µ-intégrable, il existe une partition de S formée d’un ensemble µ-négligeable N et d’une suite (K_n) de parties compactes telles que la restriction de f à chacun des K_n soit continue (chap. IV, § 5, n° 1); f(K_n) est par suite une partie compacte de F. L’enveloppe convexe équilibrée fermée B_n de f(K_n) est alors précompacte (Esp. vect. top., chap. II, § 4, n° 1, prop. 2) et est contenue dans la partie complète B de F, donc elle est compacte, et a fortiori faiblement compacte. Par suite (cor. de la prop. 5), f_{φ_{K_n}} est scalairement µ-intégrable, et on a $z_n = \int f_{φ_{K_n}} d\mu \in \mu(K_n)B_n \subset \mu(K_n)B$. Pour toute semi-norme continue p sur F, on a par suite $p(z_n) \leq \mu(K_n) \sup_{x \in B} p(x)$; comme B est bornée et que la série de terme général $\mu(K_n)$ est convergente et a pour somme $\mu(T)$, on voit que la suite de terme général $s_n = z_1 + z_2 + \cdots + z_n$ est une suite de Cauchy dans la partie complète $\mu(T)B$ de F. Cette suite converge donc vers un élément s de $\mu(T)B$; comme on peut supposer f(t) = 0 dans T - S, le th. de Lebesgue appliqué à chacune des fonctions $\langle z', f \rangle$ ($z' \in F'$) prouve que $s = \int f d\mu$.

### 3. Intégrales d’opérateurs.

Soient G et H deux espaces localement convexes séparés sur $\mathbf{R}$, et supposons maintenant que F soit l’espace $\mathcal{L}(G; H)$ des applications linéaires continues de G dans H, muni de la topologie de la convergence simple. Le dual F' de F est alors l'espace G ⊗ H' (Esp. vect. top., chap. IV, § 2, no 9, cor. de la prop. 11), et dire qu'une application U de T dans F est scalairement essentiellement μ-intégrable signifie que, pour tout a ∈ G et tout b ∈ H', la fonction numérique $t \to \langle U(t), a \otimes b' \rangle = \langle U(t).a, b' \rangle$ est essentiellement μ-intégrable.

#### Proposition 9 {#int-vi-s1-prop-9 .statement}

Soit U une application scalairement essentiellement μ-intégrable de T dans F = $\mathcal{L}_s(G; H)$. Pour que l'on ait $\int Ud\mu \in F$, il faut et il suffit que les deux conditions suivantes soient vérifiées :

a) Pour tout x ∈ G, on a $\int (U(t).x)d\mu(t) \in H$.

b) Pour toute partie équicontinue B' de H', l'ensemble des formes linéaires $u_{y'} : x \to \int \langle U(t).x, y' \rangle d\mu(t)$, où y' parcourt B', est équicontinu.

Les conditions a) et b) sont nécessaires. En effet, pour tout x ∈ G, l'application $\tilde{x} : V \to V.x$ de $\mathcal{L}_s(G; H)$ dans H étant linéaire et continue, on voit (no 1, prop. 1) que $\tilde{x} \circ U : t \to U(t).x$ est scalairement essentiellement μ-intégrable et que l'on a

(1)
$$
S.x = \int (U(t).x)d\mu(t)
$$
en posant $S = \int Ud\mu \in \mathcal{L}_s(G; H)$. Cela prouve a). De plus, (1) s'écrit aussi

(2)
$$
\langle S.x, y' \rangle = \int \langle U(t).x, y' \rangle d\mu(t) = \langle x, u_{y'} \rangle,
$$
autrement dit on a 'S.y' = $u_{y'}$. Comme S est continue, 'S transforme toute partie équicontinue de H' en une partie équicontinue de G', d'où b).

Inversement, supposons a) et b) vérifiées. En vertu de a), la formule (1) définit une application linéaire S de G dans H, et pour tout y' ∈ H', cette application vérifie (2) (no 1, prop. 1); mais alors la condition b) exprime que S est continue (Esp. vect. top., chap. IV, § 4, n° 1, prop. 1 et 2, et § 2, n° 2, prop. 1), donc $S \in \mathcal{L}_s(G; H)$. Enfin, la formule (2) prouve que $S = \int U d\mu$.

#### Corollaire {#int-vi-s1-n3-cor-1 .statement}

La condition b) de la prop. 9 est vérifiée dans chacun des deux cas suivants :

1° La mesure $\mu$ est bornée, et si S est son support, $U(S)$ est une partie équicontinue de $\mathcal{L}(G; H)$.

2° La condition a) de la prop. 9 est vérifiée, l’espace G est tonnelé, et pour toute partie compacte K de T, $U(K)$ est une partie bornée de $\mathcal{L}_s(G; H)$.

Plaçons-nous d’abord dans le cas 1°. On peut se borner au cas où $S = T$ (chap. V, § 7, n° 1, th. 1). Alors, pour toute partie équicontinue B′ de H′, il existe une partie équicontinue, convexe, équilibrée et faiblement fermée $A' \subset G'$ telle que $^tU(t) . y' \in A'$ pour tout $y' \in B'$ et tout $t \in T$ (Esp. vect. top., chap. IV, § 4, n° 1, prop. 2). Comme $U$ est scalairement $\mu$-intégrable, l’application $t \to ^tU(t) . y'$ de T dans le dual $G'$ de G muni de $\sigma(G', G)$, est scalairement $\mu$-intégrable, et on peut écrire

$$
u_{y'} = \int (^tU(t) . y') d\mu(t).
$$

Comme $A'$ est convexe et compacte pour $\sigma(G', G)$, le cor. de la prop. 5 du n° 2 montre que, pour tout $y' \in B'$, on a $u_{y'} \in \mu(T)A'$, ce qui prouve notre assertion.

Plaçons-nous maintenant dans le cas 2°. Pour tout $y' \in H'$ et toute partie compacte K de T, posons

$$
u_{K, y'} = \int \varphi_K(t) (^tU(t) . y') d\mu(t),
$$

élément du dual algébrique $G^*$ de G. Comme G est tonnelé, toute partie bornée de $\mathcal{L}_s(G; H)$ est équicontinue (Esp. vect. top., chap. III, § 3, n° 6, th. 2); la première partie du raisonnement, appliquée à la fonction $\varphi_K U$ et à la mesure bornée $\varphi_K . \mu$, montre que l’on a $u_{K, y'} \in G'$. En outre, pour la topologie $\sigma(G^*, G)$, on a $u_{y'} = \lim_K u_{K, y'}$, la limite étant prise suivant l’ensemble filtrant croissant des parties compactes de T (chap. V, § 2, no 2, prop. 8). Pour vérifier la condition b) de la prop. 9, il suffit, d’après la prop. 9, de prouver que l’application linéaire S de G dans H définie par (1) est continue ; en outre, G est tonnelé, et il suffit donc de prouver que S est continue quand on munit G et H de leurs topologies affaiblies (Esp. vect. top., chap. IV, § 4, no 2, cor. de la prop. 7); finalement, en vertu de (2), on est ramené à montrer que pour tout y' ∈ H', on a u_{y'} ∈ G'. Comme u_{y'} est adhérent pour σ(G*, G) à l’ensemble M' des u_{K, y'}, où K parcourt l’ensemble des parties compactes de T, il suffit de prouver que M' est équicontinu ; et comme G est tonnelé, il revient au même de dire que pour tout x ∈ G, l’ensemble des ⟨x, u_{K, y'}⟩ est borné (Esp. vect. top., chap. III, § 3, no 6, th. 2). Mais cela résulte aussitôt des relations

$$
|\langle x, u_{K, y'} \rangle| = \left| \int \varphi_K(t) \langle U(t) \cdot x, y' \rangle d\mu(t) \right| \leq \int |\langle U(t) \cdot x, y' \rangle| d\mu(t).
$$

#### Proposition 10 {#int-vi-s1-prop-10 .statement}

*Soit U une application de T dans F = $\mathcal{L}_s(G; H)$. Dans chacun des trois cas suivants, U est scalairement essentiellement $\mu$-intégrable, et on a $\int U d\mu \in \mathcal{L}_s(G; H)$:*

a) H est quasi-complet, $\mu$ est bornée, et si S est son support, U est $\mu$-mesurable et U(S) est équicontinu.

b) H est semi-réflexif, $\mu$ est bornée, et si S est son support, U est scalairement $\mu$-mesurable et U(S) est équicontinu.

c) H est semi-réflexif, G est tonnelé, U est scalairement essentiellement $\mu$-intégrable, et pour toute partie compacte K de T, U(K) est borné.

Le fait que U est scalairement essentiellement intégrable est évident dans les trois cas ; en vertu de la prop. 9 et de son corollaire il suffit de vérifier dans chacun des cas la condition a) de la prop. 9. Or, cette condition résulte de la prop. 8 du no 2 dans le premier cas, du cor. de la prop. 7 du no 2 dans les deux autres cas.

### 4. La propriété (GDF).

Nous allons dans ce no considérer des espaces localement convexes F possédant la propriété suivante (dite « du graphe dénombrablement fermé ») :

Bourbaki XXV.

(GDF) Si u est une application linéaire de F dans un espace de Banach B telle que, dans l’espace produit F × B, toute limite de toute suite convergente de points du graphe Γ de u appartienne encore à Γ, alors u est continue.

Tout espace de Fréchet possède la propriété (GDF) (Esp. vect. top., chap. I, § 3, no 3, cor. 5 du th. 1). Nous verrons dans l’Appendice d’autres exemples d’espaces possédant la propriété (GDF).

#### Proposition 11 {#int-vi-s1-prop-11 .statement}

Tout espace localement convexe séparé F possédant la propriété (GDF) est tonnelé.

Soient V un tonneau dans F, q sa jauge, qui est une semi-norme sur F ; soit H l’espace séparé associé à l’espace F muni de la topologie définie par cette seule semi-norme. Le complété $\widehat{H}$ de H est un espace de Banach ; soit $\pi$ l’application canonique de F dans $\widehat{H}$ ; nous allons montrer que $\pi$ est continue (pour la topologie initiale de F) ; cela établira la proposition, car V, image réciproque par $\pi$ de la boule unité de $\widehat{H}$, sera alors un voisinage de 0 dans F. Pour établir la continuité de $\pi$, il suffira, en vertu de (GDF), de montrer que le graphe de $\pi$ est fermé dans $F \times \widehat{H}$ ; en d’autres termes, nous devons voir que si $\mathcal{F}$ est un filtre sur F, convergent vers $x \in F$, et si son image $\pi(\mathcal{F})$ converge vers $y \in \widehat{H}$, on a $y = \pi(x)$. Or tout élément $x'$ du polaire $V^0$ de V dans $F'$ se prolonge d’une seule manière en une forme linéaire continue sur $\widehat{H}$ (notée encore $x'$), et l’ensemble de ces formes est la boule unité du dual de $\widehat{H}$ ; il suffit donc de montrer que $\langle y, x' \rangle = \langle \pi(x), x' \rangle$ pour tout $x' \in V^0$. Mais cela résulte des relations

$$
\langle y, x' \rangle = \lim_{\mathcal{F}} \langle \pi(z), x' \rangle = \lim_{\mathcal{F}} \langle z, x' \rangle = \langle x, x' \rangle = \langle \pi(x), x' \rangle.
$$

#### Théorème 1 (Gelfand-Dunford) {#int-vi-s1-thm-1 .statement}

Soient F un espace localement convexe séparé possédant la propriété (GDF), $F'_s$ son dual faible. Pour toute application $f$ de T dans $F'_s$, scalairement essentiellement $\mu$-intégrable, l’intégrale $\int f d\mu$ appartient à $F'$.

Rappelons que le dual de $F'_s$ est F (Esp. vect. top., chap. IV, § 1, no 2, prop. 1). Pour tout $z \in F$, la fonction numérique $\langle z, f \rangle$ est donc essentiellement $\mu$-intégrable ; soit $\theta(z)$ sa classe dans $L^1(\mu)$.

Pour montrer que $\int f d\mu \in F'$, il faut établir que la forme linéaire $z \mapsto \langle z, \int f d\mu \rangle$ est continue dans $F$; en fait, nous allons démontrer le résultat plus fort suivant :

#### Lemme 2 {#int-vi-s1-lem-2 .statement}

*Soit $f$ une application de $T$ dans $F_s'$, telle que, pour tout $z \in F$, la fonction numérique $\langle z, f \rangle$ appartienne à $\mathcal{L}^p(\mu)$ ($1 \leq p \leq +\infty$); soit $\theta(z)$ la classe de cette fonction dans $L^p(\mu)$. Alors $z \mapsto \theta(z)$ est une application linéaire continue de $F$ dans $L^p(\mu)$.

En vertu de la propriété (GDF), il suffit de montrer que pour toute suite $(z_n)$ d’éléments de $F$ convergente vers $z$ et telle que $(\theta(z_n))$ converge vers $u \in L^p(\mu)$, on a $u = \theta(z)$. Or, en remplaçant éventuellement la suite $(z_n)$ par une suite extraite, on peut supposer que la suite des fonctions $\langle z_n, f \rangle$ converge localement presque partout vers une fonction $h \in \mathcal{L}^p(\mu)$, de classe $u$ dans $L^p(\mu)$ (chap. IV, § 3, no 4, th. 3 et chap. V, § 2, no 2, prop. 6). Comme par hypothèse, pour tout $t \in T$, la suite $(\langle z_n, f(t) \rangle)$ converge vers $\langle z, f(t) \rangle$, on a $h(t) = \langle z, f(t) \rangle$ localement presque partout, et par suite $u = \theta(z)$.

#### Corollaire 1 {#int-vi-s1-lem-2-cor-1 .statement}

*Soient $G_i$ ($1 \leq i \leq n$) $n$ espaces localement convexes séparés possédant la propriété (GDF), et soit $F$ l’espace des formes multilinéaires séparément continues dans $\prod_{i=1}^n G_i$, muni de la topologie de la convergence simple. Pour toute application $f$ de $T$ dans $F$, scalairement essentiellement $\mu$-intégrable, on a $\int f d\mu \in F$.

L’espace $F$ est en dualité avec le produit tensoriel $\bigotimes_{i=1}^n G_i$, et la topologie de la convergence simple sur $F$ n’est autre que la topologie $\sigma(F, \bigotimes_{i=1}^n G_i)$. Le dual algébrique $F'$ est donc l’espace de toutes les formes multilinéaires sur $\prod_{i=1}^n G_i$. Soit $z = (z_1, \ldots, z_n)$ un élément de $\prod_{i=1}^n G_i$; pour toute forme multilinéaire $u \in F'$, l’application $x \to u(z_1, \ldots, z_{i-1}, x, z_{i+1}, \ldots, z_n)$ est une forme linéaire sur $G_i$ que nous noterons $\lambda_i(z)(u)$; on obtient ainsi une application linéaire $\lambda_i(z)$ de $F'{}^*$ dans le dual algébrique $G_i^*$ de $G_i$, continue pour les topologies $\sigma(F'{}^*, \bigotimes_{i=1}^n G_i)$ et $\sigma(G_i^*, G_i)$. Dire que $u \in F$ signifie que pour tout indice $i$ et tout $z \in \prod_{i=1}^n G_i$, on a $\lambda_i(z)(u) \in G_i'$.
Or, d’après la prop. 1 du n° 1, l’application $\lambda_i(z) \circ f$ est une application scalairement essentiellement $\mu$-intégrable de $T$ dans $G_i'$ muni de la topologie $\sigma(G_i', G_i)$, et on a $\int (\lambda_i(z) \circ f)d\mu = \lambda_i(z)\left( \int f d\mu \right)$.
D’après le th. 1, on a $\int (\lambda_i(z) \circ f)d\mu \in G_i'$ pour $1 \leq i \leq n$, donc $\int f d\mu \in F$.

#### Corollaire 2 {#int-vi-s1-lem-2-cor-2 .statement}

Soient $G$ un espace localement convexe séparé possédant la propriété (GDF), $H$ un espace semi-réflexif dont le dual fort $H_b'$ possède la propriété (GDF) (cf. App., n° 2, prop. 3). Soit $F$ l’espace $\mathcal{L}_s(G; H)$; pour toute application $U$ de $T$ dans $F$, scalairement essentiellement $\mu$-intégrable, l’intégrale $\int Ud\mu$ appartient à $F$.

Comme $G$ est tonnelé (prop. 11), on a $\mathcal{L}(G; H) = \mathcal{L}(G_\sigma; H_\sigma)$ (*Esp. vect. top.*, chap. IV, § 4, n° 2, cor. de la prop. 7); en outre, on peut remplacer $F = \mathcal{L}_s(G; H)$ par l’espace $\mathcal{L}_s(G_\sigma; H_\sigma)$, les deux espaces ayant même dual $G \otimes H'$ (*Esp. vect. top.*, chap. IV, § 2, n° 9, cor. de la prop. 11, et § 1, n° 2, prop. 1). Si pour tout $u \in \mathcal{L}(G; H) = \mathcal{L}(G_\sigma; H_\sigma)$, on pose $\tilde{u}(x, y') = \langle u(x), y' \rangle$ (pour $x \in G$, $y' \in H'$), l’application linéaire $u \to \tilde{u}$ est une bijection de $F$ sur l’espace $F_1$ des formes bilinéaires séparément continues sur $G_\sigma \times H'_\sigma$, où $H'_\sigma$ désigne le dual $H'$ muni de la topologie faible $\sigma(H', H)$ (*App.*, n° 1); en outre cette application est un isomorphisme de $\mathcal{L}_s(G_\sigma; H_\sigma)$ sur $F_1$ muni de la topologie de la convergence simple (*loc. cit.*). Mais comme par hypothèse $H$ est le dual de $H_b'$, $F_1$ est aussi l’espace des formes bilinéaires séparément continues sur $G \times H_b'$. Le cor. 2 résulte donc du cor. 1.

On notera que le cor. 2 s’applique en particulier lorsque G est un espace de Banach et H un espace de Banach réflexif.

### 5. Applications mesurables et applications scalairement mesurables.

Si une application f de T dans un espace localement convexe séparé F est scalairement μ-mesurable, il n’en résulte pas en général que f soit μ-mesurable (exerc. 12). Cependant :

#### Proposition 12 {#int-vi-s1-prop-12 .statement}

Si F est un espace localement convexe métrisable de type dénombrable, toute application f de T dans F, scalairement μ-mesurable, est aussi μ-mesurable.

En effet, F peut être considéré comme un sous-espace d’un produit dénombrable $\prod_{n} E_n$ d’espaces de Banach (Esp. vect. top., chap. II, § 5, no 5, prop. 7), et on peut supposer que $pr_n(F)$ est dense dans $E_n$, qui est donc de type dénombrable. Pour tout n, l’application $pr_n \circ f$ est scalairement μ-mesurable, donc μ-mesurable (chap. IV, § 5, no 5, prop. 10), et par suite f est μ-mesurable (chap. IV, § 5, no 3, th. 1).

#### Proposition 13 {#int-vi-s1-prop-13 .statement}

Soit F un espace localement convexe, limite inductive d’une suite d’espaces localement convexes métrisables $F_n$ de type dénombrable, F étant réunion des $F_n$. Soit $F'$ le dual de F muni de la topologie $\sigma(F', F)$. Toute application f de T dans $F'$, scalairement μ-mesurable, est aussi μ-mesurable.

Supposons d’abord que F soit métrisable et de type dénombrable, et soit D un ensemble dénombrable dense dans F. Soit $(V_n)$ une suite fondamentale décroissante de voisinages ouverts convexes équilibrés de 0 dans F ; les ensembles polaires $V_n^0$ sont équicontinu et leur réunion est $F'$ tout entier. Soit $T_n = \overline{f}(V_n^0)$; la suite $(T_n)$ est croissante et $T = \bigcup_n T_n$; montrons que chacun des $T_n$ est μ-mesurable. En effet, $D \cap V_n$ est dense dans $V_n$; pour tout $y \in D \cap V_n$, soit $S_y$ l’ensemble des $t \in T$ tels que $|\langle y, f(t) \rangle| \leq 1$; l’hypothèse entraîne que chacun des $S_y$ est mesurable, et $T_n$ est l’intersection de la famille dénombrable des $S_y$ ($y \in D \cap V_n$). Cela étant, pour toute partie compacte K de T et tout $\varepsilon > 0$, il existe un entier n tel que $\mu(K - (K \cap T_n)) \leq \frac{\varepsilon}{4}$, puis une partie compacte $K_1$ de $K \cap T_n$ telle que $\mu((K \cap T_n) - K_1) \leq \frac{\varepsilon}{4}$; enfin, il existe une partie compacte $K_2$ de $K_1$ telle que $\mu(K_1 - K_2) \leq \frac{\varepsilon}{2}$, et que les restrictions à $K_2$ de toutes les fonctions $\langle y, f \rangle$, où $y \in D$, soient continues (chap. IV, § 5, no 1, prop. 2). Comme l’ensemble $f(K_2) \subset f(T_n) \subset V_n^0$ est équicontinu, la topologie induite par $\sigma(F', F)$ sur $f(K_2)$ est identique à la topologie de la convergence simple dans D ($Top. gén.$, chap. X, 2e éd., § 2, no 4, th. 1); par suite, la restriction de $f$ à $K_2$ est continue, d’où notre assertion dans ce premier cas.

Passons au cas général. Si $z'$ est une forme linéaire continue sur $F$, sa restriction $z'_n$ à $F_n$ est continue; comme $F = \bigcup_n F_n$, le dual $F'$ de $F$ peut être identifié (algébriquement) à un sous-espace vectoriel du produit $\prod_n F'_n$, et on a $pr_n z' = z'_n$. En outre, toute partie finie de $F$ étant contenue dans l’un des $F_n$, la topologie $\sigma(F', F)$ n’est autre que la topologie induite par la topologie produit des topologies $\sigma(F'_n, F_n)$. Cela étant, si $f$ est scalairement $\mu$-mesurable, $pr_n \circ f$ est scalairement $\mu$-mesurable, puisque pour tout $t \in T$, $pr_n(f(t))$ est la restriction de $f(t)$ à $F_n$. La première partie de la démonstration montre que $pr_n \circ f$ est $\mu$-mesurable pour tout $n$, et il en est donc de même de $f$ (chap. IV, § 5, no 3, th. 1).

### 6. Applications : I. Extension d’une fonction continue à un espace de mesures.

Soient T un espace localement compact, F un espace localement convexe séparé et quasi-complet, $f$ une application continue de T dans F ; si $\mu$ est une mesure positive sur T, à support compact S, $f(S)$ est compact ; l’enveloppe fermée convexe de $f(S)$ est alors compacte ($Esp. vect. top.$, chap. III, § 2, no 5), donc $f$ est scalairement $\mu$-intégrable et on a $\int f d\mu \in F$ (no 2, cor.de la prop. 5). Si maintenant $\lambda$ est une mesure réelle quelconque à support compact, $\lambda^+$ et $\lambda^-$ sont des mesures positives à support compact ; si on pose $\int f d\lambda = \int f d\lambda^+ - \int f d\lambda^-$, on vérifie aussitôt (en utilisant la relation $(\lambda + \mu)^+ + \lambda^- + \mu^- = \lambda^+ + \mu^+ + (\lambda + \mu)^-$) que $\lambda \to \int f d\lambda$ est une application linéaire de l’espace $C'(T)$ des mesures à support compact sur T, dans l’espace localement convexe F.

Notons maintenant que l’espace $C'(T)$ peut être identifié au dual de l’espace $C(T)$ des fonctions continues numériques sur T (d’où sa notation), lorsqu’on munit $C(T)$ de la topologie de la convergence compacte (ce que nous supposerons toujours dans ce no et le suivant) : en effet on sait d’une part (chap. III, § 3, no 4, prop. 11) que les mesures sur T qui peuvent être prolongées en des formes linéaires continues dans $C(T)$ sont les mesures à support compact, et inversement, la restriction à $K(T)$ d’une forme linéaire continue sur $C(T)$ est une mesure (la topologie de $K(T)$ étant plus fine que celle induite par la topologie de $C(T)$).

#### Proposition 14 {#int-vi-s1-prop-14 .statement}

*Soient T un espace localement compact, F un espace localement convexe séparé et quasi-complet, f une application continue de T dans F. Si on munit l’espace $C'(T)$ des mesures sur T à support compact, de la topologie de la convergence uniforme dans les parties compactes de $C(T)$, l’application $\lambda \to \int f d\lambda$ est l’unique application linéaire continue $\tilde{f}$ de $C'(T)$ dans F telle que $\tilde{f}(\varepsilon_t) = f(t)$ pour tout $t \in T$.

Pour établir l’unicité du prolongement, il suffit de voir que les mesures ponctuelles $\varepsilon_t$ forment un ensemble total dans $C'(T)$ : comme le dual de $C'(T)$ est $C(T)$ (*Esp. vect. top.*, chap. IV, § 2, no 3, th. 2), il suffit de remarquer que toute fonction $g \in C(T)$ orthogonale à toutes les mesures $\varepsilon_t$ est égale à 0 par définition (*Esp. vect. top.*, chap. IV, § 2, no 3, *Remarque*).

Montrons maintenant que $\lambda \to \int f d\lambda$ est continue. Soit V un voisinage convexe fermé équilibré de 0 dans F ; il suffit de prouver qu’il existe une partie relativement compacte L de $C(T)$ telle que les relations $\lambda \in L^0$ et $z' \in V^0$ entraînent $\left| \left( \int f d\lambda, z' \right) \right| \leq 1,$ ou encore $\left| \int \langle \mathbf{f}, \mathbf{z}' \rangle d\lambda \right| \leq 1$. Pour cela, on va montrer que lorsque $\mathbf{z}'$ parcourt $V^0$, l’ensemble $L$ des fonctions numériques $\langle \mathbf{f}, \mathbf{z}' \rangle$ est relativement compact dans $C(T)$. Comme $V^0$ est borné pour $\sigma(F', F)$, la borne supérieure des nombres $|\langle \mathbf{f}(t), \mathbf{z}' \rangle|$ pour $t \in T$ fixe, $\mathbf{z}'$ parcourant $V^0$, est finie ; en vertu du th. d’Ascoli (*Top. gén.*, chap. X, 2e éd., § 2, no 5, cor. 2 du th. 2), il suffit donc de montrer que l’ensemble des $\langle \mathbf{f}, \mathbf{z}' \rangle$ ($\mathbf{z}' \in V^0$) est *équicontinu*. Mais, pour tout $t_0 \in T$ et tout $\delta > 0$, il existe par hypothèse un voisinage $W$ de $t_0$ dans $T$ tel que $\mathbf{f}(t) - \mathbf{f}(t_0) \in \delta V$ pour tout $t \in W$; on en conclut $|\langle \mathbf{f}(t), \mathbf{z}' \rangle - \langle \mathbf{f}(t_0), \mathbf{z}' \rangle| \leq \delta$ pour tout $t \in W$ et tout $\mathbf{z}' \in V^0$, ce qui achève la démonstration.

#### Remarque 1 {#int-vi-s1-n6-rem-1 .statement}

L’application $t \to \varepsilon_t$ est un *homéomorphisme* de $T$ dans l’espace $C'(T)$; en effet, si $L$ est une partie compacte de $C(T)$, et $t_0 \in T$, il existe (chap. X, 2e éd., § 2, no 5, cor. 2 du th. 2), un voisinage $W$ de $t_0$ tel que $|g(t) - g(t_0)| \leq 1$ pour tout $t \in V$ et toute fonction $g \in L$, donc $\varepsilon_t - \varepsilon_{t_0} \in L^0$ pour $t \in V$, ce qui démontre la continuité de $t \to \varepsilon_t$; on sait par ailleurs que l’application réciproque est déjà continue pour la topologie vague (chap. III, § 2, no 7, prop. 6), donc *a fortiori* pour la topologie de la convergence uniforme dans les parties compactes de $C(T)$. Si alors on identifie $T$ et son image dans $C'(T)$ par $t \to \varepsilon_t$, on peut dire que $\lambda \to \int \mathbf{f} d\lambda$ est l’unique *prolongement continu* de $\mathbf{f}$ en une application *linéaire*.

#### Remarque 2 {#int-vi-s1-n6-rem-2 .statement}

On notera que dans la démonstration de la continuité de $\lambda \to \int \mathbf{f} d\lambda$, on n’a pas utilisé le fait que $F$ est quasi-complet. La conclusion de la prop. 14 est donc encore valable sans cette hypothèse, lorsqu’on sait par ailleurs que $\int \mathbf{f} d\mu \in F$ pour toute mesure positive $\mu$ à support compact.

Supposons maintenant que $\mathbf{f}(T)$ soit une partie *bornée* de $F$. Alors, pour toute mesure positive *bornée* $\mu$ sur $T$, $\mathbf{f}$ est scalairement $\mu$-intégrable et on a $\int \mathbf{f} d\mu \in F$ (no 2, prop. 8). Si $\lambda$ est une mesure réelle bornée quelconque sur $T$, $\lambda^+$ et $\lambda^-$ sont bornées, et on voit aussitôt que $\lambda \to \int \mathbf{f} d\lambda$ définie comme ci-dessus est une application linéaire de l’espace $\mathcal{M}^1(T)$ des mesures bornées sur T, dans l’espace localement convexe F, qui prolonge évidemment l’application $\lambda \to \int f d\lambda$ de $C'(T)$ dans F.

#### Proposition 15 {#int-vi-s1-prop-15 .statement}

*Soient T un espace localement compact, F un espace localement convexe séparé et quasi-complet, f une application continue de T dans F telle que f(T) soit borné. Si on munit l’espace $\mathcal{M}^1(T)$ de sa topologie d’espace de Banach, l’application linéaire $\lambda \to \int f d\lambda$ de $\mathcal{M}^1(T)$ dans F est continue.*

En effet, pour tout voisinage convexe équilibré fermé V de 0 dans F, il existe $\rho > 0$ tel que $f(T) \subset \rho V$; l’enveloppe convexe fermée B de f(T) est donc contenue dans $\rho V$, et elle est complète par hypothèse. Si alors $\| \lambda \| \leq 1/\rho$ il résulte du no 2, prop. 8, et de la relation $\| \lambda \| = \lambda^+(T) + \lambda^-(T)$, que l’on a $\int f d\lambda \in B/\rho \subset V$.

### 7. *Applications : II. Extension à un espace de mesures d’une fonction continue à valeurs dans un espace d’opérateurs.*

Soient G un espace localement convexe séparé, H un espace localement convexe séparé et quasi-complet, et désignons par F l’espace $\mathcal{L}(G; H)$ des applications linéaires continues de G dans H, muni de la topologie de la *convergence compacte*. L’espace F n’est pas nécessairement quasi-complet, et si $t \to U(t)$ est une application continue de T dans F et $\mu$ une mesure positive sur T, à support compact, on n’a pas nécessairement $\int U d\mu \in F$ (exerc. 27). Toutefois, si pour toute partie compacte K de T, $U(K)$ est *équicontinu*, son enveloppe convexe équilibrée dans F est aussi équicontinue (*Esp. vect. top.*, chap. III, § 3, no 5), et comme H est quasi-complet, l’adhérence de cette enveloppe convexe sera une partie complète de F (*Esp. vect. top.*, chap. III, § 3, no 7, th. 4); on aura donc bien alors $\int U d\mu \in F$ (no 2, prop. 8).

La condition supplémentaire imposée à $U$ peut s’exprimer autrement :

#### Lemme 3 {#int-vi-s1-lem-3 .statement}

*Soient G, H deux espaces localement convexes, U une application d’un espace localement compact T dans $\mathcal{L}(G; H)$. Les conditions suivantes sont équivalentes :*

a) *L’application* $(t, x) \to U(t) . x$ *de* $T \times G$ *dans* $H$ *est continue.*

b) *Pour toute partie compacte K de T, U(K) est équicontinu, et il existe un ensemble total D \subset G tel que pour tout* $x \in D$, *l’application* $t \to U(t) . x$ *soit continue dans* $T$.

*De plus, lorsque U vérifie ces conditions, U est une application continue de T dans* $\mathcal{L}(G; H)$ *muni de la topologie de la convergence compacte.*

Pour voir que a) entraîne b), observons que pour tout voisinage V de 0 dans H et tout $t \in K$, il existe par hypothèse un voisinage $L_t$ de $t$ dans T et un voisinage $W_t$ de 0 dans G tels que les relations $t' \in L_t$ et $x \in W_t$ entraînent $U(t') . x \in V$. Il suffit de recouvrir K par un nombre fini de voisinages $L_{t_i}$ et de prendre $W = \bigcap_i W_{t_i}$ pour avoir $U(t) . x \in V$ lorsque $t \in K$ et $x \in W$, ce qui démontre l’équicontinuité de $U(K)$.

Inversement, supposons vérifié b); il suffit de montrer que pour toute partie compacte K de T, l’application $(t, x) \to U(t) . x$ est continue dans $K \times G$. Soit $M = U(K)$; comme M est équicontinu, il en résulte que sur M, la topologie de la convergence simple dans G est identique à la topologie de la convergence simple dans D (*Top. gén.*, chap. X, 2e éd., § 2, no 4, th. 1); l’hypothèse b) entraîne donc que $t \to U(t)$ est une application continue de K dans $\mathcal{L}(G; H)$ lorsqu’on munit $\mathcal{L}(G; H)$ de la topologie de la convergence simple. D’autre part, $(A, x) \to A . x$ est une application continue de $M \times G$ dans H lorsqu’on munit M de la topologie de la convergence simple (*Top. gén.*, chap. X, 2e éd., § 2, no 2, cor. 4 de la prop. 1). Comme l’application $(t, x) \to U(t) . x$ se factorise en $(t, x) \to (U(t), x) \to U(t) . x$, on en conclut qu’elle est continue.

Enfin, la dernière assertion du lemme résulte de ce que, sur M, la topologie de la convergence compacte est identique à celle de la convergence simple (*Top. gén.*, chap. X, 2e éd., § 2, no 4, th. 1).

Supposons donc que $U$ vérifie les conditions du lemme 3 ; alors (si $H$ est quasi-complet), on définit comme au n° 6 une application linéaire $\lambda \to \int Ud\lambda$ de $C'(T)$ dans $F = \mathcal{L}(G, H)$. Nous poserons $U(\lambda) = \int Ud\lambda$.

#### Proposition 16 {#int-vi-s1-prop-16 .statement}

*Soient G, H deux espaces localement convexes séparés, H étant supposé quasi-complet. Soit U une application de T dans $\mathcal{L}(G; H)$ telle que $(t, x) \to U(t).x$ soit une application continue de $T \times G$ dans H. Alors l’application bilinéaire $(\lambda, x) \to U(\lambda).x$ de $C'(T) \times G$ dans H est hypocontinue relativement aux parties équicontinues de $C'(T)$ et aux parties compactes de G (ce qui entraîne que l’application linéaire $\lambda \to U(\lambda)$ de $C'(T)$ dans F est continue).

La continuité de $\lambda \to U(\lambda)$ comme application de $C'(T)$ dans F résulte du lemme 3 et de la *Remarque 2* suivant la prop. 14 du n° 6. Reste donc à prouver que pour tout voisinage convexe, équilibré et fermé V de 0 dans H et toute partie équicontinue N de $C'(T)$, il existe un voisinage W de 0 dans G tel que les relations $x \in W, \lambda \in N$ entraînent $U(\lambda).x \in V$. On peut supposer que $N = S^0$, où S est un voisinage de 0 dans $C(T)$, et par suite on peut supposer que S est l’ensemble des fonctions $g \in C(T)$ telles que $|g(t)| \leq 1$ dans une partie compacte K de T. Il suffit de montrer que $|\langle U(\lambda).x, x'\rangle| \leq 1$ pour $x \in W, x' \in V^0$ et $\lambda \in S^0$. Or, comme $U(K)$ est équicontinu, il existe un voisinage W de 0 dans G tel que les relations $t \in K, x \in W$ entraînent $U(t).x \in V$; les relations $x \in W, x' \in V^0$ entraînent donc que la fonction $t \to \langle U(t).x, x'\rangle$ appartient à S, et par suite, que
$$
|\langle U(\lambda).x, x'\rangle| = \left| \int \langle U(t).x, x'\rangle d\lambda(t) \right| \leq 1, \text{ par définition de } S^0.
$$

Supposons maintenant que $U$ soit une application continue de T dans F et en outre que $U(T)$ soit équicontinu. Alors, le même raisonnement que ci-dessus montre (puisque H est quasi-complet) que pour toute mesure positive *bornée* $\mu$ sur T, on a $\int Ud\mu \in F$. On définit donc comme plus haut une application linéaire

λ → ∫ U dλ = U(λ) de $\mathcal{M}^1(T)$ dans F prolongeant l’application analogue de $C'(T)$ dans F. En outre, pour tout voisinage convexe équilibré fermé V de 0 dans H, il existe par hypothèse un voisinage W de 0 dans G tel que pour tout $x \in W$ et tout $t \in T$, on ait $U(t).x \in V$, et par suite (V étant faiblement fermé)
$$
\int (U(t).x)d\lambda(t) \in \| \lambda \| . V \ (\text{n}^\circ 2, \text{prop. } 5). \text{ Autrement dit :}
$$

#### Proposition 17 {#int-vi-s1-prop-17 .statement}

*Soient G, H, deux espaces localement convexes séparés, H étant supposé quasi-complet. Soit U une application de T dans $\mathcal{L}(G; H)$ telle que $(t, x) \to U(t).x$ soit continue dans $T \times G$, et que $U(T)$ soit équicontinu. Alors si on munit $\mathcal{M}^1(T)$ de sa topologie d’espace de Banach, l’application bilinéaire $(\lambda, x) \to U(\lambda).x$ de $\mathcal{M}^1(T) \times G$ dans H est continue (ce qui entraîne en particulier que l’application linéaire $\lambda \to U(\lambda)$ de $\mathcal{M}^1(T)$ dans $\mathcal{L}(G; H)$ est continue lorsqu’on munit $\mathcal{L}(G, H)$ de la topologie de la convergence bornée).

#### Proposition 18 {#int-vi-s1-prop-18 .statement}

*Soient $G_1, G_2, H_1, H_2$ quatre espaces localement convexes séparés, $H_1$ et $H_2$ étant supposés quasi-complets. Soient $A : G_1 \to G_2$ et $B : H_1 \to H_2$ deux applications linéaires continues. Soient $U_1 : T \to \mathcal{L}(G_1; H_1)$, $U_2 : T \to \mathcal{L}(G_2; H_2)$ deux applications vérifiant les conditions de la prop. 16 (resp. 17), et supposons que pour tout $t \in T$ on ait $B \circ U_1(t) = U_2(t) \circ A$. Alors, pour toute mesure à support compact (resp. bornée) $\lambda$ sur T, on a $B \circ U_1(\lambda) = U_2(\lambda) \circ A$.

En effet, pour tout $x \in G$, on a (n° 1, prop. 1)

$$
(B \circ U_1(\lambda)).x = \int ((B \circ U_1(t)).x)d\lambda(t)
$$
$$
= \int ((U_2(t) \circ A).x)d\lambda(t) = U_2(\lambda).(A.x).
$$

#### Remarque 1 {#int-vi-s1-n7-rem-1 .statement}

Supposons que G et H soient des espaces de Banach, et soit U une application de T dans $\mathcal{L}(G; H)$ telle que $(t, x) \to U(t).x$ soit continue dans $T \times G$. Notons que cela entraîne que la fonction finie $t \to \| U(t) \|$ est bornée dans toute partie compacte de T et semi-continue inférieurement dans T, étant l’enveloppe supérieure des fonctions continues $t \to | U(t).x |$ lorsque $x$ parcourt la boule $|\mathbf{x}| \leq 1$ dans G. Posons $h(t) = \| U(t) \|$. Alors, pour toute mesure positive $\mu$ sur T telle que $h$ soit $\mu$-intégrable, on a encore $\int Ud\mu \in \mathcal{L}(G; H)$. En effet, la mesure $\nu = h.\mu$ est bornée par hypothèse ; il existe donc une partition de T formée d’un ensemble $\nu$-négligeable N et d’une suite $(K_n)$ de parties compactes. Le raisonnement fait au début de ce n°, appliqué à la mesure $\varphi_{K_n}.\mu$ montre que $A_n = \int \varphi_{K_n} Ud\mu \in F = \mathcal{L}(G; H)$, et en outre (n° 2, prop. 6) $\|A_n\| \leq \int \varphi_{K_n} \|U\| d\mu \leq \nu(K_n)$. La série de terme général $A_n$ est donc absolument convergente dans l’espace de Banach $\mathcal{L}(G; H)$, et il est immédiat que sa somme est $\int Ud\mu$ et que l’on a $\left\| \int Ud\mu \right\| \leq \int \|U\| d\mu$.

#### Remarque 2 {#int-vi-s1-n7-rem-2 .statement}

Supposons que $G = H$ soit quasi-complet, et que $U$ vérifie les hypothèses de la prop. 16. Soient M une partie partout dense de l’espace $C'(T)$, pour la topologie faible $\sigma(C'(T), C(T))$, et soit X un sous-espace vectoriel fermé de H tel que $U(\lambda)(X) \subset X$ pour toute mesure $\lambda \in M$. Alors on a aussi $U(t)(X) \subset X$ pour tout $t \in T$ : en effet pour tout $x \in X$ et tout $x' \in H'$ orthogonal à X, on a par hypothèse $\langle U(\lambda).x, x' \rangle = 0$ pour tout $\lambda \in M$, ce qui s’écrit $\int \langle U(t).x, x' \rangle d\lambda(t) = 0$. La fonction continue $t \to \langle U(t).x, x' \rangle$, étant orthogonale à M, est donc 0, ce qui donne $\langle U(t).x, x' \rangle = 0$ pour tout $x' \in X^0$, d’où $U(t).x \in X$ pour tout $t \in T$ et tout $x \in X$, et cela démontre notre assertion.

## EXERCICES {#int-vi-s1-exercises}

See the [exercises for § 1](exercises/s1/).
