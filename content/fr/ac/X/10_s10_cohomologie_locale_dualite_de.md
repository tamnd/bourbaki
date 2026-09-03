---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 10
section_title: Cohomologie locale, dualité de Grothendieck
lang: fr
source: ac-x-fr
pdf_pages: 0141-0150, 0178-0180
extraction: ocr
subsections:
    - "no": 1
      title: Cohomologie locale
      page: 0
      pdf_page: 141
    - "no": 2
      title: Cohomologie locale sur un anneau de Macaulay
      page: 145
      pdf_page: 144
    - "no": 3
      title: Dualité de Grothendieck sur un anneau de Macaulay
      page: 147
      pdf_page: 146
statements: 20
exercises: 11
content_sha256: 98a442199970317d391ce1fd8ffe328343aca79a293a45ca21eccd3c51bccdac
---

## § 10. COHOMOLOGIE LOCALE, DUALITÉ DE GROTHENDIECK

### 1. Cohomologie locale

Dans ce numéro, on considère un anneau $A$ local noethérien. Rappelons (VIII, § 3, n° 3, lemme 2) que les idéaux de définition de $A$ sont les idéaux de $A$ distincts de $A$ contenant une puissance de $m_A$, ou encore les idéaux $a \subset m_A$ tels que $A/a$ soit de longueur finie. On notera $\mathscr{D}$ l’ensemble des idéaux de définition de $A$, muni de la relation d’ordre opposée à l’inclusion ; il est filtrant à droite.

Soit $M$ un $A$-module. Associons à tout idéal de définition $a$ de $A$ le $A$-module gradué $\mathrm{Ext}_A(A/a, M)$ ; si $a$ et $b$ sont des idéaux de définition avec $a \subset b$, notons $p_{ab} : A/a \to A/b$ l’application canonique et considérons l’application $A$-linéaire $\mathrm{Ext}(p_{ab}, 1_M) : \mathrm{Ext}_A(A/b, M) \longrightarrow \mathrm{Ext}_A(A/a, M)$. On obtient ainsi un système inductif de $A$-modules gradués et d’applications $A$-linéaires graduées de degré 0 relatif à l’ensemble ordonné $\mathscr{D}$. On appelle *module de cohomologie locale* de $M$, et on note $H_A(M)$, le $A$-module gradué $\varprojlim_{a \in \mathscr{D}} \mathrm{Ext}_A(A/a, M)$.

Les idéaux $m_A^n$ pour $n \geq 1$ forment une partie cofinale de $\mathscr{D}$ ; on a donc un isomorphisme canonique de modules gradués $\varprojlim_n \mathrm{Ext}_A(A/m_A^n, M) \longrightarrow H_A(M)$. Par suite tout élément de $H_A(M)$ est annulé par une puissance de $m_A$.

#### Remarque 1 {#ac-x-s10-n1-rem-1 .statement}

Soient $X$ l’espace topologique $\mathrm{Spec}(A)$, $\mathcal{O}_X$ le faisceau d’anneaux structural et $\widetilde{M}$ le $\mathcal{O}_X$-module associé à $M$. Le $A$-module gradué $H_A(M)$ s’identifie au module $H_{\{m_A\}}(X, \widetilde{M})$ de cohomologie à support dans le point fermé $m_A$ de $X$.

Pour tout homomorphisme $f : M \to N$ de $A$-modules, les applications $\mathrm{Ext}_A(1_{A/a}, f) : \mathrm{Ext}_A(A/a, M) \longrightarrow \mathrm{Ext}_A(A/a, N)$ forment un système inductif d’applications linéaires graduées. Par passage à la limite inductive, on obtient un homomorphisme gradué $H_A(f) : H_A(M) \to H_A(N)$. Pour toute suite $M \xrightarrow{f} N \xrightarrow{g} P$ de $A$-modules et d’homomorphismes, on a $H_A(g \circ f) = H_A(g) \circ H_A(f)$. Soit

$$
\begin{array}{ccccccccc}
0 & \to & M & \xrightarrow{f} & N & \xrightarrow{g} & P & \to & 0
\end{array}
$$

une suite exacte de $A$-modules. D’après $\Lambda$, $X$, p. 90, prop. 8, les homomorphismes de liaison des modules d’extensions $\mathrm{Ext}_A(A/a, P) \longrightarrow \mathrm{Ext}_A(A/a, M)$ forment un système inductif d’applications $A$-linéaires, graduées de degré (ascendant) +1. Par passage à la limite inductive, on en déduit un $A$-homomorphisme $\partial(\mathscr{E}) : H_A(P) \to H_A(M)$, gradué de degré +1 , qui rend exacte la suite d’homomorphismes

