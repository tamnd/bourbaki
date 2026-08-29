---
book: alg
book_title: Algebra
chapter: V
chapter_title: Corps commutatifs
section: 12
section_title: CORPS FINIS $^1$
lang: fr
source: alg-iv-vii-fr
book_pages: A V.89-A V.93, A V.157-A V.160
pdf_pages: 0193-0197, 0261-0264
extraction: ocr
subsections:
    - "no": 1
      title: Structure des corps finis
      page: 89
      pdf_page: 193
    - "no": 2
      title: Extensions algébriques d’un corps fini
      page: 90
      pdf_page: 194
    - "no": 3
      title: Groupe de Galois de la clôture algébrique d’un corps fini
      page: 91
      pdf_page: 195
    - "no": 4
      title: Polynômes cyclotomiques sur un corps fini
      page: 93
      pdf_page: 197
statements: 11
exercises: 14
content_sha256: 811704fc92f6ace4ac5f0f716dc47e75d74688582d6de6259f094ceb6c50a183
---

## § 12. CORPS FINIS $^1$

### 1. Structure des corps finis

#### Proposition 1 {#alg-v-s12-prop-1 .statement}

*Soit K un corps fini à q éléments.*

a) *La caractéristique de K est un nombre premier p, et il existe un entier f $\geqslant 1$ tel que $q = p^f$.*

b) *Le groupe additif de K est somme directe de f groupes cycliques d’ordre p.*

c) *Le groupe multiplicatif de K est cyclique d’ordre $q - 1$.*

Comme $\mathbf{Z}$ est infini et K fini, l’unique homomorphisme d’anneaux $\varphi : \mathbf{Z} \to K$ n’est pas injectif, et son noyau est un idéal premier de $\mathbf{Z}$, non réduit à 0. Par suite, la caractéristique de K est un nombre premier, et K est une algèbre sur le corps $\mathbf{F}_p$ à $p$ éléments (V, p. 3). Soit $f$ le degré de K sur $\mathbf{F}_p$. Si $f$ était infini, K contiendrait pour tout entier $n \geqslant 0$ un sous-espace de dimension $n$ sur $\mathbf{F}_p$, d’où $q \geqslant p^n$, ce qui est absurde. Par suite $f$ est fini. Le groupe additif de K est donc isomorphe à $(\mathbf{F}_p)^f$, d’où les assertions a) et b).

L’assertion c) résulte du lemme 1 (V, p. 75).

#### Proposition 2 {#alg-v-s12-prop-2 .statement}

*Soit K un corps fini à q éléments. Le corps K est un corps de décomposition du polynôme $X^q - X$ de $\mathbf{F}_p[X]$ et est l’ensemble des racines de ce polynôme.*

Pour tout $x \neq 0$ dans K, on a $x^{q-1} = 1$ puisque $K^*$ est un groupe fini d’ordre $q - 1$ (I, p. 49). On en déduit $x^q = x$ pour tout $x$ dans K. Le polynôme $X^q - X$ de $\mathbf{F}_p[X]$ est de degré $q$ et il a $q$ racines dans K, d’où

$$
X^q - X = \prod_{\xi \in K} (X - \xi)
$$

La prop. 2 résulte aussitôt de là.

#### Corollaire {#alg-v-s12-n1-cor-1 .statement}

*Deux corps finis de même cardinal sont isomorphes.*

Soit K’ un corps fini à $q$ éléments ; sa caractéristique est un nombre premier $p'$

$^1$ Conformément aux conventions de ce chapitre, on ne s’intéresse ici qu’aux corps finis commutatifs. En fait, tout corps fini est commutatif comme nous le verrons au chapitre VIII (cf. V, p. 160, exercice 14).

divisant $q = p^f$, d’où $p' = p$. Par suite, $K'$ est un corps de décomposition du polynôme $X^q - X$ de $F_p[X]$ (prop. 2); $K$ et $K'$ sont donc isomorphes (V, p. 21, cor.).

Lorsque $K = F_p$, la formule (1) se réduit à la relation

$$
X^p - X \equiv \prod_{i=0}^{p-1} (X - i) \mod p \mathbf{Z}[X]
$$

