---
book: ta
book_title: Topologie algébrique
chapter: III
chapter_title: HOMOTOPIE ET GROUPOÏDE DE POINCARÉ
section: 4
section_title: Homotopie et revêtements
lang: fr
source: ta-i-iv-fr
book_pages: TA III.300-TA III.307, TA III.334
pdf_pages: 0316-0323, 0350-0350
extraction: native
subsections:
    - "no": 1
      title: Homotopie et revêtements
      page: 300
      pdf_page: 316
    - "no": 2
      title: Relèvement des chemins
      page: 301
      pdf_page: 317
    - "no": 3
      title: Opérations du groupoïde de Poincaré dans les revêtements
      page: 303
      pdf_page: 319
    - "no": 4
      title: Cas des revêtements associés à un revêtement principal
      page: 305
      pdf_page: 321
statements: 16
exercises: 1
content_sha256: a750048c9fd54f1eedac19d785b692367add6fdf7ee793afa41d547643b4161e
---

## § 4. HOMOTOPIE ET REVÊTEMENTS

### 1. Homotopie et revêtements

#### Proposition 1 {#ta-iii-s4-prop-1 .statement tag=01Z5}

Soit B un espace topologique et soit E un revêtement de B. Soit $B'$ un espace topologique et soient $f_0$ et $f_1$ des applications continues de $B'$ dans B. Si les applications $f_0$ et $f_1$ sont homotopes, les revêtements $f_0^*(E)$ et $f_1^*(E)$ de $B'$ sont isomorphes.

Soit $\sigma : B'\times \mathbf{I}\rightarrow B$ une homotopie reliant $f_0$ à $f_1$. Notons $i_0$ et $i_1$ les applications $x\mapsto (x,0)$ et $x\mapsto (x,1)$ de $B'$ dans $B'\times \mathbf{I}$. Si $t\in  \{0,1\}$, on a $f_t=\sigma \circ i_t$ et les revêtements $f_t^*(E)$ et $i^*_t(\sigma^*(E))$ de $B'$ sont donc isomorphes (I, p. 15). Comme l’espace topologique $\mathbf{I}$ est localement connexe et simplement connexe (I, p. 127, corollaire), les revêtements $i^*_0(\sigma^*(E))$ et $i^*_1(\sigma^*(E))$ de $B'$ sont isomorphes (I, p. 130, cor. 1 de la prop. 8).

#### Corollaire {#ta-iii-s4-n1-cor-1 .statement tag=01Z6}

Un espace topologique homéotope à un espace topologique simplement connexe est simplement connexe.

Soient B et $B'$ des espaces topologiques, soit $f: B\rightarrow B'$ une homéo-topie et soit $g: B'\rightarrow B$ une application continue, réciproque à homotopie près de $f$. Soit E un revêtement de B. Comme $g\circ f$ est homotope à l’application identique de B, le revêtement B est isomorphe au revêtement $f^*(g^*(E))$ (prop. 1). Si l’espace $B'$ est simplement connexe, le revêtement $g^*(E)$ est trivialisable. Par suite, le revêtement E est trivialisable. Cela prouve que l’espace B est simplement connexe.

#### Remarque {#ta-iii-s4-n1-rem-1 .statement tag=01Z7}

Soit G un groupe topologique discret. Avec les notations de la proposition, supposons que E soit un revêtement principal de groupe G. Les revêtements $f_0^*(E)$ et $f_1^*(E)$ sont alors des revêtements principaux isomorphes (I, p. 131, remarque).

#### Proposition 2 (Relèvement des homotopies) {#ta-iii-s4-prop-2 .statement tag=01Z8}

Soit B un espace topologique et soit E un revêtement de B. Soit $B'$ un espace topologique et soient $f_0$ et $f_1$ des applications continues de $B'$ dans B. Soit $\sigma : B'\times$ $\mathbf{I}\rightarrow B$ une homotopie reliant $f_0$ à $f_1$. Soit $g_0: B'\rightarrow E$ un relèvement continu de $f_0$ à E. Il existe une unique application continue $\widetilde{\sigma}: B'\times \mathbf{I}\rightarrow$ E relevant $\sigma$ qui est une homotopie d’origine $g_0$. Son terme $g_1: B'\rightarrow E$ est un relèvement continu de $f_1$ à E.

