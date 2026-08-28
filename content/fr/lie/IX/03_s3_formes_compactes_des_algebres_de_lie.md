---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: GROUPES DE LIE RÉELS COMPACTS
section: 3
section_title: Formes compactes des algèbres de Lie semi-simples complexes
lang: fr
source: lie-ix-fr
book_pages: LIE IX.16-LIE IX.23, LIE IX.110-LIE IX.112
pdf_pages: 0019-0026, 0113-0115
extraction: ocr
subsections:
    - "no": 1
      title: Formes réelles
      page: 16
      pdf_page: 19
    - "no": 2
      title: Formes réelles associées à un système de Chevalley
      page: 17
      pdf_page: 20
    - "no": 3
      title: Conjugaison des formes compactes
      page: 19
      pdf_page: 22
    - "no": 4
      title: 'Exemple I : algèbres compactes de type $A_n$'
      page: 20
      pdf_page: 23
    - "no": 5
      title: 'Exemple II : algèbres compactes de type $B_n$ et $D_n$'
      page: 21
      pdf_page: 24
    - "no": 6
      title: Groupes compacts de rang 1
      page: 22
      pdf_page: 25
statements: 16
exercises: 9
content_sha256: cb86081049ae95a2b93a4811c79a54442596b1cb412021fbc2d5c405096f7bbe
---

## § 3. FORMES COMPACTES DES ALGÈBRES DE LIE SEMI-SIMPLES COMPLEXES

### 1. Formes réelles

Si $a$ est une algèbre de Lie complexe, on note $a_{[\mathbf{R}]}$ (ou parfois $a$) l’algèbre de Lie réelle obtenue par restriction des scalaires. Si $g$ est une algèbre de Lie réelle, on note $g_{(\mathbf{C})}$ (ou parfois $g_{\mathbf{C}}$) l’algèbre de Lie complexe $\mathbf{C} \otimes_{\mathbf{R}} g$ obtenue par extension des scalaires. Les homomorphismes d’algèbres de Lie réelles $g \to a_{[\mathbf{R}]}$ correspondent bijectivement aux homomorphismes d’algèbres de Lie complexes $g_{(\mathbf{C})} \to a$ : si $f : g \to a_{[\mathbf{R}]}$ et $g : g_{(\mathbf{C})} \to a$ se correspondent, on a $f(x) = g(1 \otimes x)$ et $g(\lambda \otimes x) = \lambda f(x)$ pour $x \in g, \lambda \in \mathbf{C}$.

#### Définition 1 {#lie-ix-s3-def-1 .statement tag=01B1}

Soit $a$ une algèbre de Lie complexe. On appelle forme réelle de $a$ toute sous-algèbre réelle $g$ de $a$ qui est une $\mathbf{R}$-structure sur le $\mathbf{C}$-espace vectoriel $a$ (A, II, p. 119, déf. 1).

Cela signifie donc que l’homomorphisme d’algèbres de Lie complexes $g_{(\mathbf{C})} \to a$ associé à l’injection canonique $g \to a_{[\mathbf{R}]}$ est bijectif. Une sous-algèbre réelle $g$ de $a$ est donc une forme réelle de $a$ si et seulement si les sous-espaces $g$ et $ig$ de l’espace vectoriel réel $a$ sont supplémentaires. On appelle alors conjugaison de $a$ relativement à la forme réelle $g$ l’application $\sigma : a \to a$ telle que

$$
\sigma(x + iy) = x - iy, \quad x, y \in g.
$$

#### Proposition 1 {#lie-ix-s3-prop-1 .statement tag=01JF}

a) Soient $g$ une forme réelle de $a$ et $\sigma$ la conjugaison de $a$ relativement à $g$. On a alors :

$$
\sigma^2 = \mathrm{Id}_a, \quad \sigma(\lambda x + \mu y) = \overline{\lambda} \sigma(x) + \overline{\mu} \sigma(y), \quad [\sigma(x), \sigma(y)] = \sigma[x, y]
$$

pour $\lambda, \mu \in \mathbf{C}, x, y \in a$. Pour qu’un élément $x$ de $a$ appartienne à $g$, il faut et il suffit que $\sigma(x) = x$.

b) Soit $\sigma : a \to a$ une application satisfaisant à (2). Alors l’ensemble $g$ des points fixes de $\sigma$ est une forme réelle de $a$, et $\sigma$ est la conjugaison de $a$ relativement à $g$.

La démonstration est immédiate.

Notons que si l’on désigne par $B$ la forme de Killing de $a$, et si $g$ est une forme réelle de $a$, la restriction de $B$ à $g$ est la forme de Killing de $g$; en particulier $B$ est à valeurs réelles sur $g \times g$. Supposons $a$ réductive ; pour que l’algèbre de Lie réelle $g$ soit compacte, il faut et il suffit que la restriction de $B$ à $g$ soit négative (\$ 1, no 3). On dit alors que $g$ est une forme réelle compacte de $a$.

