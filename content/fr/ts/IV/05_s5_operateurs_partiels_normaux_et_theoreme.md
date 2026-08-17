---
book: ts
book_title: Théories spectrales
chapter: IV
chapter_title: THÉORIE SPECTRALE HILBERTIENNE
section: 5
section_title: Opérateurs partiels normaux et théorème spectral
lang: fr
source: ts-iii-v-fr
book_pages: TS IV.262-TS IV.311, TS IV.352-TS IV.372
pdf_pages: 0275-0324, 0365-0385
extraction: native
subsections:
    - "no": 1
      title: Bornification
      page: 262
      pdf_page: 275
    - "no": 2
      title: Opérateurs partiels normaux et théorème spectral
      page: 265
      pdf_page: 278
    - "no": 3
      title: Calcul fonctionnel universellement mesurable
      page: 270
      pdf_page: 283
    - "no": 4
      title: Projecteurs spectraux
      page: 277
      pdf_page: 290
    - "no": 5
      title: La formule de Helffer–Sjöstrand
      page: 280
      pdf_page: 293
    - "no": 6
      title: Topologies résolvantes et continuité du calcul fonctionnel
      page: 285
      pdf_page: 298
    - "no": 7
      title: Décomposition polaire
      page: 289
      pdf_page: 302
    - "no": 8
      title: Opérateurs auto-adjoints définis par une forme hermitienne partielle positive
      page: 291
      pdf_page: 304
    - "no": 9
      title: Principes variationnels pour le spectre des opérateurs positifs
      page: 296
      pdf_page: 309
    - "no": 10
      title: Perturbation compacte et spectre essentiel
      page: 303
      pdf_page: 316
    - "no": 11
      title: Perturbation
      page: 305
      pdf_page: 318
    - "no": 12
      title: Opérateurs à résolvante compacte
      page: 307
      pdf_page: 320
statements: 75
exercises: 43
content_sha256: d991f35c8f7c0acffc5b7432b05db05a7ea5b27962d1e1458c8bc3b1169340db
---

## § 5. OPÉRATEURS PARTIELS NORMAUX ET THÉORÈME SPECTRAL

### 1. Bornification

Soit E un espace hilbertien complexe. On note $s$ l’application unitaire $(x, y)\mapsto (-y, x)$ sur $E\oplus E$. Soit $u$ un opérateur partiel fermé à domaine dense sur E. L’opérateur partiel $u^*u$ est auto-adjoint et positif (prop. 12 de IV, p. 241), donc $-1\in /$ Sp($u^*u$) (prop. 17 de IV, p. 248). On note $W(u) = (1_E+u^*u)^{-1}=-R(u^*u,-1)$; c’est un endomorphisme positif et injectif de E.

Notons $p_1$ et $p_2$ les deux projections canoniques de $\Gamma_u$ dans E. Ce sont des éléments de $\mathscr{L}(\Gamma_u; E)$, et on a l’égalité de correspondances $p_2=u\circ p_1$. Soit $(j,|p^*_1|)$ la décomposition polaire (déf. 4 de I, p. 140) de l’endomorphisme $p^*_1\in \mathscr{L}(E; \Gamma_u)$, de sorte que $p^*_1=|p^*_1| \circ j$. L’application $j$ est une isométrie partielle de E dans $\Gamma_u$.

#### Définition 1 {#ts-iv-s5-def-1 .statement tag=0359}

L’endomorphisme $p_2\circ j$ de E est appelé la bornification de $u$; on note $b(u)$ cet endomorphisme.

On a $\|b(u)\|\leqslant 1$.

#### Proposition 1 {#ts-iv-s5-prop-1 .statement tag=035A}

On a les formules

$$
|p^*_1|= W(u)^{1/2} \tag{1}
$$

$$
b(u) =u\circ W(u)^{1/2}=u\circ  |p^*_1| \tag{2}
$$

$$
1_E-b(u)^*b(u) = W(u) \tag{3}
$$

$$
b(u)W(u) = W(u^*)b(u),b(u)W(u)^{1/2}= W(u^*)^{1/2}b(u) \tag{4}
$$

Soit $x\in E$. Notons $y= W(u)(x)\in$ dom($u^*u$). On a $y\in$ dom($u$) et $u(y)\in$ dom($u^*$). Pour tout élément $(y_1, u(y_1))$ de $\Gamma_u$, où $y_1\in$ dom($u$), on calcule

$$
\langle (y, u(y))|(y_1, u(y_1))\rangle =\langle y|y_1\rangle +\langle u(y)|u(y_1)\rangle
$$

$$
=\langle y+u^*u(y)|y_1\rangle =\langle x|p_1(y_1, u(y_1))\rangle
$$

Cela signifie que $p^*_1(x) = (y, u(y))$, d’où $p_1\circ p^*_1(x) =y= W(u)(x)$. Par conséquent, on a $p_1\circ p^*_1= W(u)$, donc $|p^*_1|= W(u)^{1/2}$, c’est-à-dire la formule (1). En particulier, comme Im($p_1$) $=$ Im($|p^*_1|$) d’après le cor. de la prop. 11 de I, p. 140, il vient dom($u$) $=$ Im($p_1$) $=$ Im(W($u$)$^{1/2})$. L’opérateur partiel $u\circ W(u)^{1/2}$ a donc pour domaine l’espace E. La relation $p_1\circ j= (p^*_1)^*\circ j=|p^*_1|= W(u)^{1/2}$ (prop. 11, a) de I, p. 140) implique alors que

$$
b(u) =p_2\circ j=u\circ p_1\circ j=u\circ W(u)^{1/2}
$$

ce qui est la formule (2).

On a Ker($j$) $=$ Ker($|p^*_1|$) (prop. 10, b) de I, p. 139) et la formule (1) implique donc que l’isométrie partielle $j: E\rightarrow \Gamma_u$ est injective, donc isométrique, d’où $j^*\circ j= 1_E$. En écrivant $j= (p_1\circ j, b(u))$, on trouve

$$
1_E=j^*\circ j= (p_1\circ j)^*(p_1\circ j) +b(u)^*b(u) = W(u) +b(u)^*b(u)
$$

d’où la formule (3).

Soit $x\in$ dom($u$) et posons $y= W(u)(x)$. On a $y\in$ dom($u$) et la formule $y+u^*u(y) =x$ implique que $u^*u(y)\in$ dom($u$). On a alors

$$
W(u^*)^{-1}(u(y)) = (1_E+uu^*)(u(y))
$$

$$
=u(y) +uu^*u(y) =u(y+u^*u(y)) =u(x)
$$

ce qui signifie que la réduction de $u\circ W(u)$ au domaine de $u$ est égale à $W(u^*)\circ u$. Comme l’image de $|p^*_1|$ est égale à celle de $p_1$ (cor. de la prop. 11 de I, p. 140) donc au domaine de $u$, il vient

$$
u\circ W(u)\circ  |p^*_1|= W(u^*)\circ u\circ  |p^*_1|= W(u^*)\circ b(u)
$$

(formule (2)). De plus, $|p^*_1|= W(u)^{1/2}$ commute avec $W(u)$, donc on obtient

$$
b(u)\circ W(u) =u\circ  |p^*_1| \circ W(u) =u\circ W(u)\circ  |p^*_1|= W(u^*)\circ b(u)
$$

Cette relation implique que $b(u)\circ f(W(u)) =f(W(u^*))\circ b(u)$ pour toute fonction $f\in \mathscr{C}(\mathbf{R}_+)$ (prop. 11 de I, p. 113), donc en particulier que $b(u)\circ W(u)^{1/2}= W(u^*)^{1/2}\circ b(u)$. Cela démontre la formule (4) et conclut la démonstration.

#### Corollaire {#ts-iv-s5-n1-cor-1 .statement tag=035B}

On a $b(u)^*=b(u^*)$.

Notons $q_1$ et $q_2$ les projections $\Gamma_{u^*}\rightarrow E$ et notons $(k,|q_1^*|)$ la décomposition polaire de $q_1^*$, de sorte que $b(u^*) =q_2\circ k$. Pour tous $x$ et $y$ dans E, on a $j(x)\in \Gamma_u$ et $k(y)\in \Gamma_{u^*}$, et comme $\Gamma_u$ est orthogonal à $s(\Gamma_{u^*})$ d’après la prop. 7 de IV, p. 236, il vient

$$
0 =\langle j(x)|s(k(y))\rangle =\langle p_1\circ j(x)| -q_2\circ k(y)\rangle +\langle p_2\circ j(x)|q_1\circ k(y)\rangle
$$

Comme $p_1\circ j=|p^*_1|$ et $q_1\circ k=|q^*_1|$ (prop. 11, b) de I, p. 140) on obtient

$$
\langle b(u)x| |q^*_1|y\rangle =\langle |p^*_1|x|b(u^*)y\rangle
$$

donc $|q^*_1|b(u) =b(u^*)^*|p^*_1|$. En utilisant les formules (1) et (4), on en conclut que $b(u)|p^*_1|=|q^*_1|b(u) =b(u^*)^*|p^*_1|$, et comme l’image de $|p^*_1|$ est le domaine de $u$, qui est dense dans E, on en déduit $b(u) =b(u^*)^*$.

On note Ω(E) l’ensemble des $v\in \mathscr{L}(E)$ tels que $1_E-v^*v$ est positif et injectif. Pour $v\in \Omega (E)$, l’endomorphisme hermitien $(1_E-v^*v)^{1/2}$ est injectif, puisque son carré l’est, et on note $B(v)$ l’opérateur partiel $v\circ ((1_E-v^*v)^{1/2})^{-1}$.

Notons que $1_E-v^*v$ est positif si et seulement si $\|v\|\leqslant 1$, puisque on a $\langle x|(1_E-v^*v)(x)\rangle =\|x\|^2- \|v(x)\|^2$ pour tout $x\in E$.

#### Lemme 1 {#ts-iv-s5-lem-1 .statement tag=035C}

Le sous-ensemble Ω(E) est auto-adjoint dans $\mathscr{L}(E)$.

Soit $v\in \Omega (E)$. On a $\|v^*\|=\|v\|\leqslant 1$ donc l’endomorphisme $1_E-vv^*$ est positif. Il est injectif : si $x\in$ Ker(1$_E-vv^*)$, on a $vv^*(x) =x$, d’où $v^*(v(v^*(x))) =v^*(x)$ puis $v^*(x) = 0$, puisque $1_E-v^*v$ est injectif, et enfin $x=v(v^*(x)) = 0$. Le lemme en résulte.

#### Proposition 2 {#ts-iv-s5-prop-2 .statement tag=035D}

L’application $u\mapsto b(u)$ définit une bijection de l’ensemble des opérateurs partiels fermés à domaine dense sur E sur l’ensemble Ω(E). La bijection réciproque est donnée par $v\mapsto B(v)$.

La relation $1_E-b(u)^*b(u) = W(u)$ (formule (3)) implique que $b(u)$ appartient à Ω(E) puisque $W(u)$ est positif et injectif. Comme de plus $b(u) =u\circ W(u)^{1/2}$ (formule (2)), on obtient

$$
u=b(u)\circ (W(u)^{1/2})^{-1}=b(u)\circ ((1-b(u)^*b(u))^{1/2})^{-1}= B(b(u))
$$

Réciproquement, soit $v\in \Omega (E)$. Posons $w= (1_E-v^*v)^{1/2}$ et notons $u= B(v) =v\circ w^{-1}$. Le domaine de $u$ est l’image de $w$, qui est dense dans E puisque $w$ est hermitien et injectif (EVT, V, p. 41, prop. 4 (i)). Pour tout $x\in$ dom($u$), il vient

$$
\|u(x)\|^2=\langle (v^*v)(w^{-1}(x))|w^{-1}(x)\rangle
$$

$$
=-\langle (1_E-v^*v)(w^{-1}(x))|w^{-1}(x)\rangle +\|w^{-1}(x)\|^2
$$

$$
=-\langle w(x)|w^{-1}(x)\rangle +\|w^{-1}(x)\|^2
$$

puisque $(1_E-v^*v)\circ w^{-1}$ est la réduction de $w$ au domaine de $w^{-1}$. Comme $w$ est auto-adjoint, on en déduit que

$$
\|w^{-1}(x)\|^2=\|x\|^2+\|v\circ w^{-1}(x)\|^2=\|x\|^2+\|u(x)\|^2
$$

et l’opérateur partiel $B(v) =u=v\circ w^{-1}$ est donc fermé d’après le lemme 2 de IV, p. 231.

Démontrons finalement que $b(B(v)) =v$. Comme $u=v\circ w^{-1}$, on a $v=u\circ w$, et il suffit donc de vérifier que $w= W(u)^{1/2}$ (formule (2)), ou même que $1_E-v^*v= W(u)$.

L’endomorphisme $v^*$ appartient à Ω(E) d’après le lemme 1. Posons $w'= (1_E-vv^*)^{1/2}$. C’est un endomorphisme positif injectif de E, et on a $v\circ w=w'\circ v$ (prop. 11 de I, p. 113). Le graphe de $u$ est l’ensemble des éléments de la forme $(w(x), v(x))$ pour $x\in E$. D’après la prop. 7 de IV, p. 236, le graphe de $u^*$ est $s(\Gamma_u)^{\circ}$. Comme, pour tous $x$ et $y\in E$, on a

$$
\langle (w'(x), v^*(x))|(-v(y), w(y))\rangle =-\langle x|w'v(y)\rangle +\langle x|vw(y)\rangle = 0
$$

le graphe de $u^*$ contient les éléments de la forme $(w'(x), v^*(x))$ pour $x\in E$, et on a alors $u^*(w'(x)) =v^*(x)$. En particulier, le domaine de $u^*$ contient l’image de $w'$.

Soit $x\in E$ et posons $y=w^2(x) = (1_E-v^*v)(x)$, donc $x=y+v^*v(x)$. On a $y\in$ dom($u$) et $u(y) =v(w^{-1}(y)) =v(w(x)) =w'(v(x))$. En particulier, $u(y)\in$ Im($w$)$\subset$ dom($u^*$), et $u^*(u(y)) =v^*(v(x))$. Il vient donc $x=y+v^*v(x) =y+u^*u(y)$, d’où $y= W(u)(x)$, c’est-à-dire

$$
(1_E-v^*v)(x) = W(u)(x)
$$

On a donc démontré que $1_E-v^*v= W(u)$, comme désiré.

#### Corollaire {#ts-iv-s5-n1-cor-2 .statement tag=035E}

L’endomorphisme $b(u)$ est hermitien si et seulement si $u$ est auto-adjoint.

Cela résulte de l’injectivité de l’application $u\mapsto b(u)$ (prop. 2) et de la formule $b(u^*) =b(u)^*$ (cor. de la prop. 1).

### 2. Opérateurs partiels normaux et théorème spectral

Dans ce numéro, E est un espace hilbertien complexe.

#### Définition 2 {#ts-iv-s5-def-2 .statement tag=035F}

Soit $u$ un opérateur partiel sur E. On dit que $u$ est normal si $u$ est fermé à domaine dense et si sa bornification $b(u)$ est un endomorphisme normal de E.

Si $u\in \mathscr{L}$ (E), cette définition coïncide avec EVT, V, p. 42, déf. 4, d’après les formules $1_E-b(u)^*b(u) = W(u) = (1_E+u^*u)^{-1}$ (prop. 1 de IV, p. 262) et $b(u^*) =b(u)^*$ (cor. de loc. cit.).

Si $u$ est un opérateur partiel auto-adjoint sur E, alors $b(u)$ est hermitien (cor. de la prop. 2 de IV, p. 264) donc $u$ est normal.

Soit D le disque unité ouvert dans $\mathbf{C}$. On note $\beta$ la fonction de $\mathbf{C}$ dans D définie par $\beta (z) =z/\overline{1 + |z|^2}$. C’est un homéomorphisme, dont l’inverse vérifie $\beta^{-1}(z) =z/\overline{1 - |z|^2}$ pour $z\in D$.

Soit $u\in \mathscr{L}(E)$. Il résulte des formules (2) et (3) de la proposition 1 de IV, p. 262 que $u=\beta^{-1}(b(u))$, et donc

$$
b(u) =\beta (u) \tag{5}
$$

#### Lemme 2 {#ts-iv-s5-lem-2 .statement tag=035G}

Soit X un espace topologique localement compact et soit $\mu$ une mesure positive sur X.

a) Soit $g$ une fonction $\mu$-mesurable sur X. L’opérateur de multiplication $m_g$ sur $L^2(X, \mu)$ est normal et $b(m_g) =m_{\beta\circ g}$;

b) Soit $h: X\rightarrow D$ une fonction $\mu$-mesurable. L’endomorphisme $m_h$ appartient à $\Omega (L^2(X, \mu))$ et $B(m_h) =m_{\beta^{-1}\circ h}$.

L’opérateur partiel $m_g$ est fermé à domaine dense. Comme $m^*_gm_g=$ $m_{\overline{g}}m_g=m_{|g|^2}$ (prop. 23 de IV, p. 253 et prop. 24 de IV, p. 255) on a

$$
W(m_g) =-R(m_{|g|^2},-1) =m_{(1+|g|^2)^{-1}}
$$

(prop. 22 de IV, p. 252). Cela implique

$$
b(m_g) =m_g\circ W(m_g)^{1/2}=m_g\circ m_{(1+|g|^2)^{-1/2}}=m_{\beta\circ g}
$$

d’après la formule (2) de IV, p. 262, le cor. de la prop. 6 de IV, p. 187 et le lemme 6 de IV, p. 254. Appliquant finalement la prop. 6 de IV, p. 187, on obtient l’assertion a).

Démontrons b). Comme $1- |h(x)|^2>0$ pour tout $x\in X$, on a $m_h\in$ $\Omega (L^2(X, \mu))$ (cor. de la prop. 6 de IV, p. 187). Puisque l’application $u\mapsto b(u)$ est injective (prop. 2 de IV, p. 264) et que les endomorphismes $b(B(m_h))$ et $b(m_{\beta^{-1}\circ h})$ sont égaux à $m_h$ d’après l’assertion a), on a bien $B(m_h) =m_{\beta^{-1}\circ h}$.

#### Théorème 1 (« Théorème spectral ») {#ts-iv-s5-thm-1 .statement tag=035H}

Soit $u$ un opérateur partiel normal sur l’espace hilbertien E. Il existe un espace topologique localement compact X, une mesure positive $\mu$ sur X, un isomorphisme isométrique $\theta$ de $L^2(X, \mu)$ sur E et une fonction continue $g$ sur X, tels que $u=\theta \circ m_g\circ \theta^{-1}$.

L’endomorphisme $b(u)$ de E est normal par définition. D’après le théorème spectral pour les endomorphismes normaux de E (corollaire 1 de IV, p. 193), il existe donc un espace topologique localement compact $\widetilde{X}$, une mesure positive $\mu$ sur $\widetilde{X}$, un isomorphisme isométrique $\widetilde{\theta}$ de $L^2(\widetilde{X}, \mu)$ sur E, et une fonction continue bornée $h$ sur $\widetilde{X}$, de sorte que $b(u)$ coïncide avec $\widetilde{\theta}\circ m_h\circ \widetilde{\theta}^{-1}$.

Soit N le sous-ensemble fermé des $x\in \widetilde{X}$ tels que $|h(x)|\geqslant 1$. Puisque l’endomorphisme $1-b(u)^*b(u) =\widetilde{\theta}\circ m_{1-|h|^2}\circ \widetilde{\theta}^{-1}$ est positif et injectif, l’ensemble N est localement $\mu$-négligeable (lemme 7 de IV, p. 186 et cor. de la prop. 6 de IV, p. 187). Posons alors $X =\widetilde{X}-$ N. C’est un espace localement compact, et la restriction des fonctions à X induit un isomorphisme isométrique de $L^2(\widetilde{X}, \mu)$ sur $L^2(X, \mu|X)$ (prop. 1 de IV, p. 179). La composition de $\widetilde{\theta}$ et de la restriction des fonctions à X induit donc un isomorphisme isométrique $\theta$ de $L^2(X, \mu|X)$ sur E. Comme $b(u) =\theta \circ m_{h|X}\circ \theta^{-1}$, il vient $u=\theta \circ m_{\beta^{-1}\circ(h|X)}\circ \theta^{-1}$ (lemme 2). Le théorème résulte de cette formule.

#### Lemme 3 {#ts-iv-s5-lem-3 .statement tag=035I}

Soit $u$ un opérateur partiel normal sur E. On a

Sp($b(u)$)$\cap D =\beta$(Sp($u$)).

On a $b(u) =u\circ W(u)^{1/2}$ (prop. 1 de IV, p. 262). L’endomorphisme $W(u)^{1/2}$ est injectif et son image est le domaine de $u$ (formule (1) de IV, p. 262).

Soit $\lambda \in \mathbf{C}$. Le nombre $\lambda$ appartient à l’ensemble résolvant de $u$ si et seulement si $(u-\lambda 1_E)\circ W(u)^{1/2}$ est une application linéaire bijective de E dans E (remarque 3 de IV, p. 245). Or, d’après la formule (3) de IV, p. 262, on a

$$
(u-\lambda 1_E)\circ W(u)^{1/2}=b(u)-\lambda (1_E-b(u)^*b(u))^{1/2}=f_{\lambda}(b(u))
$$

