---
book: alg
book_title: Algebra
chapter: III
chapter_title: ALGÈBRES TENSORIELLES, ALGÈBRES EXTÉRIEURES, ALGÈBRES SYMÉTRIQUES
section: 5
section_title: Algèbre tensorielle, tenseurs
lang: fr
source: alg-i-iii-fr
book_pages: A III.184-A III.188
pdf_pages: 0442-0454, 0571-0575
extraction: ocr
subsections:
    - "no": 1
      title: Définition de l’algèbre tensorielle d’un module
      page: 55
      pdf_page: 442
    - "no": 2
      title: Propriétés fonctorielles de l’algèbre tensorielle
      page: 56
      pdf_page: 443
    - "no": 3
      title: Extension de l’anneau des scalaires
      page: 59
      pdf_page: 446
    - "no": 4
      title: Limite inductive d’algèbres tensorielles
      page: 60
      pdf_page: 447
    - "no": 5
      title: Algèbre tensorielle d’une somme directe. Algèbre tensorielle d’un module libre. Algèbre tensorielle d’un module gradué
      page: 61
      pdf_page: 448
    - "no": 6
      title: Tenseurs et notation tensorielle
      page: 63
      pdf_page: 450
statements: 14
exercises: 10
content_sha256: 06b53b876114cba75ae4c0014d6ae6dfc48cf40de6aaf3b4739f8867e2c85cb3
---

## § 5. ALGÈBRE TENSORIELLE, TENSEURS

### 1. Définition de l’algèbre tensorielle d’un module

Soient A un anneau commutatif, M un A-module. Pour tout entier $n \geqslant 0$, nous noterons $\bigotimes^n M$, ou $M^{\otimes n}$, ou $T^n(M)$, ou $T^n_A(M)$, ou $\mathrm{Tens}^n(M)$ le A-module produit tensoriel de n modules égaux à M (dit aussi *puissance tensorielle n-ème* de M); on a donc $T^1(M) = M$; on pose en outre $T^0(M) = A$. Notons $T(M)$ ou $\mathrm{Tens}(M)$ le A-module *somme directe* $\bigoplus_{n \geqslant 0} T^n(M)$. Nous allons définir sur $T(M)$ une structure de A-algèbre graduée de type $\mathbf{N}$, en définissant pour tout couple d’entiers $p \geqslant 0$, $q \geqslant 0$, une application A-linéaire $m_{pq} : T^p(M) \otimes_A T^q(M) \to T^{p+q}(M)$ (III, p. 31, *Remarque*). Pour $p > 0$ et $q > 0$, $m_{pq}$ est l’isomorphisme d’associativité (II, p. 72), et lorsque $p = 0$ (resp. $q = 0$), $m_{0,q}$ est l’isomorphisme canonique de $A \otimes_A T^q(M)$ sur $T^q(M)$ (resp. $m_{p,0}$ est l’isomorphisme canonique de $T^p(M) \otimes_A A$ sur $T^p(M)$) (II, p. 55, prop. 4). On a donc, pour $x_i \in M, \alpha \in A$,

$$
\begin{align*}
(x_1 \otimes \cdots \otimes x_p) \cdot (x_{p+1} \otimes \cdots \otimes x_{p+q}) &= x_1 \otimes \cdots \otimes x_p \otimes x_{p+1} \otimes \cdots \otimes x_{p+q} \\
\alpha \cdot (x_1 \otimes \cdots \otimes x_p) &= \alpha(x_1 \otimes \cdots \otimes x_p)
\end{align*}
$$

Il est immédiat que la multiplication ainsi définie sur $\mathbf{T}(M)$ est associative et admet pour élément unité l’élément unité 1 de $A = \mathbf{T}^0(M)$.

#### Définition 1 {#alg-iii-s5-def-1 .statement}

Pour tout module $M$ sur un anneau commutatif $A$, on appelle algèbre tensorielle de $M$, et on note $\mathbf{T}(M)$ ou Tens $(M)$ (ou $\mathbf{T}_A(M)$), l’algèbre $\bigoplus_{n \geq 0} \mathbf{T}^n(M)$ munie de la multiplication définie par (1). On appelle injection canonique de $M$ dans $\mathbf{T}(M)$ l’injection canonique $\varphi : \mathbf{T}^1(M) \to \mathbf{T}(M)$ (II, p. 12) (on écrit aussi $\varphi_M$).

#### Proposition 1 {#alg-iii-s5-prop-1 .statement}

Soient $E$ une $A$-algèbre (unifère), $f : M \to E$ une application $A$-linéaire. Il existe un homomorphisme et un seul de $A$-algèbres $g : \mathbf{T}(M) \to E$ tel que $f = g \circ \varphi$.

En d’autres termes, $(\mathbf{T}(M), \varphi)$ est solution du problème d’application universelle (E, IV, p. 23), où $\Sigma$ est l’espèce de structure de $A$-algèbre, les $\alpha$-applications étant les applications $A$-linéaires du module $M$ dans une $A$-algèbre. On observera qu’il n’est pas question ici de graduation sur l’algèbre $\mathbf{T}(M)$.