### 2. Formes réelles associées à un système de Chevalley

Dans ce numéro, on considère une algèbre de Lie semi-simple déployée ($\mathfrak{a}, \mathfrak{h}$) sur le corps $\mathbf{C}$ (VIII, § 2, n° 1), de système de racines $R(\mathfrak{a}, \mathfrak{h}) = \mathbf{R}$, et un système de Chevalley $(X_\alpha)_{\alpha \in \mathbf{R}}$ de $(\mathfrak{a}, \mathfrak{h})$ (VIII, § 2, n° 4, déf. 3).

Rappelons (*loc. cit.*) que l’application linéaire $\theta : \mathfrak{a} \to \mathfrak{a}$ qui coïncide avec $-\mathrm{Id}_{\mathfrak{h}}$ sur $\mathfrak{h}$ et applique $X_\alpha$ sur $X_{-\alpha}$ pour tout $\alpha \in \mathbf{R}$ est un automorphisme de $\mathfrak{a}$. Par ailleurs (*loc. cit.*, prop. 7), si $\alpha, \beta, \alpha + \beta$ sont des racines, on a
$$
[X_\alpha, X_\beta] = N_{\alpha, \beta} X_{\alpha + \beta}
$$
avec $N_{\alpha, \beta} \in \mathbf{R}^*$ et
$$
N_{-\alpha - \beta} = N_{\alpha, \beta}.
$$

Notons $\mathfrak{h}_0$ le sous-espace vectoriel réel de $\mathfrak{h}$ formé des $H \in \mathfrak{h}$ tels que $\alpha(H) \in \mathbf{R}$ pour tout $\alpha \in \mathbf{R}$. Alors $\mathfrak{h}_0$ est une $\mathbf{R}$-structure sur l’espace vectoriel complexe $\mathfrak{h}$, on a $[X_\alpha, X_{-\alpha}] \in \mathfrak{h}_0$ pour tout $\alpha \in \mathbf{R}$, et la restriction de la forme de Killing $B$ de $\mathfrak{a}$ à $\mathfrak{h}_0$ est positive séparante (VIII, § 2, n° 2, remarque 2). De plus, on a
$$
B(H, X_\alpha) = 0,\quad B(X_\alpha, X_\beta) = 0 \text{ si } \alpha + \beta \neq 0,\quad B(X_\alpha, X_{-\alpha}) < 0
$$
(VIII, § 2, n° 2, prop. 1 et n° 4, lemme 3).

**Proposition 2. — a)** *Le sous-espace vectoriel réel $\mathfrak{a}_0 = \mathfrak{h}_0 + \sum_{\alpha \in \mathbf{R}} \mathbf{R} X_\alpha$ de $\mathfrak{a}$ est une forme réelle de $\mathfrak{a}$, dont $\mathfrak{h}_0$ est une sous-algèbre de Cartan. Le couple $(\mathfrak{a}_0, \mathfrak{h}_0)$ est une algèbre de Lie réelle semi-simple déployée, dont $(X_\alpha)$ est un système de Chevalley.*

*b)* *Soit $\sigma$ la conjugaison de $\mathfrak{a}$ relativement à $\mathfrak{a}_0$. On a $\sigma \circ \theta = \theta \circ \sigma$. L’ensemble des points fixes de $\sigma \circ \theta$ est une forme réelle compacte $\mathfrak{a}_u$ de $\mathfrak{a}$, dont $i \mathfrak{h}_0$ est une sous-algèbre de Cartan.*

La partie *a)* résulte immédiatement de ce qui précède. Démontrons *b)*. Comme $\sigma \circ \theta$ et $\theta \circ \sigma$ sont deux applications semi-linéaires de $\mathfrak{a}$ dans $\mathfrak{a}$ qui coïncident sur $\mathfrak{a}_0$, elles coïncident. Alors $\sigma \circ \theta$ satisfait aux conditions (2) du n° 1, donc est la conjugaison de $\mathfrak{a}$ relativement à la forme réelle $\mathfrak{a}_u$ formée des $x \in \mathfrak{a}$ tels que $\sigma \circ \theta(x) = x$ (prop. 1). Posons pour tout $\alpha \in \mathbf{R}$
$$
u_\alpha = X_\alpha + X_{-\alpha},\quad v_\alpha = i(X_\alpha - X_{-\alpha}).
$$
Alors le $\mathbf{R}$-espace vectoriel $\mathfrak{a}_u$ est engendré par $i \mathfrak{h}_0$, les $u_\alpha$ et les $v_\alpha$. Plus précisément, si on choisit une chambre $C$ de $\mathbf{R}$, on a
$$
\mathfrak{a}_u = i \mathfrak{h}_0 \oplus \bigoplus_{\alpha \in \mathbf{R}_+(C)} (\mathbf{R} u_\alpha + \mathbf{R} v_\alpha).
$$