Cela résulte du corollaire 3 de la prop. 8 de I, p. 130, appliqué à l’espace topologique simplement connexe et localement connexe $\mathbf{I}$.

### 2. Relèvement des chemins

#### Proposition 3 {#ta-iii-s4-prop-3 .statement tag=01Z9}

Soit B un espace topologique et soit $p: E\rightarrow B$ un revêtement. Notons $\widetilde{p}:\mathscr{C}_c(\mathbf{I}; E)\rightarrow \mathscr{C}_c(\mathbf{I}; B)$ l’application $c\mapsto p\circ c$. Notons $o_E:\mathscr{C}_c(\mathbf{I}; E)\rightarrow E$ ( resp. $o_B:\mathscr{C}_c(\mathbf{I}; B)\rightarrow B$) l’application définie par $c\mapsto c(0)$. Alors, le diagramme

$\mathscr{C}_c(\mathbf{I}; E)^{o_E}$ E

$\widetilde{p}p$

$\mathscr{C}_c(\mathbf{I}; B)^{o_B}$ B est un carré cartésien.

L’espace topologique $\mathbf{I}$ est localement connexe, localement compact et simplement connexe. La proposition résulte ainsi de la prop. 9 de I, p. 131, appliquée avec $T =\mathbf{I}$ et $t= 0$.

#### Corollaire 1 {#ta-iii-s4-prop-3-cor-1 .statement tag=01ZA}

L’application $\widetilde{p}:\mathscr{C}_c(\mathbf{I}; E)\rightarrow \mathscr{C}_c(\mathbf{I}; B)$ est un revêtement.

Cela résulte de I, p. 71, cor. 2 de la prop. 1.

#### Corollaire 2 (Relèvement des chemins) {#ta-iii-s4-prop-3-cor-2 .statement tag=01ZB}

Soit $p: E\rightarrow B$ un revêtement, soit $x$ un point de E et $a=p(x)$. L’application $c\mapsto p\circ c$ est un homéomorphisme de l’espace $\Lambda_x(E)$ des chemins dans E d’origine $x$ sur l’espace $\Lambda_a(B)$ des chemins dans B d’origine $a$.

Avec les notations de la proposition 3, on a $\Lambda_a(B) =o^{-1}_B(a)$ et $\Lambda_x(E) =\overset{-1}{o_{E}}(x)$. Le corollaire résulte alors de I, p. 10, cor. de la prop. 4.

On dira qu’une application continue $p: E\rightarrow B$ vérifie la propriété de relèvement des chemins si, pour tout chemin $c:\mathbf{I}\rightarrow$ B et tout point $x$ de E relevant $c(0)$, il existe un chemin $c'$ dans E d’origine $x$ qui relève $c$. Un tel chemin est alors unique si $p$ est étale et séparée (I, p. 34, cor. 1 de la prop. 11). Soient E un revêtement et $p$ sa projection ; l’application $p$ est étale, séparée et possède la propriété de relèvement des chemins (corollaire 2). Pour une réciproque partielle, cf. III, p. 315, corollaire.

#### Proposition 4 {#ta-iii-s4-prop-4 .statement tag=01ZC}

Soit $p: E\rightarrow B$ une application étale et séparée qui vérifie la propriété de relèvement des chemins. Soient $a$ et $b$ des points de B et soit $x$ un point de E tel que $p(x) =a$. Soient $c_0$ et $c_1$ deux chemins strictement homotopes reliant $a$ à $b$ dans B. Les chemins d’origine $x$ dans E qui relèvent respectivement $c_0$ et $c_1$ ont même terme et sont strictement homotopes.