Pour toute famille finie $(x_i)_{1 \leq i \leq n}$ de $n$ éléments de $M$, on a par définition du produit dans $\mathbf{T}(M)$, $x_1 \otimes x_2 \otimes \cdots \otimes x_n = \varphi(x_1) \varphi(x_2) \cdots \varphi(x_n)$; on a donc nécessairement $g(x_1 \otimes x_2 \otimes \cdots x_n) = f(x_1) f(x_2) \cdots f(x_n)$ pour $n \geq 1$, et $g(\alpha) = \alpha e$ (si $e$ est l’élément unité de $E$) pour $\alpha \in A$, ce qui prouve l’unicité de $g$. Réciproquement, notons que, pour tout $n > 0$, l’application
$$
(x_1, \ldots, x_n) \mapsto f(x_1) f(x_2) \cdots f(x_n)
$$
de $M^n$ dans $E$ est $A$-multilinéaire; donc il lui correspond une application $A$-linéaire $g_n : \mathbf{T}^n(M) \to E$ telle que
$$
g_n(x_1 \otimes x_2 \otimes \cdots \otimes x_n) = f(x_1) f(x_2) \cdots f(x_n).
$$
Définissons d’autre part l’application $g_0 : \mathbf{T}^0(M) \to E$ comme égale à $\eta_E$ (III, p. 6) autrement dit $g_0(\alpha) = \alpha e$ pour $\alpha \in A$. Soit $g$ l’unique application $A$-linéaire de $\mathbf{T}(M)$ dans $E$ dont la restriction à $\mathbf{T}^n(M)$ est $g_n$ ($n \geq 0$); il est immédiat que $g \circ \varphi = g_1 = f$, et il reste à vérifier que $g$ est un homomorphisme de $A$-algèbres. On a par construction $g(1) = e$, et il suffit, par linéarité, de voir que $g(uv) = g(u) g(v)$ pour $u \in \mathbf{T}^p(M)$ et $v \in \mathbf{T}^q(M)$ ($p > 0,\ q > 0$); or il résulte des formules (1) et (2) que cette relation est vraie lorsque $u = x_1 \otimes x_2 \otimes \cdots \otimes x_p$ et $v = x_{p+1} \otimes \cdots \otimes x_{p+q}$ (où les $x_i$ appartiennent à $E$). Elle est donc vraie pour $u \in \mathbf{T}^p(M)$ et $v \in \mathbf{T}^q(M)$ par linéarité.

#### Remarque {#alg-iii-s5-n1-rem-1 .statement}

Supposons que $E$ soit une $A$-algèbre graduée de type $\mathbf{Z}$, de graduation $(E_n)$, et supposons en outre que l’on ait
$$
f(M) \subset E_1.
$$
Alors il résulte de (2) que $g(\mathbf{T}^p(M)) \subset E_p$ pour tout $p \geq 0$, donc $g$ est un homomorphisme d’algèbres graduées.

### 2. Propriétés fonctorielles de l’algèbre tensorielle

#### Proposition 2 {#alg-iii-s5-prop-2 .statement}

Soient $A$ un anneau commutatif, $M$ et $N$ deux $A$-modules, $u : M \to N$ une application A-linéaire. Il existe un homomorphisme de A-algèbres et un seul, $u': T(M) \to T(N)$, tel que le diagramme