dans l’anneau de polynômes $\mathbf{Z}[X]$.

La formule (2) peut aussi s’écrire

$$
X^{p-1} - 1 \equiv \prod_{i=1}^{p-1} (X - i) \mod p \mathbf{Z}[X].
$$

En particulier, pour $X = 0$, on obtient (« formule de Wilson »)

$$
(p-1)! \equiv -1 \mod p.
$$

### 2. Extensions algébriques d’un corps fini

#### Proposition 3 {#alg-v-s12-prop-3 .statement}

Soient $K$ un corps fini à $q$ éléments, $\Omega$ une extension algébriquement close de $K$, et $m$ un entier $\geqslant 1$.

a) Il existe une unique sous-extension $K_m$ de $\Omega$ qui soit de degré $m$ sur $K$.

b) Le corps $K_m$ a $q^m$ éléments et c’est l’ensemble des points fixes de l’automorphisme $x \mapsto x^{q^m}$ de $\Omega$.

c) On a $K_m = K(\zeta)$ pour tout générateur $\zeta$ du groupe cyclique $K_m^*$.

Soient $p$ la caractéristique de $K$ et $f$ le degré de $K$ sur $F_p$. On a $q^m = p^{f m}$, et l’application $x \mapsto x^{q^m}$ est donc un automorphisme du corps parfait $\Omega$ (V, p. 6, prop. 4). Par suite, l’ensemble $K_m$ des racines du polynôme $X^{q^m} - X$ de $K[X]$ est un sous-corps de $\Omega$. Comme la dérivée de $X^{q^m} - X$ est égale à $-1$, toutes les racines de ce polynôme sont simples (IV, p. 16, prop. 7), et $K_m$ a donc $q^m$ éléments. On en déduit $[K_m : K] = m$.

Soit maintenant $L$ une sous-extension de $\Omega$, de degré $m$ sur $K$. Comme espace vectoriel sur $K$, $L$ est isomorphe à $K^m$, donc a $q^m$ éléments. On a donc $x^{q^m} = x$ pour tout $x \in L$ (prop. 2), d’où $L \subset K_m$. Comme on a $[L : K] = [K_m : K] = m$, on a finalement $L = K_m$.

On a donc prouvé les assertions a) et b), et l’assertion c) est triviale.

#### Corollaire {#alg-v-s12-n2-cor-1 .statement}

Soient $K$ un corps fini et $\Omega$ une extension algébriquement close de $K$. La fermeture algébrique $\overline{K}$ de $K$ dans $\Omega$ se compose de $0$ et des racines de l’unité et c’est une clôture algébrique de $K$.

On sait que $\overline{K}$ est une clôture algébrique de $K$ (V, p. 22, exemple 2), et il est clair que toute racine de l’unité dans $\Omega$ appartient à $\overline{K}$. Par ailleurs, soit $x \neq 0$ dans $\overline{K}$, de degré $m$ sur $K$. Si le corps $K$ a $q$ éléments, le corps $K(x)$ en a $q^m$, d’où $x^{q^m - 1} = 1$, et $x$ est une racine de l’unité dans $\Omega$.

Soit $p$ un nombre premier, et soit $\mathbf{F}_p = \mathbf{Z}/p\mathbf{Z}$ le corps à $p$ éléments. Choisissons une clôture algébrique $\Omega$ de $\mathbf{F}_p$, dont l’existence résulte du théorème de Steinitz (V, p. 22, th. 2). Soient $f$ un entier positif et $q = q^f$. D’après la prop. 3, il existe un unique sous-corps de $\Omega$, qui soit de degré $f$ sur $\mathbf{F}_p$; on le notera $\mathbf{F}_q(\Omega)$, ou par abus de notations $\mathbf{F}_q$. C’est l’unique sous-extension de $\Omega$, qui soit de degré $f$ sur $\mathbf{F}_p$. C’est l’unique sous-corps de $\Omega$ de cardinal $q$, et tout corps de cardinal $q$ est isomorphe (non canoniquement) à $\mathbf{F}_q$ (cor. de la prop. 2). On notera que $\mathbf{F}_q$ se compose des $x$ dans $\Omega$ tels que $x^q = x$, et que l’on a $\mathbf{F}_q \subset \mathbf{F}_{q'}$ si et seulement si $q'$ est une puissance de $q$.

#### Proposition 4 {#alg-v-s12-prop-4 .statement}

*Soient $\mathbf{K}$ un corps fini à $q$ éléments et $\mathbf{K}_m$ une extension de degré fini $m$ de $\mathbf{K}$.*

a) *Le corps $\mathbf{K}_m$ est une extension galoisienne de $\mathbf{K}$, dont le groupe de Galois est le groupe cyclique d’ordre $m$ engendré par l’automorphisme $\sigma_q : x \mapsto x^q$.*

