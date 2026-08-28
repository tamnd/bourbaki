---
book: alg
book_title: Algebra
chapter: II
chapter_title: ALGÈBRE LINÉAIRE
section: 4
section_title: Relations entre produits tensoriels et modules d'homomorphismes
lang: fr
source: alg-i-iii-fr
book_pages: A II.190-A II.191
pdf_pages: 0250-0258, 0367-0368
extraction: ocr
subsections:
    - "no": 1
      title: Les isomorphismes
      page: 0
      pdf_page: 250
    - "no": 2
      title: L’homomorphisme** $E^* \otimes_A F \to \mathrm{Hom}_A(E, F)$.
      page: 74
      pdf_page: 251
    - "no": 3
      title: Trace d’un endomorphisme
      page: 78
      pdf_page: 255
    - "no": 4
      title: L’homomorphisme
      page: 79
      pdf_page: 256
statements: 15
exercises: 9
content_sha256: b14f871e442d2c9eb946f3fc7cf7f12be5c3e58f35a9cdf3ae02e8ccec04e962
---

## § 4. RELATIONS ENTRE PRODUITS TENSORIELS ET MODULES D’HOMOMORPHISMES

### 1. Les isomorphismes
$$
\operatorname{Hom}_B(E \otimes_A F, G) \to \operatorname{Hom}_A(F, \operatorname{Hom}_B(E, G))
$$
et
$$
\operatorname{Hom}_C(E \otimes_A F, G) \to \operatorname{Hom}_A(E, \operatorname{Hom}_C(F, G)).
$$

Soient E un A-module à droite, F un A-module à gauche, G un $\mathbf{Z}$-module, H le $\mathbf{Z}$-module des applications $f : E \times F \to G$ qui sont $\mathbf{Z}$-bilinéaires et telles que
$$
f(x \lambda, y) = f(x, \lambda y) \quad \text{pour } x \in E, y \in F, \lambda \in A.
$$
On a vu (II, p. 51, prop. 1) qu’il existe un isomorphisme canonique de $\mathbf{Z}$-modules
$$
H \to \operatorname{Hom}_Z(E \otimes_A F, G).
$$
D’autre part, on a défini sur $\operatorname{Hom}_Z(E, G)$ une structure de A-module à gauche et sur $\operatorname{Hom}_Z(F, G)$ une structure de A-module à droite (II, p. 54); on peut donc considérer les $\mathbf{Z}$-modules $\operatorname{Hom}_A(E, \operatorname{Hom}_Z(F, G))$ et $\operatorname{Hom}_A(F, \operatorname{Hom}_Z(E, G))$. Une application $f$ de $E \times F$ dans $G$ s’identifie canoniquement à une application de $E$ dans l’ensemble $G^F$ des applications de $F$ dans $G$ (E, II, p. 31); en exprimant que cette dernière application appartient à $\operatorname{Hom}_A(E, \operatorname{Hom}_Z(F, G))$, on obtient précisément le fait que $f$ est biadditive et les conditions (1); d’où un isomorphisme canonique
$$
H \to \operatorname{Hom}_A(E, \operatorname{Hom}_Z(F, G))
$$
et on définit de même un isomorphisme canonique
$$
H \to \operatorname{Hom}_A(F, \operatorname{Hom}_Z(E, G)).
$$
Supposons maintenant que E et G soient aussi munis de structures de B-module à gauche (resp. à droite), et que sur E les structures de A-module et de B-module soient compatibles. Alors $E \otimes_A F$ est canoniquement muni d’une structure de B-module à gauche (resp. à droite) (II, p. 54), et d’autre part $\operatorname{Hom}_B(E, G)$ est canoniquement muni d’une structure de A-module à gauche (II, p. 35). On peut donc considérer les $\mathbf{Z}$-modules $\operatorname{Hom}_B(E \otimes_A F, G)$ et $\operatorname{Hom}_A(F, \operatorname{Hom}_B(E, G))$, qui sont des sous-modules de $\operatorname{Hom}_Z(E \otimes_A F, G)$ et de $\operatorname{Hom}_A(F, \operatorname{Hom}_Z(E, G))$ respectivement (II, p. 37, th. 2). Cherchons à quelle condition une application $f \in H$ a pour image par les isomorphismes (2) et (4) un élément de $\operatorname{Hom}_B(E \otimes_A F, G)$ et un élément de $\operatorname{Hom}_A(F, \operatorname{Hom}_B(E, G))$ respectivement; dans chacun des deux cas on trouve la même condition
$$
f(\beta x, y) = \beta f(x, y)
$$
(resp.
$$
f(x \beta, y) = f(x, y) \beta)
$$
pour $x \in E, y \in F, \beta \in B$.