$$
\ldots \longrightarrow H_A^{n-1}(P) \xrightarrow{\partial^{n-1}(\mathscr{E})} H_A^n(M) \xrightarrow{H_A^n(f)} H_A^n(N) \xrightarrow{H_A^n(g)} H_A^n(P) \xrightarrow{\partial^n(\mathscr{E})} H_A^{n+1}(M) \longrightarrow \ldots
$$

Soit M un A-module. Pour tout idéal $\alpha$ de A, le A-module $\mathrm{Hom}_A(A/\alpha, M)$ s’identifie canoniquement au sous-module de M formé des éléments annulés par $\alpha$. Ainsi $H_A^0(M)$ s’identifie au sous-module de M formé des éléments $m$ qui sont annulés par une puissance de $\mathfrak{m}_A$, c’est-à-dire tels que $\mathrm{long}_A(Am) < +\infty$. On a en particulier $H_A^0(M) = M$ lorsque M est artinien.

#### Exemple 1 {#ac-x-s10-n1-exa-1 .statement}

Si M est injectif, le A-module $H_A^i(M)$ est nul pour $i > 0$ et injectif pour $i = 0$ (§ 8, n° 2, lemme 1, c)).

#### Exemple 2 {#ac-x-s10-n1-exa-2 .statement}

Si $H_A^0(M) = M$ (par exemple si M est artinien), $H_A^i(M)$ est nul pour $i > 0$. Soit en effet (I, e) une enveloppe injective de M. Le sous-module $H_A^0(I)$ de I est injectif (exemple 1) et contient $e(M)$, donc est égal à I. Posons $N = \mathrm{Coker}\,e$ et considérons la suite exacte $0 \to M \xrightarrow{e} I \xrightarrow{p} N \to 0$. Comme $I = H_A^0(I)$, on a $N = H_A^0(N)$ et l’homomorphisme $H_A^0(p)$ est surjectif. Puisque $H_A^i(I)$ est nul pour $i > 0$ (exemple 1), $H_A^1(M)$ est nul et $H_A^i(M)$ est isomorphe à $H_A^{i-1}(N)$ pour $i > 1$; on conclut en raisonnant par récurrence sur l’entier $i$.

#### Exemple 3 {#ac-x-s10-n1-exa-3 .statement}

Soit $\Omega$ un A-module dualisant. Pour $i \neq \dim(A)$, on a $\mathrm{Ext}_A^i(A/\alpha, \Omega) = 0$ pour tout idéal de définition $\alpha$ de A (§ 8, n° 5, exemple 3), d’où $H_A^i(\Omega) = 0$; pour $i = \dim(A)$, le A-module $H_A^i(\Omega)$, qui est isomorphe à $\varprojlim \mathrm{Ext}_A^i(A/\mathfrak{m}_A^n, \Omega)$, est un A-module de Matlis (*loc. cit.*, exemple 6).

#### Exemple 4 {#ac-x-s10-n1-exa-4 .statement}

Soit A un anneau local noethérien intègre ; notons K son corps des fractions, et supposons $A \neq K$. C’est un A-module injectif (A, X, p. 18, exemple 1), de sorte que le module $H_A(K)$ est nul (exemple 1). De la suite exacte $0 \to A \to K \to K/A \to 0$, on tire pour tout $i$ un isomorphisme $H_A^i(K/\Lambda) \to H_A^{i+1}(A)$.

Plus généralement, pour tout A-module sans torsion M et tout entier $i$, on déduit de la suite exacte

$$
0 \to M \to K \otimes_A M \to (K/A) \otimes_A M \to 0
$$

un isomorphisme $H_A^i((K/A) \otimes_A M) \to H_A^{i+1}(M)$.

#### Exemple 5 {#ac-x-s10-n1-exa-5 .statement}

Conservons les hypothèses de l’exemple précédent et supposons de plus $\dim(A) = 1$. Soit N un A-module de torsion ; comme tout idéal non nul de A distinct de A est un idéal de définition (VIII, § 1, n° 3, prop. 6, e)), on a $H_A^0(N) = N$, et par suite $H_A^i(N) = 0$ pour $i > 0$ (exemple 2).

Soit M un A-module ; notons T(M) son sous-module de torsion. Considérons la suite exacte longue de cohomologie locale associée à la suite exacte

$$
0 \to T(M) \to M \to M/T(M) \to 0 ;
$$

