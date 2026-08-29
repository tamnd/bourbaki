---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: GROUPES DE LIE RÉELS COMPACTS
section: 4
section_title: Système de racines associé à un groupe compact
lang: fr
source: lie-ix-fr
book_pages: LIE IX.24-LIE IX.43, LIE IX.112-LIE IX.118
pdf_pages: 0027-0046, 0115-0121
extraction: ocr
subsections:
    - "no": 1
      title: Le groupe $X(H)$
      page: 24
      pdf_page: 27
    - "no": 2
      title: Le groupe nodal d’un tore
      page: 25
      pdf_page: 28
    - "no": 3
      title: Poids d’une représentation linéaire
      page: 27
      pdf_page: 30
    - "no": 4
      title: Racines
      page: 29
      pdf_page: 32
    - "no": 5
      title: Vecteurs nodaux et racines inverses
      page: 31
      pdf_page: 34
    - "no": 6
      title: Groupe fondamental
      page: 34
      pdf_page: 37
    - "no": 7
      title: Sous-groupes de rang maximum
      page: 35
      pdf_page: 38
    - "no": 8
      title: Diagrammes radiciels
      page: 37
      pdf_page: 40
    - "no": 9
      title: Groupes de Lie compacts et diagrammes radiciels
      page: 38
      pdf_page: 41
    - "no": 10
      title: Automorphismes d’un groupe de Lie compact connexe
      page: 41
      pdf_page: 44
statements: 56
exercises: 22
content_sha256: c90a2a84199892fd556bed350e9419d303ab5ee816e98fb3406d94a18ae649e7
---

## § 4. SYSTÈME DE RACINES ASSOCIÉ À UN GROUPE COMPACT

Dans les paragraphes 4 à 8, on désigne par $G$ un groupe de Lie compact connexe et par $T$ un tore maximal de $G$. On note $g$ (resp. $t$) l’algèbre de Lie de $G$ (resp. $T$), $g_c$ (resp. $t_c$) l’algèbre de Lie complexifiée de $g$ (resp. $t$), et $W$ le groupe de Weyl de $G$ relativement à $T$ ($§ 2$, no 5).

### 1. Le groupe $X(H)$

Soit $H$ un groupe de Lie compact. On note $X(H)$ le groupe (commutatif) des homomorphismes continus de $H$ dans le groupe topologique $C^*$. D’après III, $§ 8$, no 1, th. 1, les éléments de $X(H)$ sont des morphismes de groupes de Lie ; pour tout $a \in X(H)$, la différentielle de $a$ est une application $\mathbf{R}$-linéaire $L(a) : L(H) \to L(C^*)$. Nous identifierons désormais l’algèbre de Lie de $C^*$ à $C$ de façon que l’application exponentielle de $C^*$ coïncide avec l’application $z \mapsto e^z$ de $C$ dans $C^*$. A tout élément $a$ de $X(H)$ est alors associé un élément $L(a) \in \mathrm{Hom}_{\mathbf{R}}(L(H), C)$; on note $\delta(a)$ l’élément de $\mathrm{Hom}_C(L(H)_c, C)$ qui lui correspond (c’est-à-dire dont la restriction à $L(H) \subset L(H)_c$ est égale à $L(a)$).

Pour tout $x \in L(H)$ et tout $a \in X(H)$, on a
$$
a(\exp_H x) = e^{\delta(a)(x)},
$$
par fonctorialité de l’application exponentielle (III, $§ 6$, no 4, prop. 10).

On notera le plus souvent additivement le groupe $X(H)$; en ce cas, on notera $g^a$ l’élément $a(g)$ de $C^*$. Avec cette notation, on a les formules
$$
g^{a+b} = g^a g^b,\quad g \in H,\quad a, b \in X(H),
$$
et
$$
(\exp_H x)^a = e^{\delta(a)(x)},\quad x \in L(H),\quad a \in X(H).
$$

Puisque $H$ est compact, les éléments de $X(H)$ prennent leurs valeurs dans le sous-groupe $U = U(1, C)$ des nombres complexes de valeur absolue 1, de sorte que $X(H)$ s’identifie au groupe des homomorphismes continus (ou analytiques) de $H$ dans $U$. Il en résulte que, pour tout $a \in L(H)$, l’application $L(a)$ prend ses valeurs dans le sous-espace $Ri$ de $C$, donc $\delta(a)$ applique $L(H)$ dans $Ri$.

Si $H$ est commutatif, $X(H)$ n’est autre que le groupe (discret) dual de $H$ (TS, II, $§ 1$, no 1). Si $H$ est commutatif et fini, $X(H)$ s’identifie au groupe fini dual $D(H) = \mathrm{Hom}_\mathbf{Z}(H, \mathbf{Q}/\mathbf{Z})$ (où conformément à A, VII, p. 27, exemple 1, on identifie $\mathbf{Q}/\mathbf{Z}$ à un sous-groupe de $C^*$ par l’homomorphisme $r \mapsto \exp(2\pi i r)$).

Pour tout morphisme $f : H \to H'$ de groupes de Lie compacts, on note $X(f)$ l’homomorphisme $a \mapsto a \circ f$ de $X(H')$ dans $X(H)$. Si $K$ est un sous-groupe distingué fermé du groupe de Lie compact $H$, on a une suite exacte de $\mathbf{Z}$-modules $0 \to X(H/K) \to X(H) \to X(K)$.

#### Proposition 1 {#lie-ix-s4-prop-1 .statement tag=01JH}

*Pour tout groupe de Lie compact* $H$, le *$\mathbf{Z}$-module* $X(H)$ *est de type fini*. *Il est libre si* $H$ *est connexe*.

Supposons d’abord $H$ connexe ; tout élément de $X(H)$ s’annule sur le groupe dérivé $D(H)$ de $H$, d’où un isomorphisme $X(H/D(H)) \to X(H)$. Mais $H/D(H)$ est connexe et commutatif, donc est un tore, et $X(H/D(H))$ est un $\mathbf{Z}$-module libre de type fini (TS, II, § 2, no 1, cor. 2 à la prop. 1). Dans le cas général, il résulte de l’exactitude de la suite

$$
0 \to X(H/H_0) \to X(H) \to X(H_0),
$$

où $X(H_0)$ est libre de type fini et $X(H/H_0)$ fini, que $X(H)$ est de type fini.

#### Proposition 2 {#lie-ix-s4-prop-2 .statement tag=01JI}

*Soient* $H$ *un groupe de Lie compact commutatif*, et $(a_i)_{i \in I}$ *une famille d’éléments de* $X(H)$; *pour que les* $a_i$ *engendrent* $X(H)$, *il faut et il suffit que l’intersection des* $\mathrm{Ker}\ a_i$ *soit réduite à l’élément neutre*.

D’après TS, II, § 1, no 7, th. 4, l’orthogonal du noyau de $a_i$ est le sous-groupe $A_i$ de $X(H)$ engendré par $a_i$; d’après *loc. cit.*, cor. 2 au th. 4, l’orthogonal de $\bigcap \mathrm{Ker}\ a_i$ est le sous-groupe de $X(H)$ engendré par les $A_i$, d’où la proposition.

### 2. Le groupe nodal d’un tore

On appelle *groupe nodal* du tore $S$ et on note $\Gamma(S)$ le noyau de l’application exponentielle $L(S) \to S$. C’est un sous-groupe discret de $L(S)$, dont le rang est égal à la dimension de $S$, et l’application $\mathbf{R}$-linéaire $\mathbf{R} \otimes_{\mathbf{Z}} \Gamma(S) \to L(S)$ qui prolonge l’injection canonique de $\Gamma(S)$ dans $L(S)$ est bijective. Elle induit par passage au quotient un isomorphisme $\mathbf{R}/\mathbf{Z} \otimes_{\mathbf{Z}} \Gamma(S) \to S$.

Par exemple, le groupe nodal $\Gamma(U)$ de $U$ est le sous-groupe $2\pi i \mathbf{Z}$ de $L(U) = i\mathbf{R}$.

Pour tout morphisme $f : S \to S'$ de tores, on note $\Gamma(f)$ l’homomorphisme $\Gamma(S) \to \Gamma(S')$ déduit de $L(f)$. On a un diagramme commutatif