De même, supposons que F et G soient des C-modules à gauche (resp. à droite), et que sur F les structures de A-module et de C-module soient compatibles. Alors, pour qu’une application $f \in H$ ait pour image par (2) ou (3) un élément de $\mathrm{Hom}_C(E \otimes_A F, G)$ ou $\mathrm{Hom}_A(E, \mathrm{Hom}_C(F, G))$ respectivement, il faut et il suffit qu’elle satisfasse à la même condition

$$
f(x, \gamma y) = \gamma f(x, y)
$$
(resp.
$$
f(x, y \gamma) = f(x, y) \gamma)
$$
pour $x \in E, y \in F, \gamma \in C$.

On a donc établi le résultat suivant (avec les notations introduites ci-dessus) :

#### Proposition 1 {#alg-ii-s4-prop-1 .statement}

a) *Soient E un (B, A)-bimodule, F un A-module à gauche, G un B-module à gauche. Pour toute application $g \in \mathrm{Hom}_B(E \otimes_A F, G)$, soit $g'$ l’application de F dans $\mathrm{Hom}_B(E, G)$ définie par $(g'(y))(x) = g(x \otimes y)$ pour $x \in E, y \in F$. L’application $g \mapsto g'$ est un isomorphisme*

(5)
$$
\beta : \mathrm{Hom}_B(E \otimes_A F, G) \to \mathrm{Hom}_A(F, \mathrm{Hom}_B(E, G)).
$$

b) *Soient E un A-module à droite, F un (A, C)-bimodule, G un C-module à droite. Pour toute application $h \in \mathrm{Hom}_C(E \otimes_A F, G)$, soit $h'$ l’application de E dans $\mathrm{Hom}_C(F, G)$ définie par $(h'(x))(y) = h(x \otimes y)$ pour $x \in E, y \in F$. L’application $h \mapsto h'$ est un isomorphisme*

(6)
$$
\gamma : \mathrm{Hom}_C(E \otimes_A F, G) \to \mathrm{Hom}_A(E, \mathrm{Hom}_C(F, G)).
$$

On peut en particulier prendre pour B et C un sous-anneau $\Gamma$ du centre de l’anneau A ; alors pour tout $\Gamma$-module G, les trois $\Gamma$-modules

$$
\mathrm{Hom}_\Gamma(E \otimes_A F, G), \quad \mathrm{Hom}_A(E, \mathrm{Hom}_\Gamma(F, G)), \quad \mathrm{Hom}_A(F, \mathrm{Hom}_\Gamma(E, G))
$$

sont canoniquement isomorphes au $\Gamma$-module des applications $\Gamma$-*bilinéaires* de $E \times F$ dans G qui vérifient (1) (II, p. 73). Plus particulièrement :

#### Corollaire {#alg-ii-s4-n0-cor-1 .statement}

*Si C est un anneau commutatif, E, F, G trois C-modules, alors les C-modules*

$$
\begin{array}{ll}
\mathrm{Hom}_C(E \otimes_C F, G), & \mathrm{Hom}_C(E, \mathrm{Hom}_C(F, G)), \\
\mathrm{Hom}_C(F, \mathrm{Hom}_C(E, G)), & \mathcal{L}_2(E, F; G)
\end{array}
$$

*sont canoniquement isomorphes*.

### 2. L’homomorphisme** $E^* \otimes_A F \to \mathrm{Hom}_A(E, F)$.

Soient A, B deux anneaux, E un A-module à gauche, F un B-module à gauche, G un (A, B)*-bimodule*. Le $\mathbf{Z}$-module $\mathrm{Hom}_A(E, G)$ est canoniquement muni d’une structure de B*-module à droite (II, p. 35) telle que $(u \beta)(x) = u(x) \beta$ pour $\beta \in B$, $u \in \mathrm{Hom}_A(E, G)$, $x \in E$. D’autre part, $G \otimes_B F$ est canoniquement muni d’une structure de A-module à gauche (II, p. 54). Nous allons définir un $\mathbf{Z}$-homomorphisme canonique

(7) $$
\nu : \operatorname{Hom}_A(E, G) \otimes_B F \to \operatorname{Hom}_A(E, G \otimes_B F).
$$