$$
\begin{array}{ccc}
M & \xrightarrow{u} & N \\
\varphi_M \downarrow & & \varphi_N \downarrow \\
T(M) & \xrightarrow{u'} & T(N)
\end{array}
$$

soit commutatif. En outre, $u'$ est un homomorphisme d’algèbres graduées.

L’existence et l’unicité de $u'$ résultent de III, p. 56, prop. 1, appliquée à l’algèbre $T(N)$ et à l’application linéaire $\varphi_N \circ u : M \to T(N)$; comme
$$
u(M) \subset T^1(N) = N,
$$
le fait que $u'$ soit un homomorphisme d’algèbres graduées résulte de la Remarque de III, p. 56.

L’homomorphisme $u'$ de la prop. 2 sera désormais noté $T(u)$. Si P est un A-module et $v : N \to P$ une application A-linéaire, on a
$$
T(v \circ u) = T(v) \circ T(u)
$$
car $T(v) \circ T(u)$ est un homomorphisme d’algèbres qui rend commutatif le diagramme

$$
\begin{array}{ccc}
M & \xrightarrow{v \circ u} & P \\
\varphi_M \downarrow & & \varphi_P \downarrow \\
T(M) & \xrightarrow{T(v) \circ T(u)} & T(P)
\end{array}
$$

On dit parfois que $T(u)$ est le prolongement canonique de $u$ à $T(M)$ (qui contient $M = T^1(M)$). On notera que la restriction $T^n(u) : T^n(M) \to T^n(N)$ n’est autre que l’application linéaire $u^{\otimes n} = u \otimes u \otimes \cdots \otimes u$ ($n$ fois), car on a
$$
T^n(u)(x_1 \otimes \cdots \otimes x_n) = u(x_1) \otimes \cdots \otimes u(x_n)
$$
puisque $T(u)$ est un homomorphisme d’algèbres et $T^1(u) = u$; la restriction $T^0(u)$ à A est l’application identique. On dit que $T^n(u) = u^{\otimes n}$ est la puissance tensorielle $n$-ème de $u$.

#### Proposition 3 {#alg-iii-s5-prop-3 .statement}

Si $u : M \to N$ est une application A-linéaire surjective, l’homomorphisme $T(u) : T(M) \to T(N)$ est surjectif, et son noyau est l’idéal bilatère de $T(M)$ engendré par le noyau $P \subset M \subset T(M)$ de $u$.

En effet, $T^0(u) : T^0(M) \to T^0(N)$ est bijectif, et pour tout entier $n > 0$, $T^n(u) : T^n(M) \to T^n(N)$ est surjectif, comme on le voit par récurrence sur $n$ en utilisant II, p. 59, prop. 6; cette dernière proposition montre aussi, par récurrence sur $n$, que le noyau $S_n$ de $T^n(u)$ est le sous-module de $T^n(M)$ engendré par les produits $x_1 \otimes x_2 \otimes \cdots \otimes x_n$ où l’un au moins des $x_i$ appartient à $P$. Cela montre que le noyau $\mathfrak{J} = \bigoplus_{n \geq 1} \mathfrak{J}_n$ de $T(u)$ est l’idéal bilatère engendré par $P$ dans $T(M)$.

Si $u : M \to N$ est une application linéaire injective, il n’est pas toujours vrai que $T(u)$ soit une application injective (III, p. 184, exerc. 1). Toutefois, il en est ainsi lorsque $u$ est une injection telle que $u(M)$ soit un facteur direct de $N$, car alors il existe une application linéaire $v : N \to M$ telle que $v \circ u$ soit l’application identique de $M$, et par suite $T(v \circ u) = T(v) \circ T(u)$ est l’application identique de $T(M)$, donc $T(u)$ est injective et son image (isomorphe à $T(M)$) est facteur direct de $T(N)$ (II, p. 20, prop. 15). Plus précisément:

#### Proposition 4 {#alg-iii-s5-prop-4 .statement}

*Soient $N$ et $P$ deux sous-modules d’un $A$-module $M$, tels que leur somme $N + P$ soit facteur direct dans $M$, et que leur intersection $N \cap P$ soit facteur direct dans $N$ et dans $P$. Alors les homomorphismes $T(N) \to T(M)$, $T(P) \to T(M)$ et $T(N \cap P) \to T(M)$ prolongements canoniques des injections canoniques, sont injectifs ; si l’on identifie $T(N)$, $T(P)$ et $T(N \cap P)$ à des sous-algèbres de $T(M)$ au moyen de ces homomorphismes, on a*

$$
T(N \cap P) = T(N) \cap T(P).
$$

Par hypothèse, il existe des sous-modules $N' \subset N$ et $P' \subset P$ tels que $N = N' \oplus (N \cap P)$, $P = P' \oplus (N \cap P)$; on a alors

$$
N + P = N' \oplus P' \oplus (N \cap P),
$$

et il existe, par hypothèse, un sous-module $M'$ de $M$ tel que

$$
M = M' \oplus (N + P) = M' \oplus N' \oplus P' \oplus (N \cap P)
= M' \oplus P' \oplus N = M' \oplus N' \oplus P.
$$

En particulier $N + P, N, P$ et $N \cap P$ sont facteurs directs dans $M$, ce qui entraîne, comme on l’a vu plus haut, que les homomorphismes canoniques $T(N + P) \to T(M)$, $T(N) \to T(M)$, $T(P) \to T(M)$, $T(N \cap P) \to T(M)$ sont injectifs. Les trois algèbres $T(N)$, $T(P)$ et $T(N \cap P)$ s’identifient donc à des sous-algèbres de $T(N + P)$ et cette dernière à une sous-algèbre de $T(M)$; posant $Q = N \cap P$, il reste à montrer que, si on identifie $T(Q)$, $T(N' \oplus Q)$ et $T(P' \oplus Q)$ à des sous-algèbres de $T(N' \oplus P' \oplus Q)$, on a

$$
T(N' \oplus Q) \cap T(P' \oplus Q) = T(Q).
$$

Or, considérons le diagramme commutatif

$$
\begin{array}{ccc}
N' \oplus Q & \longrightarrow & N' \oplus P' \oplus Q \\
\downarrow & & \downarrow \\
Q & \longrightarrow & P' \oplus Q
\end{array}
$$

où les flèches horizontales sont les injections canoniques, et les flèches verticales les projections. On en déduit un diagramme commutatif

$$
\begin{array}{ccc}
T(N' \oplus Q) & \xrightarrow{u} & T(N' \oplus P' \oplus Q) \\
r \downarrow & & s \downarrow \\
T(Q) & \xrightarrow{v} & T(P' \oplus Q)
\end{array}
$$

(7)

où $r$ et $s$ sont des homomorphismes surjectifs (III, p. 57, prop. 3) et $u$ et $v$ des homomorphismes injectifs. Cela étant, pour prouver (6), notons que le second membre est évidemment contenu dans le premier; il suffit donc de voir que si

$$
x \in T(N' \oplus Q) \cap T(P' \oplus Q),
$$

alors on a $x \in T(Q)$. Or, la définition de l’homomorphisme $s$ montre que sa restriction à $T(P' \oplus Q)$ (identifié à une sous-algèbre de $T(N' \oplus P' \oplus Q)$) est l’application identique; l’hypothèse sur $x$ entraîne donc que $s(u(x)) = x$. Mais alors on a aussi $v(r(x)) = x$, autrement dit $x$ appartient à l’image de $T(Q)$ dans $T(P' \oplus Q)$, ce qu’il fallait démontrer.

#### Remarque {#alg-iii-s5-n2-rem-1 .statement}

On notera en particulier que les hypothèses de la prop. 4 sont toujours vérifiées pour des sous-modules quelconques $N, P$ de $M$, lorsque $A$ est un corps (II, p. 98, prop. 4). En outre, si $N \subset P$ et $N \neq P$, on a alors $T^n(N) \neq T^n(P)$ pour tout $n \geqslant 1$, puisque si $R$ est un supplémentaire de $P$ dans $N$, on a $T^n(P) \cap T^n(R) = \{0\}$ en vertu de (4), et $T^n(R) \neq \{0\}$.

#### Corollaire {#alg-iii-s5-n2-cor-1 .statement}

*Soient K un corps commutatif, M un espace vectoriel sur K. Pour tout élément $z \in T(M)$, il existe un plus petit sous-espace vectoriel N de M tel que $z \in T(N)$, et N est de rang fini sur K.*

Il est sous-entendu dans cet énoncé que pour tout sous-espace vectoriel $P$ de $M$, on identifie canoniquement $T(P)$ à une sous-algèbre de $T(M)$. Soit $z \in T(M)$; $z$ s’exprime comme combinaison linéaire d’éléments dont chacun est un produit fini d’éléments de $M = T^1(M)$; tous les éléments de $M$ qui interviennent dans ces produits engendrent un sous-espace vectoriel $Q$ de rang fini et l’on a $z \in T(Q)$. Soit $\mathcal{F}$ l’ensemble (non vide) des sous-espaces vectoriels $P$ de rang fini tels que $z \in T(P)$. Toute suite décroissante d’éléments de $\mathcal{F}$ est stationnaire, puisque ce sont des espaces vectoriels de rang fini. Donc $\mathcal{F}$ possède un élément minimal $N$ (E, III, p. 51). Il reste à voir que tout $P \in \mathcal{F}$ contient $N$; or, on a $z \in T(P) \cap T(N) = T(P \cap N)$ (III, p. 58, prop. 4); vu la définition de $N$, cela entraîne $N \cap P = N$, c’est-à-dire $P \supset N$.

On dit que le sous-espace $N$ de $M$ est *associé* à $z$.

### 3. Extension de l’anneau des scalaires

Soient $A, A'$ deux anneaux commutatifs, $\rho : A \to A'$ un homomorphisme d’anneaux. Soient $M$ un $A$-module, $M'$ un $A'$-module, $u : M \to M'$ un $A$-homomorphisme; comme l’injection canonique $\varphi_{M'} : M' \to T_{A'}(M')$ est aussi un

A-homomorphisme (par restriction des scalaires), il en est de même du composé $M \xrightarrow{u} M' \xrightarrow{\varphi_{M'}} T_{A'}(M')$. On en déduit (III, p. 57) un homomorphisme de A-algèbres $T_A(M) \to \rho_*(T_{A'}(M'))$, que l’on note encore $T(u): T_A(M) \to T_{A'}(M')$, qui est l’unique A-homomorphisme rendant commutatif le diagramme