compte tenu de ce qui précède, on en déduit des isomorphismes canoniques $T(M) \to H_A^0(M)$ et $H_A^1(M) \to H_A^1(M/T(M))$. Comme l’homomorphisme canonique $(K/A) \otimes_A M \to (K/A) \otimes_A (M/T(M))$ est bijectif, on obtient finalement des *isomorphismes canoniques*

$$
H_A^0(M) \to T(M) , \qquad H_A^1(M) \to (K/A) \otimes_A M .
$$

#### Proposition 1 {#ac-x-s10-prop-1 .statement}

Soient $A$ un anneau local noethérien et $M$ un $A$-module de type fini.

a) Le $A$-module $H_A(M)$ est artinien, et nul en degré $> \dim(M)$.

b) Posons $p = \operatorname{prof}_A(M)$. On a $H_A^i(M) = 0$ pour $i < p$, et $H_A^p(M) \neq 0$ si $M$ est non nul.

Prouvons a) en raisonnant par récurrence sur $\dim(M)$. Le cas $\dim(M) \leq 0$ résulte de l’exemple 2 ci-dessus. Supposons $\dim(M) > 0$ et prenons d’abord $M$ de la forme $A/\mathfrak{p}$, où $\mathfrak{p}$ est un idéal premier de $A$ distinct de $\mathfrak{m}_A$. Soit $x$ un élément de $\mathfrak{m}_A - \mathfrak{p}$; on a une suite exacte $0 \to M \xrightarrow{xM} M \longrightarrow M/xM \to 0$, avec $\dim(M/xM) = \dim(M) - 1$. On en déduit une suite exacte de cohomologie locale

$$
H_A^{i-1}(M/xM) \longrightarrow H_A^i(M) \xrightarrow{x} H_A^i(M)
$$

Tout élément de $H_A^i(M)$ est annulé par une puissance de $\mathfrak{m}_A$; pour prouver que ce module est artinien, il suffit donc de prouver que le socle de $H_A^i(M)$ est de dimension finie sur $\kappa_A$ (§ 8, n° 3, lemme 3). Par l’hypothèse de récurrence, le noyau $N$ de l’homothétie de rapport $x$ dans $H_A^i(M)$ est artinien; comme $x$ appartient à $\mathfrak{m}_A$, le socle de $H_A^i(M)$ s’identifie à celui de $N$, donc est de dimension finie. Si $i > \dim(M)$, on a $H_A^{i-1}(M/xM) = 0$ par l’hypothèse de récurrence, de sorte que l’homothétie de rapport $x$ est injective dans $H_A^i(M)$; comme tout élément de $H_A^i(M)$ est annulé par une puissance de $x$, on en déduit $H_A^i(M) = 0$, d’où a) dans le cas considéré.

Passons au cas général. Le $A$-module $M$ admet une suite de composition $(M_j)_{0 \leq j \leq n}$ telle que chaque quotient $M_j/M_{j+1}$ soit isomorphe à $A/\mathfrak{p}_j$, où $\mathfrak{p}_j$ est un idéal premier de $A$ (IV, § 1, n° 4, th. 1). Prouvons par récurrence sur $n$ que $M$ satisfait a). Le cas $n = 0$ est trivial. La suite exacte $0 \to M_1 \to M \to A/\mathfrak{p}_0 \to 0$ fournit une suite exacte de cohomologie locale

$$
H_A^i(M_1) \longrightarrow H_A^i(M) \longrightarrow H_A^i(A/\mathfrak{p}_0)
$$

le $A$-module $H_A^i(M_1)$ est artinien par l’hypothèse de récurrence, et il en est de même de $H_A^i(A/\mathfrak{p}_0)$ par les cas déjà traités; par suite $H_A^i(M)$ est artinien. Si $i > \dim(M)$, les modules $M_1$ et $A/\mathfrak{p}_0$ sont de dimension $< i$; les modules $H_A^i(M_1)$ et $H_A^i(A/\mathfrak{p}_0)$ sont donc nuls d’après l’hypothèse de récurrence et les cas déjà traités, ce qui entraîne $H_A^i(M) = 0$.

Supposons $M$ non nul, et prouvons b) par récurrence sur l’entier $p = \operatorname{prof}(M)$. Le cas $p = 0$ résulte de la définition de la profondeur. Supposons $p > 0$ et choisissons un élément $x$ de $\mathfrak{m}_A$ tel que l’homothétie $x_M$ soit injective. On obtient comme ci-dessus une suite exacte de cohomologie locale

$$
H_A^{i-1}(M/xM) \longrightarrow H_A^i(M) \xrightarrow{x} H_A^i(M)
$$