Pour cela, considérons, pour tout $y \in F$ et tout $u \in \operatorname{Hom}_A(E, G)$, l’application $\nu'(u, y) : x \mapsto u(x) \otimes y$ de E dans $G \otimes_B F$. On vérifie immédiatement que $\nu'(u, y)$ est A-linéaire, et que $\nu'$ est une application $\mathbf{Z}$-bilinéaire de $\operatorname{Hom}_A(E, G) \times F$ dans $\operatorname{Hom}_A(E, G \otimes_B F)$; en outre, pour tout $\beta \in B$, $\nu'(u\beta, y)$ et $\nu'(u, \beta y)$ sont égales, car $(u(x)\beta) \otimes y = u(x) \otimes (\beta y)$. On en conclut (II, p. 51, prop. 1) l’existence de l’homomorphisme $\nu$ cherché, tel que $\nu(u \otimes y)$ soit l’application A-linéaire $x \mapsto u(x) \otimes y$.

On vérifie aussitôt que si E est un $(A, (C'_i); (D'_j))$-multimodule, F un $(B, (C''_h); (D''_k))$-multimodule, G un $(A, (C'''_l); B, (D'''_m))$-multimodule, l’application (7) est un homomorphisme de $((D'_j), (C''_h), (C'''_l); (C'_i), (D''_k), (D'''_m))$-multimodules.

#### Proposition 2 {#alg-ii-s4-prop-2 .statement}

(i) *Lorsque F est un B-module projectif* (resp. *projectif de type fini*), *l’homomorphisme canonique* (7) *est injectif* (resp. *bijectif*).

(ii) *Lorsque E est un A-module projectif de type fini*, *l’homomorphisme canonique* (7) *est bijectif*.

(i) Fixons E et G, et pour tout B-module à gauche F, posons $T(F) = \operatorname{Hom}_A(E, G) \otimes_B F$, $T'(F) = \operatorname{Hom}_A(E, G \otimes_B F)$; pour tout homomorphisme $u : F \to F'$ de B-modules à gauche, posons $T(u) = 1 \otimes u$ (1 désignant ici l’application identique de $\operatorname{Hom}_A(E, G)$), $T'(u) = \operatorname{Hom}(1_E, 1_G \otimes u)$; écrivons d’autre part $\nu_F$ au lieu de $\nu$. On a alors les lemmes suivants:

#### Lemme 1 {#alg-ii-s4-lem-1 .statement}

*Pour tout homomorphisme* $u : F \to F'$, *le diagramme*

$$
\begin{array}{ccc}
T(F) & \xrightarrow{\nu_F} & T'(F) \\
| & & | \\
T(u) & & T'(u) \\
T(F') & \xrightarrow{\nu_{F'}} & T'(F')
\end{array}
$$

*est commutatif*.

La vérification est immédiate.

#### Lemme 2 {#alg-ii-s4-lem-2 .statement}

*Soient M, N deux sous-modules supplémentaires dans F, et soient i : M \to F, j : N \to F les injections canoniques. Le diagramme*

$$
\begin{array}{ccc}
T(M) \oplus T(N) & \xrightarrow{\nu_M \oplus \nu_N} & T'(M) \oplus T'(N) \\
| & & | \\
T(i) + T(j) & & T'(i) + T'(j) \\
T(F) & \xrightarrow{\nu_F} & T'(F)
\end{array}
$$

*est commutatif, et les flèches verticales sont bijectives*.

La commutativité résulte du lemme 1; les autres assertions, de II, p. 13, cor. 2 et de II, p. 61, prop. 7.

#### Lemme 3 {#alg-ii-s4-lem-3 .statement}

Sous les hypothèses du lemme 2, pour que $\nu_F$ soit injective (resp. surjective), il faut et il suffit que $\nu_M$ et $\nu_N$ le soient.

Cela résulte du lemme 2 et de II, p. 13, cor. 1.