Soit $\sigma :\mathbf{I}\times \mathbf{I}\rightarrow$ B une homotopie stricte reliant $c_0$ à $c_1$. Pour $s\in \mathbf{I}$, soit $c'_s$ l’unique chemin d’origine $x$ dans E qui relève le chemin $t\mapsto \sigma (t, s)$. Pour $(t, s)\in \mathbf{I}\times \mathbf{I}$, posons $\sigma '(t, s) =c'_s(t)$ ; on a $p\circ \sigma '=\sigma$. L’application $\sigma '$ est constante sur $\{0\} \times \mathbf{I}$; par construction, elle est continue sur $\mathbf{I}\times  \{s\}$ pour tout $s\in \mathbf{I}$. Elle est donc continue, d’après I, p. 37, cor. 1 du th. 1. En particulier, l’application de $\mathbf{I}$ dans $E_b$ donnée par $s\mapsto \sigma '(1, s)$ est un relèvement continu du chemin constant d’image $b$; elle est donc constante. Cela prouve que l’application $\sigma '$ est une homotopie stricte reliant $c'_0$ à $c'_1$.

#### Corollaire 1 {#ta-iii-s4-prop-4-cor-1 .statement tag=01ZD}

Soit B un espace topologique et soit E un revêtement de B ; notons $p$ sa projection. Pour tout couple $(x, y)$ de points de E, l’application $\varpi_{x,y}(p):\varpi_{x,y}(E)\rightarrow \varpi_{p(x),p(y)}(B)$ est injective. En particulier, pour tout point $x$ de E, l’homomorphisme $\pi_1(p, x):\pi_1(E, x)\rightarrow \pi_1(B, p(x))$ est injectif.

#### Corollaire 2 {#ta-iii-s4-prop-4-cor-2 .statement tag=01ZE}

Soit B un espace topologique et soit E un revêtement de B ; notons $p$ sa projection. Soit $x$ un point de E, posons $b=p(x)$. Pour que la classe dans $\pi_1(B, b)$ d’un lacet $c$ de B en $a$ appartienne au sous-groupe image de l’homomorphisme $\pi_1(p, x)$, il faut et il suffit que le chemin $c'$ d’origine $x$ relevant $c$ soit un lacet de E en $x$.

La condition est évidemment suffisante. Inversement, soit $c'_1$ un lacet de E en $x$. Posons $c_1=p\circ c'_1$ et supposons que les lacets $c$ et $c_1$ soient strictement homotopes. D’après la prop. 4, le chemin $c'$ a même terme que le chemin $c'_1$. C’est donc un lacet en $x$.

#### Corollaire 3 {#ta-iii-s4-prop-4-cor-3 .statement tag=01ZF}

Soit B un espace topologique et soient $(E_1, p_1)$ et $(E_2, p_2)$ des revêtements de B. Notons $(E, p)$ leur B-espace produit et soit $x= (x_1, x_2)$ un point de E. L’image de l’homomorphisme $\pi_1(p, x)$ est l’intersection des images des homomorphismes $\pi_1(p_1, x_1)$ et $\pi_1(p_2, x_2)$.

Soit $c$ un lacet de B en $p_1(x_1) =p_2(x_2)$ et, pour $i\in  \{1,2\}$, soit $c'_i$ le chemin d’origine $x_i$ dans $E_i$ relevant $c$. Le B-espace $E = E_1\times_BE_2$ est un revêtement de B (I, p. 72, cor. 3 de la prop. 2) et le chemin $c':t\mapsto$ $(c'_1(t), c'_2(t))$ est l’unique chemin d’origine $x$ dans E qui relève $c$. Pour que $c'$ soit un lacet, il faut et il suffit que $c'_1$ et $c'_2$ le soient. Le corollaire 3 résulte ainsi du corollaire 2.

### 3. Opérations du groupoïde de Poincaré dans les revêtements