$$
\begin{array}{ccccccccc}
0 & \to & \Gamma(S) & \to & L(S) & \xrightarrow{\exp_s} & S & \to & 0 \\
& & \downarrow_{\Gamma(f)} & & \downarrow_{L(f)} & & \downarrow_f & & \\
0 & \to & \Gamma(S') & \to & L(S') & \xrightarrow{\exp_{s'}} & S' & \to & 0 .
\end{array}
$$

Soit $a \in X(S)$; appliquant ce qui précède au morphisme de $S$ dans $U$ défini par $a$, on voit que l’application $\mathbf{C}$-linéaire $\delta(a) : L(S)_{(c)} \to \mathbf{C}$ du no 1 applique $\Gamma(S)$ dans $2\pi i \mathbf{Z}$. On définit donc une forme *$\mathbf{Z}$*-*bilinéaire* sur $X(S) \times \Gamma(S)$ en posant

$$
\langle a, X \rangle = \frac{1}{2\pi i} \delta(a)(X), \quad a \in X(S), \quad X \in \Gamma(S).
$$

#### Proposition 3 {#lie-ix-s4-prop-3 .statement tag=01BP}

*La forme bilinéaire* $(a, X) \mapsto \langle a, X \rangle$ sur $X(S) \times \Gamma(S)$ est *inversible*.

Rappelons (A, IX) que par définition cela signifie que les applications linéaires $X(S) \to \mathrm{Hom}_{\mathbf{Z}}(\Gamma(S), \mathbf{Z})$ et $\Gamma(S) \to \mathrm{Hom}_{\mathbf{Z}}(X(S), \mathbf{Z})$ associées à cette forme bilinéaire sont bijectives.

On voit aussitôt que si la conclusion de la proposition est vraie pour deux tores, elle est aussi vraie pour leur produit. Comme tout tore de dimension $n$ est isomorphe à $\mathbf{U}^n$, on est donc ramené au cas où $S = \mathbf{U}$. Dans ce cas particulier, l’assertion est immédiate.

Soit $f : S \to S'$ un morphisme de tores. Alors les applications linéaires $X(f) : X(S') \to X(S)$ et $\Gamma(f) : \Gamma(S) \to \Gamma(S')$ sont transposées l’une de l’autre : pour tout $a' \in X(S')$ et tout $X \in \Gamma(S)$, on a
$$
\langle X(f)(a'), X \rangle = \langle a', \Gamma(f)(X) \rangle .
$$

#### Proposition 4 {#lie-ix-s4-prop-4 .statement tag=01BQ}

*Soient S et S' deux tores. Notons M(S, S') le groupe des morphismes de groupes de Lie de S dans S'. Les applications $f \mapsto X(f)$ et $f \mapsto \Gamma(f)$ sont des isomorphismes de groupes de M(S, S') sur $\mathrm{Hom}_{\mathbf{Z}}(X(S'), X(S))$ et $\mathrm{Hom}_{\mathbf{Z}}(\Gamma(S), \Gamma(S'))$ respectivement.*

Si $f$ est un morphisme de groupes de Lie de S dans S', l’homomorphisme $X(f)$ n’est autre que l’homomorphisme *dual* de $f$ au sens de TS, II, § 1, no 7. L’application $\varphi \mapsto \hat{\varphi}$ de $\mathrm{Hom}_{\mathbf{Z}}(X(S'), X(S))$ dans $M(S, S')$ définie dans *loc. cit.* est réciproque de l’application $f \mapsto X(f)$ de $M(S, S')$ dans $\mathrm{Hom}_{\mathbf{Z}}(X(S'), X(S))$ ; cette dernière est donc bijective. Si l’on identifie $\Gamma(S)$ (resp. $\Gamma(S')$) au $\mathbf{Z}$-module dual de $X(S)$ (resp. $X(S')$) (prop. 3), $\Gamma(f)$ coïncide avec l’homomorphisme transposé de $X(f)$, d’où la proposition.

*Remarques. — 1) Soit $f : S \to S'$ un morphisme de tores. Le diagramme du serpent (A, X, § 1, no 2) associé à (1) donne une suite exacte*
$$
\begin{array}{ccccccccc}
0 & \longrightarrow & \mathrm{Ker}\ \Gamma(f) & \longrightarrow & \mathrm{Ker}\ L(f) & \longrightarrow & \mathrm{Ker}\ f & \xrightarrow{d} & \mathrm{Coker}\ \Gamma(f) \\
& & & & & & & & \longrightarrow \mathrm{Coker}\ L(f) \longrightarrow \mathrm{Coker}\ f \longrightarrow 0 .
\end{array}
$$
En particulier, supposons $f$ surjectif, de noyau fini N, de sorte qu’on a la suite exacte
$$
0 \longrightarrow N \xrightarrow{i} S \xrightarrow{f} S' \longrightarrow 0 ,
$$
où $i$ est l’injection canonique. Alors $L(f)$ est bijectif, et on tire de (4) un isomorphisme $N \to \mathrm{Coker}\ \Gamma(f)$, d’où une suite exacte
$$
0 \to \Gamma(S) \xrightarrow{\Gamma(f)} \Gamma(S') \to N \to 0 .
$$
Par ailleurs, d’après TS, II, § 1, no 7, th. 4, la suite
$$
0 \to X(S') \xrightarrow{X(f)} X(S) \xrightarrow{X(i)} X(N) \to 0
$$
est exacte.

2) D’après la prop. 4, l’application $f \mapsto \Gamma(f)(2\pi i)$ de $M(U, S)$ dans $\Gamma(S)$ est un isomorphisme ; si $a \in X(S) = M(S, U)$ et $f \in M(U, S)$, alors le composé $a \circ f \in M(U, U)$ est l’endomorphisme $u \mapsto u^r$, où $r = \langle a, \Gamma(f)(2\pi i) \rangle$. On identifiera dans la suite $M(U, U) = X(U)$ à $\mathbf{Z}$, l’élément $r$ de $\mathbf{Z}$ étant associé à l’endomorphisme $u \mapsto u^r$; avec les notations ci-dessus, on a donc
$$
a \circ f = \langle a, \Gamma(f)(2\pi i) \rangle .
$$
3) À la suite exacte $0 \to \Gamma(S) \to L(S) \xrightarrow{\exp s} S \to 0$, est associé un isomorphisme de $\Gamma(S)$ sur le groupe fondamental de $S$, dit dans la suite canonique. Pour tout morphisme $f : S \to S'$ de tores, $\Gamma(f)$ s’identifie par les isomorphismes canoniques $\Gamma(S) \to \pi_1(S)$ et $\Gamma(S') \to \pi_1(S')$ à l’homomorphisme $\pi_1(f) : \pi_1(S) \to \pi_1(S')$ déduit de $f$. Cela donne notamment une autre interprétation de la suite exacte (5) (cf. TG, XI, à paraître).
4) Les homomorphismes de $\mathbf{Z}$-modules $\delta : X(S) \to \mathrm{Hom}_C(L(S)_{(C)}, C)$ et $\iota : \Gamma(S) \to L(S)_{(C)}$ ($\iota$ est déduit de l’injection canonique de $\Gamma(S)$ dans $L(S)$) se prolongent en des isomorphismes de $C$-espaces vectoriels
$$
u : C \otimes X(S) \to \mathrm{Hom}_C(L(S)_{(C)}, C)
$$
$$
v : C \otimes \Gamma(S) \to L(S)_{(C)}
$$
que nous appellerons dans la suite canoniques. On notera que, si l’on étend par $C$-linéarité l’accouplement entre $X(S)$ et $\Gamma(S)$ en une forme bilinéaire $\ll , \gg$ sur $(C \otimes X(S)) \times (C \otimes \Gamma(S))$, on a
$$
\langle u(a), v(b) \rangle = 2\pi i \ll a, b \gg .
$$

### 3. Poids d’une représentation linéaire

Dans ce numéro, on désigne par $k$ l’un des corps $\mathbf{R}$ ou $\mathbf{C}$.
Soient $V$ un espace vectoriel sur $k$ de dimension finie, et $\rho : G \to \mathrm{GL}(V)$ une représentation continue (donc analytique réelle, III, § 8, no 1, th. 1) du groupe de Lie compact connexe $G$ dans $V$. Définissons un espace vectoriel complexe $\tilde{V}$ et une représentation continue $\tilde{\rho} : G \to \mathrm{GL}(\tilde{V})$ comme suit : si $k = \mathbf{C}$, on pose $\tilde{V} = V$, $\tilde{\rho} = \rho$; si $k = \mathbf{R}$, on pose $\tilde{V} = V_{(C)}$, et $\tilde{\rho}$ est le composé de $\rho$ et de l’homomorphisme canonique $\mathrm{GL}(V) \to \mathrm{GL}(\tilde{V})$.
Pour tout $\lambda \in X(G)$, on note $\tilde{V}_\lambda(G)$ le sous-espace vectoriel de $\tilde{V}$ formé des $v \in \tilde{V}$ tels que $\tilde{\rho}(g)v = g^\lambda v$ pour tout $g \in G$ (cf. VII, § 1, no 1). D’après loc. cit., prop. 3, la somme des $\tilde{V}_\lambda(G)$ (pour $\lambda$ parcourant $X(G)$) est directe. De plus :

#### Lemme 1 {#lie-ix-s4-lem-1 .statement tag=01BV}

Si $G$ est commutatif, $\tilde{V}$ est la somme directe des $\tilde{V}_\lambda(G)$ pour $\lambda \in X(G)$.
Comme $\rho$ est semi-simple (§ 1, no 1), il suffit de démontrer le lemme dans le cas où $\rho$ est simple. En ce cas, le commutant $Z$ de $\rho(G)$ dans $\mathrm{End}(\tilde{V})$ est réduit aux homothéties (A, VIII, § 3, no 2, th. 1); l’homomorphisme $\tilde{\rho}$ se factorise donc par le sous-groupe $C^*.1_V$ de $\mathrm{GL}(\tilde{V})$, et il existe $\lambda \in X(G)$ tel que $\tilde{V} = \tilde{V}_\lambda(G)$.

#### Définition 1 {#lie-ix-s4-def-1 .statement tag=01BW}

On appelle poids de la représentation $\rho$ de $G$, relativement au tore maximal $T$ de $G$, les éléments $\lambda$ de $X(T)$ tels que $\tilde{V}_\lambda(T) \neq 0$.

On note $P(\rho, T)$, ou $P(\rho)$ s'il n'y a aucune confusion possible sur le choix de $T$, l'ensemble des poids de $\rho$ relativement à $T$. On a d'après le lemme 1

(7)
$$
\tilde{V} = \bigoplus_{\lambda \in P(\rho, T)} \tilde{V}_\lambda(T).
$$

Soient $T'$ un autre tore maximal de $G$ et $g$ un élément de $G$ tel que $(\mathrm{Int}\, g)\, T = T'$ (§ 2, no 2, th. 2). Pour tout $\lambda \in X(T)$, on a

(8)
$$
\tilde{\rho}(g)\, (\tilde{V}_\lambda(T)) = \tilde{V}_{\lambda'}(T'), \quad \text{où} \quad \lambda' = X(\mathrm{Int}\, g^{-1})\, (\lambda).
$$

Par conséquent

(9)
$$
X(\mathrm{Int}\, g)\, (P(\rho, T')) = P(\rho, T).
$$

Le groupe de Weyl $W = W_G(T)$ opère à gauche sur le $\mathbf{Z}$-module $X(T)$ par l'opération $w \mapsto X(w^{-1})$; pour $t \in T, \lambda \in X(T), w \in W$, on a donc $t^{w\lambda} = (w^{-1}(t))^{\lambda}$.

#### Proposition 5 {#lie-ix-s4-prop-5 .statement tag=01BX}

L'ensemble $P(\rho, T)$ est stable pour l'opération du groupe de Weyl $W$. Soit $n \in N_G(T)$, et soit $w$ sa classe dans $W$; pour $\lambda \in X(T)$, on a $\rho(n)\, (\tilde{V}_\lambda(T)) = \tilde{V}_{w\lambda}(T)$ et $\dim \tilde{V}_{w\lambda}(T) = \dim \tilde{V}_\lambda(T)$.

La formule (9), avec $T' = T, g = n$, entraîne que $P(\rho, T)$ est stable par $w$; de plus $\tilde{\rho}(n)$ induit un isomorphisme de $\tilde{V}_\lambda(T)$ sur $\tilde{V}_{w\lambda}(T)$ (formule (8)), d'où la proposition.

#### Proposition 6 {#lie-ix-s4-prop-6 .statement tag=01BY}

Pour que l'homomorphisme $\rho : G \to \mathbf{GL}(V)$ soit injectif, il faut et il suffit que $P(\rho, T)$ engendre le $\mathbf{Z}$-module $X(T)$.

Pour que $\rho$ soit injectif, il est nécessaire et suffisant que sa restriction à $T$ le soit (§ 2, no 6, prop. 9). Par ailleurs, comme l'homomorphisme canonique $\mathbf{GL}(V) \to \mathbf{GL}(\tilde{V})$ est injectif, on peut remplacer $\rho$ par $\tilde{\rho}$. Il résulte alors de (7) que le noyau de la restriction de $\rho$ à $T$ est l'intersection des noyaux des éléments de $P(\rho, T)$. La conclusion résulte donc de la prop. 2 du no 1.

La représentation linéaire $L(\rho)$ de $t$ dans $\mathrm{gl}(\tilde{V})$ s'étend en un homomorphisme de C-algèbres de Lie
$$
\tilde{L}(\rho) : t_\mathbf{C} \to \mathrm{gl}(\tilde{V}).
$$
Rappelons par ailleurs qu'à tout élément $\lambda$ de $X(T)$ a été associée (no 1) une forme linéaire $\delta(\lambda)$ sur $t_\mathbf{C}$ telle que
(10)
$$
(\exp_T x)^{\lambda} = e^{\delta(\lambda)(x)}, \quad x \in t.
$$
Rappelons enfin (VII, § 1, no 1) que pour toute application $\mu : t_\mathbf{C} \to \mathbf{C}$, on note $\tilde{V}_\mu(t_\mathbf{C})$ le sous-espace vectoriel de $\tilde{V}$ formé des $v$ tels que $(\tilde{L}(\rho)(u))(v) = \mu(u).v$ pour tout $u \in t_\mathbf{C}$.

On déduit alors de (7) et de loc. cit., prop. 3 :

#### Proposition 7 {#lie-ix-s4-prop-7 .statement tag=01BZ}

a) Pour tout $\lambda \in X(T)$, on a $\tilde{V}_\lambda(T) = \tilde{V}_{\delta(\lambda)}(t_c)$.

b) L’application $\delta : X(T) \to \mathrm{Hom}_c(t_c, C)$ induit une bijection de $P(\rho, T)$ sur l’ensemble des poids de $t_c$ dans $\tilde{V}$.