Cela étant, le lemme 3, joint à II, p. 39, prop. 4, montre qu’il suffit de considérer le cas où F est un module libre. Or, si $(b_\mu)$ est une base de F, tout élément de $\mathrm{Hom}_A(E, G) \otimes_B F$ s’écrit alors d’une seule manière $\sum_\mu u_\mu \otimes b_\mu$, où $u_\mu \in \mathrm{Hom}_A(E, G)$ (II, p. 62, cor. 1); l’image de cet élément par $\nu$ est l’application A-linéaire $x \mapsto \sum_\mu u_\mu(x) \otimes b_\mu$; elle ne peut être nulle pour tout $x \in E$ que si $u_\mu(x) = 0$ pour tout $x \in E$ et tout $\mu$, ce qui équivaut à dire que $u_\mu = 0$ pour tout $\mu$; donc $\nu$ est injectif. Lorsqu’en outre F admet une base finie, le lemme 3 montre (par récurrence sur le nombre d’éléments de la base de F) que pour prouver que $\nu$ est surjectif, il suffit de le faire lorsque $F = B_s$; mais dans ce cas les deux membres de (7) s’identifient canoniquement à $\mathrm{Hom}_A(E, G)$ (II, p. 55, prop. 4) et $\nu$ devient l’identité.

(ii) Pour démontrer la proposition lorsque E est projectif et de type fini, fixons cette fois F et G, et posons, pour tout A-module à gauche E, $T(E) = \mathrm{Hom}_A(E, G) \otimes_B F$, $T'(E) = \mathrm{Hom}_A(E, G \otimes_B F)$, et pour tout homomorphisme $v : E \to E'$ de A-modules à gauche, $T(v) = \mathrm{Hom}(v, 1_G) \otimes 1_F$, $T'(v) = \mathrm{Hom}(v, 1_G \otimes 1_F)$; écrivons d’autre part $\nu_E$ au lieu de $\nu$. On a alors les deux lemmes:

#### Lemme 4 {#alg-ii-s4-lem-4 .statement}

Pour tout homomorphisme $v : E \to E'$, le diagramme

$$
\begin{array}{ccc}
T(E') & \xrightarrow{\nu_{E'}} & T'(E') \\
| & & | \\
T(v) & & T'(v) \\
\downarrow & & \downarrow \\
T(E) & \xrightarrow{\nu_E} & T'(E)
\end{array}
$$

est commutatif.

#### Lemme 5 {#alg-ii-s4-lem-5 .statement}

Soient M et N deux sous-modules supplémentaires dans E, et soient $p : E \to M$, $q : E \to N$ les projections canoniques. Le diagramme

$$
\begin{array}{ccc}
T(M) \oplus T(N) & \xrightarrow{\nu_M \oplus \nu_N} & T'(M) \oplus T'(N) \\
| & & | \\
T(p) + T(q) & & T'(p) + T'(q) \\
\downarrow & & \downarrow \\
T(E) & \xrightarrow{\nu_E} & T'(E)
\end{array}
$$

est commutatif, et les flèches verticales sont bijectives.

Ils se démontrent comme les lemmes 1 et 2, compte tenu de II, p. 13, cor. 2, de II, p. 37, prop. 1 et de II, p. 61, prop. 7.

Le reste de la démonstration procède alors comme dans (i) et on est ramené au cas où $E = A_s$; les deux membres de (7) s’identifient alors canoniquement à $G \otimes_B F$ et $\nu$ devient l’identité.

C. Q. F. D.

Prenons en particulier $B = A$, et pour $G$ le $(A, A)$-bimodule ${}_sA_d$ (II, p. 55), de sorte que le $A$-module à droite $\mathrm{Hom}_A(E, {}_sA_d)$ n’est autre que le *dual* $E^*$ de $E$, et $({}_sA_d) \otimes_A F$ s’identifie canoniquement à $F$ (II, p. 55, prop. 4). L’homomorphisme (7) se particularise alors en un $\mathbf{Z}$-homomorphisme canonique

$$
\theta : \quad E^* \otimes_A F \to \mathrm{Hom}_A(E, F)
$$

et $\theta(x^* \otimes y)$ est l’application linéaire de $E$ dans $F$

$$
x \mapsto \langle x, x^*\rangle y.
$$

*Remarque 1).* — La caractérisation des $A$-modules *projectifs* donnée dans II, p. 46, prop. 12, peut encore s’exprimer de la façon suivante: pour qu’un $A$-module à gauche de type fini $E$ soit projectif, il faut et il suffit que l’homomorphisme canonique

$$
\theta_E : \quad E^* \otimes_A E \to \mathrm{Hom}_A(E, E) = \mathrm{End}_A(E)
$$

soit tel que $1_E$ *appartienne à l’image de* $\theta_E$.

#### Corollaire {#alg-ii-s4-n2-cor-1 .statement}

(i) *Lorsque* $F$ *est un module projectif* (resp. *projectif de type fini*), *l’homomorphisme canonique* (11) *est injectif* (resp. *bijectif*).