On a $\operatorname{prof}(M/xM) = \operatorname{prof}(M) - 1$ (§ 1, n° 4, prop. 7), d’où $H_A^{i-1}(M/xM) = 0$ pour $i < p$ par l’hypothèse de récurrence, ce qui implique comme ci-dessus $H_A^i(M) = 0$. En particulier $H_A^{p-1}(M)$ est nul, de sorte que l’homomorphisme $H_A^{p-1}(M/xM) \longrightarrow H_A^p(M)$ est injectif; ainsi $H_A^p(M)$ est non nul par l’hypothèse de récurrence.

On peut montrer que le module $H_A^{\dim(M)}(M)$ est non nul lorsque $M$ est non nul (exerc. 4 ; cf. n° 3, cor. du th. 2).

#### Corollaire {#ac-x-s10-n1-cor-1 .statement}

**Soit $M$ un $A$-module macaulayen, non nul et de type fini. Le $A$-module $H_A^i(M)$ est nul pour $i \neq \dim(M)$ et non nul pour $i = \dim(M)$.**

#### Remarque 2 {#ac-x-s10-n1-rem-2 .statement}

Pour tout idéal de définition $\alpha$ de $A$, le $A$-module $\mathrm{Ext}_A(A/\alpha, M)$ est annulé par $\alpha$, et $A/\alpha$ s’identifie à $\widehat{A}/\alpha \widehat{A}$; par conséquent, le $A$-module gradué $\mathrm{Ext}_A(A/\alpha, M)$ s’identifie à $\widehat{A} \otimes_A \mathrm{Ext}_A(A/\alpha, M)$, donc aussi à $\mathrm{Ext}_{\widehat{A}}(\widehat{A}/\alpha \widehat{A}, \widehat{A} \otimes_A M)$ (A, X, p. 111, prop. 10). L’ensemble des idéaux $\alpha \widehat{A}$, pour $\alpha \in \mathscr{D}$, contient les puissances de $m_{\widehat{A}}$, donc est cofinal dans l’ensemble des idéaux de définition de $\widehat{A}$; on déduit donc de ce qui précède un isomorphisme canonique de $A$-modules gradués

$$
H_A(M) \longrightarrow H_{\widehat{A}}(\widehat{A} \otimes_A M)
$$

Si le $A$-module $M$ est de type fini, le $A$-module $\widehat{A} \otimes_A M$ s’identifie au complété $\widehat{M}$ de $M$ (III, § 3, n° 4, th. 3), et on a un isomorphisme $H_A(M) \to H_{\widehat{A}}(\widehat{M})$, gradué de degré 0.

### 2. Cohomologie locale sur un anneau de Macaulay

Dans ce numéro, on suppose que $A$ est un anneau de Macaulay local ; on pose $\dim(A) = d$.

Les idéaux engendrés par une suite d’éléments de $m_A$ complètement sécante pour $A$ et de longueur $d = \dim(A)$ forment une partie cofinale $\mathscr{D}_{cs}$ dans l’ensemble $\mathscr{D}$ des idéaux de définition de $A$. En effet, soit $(x_1, \ldots, x_d)$ une suite d’éléments de $m_A$ complètement sécante pour $A$ (§ 2, n° 3, prop. 3) ; pour tout entier $n$, la suite $(x_1^n, \ldots, x_d^n)$ est complètement sécante pour $A$ (A, X, p. 158, prop. 6, c)), et engendre un idéal de définition (VIII, § 3, n° 2, cor. de la prop. 3 et th. 1) contenu dans $m_A^n$.

Soit $\alpha \in \mathscr{D}_{cs}$, et soit $\pi : L \to A/\alpha$ une résolution libre de type fini, nulle en degré $> d$ (par exemple le complexe de Koszul associé à une suite complètement sécante pour $A$ engendrant $\alpha$). Considérons le dual $L^* = \mathrm{Homgr}_A(L, A)$ de $L$ ; puisque la profondeur de $A$ est égale à $d$, on a $\mathrm{Ext}_A^i(A/\alpha, A) = 0$ pour $i < d$ (§ 1, n° 1, cor. 2 de la prop. 2). Comme $L^*$ est de longueur $\leq d$, on en déduit que $H^i(L^*)$ est nul pour $i \neq d$ et que $H^d(L^*)$ s’identifie à $\mathrm{Ext}_A^d(A/\alpha, A)$ (A, X, p. 100, th. 1). On a par suite un homologisme

$$
\pi^* : L^*(-d) \longrightarrow \mathrm{Ext}_A^d(A/\alpha, A)
$$

qui définit une résolution libre de type fini de $\mathrm{Ext}_A^d(A/\alpha, A)$.