Notons d’ailleurs que, si l’on fait opérer W sur $t_c$ en associant à tout élément $w$ de W l’endomorphisme $L(w)_{(c)}$ de $t_c$, l’application $\delta$ est compatible avec l’action de W sur $X(T)$ et $\mathrm{Hom}_c(t_c, C)$.

Supposons maintenant $k = \mathbf{R}$. Notons $\sigma$ la conjugaison de $\tilde{V}$ relativement à V, définie par $\sigma(x + iy) = x - iy$ pour $x, y$ dans V ; pour tout sous-espace vectoriel complexe E de $\tilde{V}$, le plus petit sous-espace rationnel sur $\mathbf{R}$ de $\tilde{V}$ contenant E est $E + \sigma(E)$. En particulier, pour tout $\lambda \in X(T)$, il existe un sous-espace vectoriel réel $V(\lambda)$ de V tel que le sous-espace $V(\lambda)_{(c)}$ de $\tilde{V}$ soit $\tilde{V}_\lambda(T) + \tilde{V}_{-\lambda}(T)$ (noter que $\sigma(\tilde{V}_\lambda(T)) = \tilde{V}_{-\lambda}(T)$). On a $V(\lambda) = V(-\lambda)$, et les $V(\lambda)$ sont les composants isotypiques de la représentation de T dans V déduite de $\rho$.

### 4. Racines

On appelle racines de G relativement à T les poids non nuls de la représentation adjointe de G. L’ensemble des racines de G relativement à T est noté $R(G, T)$, ou simplement R s’il n’y a pas de confusion possible. D’après la prop. 6, l’application

$$
\delta : X(T) \to t_c^*
$$

(on note $t_c^*$ le dual de l’espace vectoriel complexe $t_c$) applique bijectivement $R(G, T)$ sur l’ensemble $R(g_c, t_c)$ des racines de l’algèbre réductive déployée $(g_c, t_c)$ (VIII, § 2, no 2, remarque 4). Si l’on pose, pour tout $\alpha \in \mathbf{R}$

$$
g^\alpha = (g_c)_\alpha(T) = (g_c)_{\delta(\alpha)}(t_c),
$$

chaque $g^\alpha$ est de dimension 1 sur $\mathbf{C}$ (loc. cit., th. 1) et on a

$$
g_c = t_c \oplus \bigoplus_{\alpha \in \mathbf{R}} g^\alpha.
$$

Pour chaque $\alpha \in \mathbf{R}$, désignons par $V(\alpha)$ le sous-espace de dimension 2 de g tel que $V(\alpha)_{(c)} = g^\alpha + g^{-\alpha}$; les composants isotypiques non nuls de g pour la représentation adjointe de T sont t et les $V(\alpha)$. Soit par ailleurs K la forme quadratique associée à la forme de Killing de g ; elle est négative (§ 1, no 3, prop. 1) et sa restriction $K(\alpha)$ à $V(\alpha)$ est négative et séparante. Pour chaque élément $t$ de T, Ad $t$ laisse stable $K(\alpha)$, d’où un morphisme de groupes de Lie

$$
\iota_\alpha : T \to \mathrm{SO}(K(\alpha)).
$$

Il existe alors un unique isomorphisme $\rho_\alpha : U \to \mathrm{SO}(K(\alpha))$ tel que $\iota_\alpha = \rho_\alpha \circ \alpha$. En effet, soit $X$ un élément non nul de $g^\alpha$, et soit $Y$ l’image de $X$ par la conjugaison de $g_c$ relativement à g ; alors $Y \in g^{-\alpha}$, et on obtient une base $(U, V)$ de $V(\alpha)$ en posant $U = X + Y, V = i(X - Y)$; sur la base $(U, V)$, la matrice de l’endomorphisme de $V(\alpha)$ induit par $Ad\ t,\ t \in T$, est

$$
\begin{pmatrix}
\mathcal{R}(t^\alpha) & -\mathcal{I}(t^\alpha) \\
\mathcal{I}(t^\alpha) & \mathcal{R}(t^\alpha)
\end{pmatrix},
$$

d’où l’assertion.

#### Proposition 8 {#lie-ix-s4-prop-8 .statement tag=01C0}

*Soit Q(R) le sous-groupe de X(T) engendré par les racines de G.*

a) *Le centre C(G) de G est un sous-groupe fermé de T, égal à l’intersection des noyaux des racines. L’application canonique $X(T/C(G)) \to X(T)$ est injective et d’image Q(R).*

b) *Le groupe compact C(G) est isomorphe au dual du groupe discret X(T)/Q(R)* (TS, II, § 1, no 1, déf. 2).

c) *Pour que C(G) soit réduit à l’élément neutre, il faut et il suffit que Q(R) soit égal à X(T).*

D’après § 2, no 2, cor. 2 au th. 2, C(G) est contenu dans T. Comme c’est le noyau de la représentation adjointe, c’est l’intersection des noyaux des racines, c’est-à-dire l’orthogonal du sous-groupe Q(R) de X(T). La proposition résulte alors de TS, II, § 1, no 7, th. 4 et no 5, th. 2.

#### Proposition 9 {#lie-ix-s4-prop-9 .statement tag=01C1}

*Tout automorphisme du groupe de Lie G qui induit l’identité sur T est de la forme Int t, avec $t \in T$.*

Supposons d’abord C(G) réduit à l’élément neutre, c’est-à-dire $X(T) = Q(R)$ (prop. 8). Soient $f$ un automorphisme de G induisant l’identité sur T, et $\varphi = L(f)_{(c)}$; alors $\varphi$ est un automorphisme de $g_c$ induisant l’identité sur $t_c$. D’après VIII, § 5, no 2, prop. 2, il existe un unique homomorphisme $\theta : Q(R) \to \mathbf{C}^*$ tel que $\varphi$ induise sur chaque $g^\alpha$ l’homothétie de rapport $\theta(\alpha)$. Comme $\varphi$ laisse stable la forme réelle g de $g_c$, il commute à la conjugaison $\sigma$ de $g_c$ par rapport à g ; mais on a $\sigma(g^\alpha) = g^{-\alpha}$, donc $\theta(-\alpha) = \overline{\theta(\alpha)}$ pour tout $\alpha \in R$. Cela implique $\theta(\alpha)\ \overline{\theta(\alpha)} = \theta(\alpha)\ \theta(-\alpha) = 1$. Il en résulte que $\theta$ est à valeurs dans U, donc correspond par dualité à un élément $t$ de T tel que $(Ad\ t)_{(c)} = \varphi$, donc Int $t = f$.

Dans le cas général, ce qui précède s’applique au groupe $G/C(G)$, dont le centre est réduit à l’élément neutre, et à son tore maximal $T/C(G)$. On en déduit que, si $f$ est un automorphisme de G induisant l’identité sur T, il existe un élément $t$ de T tel que $f$ et Int $t$ induisent par passage au quotient le même automorphisme de $G/C(G)$. Alors, comme le morphisme canonique $D(G) \to G/C(G)$ est un revêtement fini (\§ 1, no 4, cor. 1 à la prop. 4), $f$ et Int $t$ induisent le même automorphisme de $D(G)$, donc de $D(G) \times C(G)$, donc aussi de G (*loc. cit.*).

#### Corollaire {#lie-ix-s4-n4-cor-1 .statement tag=01C2}

*Soient u un automorphisme de G et H le sous-groupe fermé de G formé des points fixes de u. Pour que l’automorphisme u soit intérieur, il faut et il suffit que $H_0$ soit de rang maximum.*

Si $u$ est égal à Int $g$, avec $g \in G$, le sous-groupe $H_0 = Z(g)_0$ est de rang maximum ($\S$ 2, no 2, cor. 3). Inversement, si $H$ contient un tore maximal $S$, l’automorphisme $u$ est de la forme Int $s$ avec $s \in S$ (prop. 9).

### 5. Vecteurs nodaux et racines inverses

#### Lemme 2 {#lie-ix-s4-lem-2 .statement tag=01C3}

Soient $S$ un sous-groupe fermé de $T$ et $Z(S)$ son centralisateur dans $G$.
(i) $R(Z(S)_0, T)$ est l’ensemble des $\alpha \in R(G, T)$ tels que $\alpha(S) = \{ 1 \}$;
(ii) Le centre de $Z(S)_0$ est l’intersection des Ker $\alpha$ pour $\alpha \in R(Z(S)_0, T)$;
(iii) Si $S$ est connexe, $Z(S)$ est connexe.

L’algèbre de Lie $L(Z(S))_{(C)}$ est formée des invariants de $S$ dans $g_C$ (III, $\S$ 9, no 3, prop. 8), donc est somme directe de $t_C$ et des $g^\alpha$ pour lesquels $\alpha(S) = \{ 1 \}$, d’où (i). L’assertion (ii) résulte alors de la prop. 8 (no 4), et l’assertion (iii) a déjà été démontrée ($\S$ 2, no 2, cor. 5 au th. 2).

#### Théorème 1 {#lie-ix-s4-thm-1 .statement tag=01C4}

Soit $\alpha \in R(G, T)$. Le centralisateur $Z_\alpha$ du noyau de $\alpha$ est un sous-groupe fermé connexe de $G$; son centre est Ker $\alpha$; son groupe dérivé $D(Z_\alpha) = S_\alpha$ est un sous-groupe fermé connexe semi-simple de rang 1 de $G$. On a $R(Z_\alpha, T) = \{ \alpha, -\alpha \}$ et $\dim Z_\alpha = \dim T + 2$.

Soit $Z'_\alpha$ le centralisateur de $(\mathrm{Ker}\ \alpha)_0$. D’après le lemme 2, c’est un sous-groupe fermé connexe de $G$, et $R(Z'_\alpha, T)$ est l’ensemble des $\beta \in R(G, T)$ tels que $\beta((\mathrm{Ker}\ \alpha)_0) = \{ 1 \}$. On a évidemment $\{ \alpha, -\alpha \} \subset R(Z'_\alpha, T)$. Inversement, soit $\beta \in R(Z'_\alpha, T)$; puisque $(\mathrm{Ker}\ \alpha)_0$ est d’indice fini dans Ker $\alpha$, il existe un entier $r \neq 0$ tel que $t^{r\beta} = 1$ pour $t \in \mathrm{Ker}\ \alpha$. De l’exactitude de la suite

$$
0 \to Z \to X(T) \to X(\mathrm{Ker}\ \alpha) \to 0
$$

correspondant par dualité à la suite exacte

$$
0 \to \mathrm{Ker}\ \alpha \to T \xrightarrow{\alpha} U \to 0,
$$