Il est clair que $i\mathfrak{h}_0$ est une sous-algèbre de Cartan de $\alpha_u$, et il reste à prouver que la restriction de $B$ à $\alpha_u$ est négative. Or $i\mathfrak{h}_0$ et les différents sous-espaces $R u_\alpha \oplus R v_\alpha$ sont orthogonaux pour $B$, vu (5); la restriction de $B$ à $i\mathfrak{h}_0$ est négative et l’on a

$$
B(u_\alpha, u_\alpha) = B(v_\alpha, v_\alpha) = 2B(X_\alpha, X_{-\alpha}) < 0 , \quad B(u_\alpha, v_\alpha) = 0 ,
$$

d’où la conclusion.

#### Remarque {#lie-ix-s3-n2-rem-1 .statement tag=01B2}

Avec les notations précédentes, on a les formules suivantes :

(9) $$ [h, u_\alpha] = - i \alpha(h) v_\alpha , \quad [h, v_\alpha] = i \alpha(h) u_\alpha , \quad [u_\alpha, v_\alpha] = 2iH_\alpha , \quad (h \in \mathfrak{h}) $$
(10) $$ [u_\alpha, u_\beta] = N_{\alpha, \beta} u_{\alpha + \beta} + N_{\alpha, -\beta} u_{\alpha - \beta} , \quad \alpha \neq \pm \beta , $$
(11) $$ [v_\alpha, v_\beta] = - N_{\alpha, \beta} u_{\alpha + \beta} + N_{\alpha, -\beta} u_{\alpha - \beta} , \quad \alpha \neq \pm \beta , $$
(12) $$ [u_\alpha, v_\beta] = N_{\alpha, \beta} v_{\alpha + \beta} - N_{\alpha - \beta} v_{\alpha, -\beta} , \quad \alpha \neq \pm \beta , $$

(dans les trois dernières formules, on convient, comme d’habitude, que $N_{\gamma, \delta} = 0$ lorsque $\gamma + \delta$ n’est pas une racine).

On notera que $\sum R u_\alpha$ est une sous-algèbre réelle de $\alpha$, qui n’est autre que $\alpha_0 \cap \alpha_u$.

Soit $Q(R)$ le groupe des poids radiciels de $R$ (VI, § 1, no 9). Rappelons qu’à tout homomorphisme $\gamma : Q(R) \to \mathbf{C}^*$, on associe un automorphisme élémentaire $f(\gamma)$ de $\alpha$ tel que $f(\gamma)(h) = h$ pour $h \in \mathfrak{h}$ et $f(\gamma) X_\alpha = \gamma(\alpha) X_\alpha$ (VIII, § 5, no 2).

#### Proposition 3 {#lie-ix-s3-prop-3 .statement tag=01B3}

Soit $g$ une forme réelle compacte de $\alpha$ telle que $g \cap \mathfrak{h} = i\mathfrak{h}_0$. Il existe un homomorphisme $\gamma : Q(R) \to \mathbf{R}_+^*$ tel que $g = f(\gamma)(\alpha_u)$.

Soit $\tau$ la conjugaison de $\alpha$ relativement à $g$. On a par hypothèse $\tau(x) = x$ pour $x \in i\mathfrak{h}_0$, donc $\tau(x) = -x$ pour $x \in \mathfrak{h}_0$. Pour tout $\alpha \in R$, et tout $h \in \mathfrak{h}_0$, on a donc

$$
[h, \tau(X_\alpha)] = [-\tau(h), \tau(X_\alpha)] = -\tau([h, X_\alpha]) = -\tau(\alpha(h) X_\alpha) ;
$$

il s’ensuit que $[h, \tau(X_\alpha)] = -\alpha(h) \tau(X_\alpha)$ pour tout $h \in \mathfrak{h}_0$, donc aussi pour tout $h \in \mathfrak{h}$. Il existe donc $c_\alpha \in \mathbf{C}^*$ tel que $\tau(X_\alpha) = c_\alpha X_{-\alpha}$. Puisque $[X_\alpha, X_{-\alpha}] \in \mathfrak{h}_0$, on a $[\tau(X_\alpha), \tau(X_{-\alpha})] = -[X_\alpha, X_{-\alpha}]$, donc $c_\alpha \cdot c_{-\alpha} = 1$; de même, on tire des formules (3) et (4) que $c_{\alpha + \beta} = c_\alpha c_\beta$ lorsque $\alpha, \beta, \alpha + \beta$ sont des racines. D’après VI, § 1, no 6, cor. 2 à la prop. 19, il existe un homomorphisme $\delta : Q(R) \to \mathbf{C}^*$ tel que $\delta(\alpha) = c_\alpha$ pour tout $\alpha \in R$.