Soit $M$ un $A$-module ; considérons les isomorphismes canoniques (*loc. cit.*)

$$
\varphi(L, M) : H(\mathrm{Homgr}_A(L, M)) \to \mathrm{Ext}_A(A/\alpha, M)
$$
$$
\psi(M, L^*(-d)) : \mathrm{Tor}^A(M, \mathrm{Ext}_A^d(A/\alpha, A)) \to H(M \otimes_A L^*)(-d)
$$

Comme le complexe L est libre de type fini, le morphisme canonique de complexes $M \otimes_A L^* \to \mathrm{Homgr}_A(L, M)$ est un isomorphisme ; on en déduit un isomorphisme de A-modules gradués $H(M \otimes_A L^*) \to H(\mathrm{Homgr}_A(L, M))$. Par composition des isomorphismes précédents, on obtient un isomorphisme de A-modules gradués, dit *canonique*

$$
\tau(L, M) : \mathrm{Tor}^A(M, \mathrm{Ext}_A^d(A/\alpha, A))(d) \longrightarrow \mathrm{Ext}_A(A/\alpha, M)
$$

qui induit pour chaque entier $i$ un isomorphisme

$$
\tau^i(L, M) : \mathrm{Tor}_{d-i}^A(M, \mathrm{Ext}_A^d(A/\alpha, A)) \longrightarrow \mathrm{Ext}_A^i(A/\alpha, M)
$$

Pour $M = A$, $\tau^d(L, A)$ est l’isomorphisme canonique de $A \otimes_A \mathrm{Ext}_A^d(A/\alpha, A)$ sur $\mathrm{Ext}_A^d(A/\alpha, A)$.

Soit $b$ un idéal de $\mathcal{D}_{cs}$ contenu dans $\alpha$. Soit $\rho : R \to A/b$ une résolution libre de type fini de longueur $\leq d$ et soit $p_{ab} : A/b \to A/\alpha$ la surjection canonique. D’après A, X, p. 49, prop. 3, il existe un morphisme de complexes $P_{LR} : R \to L$ tel que $\pi \circ P_{LR} = p_{ab} \circ \rho$. D’après la prop. 2 de A, X, p. 103, on a un diagramme commutatif

$$
\begin{array}{ccc}
\mathrm{Tor}^A(M, \mathrm{Ext}_A^d(A/\alpha, A))(d) & \xrightarrow{\mathrm{Tor}(1_M, \mathrm{Ext}^d(p_{ab}, 1_A))} & \mathrm{Tor}^A(M, \mathrm{Ext}_A^d(A/b, A))(d) \\
\downarrow \psi(L^*(-d), M) & & \downarrow \psi(R^*(-d), M) \\
H(M \otimes_A L^*) & \xrightarrow{H(1_M \otimes^t P_{LR})} & H(M \otimes_A R^*) \\
\downarrow & & \downarrow \\
H(\mathrm{Homgr}_A(L, M)) & \xrightarrow{H(\mathrm{Homgr}(P_{LR}, M))} & H(\mathrm{Homgr}_A(R, M)) \\
\downarrow \varphi(L, M) & & \downarrow \varphi(R, M) \\
\mathrm{Ext}_A(A/\alpha, M) & \xrightarrow{\mathrm{Ext}(p_{ab}, 1_M)} & \mathrm{Ext}_A(A/b, M)
\end{array}
$$

Il en résulte d’abord, en prenant $\alpha = b$, que l’isomorphisme $\tau(L, M)$ ne dépend pas du choix de la résolution L de $A/\alpha$; notons-le $\tau_\alpha(M)$. Il en résulte ensuite que les $\tau_\alpha(M)$ pour $\alpha \in \mathcal{D}_{cs}$ forment un système inductif d’isomorphismes. Passant à la limite inductive, on obtient pour chaque entier $i$, compte tenu de A, X, p. 70, prop. 8, un *isomorphisme de A-modules*

$$
\tau^i(M) : \mathrm{Tor}_{d-i}^A(M, H_A^d(A)) \longrightarrow H_A^i(M)
$$

Pour $M = A$, $\tau^d(A)$ est l’isomorphisme canonique de $A \otimes_A H_A^d(A)$ sur $H_A^d(A)$.

#### Remarque 1 {#ac-x-s10-n2-rem-1 .statement}

Soit $f : M \to N$ un homomorphisme de A-modules. En utilisant A, X, p. 103, prop. 2, on prouve que les diagrammes suivants sont commutatifs :