Soit B un espace topologique et soit $p: E\rightarrow$ B une application étale et séparée qui vérifie la propriété de relèvement des chemins (III, p. 302) ; c’est le cas si l’application $p$ fait de E un revêtement de B (loc. cit.). Soient $b$ et $b'$ des points de B et soit $c\in \Lambda_{b,b'}(B)$ un chemin dans B reliant $b$ à $b'$. Pour tout point $x$ de la fibre $E_b$, notons $x\cdot c$ le terme du chemin d’origine $x$ dans E qui relève $c$. Le point $x\cdot c$ appartient à la fibre $E_{b'}$ et ne dépend que de la classe $\gamma \in \varpi_{b,b'}(B)$ du chemin $c($III, p. 302, prop. 4) ; on écrira ainsi $x\cdot \gamma$ au lieu de $x\cdot c$.

Si $c$ est le chemin constant en $b$, on a $x\cdot \gamma =x$ car le chemin constant d’origine $x$ relève $c$.

Soit $b''$ un autre point de B et soit $c'\in \Lambda_{b',b''}(B)$. Pour tout point $x$ de $E_b$, on a :

$$
(x\cdot c)\cdot c'=x\cdot (c*c') \tag{1}
$$

En effet, notons $\widetilde{c}$ le relèvement d’origine $x$ de $c$ et $\widetilde{c}'$ le relèvement de $c'$ d’origine $x\cdot c=\widetilde{c}(1)$. Les chemins $\widetilde{c}$ et $\widetilde{c}'$ sont juxtaposables et $\widetilde{c}*\widetilde{c}'$ est le chemin d’origine $x$ relevant $c*c'$.

Notons $\varphi_{b,b'}:\varpi_{b,b'}(B)\rightarrow \mathscr{F}(E_b; E_{b'})$ l’application telle que, pour $\gamma \in \varpi_{b,b'}(B)$ et $x\in E_b$, on ait

$$
\varphi_{b,b'}(\gamma )(x) =x\cdot \gamma
$$

Pour tout $\gamma \in \varpi_{b,b'}(B)$ et tout $\gamma '\in \varpi_{b',b''}(B)$, il résulte de la relation (1) que l’on a

$$
\varphi_{b,b''}(\gamma \gamma ') =\varphi_{b',b''}(\gamma ')\circ \varphi_{b,b'}(\gamma ) \tag{2}
$$

La famille $\varphi = (\varphi_{b,b'})_{(b,b')\in B\times B}$ définit donc une loi d’opération à droite du groupoïde $\varpi (B)$ sur l’ensemble E relativement à l’application $p: E\rightarrow$ B (II, p. 167). On l’appelle l’opération canonique du groupoïde $\varpi (B)$ associée à l’application $p: E\rightarrow B$. L’application $\varphi_{b,b}:\pi_1(B, b)\rightarrow \mathscr{F}(E_b; E_b)$ définit une loi d’opération à droite du groupe $\pi_1(B, b)$ sur la fibre $E_b$ de E. Cette opération est appelée opération canonique de $\pi_1(B, b)$ sur la fibre $E_b$.

#### Remarque {#ta-iii-s4-n3-rem-1 .statement tag=01ZG}

Soient $b$ et $b'$ deux points de B$,x$ un point de $E_b,c\in$ $\Lambda_{b,b'}(B)$ un chemin dans B et $\widetilde{c}$ le chemin dans E d’origine $x$ qui relève $c$. Pour tout $s\in \mathbf{I}$, notons $c_s$ le chemin $t\mapsto c(st)$ ; le chemin dans E d’origine $x$ relevant $c_s$ est le chemin $t\mapsto \widetilde{c}(st)$ dont le terme est le point $\widetilde{c}(s)$. On a donc $\widetilde{c}(s) =x\cdot c_s$ pour tout $s\in \mathbf{I}$.

Soit $B'$ un espace topologique et soit $p': E'\rightarrow B'$ une application étale et séparée qui vérifie la propriété de relèvement des chemins. Soient $f: B\rightarrow B'$ et $g: E\rightarrow E'$ des applications continues telles que $p'\circ g=f\circ p$. Pour $b,b'\in B,\gamma \in \varpi_{b,b'}(B)$ et $x\in E_b$, on a :

$$
g(x\cdot \gamma ) =g(x)\cdot f_*(\gamma ) \tag{3}
$$

En effet, soit $c$ un chemin dans B dont $\gamma$ est la classe d’homotopie stricte, notons $\widetilde{c}$ le chemin dans E d’origine $x$ qui relève $c$; le chemin $g\circ \widetilde{c}$ est alors le relèvement d’origine $g(x)$ de $f\circ c$ dans $E'$.

En particulier, pour $B = B'$ et $f=$ Id$_B$, on a

$$
g(x\cdot \gamma ) =g(x)\cdot \gamma \tag{4}
$$

Soient $p: E\rightarrow B$ et $p': E'\rightarrow B$ des applications étales et séparées qui vérifient la propriété de relèvement des chemins. Soit $b$ un point de B. Si $f: E\rightarrow E'$ est un B-morphisme, l’application $f_b: E_b\rightarrow E'_b$ est un $\pi_1(B, b)$-morphisme.

#### Théorème 1 {#ta-iii-s4-thm-1 .statement tag=01ZH}

Soit B un espace topologique, soit $(E, p)$ un revêtement de B, soit $b$ un point de B et soit $x$ un point de la fibre $E_b$.

a) L’orbite de $x$ pour l’opération canonique du groupe $\pi_1(B, b)$ est l’intersection de $E_b$ et de la composante connexe par arcs de $x$ dans E. En particulier, si l’espace E est connexe par arcs, cette opération est transitive.

b) Le fixateur (A, I, p. 51) de $x$ est le sous-groupe $p_*(\pi_1(E, x))$ de $\pi_1(B, b)$.

c) Pour tout $\gamma \in \pi_1(B, b)$, on a $p_*(\pi_1(E, x)) =$ Int($\gamma$ )$(p_*(\pi_1(E, x\cdot$ $\gamma )))$.

d) Si l’espace B est connexe et que le revêtement E est galoisien, le sous-groupe $p_*(\pi_1(E, x))$ est distingué dans $\pi_1(B, b)$.