$$
\begin{array}{ccc}
M & \xrightarrow{u} & M' \\
\varphi_M \downarrow & & \varphi_{M'} \downarrow \\
T_A(M) & \xrightarrow{T(u)} & T_{A'}(M')
\end{array}
$$

Si $\sigma: A' \to A''$ est un homomorphisme d’anneaux commutatifs, $M''$ un $A''$-module, $v: M' \to M''$ un $A'$-homomorphisme, la propriété d’unicité précédente montre que l’on a

$$
T(v \circ u) = T(v) \circ T(u).
$$

#### Proposition 5 {#alg-iii-s5-prop-5 .statement}

*Soient A, B deux anneaux commutatifs, $\rho : A \to B$ un homomorphisme d’anneaux, M un A-module. Le prolongement canonique*

$$
\psi : T_B(B \otimes_A M) \to B \otimes_A T_A(M)
$$

*de l’application B-linéaire $1_B \otimes \varphi_M : B \otimes_A M \to B \otimes_A T_A(M)$, est un isomorphisme de B-algèbres graduées.*

Considérons les deux homomorphismes de A-algèbres : l’injection canonique $j : B = T^0(B \otimes_A M) \to T(B \otimes_A M)$ et l’homomorphisme

$$
h = T(i) : T(M) \to T(B \otimes_A M),
$$

déduit (cf. formule (8)) de l’application A-linéaire canonique $i : M \to B \otimes_A M$. Comme $T^0(B \otimes_A M)$ est contenu dans le centre de $T(B \otimes_A M)$, on peut appliquer la prop. 5 de III, p. 36, et on obtient donc un homomorphisme de A-algèbres $\psi' : B \otimes_A T(M) \to T(B \otimes_A M)$ tel que, pour $\beta \in B, x_i \in M$ pour $1 \leq i \leq n$, on ait

$$
\psi'(\beta \otimes (x_1 \otimes x_2 \otimes \cdots \otimes x_n)) = \beta((1 \otimes x_1) \otimes (1 \otimes x_2) \otimes \cdots \otimes (1 \otimes x_n))
$$

ce qui montre aussitôt que $\psi'$ est aussi un homomorphisme de B-algèbres. Il suffit de prouver que $\psi \circ \psi'$ et $\psi' \circ \psi$ sont les applications identiques de $B \otimes_A T(M)$ et de $T(B \otimes_A M)$ respectivement. Or, ces deux algèbres sont engendrées par $B \otimes_A M$, et il est clair que $\psi \circ \psi'$ et $\psi' \circ \psi$ coïncident avec l’application identique dans $B \otimes_A M$, d’où la conclusion.

### 4. Limite inductive d’algèbres tensorielles

Soient $(A_\alpha, \varphi_{\beta \alpha})$ un système inductif filtrant d’anneaux commutatifs, $(M_\alpha, f_{\beta \alpha})$ un système inductif de $A_\alpha$-modules (II, p. 90); soient $A = \lim \longrightarrow A_\alpha$, $M = \lim \longrightarrow M_\alpha$, qui est un A-module. Pour $\alpha \leq \beta$ on déduit canoniquement du $A_\alpha$-homomorphisme $f_{\beta \alpha} : M_\alpha \to M_\beta$ un homomorphisme de $A_\alpha$-algèbres (III, p. 60, formule (8)) $f'_{\beta \alpha} = T(f_{\beta \alpha}) : T_{A_\alpha}(M_\alpha) \to T_{A_\beta}(M_\beta)$, et il résulte de (9) (III, p. 60) que $(T_{A_\alpha}(M_\alpha), f'_{\beta \alpha})$ est un système inductif de $A_\alpha$-algèbres. Soit d’autre part $f_\alpha : M_\alpha \to M$ le $A_\alpha$-homomorphisme canonique; on en déduit (III, p. 60, formule (8)) un homomorphisme de $A_\alpha$-algèbres, $f'_\alpha : T_{A_\alpha}(M_\alpha) \to T_A(M)$, et il résulte encore de (9) (III, p. 60) que les $f'_\alpha$ constituent un système inductif de $A_\alpha$-homomorphismes.

#### Proposition 6 {#alg-iii-s5-prop-6 .statement}

*Le A-homomorphisme* $f' = \varprojlim f'_\alpha : \varprojlim T_{A_\alpha}(M_\alpha) \to T_A(M)$ *est un isomorphisme d’algèbres graduées*.

Posons pour simplifier $E = T_A(M)$, $E' = \varprojlim T_{A_\alpha}(M_\alpha)$, et soit
$$
g_\alpha : T_{A_\alpha}(M_\alpha) \to E'
$$
le $A_\alpha$-homomorphisme canonique. Il est clair que les applications $A_\alpha$-linéaires composées $M_\alpha \xrightarrow{\varphi_{M_\alpha}} T_{A_\alpha}(M_\alpha) \xrightarrow{g_\alpha} E'$ forment un système inductif, et il y a donc une application $A$-linéaire et une seule $u = \varprojlim (g_\alpha \circ \varphi_{M_\alpha}) : M \to E'$ telle que $u \circ f_\alpha = g_\alpha \circ \varphi_{M_\alpha}$ pour tout $\alpha$. Cette application se factorise elle-même d’une seule manière (III, p. 56, prop. 1) en $M \xrightarrow{\varphi_M} E \xrightarrow{h} E'$, où $h$ est un homomorphisme de $A$-algèbres. Il suffira de prouver que $h \circ f' = 1_{E'}$, et $f' \circ h = 1_E$.

Notons pour cela que, pour tout indice $\alpha$, on a (III, p. 60, formule (8))
$$
h \circ f'_\alpha \circ \varphi_{M_\alpha} = h \circ \varphi_M \circ f_\alpha = u \circ f_\alpha = g_\alpha \circ \varphi_{M_\alpha}
$$
d’où, par l’assertion d’unicité de III, p. 56, prop. 1, $h \circ f'_\alpha = g_\alpha$ pour tout $\alpha$; on en tire $(h \circ f') \circ g_\alpha = g_\alpha$ pour tout $\alpha$, donc $h \circ f' = 1_{E'}$ par définition d’une limite inductive.