où $f_{\lambda}$ est la fonction continue définie sur D par $z\mapsto z-\lambda (1- |z|^2)^{1/2}$. L’endomorphisme $f_{\lambda}(b(u))$ est bijectif si et seulement si son spectre ne contient pas 0. Comme Sp($f_{\lambda}(b(u))$) $=f_{\lambda}$(Sp($b(u)$)) (cor. 2 de la prop. 7 de I, p. 111), c’est le cas si et seulement si 0 n’appartient pas à l’ensemble $f_{\lambda}$(Sp($b(u)$)). Ainsi, $\lambda \in$ Sp($u$) si et seulement s’il existe $z\in$ Sp($b(u)$)$\cap D$ tel que

$$
z-\lambda (1- |z|^2)^{1/2}= 0
$$

Cette égalité, si elle est valide, implique que $z\in D$, et signifie que que $\lambda =\beta^{-1}(z)$. On conclut que Sp($u$) $=\beta^{-1}$(Sp($b(u)$)$\cap D)$, comme énoncé.

Soit $u$ un opérateur partiel normal sur E. Soit $f\in \mathscr{K}$ (Sp($u$)). L’application $z\mapsto f(\beta^{-1}(z))$ de Sp($b(u)$)$\cap D$ dans $\mathbf{C}$ est continue et à support compact ; l’unique application $f_{\beta}$ de Sp($b(u)$) dans $\mathbf{C}$ qui la prolonge par zéro est donc continue.

#### Définition 3 {#ts-iv-s5-def-3 .statement tag=035J}

Pour toute fonction $f\in \mathscr{K}$ (Sp($u$)), on définit l’endomorphisme $f(u)$ de E par $f(u) =f_{\beta}(b(u))$.

L’application $f\mapsto f_{\beta}$ est un morphisme d’algèbres complexes de $\mathscr{K}$ (Sp($u$)) dans $\mathscr{C}$(Sp($b(u)$)), donc l’application $f\mapsto f(u)$ est un morphisme d’algèbres complexes de $\mathscr{K}$ (Sp($u$)) dans $\mathscr{L}(E)$. On a $\overline{f}(u) =f(u)^*$ puisque $\overline{f}_{\beta}=\overline{f_{\beta}}$. Si $f\geqslant 0$ alors $f_{\beta}\geqslant 0$, donc $f(u)$ est un endomorphisme positif de E.

#### Remarque {#ts-iv-s5-n2-rem-3 .statement tag=035K}

Supposons que $u$ est un endomorphisme normal de E, donc que Sp($u$) est une partie compacte de $\mathbf{C}$. Comme la bornification $b(u)$ coïncide avec $\beta (u)$ (formule (5)), et que Sp($b(u)$) $=\beta$(Sp($u$)) (cor. 2 de la prop. 7 de I, p. 111), le spectre de $b(u)$ est une partie compacte de D. Pour toute fonction continue $f\in \mathscr{C}$ (Sp($u$)), la fonction $f_{\beta}$ coïncide avec la restriction de $f\circ \beta^{-1}$ à Sp($u$). Par conséquent, $f_{\beta}(\beta (u))$ coïncide avec l’endomorphisme $f(u)$ défini par le calcul fonctionnel continu de $u$. La définition ci-dessus est donc compatible avec celle du calcul fonctionnel continu de l’algèbre stellaire $\mathscr{L}(E)$.

Soit $f\in \mathscr{K}$ (Sp($u$)). On a

$$
\|f(u)\|\leqslant \|f_{\beta}\|_{\infty}=\|f\|_{\infty}
$$

de sorte que, pour tous $x$ et $y$ dans E, on obtient la majoration $|\langle x|f(u)y\rangle |\leqslant \|x\| \|y\| \|f\|_{\infty}$. L’application $f\mapsto  \langle x|f(u)y\rangle$ est donc une mesure bornée sur Sp($u$), de masse totale $\leqslant \|x\|\|y\|$ (INT, IV, p. 154, § 4, n$^o7)$. Si $x=y$, c’est une mesure positive, puisque $f(u)$ est positif lorsque $f\geqslant 0$.

#### Définition 4 {#ts-iv-s5-def-4 .statement tag=035L}

Soit $u$ un opérateur partiel normal sur un espace hilbertien complexe E. Soient $x$ et $y$ dans E. La mesure bornée sur Sp($u$) définie par $f\mapsto  \langle x|f(u)y\rangle$ pour $f\in \mathscr{K}$ (Sp($u$)) s’appelle la mesure spectrale de $(x, y)$ relative à $u$. Lorsque $x=y$, on dit que c’est la mesure spectrale de $x$ relative à $u$.

#### Remarque 1 {#ts-iv-s5-n2-rem-1 .statement tag=035M}

Lorsque $u$ est continu, cette définition coïncide avec celle de la déf. 2 de IV, p. 190.

#### Remarque 2 {#ts-iv-s5-n2-rem-2 .statement tag=035N}

Soit $j$ l’inclusion canonique de Sp($u$) dans $\mathbf{C}$. Puisque Sp($u$) est fermé, l’application $j$ est $\mu$-propre pour toute mesure bornée $\mu$ sur Sp($u$) (INT, V, p. 68, § 6, n$^o1$, prop. 1). On identifiera souvent les mesures spectrales de $u$ avec les mesures sur $\mathbf{C}$ qui sont leurs images par $j($cf. INT, V, p. 84, § 7, n$^o2)$.

L’application de $E\times E$ dans l’espace de Banach $\mathscr{M}^1$(Sp($u$)) qui associe à $(x, y)$ la mesure spectrale de $(x, y)$ relative à $u$ est sesquilinéaire et continue de norme $\leqslant 1$.

#### Lemme 4 {#ts-iv-s5-lem-4 .statement tag=035O}

Soit X un espace topologique localement compact, soit $\mu$ une mesure positive sur X et soit $g$ une fonction $\mu$-mesurable sur X. Soit $m_g$ l’opérateur de multiplication par $g$ sur $L^2(X, \mu)$.

a) L’application $f\mapsto f(m_g)$ de $\mathscr{K}$ (Sp($m_g$)) dans $\mathscr{L}(L^2(X, \mu))$ est donnée par $f\mapsto m_{f\circ g}$;

b) Pour $f_1$ et $f_2$ dans $\mathscr{L}^2(X, \mu)$ de classes $\widetilde{f}_1$ et $\widetilde{f}_2$ dans $L^2(X, \mu)$, la mesure spectrale de $(\widetilde{f}_1,\widetilde{f}_2)$ relative à $m_g$ est la restriction à Sp($m_g$) de la mesure image $g(f_1f_2\cdot \mu)$.

L’opérateur partiel $m_g$ est normal et $b(m_g) =m_{\beta\circ g}=m_{g(1+|g|^2)^{-1/2}}$ (lemme 2). De plus $\beta (g(x))$ appartient à Sp($m_{\beta\circ g}$) pour tout $x$ en dehors d’un ensemble localement $\mu$-négligeable $Y\subset X$ (proposition 22 de IV, p. 252 et lemme 1 de IV, p. 181). Comme $f_{\beta}(\beta (g(x))) =f(g(x))$ pour tout $x\in X$ - Y, on en déduit que $f(m_g) =m_{f\circ g}$ d’après la définition 3 et le cor. de la prop. 6 de IV, p. 187.

Soient $f_1$ et $f_2$ dans $\mathscr{L}^2(X, \mu)$ de classes $\widetilde{f}_1$ et $\widetilde{f}_2$ dans $L^2(X, \mu)$. Puisque la mesure $\nu =f_1f_2\cdot \mu$ est bornée, la mesure image $g(\nu )$ est définie (INT, V, p. 69, § 6, n$^o1$, rem. 1). Soit $f\in \mathscr{K}$ (Sp($m_g$)). On a $f(m_g) =m_{f\circ g}$ d’après a), d’où

$$
\langle \widetilde{f}_1|f(m_g)\widetilde{f}_2\rangle =\int_X\overline{f}_1(f\circ g)f_2d\mu=\int_X(f\circ g) (\overline{f}_1f_2d\mu) =\int_{\mathbf{C}}f d\nu
$$

(INT, V, p. 69, § 6, n$^o1$, formule (1)), ce qui établit l’assertion b).

#### Exemple {#ts-iv-s5-n2-exa-1 .statement tag=035P}

Soit $n\in \mathbf{N}$. On munit $\mathbf{R}^n$ de la mesure de Lebesgue, et on identifie $\mathbf{R}^n$ et son groupe dual comme dans le corollaire 3 de II, p. 236. Notons N la norme euclidienne sur $\mathbf{R}^n$ et $\mathscr{F}$ la transformation de Fourier sur $\mathscr{S}(\mathbf{R}^n)$ et sur $\mathscr{S}'(\mathbf{R}^n)$ (n$^o12$ de IV, p. 217).

Soit $\Delta_{\mathscr{S}}$ l’opérateur partiel sur $L^2(\mathbf{R}^n)$ dont le domaine est l’espace $\mathscr{S}(\mathbf{R}^n)$ et qui vérifie

$$
\Delta_{\mathscr{S}}(\varphi ) =-\sum_{i=1}^n\partial_i^2\varphi
$$

pour tout $\varphi \in \mathscr{S}(\mathbf{R}^n)$. On a alors $\mathscr{F}(\Delta_{\mathscr{S}}(\varphi )) = 4\pi^2N^2\mathscr{F}(\varphi )$ pour toute fonction $\varphi \in \mathscr{S}(\mathbf{R}^n)$ (remarque 12 de IV, p. 220). Comme la transformation de Fourier est un automorphisme de $\mathscr{S}(\mathbf{R}^n)$ (prop. 18 de IV, p. 219), cela signifie que l’opérateur partiel $u=\mathscr{F}\circ \Delta_{\mathscr{S}}\circ \mathscr{F}^{-1}$ est la réduction de l’opérateur de multiplication $m_{4\pi^2N^2}$ à l’espace $\mathscr{S}(\mathbf{R}^n)$. L’opérateur partiel $u$ est fermable et symétrique ; sa fermeture est l’opérateur partiel auto-adjoint positif $m_{4\pi^2N^2}$ (prop. 6 de IV, p. 232, appliquée à l’espace $\mathscr{D}(\mathbf{R}^n)\subset \mathscr{S}(\mathbf{R}^n)$ à l’aide de la prop. 4 de IV, p. 202). Par conséquent, l’opérateur partiel $\Delta_{\mathscr{S}}$ est essentiellement auto-adjoint. On note Δ sa fermeture ; c’est un opérateur auto-adjoint positif, et c’est l’unique laplacien sur $\mathbf{R}^n($cf. exemple du n$^o6$ de IV, p. 243 et cor. de la prop. 26 de IV, p. 257).

D’après la prop. 21 de IV, p. 223, l’espace de Sobolev $H^2(\mathbf{R}^n)$ est l’ensemble des $f\in L^2(\mathbf{R}^n)$ tels que $(1 + N^2)\mathscr{F}(f)$ appartient à $L^2(\mathbf{R}^n)$, c’est-à-dire tels que $\mathscr{F}(f)$ appartient au domaine de $m_{4\pi^2N^2}$. Comme la transformation de Fourier est un isomorphisme isométrique de l’espace $L^2(\mathbf{R}^n)$ dans lui-même (th. 1 de II, p. 215), le domaine du laplacien Δ est $H^2(\mathbf{R}^n)$. On a $\Delta  =\mathscr{F}^{-1}\circ m_{4\pi^2N^2}\circ \mathscr{F}$. En particulier, le spectre de Δ est égal à $\mathbf{R}_+$.

### 3. Calcul fonctionnel universellement mesurable

Dans ce numéro les espaces hilbertiens considérés sont complexes.

Soit $u$ un opérateur partiel normal sur un espace hilbertien E. On note $\mu_{x,y}$ (resp. $\mu_y)$ la mesure spectrale de $(x, y)\in E\times E$ (resp. de $y)$ relative à $u$.

Soit $y\in E$. L’application $\mathscr{K}$ (Sp($u$))$\rightarrow E$ définie par $f\mapsto f(u)(y)$ vérifie

$$
\|f(u)(y)\|^2=\int|f|^2\mu_y=\|f\|^2_{\mathscr{L}^2(Sp(u),\mu_y)}
$$

Sp($u$)

Il existe donc une unique application linéaire isométrique ev$_y$ de l’espace $L^2$(Sp($u$)$, \mu_y)$ dans E telle que ev$_y(\widetilde{f}) =f(u)(y)$ si $\widetilde{f}$ est la classe d’une fonction $f\in \mathscr{K}$ (Sp($u$)).

Soit $f$ une fonction universellement mesurable définie sur le spectre de $u$. On note $D_f$ l’ensemble des éléments $y\in E$ tels que $f$ appartient à $\mathscr{L}^2$(Sp($u$)$, \mu_y)$.

#### Proposition 3 {#ts-iv-s5-prop-3 .statement tag=035Q}

Soit $f$ une fonction universellement mesurable définie sur le spectre de $u$. L’ensemble $D_f$ est un sous-espace vectoriel dense de E. L’application $y\mapsto$ ev$_y(f)$ est un opérateur partiel normal sur E dont le domaine est $D_f$, et qui est noté $f(u)$.

Pour tout $x\in E$ et tout $y\in D_f$, on a $f\in \mathscr{L}^1$(Sp($u$)$, \mu_{x,y})$ et

$$
\langle x|f(u)y\rangle =\int f \mu_{x,y} \tag{6}
$$

Sp($u$)

Nous allons démontrer l’énoncé plus précis suivant :

#### Proposition 4 {#ts-iv-s5-prop-4 .statement tag=035R}

Soit $f$ une fonction universellement mesurable dans le spectre de $u$.

a) L’ensemble $D_f$ est un sous-espace vectoriel dense de E. L’application $f(u) :y\mapsto$ ev$_y(f)$ de $D_f$ dans E est linéaire et coïncide avec $1_E$ si $f= 1$;

b) Soit $g\in \mathscr{L}_u$(Sp($u$)). Pour tout $y\in D_f$ et tout $x\in D_g$, on a $f g\in \mathscr{L}^1$(Sp($u$)$, \mu_{x,y})$, et

$$
\langle g(u)x|f(u)y\rangle =\int gf \mu_{x,y} \tag{7}
$$

Sp($u$)

c) Supposons que $E = L^2(X, \mu)$ où X est un espace topologique localement compact et $\mu$ une mesure positive sur X, et que $u=m_h$, où $h: X\rightarrow \mathbf{C}$ est $\mu$-mesurable. On a $f(m_h) =m_{f\circ h}$.

D’après le théorème 1 de IV, p. 266, on peut supposer être dans la situation de l’assertion c), c’est-à-dire que $E = L^2(X, \mu)$ et $u=m_h$, où X est un espace topologique localement compact, $\mu$ une mesure positive sur X et $h: X\rightarrow \mathbf{C}$ est $\mu$-mesurable. On notera $\widetilde{\varphi}$ la classe dans $L^2(X, \mu)$ d’une fonction $\varphi \in \mathscr{L}^2(X, \mu)$.

Soit S = Sp($m_h$). On note $\mu_{\widetilde{\varphi}_1,\widetilde{\varphi}_2}$ (resp. $\mu_{\widetilde{\varphi}})$ la mesure spectrale de $(\widetilde{\varphi}_1,\widetilde{\varphi}_2)$ (resp. de $\widetilde{\varphi})$ relative à $m_h$ pour tout $(\varphi_1, \varphi_2)\in \mathscr{L}^2(X, \mu)^2$ (resp. tout $\varphi \in \mathscr{L}^2(X, \mu))$.

Soit $\varphi \in \mathscr{L}^2(X, \mu)$. La mesure spectrale $\mu_{\widetilde{\varphi}}$ est égale à la mesure image $h(|\varphi |^2\cdot \mu)$ sur S (lemme 4 de IV, p. 269). Comme la fonction $f$ est $\mu_{\varphi}$-mesurable, on a $\varphi \in D_f$ si et seulement si les intégrales

$$
\int_S^*|f|^2d\mu_{\widetilde{\varphi}}=\int_S^*|f|^2h(|\varphi |^2d\mu) =\int_X^*|f\circ h|^2|\varphi |^2d\mu
$$

sont finies (INT, V, p. 70, § 6, n$^o2$, prop. 2). Cela signifie que $D_f$ est le domaine de l’opérateur de multiplication $m_{f\circ h}$, qui est un sous-espace dense dans E (prop. 5 de IV, p. 232).

La restriction de ev$_{\widetilde{\varphi}}$ aux classes de fonctions $g\in \mathscr{K}(S)$ est l’application qui à une classe $\widetilde{g}$ associe l’élément $g(m_h)(\widetilde{\varphi}) =m_{g\circ h}(\widetilde{\varphi})$ (lemme 4 de IV, p. 269). L’application ev$_{\varphi}$ coïncide donc avec l’application isométrique de $L^2(S, \mu_{\varphi})$ dans $L^2(X, \mu)$ déduite par passage aux quotients de l’application $g\widetilde{\mapsto}(g\circ h)\cdot \varphi$ de $\mathscr{L}^2(S, \mu_{\widetilde{\varphi}})$ dans $\mathscr{L}^2(X, \mu)$.

En particulier, on a donc ev$_{\varphi}(f) =m_{f\circ h}(\widetilde{\varphi})$, de sorte que l’application $f(m_h)$ de $D_f$ dans E coïnc$\widetilde{i}$de avec l’opérateur partiel $m_{f\circ h}$. Cela démontre l’assertion c) ; si $f= 1$, on trouve ev$_{\varphi}(1) =\widetilde{\varphi}$, ce qui conclut également la preuve de a).

Démontrons l’assertion b). Soient $\varphi_1$ et $\varphi_2$ des fonctions telles que $\widetilde{\varphi}_1\in D_f$ et $\widetilde{\varphi}_2\in D_g$. Il vient (INT, V, loc. cit.)

$$
\int_S^*|f g| |\mu_{\widetilde{\varphi}_1,\widetilde{\varphi}_2}|=\int_X^*|(f\circ h)(g\circ h)\varphi_1\varphi_2|d\mu
$$

$$
\leqslant \|(f\circ h)\varphi_1\| \|(g\circ h)\varphi_2\|
$$

qui est fini, donc $f g\in \mathscr{L}^1(S, \mu_{\widetilde{\varphi}_1,\widetilde{\varphi}_2})$. De plus, on a alors

$$
\langle g(m_h)(\widetilde{\varphi}_2)|f(m_h)(\widetilde{\varphi}_1)\rangle =\int_X\overline{(g\circ h) \varphi_2}(f\circ h)\varphi_1d\mu
$$

$$
=\int_Sgf d\mu_{\widetilde{\varphi}_1,\widetilde{\varphi}_2}
$$

ce qui conclut la démonstration.

#### Définition 5 {#ts-iv-s5-def-5 .statement tag=035S}

L’application $f\mapsto f(u)$ de $\mathscr{L}_u$(Sp($u$)) dans l’ensemble des opérateurs partiels normaux sur E définie par la prop. 3 de IV, p. 271 est appelée application de calcul fonctionnel universellement mesurable associée à $u$.

Plus généralement, soient T un ensemble et $g:$ Sp($u$)$\times T\rightarrow \mathbf{C}$ une application ; soit $t\in T$ tel que la fonction $g_t:z\mapsto g(z, t)$ est universellement mesurable sur Sp($u$). On note alors $g(u, t) =g_t(u)$.

La formule (7) implique en particulier que (8) $\|f(u)(y)\|^2=\int|f|^2\mu_y$

Sp($u$)

pour tout $f\in \mathscr{L}_u$(Sp($u$)) et tout $y\in D_f$. On en déduit en prenant $f= 1$ que $\mu_y$ est une mesure positive de masse totale $\|y\|^2$.

Si $u$ est un opérateur partiel normal sur un espace hilbertien E et $f\in \mathscr{K}$ (Sp($u$)), alors $D_f= E$ et l’opérateur partiel $f(u)$ est alors continu, puisque

$$
\|f(u)y\|\leqslant \|f\|_{\infty}\|y\|
$$

pour tout $y\in E$ d’après (8). L’endomorphisme $f(u)$ coïncide avec celui de la définition 3 de IV, p. 268.

#### Corollaire 1 {#ts-iv-s5-def-5-cor-1 .statement tag=035T}

a) Pour tout $f\in \mathscr{L}_u$(Sp($u$)), l’opérateur partiel $f(u)$ est normal et $f(u)^*=\overline{f}(u)$. De plus $f(u)$ est positif si $f\geqslant 0$, et auto-adjoint si $f$ est à valeurs réelles ;

b) Soient $k\in \mathbf{N}$ et $f(z) =z^k$ pour $z\in$ Sp($u$). On a $f(u) =u^k$;

c) Soient $\lambda \in \mathbf{C}-$ Sp($u$) et $f(z) = (\lambda -z)^{-1}$ pour $z\in$ Sp($u$). On a $f(u) = R(u, \lambda )$;

d) On a $\beta (u) =b(u)$;

e) Soient $f\in \mathscr{L}_u$(Sp($u$)) et $g\in \mathscr{L}_u$(Sp($u$)) tels que $|g|\leqslant 1 +|f|$. Le domaine de $g(u)$ est un cœur pour $f(u)$.

Au vu du théorème spectral (th. 1 de IV, p. 266), cela résulte de la proposition précédente combinée, respectivement, avec :

a) le lemme 2, a) de IV, p. 266, la prop. 23 de IV, p. 253, et son corollaire ;

b) la prop. 24, b) de IV, p. 255;

c) la prop. 22, b) de IV, p. 252;

d) le lemme 2, a) de IV, p. 266;

e) la prop. 6, b) de IV, p. 232.

#### Remarque {#ts-iv-s5-n3-rem-1 .statement tag=035U}