b) *Pour tout $x \in \mathbf{K}_m$, la norme de $x$ par rapport à $\mathbf{K}$ est égale à $x^{(q^m - 1)/(q - 1)}$.*

c) *Tout élément de $\mathbf{K}$ est la trace (resp. la norme) d’un élément de $\mathbf{K}_m$.*

Soit $\Gamma$ le groupe cyclique d’automorphismes de $\mathbf{K}_m$ engendré par $\sigma_q$. Le corps des invariants de $\Gamma$ se compose des éléments $x$ de $\mathbf{K}_m$ tels que $x^q = x$, donc est égal à $\mathbf{K}$. Par suite, $\mathbf{K}_m$ est une extension galoisienne de $\mathbf{K}$, de groupe de Galois $\Gamma$, et ce dernier est d’ordre égal à $[\mathbf{K}_m : \mathbf{K}] = m$ (V, p. 64, th. 3). D’où a).

On a $\Gamma = \{ 1, \sigma_q, \sigma_q^2, \ldots, \sigma_q^{m-1} \}$; la norme d’un élément $x$ de $\mathbf{K}_m$ par rapport à $\mathbf{K}$ est donc $\mathrm{N}(x) = \prod_{i=0}^{m-1} \sigma_q^i(x) = x^{1 + q + \cdots + q^{m-1}}$ et l’on a $1 + q + \cdots + q^{m-1} = \frac{q^m - 1}{q - 1}$.

Ceci prouve b). Soit $\zeta$ un générateur du groupe cyclique $\mathbf{K}_m^*$; l’image de la norme $\mathrm{N} : \mathbf{K}_m^* \to \mathbf{K}^*$ est le sous-groupe cyclique de $\mathbf{K}^*$ engendré par l’élément $\xi = \mathrm{N}(\zeta) = \zeta^{(q^m - 1)/(q - 1)}$; comme $\zeta$ est d’ordre $q^m - 1$, $\xi$ est d’ordre $q - 1$, donc engendre $\mathbf{K}^*$. Ceci prouve que tout élément non nul de $\mathbf{K}$ est norme d’un élément non nul de $\mathbf{K}_m$; de plus, on a $0 = \mathrm{N}(0)$.

Enfin, comme $\mathbf{K}_m$ est une extension algébrique et séparable de $\mathbf{K}$, la trace est une forme linéaire non nulle sur l’espace vectoriel $\mathbf{K}_m$ sur $\mathbf{K}$ (V, p. 48, cor.) ; tout élément de $\mathbf{K}$ est donc trace d’un élément de $\mathbf{K}_m$.

### 3. Groupe de Galois de la clôture algébrique d’un corps fini

Soit $S \neq \{ 1 \}$ un ensemble d’entiers $\geqslant 1$, stable par multiplication ; ordonnons-le par la relation « $m$ divise $n$ ». Lorsque $m$ divise $n$, on a $m\mathbf{Z} \supset n\mathbf{Z}$, d’où un homomorphisme canonique $\pi_{m,n}$ de l’anneau $\mathbf{Z}/n\mathbf{Z}$ sur l’anneau $\mathbf{Z}/m\mathbf{Z}$. Notons $\mathrm{A}(S)$ la limite projective du système projectif d’anneaux $(\mathbf{Z}/m\mathbf{Z}, \pi_{m,n})$ indexé par $S$. On munit chaque ensemble fini $\mathbf{Z}/m\mathbf{Z}$ de la topologie discrète, et $\mathrm{A}(S)$ de la topologie induite par celle du produit $\prod_{n \in S} (\mathbf{Z}/n\mathbf{Z})$. Alors $\mathrm{A}(S)$ est un anneau topologique compact (TG, I, p. 64, prop. 8). On voit immédiatement que l’unique homomorphisme d’anneaux $\varphi$ de $\mathbf{Z}$ dans $\mathrm{A}(S)$ est injectif et d’image dense ; *on identifiera $\mathbf{Z}$ à son image par $\varphi$ dans $\mathrm{A}(S)$*.