D’autre part, on a, en vertu de III, p. 60, formule (8),
$$
f' \circ u \circ f_\alpha = f' \circ g_\alpha \circ \varphi_{M_\alpha} = f'_\alpha \circ \varphi_{M_\alpha} = \varphi_M \circ f_\alpha,
$$
d’où de nouveau $f' \circ u = \varphi_M$ par définition d’une limite inductive; on en conclut que $f' \circ h \circ \varphi_M = \varphi_M$, et la propriété d’unicité de III, p. 56, prop. 1 donne $f' \circ h = 1_E$.

On peut aussi démontrer la prop. 6 en observant que, pour tout entier $n \geqslant 1$, on a un isomorphisme canonique de $A$-modules $\varprojlim T^n_{A_\alpha}(M_\alpha) \to T^n_A(M)$, comme il résulte par récurrence sur $n$ de II, p. 93, prop. 7. Il est immédiat de vérifier que ces isomorphismes sont les restrictions de $f'$.

### 5. Algèbre tensorielle d’une somme directe. Algèbre tensorielle d’un module libre. Algèbre tensorielle d’un module gradué

Soient $A$ un anneau commutatif, $M = \bigoplus_{\lambda \in L} M_\lambda$ la somme directe d’une famille de $A$-modules. Il résulte de II, p. 61, prop. 7, par récurrence sur $n$, que $T^n(M)$ est somme directe des sous-modules images des injections canoniques
$$
M_{\lambda_1} \otimes M_{\lambda_2} \otimes \cdots \otimes M_{\lambda_n} \to T^n(M) = M^{\otimes n}
$$

relatives à toutes les suites $(\lambda_i) \in L^n$. Identifiant $M_{\lambda_1} \otimes M_{\lambda_2} \otimes \cdots \otimes M_{\lambda_n}$ à cette image, on voit que $\mathcal{T}(M)$ est somme directe de tous les modules

$$
M_{\lambda_1} \otimes M_{\lambda_2} \otimes \cdots \otimes M_{\lambda_n},
$$

où $n$ parcourt $\mathbf{N}$, et, pour chaque $n$, $(\lambda_i)$ parcourt $L^n$.

On en déduit d’abord la conséquence suivante:

#### Théorème 1 {#alg-iii-s5-thm-1 .statement}

Soient $A$ un anneau commutatif, $M$ un $A$-module libre, $(e_\lambda)_{\lambda \in L}$ une base de $M$. Alors les éléments $e_s = e_{\lambda_1} \otimes e_{\lambda_2} \otimes \cdots \otimes e_{\lambda_n}$, où $s = (\lambda_1 \ldots, \lambda_n)$ parcourt l’ensemble de toutes les suites finies d’éléments de $L$, et où on convient que $e_\varnothing$ est l’élément unité de $\mathcal{T}(M)$, forment une base du $A$-module $\mathcal{T}(M)$.

Les éléments de cette base sont évidemment homogènes, et la table de multiplication est donnée par

$$
e_s e_t = e_{st}
$$

en notant $st$ la suite d’éléments de $L$ obtenue par juxtaposition des suites $s$ et $t$ (I, p. 79).

On voit que la base $(e_s)$ de $\mathcal{T}(M)$, munie de la loi multiplicative (10), est canoniquement isomorphe au monoïde libre construit sur l’ensemble $L$ (I, p. 79), l’isomorphisme s’obtenant en faisant correspondre à chaque mot $s$ de ce monoïde l’élément $e_s$. On en conclut (III, p. 22) que l’algèbre tensorielle $\mathcal{T}(M)$ d’un module libre $M$ muni d’une base dont $L$ est l’ensemble d’indices, est canoniquement isomorphe à l’algèbre associative libre de $L$ sur $A$. En particulier (III, p. 22, prop. 7) pour toute application $f : L \to E$ de $L$ dans une $A$-algèbre $E$, il existe un homomorphisme $\tilde{f} : \mathcal{T}(M) \to E$ de $A$-algèbres et un seul tel que $\tilde{f}(e_\lambda) = f(\lambda)$.

#### Remarque {#alg-iii-s5-n5-rem-1 .statement}

Les résultats précédents peuvent également s’obtenir comme conséquence des propriétés universelles de l’algèbre associative libre et de l’algèbre tensorielle, compte tenu de (II, p. 62, cor. 2).

#### Corollaire {#alg-iii-s5-n5-cor-1 .statement}

Si $M$ est un $A$-module projectif, $\mathcal{T}(M)$ est un $A$-module projectif.

En effet, $M$ est facteur direct d’un $A$-module libre $N$ (II, p. 39, prop. 4), donc $\mathcal{T}(M)$ est facteur direct de $\mathcal{T}(N)$ (III, p. 58); comme $\mathcal{T}(N)$ est libre (th. 1), cela montre que $\mathcal{T}(M)$ est projectif (II, p. 39).

#### Proposition 7 {#alg-iii-s5-prop-7 .statement}

Soient $\Delta$ un monoïde commutatif, $M$ un $A$-module gradué de type $\Delta$, $(M_\alpha)_{\alpha \in \Delta}$ sa graduation. Pour tout couple $(\alpha, n) \in \Delta \times \mathbf{N}$, soit $\mathcal{T}^{\alpha, n}(M)$ la somme (directe) des sous-modules $M_{\alpha_1} \otimes M_{\alpha_2} \otimes \cdots \otimes M_{\alpha_n}$ de $\mathcal{T}^n(M)$ tels que

$$
\sum_{i=1}^n \alpha_i = \alpha;
$$

alors $(\mathcal{T}^{\alpha, n}(M))_{(\alpha, n) \in \Delta \times \mathbf{N}}$ est la seule graduation de type $\Delta \times \mathbf{N}$ compatible avec la structure d’algèbre de $\mathcal{T}(M)$ et qui induise sur $M = \mathcal{T}^1(M)$ la graduation donnée.