il résulte que $r\beta$ est un multiple de $\alpha$; d’après VIII, $\S$ 2, no 2, th. 2, (i), cela implique $\beta \in \{ \alpha, -\alpha \}$. On a donc $R(Z'_\alpha, T) = \{ \alpha, -\alpha \}$. Il s’ensuit (lemme 2) que le centre de $Z'_\alpha$ est Ker $\alpha$, donc que $Z'_\alpha = Z_\alpha$. Enfin, d’après le cor. 1 à la prop. 4 ($\S$ 1, no 4), $D(Z_\alpha)$ est un sous-groupe fermé connexe semi-simple de $G$; il est de rang 1 puisque $\mathcal{D}L(Z_\alpha)_{(C)} = g^\alpha + g^{-\alpha} + [g^\alpha, g^{-\alpha}]$.

#### Corollaire {#lie-ix-s4-n5-cor-1 .statement tag=01C7}

Il existe un morphisme de groupes de Lie $v : \mathbf{SU}(2, C) \to G$ ayant les propriétés suivantes :
a) L’image de $v$ et le noyau de $\alpha$ commutent.
b) Pour tout $a \in U$, on a $v \begin{pmatrix} a & 0 \\ 0 & \overline{a} \end{pmatrix} \in T$ et $\alpha \circ v \begin{pmatrix} a & 0 \\ 0 & \overline{a} \end{pmatrix} = a^2$.

Si $v_1$ et $v_2$ sont deux morphismes de $\mathbf{SU}(2, C)$ dans $G$ possédant les propriétés précédentes, il existe $a \in U$ tel que $v_2 = v_1 \circ \mathrm{Int} \begin{pmatrix} a & 0 \\ 0 & \overline{a} \end{pmatrix}$.

D’après le th. 1 et la prop. 6 du § 3, no 6, il existe un morphisme de groupes de Lie $\nu : \mathrm{SU}(2, \mathbf{C}) \to S_\alpha$, surjectif à noyau discret. Alors $\nu^{-1}(T \cap S_\alpha)$ est un tore maximal de $\mathrm{SU}(2, \mathbf{C})$ ($§ 2$, no 3, prop. 1). Puisque les tores maximaux de $\mathrm{SU}(2, \mathbf{C})$ sont conjugués ($§ 2$, no 2, th. 2), on peut supposer, quitte à remplacer $\nu$ par $\nu \circ \mathrm{Int}\ s$ (avec $s \in \mathrm{SU}(2, \mathbf{C})$), que $\nu^{-1}(T \cap S_\alpha)$ est le groupe des matrices diagonales de $\mathrm{SU}(2, \mathbf{C})$. On a alors $\nu \begin{pmatrix} a & 0 \\ 0 & \overline{a} \end{pmatrix} \in T$ pour tout $a \in U$, et l’application

$$
\begin{pmatrix} a & 0 \\ 0 & \overline{a} \end{pmatrix} \mapsto \alpha \circ \nu \begin{pmatrix} a & 0 \\ 0 & \overline{a} \end{pmatrix}
$$

est une racine de $\mathrm{SU}(2, \mathbf{C})$, donc est égale à l’une des deux applications $\begin{pmatrix} a & 0 \\ 0 & \overline{a} \end{pmatrix} \mapsto a^2$ ou $\begin{pmatrix} a & 0 \\ 0 & \overline{a} \end{pmatrix} \mapsto a^{-2}$ ($§ 3$, no 6, formules (19)). Dans le premier cas, l’homomorphisme $\nu$ convient ; dans le second cas, l’homomorphisme $\nu \circ \mathrm{Int}\ \theta$ convient (*loc. cit.*, formules (18)).

Si $\nu_1$ et $\nu_2$ sont deux morphismes de $\mathrm{SU}(2, \mathbf{C})$ dans $G$ répondant aux conditions exigées, ils appliquent tous deux $\mathrm{SU}(2, \mathbf{C})$ dans $S_\alpha$ (condition *a*)), donc sont tous deux des revêtements universels de $S_\alpha$. Il existe donc un automorphisme $\varphi$ de $\mathrm{SU}(2, \mathbf{C})$ tel que $\nu_2 = \nu_1 \circ \varphi$, et on conclut par la prop. 9 du no 4.

Il résulte du corollaire précédent que l’homomorphisme $\nu_T$ de $U$ dans $T$, défini par $\nu_T(a) = \nu \begin{pmatrix} a & 0 \\ 0 & \overline{a} \end{pmatrix}$ pour $a \in U$, est indépendant du choix de $\nu$. On note $K_\alpha \in \Gamma(T)$ l’image par $\Gamma(\nu_T)$ de l’élément $2\pi i$ de $\Gamma(U) = 2\pi i \mathbf{Z}$; on dit que c’est le *vecteur nodal associé à la racine* $\alpha$. On a $\langle \alpha, K_\alpha \rangle = 2$, c’est-à-dire (no 2, formule (2)) $\delta(\alpha)(K_\alpha) = 4\pi i$; comme $K_\alpha$ appartient à l’intersection de $t$ et de $L(S_\alpha)_\mathbf{C}$, on a donc

$$
K_\alpha = 2\pi i H_{\delta(\alpha)},
$$

où $H_{\delta(\alpha)}$ est la *racine inverse* associée à la racine $\delta(\alpha)$ de $(g_\mathbf{C}, t_\mathbf{C})$ (VIII, § 2, no 2). Autrement dit, lorsqu’on identifie $\Gamma(T) \otimes \mathbf{R}$ au dual de $X(T) \otimes \mathbf{R}$ *via* l’accouplement $\langle \ , \ \rangle$, $K_\alpha$ s’identifie à la *racine inverse* $\alpha^\vee \in (X(T) \otimes \mathbf{R})^*$.

#### Remarque {#lie-ix-s4-n5-rem-1 .statement tag=01C5}

Pour tout $x \in \mathbf{R}$, on a

$$
\nu \begin{pmatrix} \exp(2\pi i x) & 0 \\ 0 & \exp(-2\pi i x) \end{pmatrix} = \nu_T(e^{2\pi i x}) = \exp(x K_\alpha).
$$

En particulier :

$$
\nu \begin{pmatrix} -1 & 0 \\ 0 & -1 \end{pmatrix} = \nu_T(-1) = \exp(\frac{1}{2} K_\alpha).
$$

Il en résulte que $\nu$ est *injectif* si et seulement si $K_\alpha \notin 2\Gamma(T)$, c’est-à-dire s’il existe $\lambda \in X(T)$ tel que $\langle \lambda, K_\alpha \rangle \notin 2\mathbf{Z}$. Lorsque $g_\mathbf{C}$ est simple, $\nu$ est injectif sauf lorsque $g_\mathbf{C}$ est de type $B_n$, $C(G) = \{1\}$ et $\alpha$ est une racine courte (*cf.* VI, planches).

On note dans la suite de ce paragraphe $R^\vee(G, T)$ l’ensemble des vecteurs nodaux $K_\alpha$ pour $\alpha \in R(G, T)$. C’est une partie de $\Gamma(T)$ que l’injection canonique de $\Gamma(T)$ dans $t_C$ identifie à l’homothétique de rapport $2\pi i$ du système de racines inverse $R^\vee(g_C, t_C) = \{ H_{\delta(\alpha)} \}$ de $\delta(R)$. Il en résulte que $R^\vee(G, T)$ engendre le $\mathbf{R}$-espace vectoriel $L(T \cap D(G))$, donc que son orthogonal dans $X(T)$ est $X(T/(T \cap D(G)))$.

Notons $\mathrm{Aut}(T)$ le groupe des automorphismes du groupe de Lie $T$; le groupe de Weyl $W = W_G(T)$ (§ 2, no 5) s’identifie à un sous-groupe de $\mathrm{Aut}(T)$. Rappelons d’autre part (VIII, § 2, no 2, remarque 4) que le groupe de Weyl $W(g_C, t_C)$ de l’algèbre réductive déployée $(g_C, t_C)$ opère dans $t_C$, et s’identifie donc canoniquement à un sous-groupe de $\mathbf{GL}(t_C)$.

#### Proposition 10 {#lie-ix-s4-prop-10 .statement tag=01C6}

*L’application* $u \mapsto L(u)_{(C)}$ *de* $\mathrm{Aut}(T)$ *dans* $\mathbf{GL}(t_C)$ *induit un isomorphisme de* $W$ *sur le groupe de Weyl de l’algèbre réductive déployée* $(g_C, t_C)$. *Pour tout* $\alpha \in \mathbf{R}$, $W_{Z_\alpha}(T)$ *est d’ordre* 2, *et l’image par l’isomorphisme précédent de l’élément non neutre de* $W_{Z_\alpha}(T)$ *est la réflexion* $s_{H_{\delta(\alpha)}}$.

L’application considérée est injective. Il s’agit de montrer que son image est égale à $W(g_C, t_C)$.

Soit $g \in N_G(T)$. Avec les notations de VIII, § 5, no 2, on a $\mathrm{Ad}\, g \in \mathrm{Aut}(g_C, t_C) \cap \mathrm{Int}(g_C)$, donc $\mathrm{Ad}\, g \in \mathrm{Aut}_0(g_C, t_C)$ (*loc. cit.*, no 5, prop. 11). D’après *loc. cit.*, no 2, prop. 4, l’automorphisme de $t_C$ induit par $\mathrm{Ad}\, g$ appartient à $W(g_C, t_C)$. L’image de $W$ dans $\mathbf{GL}(t_C)$ est donc contenue dans $W(g_C, t_C)$.

Soit $\alpha \in R(G, T)$, et soit $v : \mathrm{SU}(2, \mathbf{C}) \to G$ un morphisme de groupes de Lie ayant les propriétés du cor. au th. 1. L’image par $v$ de l’élément $\theta$ de $\mathrm{SU}(2, \mathbf{C})$ a les propriétés suivantes (§ 3, no 6, formules (17)) :

$a) \quad (\mathrm{Int}\, v(\theta))(t) = t$ si $t \in \mathrm{Ker}\, \alpha$,

$b) \quad (\mathrm{Int}\, v(\theta))(t) = t^{-1}$ si $t \in T \cap S_\alpha$.

Il s’ensuit que $\mathrm{Ad}\, v(\theta)$ induit l’identité sur $\mathrm{Ker}\, \delta(\alpha) \subset t_C$, et induit l’application $x \mapsto -x$ sur $[g^\alpha, g^{-\alpha}]$, donc coïncide avec la réflexion $s_{H_{\delta(\alpha)}}$. Ainsi l’image de $W$ contient tous les $s_{H_{\delta(\alpha)}}$, donc est égale à $W(g_C, t_C)$. En particulier $W_{Z_\alpha}(T)$ est d’ordre 2, donc formé de l’identité et de $\mathrm{Int}\, v(\theta)$. Ceci achève la démonstration de la proposition.

#### Corollaire {#lie-ix-s4-n5-cor-2 .statement tag=01JJ}

*Supposons* $G$ *semi-simple*. *Alors tout élément de* $G$ *est le commutateur de deux éléments de* $G$.

Soit $c$ une transformation de Coxeter du groupe de Weyl $W(g_C, t_C)$ (V, § 6, no 1), et soit $n$ un élément de $N_G(T)$ dont la classe dans $W$ s’identifie à $c$ par l’isomorphisme défini dans la proposition. Notons $f_c$ le morphisme $t \mapsto (n, t)$ de $T$ dans $T$; pour $x \in t_C$, on a $L(f_c)_{(C)}(x) = (\mathrm{Ad}\, n)(x) - x = c(x) - x$.