Pour la topologie induite sur $\mathbf{Z}$ par celle de $A(S)$, les ensembles $m\mathbf{Z}$ (pour $m \in S$) forment une base de voisinages de 0.

Lorsque $S = \mathbf{N}^*$, $A(S)$ est noté $\hat{\mathbf{Z}}$. Lorsque $S$ est formé des puissances d’un nombre premier $l$, $A(S)$ est noté $\mathbf{Z}_l$ et appelé « anneau des entiers $l$-adiques ». On a donc

$$
\hat{\mathbf{Z}} = \lim_{\leftarrow m \geq 1} \mathbf{Z}/m\mathbf{Z} , \quad \mathbf{Z}_l = \lim_{\leftarrow n \geq 0} \mathbf{Z}/l^n\mathbf{Z} .
$$

Lorsque $S$ et $T$ sont deux ensembles d’entiers stables par multiplication, tels que $S \supset T$, on a une projection naturelle $A(S) \to A(T)$ qui est un homomorphisme continu d’anneaux topologiques. En particulier, on a pour chaque nombre premier $l$ un homomorphisme continu $\hat{\mathbf{Z}} \to \mathbf{Z}_l$. On en déduit un homomorphisme continu

$$
\hat{\mathbf{Z}} \to \prod_l \mathbf{Z}_l
$$

(produit étendu à tous les nombres premiers); c’est un isomorphisme d’anneaux topologiques, comme il résulte par passage à la limite projective de I, p. 107, prop. 11.

Soit $K$ un corps fini à $q$ éléments, et soit $\overline{K}$ une clôture algébrique de $K$. Pour tout entier $m \geq 1$, on note $K_m$ l’unique sous-corps de $\overline{K}$ qui est de degré $m$ sur $K$ (prop. 3). On a $\overline{K} = \bigcup_{m \geq 1} K_m$. On note par ailleurs $\sigma_q$ l’automorphisme $x \mapsto x^q$ du corps parfait $\overline{K}$; on l’appelle l’automorphisme de Frobenius de $\overline{K}$ (relativement à $K$).

#### Proposition 5 {#alg-v-s12-prop-5 .statement}

Il existe un unique isomorphisme de groupes topologiques $\pi_K : \hat{\mathbf{Z}} \to \mathrm{Gal}(\overline{K}/K)$ tel que $\pi_K(1) = \sigma_q$.

Soit $\Gamma$ le sous-groupe de $\mathrm{Gal}(\overline{K}/K)$ engendré par $\sigma_q$. Pour tout entier $m > 0$, on a $\sigma_q^m(x) = x^{q^m}$ pour tout $x \in \overline{K}$, et par suite l’ensemble des points fixes de $\sigma_q^m$ est égal à $K_m$. Comme on a $K_m \neq \overline{K}$, on a $\sigma_q^m \neq 1$. Il existe par suite un isomorphisme $\pi_0$ de $\mathbf{Z}$ sur $\Gamma$ qui applique 1 sur $\sigma_q$.

Le corps des invariants de $\Gamma$ se compose des $x \in \overline{K}$ tels que $x^q = x$, donc est égal à $K$. Par suite (V, p. 65, lemme 2), le groupe $\Gamma$ est dense dans $\mathrm{Gal}(\overline{K}/K)$. Comme toute sous-extension de $\overline{K}$ de degré fini sur $K$ est l’un des corps $K_m$, un système fondamental de voisinages de 1 dans $\mathrm{Gal}(\overline{K}/K)$ est formé des sous-groupes $\mathrm{Gal}(\overline{K}/K_m)$. Il est clair que $\Gamma \cap \mathrm{Gal}(\overline{K}/K_m)$ est le groupe cyclique engendré par $\sigma_q^m$, donc est égal à $\pi_0(m\mathbf{Z})$.