On a vu au début de ce n° que $\mathcal{T}(M)$ est somme directe des $\mathcal{T}^{\alpha, n}(M)$, et le fait qu’il s’agisse d’une graduation compatible avec la structure d’algèbre résulte aussitôt des définitions. Si $(\mathcal{{T}'}^{\alpha, n})$ est une autre graduation de type $\Delta \times \mathbf{N}$ sur

T(M), compatible avec la structure d’algèbre, et telle que $T^{\alpha,1}(M) = T^{\prime\alpha,1}$ pour $\alpha \in \Delta$, il résulte aussitôt des définitions que l’on aura, pour tout $n \geq 1$ et tout $\alpha \in \Delta$, $T^{\alpha,n}(M) \subset T^{\prime\alpha,n}$; mais puisque $T(M)$ est aussi somme directe des $T^{\alpha,n}(M)$, cela entraîne $T^{\prime\alpha,n} = T^{\alpha,n}(M)$ (II, p. 18, Remarque).

### 6. Tenseurs et notation tensorielle

Soient A un anneau commutatif, M un A-module, M* le dual de M (II, p. 40), I et J deux ensemble finis disjoints; on note $T_J^I(M)$ le A-module $\bigotimes_{i \in I \cup J} E_i$, où $E_i = M$ si $i \in I$, $E_i = M^*$ si $i \in J$; les éléments de $T_J^I(M)$ sont dits tenseurs de type (I, J) sur M. On dit qu’ils sont contravariants si $J = \varnothing$, covariants si $I = \varnothing$, mixtes dans les autres cas.

Soient I', I'' deux parties de I et J', J'' deux parties de J, telles que $I' \cup I'' = I$, $I' \cap I'' = \varnothing$, $J' \cup J'' = J$, $J' \cap J'' = \varnothing$; alors on a un isomorphisme canonique d’associativité (II, p. 72)

$$
T_J^I(M) \to T_{J'}^{I'}(M) \otimes_A T_{J''}^{I''}(M).
$$

Si l’on considère l’algèbre tensorielle $T(M \oplus M^*)$, il résulte de III, p. 62 que $T^n(M \oplus M^*)$ s’identifie canoniquement à la somme directe des $T_J^I(M)$ où I parcourt l’ensemble des parties de l’intervalle $[1, n]$ de $\mathbf{N}$, et J est le complémentaire de I dans $[1, n]$.

Lorsque $I = [1, p]$ et $J = [p+1, p+q]$ avec des entiers $p \geq 0, q \geq 0$ (en convenant de remplacer I (resp. J) par $\varnothing$ lorsque $p = 0$ (resp. $q = 0$)), le A-module $T_J^I(M)$ se note aussi $T_q^p(M)$; les A-modules $T_0^n(M)$ et $T_n^0(M)$ sont donc par définition les A-modules $T^n(M)$ et $T^n(M^*)$ respectivement. Lorsque I et J sont des ensembles finis quelconques, de cardinaux $p = \mathrm{Card}(I)$ et $q = \mathrm{Card}(J)$, munissons chacun d’eux d’une structure d’ordre total; il existe alors une bijection croissante de I (resp. J) sur $[1, p]$ (resp. $[p+1, p+q]$), et ces bijections définissent donc un isomorphisme

$$
T_J^I(M) \to T_q^p(M).
$$

Lorsque M est un A-module projectif de type fini, il résulte de II, p. 47, cor. 4 et de II, p. 80, cor. 1, que l’on a un isomorphisme canonique

$$
(T_J^I(M))^* \to T_I^J(M).
$$

Supposons maintenant que M soit un A-module libre de type fini, et soit $(e_\lambda)_{\lambda \in L}$ une base de M (L étant donc un ensemble fini). On notera $(e^\lambda)_{\lambda \in L}$ la base de $M^*$, duale de $(e_\lambda)$ (II, p. 45). Les bases $(e_\lambda)$ et $(e^\lambda)$ de M et $M^*$ respectivement définissent (III, p. 62) une base de $T_J^I(M)$, qu’on explicite comme suit: étant données deux applications $f : I \to L$ et $g : J \to L$, soit $e_f^g$ l’élément $\bigotimes_{i \in I \cup J} x_i$ de $T_J^I(M)$, défini par

$$
x_i = e_{f(i)} \quad \text{si} \quad i \in I, \qquad x_i = e^{g(i)} \quad \text{si} \quad i \in J.
$$

Lorsque $(f, g)$ parcourt l’ensemble des couples d’applications $f : I \to L$ et $g : J \to L$, les $e_f^g$ forment une base du A-module $T_J^I(M)$, dite associée à la base donnée $(e_\lambda)$ de M. Pour $z \in T_J^I(M)$, on peut donc écrire

$$
z = \sum_{(f, g)} \alpha_g^f(z) \cdot e_f^g
$$

où les $\alpha_g^f$ sont les formes coordonnées relatives à la base $(e_f^g)$; par abus de langage, on dit que les $\alpha_g^f(z)$ sont les coordonnées du tenseur $z$ par rapport à la base $(e_\lambda)$ du module M. Les $\alpha_g^f$ constituent la base duale de $(e_f^g)$, autrement dit s’identifient aux éléments de la base de $T_I^J(M)$, associée à $(e_\lambda)$. Lorsque I et J sont des parties complémentaires d’un intervalle $[1, n]$ de $\mathbf{N}$, on note encore $\alpha_g^f$ (ou $\alpha_g^f(z)$) de la façon suivante: on écrit en indices supérieurs chaque élément $f(i)$ à la $i$-ème place pour $i \in I$, et un point à la $i$-ème place pour $i \in J$; de même, on écrit en indices inférieurs $g(i)$ à la $i$-ème place pour $i \in J$, un point à la $i$-ème place pour $i \in I$. Par exemple, pour $I = \{1, 4\}, J = \{2, 3\}$, on écrira $\alpha_{v; \rho;}^\lambda \mu$ si $f(1) = \lambda, f(4) = \mu, g(2) = v, g(3) = \rho$.

Soit $(\bar{e}_\lambda)_{\lambda \in L}$ une autre base de M, et soit $P$ la matrice de passage de $(e_\lambda)$ à $(\bar{e}_\lambda)$ (II, p. 152). Alors la matrice de passage de $(e^\lambda)$ à $(\bar{e}^\lambda)$ (base duale de $(\bar{e}_\lambda)$) est la contragrédiente $tP^{-1}$ de $P$ (II, p. 153, prop. 5). Il en résulte (II, p. 157) que la matrice de passage de la base $(e_f^g)$ de $T_J^I(M)$ à la base $(\bar{e}_f^g)$ (où $f$ (resp. $g$) parcourt l’ensemble des applications de I dans L (resp. de J dans L)) est la matrice

$$
\bigotimes_{i \in I \cup J} Q_i, \quad \text{où } Q_i = P \text{ si } i \in I, \quad Q_i = tP^{-1} \text{ si } i \in J.
$$

La transposée de cette matrice de passage s’identifie par suite à

$$
\bigotimes_{i \in I \cup J} R_i, \quad \text{où } R_i = tP^{-1} \text{ si } i \in I, \quad R_i = P \text{ si } i \in J;
$$

Supposons de nouveau le module M quelconque. Soient $i \in I, j \in J$, et posons $I' = I - \{i\}, J' = J - \{j\}$; on va définir une application A-linéaire canonique

$$
c_j^i : T_J^I(M) \to T_{J'}^{I'}, (M),
$$

dite contraction de l’indice $i$ et de l’indice $j$. Pour cela, on remarque que l’application de $M^I \times (M^*)^J$, qui à toute famille $(x_i)_{i \in I \cup J}$ où $x_i \in M$ si $i \in I$ et $x_i \in M^*$ si $j \in J$, fait correspondre l’élément

$$
\langle x_i, x_j \rangle_{k \in (I \cup J) - \{i, j\}} x_k
$$

de $T_{J'}^{I'}(M)$, est A-multilinéaire; $c_j^i$ est l’application A-linéaire correspondante.

Supposons maintenant que M soit libre de type fini, et soit $(e_\lambda)_{\lambda \in L}$ une base de M. Etant données deux applications $f : I \to L, g : J \to L$, notons $f_i$ la restriction de $f$ à $I' = I - \{i\}$, et $g_j$ la restriction de $g$ à $J' = J - \{j\}$; on a alors en vertu de (12)

$$
c_j^i(e_f^g) = \begin{cases}
0 & \text{si } f(i) \neq g(j) \\
e_{f_i}^{g_j} & \text{si } f(i) = g(j)
\end{cases}
$$

On en déduit l’expression des coordonnées de $c_j^i(z)$ en fonction de celles de $z$; pour toute application $f'$ (resp. $g'$) de $I'$ dans $L$ (resp. de $J'$ dans $L$), et tout $\lambda \in L$, désignons par $(f', \lambda)$ (resp. $(g', \lambda)$) l’application de $I$ dans $L$ (resp. de $J$ dans $L$) dont la restriction à $I'$ (resp. $J'$) est $f'$ (resp. $g'$), et qui prend la valeur $\lambda$ en l’élément $i$ (resp. $j$). Alors, si on désigne par $\beta_{g'}^{f'}$ les formes coordonnées relatives à la base $(e_{f'}^{g'})$ de $T_{J'}^I(M)$, on a

$$
\beta_{g'}^{f'}(c_j^i(z)) = \sum_{\lambda \in L} \alpha_{(g', \lambda)}^{(f', \lambda)}(z).
$$

**Exemples de tenseurs.** — 1) Soit $M$ un $A$-module *projectif de type fini*. On sait (II, p. 77, corollaire) que l’on a un isomorphisme canonique de $A$-modules