D’après le th. 1 de V, § 6, no 2, l’endomorphisme $c$ de $t_C$ n’a pas de valeur propre égale à 1. Par suite, $L(f_c)$ est surjectif, et il en est de même de $f_c$. Il en résulte que tout élément de $T$ est le commutateur de deux éléments de $G$, ce qui entraîne le corollaire compte tenu du th. 2, § 2, no 2.

### 6. Groupe fondamental

Dans la proposition qui suit, on note $f(G, T)$ l’homomorphisme de $\Gamma(T)$ dans $\pi_1(G)$ composé de l’isomorphisme canonique de $\Gamma(T)$ sur $\pi_1(T)$ (n° 2, remarque 3) et de l’homomorphisme $\pi_1(i)$, où $i$ est l’injection canonique $T \to G$.

#### Proposition 11 {#lie-ix-s4-prop-11 .statement tag=01C8}

*L’homomorphisme* $f(G, T): \Gamma(T) \to \pi_1(G)$ *est surjectif*. *Son noyau est le sous-groupe* $N(G, T)$ *de* $\Gamma(T)$ *engendré par la famille des vecteurs nodaux* $(K_\alpha)_{\alpha \in R(G, T)}$.

L’homomorphisme $f(G, T)$ est surjectif d’après la prop. 3 (§ 2, n° 4). Notons $A(G, T)$ l’assertion : « le noyau de $f(G, T)$ est engendré par les $K_\alpha$ » qu’il nous reste à démontrer, et distinguons plusieurs cas :

*a) G est simplement connexe.* Soit $\rho: g_C \to \mathrm{gl}(V)$ une représentation linéaire de $g_C$ dans un espace vectoriel complexe $V$ de dimension finie. Par restriction à $g$, on en déduit une représentation de $g$ dans l’espace vectoriel réel $V_{[\mathbf{R}]}$; puisque $G$ est simplement connexe, il existe une représentation linéaire analytique $\pi$ de $G$ dans $V_{[\mathbf{R}]}$ telle que $\rho = L(\pi)$. On déduit alors de la prop. 7 du n° 3 que l’image $\delta(X(T))$ de $X(T)$ dans $t_C^*$ contient tous les poids de $\rho$ dans $V$. Ceci étant vrai pour toute représentation $\rho$ de $g_C$, il résulte de VIII, § 7, n° 2, th. 1 que $\delta(X(T))$ contient le groupe des poids de $\delta(R)$, qui est par définition l’ensemble des $\lambda \in t_C^*$ tels que $\lambda(H_{\delta(\alpha)}) \in \mathbf{Z}$ pour tout $\alpha \in R$, c’est-à-dire $\lambda(K_\alpha) \in 2\pi i \mathbf{Z}$ pour tout $\alpha \in R$. Le groupe $X(T)$ contient donc tous les éléments $\lambda$ de $X(T) \otimes \mathbf{Q}$ tels que $\langle \lambda, K_\alpha \rangle \in \mathbf{Z}$ pour tout $\alpha \in R$, ce qui entraîne par dualité que $\Gamma(T)$ est engendré par les $K_\alpha$, d’où l’assertion $A(G, T)$.

*b) G est produit direct d’un groupe simplement connexe $G'$ par un tore S.* Alors $T$ est le produit direct d’un tore maximal $T'$ de $G'$ par $S$, $\Gamma(T)$ s’identifie à $\Gamma(T') \times \Gamma(S)$, $\pi_1(G)$ à $\pi_1(G') \times \pi_1(S)$, et $f(G, T)$ à l’homomorphisme de composantes $f(G', T')$ et $f(S, S)$. Comme $f(S, S)$ est bijectif, l’application canonique $\Gamma(T') \to \Gamma(T)$ applique bijectivement $\mathrm{Ker}\, f(G', T')$ sur $\mathrm{Ker}\, f(G, T)$. Par ailleurs, les $K_\alpha$ appartiennent à l’algèbre de Lie du groupe dérivé $G'$ de $G$, donc à l’image de $\Gamma(T')$, et il est alors immédiat que $A(G', T')$ implique $A(G, T)$, d’où l’assertion $A(G, T)$, vu *a*.