Montrons maintenant que chaque $c_\alpha$ est réel strictement positif. En effet, on a $c_\alpha B(X_\alpha, X_{-\alpha}) = B(X_\alpha, \tau(X_\alpha))$, et puisque $B(X_\alpha, X_{-\alpha})$ est négatif, il suffit de montrer qu’on a $B(z, \tau(z)) < 0$ pour tout élément non nul $z$ de $\alpha$; or tout élément de $\alpha$ s’écrit $x + iy$, avec $x$ et $y$ dans $g$, et on a

$$
B(x + iy, \tau(x + iy)) = B(x + iy, x - iy) = B(x, x) + B(y, y) ,
$$

d’où l’assertion annoncée, la restriction de $B$ à $g$ étant par hypothèse négative et séparante.

Il s'ensuit que l'homomorphisme $\delta$ est à valeurs dans $\mathbf{R}_+^*$; il existe donc un homomorphisme $\gamma : Q(\mathbf{R}) \to \mathbf{R}_+^*$ tel que $\delta = \gamma^{-2}$. Alors $f(\gamma)^{-1}(g)$ est une forme réelle de $\alpha$; la conjugaison correspondante est $\tau' = f(\gamma)^{-1} \circ \tau \circ f(\gamma)$. Pour tout $\alpha \in \mathbf{R}$, on a
$$
\tau'(X_\alpha) = f(\gamma)^{-1}(\tau(c_\alpha^{-1/2} X_\alpha)) = f(\gamma)^{-1}(c_\alpha^{1/2} X_{-\alpha}) = X_{-\alpha},
$$
et $\tau'(h) = \tau(h) = h$ pour $h \in i\mathfrak{h}_0$; il s'ensuit que $\tau'$ est la conjugaison par rapport à $a_u$, donc que $f(\gamma)^{-1}(g) = a_u$.

### 3. Conjugaison des formes compactes

#### Théorème 1 {#lie-ix-s3-thm-1 .statement tag=01B4}

Soit $a$ une algèbre de Lie semi-simple complexe.
a) $a$ possède des formes réelles compactes (resp. déployables).
b) Le groupe $\mathrm{Int}(a)$ opère transitivement dans l'ensemble des formes réelles compactes (resp. déployables) de $a$.

Soit $\mathfrak{h}$ une sous-algèbre de Cartan de $a$. Alors $(\alpha, \mathfrak{h})$ est déployée (VIII, § 2, n° 1, remarque 2), et possède un système de Chevalley $(X_\alpha)$ (VIII, § 4, n° 4, cor. à la prop. 5). La partie a) résulte alors de la prop. 2. Soit $g$ une forme réelle compacte de $a$; montrons qu'il existe $v \in \mathrm{Int}(a)$ tel que $v(a_u) = g$. Soit $t$ une sous-algèbre de Cartan de $g$; alors $t_{(C)}$ est une sous-algèbre de Cartan de $a$; comme $\mathrm{Int}(a)$ opère transitivement sur l'ensemble des sous-algèbres de Cartan de $a$ (VII, § 3, n° 2, th. 1), on peut se ramener au cas où $t_{(C)} = \mathfrak{h}$. Comme la forme $g$ est compacte, les valeurs propres des endomorphismes $ad\ h$, pour $h \in t$, sont imaginaires pures (§ 1, n° 3, prop. 1), donc les racines $\alpha \in \mathbf{R}$ appliquent $t$ dans $i\mathbf{R}$; cela implique $t = i\mathfrak{h}_0$. D'après la prop. 3 (n° 2), il existe alors $v \in \mathrm{Int}(a)$ tel que $v(a_u) = g$, d'où b) dans le cas des formes compactes. Enfin, soient $m_1$ et $m_2$ deux formes réelles déployables de $a$. Il existe des épingleages $(m_1, \mathfrak{h}_1, B_1, (X_\alpha^1))$ et $(m_2, \mathfrak{h}_2, B_2, (X_\alpha^2))$ (VIII, § 4, n° 1). Ceux-ci s'étendent de manière évidente en épingleages $e_1$ et $e_2$ de $a$. Un automorphisme de $a$ qui applique $e_1$ sur $e_2$ applique $m_1$ sur $m_2$; il suffit donc d'appliquer la prop. 5 de VIII, § 5, n° 3, pour obtenir l'existence d'un élément $u$ de $\mathrm{Aut}_0(a) = \mathrm{Int}(a)$ tel que $u(m_1) = m_2$.