Pour $f=$ Id$_{Sp(u)}$, on a $f(u) =u$ (assertion b) pour $k= 1)$. Le domaine de $u$ coïncide donc avec l’ensemble des $x\in E$ tels que la fonction identité de Sp($u$) appartient à $\mathscr{L}^2$(Sp($u$)$, \mu_x)$; il contient en particulier les éléments $x\in E$ tels que la mesure $\mu_x$ est à support compact.

Le corollaire suivant généralise le cor. de la prop. 16 de IV, p. 247 et la prop. 17 de IV, p. 248.

#### Corollaire 2 {#ts-iv-s5-def-5-cor-2 .statement tag=035V}

Soit $u$ un opérateur partiel normal sur l’espace hilbertien E. On suppose que E est non nul.

a) Le spectre de $u$ est non vide;

b) Pour tout $\lambda \in \mathbf{C}-$ Sp($u$), la norme de la résolvante $R(u, \lambda )$ est égale à $1/\delta$, où $\delta  >0$ est la distance dans $\mathbf{C}$ de $\lambda$ au spectre de $u$.

c) Pour tout $\varepsilon  >$ 0, le $\varepsilon$-pseudo-spectre PSp$_{\varepsilon}(u)$ est l’ensemble des $\lambda \in \mathbf{C}$ à distance $< \varepsilon$ de Sp($u$).

Supposons que le spectre de $u$ est vide. Alors $u$ est injectif, et l’endomorphisme $u^{-1}=-R(u,0)$ est normal (cor. 1, c) et a)). On a Sp($u^{-1}$)$\subset  \{0\}$ (prop. 15, a)), donc Sp($u^{-1}$) $=\{0\}($I, p. 26, cor. 1). Puisque $u^{-1}$ est normal, cela implique que $u^{-1}= 0 ($I, p. 110, exemple 1), ce qui est une contradiction puisque E n’est pas nul.

Pour démontrer b), on peut supposer que $u$ est l’opérateur de multiplication $m_g$ sur $L^2(X, \mu)$, où $g$ est une fonction continue sur un espace topologique localement compact X muni d’une mesure positive $\mu$ (th. 1 de IV, p. 266). Soit $\lambda \in \mathbf{C}-$ Sp($u$) et $\delta  >0$ la distance de $\lambda$ au spectre de $u$. Pour démontrer que $\|R(u, \lambda )\|=\delta^{-1}$, on se ramène au cas $\lambda = 0$ en remplaçant $u$ par $u-\lambda 1_E$. Le nombre réel $\delta$ est alors la distance de 0 au spectre de $m_g$. Comme celui-ci coïncide avec l’image $\mu$-essentielle de $g$, le résultat est une conséquence du lemme 3 de IV, p. 182.

Finalement, l’assertion c) résulte de b) et de la définition de PSp$_{\varepsilon}(u)$ (IV, p. 250, déf. 9).

#### Corollaire 3 {#ts-iv-s5-def-5-cor-3 .statement tag=035W}

Soit $u$ un opérateur partiel normal sur un espace hilbertien E. Soit $f\in \mathscr{L}_u$(Sp($u$)). Pour tous $x$ et $y$ dans E, la mesure spectrale de $(x, y)$ relative à $f(u)$ est la mesure image $f(\mu)$, où $\mu$ est la mesure spectrale de $(x, y)$ relative à $u$.

Au vu du théorème spectral (th. 1 de IV, p. 266), on peut supposer que $u$ est l’opérateur de multiplication $m_g$ sur $L^2(X, \mu)$, où X est un espace topologique localement compact, $\mu$ une mesure positive sur X et $g\in \mathscr{C}(X)$. Soient $f_1$ et $f_2$ dans $\mathscr{L}^2(X, \mu)$ de classes $\widetilde{f}_1$ et $\widetilde{f}_2$ dans $L^2(X, \mu)$. Comme $f(m_g) =m_{f\circ g}$ (prop. 4, c)), la mesure spectrale de $(\widetilde{f}_1,\widetilde{f}_2)$ relative à $f(m_g)$ est la mesure image $(f\circ g)(f_1f_2\cdot \mu)$ (lemme 4, b) de IV, p. 269). Cette mesure est égale à la mesure image $f(g(f_1f_2\cdot \mu))$ (INT, V, p. 72, § 6, n$^o4$, prop. 4, a)), d’où l’assertion (lemme 4, b) de IV, p. 269).

#### Corollaire 4 {#ts-iv-s5-def-5-cor-4 .statement tag=035X}

Soit $g\in \mathscr{L}_u$(Sp($f(u)$)). On a $g(f(u)) = (g\circ f)(u)$.

On a $g\circ f\in \mathscr{L}_u$(Sp($u$)) (lemme 5 de IV, p. 184). Pour tous $x$ et $y$ dans E, notons $\mu'_{x,y}$ la mesure spectrale de $(x, y)$ relative à $f(u)$. D’après le corollaire précédent et INT, V, p. 71, § 6, n$^o2$, th. 1, on a $g\in \mathscr{L}^2$(Sp($f(u)$)$, \mu'_{x,y})$ si et seulement si $g\circ f\in \mathscr{L}^2$(Sp($u$)$, \mu_{x,y})$, de sorte que le domaine de $g(f(u))$ est égal au domaine de $(g\circ f)(u)$. Pour tous $x\in E$ et $y\in$ dom($g(f(u))$), on a alors la formule

$$
\langle x|g(f(u))y\rangle =\int g \mu'_{x,y}
$$

Sp($f(u)$)

$=\int g f(\mu_{x,y}) =\langle x|(g\circ f)y\rangle$

Sp($f(u)$)

(loc. cit.), d’où $g(f(u)) = (g\circ f)(u)$.

#### Proposition 5 {#ts-iv-s5-prop-5 .statement tag=035Y}

Soit $u$ un opérateur partiel normal sur un espace hilbertien E.

a) Si $f\in \mathscr{L}_u^{\infty}$(Sp($u$)), alors $f(u)\in \mathscr{L}(E)$;

b) Si $f\in \mathscr{L}_u^{\infty}$(Sp($u$)) et $g\in \mathscr{L}_u$(Sp($u$)), alors $f(u)\circ g(u)\subset (f g)(u)$;

c) L’application $f\mapsto f(u)$ de $\mathscr{L}_u^{\infty}$(Sp($u$)) dans $\mathscr{L}(E)$ est un morphisme unifère continu d’algèbres stellaires. En particulier, on a $\|f(u)\|\leqslant \|f\|_{\infty}$ pour $f\in \mathscr{L}_u^{\infty}$(Sp($u$));

d) Si $u\in \mathscr{L}(E)$, alors pour tout $f\in \mathscr{L}_u^{\infty}$(Sp($u$)), l’endomorphisme $f(u)$ appartient au bicommutant de $u$ dans $\mathscr{L}(E)$.

Soit $f\in \mathscr{L}_u^{\infty}$(Sp($u$)). On a $D_f= E$ et $f(u)$ est un endomorphisme continu de E d’après la formule (8), p. 272, d’où l’assertion a).

Soit $g\in \mathscr{L}_u$(Sp($u$)). Soit $y\in D_g$. On a $y\in D_{f g}$ et, pour tout $x\in E$, il vient $\langle f(u)x|g(u)y\rangle =\langle x|(f g)(u)y\rangle$ par la formule (7), p. 271, d’où $f(u)(g(u)y) = (f g)(u)(y)$, ce qui démontre b).

D’après a) et b), l’application $f\mapsto f(u)$ de $\mathscr{L}_u^{\infty}$(Sp($u$)) dans $\mathscr{L}(E)$ est un morphisme unifère d’algèbres involutives ; par conséquent, c’est un morphisme continu de norme $\leqslant 1$(I, p. 104, prop. 2), d’où l’assertion c).

Supposons que $u$ est un endomorphisme de E. Soit $v\in \mathscr{L}(E)$ permutable avec $u$. On a alors $v\circ f(u) =f(u)\circ v$ pour $f\in \mathscr{C}$ (Sp($u$)) d’après les propriétés du calcul fonctionnel continu (I, p. 110, remarque). Soient $x$ et $y$ dans E. Les formules

$$
\langle x|(v\circ f(u))y\rangle =\langle x|(f(u)\circ v)y\rangle \tag{9}
$$

valides pour toute fonction $f\in \mathscr{C}$ (Sp($u$)), signifient que les mesures spectrales de $(v^*(x), y)$ et de $(x, v(y))$ relatives à $u$ sont égales. Cette égalité implique d’après la formule (6), p. 271, que la formule (9) est valide pour tout $f\in \mathscr{L}_u^{\infty}$(Sp($u$)). On a donc $v\circ f(u) =f(u)\circ v$.

#### Corollaire {#ts-iv-s5-n3-cor-1 .statement tag=035Z}

Soient $f$ et $g$ dans $\mathscr{L}_u$(Sp($u$)) et $(x, y)\in D_f\times D_g$. La mesure spectrale de $(f(u)x, g(u)y)$ relative à $u$ est la mesure $f g\cdot \mu_{x,y}$, où $\mu_{x,y}$ est la mesure spectrale de $(x, y)$ relative à $u$.

Notons $\nu$ la mesure spectrale de $(f(u)x, g(u)y)$ relative à $u$. Pour toute fonction $\varphi \in \mathscr{K}$ (Sp($u$)), on a

$$
\int\varphi  \nu =\langle f(u)x|\varphi (u)(g(u)y)\rangle
$$

Sp($u$)

$=\langle f(u)x|(\varphi g)(u)y\rangle =\int f \varphi g \mu_{x,y}$,

Sp($u$)

(prop. 5, b)) d’où $\nu =f g\cdot \mu_{x,y}$.

#### Proposition 6 {#ts-iv-s5-prop-6 .statement tag=0360}

Soit $u$ un opérateur partiel normal sur un espace hilbertien E. Soit $(f_n)_{n\in\mathbf{N}}$ une suite dans $\mathscr{L}_u$(Sp($u$)) qui converge simplement vers $f\in \mathscr{L}_u$(Sp($u$)) et telle qu’il existe $g\in \mathscr{L}_u$(Sp($u$)) vérifiant $|f_n|\leqslant g$ pour tout $n\in \mathbf{N}$. On a alors dom($g(u)$)$\subset$ dom($f_n(u)$) pour tout $n\in \mathbf{N}$ et dom($g(u)$)$\subset$ dom($f(u)$). De plus, pour tout élément $y$ du domaine de $g(u)$, on a

$f(u)(y) =_{n\rightarrow}$lim$_{+\infty}f_n(u)(y)$.

En particulier, si $f_n\in \mathscr{L}_u^{\infty}$(Sp($u$)) pour tout $n\in \mathbf{N}$ et si les fonctions $f_n$ sont uniformément bornées, alors $f_n(u)$ converge vers $f(u)$ dans l’espace $\mathscr{L}(E)$ muni de la topologie de la convergence simple.

Notons $\mu_{x,y}$ (resp. $\mu_x)$ la mesure spectrale de $(x, y)$ (resp. de $x)$ relative à $u$.

Soit $y\in$ dom($g(u)$), de sorte que $g\in \mathscr{L}^2$(Sp($u$)$, \mu_y)$. La condition $|f_n|\leqslant g$ implique que $f_n\in \mathscr{L}^2$(Sp($u$)$, \mu_y)$, donc $y\in$ dom($f_n(u)$).

Comme $(f_n)$ converge simplement vers $f$ et que $|f_n|\leqslant g$, on a $f\in \mathscr{L}^2$(Sp($u$)$, \mu_y)$ d’après le théorème de Lebesgue (INT, IV, p. 137, § 3, n$^o7$, th. 6), donc $y\in$ dom($f(u)$). De plus, la suite $(f_n)$ converge vers $f$ dans $\mathscr{L}^2$(Sp($u$)$, \mu_y)$, donc la norme de $f_n(u)y$ converge vers la norme de $f(u)y$.

Soit $x\in E$. Les fonctions $f$ et $g$, ainsi que les fonctions $f_n$ pour tout $n\in \mathbf{N}$, appartiennent à $\mathscr{L}^1$(Sp($u$)$, \mu_{x,y})$ (prop. 3). D’après le théorème de Lebesgue (INT, IV, loc. cit.), la suite $(f_n)$ converge vers $f$ dans $\mathscr{L}^1$(Sp($u$)$, \mu_{x,y})$, d’où

$$
\langle x|f_n(u)y\rangle =\int f_n\mu_{x,y}\rightarrow \int f \mu_{x,y}=\langle x|f(u)y\rangle
$$

Sp($u$) Sp($u$)

On en conclut que $f_n(u)(y)$ converge vers $f(u)(y)$ (EVT, V, p. 17, prop. 10).

#### Proposition 7 {#ts-iv-s5-prop-7 .statement tag=0361}

Soient X un espace topologique localement compact et $\nu$ une mesure sur X. Soit $g:\mathbf{C}\times X\rightarrow \mathbf{C}$ une fonction continue à support compact. Pour $z\in \mathbf{C}$, posons

$$
h(z) =\int_Xg(z, x)d\nu (x)
$$

a) L’application $h$ de $\mathbf{C}$ dans $\mathbf{C}$ est continue et bornée;

b) L’application de X dans $\mathscr{L}(E)$ définie par $x\mapsto g(u, x)$ est $\nu$-intégrable et on a

$$
h(u) =\int_Xg(u, x)d\nu (x)
$$

La fonction $h$ est bornée car $g$ est continue à support compact, et elle est continue d’après INT, IV, p. 144, § 4, n$^o3$, cor. 1. Comme $g$ est continue et à support compact, l’application $x\mapsto g(u, x)$ est continue de X dans $\mathscr{L}(E)$ (TG, X, p. 28, th. 3 et prop. 5, c)). Cette application est à support compact, donc bornée et intégrable sur X par rapport à $\nu$. Notons

$$
v=\int_Xg(u, x)d\nu (x)\in \mathscr{L}(E)
$$

Soient $y$ et $z$ des éléments de E et $\mu$ la mesure spectrale de $(y, z)$ relative à $u$. On a

$$
\langle y|v(z)\rangle =\int\langle y|g(u, x)z\rangle d\nu (x) =\int\int g(\lambda , x)d\mu(\lambda )d\nu (x)
$$

X X Sp($u$)

(formule (6), p. 271). Puisque $g\in \mathscr{K}(\mathbf{C}\times X)$, il vient

$$
\langle y|v(z)\rangle =\int_{Sp(u)}\int_Xg(\lambda , x)d\nu (x)d\mu(\lambda ) =\langle y|h(u)z\rangle
$$

d’après INT, III, p. 84, § 4, n$^o1$, th. 2 et la formule (6), p. 271. Cela démontre que $v=h(u)$, comme désiré.

### 4. Projecteurs spectraux

Soit $u$ un opérateur partiel normal sur un espace hilbertien complexe E. Soient A une partie universellement mesurable de Sp($u$) et $\varphi_A$ sa fonction caractéristique. Comme $\varphi_A$ est bornée et vérifie $\varphi^2_A=\varphi_A$, l’endomorphisme $\varphi_A(u)$ de E est un orthoprojecteur de E. Il est appelé le projecteur spectral de $u$ défini par A. On note $p_A=\varphi_A(u)$. On a $p_{\emptyset}= 0$ et $p_{Sp(u)}= 1_E$.

Soit A une partie universellement mesurable de $\mathbf{C}$. Le projecteur spectral de $u$ défini par A est le projecteur spectral $p_{Sp(u)\cap A}$. Il est aussi noté simplement $p_A$. Pour toute fonction $f\in \mathscr{L}_u$(Sp($u$)), tout $x\in E$ et tout $y\in$ dom($f(u)$), on a la formule

$$
\langle p_A(x)|f(u)y\rangle =\int f d\mu \tag{10}
$$

Sp($u$)$\cap A$

où $\mu$ est la mesure spectrale de $(x, y)$ relative à $u$ (formule (7), p. 271).

Soient A et B des parties universellement mesurables de Sp($u$). Comme $\varphi_A\varphi_B=\varphi_{A\cap B}$, on a $p_A\circ p_B=p_{A\cap B}$ (prop. 5 de IV, p. 275, c)). En particulier, si A et B sont disjointes, les images de $p_A$ et de $p_B$ sont orthogonales.

#### Proposition 8 {#ts-iv-s5-prop-8 .statement tag=0362}

Soit $(A_i)_{i\in I}$ une famille dénombrable de parties universellement mesurables deux à deux disjointes de Sp($u$) et $p_i$ le projecteur spectral de $u$ défini par $A_i$. La réunion A des ensembles $A_i$ est une partie universellement mesurable de Sp($u$) et la série $\sum_ip_i$ converge vers $p_A$ dans $\mathscr{L}(E)$ muni de la topologie de la convergence simple.

L’ensemble A est universellement mesurable d’après INT, IV, p. 177, § 5, n$^o4$, cor. 2. La série $\sum_i\varphi_{A_i}$ converge simplement vers $\varphi_A$ et ses sommes partielles sont bornées par 1. L’assertion résulte donc de la prop. 6 de IV, p. 276.

#### Proposition 9 {#ts-iv-s5-prop-9 .statement tag=0363}

Soit A une partie fermée de Sp($u$). Soit $\varphi_A$ la fonction caractéristique de A et $p_A=\varphi_A(u)$ le projecteur spectral de $u$ défini par A. Notons $E_A$ l’image de $p_A$. C’est un sous-espace fermé de E.

a) Le sous-espace $E_A$ est l’espace des $x\in E$ tels que le support de la mesure spectrale de $x$ relative à $u$ est contenu dans A ;

b) Si A est borné dans $\mathbf{C}$, alors $E_A$ est contenu dans le domaine de $u$;

c) Pour tout $x$ appartenant au domaine de $u$, on a $p_A(x)\in$ dom($u$) et $u(p_A(x))\in E_A$, en particulier $u(x)\in E_A$ si $x\in$ dom($u$)$\cap E_A$.

Pour $x$ dans E, on note $\mu_x$ la mesure spectrale de $x$ relative à $u$.

Démontrons a). Soit $x$ un élément de $E_A$. Soient $z\in \mathbf{C}-$ A et U un voisinage ouvert relativement compact de $z$ qui ne rencontre pas A. Pour toute fonction $f\in \mathscr{K}(\mathbf{C})$ à support contenu dans U, on a

$$
\int f \mu_x=\langle x|f(u)x\rangle =\langle p_A(x)|f(u)x\rangle =\int f \mu_x= 0
$$

Sp($u$) Sp($u$)$\cap A$ d’après la formule (10). Cela signifie que $z$ n’appartient pas au support de $\mu_x$. Par conséquent, le support de $\mu_x$ est contenu dans A.

Réciproquement, soit $x\in E$ tel que le support de $\mu_x$ est contenu dans A. Il vient

$$
\langle x|p_A(x)\rangle =\int\mu_x=\int\mu_x=\langle x|x\rangle
$$

Sp($u$)$\cap A$ Sp($u$)

(loc. cit.) donc $\|p_A(x)-x\|^2=\|p_A(x)\|^2- \|x\|^2\leqslant 0$ et par conséquent $p_A(x) =x$, c’est-à-dire $x\in E_A$.

L’assertion b) résulte de a) et de la remarque de IV, p. 273.

Démontrons c). Le domaine de $u$ est l’ensemble des $x\in E$ tels que la fonction identique de Sp($u$) appartient à $\mathscr{L}^2$(Sp($u$)$, \mu_x) ($loc. cit.). Comme $\mu_{p_A(x)}=\varphi_A\cdot \mu_x$ pour $x\in E$ (cor. de la prop. 5 de IV, p. 275), on a $p_A(x)\in$ dom($u$) si $x\in$ dom($u$).

Soit $x\in$ dom($u$) et $y=p_A(x)$; on a $y\in$ dom($u$)$\cap E_A$ d’après c). La mesure spectrale de $u(y)$ relative à $u$ est $|$Id$_{Sp(u)}|^2\cdot \mu_y($loc. cit.). Puisque $\mu_y$ est à support dans A, il en est de même de $\mu_{u(y)}$, donc $u(y)\in E_A$ d’après a).

#### Corollaire {#ts-iv-s5-n4-cor-1 .statement tag=0364}

Soit $\lambda \in$ Sp($u$). L’image de $p_{\{\lambda\}}$ est le sous-espace propre de $u$ relatif à $\lambda$.

Soit $x\in$ dom($u$). Notons $\mu$ (resp. $\nu )$ la mesure spectrale de l’élément $x$ relative à $u$ (resp. la mesure spectrale de $(x, u(x))$ relative à $u)$. On a $\nu =$ Id$_{Sp(u)}\cdot \mu$ (cor. de la prop. 5 de IV, p. 275). Si $u(x) =\lambda x$, on a également $\nu =\lambda \mu$, d’où l’égalité Id$_{Sp(u)}\cdot \mu=\lambda \mu$. Celle-ci implique que le support de $\mu$ est contenu dans $\{\lambda \}($cf. INT, V, p. 46, § 5, n$^o3$, cor. 2) et donc $x$ appartient à l’image de $p_{\{\lambda\}}$ (prop. 9, a)).

Réciproquement, supposons que $x$ appartient à l’image $E_{\lambda}$ de $p_{\{\lambda\}}$. Alors $x$ appartient à dom($u$) et $u(x)$ appartient aussi à $E_{\lambda}($loc. cit., b)). Puisque $\varphi_{\{\lambda\}}\cdot$ (Id$_{Sp(u)}-\lambda ) = 0$, on a la relation $p_{\{\lambda\}}\circ (u-\lambda 1_E)\subset 0$ (prop. 5 de IV, p. 275, c)), d’où $0 =p_{\{\lambda\}}(u(x))-\lambda p_{\{\lambda\}}(x) =u(x)-\lambda x$.