$$
\begin{array}{ccc}
\mathrm{Tor}_{d-i}^A(M, H_A^d(A)) & \xrightarrow{\tau^i(M)} & H_A^i(M) \\
\downarrow \mathrm{Tor}_{d-i}(f,1) & & \downarrow H^i(f) \\
\mathrm{Tor}_{d-i}^A(N, H_A^d(A)) & \xrightarrow{\tau^i(N)} & H_A^i(N)
\end{array}
$$

#### Remarque 2 {#ac-x-s10-n2-rem-2 .statement}

Soit
$$
(\mathcal{E}) \quad 0 \to M \to N \to P \to 0
$$
une suite exacte de A-modules. En utilisant A, X, p. 104, prop. 3 et p. 106, prop. 4, on prouve que les diagrammes suivants sont commutatifs :

$$
\begin{array}{ccc}
\mathrm{Tor}_{d-i}^A(P, H_A^d(A)) & \xrightarrow{\tau^i(P)} & H_A^i(P) \\
\downarrow \partial_{d-i}(\mathcal{E}, H_A^d(A)) & & \downarrow \partial^i(\mathcal{E}) \\
\mathrm{Tor}_{d-i-1}^A(M, H_A^d(A)) & \xrightarrow{\tau^{i+1}(M)} & H_A^{i+1}(M)
\end{array}
$$

#### Remarque 3 {#ac-x-s10-n2-rem-3 .statement}

Considérons l’isomorphisme
$$
\tau^d(M) : M \otimes_A H_A^d(A) \longrightarrow H_A^d(M)
$$
Pour $x \in M$, notons $f_x$ l’application $a \mapsto ax$ de A dans M. Pour tout $u \in H_A^d(A)$, on a
$$
\tau^d(M)(x \otimes u) = H_A^d(f_x)(u)
$$
Cela résulte en effet de la remarque 1 appliquée à l’homomorphisme $f_x : A \to M$.

### 3. Dualité de Grothendieck sur un anneau de Macaulay

On suppose toujours que A est un anneau de Macaulay local, de dimension d. Soit $\Omega$ un A-module dualisant. Le A-module $H_A^d(\Omega)$ est un module de Matlis (§ 8, n° 5, exemple 6) ; conformément aux notations du § 8, nous poserons $D(M) = \mathrm{Hom}_A(M, H_A^d(\Omega))$ pour tout A-module M.

Considérons l’isomorphisme $\tau^d(\Omega) : \Omega \otimes H_A^d(A) \to H_A^d(\Omega)$ (n° 2). On en déduit un homomorphisme $\omega : H_A^d(A) \to \mathrm{Hom}_A(\Omega, H_A^d(\Omega))$ qui associe à un élément $u$ de $H_A^d(A)$ l’homomorphisme $x \mapsto H_A^d(f_x)(u)$ (remarque 3 ci-dessus).

#### Proposition 2 {#ac-x-s10-prop-2 .statement}

*Soit A un anneau de Macaulay local, de dimension d*, et soit $\Omega$ *un A-module dualisant*. *L’homomorphisme* $\omega : H_A^d(A) \to D(\Omega)$ *est bijectif*.

L’homomorphisme $\omega$ est la limite du système inductif d’applications $(\omega_\alpha)_{\alpha \in \mathscr{D}_{cs}}$, où
$$
\omega_\alpha : \mathrm{Ext}_A^d(A/\alpha, A) \longrightarrow \mathrm{Hom}_A(\Omega, \mathrm{Ext}_A^d(A/\alpha, \Omega))
$$

associe à un élément $u$ de $\mathrm{Ext}_A^d(A/\alpha, A)$ l’application $x \mapsto f_x \circ u$ (A, X, p. 114). Il suffit donc de prouver que chacune des applications $\omega_\alpha$ est bijective.

Soit $\alpha$ un idéal de $\mathscr{D}_{cs}$, engendré par une suite $x = (x_1, \ldots, x_d)$ complètement sécante pour $A$. Le complexe de Koszul $K^\bullet(x, A)$ fournit une résolution projective de $A/\alpha$; pour tout $A$-module $M$, le $A$-module $H^d(\mathrm{Homgr}_A(K^\bullet(x, A), M))$ s’identifie canoniquement à $M/\alpha M$ (A, X, p. 155). On en déduit un isomorphisme (A, X, p. 100)
$$
\varphi_M : M/\alpha M \longrightarrow \mathrm{Ext}_A^d(A/\alpha, M) .
$$
Soit $x \in \Omega$. Compte tenu de loc. cit., p. 103, prop. 2, on a un diagramme commutatif