*c) Cas général.* Il existe un morphisme surjectif de noyau fini $p: G' \to G$, où $G'$ est produit direct d’un groupe simplement connexe par un tore (§ 1, n° 4, prop. 4). Si $T'$ est l’image réciproque de $T$ dans $G'$ (c’est un tore maximal de $G'$ d’après § 2, n° 3, prop. 1), et $N$ le noyau de $p$, on a des suites exactes $0 \to N \to G' \to G \to 0$ et $0 \to N \to T' \to T \to 0$, d’où un diagramme commutatif à lignes exactes (n° 2, remarque 1 et TG, XI, à paraître)

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & \Gamma(T') & \longrightarrow & \Gamma(T) & \longrightarrow & N & \longrightarrow & 0 \\
& & f(G', T') \downarrow & & f(G, T) \downarrow & & \mathrm{Id}_N \downarrow & & \\
0 & \longrightarrow & \pi_1(G') & \longrightarrow & \pi_1(G) & \longrightarrow & N & \longrightarrow & 0
\end{array}
$$

Il résulte alors aussitôt du diagramme du serpent (A, X, p. 4, prop. 2) que $A(G', T')$ entraîne $A(G, T)$, d’où la proposition, vu *b*).

#### Corollaire 1 {#lie-ix-s4-prop-11-cor-1 .statement tag=01C9}

Pour que G soit simplement connexe, il faut et il suffit que la famille $(K_\alpha)_{\alpha \in R(G, T)}$ engendre $\Gamma(T)$.

#### Corollaire 2 {#lie-ix-s4-prop-11-cor-2 .statement tag=01CA}

Soit H un sous-groupe fermé connexe de G contenant T ; on a une suite exacte

$$
0 \to N(H, T) \to N(G, T) \to \pi_1(H) \to \pi_1(G) \to 0 .
$$

Cela résulte de A, X, p. 4, prop. 2 (diagramme du serpent), appliqué au diagramme commutatif

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & N(H, T) & \longrightarrow & \Gamma(T) & \longrightarrow & \pi_1(H) & \longrightarrow & 0 \\
   &                & \downarrow      &                & \downarrow      &                & \downarrow      &                & \\
0 & \longrightarrow & N(G, T) & \longrightarrow & \Gamma(T) & \longrightarrow & \pi_1(G) & \longrightarrow & 0 .
\end{array}
$$

#### Remarque {#lie-ix-s4-n6-rem-1 .statement tag=01CB}

On peut montrer (cf. exercice 2 du § 5) que $\pi_2(G)$ est nul. On déduit alors de l’exactitude de la suite précédente un isomorphisme de $\pi_2(G/H)$ sur $N(G, T)/N(H, T)$.

#### Corollaire 3 {#lie-ix-s4-prop-11-cor-3 .statement tag=01CC}

L’homomorphisme $\pi_1(D(G)) \to \pi_1(G)$ déduit de l’inclusion de D(G) dans G induit un isomorphisme de $\pi_1(D(G))$ sur le sous-groupe de torsion de $\pi_1(G)$.

En effet, $T \cap D(G)$ est un tore maximal de D(G) ($§ 2, n^o 3,$ prop. 1, c)) ; de la suite exacte

$$
0 \to \Gamma(T \cap D(G)) \to \Gamma(T) \to \Gamma(T/(T \cap D(G))) \to 0 ,
$$

et de la proposition 11, on tire une suite exacte

$$
0 \to \pi_1(D(G)) \to \pi_1(G) \to \Gamma(T/(T \cap D(G))) \to 0 ,
$$

d’où le corollaire, puisque $\pi_1(D(G))$ est fini et $\Gamma(T/(T \cap D(G)))$ libre.

### 7. Sous-groupes de rang maximum

Rappelons (VI, § 1, n° 7) qu’une partie P de $R = R(G, T)$ est dite close si $(P + P) \cap R \subset P$, et symétrique si $P = -P$.

#### Proposition 12 {#lie-ix-s4-prop-12 .statement tag=01CD}

Soit $\mathcal{H}$ l’ensemble des sous-groupes fermés connexes de G contenant T, ordonné par inclusion. L’application $H \mapsto R(H, T)$ est une bijection croissante de $\mathcal{H}$ sur l’ensemble des parties closes et symétriques de $R(G, T)$, ordonné par inclusion.

Si $H \in \mathcal{H}$, alors $L(H)_c$ est somme directe de $t_c$ et des $g^\alpha$ pour $\alpha \in R(H, T)$; comme c’est une sous-algèbre réductive dans $g_c$, la partie $R(H, T)$ de R satisfait aux conditions énoncées (VIII, § 3, n° 1, lemme 2 et prop. 2). Inversement, si P est une partie de R satisfaisant à ces conditions, alors $t_c \oplus \sum_{\alpha \in P} g^\alpha$ est une sous-algèbre de $g_c$ (loc. cit.) qui est rationnelle sur $\mathbf{R}$ (n° 3), donc de la forme $h_{(c)}$, où $h$ est une sous-algèbre de g. Soit $H(P)$ le sous-groupe intégral de G défini par $h$; il est fermé ($§ 2, n^o 4$, remarque 1). On vérifie aussitôt que les applications $H \mapsto R(H, T)$ et $P \mapsto H(P)$ sont croissantes et réciproques l'une de l'autre.

#### Corollaire 1 {#lie-ix-s4-prop-12-cor-1 .statement tag=01CE}

Les sous-groupes fermés de $G$ contenant $T$ sont en nombre fini.
Soit $H$ un tel sous-groupe ; on a $H_0 \in \mathcal{H}$, et $\mathcal{H}$ est fini. Par ailleurs, $H$ est un sous-groupe de $N_G(H_0)$ contenant $H_0$, et $N_G(H_0)/H_0$ est fini (§ 2, no 4, prop. 4 et remarque 2).

#### Corollaire 2 {#lie-ix-s4-prop-12-cor-2 .statement tag=01CF}

Soit $H$ un sous-groupe fermé connexe de $G$ contenant $T$, et soit $W_G^H(T)$ le stabilisateur dans $W_G(T)$ de la partie $R(H, T)$ de $R$. Le groupe $N_G(H)/H$ est isomorphe au groupe quotient $W_G^H(T)/W_H(T)$.
Il résulte en effet de la prop. 7 du § 2, no 5, appliquée à $N_G(H)$, que $N_G(H)/H$ est isomorphe à $W_{N(H)}(T)/W_H(T)$, où $W_{N(H)}(T)$ est l'ensemble des éléments de $W_G(T)$ dont les représentants dans $N_G(T)$ normalisent $H$. Soit $n \in N_G(T)$, et soit $w$ sa classe dans $W_G(T)$. D'après III, § 9, no 4, prop. 11, $n$ normalise $H$ si et seulement si on a $(\mathrm{Ad}\ n)\ (L(H)) = L(H)$; compte tenu de la prop. 5 du no 3, cela signifie aussi que la partie $R(H, T)$ de $R$ est stable par $w$, d'où le corollaire.

#### Remarque 1 {#lie-ix-s4-n7-rem-1 .statement tag=01CG}

Le groupe $W_G^H(T)$ est aussi le stabilisateur dans $W_G(T)$ du sous-groupe $C(H)$ de $T$ : cela résulte de la prop. 8 du no 4.

#### Proposition 13 {#lie-ix-s4-prop-13 .statement tag=01CH}

Soient $H$ un sous-groupe fermé connexe de $G$ de rang maximum, $C$ son centre. Alors $C$ contient le centre de $G$, et $H$ est la composante neutre du centralisateur de $C$.
Soit $S$ un tore maximal de $H$. Puisque le centre de $G$ est contenu dans $S$, il est contenu dans $C$. Posons $L = Z(C)_0$ ; c'est un sous-groupe fermé connexe de $G$ contenant $H$, donc de rang maximum, et son centre est égal à $C$. Notons $R_H$ et $R_L$ les systèmes de racines de $H$ et $L$ respectivement, relativement à $S$ ; on a $R_H \subset R_L \subset R(G, S)$. Puisque $C(H) = C(L)$, la prop. 8 (no 4) entraîne l'égalité $Q(R_H) = Q(R_L)$ ; mais on a $Q(R_H) \cap R_L = R_H$ (VI, § 1, no 7, prop. 23), d'où $R_H = R_L$ et $H = L$ (prop. 12).

#### Remarque 2 {#lie-ix-s4-n7-rem-2 .statement tag=01CI}

Disons qu'un sous-groupe $C$ de $G$ est radiciel s'il existe un tore maximal $S$ de $G$ et une partie $P$ de $R(G, S)$ tels que $C = \bigcap_{\alpha \in P} \mathrm{Ker}\ \alpha$. Il résulte de la prop. 13 et du lemme 2 du no 5 que l'application $H \mapsto C(H)$ induit une bijection de l'ensemble des sous-groupes fermés connexes de rang maximum sur l'ensemble des sous-groupes radiciels de $G$. La bijection réciproque est l'application $C \mapsto Z(C)_0$.

#### Corollaire {#lie-ix-s4-n7-cor-1 .statement tag=01CJ}

L'ensemble des $g \in G$ tels que $T \cap gTg^{-1} \neq C(G)$ est une réunion finie de sous-variétés analytiques fermées de $G$ distinctes de $G$.
En effet, posons $A_g = T \cap gTg^{-1}$ ; on a $T \subset Z(A_g)$ et $gTg^{-1} \subset Z(A_g)$. Il existe donc $x \in Z(A_g)$ tel que $xTx^{-1} = gTg^{-1}$ (§ 2, no 2, th. 2), ce qui implique $g \in Z(A_g).N_G(T)$. Notons $\mathcal{A}$ l'ensemble fini (cor. 1) des sous-groupes fermés de $G$ contenant $T$ et distincts de $G$, et posons $X = \bigcup_{H \in \mathcal{A}} H.N_G(T)$ ; c'est une réunion finie de sous-variétés fermées de G, distinctes de G. Si $A_g \neq C(G)$, on a $Z(A_g) \in \mathcal{A}$, et $g$ appartient à X. Inversement si $g \in H.N_G(T)$, avec $H \in \mathcal{A}$, alors $A_g$ contient $C(H)$, donc $A_g \neq C(G)$ (prop. 13).

#### Proposition 14 {#lie-ix-s4-prop-14 .statement tag=01CK}

*Soit X une partie de T, et soit $R_X$ l’ensemble des racines $\alpha \in R(G, T)$ telles que $\alpha(X) = \{1\}$. Le groupe $Z_G(X)/Z_G(X)_0$ est isomorphe au quotient du fixateur de X dans $W_G(T)$ par le sous-groupe engendré par les réflexions $s_\alpha$ pour $\alpha \in R_X$.

Posons $H = Z_G(X)$; puisque $L(H)_{(c)}$ est l’ensemble des points de $g_c$ fixes par $\mathrm{Ad}(X)$, c’est la somme de $t_c$ et des $g^\alpha$ pour $\alpha(X) = \{1\}$. On a par conséquent $R(H_0, T) = R_X$, de sorte que $W_{H_0}(T)$ est engendré par les réflexions $s_\alpha$ pour $\alpha \in R_X$. Il suffit alors d’appliquer la prop. 7 du § 2, n° 5.

On verra ci-dessous (§ 5, n° 3, th. 1) que si G est simplement connexe et X réduit à un point, le centralisateur $Z(X)$ est connexe.

### 8. Diagrammes radiciels

#### Définition 2 {#lie-ix-s4-def-2 .statement tag=01CL}

*On appelle diagramme radiciel (ou simplement diagramme si aucune confusion n’en peut résulter) un triplet $D = (M, M_0, R)$ où :

(DR₀) $M$ est un $\mathbf{Z}$-module libre de type fini et $M_0$ un sous-module facteur direct de $M$;
(DR₁) $R$ est une partie finie de $M$; $R \cup M_0$ engendre le $\mathbf{Q}$-espace vectoriel $\mathbf{Q} \otimes M$;
(DR₂) pour tout $\alpha \in R$, il existe un élément $\alpha^\vee$ de $M^* = \mathrm{Hom}_\mathbf{Z}(M, \mathbf{Z})$ tel que $\alpha^\vee(M_0) = 0$, $\alpha^\vee(\alpha) = 2$ et que l’endomorphisme $x \mapsto x - \alpha^\vee(x)\alpha$ de $M$ laisse stable $R$.

D’après VI, § 1, n° 1, pour tout $\alpha \in R$, l’élément $\alpha^\vee$ de $M^*$ est uniquement déterminé par $\alpha$; on note $s_\alpha$ l’endomorphisme $x \mapsto x - \alpha^\vee(x)\alpha$ de $M$. De plus (*loc. cit.*), le $\mathbf{Q}$-espace vectoriel $\mathbf{Q} \otimes M$ est somme directe de $\mathbf{Q} \otimes M_0$ et du sous-espace vectoriel $V(R)$ engendré par $R$, et $R$ est un système de racines dans $V(R)$ (*loc. cit.*, déf. 1).

Les éléments de $R$ s’appellent les *racines* du diagramme radiciel $D$, et les éléments $\alpha^\vee$ de $M^*$ les *racines inverses*. Le groupe engendré par les automorphismes $s_\alpha$ de $M$ s’appelle le *groupe de Weyl* de $D$ et se note $W(D)$; les éléments de $W(D)$ induisent l’identité sur $M_0$, et induisent sur $V(R)$ les transformations du groupe de Weyl du système de racines $R$.

#### Exemple 1 {#lie-ix-s4-n8-exa-1 .statement tag=01CM}

Pour tout $\mathbf{Z}$-module libre de type fini $M$, le triplet $(M, M, \varnothing)$ est un diagramme radiciel.

#### Exemple 2 {#lie-ix-s4-n8-exa-2 .statement tag=01CN}

Si $D = (M, M_0, R)$ est un diagramme radiciel, soit $M_0^*$ l’orthogonal de $V(R)$ dans $M^*$, et soit $R^\vee$ l’ensemble des racines inverses de $D$. Alors $D^\vee = (M^*, M_0^*, R^\vee)$ est un diagramme radiciel, dit *inverse* de $D$. Pour tout $\alpha \in R$, la symétrie $s_{\alpha^\vee}$ de $M^*$ est l’automorphisme contragrédient de la symétrie $s_\alpha$ de $M$; l’application $w \mapsto {}^t_w^{-1}$ est un isomorphisme de $W(D)$ sur $W(D^\vee)$. De plus, $V(R^\vee)$ s’identifie naturellement au dual du Q-espace vectoriel V(R), $R^\vee$ s’identifiant alors au système de racines inverse de R.

Si l’on identifie le dual de $M^*$ à M, le diagramme inverse de $D^\vee$ s’identifie à D.

#### Exemple 3 {#lie-ix-s4-n8-exa-3 .statement tag=01CO}

Soient $(g, h)$ une Q-algèbre de Lie réductive déployée, et $M \subset h$ un réseau permis (VIII, § 12, n° 6, déf. 1). Soient $M_0$ le sous-groupe de M orthogonal aux racines de $(g, h)$ et $R^\vee$ l’ensemble des $H_\alpha$, $\alpha \in R(g, h)$. Alors $(M, M_0, R^\vee)$ est un diagramme radiciel, et $(M^*, M_0^*, R(g, h))$ en est le diagramme inverse.

#### Exemple 4 {#lie-ix-s4-n8-exa-4 .statement tag=01CP}

Soient V un espace vectoriel sur Q et R un système de racines dans V ; notons P(R) le groupe des poids de R et Q(R) le groupe des poids radiciels de R (VI, § 1, n° 9). Alors $(Q(R), 0, R)$ et $(P(R), 0, R)$ sont des diagrammes radiciels. Pour qu’un diagramme $(M, M_0, S)$ soit isomorphe à un diagramme de la forme $(Q(R), 0, R)$ (resp. $(P(R), 0, R)$)), il faut et il suffit que M soit engendré par S (resp. que $M^*$ soit engendré par $S^\vee$).

Pour tout sous-groupe X de P(R) contenant Q(R), $(X, 0, R)$ est un diagramme radiciel, et on obtient ainsi, à isomorphisme près, tous les diagrammes $(M, M_0, S)$ tels que $M_0 = 0$, c’est-à-dire tels que S engendre un sous-groupe d’indice fini de M.

On dit que le diagramme radiciel $(M, M_0, R)$ est réduit si le système de racines R l’est (c’est-à-dire (VI, § 1, n° 4) si les relations $\alpha, \beta \in R, \lambda \in \mathbf{Z}, \beta = \lambda \alpha$ impliquent $\lambda = 1$ ou $\lambda = -1$). Les diagrammes des exemples 1) et 3) sont réduits.

### 9. Groupes de Lie compacts et diagrammes radiciels

Avec la terminologie introduite au numéro précédent, on peut résumer une partie importante des résultats des numéros 4 et 5 dans le théorème suivant :

#### Théorème 2 {#lie-ix-s4-thm-2 .statement tag=01CQ}

a) $(X(T), X(T/(T \cap D(G))), R(G, T))$ est un diagramme radiciel réduit ; son groupe de Weyl est formé des $X(w)$, pour $w \in W$ ; le groupe $X(C(G))$ est isomorphe au quotient de $X(T)$ par le sous-groupe engendré par $R(G, T)$.

b) $(\Gamma(T), \Gamma(C(G)_0), R^\vee(G, T))$ est un diagramme radiciel réduit ; son groupe de Weyl est formé des $\Gamma(w)$, pour $w \in W$ ; le groupe $\pi_1(G)$ est isomorphe au quotient de $\Gamma(T)$ par le sous-groupe engendré par $R^\vee(G, T)$.

c) Si l’on identifie chacun des $\mathbf{Z}$-modules $X(T)$ et $\Gamma(T)$ au dual de l’autre (n° 2, prop. 3), chacun des diagrammes radiciels précédents s’identifie au diagramme inverse de l’autre.

On note $D^*(G, T)$ le diagramme $(X(T), X(T/(T \cap D(G))), R(G, T))$ et $D_*(G, T)$ le diagramme $(\Gamma(T), \Gamma(C(G)_0), R^\vee(G, T))$ ; on dit que ce sont respectivement le diagramme contravariant et le diagramme covariant de G (relativement à T).

#### Exemple 1 {#lie-ix-s4-n9-exa-1 .statement tag=01CR}