#### Proposition 10 {#ts-iv-s5-prop-10 .statement tag=0365}

Soit $\lambda \in \mathbf{C}$. On a $\lambda \in$ Sp($u$) si et seulement si, pour tout voisinage ouvert V de $\lambda$ dans $\mathbf{C}$, le projecteur spectral $p_V$ de $u$ relatif à V est non nul.

Si $\lambda  /\in$ Sp($u$), alors il existe un voisinage ouvert V de $\lambda$ dans $\mathbf{C}$ qui ne rencontre pas Sp($u$), et alors $p_V=p_{\emptyset}= 0$.

Réciproquement, supposons qu’il existe un voisinage ouvert V de $\lambda$ dans $\mathbf{C}$ tel que $p_V= 0$. Soit $c >0$ tel que le disque de centre $\lambda$ et de rayon $c$ est contenu dans V.

Soit $x\in$ dom($u$) et soit $\mu_x$ la mesure spectrale de $x$ relative à $u$. Comme $\mu_x(V) =\langle x|p_V(x)\rangle = 0$, on calcule

$$
\int_{\mathbf{C}}|z-\lambda |^2d\mu_x(z) =\int_{\mathbf{C}-V}|z-\lambda |^2d\mu_x(z)
$$

$$
\geqslant c^2\int_{\mathbf{C}-V}d\mu_x(z) =c^2\int_{\mathbf{C}}d\mu_x(z) =c^2\|x\|^2
$$

Mais, par ailleurs, on a

$$
\|u(x)-\lambda x\|^2=\int_{\mathbf{C}}|z-\lambda |^2d\mu_x(z) =\|u^*(x)-\lambda x\|^2
$$

(formule (8), p. 272), d’où $\|u(x)-\lambda x\|\geqslant c\|x\|$ et $\|u^*(x)-\lambda x\|\geqslant c\|x\|$. Il en résulte que $\lambda$ appartient à l’ensemble résolvant de $u$ (lemme 5 de IV, p. 248). Cela conclut la démonstration.

#### Corollaire {#ts-iv-s5-n4-cor-2 .statement tag=0366}

Soient A un ouvert dans $\mathbf{C}$ et $n\in \mathbf{N}$. Si A contient $n$ éléments de Sp($u$), alors la dimension de l’image du projecteur spectral $p_A$ de $u$ relatif à A est au moins égale à $n$.

Soient $\lambda_1, . . .,\lambda_n$ des éléments distincts du spectre de $u$ appartenant à A. Il existe une famille $(V_i)_{1\leqslant i\leqslant n}$ d’ouverts deux à deux disjoints de $\mathbf{C}$ tels que $\lambda_i\in V_i$ pour $1\leqslant i\leqslant n$. Soit B l’union des ensembles $V_i$. L’image de $p_A$ contient l’image du projecteur spectral $p_B$; comme de plus $p_B$ est la somme des projecteurs $p_{V_i}$, et comme l’image de $p_{V_i}$ est orthogonale à l’image de $p_{V_j}$ pour tous $i\not =j$, le résultat découle de la prop. 10.

### 5. La formule de Helffer–Sjöstrand

Dans ce numéro, E désigne un espace hilbertien complexe. Nous allons obtenir une formule pour certains cas du calcul fonctionnel d’un opérateur partiel auto-adjoint qui s’exprime directement en fonction de la résolvante de l’opérateur concerné.

On munit $\mathbf{R}$ (resp. $\mathbf{C})$ de la mesure de Lebesgue, notée $\mu$, et on identifie le groupe $\mathbf{R}$ et son groupe dual par l’application $(x, y)\mapsto$ exp(2$i\pi xy) ($cf. corollaire 3 de II, p. 236).

Pour toute fonction $f$ définie et différentiable sur un ouvert U de $\mathbf{R}^2$, identifié à $\mathbf{C}$, avec coordonnées réelles $x$ et $y$, on note

$\partial f$ 1 $\partial f\partial f$

= $+i$

$\partial z$ 2 $\partial x\partial y$ (cf. VAR, R2, 8.8.10, p. 24).

#### Lemme 5 {#ts-iv-s5-lem-5 .statement tag=0367}

Soit $f\in \mathscr{D}(\mathbf{R})$. Il existe une fonction $\widetilde{f}$ dans $\mathscr{D}(\mathbf{C})$ qui coïncide avec $f$ sur $\mathbf{R}$ et vérifie

$$
\partial \widetilde{f}
$$

$$
(x,0) = 0 \tag{11}
$$

$$
\partial z
$$

pour tout $x\in \mathbf{R}$. On a alors

$$
\partial \widetilde{f}'
$$

$$
(x,0) =if(x) \tag{12}
$$

$$
\partial y
$$

pour tout $x\in \mathbf{R}$ et il existe un nombre réel $C\geqslant 0$ tel que

$$
\partial \widetilde{f}
$$

$$
(x, y)\leqslant C|y| \tag{13}
$$

$$
\partial z
$$

pour tout $(x, y)\in \mathbf{R}^2$.

Il existe $\varphi \in \mathscr{D}(\mathbf{R})$ dont le support est contenu dans $[-2,2]$ et qui est égale à 1 sur $[-1,1]$ (lemme 1 de IV, p. 196). Posons

$$
\widetilde{f}(x, y) =f(x) +iyf'(x)\varphi (y)
$$

pour $(x, y)\in \mathbf{R}^2$. On a $\widetilde{f}\in \mathscr{D}(\mathbf{C})$ et $\widetilde{f}$ coïncide avec $f$ sur $\mathbf{R}$. De plus, quel que soit $(x, y)\in \mathbf{R}^2$, il vient