D’après les remarques faites sur la topologie de $\hat{\mathbf{Z}}$, l’isomorphisme $\pi_0 : \mathbf{Z} \to \Gamma$ se prolonge de manière unique en un isomorphisme de groupes topologiques $\pi_K : \hat{\mathbf{Z}} \to \mathrm{Gal}(\overline{K}/K)$.

Soit $m \geq 1$ un entier ; il est immédiat que l’automorphisme de Frobenius de $\overline{K}$ relativement à $K_m$ est $\sigma_q^m$. On en déduit la relation

$$
\pi_{K_m}(a) = \pi_K(ma) \quad \text{pour} \quad a \in \hat{\mathbf{Z}} .
$$

### 4. Polynômes cyclotomiques sur un corps fini

Soient K un corps fini à q éléments, $n \geqslant 1$ un entier non divisible par la caractéristique $p$ de K et $R_n$ une extension cyclotomique de niveau $n$ de K (V, p. 77). On sait que le groupe $\mu_n(R_n) = \mu_n$ des racines $n$-ièmes de l’unité dans $R_n$ est cyclique d’ordre $n$, qu’on a $R_n = K(\mu_n)$ et qu’il existe un homomorphisme injectif

$$
\varphi_n : \mathrm{Gal}(R_n/K) \to (\mathbf{Z}/n\mathbf{Z})^*
$$

tel que $\sigma(\zeta) = \zeta^j$ pour $\sigma \in \mathrm{Gal}(R_n/K)$, $\zeta \in \mu_n$ et $j \in \varphi_n(\sigma)$.

Par ailleurs, si $f$ est le degré de $R_n$ sur K, le groupe de Galois de $R_n$ sur K est cyclique d’ordre $f$, engendré par l’automorphisme $\sigma_q : x \mapsto x^q$ (V, p. 91, prop. 4). On a aussitôt :

#### Proposition 6 {#alg-v-s12-prop-6 .statement}

*L’image par $\varphi_n$ de l’automorphisme de Frobenius $\sigma_q$ est la classe de $q$ mod. $n$*.

Par conséquent, compte tenu de la prop. 6 de V, p. 80 :

#### Corollaire {#alg-v-s12-n4-cor-1 .statement}

*Le degré de $R_n$ sur K est le plus petit entier $f \geqslant 1$ tel que $q^f \equiv 1$ mod. $n$. Pour que le polynôme cyclotomique $\Phi_n$ soit irréductible sur K, il faut et il suffit que le groupe $(\mathbf{Z}/n\mathbf{Z})^*$ soit engendré par la classe de $q$ modulo $n$*.

#### Exemple 1 {#alg-v-s12-n4-exa-1 .statement}

Le polynôme $\Phi_3(X) = X^2 + X + 1$ est irréductible dans $F_q[X]$ si et seulement si l’on a $q \equiv 2$ mod. 3. De même, $\Phi_4(X) = X^2 + 1$ est irréductible dans $F_q[X]$ si et seulement si $q \equiv 3$ mod. 4, et pour $\Phi_5(X) = X^4 + X^3 + X^2 + X + 1$, la condition d’irréductibilité s’écrit $q \equiv 2, 3$ mod. 5.

#### Exemple 2 {#alg-v-s12-n4-exa-2 .statement}

On a $5^2 \equiv 1$ mod. 12, donc la classe de 5 modulo 12 n’engendre pas $(\mathbf{Z}/12\mathbf{Z})^*$. Le polynôme $\Phi_{12}(X) = X^4 - X^2 + 1$ n’est donc pas irréductible dans $F_5[X]$; on a en fait

$$
\Phi_5(X) = (X^2 + 2X - 1)(X^2 - 2X - 1)
$$

dans $F_5[X]$.

## EXERCICES {#alg-v-s12-exercises}

See the [exercises for § 12](exercises/s12/).