Si G est semi-simple de rang 1, alors $D^*(G, T)$ et $D_*(G, T)$ sont nécessairement isomorphes à l’un des deux diagrammes $\Delta_2 = (\mathbf{Z}, 0, \{2, -2\})$, $\Delta_1 = (\mathbf{Z}, 0, \{1, -1\})$. Si G est isomorphe à SU(2, C), $D_*(G, T)$ est isomorphe à $\Delta_1$ (puisque G est simplement connexe), donc $D^*(G, T)$ isomorphe à $\Delta_2$. Si G est isomorphe à $SO(3, \mathbf{R})$, $D^*(G, T)$ est isomorphe à $\Delta_1$ (puisque $C(G) = \{1\}$), donc $D_*(G, T)$ est isomorphe à $\Delta_2$.

#### Exemple 2 {#lie-ix-s4-n9-exa-2 .statement tag=01CS}

Si $G$ et $G'$ sont deux groupes de Lie compacts connexes, de tores maximaux respectifs $T$ et $T'$, et si $D^*(G, T) = (M, M_0, R)$ et $D^*(G', T') = (M', M'_0, R')$, alors $D^*(G \times G', T \times T')$ s’identifie à $(M \oplus M', M_0 \oplus M'_0, R \cup R')$. De même pour les diagrammes covariants.

#### Exemple 3 {#lie-ix-s4-n9-exa-3 .statement tag=01CT}

Soit $N$ un sous-groupe fermé de $T$, central dans $G$, et soit $(M, M_0, R)$ le diagramme contravariant de $G$ relativement à $T$. Alors le diagramme contravariant de $G/N$ relativement à $T/N$ s’identifie à $(M', M'_0, R)$, où $M'$ est le sous-groupe de $M$ formé des $\lambda$ tels que $\lambda(N) = \{1\}$ et $M'_0 = M' \cap M_0$.

#### Exemple 4 {#lie-ix-s4-n9-exa-4 .statement tag=01CU}

De même, soit $N$ un groupe commutatif fini, et $\varphi : \pi_1(G) \to N$ un homomorphisme surjectif. Soit $G'$ le revêtement de $G$ associé à cet homomorphisme ; c’est un groupe de Lie compact connexe, dont $N$ est un sous-groupe central (TG, XI, à paraître), et $G$ s’identifie naturellement à $G'/N$. Soit $T'$ le tore maximal de $G'$ image réciproque de $T$. Si $(P, P_0, S)$ est le diagramme covariant de $G$ relativement à $T$, le diagramme covariant de $G'$ relativement à $T'$ s’identifie à $(P', P'_0, S)$, où $P'$ est le noyau de l’homomorphisme composé $\varphi \circ f(G, T) : P \to N$ (\emph{cf.} n° 6, prop. 11), et $P'_0 = P_0 \cap P'$.

#### Remarque 1 {#lie-ix-s4-n9-rem-1 .statement tag=01CV}

Soit $c$ le centre de $g_C$; on a donc $c = L(C(G))_{(C)}$. On a les relations suivantes entre les diagrammes de $G$ relativement à $T$ et les systèmes de racines direct et inverse de l’algèbre réductive déployée $(g_C, t_C)$ :

a) L’isomorphisme canonique de $C \otimes \Gamma(T)$ sur $t_C$ induit une bijection de $C \otimes \Gamma(C(G)_0)$ sur $c$ et une bijection de $1 \otimes R^\vee(G, T)$ sur $2\pi i . R^\vee(g_C, t_C)$.

b) L’isomorphisme canonique de $C \otimes X(T)$ sur le dual $t_C^*$ de $t_C$ induit une bijection de $C \otimes X(T/(T \cap D(G)))$ sur l’orthogonal de $t_C \cap \mathcal{D}(g)_C$, et une bijection de $1 \otimes R(G, T)$ sur $R(g_C, t_C)$.

#### Remarque 2 {#lie-ix-s4-n9-rem-2 .statement tag=01CW}

Supposons le groupe $G$ semi-simple ; notons $R$ (resp. $R^\vee$) le système de racines $R(G, T)$ (resp. $R^\vee(G, T)$), de sorte qu’on a les inclusions

$$
Q(R) \subset X(T) \subset P(R) \quad Q(R^\vee) \subset \Gamma(T) \subset P(R^\vee).
$$

Les groupes commutatifs finis $P(R)/Q(R)$ et $P(R^\vee)/Q(R^\vee)$ sont en dualité (VI, § 1, n° 9); si on désigne par $M^\wedge$ le groupe dual d’un groupe commutatif fini $M$, on déduit de ce qui précède des *isomorphismes canoniques*

$$
\begin{align*}
\Gamma(T)/Q(R^\vee) &\to \pi_1(G) & P(R^\vee)/\Gamma(T) &\to C(G) \\
P(R)/X(T) &\to (\pi_1(G))^\wedge & X(T)/Q(R) &\to (C(G))^\wedge .
\end{align*}
$$

En particulier, le *produit des ordres de $\pi_1(G)$ et de $C(G)$* est égal à *l’indice de connexion* $f$ de $R(G, T)$ (*loc. cit.*).

Soient maintenant $G'$ un autre groupe de Lie compact connexe, $T'$ un tore maximal de $G'$. Soit $f : G \to G'$ un isomorphisme de groupes de Lie tel que $f(T) = T'$; notons $f_T$ l’isomorphisme de $T$ sur $T'$ qu’il définit. Alors $X(f_T)$ est un isomorphisme de $D^*(G', T')$ sur $D^*(G, T)$, noté $D^*(f)$, et $\Gamma(f_T)$ est un isomorphisme de $D_*(G, T)$ sur $D_*(G', T')$, noté $D_*(f)$. Si $t \in T$, et si on pose $g = f \circ \mathrm{Int}\ t = (\mathrm{Int}\ f(t)) \circ f$, alors $D^*(g) = D^*(f)$, $D_*(g) = D_*(f)$.

#### Proposition 15 {#lie-ix-s4-prop-15 .statement tag=01CX}

*Soit $\varphi$ un isomorphisme de $D^*(G', T')$ sur $D^*(G, T)$ (resp. de $D_*(G, T)$ sur $D_*(G', T')$). Il existe un isomorphisme $f : G \to G'$ tel que $f(T) = T'$ et que $\varphi = D^*(f)$ (resp. et que $\varphi = D_*(f)$) ; si $f_1$ et $f_2$ sont deux tels isomorphismes, il existe un élément $t$ de $T$ tel que $f_2 = f_1 \circ \mathrm{Int}\ t$.

La seconde assertion résulte aussitôt de la prop. 9 (n° 4) ; démontrons la première, par exemple pour les diagrammes covariants. Notons $g'$ (resp. $t'$) l’algèbre de Lie de $G'$ (resp. $T'$), et $g'_c$ (resp. $t'_c$) son algèbre de Lie complexifiée. D’après VIII, § 4, n° 4, th. 2, (i), il existe un isomorphisme $\psi : g_c \to g'_c$ qui applique $t_c$ dans $t'_c$ et induit sur $\Gamma(T) \subset t_c$ l’isomorphisme $\varphi : \Gamma(T) \to \Gamma(T')$ donné. Alors $g$ et $\psi^{-1}(g')$ sont deux formes compactes de $g_c$ qui ont même intersection $t$ avec $t_c$ ; d’après le § 3, n° 2, prop. 3, il existe un automorphisme intérieur $\theta$ de $g_c$ induisant l’identité sur $t_c$ et tel que $\theta(g) = \psi^{-1}(g')$. Remplaçant $\psi$ par $\psi \circ \theta$, on peut donc supposer que $\psi$ applique $g$ dans $g'$. Par ailleurs, d’après la prop. 4 du n° 2, il existe un unique morphisme $f_T : T \to T'$ tel que $\Gamma(f_T) = \varphi$. Alors la restriction de $\psi$ à $t$ est $L(f_T)$, et d’après le § 2, n° 6, prop. 8, il existe un unique morphisme $f : G \to G'$ qui induise $f_T$ sur $T$ et $\psi$ sur $g_c$. Appliquant ce qui précède à $\varphi^{-1}$ et $\psi^{-1}$, on construit un morphisme réciproque de $f$, qui est donc un isomorphisme. On a $D_*(f) = \Gamma(f_T) = \varphi$, d’où la proposition.

Notons que, si $T$ et $T'$ sont deux tores maximaux de $G$, les diagrammes $D^*(G, T)$ et $D^*(G, T')$ sont isomorphes (si $g \in G$ est tel que $gTg^{-1} = T'$, alors $\mathrm{Int}\ g$ est un isomorphisme de $G$ sur $G$ qui applique $T$ sur $T'$). On note $D^*(G)$ la classe d’isomorphisme de $D^*(G, T)$ (*cf.* E, II, p. 47) ; c’est un diagramme radiciel qui ne dépend que de $G$ et qu’on appelle le diagramme contravariant de $G$. On définit de même le diagramme covariant $D_*(G)$ de $G$, et on obtient :

#### Corollaire {#lie-ix-s4-n9-cor-1 .statement tag=01CY}

*Pour que les groupes de Lie compacts connexes $G$ et $G'$ soient isomorphes, il faut et il suffit que les diagrammes $D^*(G)$ et $D^*(G')$ (resp. $D_*(G)$ et $D_*(G')$) soient égaux.*

#### Proposition 16 {#lie-ix-s4-prop-16 .statement tag=01CZ}

*Pour tout diagramme radiciel réduit $D$, il existe un groupe de Lie compact connexe $G$ tel que $D^*(G)$ (resp. $D_*(G)$) soit isomorphe à $D$.

a) Remplaçant éventuellement $D$ par son diagramme inverse, on se ramène à construire $G$ tel que $D^*(G)$ soit isomorphe à $D$. Posons $D = (M, M_0, R)$ ; alors $Q \otimes M$ est somme directe de $Q \otimes M_0$ et du sous-espace vectoriel $V(R)$ engendré par $R$. De plus, puisque les racines inverses prennent des valeurs entières sur $M$, la projection de $M$ dans $V(R)$ parallèlement à $Q \otimes M_0$ est contenue dans le groupe des poids $P(R)$ de $R$, de sorte que $M$ est un sous-groupe d’indice fini de $M_0 \oplus P(R)$. Notons $D'$ le diagramme $(M_0 \oplus P(R), M_0, R)$.

b) Soit $\alpha$ une algèbre de Lie semi-simple complexe dont le système de racines canonique soit isomorphe à $R \subset C \otimes V(R)$ (VIII, § 4, n° 3), et soit $g_1$ une forme réelle compacte de $\alpha$ ($§ 3$, no 2, th. 1). Soit $G_1$ un groupe de Lie réel simplement connexe d’algèbre de Lie isomorphe à $g_1$; alors $G_1$ est compact ($§ 1$, no 4, th. 1). Soit $T_1$ un tore maximal de $G_1$. D’après le th. 1, le diagramme $D^*(G_1, T_1)$ est isomorphe à $(P(\mathbf{R}), 0, \mathbf{R})$.

c) Soit $T_0$ un tore de dimension égale au rang de $M_0$; alors $D^*(T_0, T_0)$ est isomorphe à $(M_0, M_0, \varnothing)$, donc $D^*(G_1 \times T_0, T_1 \times T_0)$ isomorphe à $D'$ (exemple 2).

d) Enfin, soit $N$ le sous-groupe fini de $T_1 \times T_0$ orthogonal à $M$. Posons $G = (G_1 \times T_0)/N, T = (T_1 \times T_0)/N$. Alors $G$ est un groupe de Lie compact connexe, $T$ un tore maximal de $G$, et $D(G, T)$ est isomorphe à $D$ (exemple 3).