#### Remarque {#lie-ix-s3-n3-rem-1 .statement tag=01B5}

Nous verrons plus tard une classification générale des formes réelles d'une algèbre de Lie semi-simple complexe.

#### Corollaire 1 {#lie-ix-s3-thm-1-cor-1 .statement tag=01B6}

Soient $g$ et $g'$ deux algèbres de Lie réelles compactes. Pour que $g$ et $g'$ soient isomorphes, il faut et il suffit que les algèbres de Lie complexes $g_{(C)}$ et $g'_{(C)}$ soient isomorphes.

La condition est évidemment nécessaire. Inversement, supposons $g_{(C)}$ et $g'_{(C)}$ isomorphes. Soient $c$ (resp. $c'$) le centre de $g$ (resp. $g'$) et $s$ (resp. $s'$) l'algèbre dérivée de $g$ (resp. $g'$). Alors $c_{(C)}$ et $c'_{(C)}$ sont respectivement les centres de $g_{(C)}$ et $g'_{(C)}$, donc sont isomorphes ; il s'ensuit que les algèbres commutatives $c$ et $c'$ sont isomorphes.

De même $s_{(c)}$ et $s'_{(c)}$ sont isomorphes, donc $s$ et $s'$, qui sont des formes réelles compactes de deux algèbres semi-simples complexes isomorphes, sont isomorphes d’après le th. 1, *b*).

#### Corollaire 2 {#lie-ix-s3-thm-1-cor-2 .statement tag=01B7}

*Soit $a$ une algèbre de Lie complexe. Les conditions suivantes sont équivalentes* :
(i) *$a$ est réductive*.
(ii) *Il existe une algèbre de Lie réelle compacte $g$ telle que $a$ soit isomorphe à $g_{(c)}$*.
(iii) *Il existe un groupe de Lie compact $G$ tel que $a$ soit isomorphe à $L(G)_{(c)}$*.

D’après la déf. 1 du § 1, n° 3, les conditions (ii) et (iii) sont équivalentes et impliquent (i). Si $a$ est réductive, elle est produit direct d’une algèbre commutative, qui possède évidemment une forme réelle compacte, et d’une algèbre semi-simple qui en possède une d’après le th. 1, *a*), donc (i) implique (ii).

#### Corollaire 3 {#lie-ix-s3-thm-1-cor-3 .statement tag=01B8}

*Soient $a_1$ et $a_2$ deux algèbres de Lie semi-simples complexes. Les formes réelles compactes de $a_1 \times a_2$ sont les produits $g_1 \times g_2$, où, pour $i = 1,\ 2$, $g_i$ est une forme réelle compacte de $a_i$*.

En effet, il existe une forme réelle compacte $g_1$ (resp. $g_2$) de $a_1$ (resp. $a_2$); alors $g_1 \times g_2$ est une forme réelle compacte de $a_1 \times a_2$. Le corollaire résulte alors du th. 1, *b*), appliqué à $a_1$, $a_2$ et $a_1 \times a_2$.

Il résulte notamment du cor. 3 ci-dessus qu’une algèbre de Lie réelle compacte $g$ est simple si et seulement si l’algèbre de Lie complexe $g_{(c)}$ est simple. On dit alors que $g$ est de *type* $A_n$, ou $B_n$, ..., si $g_{(c)}$ est de type $A_n$, ou $B_n$, ... (VIII, § 2, n° 2). D’après le cor. 1 ci-dessus, *deux algèbres de Lie réelles simples compactes sont isomorphes si et seulement si elles sont de même type*.

Soit $G$ un groupe de Lie compact connexe presque simple (III, § 9, n° 8, déf. 3). On dit que $G$ est de type $A_n$, ou $B_n$, ... si son algèbre de Lie est de type $A_n$, ou $B_n$, .... Deux groupes de Lie compacts presque simples simplement connexes sont isomorphes si et seulement s’ils sont de même type.

### 4. Exemple I : algèbres compactes de type $A_n$

Soient $V$ un espace vectoriel complexe de dimension finie et $\Phi$ une forme hermitienne positive séparante sur $V$. Le *groupe unitaire associé à $\Phi$* (*cf.* A, IX) est le sous-groupe $U(\Phi)$ de $\mathbf{GL}(V)$ formé des automorphismes de l’espace hilbertien complexe $(V, \Phi)$; c’est un sous-groupe de Lie (réel) du groupe $\mathbf{GL}(V)$, dont l’algèbre de Lie est la sous-algèbre $u(\Phi)$ de l’algèbre de Lie réelle $\mathbf{gl}(V)$ formée des endomorphismes $x$ de $V$ tels que $x^* = -x$ (III, § 3, n° 10, cor. 2 à la prop. 37), où l’on désigne par $x^*$ l’adjoint de $x$ relativement à $\Phi$. Comme le groupe $U(\Phi)$ est compact (§ 1, n° 1), $u(\Phi)$ est donc une algèbre de Lie réelle *compacte*. De même, le groupe *spécial unitaire* $SU(\Phi) = U(\Phi) \cap \mathbf{SL}(V)$ est un sous-groupe de Lie compact de $\mathbf{SL}(V)$, dont l’algèbre de Lie est $su(\Phi) = u(\Phi) \cap \mathfrak{sl}(V)$.