L’assertion a) est immédiate. L’assertion b) résulte du cor. 2 de la prop. 4 (III, p. 303). L’assertion c) résulte de b) et de la proposition 2 de A, I, p. 52. Supposons enfin que B soit connexe et que E soit un revêtement galoisien de B. Pour tout $\gamma \in \pi_1(B, b)$, il existe un B-automorphisme $g$ de E tel que $g(x) =x\cdot \gamma ($I, p. 102, th. 2, c)). On a $p=p\circ g$, d’où $p_*(\pi_1(E, x)) =p_*(\pi_1(E, x\cdot \gamma ))$. L’assertion d) résulte donc de c).

### 4. Cas des revêtements associés à un revêtement principal

Soit B un espace topologique, soit G un groupe topologique discret et soit E un revêtement de B, principal de groupe G. Notons $p$ la projection du B-espace E. Soit $b$ un point de B et soit $x$ un point de $E_b$.

#### Proposition 5 {#ta-iii-s4-prop-5 .statement tag=01ZI}

L’application $h_{(E,x)}$ de $\pi_1(B, b)$ dans G qui, à $\gamma \in$ $\pi_1(B, b)$, associe l’unique élément $g$ de G tel que $x\cdot g=x\cdot \gamma^{-1}$, est un homomorphisme de groupes, de noyau le sous-groupe $p_*(\pi_1(E, x))$ de $\pi_1(B, b)$. Si E est connexe, cet homomorphisme est surjectif.

Pour tout $g\in G$, on a $h_{(E,x\cdot g)}=$ Int($g^{-1}$)$\circ h_{(E,x)}$.

Soit E un revêtement de B, principal de groupe G, soit $x$ un point de $E_b$ et notons $p$ la projection de E. Pour tout $g\in G$, l’application $y\mapsto y\cdot g$ est un B-automorphisme de E. On a donc, pour tout $g\in G$, tout $y\in E_b$ et tout $\gamma \in \pi_1(B, b)$, la relation $(y\cdot g)\cdot \gamma = (y\cdot \gamma )\cdot g($cf. III, p. 305, relation (4)). Par suite, pour $\gamma , \delta \in \pi_1(B, b)$, on a

$$
x\cdot h_{(E,x)}(\gamma \delta ) =x\cdot \delta^{-1}\gamma^{-1}
$$

$$
= (x\cdot h_{(E,x)}(\delta ))\cdot \gamma^{-1}
$$