$$
\begin{array}{ccc}
A/\alpha & \xrightarrow{\varphi_A} & \mathrm{Ext}_A^d(A/\alpha, A) \\
\downarrow f_x & & \downarrow \mathrm{Ext}(1_{A/\alpha}, f_x) \\
\Omega/\alpha \Omega & \xrightarrow{\varphi_\Omega} & \mathrm{Ext}_A^d(A/\alpha, \Omega)
\end{array}
$$

où $f_x$ est l’homomorphisme déduit de $f_x$ par passage aux quotients. Il en résulte que si pour tout $A$-module $M$ on identifie $\mathrm{Ext}_A^d(A/\alpha, M)$ à $M/\alpha M$ à l’aide de $\varphi_M$, l’homomorphisme $\omega_\alpha$ s’identifie à l’application $A$-linéaire de $A/\alpha$ dans $\mathrm{Hom}_A(\Omega, \Omega/\alpha \Omega)$ qui envoie 1 sur la surjection canonique, c’est-à-dire encore à l’application canonique $A/\alpha \longrightarrow \mathrm{End}_{A/\alpha}(\Omega/\alpha \Omega)$. Mais puisque le $A/\alpha$-module $\Omega/\alpha \Omega$ est dualisant (§ 9, n° 2, prop. 4), celle-ci est bijective (§ 9, n° 4, prop. 6), ce qui prouve la proposition.

Identifions le bidual de Matlis $D(D(\Omega))$ à $\widehat{\Omega}$ par l’isomorphisme $\widehat{\alpha}_\Omega$ (§ 8, n° 3, th. 2, b)).

#### Corollaire {#ac-x-s10-n3-cor-1 .statement}

*L’homomorphisme* $D(\omega) : \widehat{\Omega} \to D(H^d_A(A))$ *est un isomorphisme*.

Soient $M$ un $A$-module, et $i$ un entier. Considérons les homomorphismes canoniques (§ 8, n° 7)

$$
\rho_{d-i}(M, \Omega) : \mathrm{Tor}^A_{d-i}(M, D(\Omega)) \longrightarrow D(\mathrm{Ext}_A^{d-i}(M, \Omega))
$$
$$
\theta^{d-i}(M, H^d_A(A)) : \mathrm{Ext}_A^{d-i}(M, D(H^d_A(A))) \longrightarrow D(\mathrm{Tor}^A_{d-i}(M, H^d_A(A))) .
$$

À l’aide des isomorphismes $\omega : H^d_A(A) \to D(\Omega)$, $D(\omega) : \widehat{\Omega} \to D(H^d_A(A))$ (cor. 1 de la prop. 2) et $\tau^i(M) : \mathrm{Tor}^A_{d-i}(M, H^d_A(A)) \to H^i_A(M)$ (n° 2), on en déduit des *homomorphismes canoniques de $A$-modules*

$$
\gamma^i(M) : H^i_A(M) \longrightarrow D(\mathrm{Ext}_A^{d-i}(M, \Omega))
$$
$$
\delta^i(M) : \mathrm{Ext}_A^{d-i}(M, \widehat{\Omega}) \longrightarrow D(H^i_A(M)) .
$$

#### Théorème 1 (Dualité de Grothendieck) {#ac-x-s10-thm-1 .statement}

Soit $A$ un anneau de Macaulay local, de dimension $d$, et soit $\Omega$ un $A$-module dualisant.

a) Le $A$-module $H_A^d(\Omega)$ est un module de Matlis ; pour tout $A$-module $P$, notons $D(P)$ le dual de Matlis $\mathrm{Hom}_A(P, H_A^d(\Omega))$.

b) Pour tout $A$-module de type fini $M$ et tout entier $i$, l’homomorphisme canonique
$$
\gamma^i(M) : H_A^i(M) \longrightarrow D(\mathrm{Ext}_A^{d-i}(M, \Omega))
$$
est un isomorphisme de $A$-modules artiniens.

c) Pour tout $A$-module $M$ et tout entier $i$, l’homomorphisme canonique
$$
\delta^i(M) : \mathrm{Ext}_A^{d-i}(M, \widehat{\Omega}) \longrightarrow D(H_A^i(M))
$$
est un isomorphisme de $\widehat{A}$-modules.

Cela résulte de la prop. 6 du § 8, n° 7.

#### Corollaire {#ac-x-s10-n3-cor-2 .statement}

Soient $A$ un anneau de Macaulay local, $M$ un $A$-module non nul de type fini, de dimension $e$. Le $A$-module $H_A^e(M)$ est non nul.