Lorsque $V = \mathbf{C}^n$ et que $\Phi$ est la forme hermitienne usuelle (pour laquelle la base canonique de $\mathbf{C}^n$ est orthonormale), on écrit $U(n, \mathbf{C}), SU(n, \mathbf{C}), u(n, \mathbf{C}), su(n, \mathbf{C})$ au lieu de $U(\Phi), SU(\Phi), u(\Phi), su(\Phi)$. Les éléments de $U(n, \mathbf{C})$ (resp. $u(n, \mathbf{C})$) sont les matrices $A \in M_n(\mathbf{C})$ telles que $A \cdot {}^t \overline{A} = I_n$ (resp. $A = - {}^t \overline{A}$), qui sont dites unitaires (resp. antihermitiennes).

#### Proposition 4 {#lie-ix-s3-prop-4 .statement tag=01B9}

*a)* *Les formes réelles compactes de l’algèbre de Lie complexe sl(V) sont les algèbres su(Φ), où Φ parcourt l’ensemble des formes hermitiennes positives séparantes sur l’espace vectoriel complexe V.*

*b)* *Les algèbres u(Φ) sont des formes réelles compactes de gl(V).*

Soit $\Phi$ une forme hermitienne positive séparante sur $V$. Pour tout $x \in gl(V)$, posons $\sigma(x) = - x^*$ (où $x^*$ est l’adjoint de $x$ relativement à $\Phi$). Alors $\sigma$ satisfait aux conditions (2) de la prop. 1 du no 1, donc l’ensemble $u(\Phi)$ (resp. $su(\Phi)$) des points fixes de $\sigma$ dans $gl(V)$ (resp. $sl(V)$) est une forme réelle compacte de $gl(V)$ (resp. $sl(V)$). Comme $GL(V)$ opère transitivement sur l’ensemble des formes hermitiennes positives séparantes sur $V$ (A, IX) et sur l’ensemble des formes réelles compactes de $sl(V)$ (no 3, th. 1 et VIII, § 13, no 1 (VII)), la prop. 4 est ainsi démontrée.

#### Corollaire {#lie-ix-s3-n4-cor-1 .statement tag=01BA}

*Toute algèbre de Lie réelle compacte simple de type $A_n$ ($n \geqslant 1$) est isomorphe à $su(n+1, \mathbf{C})$.*

En effet, toute algèbre de Lie complexe de type $A_n$ est isomorphe à $sl(n+1, \mathbf{C})$ (VIII, § 13, no 1).

#### Remarque 1 {#lie-ix-s3-n4-rem-1 .statement tag=01BB}

On a $gl(V) = sl(V) \times \mathbf{C}.1_V, u(\Phi) = su(\Phi) \times \mathbf{R}.i1_V$; les formes réelles compactes de $gl(V)$ sont les $su(\Phi) \times \mathbf{R}.\alpha 1_V, \alpha \in \mathbf{C}^*$.

#### Remarque 2 {#lie-ix-s3-n4-rem-2 .statement tag=01BC}

Si l’on munit l’algèbre de Lie complexe $a = sl(n, \mathbf{C})$ du déploiement et du système de Chevalley introduits en VIII, § 13, no 1 (IX), on a alors, avec les notations du no 2,

$$
a_u = su(n, \mathbf{C}), \quad a_0 = sl(n, \mathbf{R}), \quad a_u \cap a_0 = o(n, \mathbf{R}).
$$

### 5. Exemple II : algèbres compactes de type $B_n$ et $D_n$

Soient $V$ un espace vectoriel réel de dimension finie et $Q$ une forme quadratique positive séparante sur $V$. Le groupe orthogonal associé à $Q$ (A, IX) est le sous-groupe $O(Q)$ de $GL(V)$ formé des automorphismes de l’espace hilbertien réel $(V, Q)$; c’est un sous-groupe de Lie de $GL(V)$, dont l’algèbre de Lie est la sous-algèbre $o(Q)$ de $gl(V)$ formée des endomorphismes $x$ de $V$ tels que $x^* = - x$ (III, § 3, no 10, cor. 2 à la prop. 37), $x^*$ désignant l’adjoint de $x$ relativement à $Q$. Comme le groupe $O(Q)$ est compact, $o(Q)$ est donc une algèbre de Lie réelle *compacte*. On pose $SO(Q) = O(Q) \cap SL(V)$; c’est un sous-groupe fermé d’indice fini de $O(Q)$ (d’indice 2 si $\dim V \neq 0$), donc aussi d’algèbre de Lie $o(Q)$.