(ii) *Lorsque* $E$ *est un module projectif de type fini*, *l’homomorphisme canonique* (11) *est bijectif*.

Même lorsque $E$ et $F$ sont tous deux de type fini, $\theta$ n’est pas nécessairement surjectif, comme le montre l’exemple $A = \mathbf{Z}$, $E = F = \mathbf{Z}/2\mathbf{Z}$; le second membre de (11) n’est pas réduit à 0, mais on a $E^* = \{0\}$. D’autre part, on peut donner des exemples où $E$ est *libre*, mais où (11) n’est ni injectif ni surjectif (II, p. 189, exerc. 3 b)).

Lorsque $E$ admet une base finie $(e_i)$, on peut expliciter de la façon suivante l’isomorphisme réciproque $\theta^{-1}$ de $\theta$. En effet, soit $(e_i^*)$ la base duale de $(e_i)$ (II, p. 45); pour tout $u \in \mathrm{Hom}_A(E, F)$ et tout $x = \sum_i \xi_i e_i$ avec $\xi_i \in A$, on a $u(x) = \sum_i \xi_i u(e_i) = \sum_i \langle x, e_i^* \rangle u(e_i)$, et par suite on a $u = \sum_i \theta(e_i^* \otimes u(e_i))$, autrement dit

$$
\theta^{-1}(u) = \sum_i e_i^* \otimes u(e_i).
$$

En particulier, si de plus $F = E$, on voit que l’image par $\theta_E^{-1}$ de l’application identique $1_E$ est l’élément $\sum_i e_i^* \otimes e_i$, qui est donc *indépendant* de la base $(e_i)$ considérée dans $E$.

Notons d’autre part que lorsque $E$ est un module projectif de type fini, on peut transporter par $\theta_E^{-1}$ la structure d’*anneau* de $\mathrm{End}_A(E)$ à $E^* \otimes_A E$; on vérifie immédiatement que pour $x, y$ dans $E$, $x^*, y^*$ dans $E^*$, on a, dans l’anneau $\mathrm{End}_A(E)$

$$
\theta_E(x^* \otimes x) \circ \theta_E(y^* \otimes y) = \theta_E((y^* \langle y, x^* \rangle) \otimes x).
$$

*Remarque 2).* — Soit $E$ un $A$-module *à droite*; remplaçant $E$ par $E^*$ dans (11), on obtient un $\mathbf{Z}$-homomorphisme canonique

$$
E^{**} \otimes_A F \to \mathrm{Hom}_A(E^*, F).
$$

D’autre part, on a un A-homomorphisme canonique $c_E : E \to E^{**}$, d’où un $\mathbf{Z}$-homomorphisme $c_E \otimes 1_F : E \otimes_A F \to E^{**} \otimes_A F$; composant avec ce dernier l’homomorphisme (14), on obtient donc un $\mathbf{Z}$-homomorphisme canonique
$$
\theta' : E \otimes_A F \to \operatorname{Hom}_A(E^*, F)
$$
tel que $\theta'(x \otimes y)$ soit l’application linéaire
$$
x^* \mapsto \langle x, x^*\rangle y.
$$

Si $E$ et $F$ sont des modules *projectifs*, l’application (15) est *injective*. En effet, $c_E$ est alors injective (II, p. 47, cor. 4), et comme $F$ est projectif, le $\mathbf{Z}$-homomorphisme $c_E \otimes 1_F : E \otimes_A F \to E^{**} \otimes_A F$ est aussi injectif (II, p. 63, cor. 6); enfin, on a vu (II, p. 75, prop. 2) que l’homomorphisme (14) est injectif, d’où la conclusion.

Si $E$ est *projectif de type fini*, l’application (15) est *bijective* car les deux applications dont elle est composée sont alors bijectives (II, p. 47, cor. 4, et II, p. 75, prop. 2).

### 3. Trace d’un endomorphisme