Grâce à la remarque 2 du n° 1, on peut supposer que l’anneau local $A$ est complet. Dans ce cas $A$ possède un module dualisant $\Omega$ ($§ 9$, n° 3, cor. 3 de la prop. 6) ; si $H_A^e(M)$ est nul, il en est de même de son dual de Matlis $\mathrm{Ext}_A^{d-e}(M, \Omega)$, ce qui contredit la prop. 3, b) du $§ 9$, n° 1.

#### Remarque 1 {#ac-x-s10-n3-rem-1 .statement}

Lorsque le $A$-module $M$ est de type fini, le $\widehat{A}$-module $\mathrm{Ext}_A^{d-i}(M, \widehat{\Omega})$ s’identifie à $\widehat{A} \otimes_A \mathrm{Ext}_A^{d-i}(M, \Omega)$ ($A$, X, p. 108, prop. 7, c)), et $\delta^i(M)$ peut aussi s’obtenir en composant $D(\gamma^i(M))$ avec l’isomorphisme de bidualité.

#### Remarque 2 {#ac-x-s10-n3-rem-2 .statement}

Soit $u : M \to M'$ un homomorphisme de $A$-modules. D’après la remarque 1 du n° 2 et celle du $§ 8$, n° 7, les diagrammes suivants sont commutatifs :

$$
\begin{array}{ccc}
H_A^i(M) & \xrightarrow{\gamma^i(M)} & D(\mathrm{Ext}_A^{d-i}(M, \Omega)) \\
\downarrow H_A^i(u) & & \downarrow D(\mathrm{Ext}(u,1)) \\
H_A^i(M') & \xrightarrow{\gamma^i(M')} & D(\mathrm{Ext}_A^{d-i}(M', \Omega))
\end{array}
$$

$$
\begin{array}{ccc}
\mathrm{Ext}_A^{d-i}(M', \widehat{\Omega}) & \xrightarrow{\delta^i(M')} & D(H_A^i(M')) \\
\downarrow \mathrm{Ext}(u,1) & & \downarrow D(H_A^i(u)) \\
\mathrm{Ext}_A^{d-i}(M, \widehat{\Omega}) & \xrightarrow{\delta^i(M)} & D(H_A^i(M))
\end{array}
$$

#### Remarque 3 {#ac-x-s10-n3-rem-3 .statement}

Soit

$$(\mathcal{E})$$
$$0 \to M' \to M \to M'' \to 0$$

une suite exacte de $A$-modules. D’après la remarque 2 du n° 2 et celle du § 8, n° 7, les diagrammes suivants sont commutatifs :

$$
\begin{array}{ccc}
H_A^{i-1}(M'') & \xrightarrow{\gamma^{i-1}(M'')} & D(\mathrm{Ext}_A^{d-i+1}(M'', \Omega)) \\
\downarrow & & \downarrow (-1)^{d-i+1}D(\delta^d i(\mathcal{E}, \Omega)) \\
H_A^i(M') & \xrightarrow{\gamma^i(M')} & D(\mathrm{Ext}_A^{d-i}(M', \Omega))
\end{array}
$$

$$
\begin{array}{ccc}
\mathrm{Ext}_A^{d-i}(M', \widehat{\Omega}) & \xrightarrow{\delta^i(M')} & D(H_A^i(M')) \\
\downarrow & & \downarrow (-1)^{d-i+1}D(\partial^{i-1}(\mathcal{E})) \\
\mathrm{Ext}_A^{d-i+1}(M'', \widehat{\Omega}) & \xrightarrow{\delta^{i-1}(M'')} & D(H_A^{i-1}(M''))
\end{array}
$$

#### Exemple {#ac-x-s10-n3-exa-1 .statement}

Soit $A$ un anneau local noethérien intègre de dimension 1 ; notons $K$ son corps des fractions. Soit $\Omega$ un $A$-module dualisant, et soit $M$ un $A$-module de type fini. Les $A$-modules $H_A^0(M)$ et $H_A^1(M)$ s’identifient canoniquement à $T(M)$ et $(K/A) \otimes_A M$ (n° 1, exemple 5). Avec ces identifications, les isomorphismes de dualité

$$\gamma^0(M) : T(M) \longrightarrow D(\mathrm{Ext}_A^1(M, \Omega)) \quad , \quad \gamma^1(M) : (K/A) \otimes_A M \longrightarrow D(\mathrm{Hom}_A(M, \Omega))$$

(th. 1) ne sont autres que les isomorphismes définis au § 9, n° 6.

Exercises

## EXERCICES {#ac-x-s10-exercises}

See the [exercises for § 10](exercises/s10/).