Lorsque $V = \mathbf{R}^n$ et que $Q$ est la forme quadratique usuelle (pour laquelle la base canonique de $\mathbf{R}^n$ est orthonormale), on écrit $\mathbf{O}(n, \mathbf{R}), \mathbf{SO}(n, \mathbf{R}), \mathfrak{o}(n, \mathbf{R})$ au lieu de $\mathbf{O}(Q), \mathbf{SO}(Q), \mathfrak{o}(Q)$. Les éléments de $\mathbf{O}(n, \mathbf{R})$ (resp. $\mathfrak{o}(n, \mathbf{R})$) sont les matrices $A \in \mathbf{M}_n(\mathbf{R})$ telles que $A \cdot ^tA = I_n$ (resp. $A = -\ ^tA$), qui sont dites orthogonales (resp. antisymétriques).

Soit $V_{(c)}$ le $\mathbf{C}$-espace vectoriel déduit de $V$ et soit $Q_{(c)}$ la forme quadratique sur $V_{(c)}$ déduite de $Q$. Identifions $\mathrm{gl}(V)_{(c)}$ à $\mathrm{gl}(V_{(c)})$; alors $\mathfrak{o}(Q)_{(c)}$ s’identifie à $\mathfrak{o}(Q_{(c)})$ : cela est clair puisque l’application $x \mapsto x^* + x$ de $\mathrm{gl}(V_{(c)})$ dans lui-même est $\mathbf{C}$-linéaire. Comme $\mathfrak{o}(Q_{(c)})$ est de type $B_n$ si $\dim V = 2n + 1,\ n \geqslant 1$, et de type $D_n$ si $\dim V = 2n,\ n \geqslant 3$ (VIII, § 13, nos 2 et 4), on en déduit :

#### Proposition 5 {#lie-ix-s3-prop-5 .statement tag=01BD}

*Toute algèbre de Lie réelle simple compacte de type $B_n,\ n \geqslant 1$* (resp. *de type $D_n,\ n \geqslant 3$*) *est isomorphe à $\mathfrak{o}(2n + 1, \mathbf{R})$* (resp. $\mathfrak{o}(2n, \mathbf{R})$).

### 6. Groupes compacts de rang 1

D’après TG, VIII, p. 5, prop. 3, p. 6, prop. 4 et p. 7, remarque 4, le groupe topologique $\mathbf{SU}(2, \mathbf{C})$ est isomorphe au groupe topologique $S_3$ des quaternions de norme 1, et le quotient de $\mathbf{SU}(2, \mathbf{C})$ par le sous-groupe $Z$ formé des matrices $I_2$ et $-I_2$ est isomorphe au groupe topologique $\mathbf{SO}(3, \mathbf{R})$. Notons que $Z$ est le centre de $\mathbf{SU}(2, \mathbf{C})$ : en effet, puisque $H = \mathbf{R}.S_3$, tout élément du centre du groupe $S_3$ est dans le centre $\mathbf{R}$ de l’algèbre $H$ donc appartient au groupe à deux éléments $S_3 \cap \mathbf{R} = \{ -1, 1 \}$.

#### Proposition 6 {#lie-ix-s3-prop-6 .statement tag=01BE}

*Toute algèbre de Lie réelle compacte semi-simple de rang 1 est isomorphe à $\mathfrak{su}(2, \mathbf{C})$ et à $\mathfrak{o}(3, \mathbf{R})$.* *Tout groupe de Lie compact semi-simple connexe de rang 1 est isomorphe à $\mathbf{SU}(2, \mathbf{C})$ s’il est simplement connexe, à $\mathbf{SO}(3, \mathbf{R})$ sinon.*

La première assertion résulte du cor. à la prop. 4 et de la prop. 5. Comme $\mathbf{SU}(2, \mathbf{C})$ est homéomorphe à $S_3$ (TG, VIII, p. 7, remarque 4), donc simplement connexe (TG, XI, à paraître), tout groupe de Lie compact semi-simple simplement connexe de rang 1 est isomorphe à $\mathbf{SU}(2, \mathbf{C})$; tout groupe de Lie compact semi-simple connexe de rang 1 non simplement connexe est isomorphe au quotient de $\mathbf{SU}(2, \mathbf{C})$ par un sous-groupe de $Z$ non réduit à l’élément neutre, donc à $\mathbf{SO}(3, \mathbf{R})$.

#### Remarque {#lie-ix-s3-n6-rem-1 .statement tag=01BF}