Soit $C$ un anneau *commutatif*, et soit $E$ un $C$-module. L’application $(x^*, x) \mapsto \langle x, x^*\rangle$ de $E^* \times E$ dans $C$ est alors $C$-*bilinéaire*, car pour tout $\gamma \in C$, on a $\langle \gamma x, x^*\rangle = \gamma \langle x, x^*\rangle$ et $\langle x, x^*\gamma \rangle = \langle x, x^*\rangle \gamma$; on en déduit une application $C$-*linéaire* canonique
$$
\tau : E^* \otimes_C E \to C
$$
telle que $\tau(x^* \otimes x) = \langle x, x^*\rangle$ (II, p. 56). Supposons maintenant en outre que $E$ soit un $C$-module *projectif de type fini*; l’isomorphisme canonique (11) de II, p. 77 est alors un isomorphisme de $C$-*modules*, et on peut donc définir par transport de structure une *forme linéaire canonique* $\operatorname{Tr} = \tau \circ \theta_E^{-1}$ sur le $C$-module $\operatorname{End}_C(E)$. Pour tout $u = \operatorname{End}_C(E)$, on dit que le scalaire $\operatorname{Tr}(u)$ est la *trace* de l’endomorphisme $u$; tout $u \in \operatorname{End}_C(E)$ peut s’écrire (en général d’une infinité de manières) sous la forme $x \mapsto \sum_i \langle x, x_i^*\rangle y_i$ où $x_i^* \in E^*$ et $y_i \in E$, en vertu de II, p. 77, corollaire; on a alors
$$
\operatorname{Tr}(u) = \sum_i \langle y_i, x_i^*\rangle \tag{cf. II, p. 158}.
$$

Par définition, on a
$$
\operatorname{Tr}(u + v) = \operatorname{Tr}(u) + \operatorname{Tr}(v) \tag{18}
$$
$$
\operatorname{Tr}(\gamma u) = \gamma \operatorname{Tr}(u) \tag{19}
$$
pour $u, v$ dans $\operatorname{End}_C(E)$ et $\gamma \in C$. En outre:

#### Proposition 3 {#alg-ii-s4-prop-3 .statement}

*Soient $C$ un anneau commutatif, $E, F$ deux $C$-modules projectifs de type fini, $u : E \to F$ et $v : F \to E$ deux applications linéaires; on a alors*
$$
\operatorname{Tr}(v \circ u) = \operatorname{Tr}(u \circ v). \tag{20}
$$

Les deux applications $(u, v) \mapsto \mathrm{Tr}(u \circ v), (u, v) \mapsto \mathrm{Tr}(v \circ u)$ de
$$
\mathrm{Hom}_C(E, F) \times \mathrm{Hom}_C(F, E)
$$
dans $C$ sont $C$-bilinéaires; il suffit donc de vérifier (20) lorsque $u$ est de la forme $x \mapsto \langle x, a^*\rangle b$ et $v$ de la forme $y \mapsto \langle y, b^*\rangle a$, avec $a \in E, a^* \in E^*, b \in F, b^* \in F^*$. Mais alors $v \circ u$ est l’application $x \mapsto \langle x, a^*\rangle \langle b, b^*\rangle a$ et $u \circ v$ l’application $y \mapsto \langle y, b^*\rangle \langle a, a^*\rangle b$. La formule (17) montre que les valeurs des deux membres de (20) sont égales à $\langle a, a^*\rangle \langle b, b^*\rangle$.

#### Corollaire {#alg-ii-s4-n3-cor-1 .statement}

*Si $u_1, \ldots, u_p$ sont des endomorphismes de $E$, on a*
$$
\mathrm{Tr}(u_1 \circ u_2 \circ \cdots \circ u_p) = \mathrm{Tr}(u_i \circ u_{i+1} \circ \cdots \circ u_p \circ u_1 \circ \cdots \circ u_{i-1})
$$
*pour $1 \leq i \leq p$ (« invariance de la trace par permutation circulaire »)*.

Il suffit d’appliquer (20) au produit
$$
(u_1 \circ u_2 \circ \cdots \circ u_{i-1}) \circ (u_i \circ u_{i+1} \circ \cdots \circ u_p).
$$
On notera par contre qu’on n’a pas nécessairement $\mathrm{Tr}(u \circ v \circ w) = \mathrm{Tr}(u \circ w \circ v)$ pour trois endomorphismes $u, v, w$ de $E$.

### 4. L’homomorphisme

$$
\mathrm{Hom}_C(E_1, F_1) \otimes_C \mathrm{Hom}_C(E_2, F_2) \to \mathrm{Hom}_C(E_1 \otimes_C E_2, F_1 \otimes_C F_2).
$$

Soient $C$ un anneau *commutatif*, $E_1, E_2, F_1, F_2$ quatre $C$-modules; on a défini dans II, p. 57, formule (13), un homomorphisme canonique de $C$-modules
$$(21)\quad \lambda : \mathrm{Hom}(E_1, F_1) \otimes \mathrm{Hom}(E_2, F_2) \to \mathrm{Hom}(E_1 \otimes E_2, F_1 \otimes F_2).$$