#### Scholie {#lie-ix-s4-n9-sch-1 .statement tag=01D0}

*La classification des groupes de Lie compacts connexes à isomorphisme près est ainsi ramenée à celle des diagrammes radiciels réduits. Les groupes de Lie compacts connexes semi-simples correspondent aux diagrammes radiciels réduits* $(M, M_0, R)$ *tels que* $M_0 = 0$; *la donnée d’un tel diagramme est équivalente à celle d’un système de racines réduit* $R$ *dans un espace vectoriel* $V$ *sur* $\mathbf{Q}$ *et d’un sous-groupe* $M$ *de* $V$ *tel que* $\mathbf{Q}(R) \subset M \subset P(\mathbf{R})$.

#### Remarque 3 {#lie-ix-s4-n9-rem-3 .statement tag=01D1}

Soient $T'$ un autre tore maximal de $G$, $B$ (resp. $B'$) une base du système de racines $R(G, T)$ (resp. $R(G', T')$) (VI, $§ 1$, no 5, déf. 2). Il existe des éléments $g \in G$ tels que $\operatorname{Int} g$ applique $T$ sur $T'$ et $B$ sur $B'$, et ces éléments forment une unique classe modulo $\operatorname{Int}(T)$ (comme $T$ et $T'$ sont conjugués, on peut supposer $T = T'$, et il suffit d’appliquer VI, $§ 1$, no 5, remarque 4 et la prop. 9 du no 4). Il en résulte que l’isomorphisme de $T$ sur $T'$ déduit de $\operatorname{Int} g$ est indépendant du choix de $g$; il en est par conséquent de même pour $D_*(\operatorname{Int} g)$ et $D^*(\operatorname{Int} g)$. Paraphrasant alors VIII, $§ 5$, no 3, remarque 2, *mutatis mutandis*, on définit le tore maximal canonique de $G$, les diagrammes radiciels covariant et contravariant canoniques de $G$, ...

### 10. Automorphismes d’un groupe de Lie compact connexe

On note $\operatorname{Aut}(G)$ le groupe de Lie des automorphismes de $G$ (III, $§ 10$, no 2), et $\operatorname{Aut}(G, T)$ le sous-groupe fermé de $\operatorname{Aut}(G)$ formé des éléments $u$ tels que $u(T) = T$. On a vu ($§ 1$, no 4, cor. 5 à la prop. 4) que la composante neutre de $\operatorname{Aut}(G)$ est le sous-groupe $\operatorname{Int}(G)$ des automorphismes intérieurs; on note $\operatorname{Int}_G(H)$ l’image dans $\operatorname{Int}(G)$ d’un sous-groupe $H$ de $G$.

Soit $D$ le diagramme covariant de $G$ relativement à $T$; notons $\operatorname{Aut}(D)$ le groupe de ses automorphismes, et $W(D)$ son groupe de Weyl. L’application $u \mapsto D_*(u)$ est un homomorphisme de $\operatorname{Aut}(G, T)$ dans $\operatorname{Aut}(D)$. La prop. 15 du no 9 donne aussitôt :

#### Proposition 17 {#lie-ix-s4-prop-17 .statement tag=01D2}

*L’homomorphisme* $\operatorname{Aut}(G, T) \to \operatorname{Aut}(D)$ *est surjectif, de noyau* $\operatorname{Int}_G(T)$.

Notons que $\operatorname{Aut}(G, T) \cap \operatorname{Int}(G) = \operatorname{Int}_G(N_G(T))$ et que l’image de $\operatorname{Int}_G(N_G(T))$ dans $\operatorname{Aut}(D)$ est $W(D)$ (no 5, prop. 10). On déduit donc de la prop. 17 un isomorphisme :
$$
\operatorname{Aut}(G, T)/(\operatorname{Aut}(G, T) \cap \operatorname{Int}(G)) \to \operatorname{Aut}(D)/W(D) .
$$

Par ailleurs, on a $\mathrm{Aut}(G) = \mathrm{Int}(G). \mathrm{Aut}(G, T)$. En effet, si $u$ appartient à $\mathrm{Aut}(G)$, $u(T)$ est un tore maximal de $T$, donc est conjugué à $T$, et il existe un automorphisme intérieur $v$ de $G$ tel que $u(T) = v(T)$, c'est-à-dire $v^{-1}u \in \mathrm{Aut}(G, T)$. Il en résulte que $\mathrm{Aut}(G)/\mathrm{Int}(G)$ s'identifie à $\mathrm{Aut}(G, T)/(\mathrm{Aut}(G, T) \cap \mathrm{Int}(G))$, d'où en vertu de ce qui précède une suite exacte

(16) $$
1 \to \mathrm{Int}(G) \to \mathrm{Aut}(G) \to \mathrm{Aut}(D)/W(D) \to 1 .
$$

Par conséquent :

#### Proposition 18 {#lie-ix-s4-prop-18 .statement tag=01K9}

*Le groupe* $\mathrm{Aut}(G)/\mathrm{Int}(G)$ *est isomorphe à* $\mathrm{Aut}(D)/W(D)$.

Supposons en particulier $G$ semi-simple ; le groupe $\mathrm{Aut}(D)$ s'identifie alors au sous-groupe de $A(R(G, T))$ (VI, § 1, no 1) formé des éléments $u$ tels que $u(X(T)) \subset X(T)$, et le sous-groupe $W(D)$ s'identifie à $W(R(G, T))$.

#### Corollaire {#lie-ix-s4-n10-cor-1 .statement tag=01D3}

*Si* $G$ *est simplement connexe, ou si* $C(G)$ *est réduit à l’élément neutre,* le groupe $\mathrm{Aut}(G)/\mathrm{Int}(G)$ *est isomorphe au groupe des automorphismes du graphe de Dynkin de* $R(G, T)$.

Cela résulte de ce qui précède et de VI, § 4, no 2, cor. à la prop. 1.

Nous nous proposons maintenant de montrer que l’extension (16) admet des sections.

Pour tout $\alpha \in R(G, T)$, notons $V(\alpha)$ le sous-espace vectoriel de dimension 2 de $g$ tel que $V(\alpha)_c = g^\alpha + g^{-\alpha}$; notons $K$ la forme quadratique associée à la forme de Killing de $g$.

#### Définition 3 {#lie-ix-s4-def-3 .statement tag=01D4}

*On appelle épinglage de* $(G, T)$ *un couple* $(B, (U_\alpha)_{\alpha \in B})$, *où* $B$ *est une base de* $R(G, T)$ *(VI, § 1, no 5, déf. 2)* *et où, pour tout* $\alpha \in B$, $U_\alpha$ *est un élément de* $V(\alpha)$ *tel que* $K(U_\alpha) = -1$.

On appelle épinglage de $G$ la donnée d’un tore maximal $T$ de $G$ et d’un épinglage de $(G, T)$.

#### Lemme 3 {#lie-ix-s4-lem-3 .statement tag=01D5}

*Soit* $B_0$ *une base de* $R(G, T)$. *Le groupe* $\mathrm{Int}_G(T)$ *opère de façon simplement transitively dans l’ensemble des épinglages de* $(G, T)$ *de la forme* $(B_0, (U_\alpha)_{\alpha \in B_0})$.

Pour tout $\alpha \in B_0$, notons $K(\alpha)$ la restriction à $V(\alpha)$ de la forme quadratique $K$; l’action de $T$ sur $V(\alpha)$ définit un morphisme $\iota_\alpha : T \to SO(K(\alpha))$. On a vu au no 4 que $SO(K(\alpha))$ s’identifie à $U$ de façon que $\iota_\alpha$ s’identifie à la racine $\alpha$. Comme $B_0$ est une base de $R$, c’est une base du $\mathbf{Z}$-module $Q(R)$ engendré par les racines, donc une base du sous-module $X(T/C(G))$ de $X(T)$. Il en résulte que le morphisme produit des $\iota_\alpha$ induit un isomorphisme de $T/C(G)$ sur le groupe produit des $SO(K(\alpha))$. Or ce dernier opère de façon simplement transitive sur l’ensemble des épinglages de $(G, T)$ dont la première composante est $B_0$.

#### Proposition 19 {#lie-ix-s4-prop-19 .statement tag=01D6}

*Le groupe* $\mathrm{Int}(G)$ *opère de façon simplement transitive dans l’ensemble des épinglages de* $G$.

Soient $e = (T, B, (U_\alpha))$ et $e' = (T', B', (U'_\alpha))$ deux épinglages de $G$. Il existe des éléments $g$ dans $G$ tels que $(\mathrm{Int}\,g)(T) = T'$, et ces éléments forment une classe modulo $N_G(T)$. On peut donc supposer $T = T'$, et il faut prouver qu’il existe un unique élément de $\mathrm{Int}_G(N_G(T))$ qui transforme $e$ en $e'$. D’après VI, § 1, n° 5, remarque 4, il existe un unique élément $w$ de $W(R)$ tel que $w(B) = B'$. Comme $W(R)$ s’identifie à $N_G(T)/T$, il existe $n \in N_G(T)$ tel que $w = \mathrm{Int}\,n$, et $n$ est bien déterminé modulo $T$. On peut donc supposer $B = B'$, et il faut prouver qu’il existe un unique élément de $\mathrm{Int}_G(T)$ qui transforme $e$ en $e'$, ce qui n’est autre que le lemme 3.

#### Corollaire {#lie-ix-s4-n10-cor-2 .statement tag=01D7}

Soit $e$ un épinglage de $(G, T)$ et soit $E$ le groupe des automorphismes de $G$ qui laissent $e$ stable. Alors $\mathrm{Aut}(G)$ est produit semi-direct de $E$ par $\mathrm{Int}(G)$, et $\mathrm{Aut}(G, T)$ est produit semi-direct de $E$ par $\mathrm{Int}(G) \cap \mathrm{Aut}(G, T) = \mathrm{Int}_G(N_G(T))$.

En effet, tout élément de $\mathrm{Aut}(G)$ transforme $e$ en un épinglage de $G$. D’après la prop. 19, toute classe de $\mathrm{Aut}(G)$ suivant $\mathrm{Int}(G)$ rencontre $E$ en un point et un seul, d’où la première assertion. La seconde se démontre de la même manière.

#### Remarque {#lie-ix-s4-n10-rem-1 .statement tag=01D8}

Soient $G$ et $G'$ deux groupes de Lie compacts connexes, et soient $e = (T, B, (U_\alpha))$ et $e' = (T', B', (U'_\alpha))$ des épinglages de $G$ et $G'$ respectivement. Soit $X$ l’ensemble des isomorphismes de $G$ sur $G'$ qui appliquent $e$ sur $e'$. L’application $f \mapsto D^*(f)$ (resp. $D_*(f)$) est une bijection de $X$ sur l’ensemble des isomorphismes de $D^*(G', T')$ sur $D^*(G, T)$ (resp. $D_*(G, T)$ sur $D_*(G', T')$) qui appliquent $B'$ sur $B$ (resp. $B$ sur $B'$). Cela résulte en effet aussitôt de la prop. 15 et du lemme 3.

## EXERCICES {#lie-ix-s4-exercises}

See the [exercises for § 4](exercises/s4/).