On a vu ci-dessus que $\mathbf{SU}(2, \mathbf{C})$ est simplement connexe et que $\pi_1(\mathbf{SO}(3, \mathbf{R}))$ est d’ordre 2. Nous verrons plus loin que ces résultats se généralisent respectivement à $\mathbf{SU}(n, \mathbf{C})\ (n \geqslant 1)\ ) et$ \mathbf{SO}(n, \mathbf{R})\ (n \geqslant 3)\ ) (*cf.* aussi § 3, exerc. 4 et 5).

Rappelons (VIII, § 1, n° 1) qu’on appelle base canonique de $\mathfrak{sl}(2, \mathbf{C})$ la base $(X_+, X_-, H)$, où

$$
X_+ = \begin{pmatrix} 0 & 1 \\ 0 & 0 \end{pmatrix}, \quad X_- = \begin{pmatrix} 0 & 0 \\ -1 & 0 \end{pmatrix}, \quad H = \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix}.
$$

On obtient donc une base $(U, V, iH)$ de $su(2, \mathbf{C})$ également dite canonique en posant
$$
U = X_+ + X_- = \begin{pmatrix} 0 & 1 \\ -1 & 0 \end{pmatrix}, \quad V = i(X_+ - X_-) = \begin{pmatrix} 0 & i \\ i & 0 \end{pmatrix},
$$
$$
iH = \begin{pmatrix} i & 0 \\ 0 & -i \end{pmatrix}.
$$
On a
(13)
$$
[iH, U] = 2V, \quad [iH, V] = -2U, \quad [U, V] = 2iH.
$$
Si B désigne la forme de Killing de $su(2, \mathbf{C})$, un calcul immédiat donne
(14)
$$
B(aU + bV + ciH, a'U + b'V + c'iH) = -8(aa' + bb' + cc'),
$$
de sorte que, si l’on identifie $su(2, \mathbf{C})$ à $\mathbf{R}^3$ au moyen de sa base canonique, la représentation adjointe de $SU(2, \mathbf{C})$ définit un homomorphisme $SU(2, \mathbf{C}) \to SO(3, \mathbf{R})$ (*cf.* ci-dessus).

Notons par ailleurs que $RiH$ est une sous-algèbre de Cartan de $su(2, \mathbf{C})$, que le tore maximal T de $SU(2, \mathbf{C})$ qui lui correspond est formé des matrices diagonales $\begin{pmatrix} a & 0 \\ 0 & \overline{a} \end{pmatrix}$, où $a \overline{a} = 1$, et que l’application exponentielle
$$
\exp : RiH \to T
$$
applique $xH$, pour $x \in \mathbf{R}i$, sur la matrice $\begin{pmatrix} \exp(x) & 0 \\ 0 & \exp(-x) \end{pmatrix}$, donc a pour noyau $Z.K$ où $K$ est l’élément de $su(2, \mathbf{C})$ défini par
(15)
$$
K = 2\pi iH = \begin{pmatrix} 2\pi i & 0 \\ 0 & -2\pi i \end{pmatrix}.
$$
Par ailleurs, le centre de $SU(2, \mathbf{C})$ est formé de l’identité et de $\exp(K/2)$.

Posons
(16)
$$
\theta = \begin{pmatrix} 0 & -1 \\ 1 & 0 \end{pmatrix} \in SU(2, \mathbf{C}).
$$
D’après VIII, § 1, no 5, on a
(17)
$$
\theta^2 = \begin{pmatrix} -1 & 0 \\ 0 & -1 \end{pmatrix}, \quad (\mathrm{Int}\ \theta)\ t = t^{-1}, \quad t \in T,
$$
(18)
$$(\mathrm{Ad}\ \theta)\ X_+ = X_-, \quad (\mathrm{Ad}\ \theta)\ X_- = X_+, \quad (\mathrm{Ad}\ \theta)\ U = U, \quad (\mathrm{Ad}\ \theta)\ V = -V.$$
Enfin, pour $t = \begin{pmatrix} a & 0 \\ 0 & \overline{a} \end{pmatrix} \in T$, on a
(19)
$$(\mathrm{Ad}\ t)\ X_+ = a^2 X_+, \quad (\mathrm{Ad}\ t)\ X_- = a^{-2} X_-, \quad (\mathrm{Ad}\ t)\ H = H,$$
(20)
$$(\mathrm{Ad}\ t)\ U = \mathcal{R}(a^2)\ U + \mathcal{I}(a^2)\ V, \quad (\mathrm{Ad}\ t)\ V = -\mathcal{I}(a^2)\ U + \mathcal{R}(a^2)\ V.$$

## EXERCICES {#lie-ix-s3-exercises}

See the [exercises for § 3](exercises/s3/).