#### Proposition 4 {#alg-ii-s4-prop-4 .statement}

*Lorsque l’un des couples $(E_1, E_2), (E_1, F_1), (E_2, F_2)$ est formé de $C$-modules projectifs de type fini, l’homomorphisme canonique (21) est bijectif*.

Il suffit évidemment de faire la démonstration pour les couples $(E_1, F_1)$ et $(E_1, E_2)$.

Considérons d’abord le cas du couple $(E_1, F_1)$; fixons $E_2, F_1, F_2$, et posons pour *tout* $C$-module $E$, $T(E) = \mathrm{Hom}(E, F_1) \otimes_C \mathrm{Hom}(E_2, F_2)$ et $T'(E) = \mathrm{Hom}(E \otimes E_2, F_1 \otimes F_2)$; pour tout $C$-homomorphisme $v : E \to E'$, posons
$$
T(v) = \mathrm{Hom}(v, 1_{F_1}) \otimes 1_{\mathrm{Hom}(E_2, F_2)} \text{ et } T'(v) = \mathrm{Hom}(v \otimes 1_{E_2}, 1_{F_1} \otimes F_2).
$$
Alors, *les lemmes 4 et 5* (II, p. 76) (où on remplace $v$ par $\lambda$) *sont valables* et se démontrent de façons tout à fait analogues.

Fixons ensuite $E_2$ et $F_2$, et posons cette fois, pour tout $C$-module $F$, $T(F) = \mathrm{Hom}(C, F) \otimes_C \mathrm{Hom}(E_2, F_2)$ et $T'(F) = \mathrm{Hom}(C \otimes E_2, F \otimes F_2)$, et pour tout $C$-homomorphisme $u : F \to F'$, $T(u) = \mathrm{Hom}(1_C, u) \otimes 1_{\mathrm{Hom}(E_2, F_2)}$ et $T'(u) = \mathrm{Hom}(1_C \otimes 1_{E_2}, u \otimes 1_{F_2})$. Cette fois on vérifie aussitôt que *les lemmes 1 et 2* (II, p. 75) (où $\lambda$ remplace toujours $v$) *sont valables*.

Cela étant, démontrons d’abord la proposition lorsque $E_1 = C$ et que $F_1$ est projectif de type fini. Le raisonnement de II, p. 76 (qui repose sur les lemmes 1 et 2), joint aux remarques ci-dessus, ramène à prouver la proposition lorsque l’on a aussi $F_1 = C$; alors $\mathrm{Hom}(E_1, F_1), E_1 \otimes E_2$ et $F_1 \otimes F_2$ s’identifient à

C, E_2, et F_2 respectivement (II, p. 55, prop. 4); les deux membres de (21) s’identifient alors canoniquement tous deux à Hom(E_2, F_2) et, après ces identifications, on vérifie que $\lambda$ devient l’identité.

Supposons F_1 projectif de type fini; le raisonnement de II, p. 76 (s’appuyant cette fois sur les lemmes 4 et 5) ramène la démonstration pour E_1 projectif de type fini quelconque au cas où E_1 = C, c’est-à-dire au premier cas traité.

Pour le couple (E_1, E_2), on procède de même en appliquant cette fois les lemmes 4 et 5 à deux reprises; nous laissons les détails au lecteur.

On notera que lorsque E_1 = C^{(I)}, E_2 = C^{(J)} sont libres (de type fini ou non), on a Hom(E_1, F_1) = F_1^I, Hom(E_2, F_2) = F_2^J, et Hom(E_1 \otimes E_2, F_1 \otimes F_2) = (F_1 \otimes F_2)^{I \times J} à des isomorphismes canoniques près, et (21) s’identifie alors à un cas particulier de l’homomorphisme canonique (22) de II, p. 61.

Lorsque E_2 = C, l’homomorphisme canonique (21) de II, p. 79, donne, après identification de Hom(E_2, F_2) à F_2 et de E_1 \otimes E_2 à E_1, un homomorphisme canonique

$$
\text{(22)} \quad \text{Hom}(E, F) \otimes G \to \text{Hom}(E, F \otimes G)
$$

pour trois C-modules quelconques E, F, G, qui n’est autre que l’homomorphisme (7) de II, p. 75 pour A = B = C.

On notera que lorsque F = C, l’homomorphisme canonique (22) redonne (11) (II, p. 77) pour le cas d’un anneau commutatif.