$$
= (x\cdot \gamma^{-1})\cdot h_{(E,x)}(\delta )
$$

$$
=x\cdot h_{(E,x)}(\gamma )h_{(E,x)}(\delta )
$$

ce qui prouve que $h_{(E,x)}$ est un homomorphisme de groupes.

Son noyau est le fixateur de $x$ pour l’opération canonique de $\pi_1(B, b)$, donc est égal à $p_*(\pi_1(E, x))$ d’après le théorème 1 de III, p. 305. L’application $g\mapsto x\cdot g$ est une bijection de G sur $E_b$. L’image de l’homomorphisme $h_{(E,x)}$ est donc l’ensemble des $g\in G$ tels que $x\cdot g$ appartienne à l’orbite de $x$ pour cette opération. Si E est connexe, $\pi_1(B, b)$ opère transitivement sur $E_b($loc. cit.) et l’homomorphisme $h_{(E,x)}$ est surjectif.

Soit $g\in G$; pour tout $\gamma \in \pi_1(B, b)$, on a

$$
x\cdot gh_{(E,x\cdot g)}(\gamma ) = (x\cdot g)\cdot \gamma^{-1}= (x\cdot \gamma^{-1})\cdot g=x\cdot h_{(E,x)}(\gamma )g
$$

d’où $h_{(E,x\cdot g)}(\gamma ) =g^{-1}h_{(E,x)}(\gamma )g$. Cela termine la preuve de la proposition.

#### Exemple 1 {#ta-iii-s4-n4-exa-1 .statement tag=01ZJ}

Soit F un ensemble discret muni d’une opération de G et soit $X = E\times^GF$ le revêtement de B associé. Notons $\varphi : E\times F\rightarrow X$ le B-morphisme canonique. C’est un morphisme de revêtements. Pour tout $\gamma \in \pi_1(B, b)$ et tout $f\in F$, on a alors

(5)

$$
\varphi (x, f)\cdot \gamma =\varphi (x\cdot \gamma , f) =\varphi (x\cdot h_{(E,x)}(\gamma )^{-1}, f) =\varphi (x, h_{(E,x)}(\gamma^{-1})\cdot f)
$$

Si l’on identifie F à $X_b$ par l’application bijective $f\mapsto \varphi (x, f)$, il en résulte que l’opération à droite $\pi_1(B, b)\rightarrow$ Aut(X$_b$)$^{\circ}$ est la composée de l’homomorphisme $h_{(E,x)}$, de l’antihomomorphisme $g\mapsto g^{-1}$ de G dans lui-même et de l’homomorphisme $G\rightarrow$ Aut(F) déduit de l’opération de G sur F.

#### Exemple 2 {#ta-iii-s4-n4-exa-2 .statement tag=01ZK}

Soit H un groupe topologique discret, soit $f: G\rightarrow H$ un morphisme de groupes. Munissons H de l’opération à gauche de G donnée par $g\cdot h=f(g)h$, pour $g\in G$ et $h\in H$. Soit $E'= E\times^GH$ le revêtement associé ; c’est un revêtement principal de groupe H (I, p. 107, exemple 6). Notons $q: E\times H\rightarrow E\times^GH$ l’application canonique et posons $x'=q(x, e)$. On a $h_{(E',x')}=f\circ h_{(E,x)}$.

En effet, soit $c$ un lacet en $b$ dans B, soit $\gamma$ sa classe dans $\pi_1(B, b)$ et soit $g=h_{(E,x)}$; on a donc $x\cdot \gamma =x\cdot g^{-1}$. Soit $\widetilde{c}$ un chemin d’origine $x$ dans E ; alors, $t\mapsto q(\widetilde{c}(t), e)$ est un chemin d’origine $x'$ dans $E'$ qui relève le chemin $p\circ \widetilde{c}$ dans B, si bien que

$$
x'\cdot \gamma =q(x\cdot \gamma , e) =q(x\cdot g^{-1}, e) =q(x, f(g)^{-1}) =q(x, e)\cdot f(g)^{-1}
$$

ce qui démontre que $h_{(E',x')}(\gamma ) =f(g)$.

## EXERCICES {#ta-iii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