$\partial \widetilde{f}$ 1 $''''$

$$
(x, y) =(if(x)-yf(x))\varphi (y) +iyf(x)\varphi (y)
$$

$\partial z$ 2

Comme la fonction $\varphi$ est égale à 1 au voisinage de 0, on a $\varphi '(0) = 0$, d’où (11).

Soit $\widetilde{f}$ dans $\mathscr{D}(\mathbf{C})$ vérifiant (11). La formule (12) en découle, et la majoration (13) est obtenue à l’aide du théorème des accroissements finis (FVR, I, p. 23, th. 2).

On dit que $\widetilde{f}$ est une extension presque analytique de $f$.

#### Lemme 6 {#ts-iv-s5-lem-6 .statement tag=0368}

Soit $\varepsilon  >0$. La fonction $\sigma_{\varepsilon}$ définie sur $\mathbf{R}$ par

$$
2i\varepsilon x
$$

$$
\sigma_{\varepsilon}(x) =
$$

$$
x^2+\varepsilon^2
$$

appartient à $L^2(\mathbf{R})$. Sa transformée de Fourier est la classe dans $L^2(\mathbf{R})$ de la fonction $\eta_{\varepsilon}$ qui est nulle en 0 et vérifie

$$
2\pi \varepsilon y_{-2\pi \varepsilon|y|}
$$

$$
\eta_{\varepsilon}(y) =e
$$

$$
|y|
$$

pour tout $y\not = 0$.

On a $\sigma_{\varepsilon}\in L^2(\mathbf{R})$ d’après la prop. 3 de IV, p. 199, et la classe de la fonction $\eta_{\varepsilon}$ appartient à $L^2(\mathbf{R})\cap L^1(\mathbf{R})$. Pour tout $x\in \mathbf{R}$, on a

$$
\overline{\mathscr{F}}(\eta_{\varepsilon})(x) = 2\pi \varepsilon \int_{\mathbf{R}_+}e^{2\pi(ix-\varepsilon)y}dy-2\pi \varepsilon \int_{\mathbf{R}_-}e^{2\pi(ix+\varepsilon)y}dy
$$

$$
\varepsilon \varepsilon 2i\varepsilon x
$$

= $-$ =,

$$
\varepsilon -ix\varepsilon +ixx^2+\varepsilon^2
$$

d’où $\overline{\mathscr{F}}(\eta_{\varepsilon}) =\sigma_{\varepsilon}$. Le résultat découle alors de la formule d’inversion de Fourier dans $L^2(\mathbf{R})$ (corollaire du théorème 2 de II, p. 220).

#### Lemme 7 {#ts-iv-s5-lem-7 .statement tag=0369}

Soit $f\in \mathscr{D}(\mathbf{R})$ et soit $\widetilde{f}\in \mathscr{D}(\mathbf{C})$ une extension presque analytique de $f$. Pour $\varepsilon  >0$, définissons $f_{\varepsilon}$ sur $\mathbf{R}$ par

1 $\int\widetilde{f}(y+i\varepsilon )\widetilde{f}(y-i\varepsilon )$

$$
f_{\varepsilon}(x) =--dy
$$

$$
2i\pi_{\mathbf{R}}y-x+i\varepsilon y-x-i\varepsilon
$$

Alors $f_{\varepsilon}$ est continue et bornée, et $f_{\varepsilon}$ converge vers $f$ dans $\mathscr{C}_b(\mathbf{R})$ quand $\varepsilon$ tend vers 0.

La continuité de $f_{\varepsilon}$ est conséquence de INT, IV, p. 144, § 4, n$^o3$, cor. 1, puisque $\widetilde{f}$ est à support compact. De plus, si $r$ est tel que le support de $\widetilde{f}$ est contenu dans $[-r, r]\times \mathbf{R}$, on a

$\int^r$ 1 $4r$

$|f_{\varepsilon}(x)|\leqslant 2\|\widetilde{f}\|_{\infty}$ 2 $_2dy\leqslant \|\widetilde{f}\|_{\infty}$,

$$
_{-r}(x-y)+\varepsilon \varepsilon
$$

donc $f_{\varepsilon}$ est bornée.

Le développement de Taylor à l’ordre 1 (FVR, I, p. 30, prop. 3) et la formule (13) démontrent qu’il existe $M\geqslant 0$ et une fonction $\varrho_1$ sur $\mathbf{R}^2$ tels que

$\widetilde{f}(y+i\gamma ) =f(y) +i\gamma f'(y) +\gamma^2\varrho_1(y;\gamma )$, et $|\varrho_1(y;\gamma )|\leqslant M$,

pour tout $y\in \mathbf{R}$ et $\gamma \in \mathbf{R}$. Comme l’application $y\mapsto \widetilde{f}(y+i\gamma )$ est à support contenu dans $[-r, r]$ pour tout $\gamma \in \mathbf{R}$, l’application $y\mapsto \varrho_1(y;\gamma )$ est à support contenu dans $[-r, r]$, pour tout $\gamma \in \mathbf{R}$.

Soit $g_{\varepsilon}$ la fonction définie sur $\mathbf{R}^2$ par

$$
\widetilde{f}(y+i\varepsilon )\widetilde{f}(y-i\varepsilon )
$$

$$
g_{\varepsilon}(x, y) =-
$$

$$
y-x+i\varepsilon y-x-i\varepsilon
$$

Pour tout $(x, y)\in \mathbf{R}^2$ et $\varepsilon  >0$, on obtient

$$
2i\varepsilon 2i\varepsilon (y-x)'
$$

$$
g_{\varepsilon}(x, y) =-f(y) +f(y)
$$

$$
(x-y)^2+\varepsilon^2(x-y)^2+\varepsilon^2
$$

$$
_2\varrho_1(y;\varepsilon )\varrho_1(y;-\varepsilon )
$$

$$
+\varepsilon -
$$

$$
y-x+i\varepsilon y-x-i\varepsilon
$$

Soient $x\in \mathbf{R}$ et $\varepsilon  >0$. On a

$$
_2\int\varrho_1(y;\varepsilon )\varrho_1(y;-\varepsilon )2\int^rdy
$$

$$
\varepsilon -dy\leqslant 2M\varepsilon
$$

$$
_{\mathbf{R}}y-x+i\varepsilon y-x-i\varepsilon -_r\overline{(x-y)^2 + \varepsilon^2}
$$

$$
\leqslant 4Mr\varepsilon
$$

Par conséquent, pour tout $x\in \mathbf{R}$, il vient

1 $\int$ 1 $'$

$$
f_{\varepsilon}(x) =-g_{\varepsilon}(x, y)dy= (f*\delta_{\varepsilon})(x)-(f*\sigma_{\varepsilon})(x) +k_{\varepsilon}(x)
$$

$$
2i\pi_{\mathbf{R}}2i\pi
$$

où $\delta_{\varepsilon}$ et $\sigma_{\varepsilon}$ sont les fonctions sur $\mathbf{R}$ définies par

1 $\varepsilon 2i\varepsilon x$

$$
\delta_{\varepsilon}(x) =_{22},\sigma_{\varepsilon}(x) =_{22}
$$

$$
\pi x+\varepsilon x+\varepsilon
$$

et $\|k_{\varepsilon}\|_{\infty}\leqslant 2Mr\varepsilon$.

La fonction $\mathscr{F}(f')\in \mathscr{S}(\mathbf{R})$ est intégrable (prop. 18 de IV, p. 219 et prop. 13 de IV, p. 213). D’après le lemme 6, il vient

$$
\int_{\mathbf{R}}|\mathscr{F}(f')(y)\mathscr{F}(\sigma_{\varepsilon})(y)|dy= 2\pi \varepsilon \int_{\mathbf{R}}|\mathscr{F}(f')(y)|e^{-2\pi \varepsilon|y|}dy
$$

$$
\leqslant 2\pi \varepsilon \int_{\mathbf{R}}|\mathscr{F}(f')(y)|dy
$$

donc $\mathscr{F}(f')\mathscr{F}(\sigma_{\varepsilon})$ converge vers 0 dans $L^1(\mathbf{R})$ quand $\varepsilon$ tend vers 0. Comme $f'$ et $\sigma_{\varepsilon}$ appartiennent à $L^2(\mathbf{R})$, la prop. 14 de II, p. 223 implique que $f'*\sigma_{\varepsilon}=\overline{\mathscr{F}}(\mathscr{F}(f')\mathscr{F}(\sigma_{\varepsilon}))$ converge vers 0 dans $\mathscr{C}_b(\mathbf{R})$.

Pour tout $\varepsilon  >0$, la mesure positive $\delta_{\varepsilon}\cdot dx$ sur $\mathbf{R}$ est de masse totale 1 (cf. FVR, III, p. 7). L’ensemble des mesures $\delta_{\varepsilon}\cdot dx$ pour $\varepsilon  >0$ et le filtre induit sur cet ensemble par le filtre des voisinages de 0 dans $\mathbf{R}_+^*$ vérifient les hypothèses du lemme 4 de INT, VIII, p. 137, § 2, n$^o7$. Les mesures $\delta_{\varepsilon}\cdot dx$ convergent donc dans $\mathscr{M}^1(\mathbf{R})$ vers la mesure ponctuelle $\varepsilon_0$ quand $\varepsilon$ tend vers 0. Il vient $f*\delta_{\varepsilon}\rightarrow f$ dans $\mathscr{C}_b(\mathbf{R})$ (INT, VIII, p. 163, § 4, n$^o4)$. Le lemme est démontré.

On note $\mu$ la mesure de Lebesgue sur $\mathbf{C}$.

#### Théorème 2 (Helffer–Sjöstrand) {#ts-iv-s5-thm-2 .statement tag=036A}

Soit $u$ un opérateur partiel auto-adjoint sur E. Soient $f\in \mathscr{D}(\mathbf{R})$ et $\widetilde{f}\in \mathscr{D}(\mathbf{C})$ une extension presque analytique de $f$. Soit $h$ l’application de $\mathbf{C}$ dans $\mathscr{L}(E)$ définie par

$$
\partial \widetilde{f}
$$

$$
h(\lambda ) =(\lambda )R(u, \lambda )
$$

$$
\partial z
$$

si $\lambda \in \mathbf{C}-\mathbf{R}$ et $h(\lambda ) = 0$ si $\lambda \in \mathbf{R}$. Alors $h$ est $\mu$-intégrable sur $\mathbf{C}$ et

$$
1\int
$$

$$
f(u) =-h(\lambda )d\mu(\lambda )
$$

$$
\pi_{\mathbf{C}}
$$

L’application $h$ est mesurable et son support est compact. Comme $u$ est auto-adjoint, on a $\|R(u, \lambda )\|\leqslant |\mathscr{I}(\lambda )|^{-1}$ pour tout $\lambda \in \mathbf{C}-\mathbf{R}$ (prop. 17 de IV, p. 248). L’application $h$ est donc bornée d’après la formule (13), et par conséquent elle est intégrable sur $\mathbf{C}$.

Soit $\varepsilon \in \mathbf{R}^*_+$. On note $F^+_{\varepsilon}$ (resp. $F^-_{\varepsilon})$ l’ensemble fermé dans $\mathbf{C}$ des $\lambda \in \mathbf{C}$ tels que $\mathscr{I}(\lambda )\geqslant \varepsilon$ (resp. $\mathscr{I}(\lambda )\leqslant -\varepsilon )$. On a

$\int_{\mathbf{C}}h(\lambda )d\mu(\lambda ) =$ lim$_{\varepsilon\rightarrow 0}\int_{F^+_{\varepsilon}}h(\lambda )d\mu(\lambda ) +\int_{F^-_{\varepsilon}}h(\lambda )d\mu(\lambda )$.

Soit $r >0$ tel que le support de $h$ est contenu dans $C = [-r, r]^2$. Notons $R_{\varepsilon}^+$ le pavé $[-2r,2r]\times [\varepsilon ,2r]$ dans $\mathbf{C}$. C’est une partie localement polyédrale de $\mathbf{C}$ (VAR, R2, 11.3, p. 48). Elle vérifie les conditions suivantes :

(i) On a $R^+_{\varepsilon}\subset 2C\cap F^+_{\varepsilon}$;

(ii) L’ensemble $R^+_{\varepsilon}$ contient l’intersection de $F^+_{\varepsilon}$ et du support de $h$;

(iii) Le bord régulier $\partial R^+_{\varepsilon}$ (VAR, R2, 11.3.2, p. 49) contient le segment $S_{\varepsilon}= [-r, r] +i\varepsilon \subset \mathbf{C}$;

(iv) On a $h(\lambda ) = 0$ si $\lambda \in \partial R_{\varepsilon}^+-S_{\varepsilon}$.

Notons $d\lambda$ (resp. $d\lambda )$ la forme différentielle de degré 1 sur $\mathbf{C}$ différentielle de l’application identité de $\mathbf{C}$ (resp. de la conjugaison complexe). Notons $g$ la fonction sur $\mathbf{C}-\mathbf{R}$ à valeurs dans $\mathscr{L}(E)$ telle que $g(\lambda ) =\widetilde{f}(\lambda )R(u, \lambda )$ pour $\lambda \in \mathbf{C}-\mathbf{R}$. Soit $\omega =g d\lambda$; c’est une forme différentielle de degré 1 sur $\mathbf{C}-\mathbf{R}$, à support compact et à valeurs dans $\mathscr{L}(E)$. Puisque la résolvante de $u$ est holomorphe (prop. 14 de IV, p. 246), on a

$$
\partial \widetilde{f}\partial
$$

$$
d\omega =(\lambda )R(u, \lambda ) +\widetilde{f}(\lambda )R(u, \lambda )d\lambda \wedge d\lambda =-h(\lambda )d\lambda \wedge d\lambda
$$

$$
\partial z\partial z
$$

La mesure vectorielle associée à $d\omega$ (VAR, R2, 10.4.3, p. 43) est la mesure de densité $-2ih$ par rapport à la mesure de Lebesgue. En appliquant la formule de Stokes à l’ensemble localement polyédral $R_{\varepsilon}^+$ et à la forme différentielle $\omega$ (VAR, R2, 11.3.4, p. 49), on obtient donc

$$
i\int i\int i\int i\int^r
$$

$$
d\omega =\omega =\omega =\widetilde{f}(y+i\varepsilon )R(u, y+i\varepsilon )dy
$$

2 $_{R^+_{\varepsilon}}$ 2 $_{\partial R^+_{\varepsilon}}$ 2 $_{S_{\varepsilon}}$ 2 $_{-r}$

d’où

$$
\int i\int
$$

$$
h(\lambda )d\mu(\lambda ) =-\widetilde{f}(y+i\varepsilon )R(u, y+i\varepsilon )dy
$$

$_{F^+_{\varepsilon}}$ 2 $_{\mathbf{R}}$

En raisonnant de même pour $F^-_{\varepsilon}$, on obtient

$$
\int i\int
$$

$$
h(\lambda )d\mu(\lambda ) =-\widetilde{f}(y-i\varepsilon )R(u, y-i\varepsilon )dy
$$

$_{F^-_{\varepsilon}}$ 2 $_{\mathbf{R}}$

et on conclut que l’intégrale de $h$ sur $\mathbf{C}$ est la limite quand $\varepsilon \rightarrow 0$ de

$$
i\int
$$

$$
v_{\varepsilon}=\widetilde{f}(y+i\varepsilon )R(u, y+i\varepsilon )-\widetilde{f}(y-i\varepsilon )R(u, y-i\varepsilon )dy
$$

2 $_{\mathbf{R}}$

D’après la prop. 7, on a $v_{\varepsilon}=\pi f_{\varepsilon}(u)$, où $f_{\varepsilon}$ est la fonction définie sur $\mathbf{R}$ par

1 $\int\widetilde{f}(y+i\varepsilon )\widetilde{f}(y-i\varepsilon )$

$$
f_{\varepsilon}(x) =--dy
$$

$$
2i\pi_{\mathbf{R}}y-x+i\varepsilon y-x-i\varepsilon
$$

Comme $f_{\varepsilon}\rightarrow f$ quand $\varepsilon \rightarrow 0$ dans $\mathscr{C}_b(\mathbf{R})$ (lemme 7), l’endomorphisme $v_{\varepsilon}=\pi f_{\varepsilon}(u)$ converge vers $\pi f(u)$ dans $\mathscr{L}(E)$ (prop. 5 de IV, p. 275). Le théorème est démontré.

### 6. Topologies résolvantes et continuité du calcul fonctionnel

Dans ce numéro, E désigne un espace hilbertien complexe. Rappelons qu’on note $\mathscr{A}(E)$ l’ensemble des opérateurs partiels auto-adjoints sur E. On va étendre à $\mathscr{A}(E)$ les propriétés de continuité du numéro 8 de IV, p. 194.

#### Définition 6 {#ts-iv-s5-def-6 .statement tag=036B}

Soit $\mathscr{T}$ une topologie localement convexe sur $\mathscr{L}(E)$. La topologie $\mathscr{T}$ -résolvante sur $\mathscr{A}(E)$ est la topologie la moins fine telle que les applications $u\mapsto R(u, \lambda )$ de $\mathscr{A}(E)$ dans $\mathscr{L}(E)$ muni de la topologie $\mathscr{T}$ sont continues pour tout $\lambda \in \mathbf{C}-\mathbf{R}$.

#### Proposition 11 {#ts-iv-s5-prop-11 .statement tag=036C}

Soit $\mathscr{T}$ une topologie localement convexe sur $\mathscr{L}(E)$ qui est moins fine que la topologie d’espace de Banach de $\mathscr{L}(E)$.

a) Soit $f\in \mathscr{C}_0(\mathbf{R})$. Pour toute suite $(u_n)_{n\in\mathbf{N}}$ dans $\mathscr{A}(E)$ qui converge vers $u$ pour la topologie $\mathscr{T}$ -résolvante, la suite $(f(u_n))_{n\in\mathbf{N}}$ converge vers $f(u)$ dans l’espace $\mathscr{L}(E)$ muni de la topologie $\mathscr{T}$;

b) Supposons que tout $u\in \mathscr{A}(E)$ admet un système fondamental dénombrable de voisinages pour la topologie $\mathscr{T}$ -résolvante. L’application de $\mathscr{C}_0(\mathbf{R})\times \mathscr{A}(E)$ dans l’espace $\mathscr{L}(E)$ muni de la topologie $\mathscr{T}$ définie par $(f, u)\mapsto f(u)$ est continue.

Démontrons a). La topologie $\mathscr{T}$ sur $\mathscr{L}(E)$ est la borne supérieure des topologies définies par les semi-normes continues pour la topologie $\mathscr{T}$ (EVT, II, p. 26, cor. et rem. suivante). Il suffit donc de prouver que pour toute semi-norme $p$ sur $\mathscr{L}(E)$ qui est continue pour la topologie $\mathscr{T}$, la suite $p(f(u_n)-f(u))$ converge vers 0 (TG, I, p. 51, prop. 10).

Soit $p$ une telle semi-norme. Notons $\mathscr{L}(E)_p$ l’espace de Banach séparé complété de l’espace $\mathscr{L}(E)$ muni de la semi-norme $p$, et notons $\varpi$ l’application canonique de $\mathscr{L}(E)$ dans $\mathscr{L}(E)_p$; elle est continue, et on a $p(u) =\|\varpi (u)\|_p$ pour tout $u\in \mathscr{L}$ (E), où la norme est celle de l’espace $\mathscr{L}(E)_p$.

Comme $\mathscr{T}$ est moins fine que la topologie d’espace de Banach de $\mathscr{L}$ (E), il existe $c\geqslant 0$ tel que $p(u)\leqslant c\|u\|$ pour tout $u\in \mathscr{L}(E)$.

Supposons d’abord que $f\in \mathscr{D}(\mathbf{R})$. Soit $\widetilde{f}$ une extension presque analytique de $f$. Notons $\mu$ la mesure de Lebesgue sur $\mathbf{C}$. D’après la formule de Helffer–Sjöstrand (th. 2 de IV, p. 284), on a

$$
1\int\partial \widetilde{f}
$$

$$
\varpi (f(u_n)) =-(\lambda )\varpi (R(u_n, \lambda ))d\mu(\lambda ) \tag{14}
$$

$$
\pi_{\mathbf{C}}\partial z
$$

pour tout $n\in \mathbf{N}$.

Soit $\lambda \in \mathbf{C}-\mathbf{R}$. Par hypothèse, la suite des résolvantes $R(u_n, \lambda )$ converge vers $R(u, \lambda )$ dans $\mathscr{L}(E)$ muni de la topologie $\mathscr{T}$, donc la suite $(\varpi (R(u_n, \lambda )))_n$ converge vers $\varpi (R(u, \lambda ))$ dans l’espace de Banach $\mathscr{L}(E)_p$.

Pour tout $n\in \mathbf{N}$, on a

$\partial \widetilde{f}$ 1 $\partial \widetilde{f}$

$$
\overline{\partial z}(\lambda )R(u^n, \lambda )\leqslant \overline{\mathscr{I} (\lambda)}\overline{\partial z}(\lambda )
$$

(prop. 17 de IV, p. 248) donc

$\partial \widetilde{f}$ 1 $\partial \widetilde{f}$

$$
\overline{\partial z}(\lambda )\varpi (R(u^n, \lambda ))_p\leqslant c\overline{\mathscr{I} (\lambda)}\overline{\partial z}(\lambda )
$$

La majoration (13) de IV, p. 281 démontre que le membre de droite de cette inégalité est une fonction bornée pour $\lambda \in \mathbf{C}-\mathbf{R}$; elle est intégrable sur $\mathbf{C}$ puisque $\widetilde{f}$ est à support compact. On déduit du théorème de Lebesgue (INT, IV, p. 137, § 3, n$^o7$, th. 6) et de la formule de Helffer–Sjöstrand appliquée à $f$ que $\varpi (f(u_n))$ converge vers $\varpi (f(u))$, donc $p(f(u_n)-f(u))$ tend vers 0.

Supposons maintenant que $f\in \mathscr{C}_0(\mathbf{R})$. Soit $\varepsilon  >0$. Il existe une fonction $f_{\varepsilon}$ dans $\mathscr{D}(\mathbf{R})$ telle que $\|f_{\varepsilon}-f\|_{\infty}\leqslant \varepsilon ($cf. prop. 4, a) de IV, p. 202 et INT, III, p. 45, § 1, n$^o2$, prop. 3). D’après la prop. 5, c) de IV, p. 275, on a alors $\|f(u)-f_{\varepsilon}(u)\|\leqslant \varepsilon$ et $\|f(u_n)-f_{\varepsilon}(u_n)\|\leqslant \varepsilon$ pour tout $n\in \mathbf{N}$. Par conséquent, il vient

$$
p(f(u_n)-f(u))\leqslant 2c\varepsilon +p(f_{\varepsilon}(u_n)-f_{\varepsilon}(u))
$$

pour tout $n\in \mathbf{N}$. Puisque $f_{\varepsilon}\in \mathscr{D}(\mathbf{R})$, la suite $(p(f_{\varepsilon}(u_n)-f_{\varepsilon}(u)))_{n\in\mathbf{N}}$ converge vers 0 d’après le cas précédent, et donc $p(f(u_n)-f(u))$ converge vers 0. Cela conclut la preuve de a).

Démontrons l’assertion b). Sous l’hypothèse concernant $\mathscr{T}$, il résulte de TG, IX, p. 17, prop. 10 et remarque suivante, et de l’assertion a), que l’application $u\mapsto f(u)$ de $\mathscr{A}(E)$ dans $\mathscr{L}(E)$ est continue lorsque $f\in \mathscr{C}_0(\mathbf{R})$. Comme les applications $f\mapsto f(u)$ de $\mathscr{C}_0(\mathbf{R})$ dans $\mathscr{L}(E)$ sont continues de norme $\leqslant 1$ pour tout $u\in \mathscr{A}(E)$ (prop. 5, c) de IV, p. 275), l’assertion b) se déduit de TG, X, p. 13, cor. 3.

#### Exemple 1 {#ts-iv-s5-n6-exa-1 .statement tag=036D}

Soit $\mathfrak{S}$ un ensemble de parties bornées de E. La $\mathfrak{S}$-topologie sur $\mathscr{L}(E)$ (EVT, III, p. 13) est une topologie localement convexe moins fine que la topologie d’espace de Banach de $\mathscr{L}(E)$.

#### Exemple 2 {#ts-iv-s5-n6-exa-2 .statement tag=036E}

Soit $\mathscr{T}_b$ la topologie d’espace de Banach de $\mathscr{L}(E)$. Pour la topologie $\mathscr{T}_b$-résolvante, tout $u\in \mathscr{A}(E)$ admet un système fondamental dénombrable de voisinages.

En effet, il suffit de démontrer que pour tout $\lambda \in$ **C-R** et tout $\varepsilon  >0$, il existe $\lambda '\in \mathbf{Q}+i\mathbf{Q}^*$ et un entier $n\geqslant 1$ tels que tout opérateur partiel $v\in \mathscr{A}(E)$ vérifiant $\|R(v, \lambda ')-R(u, \lambda ')\|<1/n$ vérifie aussi la condition $\|R(v, \lambda )-R(u, \lambda )\|< \varepsilon$; en écrivant

$$
\|R(v, \lambda )-R(u, \lambda )\|\leqslant \|R(v, \lambda )-R(v, \lambda ')\|
$$

$$
+\|R(v, \lambda ')-R(u, \lambda ')\|+\|R(u, \lambda ')-R(u, \lambda )\|
$$

cette propriété résulte de la formule (8) de IV, p. 245, des estimées de la proposition 17 de IV, p. 248 et du fait que $\mathbf{Q}+i\mathbf{Q}^*$ est partout dense dans $\mathbf{C}-\mathbf{R}$.

La conclusion de la proposition n’est pas valide en général si $\mathscr{C}_0(\mathbf{R})$ est remplacé par $\mathscr{C}_b(\mathbf{R})$ (exercice 29 de IV, p. 366, e)). Néanmoins, on a le résultat suivant.

#### Corollaire {#ts-iv-s5-n6-cor-1 .statement tag=036F}

Soit $\mathscr{T}_s$ la topologie de la convergence simple de $\mathscr{L}(E)$. Soit $f\in \mathscr{C}_b(\mathbf{R})$. Pour toute suite $(u_n)_{n\in\mathbf{N}}$ dans $\mathscr{A}(E)$ qui converge vers $u$ pour la topologie $\mathscr{T}_s$-résolvante, la suite $(f(u_n))_{n\in\mathbf{N}}$ converge vers $f(u)$ dans $\mathscr{L}(E)$ muni de la topologie $\mathscr{T}_s$.

Soit $(u_n)$ une suite dans $\mathscr{A}(E)$ qui converge vers $u$ pour la topologie $\mathscr{T}_s$-résolvante. Soit $x\in E$ et soit $\varepsilon  >0$.

Pour tout entier $N\in \mathbf{N}$, soit $\varphi_N\in \mathscr{K}(\mathbf{R})$ une fonction à support contenu dans $[-(N + 1),N + 1]$ telle que $0\leqslant \varphi_N\leqslant 1$ et $\varphi_N(t) = 1$ pour tout $t\in [-N,N]$. Les fonctions $\varphi_N$ convergent simplement vers 1 quand N tend vers l’infini, et vérifient $|\varphi_N|\leqslant 1$, donc la prop. 6 de IV, p. 276 implique qu’il existe $N\in \mathbf{N}$ tel que $\|\varphi_N(u)x-x\|\leqslant \varepsilon$. Posons $f_N=f \varphi_N$.

Pour tout $n\in \mathbf{N}$, on a

$$
\|f(u_n)x-f(u)x\|\leqslant \|f(u_n)x-f_N(u_n)x\|+ \tag{15}
$$

$$
\|f_N(u_n)x-f_N(u)x\|+\|f_N(u)x-f(u)x\|
$$

Pour tout $v\in \mathscr{A}$ (E), on a

$$
\|f(v)x-f_N(v)x\|=\|(f(1-\varphi_N))(v)x\|
$$

$$
\leqslant \|f(v)\| \|x-\varphi_N(v)x\|\leqslant \|f\|_{\infty}\|x-\varphi_N(v)x\|
$$

(prop. 5, c) de IV, p. 275). Comme $\varphi_N\in \mathscr{C}_0(\mathbf{R})$, l’assertion a) de la prop. 11 appliquée à la topologie $\mathscr{T}_s$-résolvante implique que $\varphi_N(u_n)x$ converge vers $\varphi_N(u)x$ quand $n\rightarrow +\infty$. Par conséquent, pour tout $n$ assez grand, on a

$$
\|x-\varphi_N(u_n)x\|\leqslant \|x-\varphi_N(u)x\|+\varepsilon \|x\|\leqslant (1 +\|x\|)\varepsilon
$$

L’inégalité (15) devient alors

$$
\|f(u_n)x-f(u)x\|\leqslant \|f\|_{\infty}(2 +\|x\|)\varepsilon +\|f_N(u_n)x-f_N(u)x\|
$$

pour tout $n$ assez grand. On conclut la démonstration par le truchement de l’assertion a) de loc. cit., appliquée à la fonction $f_N\in \mathscr{C}_0(\mathbf{R})$ et à la topologie $\mathscr{T}_s$-résolvante.

### 7. Décomposition polaire

#### Lemme 8 {#ts-iv-s5-lem-8 .statement tag=036G}

Soit E un espace vectoriel topologique séparé. Soient $(E_1,\|\cdot \|_1)$ et $(E_2,\|\cdot \|_2)$ des sous-espaces denses de E munis de structures hilbertiennes telles que les injections canoniques de $E_1$ et $E_2$ dans E sont continues. Soit F un sous-espace de $E_1\cap E_2$, dense dans $E_1$ et $E_2$ pour ces structures hilbertiennes. Si $\|x\|_1=\|x\|_2$ pour tout $x\in F$, alors $E_1= E_2$ et $\|\cdot \|_1=\|\cdot \|_2$.

Soit $x\in E_1$. Il existe une suite $(x_n)_{n\in\mathbf{N}}$ dans F telle que $x_n$ converge vers $x$ dans l’espace hilbertien $E_1$. Puisque $\|x_n-x_m\|_2=\|x_n-x_m\|_1$ pour tous entiers $n$ et $m$, la suite $(x_n)$ est une suite de Cauchy dans $E_2$. Soit $y$ sa limite. On a $\|y\|_2=$ lim$\|x_n\|_2=\|x\|_1$. Puisque les injections canoniques de $E_1$ et $E_2$ dans E sont continues, on a $x_n\rightarrow x$ dans E et de même $x_n\rightarrow y$ dans E. Ainsi, il vient $x=y$ et $\|x\|_1=\|x\|_2$; en particulier, $E_1\subset E_2$. On conclut par symétrie.

Soit E un espace hilbertien complexe. Soit $u$ un opérateur partiel auto-adjoint et positif sur E. Pour tout $\alpha \in \mathbf{R}_+$, on pose $u^{\alpha}=f(u)$, où $f$ est l’application continue $x\mapsto x^{\alpha}$ de $\mathbf{R}_+$ dans $\mathbf{R}$. C’est un opérateur partiel auto-adjoint et positif (cor. 1, a) de IV, p. 273). Lorsque $u\in \mathscr{L}$ (E), cette notation est compatible avec la notation relative à l’algèbre stellaire $\mathscr{L}(E) ($cf. prop. 16 de I, p. 118). Si $\alpha$ est un entier positif, l’opérateur partiel $u^{\alpha}$ coïncide avec l’opérateur partiel défini par la composition $u\circ  \cdots  \circ u$ (cor. 1, b) de IV, p. 273).

Soit $\beta \in \mathbf{R}_+$. On a $u^{\alpha \beta}= (u^{\alpha})^{\beta}$ (cor. 4 de IV, p. 274). En particulier, si $\alpha  >0$, alors l’opérateur partiel $u^{1/\alpha}$ est l’unique opérateur partiel auto-adjoint positif $v$ sur E tel que $v^{\alpha}=u$.

Supposons que $0\leqslant \alpha \leqslant \beta$. On a alors dom($u^{\beta}$)$\subset$ dom($u^{\alpha}$) $:$ en effet, pour tout nombre réel $x\geqslant 0$, on a $x^{\alpha}\leqslant 1 +x^{\beta}$, et le résultat découle alors de la définition du domaine de $u^{\alpha}($cf. prop. 3 de IV, p. 271).

Soit $u$ un opérateur fermé à domaine dense de E dans un espace hilbertien complexe F. L’opérateur partiel $u^*u$ est auto-adjoint et positif (prop. 12 de IV, p. 241). On note $|u|= (u^*u)^{1/2}$.

#### Proposition 12 {#ts-iv-s5-prop-12 .statement tag=036H}

Soit $u$ un opérateur fermé à domaine dense de E dans un espace hilbertien complexe F.

a) Le domaine de l’opérateur partiel auto-adjoint positif $|u|$ coïncide avec le domaine de $u$;

b) Il existe une unique application linéaire partiellement isométrique $j$ de E dans F telle que $u=j|u|$ et Ker($j$) $=$ Ker($u$);

c) Soient $u_1$ un opérateur auto-adjoint positif sur E et $j_1$ une application linéaire partiellement isométrique de E dans F telle que $u=j_1u_1$ et Ker($j_1$) $=$ Ker($u_1$). On a alors $u_1=|u|$ et $j_1=j$.

Le domaine de $u^*u$ est contenu dans dom($u$) et dans dom($|u|$). Il est dense dans les espaces hilbertiens $E_u($loc. cit.) et $E_{|u|}$ (cor. 1, e) de IV, p. 273) et, pour tout $x\in$ dom($u^*u$), on a

$$
\|x\|^2_u=\|x\|^2+\langle u(x)|u(x)\rangle =\|x\|^2+\langle x|(u^*u)(x)\rangle \tag{16}
$$

$$
=\|x\|^2+\langle |u|(x)| |u|(x)\rangle =\|x\|^2_{|u|}
$$

Par conséquent, les espaces hilbertiens $E_u$ et $E_{|u|}$ sont égaux (lemme 8), donc dom($u$) $=$ dom($|u|$) et $\|u(x)\|$ = $\||u|(x)\|$ pour tout $x\in$ dom($u$).

La formule (16) implique que Ker($u$) $=$ Ker($|u|$) et qu’il existe une unique application linéaire isométrique $v$ de Im($|u|$) sur Im($u$) qui vérifie $v(|u|(x)) =u(x)$ pour tout $x\in$ dom($|u|$). Puisque $|u|$ est auto-adjoint, on a Im($|u|$)$^{\circ}=$ Ker($|u|$) (prop. 7, c) de IV, p. 236). Il existe donc une unique isométrie partielle $j$ de E dans F qui prolonge $v$ et s’annule sur Ker($|u|$) $=$ Ker($u$). Comme E = Ker($u$)$\oplus$ Im($|u|$), cette application est l’unique application partiellement isométrique telle que $u=j|u|$ et Ker($j$) $=$ Ker($u$).

Démontrons c). On a $u_1j_1^*j_1u_1\subset (j_1u_1)^*j_1u_1=u^*u$. L’application linéaire $j_1^*j_1$ est l’orthoprojecteur de noyau Ker($j_1$) $=$ Ker($u_1$) (EVT, V, p. 41, prop. 5 (ii)) et donc d’image Ker($u_1$)$^{\circ}=$ Im($u_1$) (prop. 7, c) de IV, p. 236). Par conséquent, $u^2_1\subset u^*u$, d’où $u^2_1=u^*u$ puisque ces deux opérateurs sont auto-adjoints. Ainsi, il vient $u_1= (u^*u)^{1/2}$, et l’assertion d’unicité de b) démontre finalement que $j_1=j$.

#### Définition 7 {#ts-iv-s5-def-7 .statement tag=036I}

Soit $u$ un opérateur fermé à domaine dense de E dans un espace hilbertien complexe F. Le couple $(j,|u|)$ déterminé par la prop. 12 est appelé la décomposition polaire de $u$.

Supposons que $u\in \mathscr{L}(E; F)$. Sa décomposition polaire au sens de cette définition coïncide avec celle de la définition 4 de I, p. 140.

### 8. Opérateurs auto-adjoints définis par une forme hermitienne partielle positive

Dans ce numéro, E désigne un espace hilbertien complexe.

#### Définition 8 {#ts-iv-s5-def-8 .statement tag=036J}

Soit D un sous-espace vectoriel de E. Une forme hermitienne partielle sur E de domaine D, est une correspondance $q= (\Gamma ,E\times E,\mathbf{C})$ dont le domaine de définition est $D\times D$, dont le graphe Γ est fonctionnel, et telle que l’application de $D\times D$ dans $\mathbf{C}$ définie par Γ est une forme hermitienne. On note dom($q$) $= D$.

On dit que $q$ est une forme partielle positive si la forme hermitienne qu’elle définie est positive.

Soit $u$ un opérateur partiel auto-adjoint sur E. Pour tous les éléments $x$ et $y$ de E, on note $\mu_{x,y}$ (resp. $\mu_x)$ la mesure spectrale de $(x, y)$ (resp. de $x)$ relative à $u$.

Soit $(j,|u|)$ la décomposition polaire de $u$ (déf. 7 de IV, p. 290). Notons $D'$ le domaine de $|u|^{1/2}$. Par définition, c’est l’espace des $x\in E$ tels que la fonction $z\mapsto  |z|$ est intégrable sur Sp($u$) par rapport à la mesure $\mu_x$. Il contient dom($u$).

Soit $(x, y)\in D'\times D'$. La fonction identique de Sp($u$) est intégrable par rapport à la mesure $\mu_{x,y}$ (prop. 4, b) de IV, p. 271) ; on pose

$$
q_u(x, y) =\int t d\mu_{x,y}(t)
$$

Sp($u$)

Si $y\in$ dom($u$), on a $q_u(x, y) =\langle x|u(y)\rangle$ d’après la formule (6) de IV, p. 271. L’application $q_u$ est une forme hermitienne sur $D'$. Elle définit une forme hermitienne partielle sur E, dite associée à $u$. Si l’opérateur $u$ est positif, alors la forme $q_u$ est une forme hermitienne partielle positive.

#### Définition 9 {#ts-iv-s5-def-9 .statement tag=036K}

Soit $q$ une forme hermitienne partielle positive sur E. On note $E_q$ l’espace préhilbertien séparé dom($q$) muni du produit scalaire

$$
(x|y)_q=\langle x|y\rangle +q(x, y)
$$

On note $\|x\|_q$ la norme de $x\in E_q$. On dit que la forme $q$ est fermée si $E_q$ est un espace hilbertien.

#### Proposition 13 {#ts-iv-s5-prop-13 .statement tag=036L}

Soit $u$ un opérateur partiel auto-adjoint positif sur E. Soit $q_u$ la forme partielle positive associée à $u$.

a) Le domaine de $q_u$ est le domaine de $u^{1/2}$, et pour tous $x$ et $y$ dans dom($u^{1/2}$), on a $q_u(x, y) =\langle u^{1/2}(x)|u^{1/2}(y)\rangle$;

b) La forme partielle positive $q_u$ est fermée. Le domaine de $u$ est un cœur pour $q_u$.

Puisque $u$ est positif, on a $|u|=u$. Le domaine dom($|u|^{1/2}$) de $q_u$ coïncide donc avec dom($u^{1/2}$) et on a

$$
q_u(x, y) =\int t d\mu_{x,y}(t) =\int t^{1/2}\cdot t^{1/2}d\mu_{x,y}(t)
$$

Sp($u$) Sp($u$)

$$
=\langle u^{1/2}(x)|u^{1/2}(y)\rangle
$$

pour $x$ et $y$ dans dom($q_u$) (prop. 4, b) de IV, p. 271). Cela démontre l’assertion a).

Par ailleurs, l’espace préhilbertien $E_{q_u}$ coïncide alors avec l’espace préhilbertien $E_{u^{1/2}}$ associé à $u^{1/2}$ (déf. 4 de IV, p. 230). Puisque $u^{1/2}$ est un opérateur partiel fermé, cet espace est un espace hilbertien (prop. 4 de IV, p. 230) et dom($u$) est dense dans $E_{u^{1/2}}$ d’après l’assertion e) du cor. 1 de IV, p. 273.

Soit $q$ une forme hermitienne partielle sur E de domaine D dense dans E. Pour $y\in D$, notons $\lambda_y$ la forme linéaire $x\mapsto q(y, x)$ sur D. On note $\widetilde{D}$ l’ensemble des $y\in D$ tels que la forme linéaire $\lambda_y$ est continue sur D.

Soit $y\in \widetilde{D}$. Puisque D est dense dans E, il existe une unique forme linéaire continue sur E qui prolonge $\lambda_y$. On la note encore $\lambda_y$. Il existe un unique élément $u(y)$ dans E tel que $\lambda_y(x) =\langle u(y)|x\rangle$ pour tout $x\in E$ (EVT, V, p. 15, th. 3). L’application $y\mapsto u(y)$ est linéaire de $\widetilde{D}$ dans E ; on dit que l’opérateur partiel $u$ sur E de domaine $\widetilde{D}$ est l’opérateur partiel représentant $q$. On a donc

$$
q(x, y) =\langle x|u(y)\rangle
$$

pour $y\in$ dom($u$) et $x\in D$.

#### Remarque {#ts-iv-s5-n8-rem-1 .statement tag=036M}

Soient $q$ une forme partielle positive fermée et $q'$ une forme hermitienne positive continue sur E. La forme hermitienne positive définie sur dom($q$) par $(x, y)\mapsto q(x, y) +q'(x, y)$ est une forme hermitienne partielle positive fermée de même domaine que $q$. On la note $q+q'$.

D’après EVT, V, p. 16, cor. 2, il existe une unique application linéaire $u'\in \mathscr{L}(E)$ telle que $q'(x, y) =\langle x|u'(y)\rangle$ pour tout $(x, y)\in E\times E$. L’endomorphisme $u'$ est positif et l’opérateur partiel représentant la forme hermitienne partielle positive fermée $q+q'$ est $u+u'$.

#### Proposition 14 {#ts-iv-s5-prop-14 .statement tag=036N}

Soient $q$ une forme positive partielle fermée à domaine dense sur E et $u$ l’opérateur partiel représentant $q$.

a) Le domaine de $u$ est dense dans l’espace hilbertien $E_q$;

b) L’opérateur partiel $u$ est auto-adjoint et positif.

Puisque $q$ est fermée, l’espace préhilbertien $E_q$ de la définition 9 est un espace hilbertien.

Démontrons que l’opérateur partiel $u+ 1_E$ de domaine dom($u$) est bijectif. Comme

$$
\langle x|(u+ 1_E)(x)\rangle =q(x, x) +\|x\|^2\geqslant \|x\|^2
$$

pour tout $x\in$ dom($u$), cet opérateur partiel est injectif.

Soit $y\in E$. La forme linéaire sur $E_q$ définie par $x\mapsto  \langle y|x\rangle$ est continue puisque $\|x\|\leqslant \|x\|_q$. Il existe donc $y'\in E_q$ tel que

$$
\langle y|x\rangle = (y'|x)_q=\langle y'|x\rangle +q(y', x)
$$

pour tout $x\in E_q$ (EVT, V, p. 15, th. 3). Par définition, cela signifie que $y'$ appartient au domaine de l’opérateur partiel $\widetilde{u}$ représentant la forme partielle $(x, y)\mapsto (x|y)_q$ de domaine dom($q$), et que $\widetilde{u}(y') =y$. Comme $\widetilde{u}=u+ 1_E$ d’après la remarque ci-dessus, on en déduit que l’opérateur partiel $u+ 1_E$ est également surjectif, donc bijectif.

Démontrons que le domaine de $u$ est dense dans $E_q$. Soit $y\in E_q$ orthogonal à dom($u$) dans $E_q$. Il existe $y'\in$ dom($u$) tel que $u(y')+y'=y$. On a alors

$$
0 = (y|y')_q=\langle y|y'\rangle +q(y, y') =\langle y|y'+u(y')\rangle =\|y\|^2
$$

donc $y= 0$. L’assertion a) est donc démontrée.

Puisque dom($q$) est dense dans E et que $\|x\|\leqslant \|x\|_q$ pour tout $x\in$ dom($q$), l’assertion a) implique que dom($u$) est dense dans E. Comme la forme $q$ est hermitienne (resp. positive), pour tous $x$ et $y$ dans dom($u$), on a

$$
\langle y|u(x)\rangle =q(y, x) =q(x, y) =\overline{\langle x|u(y)\rangle}=\langle u(y)|x\rangle
$$

(resp. $\langle x|u(x)\rangle =q(x, x)\geqslant 0)$ de sorte que $u$ est symétrique (resp. positif). Enfin, l’opérateur partiel $u+ 1_E$ est auto-adjoint d’après le corollaire de la proposition 10 de IV, p. 240, et il en est de même de $u$.

#### Théorème 3 {#ts-iv-s5-thm-3 .statement tag=036O}

L’application qui à un opérateur auto-adjoint positif $u$ sur E associe la forme partielle positive $q_u$ est une bijection entre l’ensemble des opérateurs partiels auto-adjoints positifs sur E et l’ensemble des formes partielles positives fermées à domaine dense sur E. La bijection réciproque associe à une forme partielle positive $q$ l’opérateur partiel représentant $q$.

D’après les prop. 13, b) et 14, b), les applications décrites dans l’énoncé sont bien définies. Démontrons que ce sont des bijections réciproques l’une de l’autre.

Soient $u$ un opérateur partiel auto-adjoint positif sur E et $q$ la forme partielle positive associée à $u$. Notons $v$ l’opérateur auto-adjoint positif représentant $q$. Soit $y\in$ dom($u$)$\subset$ dom($u^{1/2}$) $=$ dom($q$). Pour tout $x\in$ dom($q$) $=$ dom($u^{1/2}$), on a

$$
q(y, x) =\langle u^{1/2}(y)|u^{1/2}(x)\rangle =\langle u(y)|x\rangle
$$

donc $y$ appartient au domaine de $v$ et vérifie $v(y) =u(y)$. L’opérateur partiel $v$ est donc une extension de $u$; comme $u$ et $v$ sont auto-adjoints, ils sont égaux.

Inversement, soient $q$ une forme partielle positive fermée à domaine dense et $u$ l’opérateur partiel auto-adjoint positif représentant $q$. On a dom($u$)$\subset$ dom($u^{1/2}$). Pour $x$ et $y$ dans dom($u$), on a

$$
q_u(x, y) =\langle u^{1/2}(x)|u^{1/2}(y)\rangle =\langle x|u(y)\rangle =q(x, y)
$$

d’après la prop. 13, a). Ainsi, les espaces hilbertiens $E_q$ et $E_{q_u}$ contiennent tous deux dom($u$) comme sous-espace dense (prop. 14, a) et prop. 13, b), respectivement) et $\|x\|_q=\|x\|_{q_u}$ pour tout $x\in$ dom($u$). Il en résulte que $E_q= E_{q_u}$ et que $q=q_u$ (lemme 8).

#### Corollaire {#ts-iv-s5-n8-cor-1 .statement tag=036P}

Soient $q$ une forme partielle positive fermée sur E et $u$ l’opérateur auto-adjoint positif représentant $q$. Le domaine de $q$ est égal au domaine de $(1_E+u)^{1/2}$, et on a

$$
\|x\|_q=\|(1_E+u)^{1/2}x\|
$$

pour tout $x\in$ dom($q$).

Le domaine de $q$ est égal au domaine de $u^{1/2}$ (prop. 13, a)), qui coïncide avec celui de $(1_E+u)^{1/2}($cf. prop. 3 de IV, p. 271). Pour tout $x\in$ dom($u$)$\subset$ dom($u^{1/2}$), on a

$$
\|(1_E+u)^{1/2}x\|^2=\langle x|(1_E+u)(x)\rangle =\|x\|^2+\langle x|u(x)\rangle =\|x\|^2_q
$$

Comme le domaine de $u$ est dense dans l’espace hilbertien $E_q$ (prop. 14, a)), cette formule s’étend par continuité à tout $x\in$ dom($u^{1/2}$).

#### Exemple {#ts-iv-s5-n8-exa-1 .statement tag=036Q}

Soit $u$ un opérateur partiel positif sur E qui n’est pas nécessairement fermé. On définit une forme partielle positive $q$ de domaine dom($u$) par

$$
q(x, y) =\langle x|u(y)\rangle
$$

pour $x$ et $y$ dans dom($u$). Soit $E_q$ l’espace préhilbertien séparé de la définition 9 de IV, p. 292. Soit $\widetilde{E}_q$ l’espace hilbertien complété de $E_q$, dont on note encore $(x, y)\mapsto (x|y)_q$ le produit scalaire. Puisque l’inclusion canonique $\iota$ de $E_q$ dans E est continue, elle admet une unique extension continue, notée $\widetilde{\iota}$, de $\widetilde{E}_q$ dans E. La forme hermitienne $q$ est continue sur $E_q$, donc se prolonge également en une unique forme hermitienne positive continue $\widetilde{q}$ sur $\widetilde{E}_q$.

Démontrons que l’application linéaire $\widetilde{\iota}$ est injective. Soit $x\in$ Ker($\widetilde{\iota}$). Considérons une suite $(x_n)_{n\in\mathbf{N}}$ dans $E_q$ qui converge vers $x$ dans $\widetilde{E}_q$. On a alors

$_{n\rightarrow}$lim$_{+\infty}\iota (x_n) =\widetilde{\iota}(x) = 0$,

donc la suite $(x_n)_{n\in\mathbf{N}}$ converge vers 0 dans E. Soit $y\in E_q$. Puisque $\widetilde{q}$ est continue sur $\widetilde{E}_q$, il vient

$(x|y)_q=_{n\rightarrow}$lim$_{+\infty}(x_n|y)_q=_{n\rightarrow}$lim$_{+\infty}\langle x_n|y\rangle +q(x_n, y)$

$=_{n\rightarrow}$lim$_{+\infty}\langle x_n|y\rangle +\langle x_n|u(y)\rangle = 0$.

Comme l’espace $E_q$ est dense dans $\widetilde{E}_q$, on en déduit que $x= 0$, comme désiré.

En identifiant $\widetilde{E}_q$ à son image par $\widetilde{\iota}$ dans E, on interprète $\widetilde{q}$ comme une forme partielle positive fermée à domaine dense qui étend $q$. L’opérateur auto-adjoint positif associé à $\widetilde{q}$ est une extension auto-adjointe de $u$. On dit que c’est l’extension de Friedrichs de $u$.

#### Remarque {#ts-iv-s5-n8-rem-2 .statement tag=036R}

Soit $c\in \mathbf{R}_+$. Soit $q$ une forme hermitienne partielle fermée à domaine dense telle que $q(x, x)\geqslant -c\|x\|^2$ pour tout $x$ appartenant au domaine de $q$. Cela signifie que la forme hermitienne partielle fermée de domaine dom($q$) définie par $\widetilde{q}(x, y) =q(x, y) +c\langle x|y\rangle$ est une forme partielle positive. Par le théorème 3, de telles formes correspondent donc aux opérateurs partiels auto-adjoints $u$ sur E tels que $u+c1_E$ est positif, c’est-à-dire tels que $u$ est minoré (déf. 7 de IV, p. 237) par $-c$.

Réciproquement, soit $u$ un opérateur partiel symétrique sur E tel que

$$
\langle x|u(x)\rangle \geqslant -c\|x\|^2 \tag{17}
$$

pour tout $x\in$ dom($u$). Alors $v=u+c1_E$ est un opérateur partiel positif sur E. On appelle extension de Friedrichs de $u$ l’opérateur auto-adjoint $\widetilde{v}-c1_E$, où $\widetilde{v}$ est l’extension de Friedrichs de $v$; c’est une extension auto-adjointe de $u$, qui ne dépend pas du choix du nombre réel $c$ vérifiant (17).

### 9. Principes variationnels pour le spectre des opérateurs positifs

Dans ce numéro, E est un espace hilbertien complexe non nul.

#### Proposition 15 {#ts-iv-s5-prop-15 .statement tag=036S}

Soit $u$ un opérateur partiel auto-adjoint sur E. On suppose que $u$ est minoré par $c\in \mathbf{R}$ (déf. 7 de IV, p. 237). On a

$$
\langle x|u(x)\rangle
$$

inf(Sp($u$)) $=$ inf $\in [c,+\infty [$.

$x\in$dom($u$)$-\{0\}\|x\|2$

Soit $m$ le membre de droite de l’égalité à démontrer. Soient $x\in E$ et $\mu_x$ la mesure spectrale de $x$ relative à $u$. On a

$$
\langle x|u(x)\rangle =\int t d\mu_x(t)
$$

Sp($u$)

$\geqslant$ inf(Sp($u$))$\int_{Sp(u)}d\mu_x(t) =$ inf(Sp($u$))$\|x\|^2$,

(formule (6), p. 271) donc inf(Sp($u$))$\leqslant m$. Réciproquement, l’opérateur partiel $u-m$ est positif, donc inf(Sp($u$))$-m=$ inf(Sp($u-m\cdot 1_E$))$\geqslant 0$ (prop. 17 de IV, p. 248).

La prop. 9 de I, p. 139 correspond au cas particulier de cette proposition lorsque $u$ est un élément hermitien de $\mathscr{L}$ (E), qui est alors nécessairement minoré. Dans ce cas, on a également

$$
\langle x|u(x)\rangle
$$

sup(Sp($u$)) $=$ sup

$x\in$dom($u$)$-\{0\}\|x\|2$

(loc. cit.) ; si $u$ n’appartient pas à $\mathscr{L}$ (E), alors cette borne supérieure est $+\infty$.

#### Définition 10 {#ts-iv-s5-def-10 .statement tag=036T}

Soit $u$ un opérateur partiel normal sur E. Un nombre complexe $\lambda \in$ Sp($u$) appartient au spectre sensible de $u$ si $\lambda$ est isolé dans Sp($u$) et si $\lambda$ est une valeur propre de multiplicité finie.

On note Sp$_s(u)$ le spectre sensible de $u$. Son complémentaire dans Sp($u$) est appelé le spectre essentiel de $u$ et noté Sp$_e(u)$.

Le spectre essentiel d’un opérateur partiel normal $u$ sur E est fermé dans $\mathbf{C}$, puisque Sp($u$) est fermé dans $\mathbf{C}$ et que le complémentaire du spectre essentiel est ouvert dans Sp($u$). Le spectre sensible de $u$ n’est pas nécessairement fermé dans $\mathbf{C}$ (exercice 36 de IV, p. 369).

#### Lemme 9 {#ts-iv-s5-lem-9 .statement tag=036U}

Soient E un espace hilbertien complexe et $u$ un opérateur partiel normal sur E. Soit $\lambda \in$ Sp($u$). On a $\lambda \in$ Sp$_s(u)$ si et seulement s’il existe un voisinage ouvert V de $\lambda$ dans $\mathbf{C}$ tel que le projecteur spectral $p_V$ de $u$ défini par V est de rang fini.

Soit $\lambda \in$ Sp$_s(u)$. Il existe un voisinage ouvert V de $\lambda$ dans $\mathbf{C}$ tel que Sp($u$)$\cap V =\{\lambda \}$; le projecteur spectral $p_V=p_{\{\lambda\}}$ est alors de rang fini (cor. de la prop. 9 de IV, p. 278).

Réciproquement, supposons qu’il existe un voisinage ouvert V de $\lambda$ tel que le projecteur spectral $p_V$ est de rang fini $n\in \mathbf{N}$. D’après le cor. de la prop. 10 de IV, p. 279, l’intersection $V\cap$ Sp($u$) contient au plus $n$ éléments, donc $\lambda$ est isolé dans Sp($u$). C’est donc une valeur propre de $u$ de multiplicité spectrale au plus $n$ d’après le cor. de la prop. 9 de IV, p. 278.

On suppose dans la suite de ce numéro que E est de dimension infinie ; les analogues des résultats ci-dessous lorsque E est de dimension finie se déduisent du n$^o4$ de IV, p. 153.

Soit $u$ un opérateur auto-adjoint minoré sur E. Soit $c$ un minorant de $u$; le spectre de $u$ est contenu dans $[c,+\infty [$ (prop. 15). Supposons que le spectre essentiel de $u$ n’est pas vide. On note alors $\varrho_e$ la borne inférieure du spectre essentiel de $u$, de sorte que $\varrho_e\geqslant c$ et $\varrho_e$ est un élément du spectre de $u$. On note Sp$_h(u) =$ Sp($u$)$\cap [\varrho_e,+\infty [$; c’est une partie fermée de Sp($u$), donc également de $\mathbf{C}$, telle que inf(Sp$_h(u)) =\varrho_e$; on l’appelle partie haute du spectre de $u$. Si le spectre essentiel de $u$ est vide, on note Sp$_h(u) =\emptyset$ et $\varrho_e= +\infty$.

L’intersection Sp$_b(u) =$ Sp($u$)$\cap [0, \varrho_e[$ est contenue dans le spectre sensible de $u$, et ses éléments sont donc des valeurs propres isolées de multiplicité finie ; on dit que c’est la partie basse du spectre de $u$. Soit $E_b$ le sous-espace fermé de E engendré par les sous-espaces propres relatifs aux valeurs propres $\lambda \in$ Sp$_b(u)$. D’après le cor. de la prop. 9 de IV, p. 278 et la prop. 8 de IV, p. 278, l’espace $E_b$ est l’image du projecteur spectral $p_{Sp_b(u)}$ défini par Sp$_b(u)$. Comme Sp($u$) est la réunion disjointe de Sp$_b(u)$ et Sp$_h(u)$, l’orthogonal $E_h$ de $E_b$ est l’image du projecteur spectral $p_{Sp_h(u)}$ défini par Sp$_h(u)$. Si Sp$_b(u)$ est fini, alors l’espace $E_b$ est de dimension finie ; l’espace $E_h$ est alors non nul, puisqu’on suppose que E est de dimension infinie.

#### Lemme 10 {#ts-iv-s5-lem-10 .statement tag=036V}

On a

$$
\langle x|u(x)\rangle \geqslant \varrho_e\|x\|^2 \tag{18}
$$

pour tout $x\in E_h\cap$ dom($u$).

Si $x\in E_h\cap$ dom($u$), alors le support de la mesure spectrale $\mu_x$ de $x$ relative à $u$ est contenu dans l’intervalle $[\varrho_e,+\infty [$ (prop. 9, a) de IV, p. 278), donc

$$
\langle x|u(x)\rangle =\int_{\mathbf{R}}td\mu_x(t)\geqslant \varrho_e\|x\|^2
$$

#### Lemme 11 {#ts-iv-s5-lem-11 .statement tag=036W}

Supposons que $E_b$ est de dimension finie. Alors, pour tout nombre réel $\varepsilon  >$ 0, l’image du projecteur spectral de $u$ défini par $[\varrho_e, \varrho_e+\varepsilon ]$ est de dimension infinie.

Si $E_b$ est de dimension finie, alors le spectre essentiel de $u$ est non vide, donc $\varrho_e$ est fini et appartient à Sp$_e(u)$. De plus, le spectre bas Sp$_b(u)$ est fini, donc il existe $\delta  >0$ tel que $[\varrho_e-\delta , \varrho_e+\delta ]\cap$ Sp($u$)$\subset [\varrho_e, \varrho_e+\delta ]$. L’assertion résulte alors du lemme 9.

#### Proposition 16 {#ts-iv-s5-prop-16 .statement tag=036X}

L’ensemble Sp$_b(u)\subset [c, \varrho_e[$ est dénombrable, discret et fermé dans $[0, \varrho_e[$. C’est l’ensemble des valeurs d’une suite strictement croissante $(\nu_k)_{0\leqslant k<Card(Sp_b(u))}$ de nombres réels positifs ; si Sp$_b(u)$ est infini, alors la suite $(\nu_k)$ converge vers $\varrho_e$.

Notons T = Sp$_b(u)\cap [0, \varrho_e[$. C’est une partie fermée et discrète de $[c, \varrho_e[$ par définition. Pour tout nombre entier $i\geqslant 1$, l’ensemble Sp$_b(u)\cap [c, \varrho_e-1/i]$ est compact et discret, donc fini. Comme T est la réunion de ces ensembles pour $i\geqslant 1$, l’ensemble T est dénombrable.

Cela conclut la preuve si Sp$_b(u)$ est fini. Si Sp$_b(u)$ est infini, on conclut en appliquant le lemme 2 de III, p. 90 à l’image S de T par l’application $\lambda \mapsto \varrho_e-\lambda$.

Pour tout entier $k$ tel que $0\leqslant k <$ Card(Sp$_b(u))$, on note $n_k\geqslant 1$ la multiplicité de la valeur propre $\nu_k$ de $u$. On note $\mathbf{N}=\mathbf{N}\cup  \{+\infty \} \subset \mathbf{R}$. Notons $M\in \mathbf{N}$ la somme des multiplicités $n_k$. C’est la dimension hilbertienne de $E_b$, si l’on convient de dire qu’un espace de dimension hilbertienne infinie est de dimension $+\infty  \in \mathbf{N}$.

Pour tout entier $n$ tel que $0\leqslant n <M$, on définit $\lambda_n(u) =\nu_k$, où $k\geqslant 0$ est l’unique entier tel que

$$
n_0+\cdots +n_{k-1}\leqslant n < n_0+\cdots +n_k
$$

Si $n\in \mathbf{N}$ vérifie $n\geqslant M$, on pose $\lambda_n(u) =\varrho_e$. Ce cas ne peut se présenter que si Sp$_b(u)$ est fini, auquel cas $\varrho_e$ est fini, puisqu’on suppose que E est de dimension infinie.

Par construction, la suite $(\lambda_n(u))_{n\in\mathbf{N}}$ est croissante et, pour tout élément $\lambda$ de Sp$_b(u)$, le nombre des entiers $n$ tels que $\lambda_n(u) =\lambda$ est égal à la multiplicité de $\lambda$ comme valeur propre de $u$. La suite $(\lambda_n(u))_{n\in\mathbf{N}}$ tend vers $+\infty$ si et seulement si le spectre essentiel de $u$ est vide.

Pour tout $n\in \mathbf{N}$, on note $\mathscr{F}_n$ (resp. $\mathscr{F}_n^u)$ l’ensemble des sous-espaces vectoriels $F\subset E$ de dimension $n$ (resp. l’ensemble des sous-espaces vectoriels $F\subset$ dom($u$) de dimension $n)$.

Soient $n\in \mathbf{N}$ tel que $n <M$ et $F\in \mathscr{F}_n^u$. On dit que F est adapté à $u$ si F admet une base orthonormale $(f_i)_{0\leqslant i\leqslant n-1}$ telle que $u(f_i) =\lambda_i(u)f_i$ pour $0\leqslant i\leqslant n-1$.

Soit $F\in \mathscr{F}_n^u$ adapté à $u$. L’espace F est contenu dans $E_b$; il est engendré par des vecteurs propres de $u$ pour des valeurs propres $\lambda \leqslant \lambda_{n-1}(u)$, et il contient les espaces propres correspondant aux valeurs propres $\lambda  < \lambda_{n-1}(u)$. De plus, pour toute partie universellement mesurable A de Sp($u$), l’espace F est stable par le projecteur spectral $p_A$ défini par A (prop. 9, c) de IV, p. 278).

#### Lemme 12 {#ts-iv-s5-lem-12 .statement tag=036Y}

Soit $F\in \mathscr{F}_n^u$ un sous-espace adapté à $u$. Tout vecteur propre de $u$ appartenant à l’espace $F^{\circ}\cap E_b$ a une valeur propre $\geqslant \lambda_n(u)$.

Soit $\ell$ tel que $\lambda_{n-1}(u) =\nu_{\ell}$. Soit $x\in F^{\circ}\cap E_b$ un vecteur propre de $u$ pour une valeur propre $\lambda$, et soit $k <$ Card(Sp$_b(u))$ tel que $\lambda =\nu_k$.

La condition $k < \ell$ est impossible, car $\nu_k< \nu_{\ell}$, et l’espace F contiendrait alors le sous-espace propre pour la valeur propre $\nu_k$, contredisant le fait que $x$ est orthogonal à F. Si $k=\ell$, alors $x$ est un vecteur propre pour la valeur propre $\lambda_{n-1}(u)$; comme $x\in F^{\circ}$, la multiplicité $n_k$ est strictement supérieure au nombre d’entiers $i < n$ tels que $\lambda_i(u) =\nu_k$, ce qui implique que $\lambda_n(u) =\lambda_{n-1}(u)$. Enfin, si $k > \ell$, on a $\lambda =\nu_k> \nu_{\ell}=\lambda_{n-1}(u)$, donc $\lambda \geqslant \lambda_n(u)$.

Pour tout sous-espace F de E, on note

$$
\langle x|u(x)\rangle
$$

$\widetilde{r}_F(u) =$ inf,

$$
_{x\in dom(u)\cap F^{\circ}}\|x\|^2
$$

$x\not =0$

$$
\langle x|u(x)\rangle
$$

$\widetilde{R}_F(u) =$ sup 2.

$$
_{x\in dom(u)\cap F}\|x\|
$$

$x\not =0$

#### Proposition 17 {#ts-iv-s5-prop-17 .statement tag=036Z}

a) Pour tout entier $n\in \mathbf{N}$, on a

$\lambda_n(u) =$ sup$_{F\in\mathscr{F}_n}\widetilde{r}_F(u) =_{F\in}$inf$_{\mathscr{F}_n^u_{+1}}\widetilde{R}_F(u)$;

b) Pour tout entier $n <M$ et pour tout sous-espace $F\in \mathscr{F}_n^u$ adapté à $u$, on a $\lambda_n(u) =\widetilde{r}_F(u)$;

c) Pour tout entier $n <M$ et pour tout sous-espace $F\in \mathscr{F}_{n+1}^u$ adapté à $u$, on a $\lambda_n(u) =\widetilde{R}_F(u)$.

Il existe une base orthonormale $(e_n)_{0\leqslant n<M}$ de l’espace $E_b$ telle que $e_n\in$ dom($u$) et $u(e_n) =\lambda_n(u)e_n$ pour tout $n$ tel que $0\leqslant n <M$. Pour tout $x\in E_b\cap$ dom($u$), on a donc

$$
\langle x|u(x)\rangle =\sum_{0\leqslant n<M}\lambda_n(u)|\langle e_n|x\rangle |^2
$$

Pour tout entier $n$ tel que $1\leqslant n <M + 1$, soit $F_n$ le sous-espace de dimension $n$ de $E_b$ engendré par $(e_0, . . . , e_{n-1})$. On a $F_n\subset$ dom($u$) et $F_n$ est adapté à $u$.

Soient $n\in \mathbf{N}$ et $F\in \mathscr{F}_n$. Démontrons que $\widetilde{r}_F(u)\leqslant \lambda_n(u)$ et, par conséquent, que

(19) Fsup$_{\in\mathscr{F}_n}\widetilde{r}_F(u)\leqslant \lambda_n(u)$.

Si $0\leqslant n <M$, en particulier si M est infini, alors la restriction à $F_{n+1}$ de l’orthoprojecteur de E sur F n’est pas injective, donc il existe $x\not = 0$ dans $F_{n+1}$ orthogonal à F. Comme

$$
\langle x|u(x)\rangle =\sum_{0\leqslant i\leqslant n}\lambda_i(u)|\langle e_i|x\rangle |^2=\lambda_n(u)|\langle e_n|x\rangle |^2\leqslant \lambda_n(u)\|x\|^2
$$

on a $\widetilde{r}_F(u)\leqslant \lambda_n(u)$.

Si $M\in \mathbf{N}$ et $n\geqslant M$, alors pour tout nombre réel $\varepsilon  >0$, il existe $x$ de norme 1 dans dom($u$) qui est orthogonal à F et dont la mesure spectrale $\mu_x$ est à support contenu dans $[\varrho_e, \varrho_e+\varepsilon ]$ (lemme 11 et prop. 9, a) de IV, p. 278), d’où

$$
\widetilde{r}_F(u)\leqslant \langle x|u(x)\rangle =\int_{Sp(u)}t d\mu_x(t)\leqslant \varrho_e+\varepsilon =\lambda_n(u) +\varepsilon
$$

par définition. Comme $\varepsilon  >0$ est arbitraire, on a donc $\widetilde{r}_F(u)\leqslant \lambda_n(u)$. L’inégalité (19) est donc établie.

Soient $n\in \mathbf{N}$ et $F\in \mathscr{F}_{n+1}^u$. Démontrons que $\widetilde{R}_F(u)\geqslant \lambda_n(u)$ et, par conséquent, que

(20) $F_{\in}$inf$_{\mathscr{F}_n^u_{+1}}\widetilde{R}_F(u)\geqslant \lambda_n(u)$.

Si $0\leqslant n <M$, observons que la restriction à F de l’orthoprojecteur sur $F_n$ n’est pas injective, donc qu’il existe un vecteur $x\not = 0$ dans F orthogonal à $F_n$. Posons $x_b=p_{Sp_b(u)}(x)$ et $x_h=p_{Sp_h(u)}(x)$. On a donc $x=x_b+x_h$. Les éléments $x_b$ et $x_h$ appartiennent au domaine de $u$ (prop. 9, c) de IV, p. 278) et sont orthogonaux à $F_n$. On a la minoration

$$
\langle x_b|u(x_b)\rangle =\sum_{i\geqslant n}\lambda_i(u)|\langle e_i|x_b\rangle |^2\geqslant \lambda_n(u)\|x_b\|^2
$$

et $\langle x_h|u(x_h)\rangle \geqslant \varrho_e\|x_h\|^2$ (formule (18)), d’où

$$
\langle x|u(x)\rangle =\langle x_b|u(x_b)\rangle +\langle x_h|u(x_h)\rangle
$$

$$
\geqslant \lambda_n(u)\|x_b\|^2+\varrho_e\|x_h\|^2\geqslant \lambda_n(u)\|x\|^2
$$

Si M est fini et $n\geqslant M$, il existe $x\not = 0$ dans F orthogonal à $E_b$, donc $x\in E_h$, et

$$
\langle x|u(x)\rangle \geqslant \varrho_e\|x\|^2=\lambda_n(u)\|x\|^2
$$

d’après (18). L’inégalité (20) est donc démontrée.

Nous allons maintenant démontrer les assertions b) et c), qui impliquent que les inégalités (19) et (20) sont des égalités lorsque $n <M$.

Démontrons l’assertion b). Soit $F\in \mathscr{F}_n^u$ un espace adapté à $u$. On a la somme hilbertienne

$F^{\circ}= E_h\oplus \bigoplus_{\lambda\in Sp_b(u)}$ Ker($u-\lambda \cdot 1_E$)$\oplus (F^{\circ}\cap$ Ker($u-\lambda_{n-1}(u)\cdot 1_E$)).

$\lambda >\lambda_{n-1}(u)$

Soit $x\in F^{\circ}-\{0\}$. Écrivons $x=x_h+y+z$, où $x_h\in E_h$ et $y$ (resp. $z)$ appartient au deuxième (resp. troisième) espace de la décomposition ci-dessus. En utilisant de nouveau (18) et le fait que toute valeur propre $\lambda  > \lambda_{n-1}(u)$ de $u$ est $\geqslant \lambda_n(u)$, on obtient

$$
\langle x|u(x)\rangle =\langle x_h|u(x_h)\rangle +\langle y|u(y)\rangle +\langle z|u(z)\rangle
$$

$$
\geqslant \varrho_e\|x_h\|^2+\lambda_n(u)\|y\|^2+\lambda_{n-1}(u)\|z\|^2
$$

Si $z\not = 0$, alors d’après le lemme 12, on a $\lambda_n(u) =\lambda_{n-1}(u)$. On en déduit donc que $\langle x|u(x)\rangle \geqslant \lambda_n(u)\|x\|^2$, d’où $\widetilde{r}_F(u)\geqslant \lambda_n(u)$. Combiné avec (19), cela implique l’assertion b).

Démontrons l’assertion c). Soit $F\in \mathscr{F}_{n+1}^u$ un sous-espace adapté à $u$. Soit $(f_i)_{0\leqslant i\leqslant n}$ une base orthonormale de F telle que $u(f_i) =\lambda_i(u)f_i$ pour $0\leqslant i\leqslant n$. Pour tout $x\in F$, on a

$$
\langle x|u(x)\rangle =\sum_{0\leqslant i\leqslant n}\lambda_i(u)|\langle f_i|x\rangle |^2\leqslant \lambda_n(u)\|x\|^2
$$

avec égalité si $x=f_n$, donc $\widetilde{R}_F(u) =\lambda_n(u)$.

Démontrons finalement que (19) et (20) sont des égalités lorsque $n\geqslant M$. Dans ce cas, M est fini, donc $E_b$ est contenu dans le domaine de $u$; de plus, on a $\lambda_n(u) =\varrho_e$ par définition.

Il existe $F\in \mathscr{F}_n$ contenant $E_b$. Tout élément $x\not = 0$ de dom($u$) orthogonal à F est donc orthogonal à $E_b$, et vérifie

$$
\langle x|u(x)\rangle
$$

$$
_2\geqslant \varrho_e
$$

$$
\|x\|
$$

(formule (18)), donc $\widetilde{r}_F(u)\geqslant \varrho_e=\lambda_n(u)$, et par conséquent

$_F$sup$_{\in\mathscr{F}_n}\widetilde{r}_F(u)\geqslant \lambda_n(u)$.

Soit $\varepsilon  >0$. Puisque $E_b$ est de dimension finie, il existe d’après le lemme 11 une famille orthonormale $(x_i)_{i\in I}$ d’éléments de E telle que le sous-espace F engendré par $E_b$ et $(x_i)_{i\in I}$ est de dimension $n+ 1$ et est contenu dans dom($u$), et telle que $\langle x_i|u(x_i)\rangle \leqslant \varrho_e+\varepsilon$ pour tout $i\in I$. On a alors $\widetilde{R}_F(u)\leqslant \varrho_e+\varepsilon$. Comme $\varepsilon  >0$ est arbitraire, on conclut que

inf $\widetilde{R}_F(u)\leqslant \varrho_e=\lambda_n(u)$.

$F\in \mathscr{F}_{n+1}^u$

La proposition est démontrée.

### 10. Perturbation compacte et spectre essentiel

Dans ce numéro, E est un espace hilbertien complexe de dimension infinie.

#### Lemme 13 {#ts-iv-s5-lem-13 .statement tag=0370}

Soit I une famille orthonormale de E. La famille I converge faiblement vers 0 selon le filtre des complémentaires des parties finies de I.

Soit $x\in E$. D’après l’inégalité de Bessel (EVT, V, p. 21, prop. 4) et TG, IV, p. 37, th. 1, la famille $(|\langle e_i|x\rangle |^2)_{i\in I}$ est sommable, donc $\langle e_i|x\rangle$ tend vers 0 selon le filtre des complémentaires des parties finies de I (TG, III, p. 38, prop. 1).

#### Proposition 18 {#ts-iv-s5-prop-18 .statement tag=0371}

Soient $u$ un opérateur partiel auto-adjoint sur E et $\lambda$ un nombre réel. On a $\lambda \in$ Sp$_e(u)$ si et seulement s’il existe une suite orthonormale $(x_n)_{n\in\mathbf{N}}$ dans E telle que $u(x_n)-\lambda x_n$ tend vers 0 dans E.

Supposons d’abord que $\lambda \in$ Sp$_e(u)$. Si le projecteur spectral de $u$ relatif à $\{\lambda \}$ est de rang infini, toute suite orthonormale $(x_n)$ dans son image répond à la question (cf. cor. de la prop. 9 de IV, p. 278). On supposera dans le suite que ce n’est pas le cas.

Pour tout $k\in \mathbf{N}$, soit $J_k$ l’ensemble des $t\in [\lambda -1, \lambda + 1]$ tels que

1 1

$$
<|t-\lambda |\leqslant
$$

$$
k+ 2k+ 1
$$

Les ensembles $J_k$ sont deux à deux disjoints. De plus, pour tout entier $K\in \mathbf{N}$, les ensembles $(J_k)_{k\geqslant K}$ forment une partition de l’ensemble

$$
I_K= [\lambda -1/(K + 1), \lambda + 1/(K + 1)]-\{0\}
$$

Comme le projecteur spectral de $u$ relatif à $I_K\cup  \{0\}$ est de rang infini (lemme 9 de IV, p. 297) et que celui relatif à $\{\lambda \}$ est supposé être de rang fini, on déduit de la prop. 8 de IV, p. 278 qu’il existe une suite $(k_n)_{n\in\mathbf{N}}$ strictement croissante dans $\mathbf{N}$ telle que le projecteur spectral $p_n$ de $u$ relatif à $J_{k_n}$ est non nul. Soit $x_n$ un vecteur de norme 1 dans l’image de $p_n$. La suite $(x_n)$ est orthonormale, puisque l’image de $p_n$ est orthogonale à celle de $p_m$ pour tous $n\not =m$ dans $\mathbf{N}$.

Soit $n\in \mathbf{N}$. Notons $\mu_n$ la mesure spectrale de $x_n$ relative à $u$; son support est contenu dans $J_{k_n}$ (prop. 9 de IV, p. 278). Il vient

$_2\int_2$ 1

$\|u(x_n)-\lambda x_n\|$ = $|t-\lambda |d\mu_n(t)\leqslant_2$,

$$
_{\mathbf{C}}k_n
$$

donc la suite $(x_n)_{n\in\mathbf{N}}$ a la propriété demandée.

Supposons réciproquement qu’il existe une suite orthonormale $(x_n)_{n\in\mathbf{N}}$ dans E telle que $u(x_n)-\lambda x_n\rightarrow$ 0. Notons $\mu_n$ la mesure spectrale de $x_n$ relative à $u$.

Soit $\varepsilon  >0$. Notons $p_{\varepsilon}$ le projecteur spectral de $u$ relatif à l’intervalle ouvert $I_{\varepsilon}= ]\lambda -\varepsilon , \lambda +\varepsilon [$. Pour tout $n\in \mathbf{N}$, il vient

$$
1 =\|x_n\|^2=\mu_n(I_{\varepsilon}) +\mu_n(\mathbf{R}-I_{\varepsilon})
$$

$$
1\int_2
$$

$$
\leqslant \mu_n(I_{\varepsilon}) +_2|t-\lambda |d\mu_n(t)
$$

$$
\varepsilon_{\mathbf{R}-I_{\varepsilon}}
$$

$_2$ 1 2

$=\|p_{\varepsilon}(x_n)\|$ + $\|u(x_n)-\lambda x_n\|$.

$$
\varepsilon^2
$$

L’hypothèse sur la suite $(x_n)$ implique donc que la norme de $p_{\varepsilon}(x_n)$ ne peut tendre vers 0. Comme la suite orthonormale $(x_n)$ converge faiblement vers 0 dans E (lemme 13), le projecteur $p_{\varepsilon}$ ne peut pas être compact (cor. de la prop. 6 de III, p. 6) et il est par conséquent de rang infini. Comme cela vaut pour tout $\varepsilon  >0$, le lemme 9 de IV, p. 297 permet de conclure que $\lambda \in$ Sp$_e(u)$.

Le théorème suivant est l’analogue pour les opérateurs partiels auto-adjoints du théorème 3 de III, p. 93.

#### Théorème 4 {#ts-iv-s5-thm-4 .statement tag=0372}

Soit $u$ un opérateur partiel auto-adjoint sur E. Le spectre essentiel de $u$ est l’intersection des ensembles Sp($u+v$) où $v$ parcourt l’ensemble des endomorphismes compacts hermitiens de E.

L’opérateur partiel $u+v$ est auto-adjoint pour tout endomorphisme hermitien $v$ de E puisque $(u+v)^*=u^*+v^*($cf. IV, p. 236).

Démontrons que si $v$ est compact, alors Sp$_e(u)\subset$ Sp$_e(u+v)$. Soit $\lambda \in$ Sp$_e(u)$ et soit $(x_n)_{n\in\mathbf{N}}$ une suite orthonormale dans E telle que $u(x_n)-\lambda x_n$ converge vers 0 (prop. 18). La suite $(x_n)$ converge faiblement vers 0 dans E (lemme 13) et comme l’endomorphisme $v$ est compact, la suite $(v(x_n))_{n\in\mathbf{N}}$ converge vers 0 dans E (cor. de la prop. 6 de III, p. 6). Par conséquent la suite $(u+v)(x_n)-\lambda x_n$ converge vers 0 dans E, et la prop. 18 implique que $\lambda \in$ Sp$_e(u+v)$.

Le spectre essentiel de $u$ est donc contenu dans l’intersection des ensembles Sp($u+v$) pour $v\in \mathscr{L}^c(E)$ hermitien.

Réciproquement, soit $\lambda \in$ Sp$_s(u)$. Notons $E_{\lambda}$ le sous-espace propre de $u$ relatif à $\lambda$, et $p_{\lambda}$ l’orthoprojecteur d’image $E_{\lambda}$; c’est le projecteur spectral de $u$ relatif à $\{\lambda \}$ (cor. de la prop. 9 de IV, p. 278). Par définition du spectre sensible, le projecteur $p_{\lambda}$ est de rang fini, donc compact. Posons $w=u+p_{\lambda}$; c’est un opérateur partiel auto-adjoint. Pour conclure la démonstration, vérifions que $\lambda$ appartient à l’ensemble résolvant de $w$.

On a $E_{\lambda}\subset$ dom($u$) et les espaces $E_{\lambda}$ et dom($u$)$\cap E^{\circ}_{\lambda}$ sont stables par $u$ (prop. 9 de IV, p. 278).

Soit $x\in$ dom($u$). Écrivons $x=p_{\lambda}(x)+y$ où $y\in$ dom($u$)$\cap E^{\circ}_{\lambda}$. D’après ce qui précède, on a

$$
\|w(x)-\lambda x\|^2=\|p_{\lambda}(x)\|^2+\|w(y)-\lambda y\|^2 \tag{21}
$$

Soient V un voisinage ouvert de $\lambda$ ne rencontrant pas le spectre de $u$ et $c >0$ tel que le disque de centre $\lambda$ et de rayon $c$ est contenu dans V. Soit $\mu_y$ la mesure spectrale de $y$ relative à $u$. Comme $y$ est orthogonal à $E_{\lambda}$, le support de $\mu_y$ ne rencontre pas V (loc. cit.). On a alors

$$
\|w(y)-\lambda y\|^2=\|u(y)-\lambda y\|^2=\int_{\mathbf{C}}|t-\lambda |^2d\mu_y(t)\geqslant c^2\|y\|^2 \tag{22}
$$

On conclut de (21) et (22) que $\|w(x)-\lambda x\|^2\geqslant$ inf($c^2,1$)$\|x\|^2$; puisque $w$ est auto-adjoint et $\lambda \in \mathbf{R}$, la conclusion résulte alors du lemme 5 de IV, p. 248.

#### Corollaire {#ts-iv-s5-n10-cor-1 .statement tag=0373}

Soient $u$ un opérateur partiel auto-adjoint sur E et $v$ un endomorphisme compact hermitien de E. On a Sp$_e(u+v) =$ Sp$_e(u)$.

Cela résulte aussitôt du théorème.

### 11. Perturbation

Dans ce numéro, E est un espace hilbertien complexe.

Si $u$ est un opérateur partiel auto-adjoint sur E et $v\in \mathscr{L}(E)$ est un endomorphisme hermitien, alors $u+v$ est auto-adjoint (cf. IV, p. 236). Ce n’est pas le cas en général lorsque $v$ est un opérateur partiel symétrique (exercice 9 de IV, p. 347). Nous allons cependant obtenir des résultats positifs de ce type dans ce numéro.

#### Définition 11 {#ts-iv-s5-def-11 .statement tag=0374}

Soit $u$ un opérateur partiel sur E. Un opérateur partiel $v$ sur E est dit borné relativement à $u$ si dom($u$)$\subset$ dom($v$) et si $v$ définit, par passage au sous-espace, une application linéaire continue de $E_u$ dans E.

Soit $u$ un opérateur partiel sur E. Soit $v$ un opérateur partiel borné relativement à $u$. Il existe un nombre réel $m$ tel que

$$
\|v(x)\|\leqslant m(\|x\|+\|u(x)\|)
$$

pour tout $x\in$ dom($u$). On appelle norme relative de $v$ par rapport à $u$, et on note $\|v\|_u$, la borne inférieure des nombres réels $a\geqslant 0$ tels qu’il existe un nombre réel $b$ tel que

$$
\|v(x)\|\leqslant a\|u(x)\|+b\|x\|
$$

pour tout $x\in$ dom($u$). La norme relative de $v$ est donc inférieure à la norme de la restriction de $v$ à l’espace $E_u$.

#### Remarque {#ts-iv-s5-n11-rem-1 .statement tag=0375}

Soit $u$ un opérateur partiel sur E. Tout endomorphisme $v\in \mathscr{L}(E)$ est borné relativement à $u$ et sa norme relative est nulle puisque $\|v(x)\|\leqslant \|v\| \|x\|$ pour tout $x\in$ dom($u$), ce qui permet de prendre $a= 0$ dans l’inégalité ci-dessus.

#### Théorème 5 (Kato–Rellich) {#ts-iv-s5-thm-5 .statement tag=0376}

Soient $u$ un opérateur partiel auto-adjoint sur E et $v$ un opérateur partiel symétrique borné relativement à $u$. Si la norme relative $\|v\|_u$ est $<1$, alors l’opérateur partiel $u+v$ de domaine dom($u$) est auto-adjoint.

Puisque $\|v\|_u<1$, il existe par définition des nombres réels positifs $a$ et $b$ tels que $a <1$ et $\|v(x)\|\leqslant a\|u(x)\|+b\|x\|$ pour tout $x\in$ dom($u$).

Soit $t\in \mathbf{R}^*$. Posons $w_t=v\circ R(u, it)$. On a dom($w_t$) $= E$ puisque l’image de $R(u, it)$ est contenue dans le domaine de $u$, qui est contenu dans le domaine de $v$ par hypothèse. Soit $x\in$ dom($u$). Comme $u$ est auto-adjoint, on a

$$
\|(it-u)x\|^2=\|itx\|^2+\|u(x)\|^2-it\langle x|u(x)\rangle +it\langle u(x)|x\rangle
$$

$$
=|t|^2\|x\|^2+\|u(x)\|^2
$$

d’où les inégalités $\|u(x)\|\leqslant \|(it-u)x\|$ et $\|x\|\leqslant |t|^{-1}\|(it-u)x\|$. Mais alors, il vient

$$
\|v(x)\|\leqslant (a+b|t|^{-1})\|(it-u)x\|
$$

En particulier, posons $x= R(u, it)y$ pour $y\in E$; on obtient

$$
\|w_t(y)\|\leqslant (a+b|t|^{-1})\|y\|
$$

On en déduit que $w_t\in \mathscr{L}(E)$ et que $\|w_t\|\leqslant a+|t|^{-1}b$.

Puisque $a <$ 1, il existe $t\in \mathbf{R}^*_+$ tel que $a+b|t|^{-1}<1$. On a alors $\|w_t\|<1$ et $\|w_{-t}\|<1$; les endomorphismes $1_E-w_t$ et $1_E-w_{-t}$ de E sont donc inversibles (prop. 2 de I, p. 22). Comme on a la formule $(1_E-w_t)\circ (it-u) =it-(u+v)$, cela implique que $u+v-it$ est surjectif ; de même, l’opérateur partiel $u+v+it$ est surjectif. Il en résulte que $u+v$ est auto-adjoint (prop. 11 de IV, p. 240).

### 12. Opérateurs à résolvante compacte

Dans ce numéro, E désigne un espace hilbertien complexe de dimension infinie.

#### Proposition 19 {#ts-iv-s5-prop-19 .statement tag=0377}

Soit $u$ un opérateur partiel auto-adjoint sur E. Les conditions suivantes sont équivalentes :

(i) Il existe une base orthonormale $B = (e_j)_{j\in J}$ de E telle que $u$ est diagonal dans la base B et la valeur absolue de la famille des valeurs propres de $u$ tend vers l’infini suivant le filtre des complémentaires des parties finies de J ;

(ii) Pour tout $\lambda$ appartenant à l’ensemble résolvant de $u$, la résolvante $R(u, \lambda )$ est compacte ;

(iii) Il existe un nombre complexe $\lambda$ appartenant à l’ensemble résolvant de $u$ tel que la résolvante $R(u, \lambda )$ est compacte ;

(iv) Le spectre de $u$ coïncide avec le spectre sensible de $u$.

Supposons que (i) est vérifiée et soit $(\lambda_j)_{j\in J}$ la famille des valeurs propres de $u$. Soit $\mu$ la mesure de comptage sur J. Le spectre de $u$ est l’image $\mu$-essentielle de la famille $(\lambda_j)$ (prop. 22 de IV, p. 252) ; c’est l’ensemble des valeurs de cette famille. Pour tout $\lambda  /\in$ Sp($u$), la résolvante $R(u, \lambda )$ est diagonale dans la base B et la famille de ses valeurs propres est $((\lambda -\lambda_j)^{-1})_{j\in J}($loc. cit.). Puisque cette famille converge vers 0, l’endomorphisme $R(u, \lambda )$ est compact (prop. 2, (iii) de IV, p. 148). Cela démontre que (i) implique (ii).

Comme l’ensemble résolvant de $u$ est non vide (cf. prop. 17 de IV, p. 248), les propriétés (ii) et (iii) sont équivalentes d’après la formule (8) de IV, p. 245 et la proposition 3 de III, p. 5.

Comme $R(u, \lambda )$ est normal pour $\lambda  /\in$ Sp($u$) (prop. 16 de IV, p. 247), la condition (iii) implique (iv) d’après la prop. 15 de IV, p. 247 et la prop. 5 de III, p. 90.

Démontrons finalement que (iv) implique (i). Soit $\mathscr{O}$ l’ensemble des parties orthonormales de E formées de vecteurs propres pour $u$. L’ensemble $\mathscr{O}$, ordonné par l’inclusion, est de caractère fini (E, III, p. 34, déf. 2) puisque O appartient à $\mathscr{O}$ si et seulement si les ensembles formés d’au plus deux éléments de O appartiennent à $\mathscr{O}$. D’après E, III, p. 35, th. 1, il existe un élément maximal O de $\mathscr{O}$. Notons F le sous-espace fermé de E engendré par O. Pour $e\in O$, il existe un unique $\lambda (e)\in \mathbf{R}$ tel que $u(e) =\lambda (e)e$ (prop. 17 de IV, p. 248).

L’ensemble des valeurs de l’application $\lambda$ de O dans $\mathbf{R}$ coïncide avec le spectre de $u$. En effet, d’une part cet ensemble est contenu dans le spectre de $u$ et d’autre part, s’il existe $\lambda_0\in$ Sp($u$) qui ne soit pas une valeur de $\lambda$, alors $\lambda_0$ est une valeur propre de $u$ par hypothèse. Il existe un vecteur $e\in$ dom($u$) de norme 1 tel que $u(e) =\lambda_0e$ et $e /\in O$; le sous-ensemble $O\cup  \{e\}$ est orthonormal (puisque des sous-espaces propres de $u$ relatifs à des valeurs propres distinctes sont orthogonaux d’après l’assertion b) du cor. de la prop. 17 de IV, p. 248) ; il appartient à $\mathscr{O}$, contredisant la maximalité de O.

Supposons que $F\not = E$. Alors $F^{\circ}$ est non nul. L’endomorphisme $R(u, i)$ de E est normal (prop. 16 de IV, p. 247). Il laisse stable le sous-espace $F^{\circ}$ de E (lemme 4 de I, p. 135). Soit $v$ l’endomorphisme de $F^{\circ}$ déduit de $R(u, i)$ par passage aux sous-espaces. C’est un endomorphisme continu et normal de $F^{\circ}($loc. cit.) dont le spectre est contenu dans celui de $R(u, i)$. Comme $F^{\circ}$ est non nul, le spectre de $v$ est non vide (cor. 1 de I, p. 26). De plus, le spectre de $v$ n’est pas réduit à 0, puisque l’endomorphisme normal $v$ est non nul (exemple 1 de I, p. 110). Soit $s\in$ Sp($v$)$-\{0\}$. Comme $s$ appartient au spectre de $R(u, i)$, il existe $e\in O$ tel que $s= (i-\lambda (e))^{-1}$, et $s$ est une valeur propre de $R(u, i)$ (prop. 15, a) de IV, p. 247). Comme $s$ est non nul, c’est un point isolé de Sp(R($u, i$)) par hypothèse, donc aussi de Sp($v$). Ainsi, $s$ est une valeur propre de $v$ (prop. 5, c) de I, p. 134). Soit $e\in F^{\circ}$ un vecteur propre de norme 1 de $v$; c’est également un vecteur propre de $u$ (prop. 15, b) de IV, p. 247), et l’ensemble $O\cup  \{e\}$ contredit le fait que O est maximal dans $\mathscr{O}$. On a donc F = E.

La famille des éléments de O est donc une base orthonormale de E formée de vecteurs propres de $u$. Le spectre de $u$ est fermé dans $\mathbf{R}$, et le spectre sensible est discret ; comme ces ensembles coïncident, l’ensemble des éléments $\lambda \in$ Sp($u$) tels que $|\lambda |\leqslant R$ est compact, donc fini, pour tout $R>0$. Ainsi la famille des valeurs absolues des valeurs propres de $u$ tend vers l’infini suivant le filtre des complémentaires des parties finies de O. Donc (iv) implique (i).

#### Définition 12 {#ts-iv-s5-def-12 .statement tag=0378}

Soit $u$ un opérateur partiel auto-adjoint sur E. On dit que $u$ est à résolvante compacte si les conditions équivalentes de la prop. 19 sont satisfaites.

#### Proposition 20 {#ts-iv-s5-prop-20 .statement tag=0379}

Soit $u$ un opérateur partiel auto-adjoint sur E. Alors $u$ est à résolvante compacte si et seulement si l’injection canonique $j$ de l’espace hilbertien $E_u$ dans E est compacte.

Supposons que $u$ est à résolvante compacte. Il existe $\lambda  /\in$ Sp($u$) tel que $R(u, \lambda )$ est compacte (prop. 19, (iii)). Soit B la boule unité de l’espace hilbertien $E_u$. Puisque $u$ est une application linéaire continue de $E_u$ dans E, le sous-ensemble $B'= (\lambda 1_E-u)(B)$ de E est borné. Puisque $R(u, \lambda )$ est compacte, le sous-ensemble $B = R(u, \lambda )(B')$ est relativement compact dans E (remarque 1 de III, p. 2). Cela démontre que $j$ est compacte.

Réciproquement, supposons que l’application linéaire $j$ est compacte. Le nombre complexe $i$ appartient à l’ensemble résolvant de $u$ (prop. 17 de IV, p. 248). On a $u\circ R(u, i) =-1_E+iR(u, i)$. Soit B la boule unité de E. Pour tout $x\in B$, on a

$$
\|u\circ R(u, i)(x)\|=\|-x+iR(u, i)(x)\|\leqslant 1 +\|R(u, i)\|
$$

et par conséquent

$$
\|R(u, i)x\|^2_u=\|R(u, i)x\|^2+\|u\circ R(u, i)x\|^2
$$

$$
\leqslant \|R(u, i)\|^2+ (1 +\|R(u, i)\|)^2
$$

L’image C de B par $R(u, i)$ est donc bornée dans $E_u$; comme $j$ est compacte par hypothèse, l’ensemble $C =j(C)$ est relativement compact dans E (III, loc. cit.). Par conséquent, la résolvante $R(u, i)$ est compacte et $u$ est à résolvante compacte (prop. 19, (iii)).

#### Corollaire {#ts-iv-s5-n12-cor-1 .statement tag=037A}

Soient $q$ une forme partielle positive fermée sur E et $u$ l’opérateur auto-adjoint positif représentant $q$. Les conditions suivantes sont équivalentes :

(i) L’opérateur partiel $u$ est à résolvante compacte ;

(ii) L’endomorphisme positif $\overline{(1_E + u)^{-1}}= (1_E+u)^{-1/2}$ de E est compact;

(iii) L’injection canonique $j$ de l’espace hilbertien $E_q$ (déf. 9 de IV, p. 292) dans E est compacte.

Comme $u$ est positif, le nombre réel $-1$ appartient à l’ensemble résolvant de $u$ (prop. 17 de IV, p. 248), donc l’endomorphisme positif $v=\overline{(1_E + u)^{-1}}$ est défini, et on a $v= (1_E+u)^{-1/2}$ d’après le calcul fonctionnel.

L’endomorphisme $v$ est compact si et seulement si $v^2= (1_E+u)^{-1}$ est compact (prop. 6 de III, p. 91), c’est-à-dire si et seulement si $u$ est à résolvante compacte (prop. 19, (iii)). Cela démontre que les conditions (i) et (ii) sont équivalentes.

Supposons que l’endomorphisme $v$ est compact. Soit B la boule unité de l’espace hilbertien $E_q$. Puisque $(1_E+u)^{1/2}$ est une application linéaire continue de $E_q$ dans E (cor. du th. 3 de IV, p. 294), le sous-ensemble $B'= (1_E+u)^{1/2}(B)$ de E est borné, donc le sous-ensemble $j(B) = B =v(B')$ est relativement compact dans E (remarque 1 de III, p. 2). Cela démontre que $j$ est compacte. Donc (ii) implique (iii).

L’application linéaire $\widetilde{v}:x\mapsto (1_E+u)^{-1/2}(x)$ de E dans $E_q$ est bien définie et isométrique (cor. du th. 3 de IV, p. 294). Comme $v=j\circ \widetilde{v}$, la condition (iii) implique (ii) (prop. 3 de III, p. 5).

#### Exemple {#ts-iv-s5-n12-exa-1 .statement tag=037B}

Soit $n\in \mathbf{N}$. Soit U un ouvert de $\mathbf{R}^n$. On munit U de la mesure de Lebesgue, notée $\mu$. Soit Δ l’opérateur différentiel scalaire $-\sum^n_{i=1}\partial_i^2$ sur U. L’opérateur partiel $\Delta_-$ de domaine $\mathscr{D}(U)$ défini par $\varphi \mapsto \Delta (\varphi )$ est fermable (prop. 13 de IV, p. 242) et symétrique (IV, p. 243). Il est positif, puisque pour tout $\varphi \in \mathscr{D}$(U), on a

$$
\langle \varphi |\Delta_-(\varphi )\rangle =\int_U\overline{\varphi}\Delta (\varphi )d\mu=-\sum_{i=1}^n\int_U\varphi  \partial_i^2\varphi  d\mu
$$

$$
=\sum_{i=1}^n\int_U\partial_i\varphi  \partial_i\varphi  d\mu=\int_U\sum_{i=1}^n|\partial_i\varphi |^2d\mu\geqslant 0
$$

On note $\Delta_D$ l’extension de Friedrichs de l’opérateur partiel positif symétrique $\Delta_-($IV, p. 295, exemple) ; c’est un laplacien sur U, appelé laplacien de Dirichlet sur U.

Soit $q$ la forme partielle positive associée à $\Delta_D$. Le domaine de $q$ est l’espace hilbertien complété de $\mathscr{D}(U)$ pour la forme hermitienne positive définie par

$$
(\varphi_1, \varphi_2)\mapsto \int_U\overline{\varphi}_1\varphi_2+\sum_{i=1}^n\int_U\overline{\partial_i\varphi_1}\partial_i\varphi_2
$$

pour tout $(\varphi_1, \varphi_2)\in \mathscr{D}(U)\times \mathscr{D}(U)$. Autrement dit, le domaine de $q$ est l’espace de Sobolev $H^1_0(U)$ (n$^o14$ de IV, p. 221).

*Supposons que U est borné. L’injection canonique de $H^1_0(U)$ dans $L^2(U)$ est compacte ; le laplacien de Dirichlet sur U est donc un opérateur à résolvante compacte (cor. de la prop. 20). Comme l’espace hilbertien $H^1_0(U)$ est de type dénombrable (prop. 20 de IV, p. 222), et comme l’image de $\Delta_D$ est de dimension infinie, il existe une suite croissante $(\lambda_n)_{n\geqslant 0}$ de nombre réels tendant vers $+\infty$ et une base orthonormale $(f_n)_{n\in\mathbf{N}}$ de $L^2$(U), dont les éléments appartiennent au domaine de $\Delta_D$, telle que $\Delta_D(f_n) =\lambda_nf_n$ pour tout $n\in \mathbf{N}$. On peut démontrer (« loi de Weyl ») que lorsque T tend vers $+\infty$, on a

$$
c_{nn/2}
$$

$$
\sum 1\sim mT
$$

$$
_{n\in\mathbf{N}}(2\pi )^n
$$

$\lambda_n\leqslant T$

où $c_n=\pi^{n/2}/\Gamma (1 +n/2)$ est le volume de la boule unité dans $\mathbf{R}^n$ (INT, V, p. 101, § 8, n$^o7)$ et $m >0$ est la mesure de Lebesgue de U.*

## EXERCICES {#ts-iv-s5-exercises}

Sauf mention du contraire, les espaces hilbertiens ci-dessous sont supposés complexes.

See the [exercises for § 5](exercises/s5/).