$$
\theta_M : M^* \otimes_A M \to \operatorname{End}_A(M)
$$

tel que $\theta_M(x^* \otimes x)$ (pour $x \in M, x^* \in M^*$) soit l’endomorphisme

$$
y \mapsto \langle y, x^* \rangle x.
$$

On peut donc au moyen de $\theta_M$, identifier $T_{\{1\}}^{\{2\}}(M)$ (isomorphe à $T_1^1(M)$) au $A$-module $\operatorname{End}_A(M)$. Supposons que $M$ soit un module libre et soit $(e_\lambda)_{\lambda \in L}$ une base de $M$; on note donc $\zeta_{\mu}^{\lambda}$ les coordonnées d’un tenseur $z \in M^* \otimes M$ relativement à la base $(e^\mu \otimes e_\lambda)$ de ce module. Comme $\theta_M(e^\mu \otimes e_\lambda)$ est l’endomorphisme $y \mapsto \langle y, e^\mu \rangle e_\lambda$, l’endomorphisme $u = \theta_M(z) = \theta_M(\sum_{\lambda, \mu} \zeta_{\mu}^{\lambda} e^\mu \otimes e_\lambda)$ transforme $y$ en $\sum_{\lambda, \mu} \zeta_{\mu}^{\lambda} \langle y, e^\mu \rangle e_\lambda$; faisant $y = e_\lambda$, on obtient la relation

$$
u(e_\lambda) = \sum_{\mu \in L} \zeta_{\lambda}^{\mu} e_\mu
$$

autrement dit, *la matrice de l’application linéaire* $u = \theta_M(z)$ *est celle dont l’élément qui figure dans la ligne d’indice* $\mu$ *et la colonne d’indice* $\lambda$ *est* $\zeta_{\lambda}^{\mu}$.

La définition de la *trace* de $u$ (II, p. 78) montre aussitôt que l’on a

$$
\operatorname{Tr}(\theta_M(z)) = c_1^2(z).
$$

Par suite, l’élément $z_0 = \sum_{\lambda \in L} e^\lambda \otimes e_\lambda$ (dont les coordonnées $\zeta_{\mu}^{\lambda}$ sont nulles pour $\lambda \neq \mu$, égales à 1 pour $\lambda = \mu$), qui est tel que $\theta_M(z_0) = 1_M$, est transformé de l’élément $1 \in A = T_0^0(M)$ par l’application *transposée de la contraction*