Supposons maintenant que F_1 = F_2 = C; comme F_1 \otimes F_2 s’identifie à C, on a cette fois un homomorphisme canonique

$$
\text{(23)} \quad \mu : \quad E^* \otimes F^* \to (E \otimes F)^*
$$

pour deux C-modules E, F; pour $x^* \in E^*, y^* \in F^*$, l’image de $x^* \otimes y^*$ par l’homomorphisme canonique (23) est la forme linéaire u sur E \otimes F telle que

$$
\text{(24)} \quad u(x \otimes y) = \langle x, x^* \rangle \langle y, y^* \rangle.
$$

En outre, si E_1, E_2, F_1, F_2 sont quatre C-modules, $f : E_1 \to E_2, g : F_1 \to F_2$ deux applications linéaires, il résulte aussitôt de (24) que le diagramme

$$
\begin{array}{ccc}
E_2^* \otimes F_2^* & \xrightarrow{\mu} & (E_2 \otimes F_2)^* \\
tf \otimes tg \downarrow & & \downarrow t(f \otimes g) \\
E_1^* \otimes F_1^* & \xrightarrow{\mu} & (E_1 \otimes F_1)^*
\end{array}
$$

est *commutatif*.

#### Corollaire 1 {#alg-ii-s4-prop-4-cor-1 .statement}

*Si l’un des modules E, F est projectif et de type fini, l’homomorphisme canonique (23) est bijectif.*

#### Corollaire 2 {#alg-ii-s4-prop-4-cor-2 .statement}

*Soient E_1, E_2 deux C-modules projectifs de type fini, u_1 un endomorphisme de E_1, u_2 un endomorphisme de E_2; on a alors*

$$
\text{(26)} \quad \operatorname{Tr}(u_1 \otimes u_2) = \operatorname{Tr}(u_1) \operatorname{Tr}(u_2).
$$

Par linéarité, il suffit de considérer le cas où $u_1$ est de la forme $x_1 \mapsto \langle x_1, x_1^* \rangle y_1$ et $u_2$ de la forme $x_2 \mapsto \langle x_2, x_2^* \rangle y_2$; alors l’image de $x_1 \otimes x_2$ par $u_1 \otimes u_2$ est par définition

$$
\langle x_1, x_1^* \rangle \langle x_2, x_2^* \rangle (y_1 \otimes y_2) = \langle x_1 \otimes x_2, x_1^* \otimes x_2^* \rangle (y_1 \otimes y_2)
$$

$x_1^* \otimes x_2^*$ étant canoniquement identifié par $\mu$ à un élément de $(E_1 \otimes E_2)^*$. Comme $\langle y_1 \otimes y_2, x_1^* \otimes x_2^* \rangle = \langle y_1, x_1^* \rangle \langle y_2, x_2^* \rangle$, la formule (26) résulte dans ce cas de (17) (II, p. 78).

#### Remarque {#alg-ii-s4-n4-rem-1 .statement}

Si $E, F, G$ sont trois $C$-modules quelconques, on vérifie aussitôt que le diagramme

$$
\begin{array}{ccc}
E^* \otimes F^* \otimes G^* & \xrightarrow{\mu \otimes 1} & (E \otimes F)^* \otimes G^* \\
1 \otimes \mu \downarrow & & \downarrow \mu \\
E^* \otimes (F \otimes G)^* & \xrightarrow{\mu} & (E \otimes F \otimes G)^*
\end{array}
$$

est *commutatif*, en vertu de la formule (24) (II, p. 80).

Notons aussi que, sans hypothèse sur les $C$-modules $E, F$, on a des *isomorphismes* canoniques

(28) $$ (E \otimes F)^* \to \mathrm{Hom}(E, F^*) $$
(29) $$ (E \otimes F)^* \to \mathrm{Hom}(F, E^*) $$

qui ne sont autres que les isomorphismes (6) et (5) de II, p. 74 pour $G = C$, $A = B = C$.

On définit ainsi une correspondance biunivoque canonique entre les *formes bilinéaires* sur $E \times F$, les *homomorphismes de E dans F* et les *homomorphismes de F dans E*: si $u$ (resp. $v$) est un homomorphisme de $E$ dans $F^*$ (resp. de $F$ dans $E^*$), la forme bilinéaire qui lui correspond est donnée par

$$
(x, y) \mapsto \langle y, u(x) \rangle \quad \text{(resp. } (x, y) \mapsto \langle x, v(y) \rangle \text{)}.
$$

## EXERCICES {#alg-ii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