$$
c_1^2 : T_{\{1\}}^{\{2\}}(M) \to A.
$$

2) Supposons toujours que $M$ soit un $A$-module *projectif de type fini*; on a un isomorphisme canonique de $A$-modules

$$
\mu : M^* \otimes_A M^* \to (M \otimes_A M)^*
$$

(II, p. 80, cor. 1), ainsi qu’un isomorphisme canonique

$$
\theta : (M \otimes_A M)^* \otimes_A M \to \mathrm{Hom}_A(M \otimes_A M, M)
$$

(II, p. 77, corollaire); d’ailleurs $\mathrm{Hom}_A(M \otimes_A M, M)$ est canoniquement isomorphe au $A$-module $\mathcal{L}_2(M, M; M)$ des applications *A-bilinéaires* de $M \times M$ dans $M$ (II, p. 71). Composant ces isomorphismes, on obtient un isomorphisme canonique

$$
\chi_M : T^{[3]}_{\{1,2\}}(M) = M^* \otimes M^* \otimes M \to \mathcal{L}_2(M, M; M)
$$

tel que, pour $x^*, y^*$ dans $M^*$, $z \in M$, $\chi_M(x^* \otimes y^* \otimes z)$ soit l’application bilinéaire

$$
(u, v) \mapsto \langle u, x^*\rangle \langle v, y^*\rangle z.
$$

On peut donc, au moyen de $\chi_M$, identifier $T^{[3]}_{\{1,2\}}(M)$ (isomorphe à $T^1_2(M)$) au $A$-module $\mathcal{L}_2(M, M; M)$. Supposons que $M$ soit un module libre et soit $(e_\lambda)_{\lambda \in L}$ une base de $M$; on note donc $\zeta_{\lambda \mu}^{;\nu}$ les coordonnées d’un tenseur $z \in M^* \otimes M^* \otimes M$ relativement à la base $(e^\lambda \otimes e^\mu \otimes e_\nu)$ de ce module. L’application bilinéaire $\chi_M(z)$ transforme le couple $(e_\lambda, e_\mu)$ en

$$
\sum_{\nu \in L} \zeta_{\lambda \mu}^{;\nu} e_\nu
$$

et par suite les $\zeta_{\lambda \mu}^{;\nu}$ ne sont autres que les *constants de structure* de l’algèbre (non associative en général) définie sur $M$ par l’application bilinéaire $\chi_M(z)$, par rapport à la base $(e_\lambda)$ (III, p. 10).

*Remarque 2*) — Soient $(e_\lambda)_{\lambda \in L}$, $(\bar{e}_\lambda)_{\lambda \in L}$ deux bases de $M$, $P$ la matrice de passage de $(e_\lambda)$ à $(\bar{e}_\lambda)$. En raison de ce qui a été vu dans l’*Exemple 1* (III, p. 65), on note $\alpha^\lambda_\mu$ l’élément de $P$ qui figure dans la ligne d’indice $\lambda$ et la colonne d’indice $\mu$, et on note $\beta^\mu_\lambda$ l’élément de la contragrédiente ${}^tP^{-1}$ qui figure dans la ligne d’indice $\lambda$ et la colonne d’indice $\mu$. On a donc (avec les notations introduites plus haut)

$$
\begin{cases}
\bar{e}_\mu = \sum_\lambda \alpha^\lambda_\mu e_\lambda \\
\bar{e}^\mu = \sum_\lambda \beta^\mu_\lambda e^\lambda
\end{cases}
$$

$$
\bar{e}_{f'}^{g'} = \sum_{(f,g)} \left( \prod_{i \in I} \alpha_{f'(i)}^{f(i)} \right) \left( \prod_{j \in J} \beta_{g'(j)}^{g(j)} \right) e_f^g
$$

quelles que soient les applications $f' : I \to L$ et $g' : J \to L$. Les coordonnées $\zeta_g^f$ § 6 n° 1
ALGÈBRE SYMÉTRIQUE

d’un tenseur $z \in T_J^I(M)$ par rapport à la base $(e_\lambda)$ s’expriment donc à l’aide des coordonnées $\bar{\zeta}_{g'}^{f'}$ de $z$ par rapport à la base $(\bar{e}_\lambda)$ à l’aide des formules

(21)
$$
\zeta_g^f = \sum_{(f', g')} \left( \prod_{i \in I} \alpha_{f'(i)}^{g(i)} \right) \left( \prod_{j \in J} \beta_{g(j)}^{f'(j)} \right) \bar{\zeta}_{g'}^{f'}.
$$

La matrice de passage $P^{-1}$ de la base $(\bar{e}_\lambda)$ à la base $(e_\lambda)$ est la transposée de $tP^{-1}$, de sorte que $\beta_\lambda^\mu$ est l’élément qui figure dans la colonne d’indice $\lambda$ et la ligne d’indice $\mu$ de $P^{-1}$. Le calcul de $e_f^g$ à l’aide des $\bar{e}_f^{g'}$ et celui des $\bar{\zeta}_{g'}^{f'}$ à l’aide des $\zeta_g^f$ se font donc en remplaçant dans les calculs précédents, $\alpha_\mu^\lambda$ par $\beta_\lambda^\mu$ et $\beta_\lambda^\mu$ par $\alpha_\mu^\lambda$, et en échangeant les rôles de $f$ et $f'$, de $g$ et $g'$. Il vient donc

(22)
$$
e_f^g = \sum_{(f', g')} \left( \prod_{j \in J} \alpha_{g'(j)}^{g(j)} \right) \left( \prod_{i \in I} \beta_{f'(i)}^{f(i)} \right) \bar{e}_f^{g'}.
$$

(23)
$$
\bar{\zeta}_{g'}^{f'} = \sum_{(f, g)} \left( \prod_{j \in J} \alpha_{g'(j)}^{g(j)} \right) \left( \prod_{i \in I} \beta_{f'(i)}^{f(i)} \right) \zeta_g^f.
$$

Les formules précédentes sont telles que la sommation porte sur des indices qui figurent une fois en indice inférieur et une fois en indice supérieur. Certains auteurs s’autorisent de cette circonstance pour supprimer dans ces formules les signes de sommation.

## EXERCICES {#alg-iii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
