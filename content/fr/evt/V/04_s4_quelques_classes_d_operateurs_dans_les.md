---
book: evt
book_title: Topological Vector Spaces
chapter: V
chapter_title: ESPACES HILBERTIENS (THÉORIE ÉLÉMENTAIRE)
section: 4
section_title: Quelques classes d’opérateurs dans les espaces hilbertiens
lang: fr
source: evt-i-v-fr
book_pages: EVT V.73-EVT V.78
pdf_pages: 0299-0321, 0335-0340
extraction: ocr
subsections:
    - "no": 1
      title: Adjoint
      page: 37
      pdf_page: 299
    - "no": 2
      title: Applications linéaires partiellement isométriques
      page: 41
      pdf_page: 303
    - "no": 3
      title: Endomorphismes normaux
      page: 42
      pdf_page: 304
    - "no": 4
      title: Endomorphismes hermitiens
      page: 43
      pdf_page: 305
    - "no": 5
      title: Endomorphismes positifs
      page: 45
      pdf_page: 307
    - "no": 6
      title: Trace d’un endomorphisme
      page: 47
      pdf_page: 309
    - "no": 7
      title: Applications de Hilbert-Schmidt
      page: 51
      pdf_page: 313
    - "no": 8
      title: Diagonalisation des applications de Hilbert-Schmidt
      page: 54
      pdf_page: 316
    - "no": 9
      title: Trace d’une forme quadratique par rapport à une autre
      page: 56
      pdf_page: 318
statements: 50
exercises: 15
content_sha256: 5a9df8f95afa72d6677cf1bb5898ea09254e44bc9e991da52cd1fe75712c0047
---

## § 4. QUELQUES CLASSES D'OPÉRATEURS DANS LES ESPACES HILBERTIENS

Dans tout ce paragraphe, on note $1_E$ l'application identique d'un espace hilbertien E. Le composé $v \circ u$ de deux applications linéaires sera noté le plus souvent $vu$ ou $v . u$.

### 1. Adjoint

#### Proposition 1 {#evt-v-s4-prop-1 .statement}

*Soient* E *et* F *deux espaces hilbertiens*. *Pour toute application* $u \in \mathcal{L}(E; F)$, *il existe une unique application* $u^* \in \mathcal{L}(F; E)$ *telle que l'on ait*
$$(1)$$
$$
\langle u(x)|y \rangle_F = \langle x|u^*(y) \rangle_E
$$

quels que soient $x \in E$ et $y \in F$. L’application $u \mapsto u^*$ de $\mathcal{L}(E; F)$ dans $\mathcal{L}(F; E)$ est bijective, isométrique et semi-linéaire (par rapport à l’automorphisme $\xi \mapsto \overline{\xi}$ de $K$).

Soit $\mathscr{S}(E, F)$ l’espace des formes sesquilinéaires continues sur $E \times F$, muni de la norme

$$
\| \Phi \| = \sup_{\| x \| \leq 1, \| y \| \leq 1} | \Phi(x, y) |
$$

On définit de manière analogue l’espace $\mathscr{S}(F, E)$. On a défini (V, p. 16, cor. 2) un isomorphisme d’espaces de Banach de $\mathcal{L}(E; F)$ sur $\mathscr{S}(F, E)$, noté $u \mapsto \Phi_u$ et caractérisé par

$$
\Phi_u(y, x) = \langle y | u(x) \rangle_F \quad (x \in E, y \in F)
$$

On définit de manière analogue un isomorphisme de $\mathcal{L}(F; E)$ sur $\mathscr{S}(E, F)$. Enfin, on définit une application $\Phi \mapsto \Phi^*$ de $\mathscr{S}(F, E)$ sur $\mathscr{S}(E, F)$ par

$$
\Phi^*(x, y) = \overline{\Phi(y, x)} \quad (x \in E, y \in F)
$$

Elle est bijective, semi-linéaire et isométrique. Or la formule (1) se traduit par $\Phi_{u^*} = (\Phi_u)^*$, d’où aussitôt la prop. 1. C.Q.F.D.

#### Définition 1 {#evt-v-s4-def-1 .statement}

Soient $E$ et $F$ deux espaces hilbertiens. Pour toute application linéaire continue $u : E \to F$, on appelle adjoint de $u$ et l’on note $u^*$ l’application linéaire continue de $F$ dans $E$ caractérisée par la formule (1).

On a

$$
\begin{align*}
(u + v)^* &= u^* + v^* \\
(\lambda u)^* &= \overline{\lambda} u^* \\
(u^*)^* &= u \\
(1_E)^* &= 1_E \\
(wu)^* &= u^* w^*
\end{align*}
$$

dans ces formules, $u$ et $v$ appartiennent à $\mathcal{L}(E; F)$, $\lambda$ appartient à $K$, et $w$ à $\mathcal{L}(F; G)$ où $G$ est un espace hilbertien. Les formules (5) et (6) expriment que $u \mapsto u^*$ est semi-linéaire. La formule (8) est évidente. Pour prouver (7), on prend le conjugué des deux membres de (1), d’où $\langle u^*(y)|x \rangle = \langle y|u(x) \rangle$, ce qui prouve que $u$ est l’adjoint de $u^*$. Enfin, avec les notations de (9), on a, pour tout $z \in G$

$$
\langle w(u(x))|z \rangle = \langle u(x)|w^*(z) \rangle = \langle x|u^*(w^*(z)) \rangle ,
$$

donc $u^* w^*$ est l’adjoint de $wu$.

Soit $u : E \to F$ une application linéaire bijective et continue donc bicontinue (I, p. 19, cor. 1). De (8) et (9), on déduit aussitôt que $u^*$ est bijective et bicontinue et que l’on a

$$
(u^{-1})^* = (u^*)^{-1} .
$$

#### Proposition 2 {#evt-v-s4-prop-2 .statement}

Pour tout $u \in \mathcal{L}(E ; F)$, on a

$$
\|u^*u\| = \|uu^*\| = \|u\|^2 = \|u^*\|^2 .
$$

On a $\|u^*\| = \|u\|$ d’après la prop. 1, d’où $\|u^*u\| \leq \|u^*\|.\|u\| \leq \|u\|^2$. D’autre part, on a

$$
\|u\|^2 = \sup_{\|x\| \leq 1} \|u(x)\|^2 = \sup_{\|x\| \leq 1} \langle u(x)|u(x) \rangle = \sup_{\|x\| \leq 1} \langle x|u^*u(x) \rangle \leq \|u^*u\| ,
$$

d’où $\|u^*u\| = \|u\|^2$. Remplaçant $u$ par $u^*$, on en déduit $\|uu^*\| = \|u^*\|^2$, d’où (11) puisque l’on a $\|u\| = \|u^*\|$.

Soient $E_1, ..., E_n$ et $F_1, ..., F_n$ des espaces hilbertiens, et pour chaque entier $i$ compris entre 1 et $n$, soit $u_i$ une application linéaire continue de $E_i$ dans $F_i$. On a alors

$$
(u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n)^* = u_1^* \hat{\otimes}_2 ... \hat{\otimes}_2 u_n^* .
$$

Notons en effet $v$ l’application linéaire continue $u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n$ de

$$
E = E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n \quad \text{dans} \quad F = F_1 \hat{\otimes}_2 ... \hat{\otimes}_2 F_n
$$

et $w$ l’application linéaire continue $u_1^* \hat{\otimes}_2 ... \hat{\otimes}_2 u_n^*$ de $F$ dans $E$. Il s’agit de prouver l’égalité $\langle y|v(x) \rangle = \langle w(y)|x \rangle$ pour $x \in E$ et $y \in F$. Par linéarité et continuité, on se ramène au cas où $x$ et $y$ sont de la forme suivante

$$
x = x_1 \otimes ... \otimes x_n , \quad y = y_1 \otimes ... \otimes y_n
$$

avec $x_i \in E_i$ et $y_i \in F_i$ pour $1 \leq i \leq n$. Compte tenu de la définition du produit scalaire dans un produit tensoriel (V, p. 27, formule (6)), on a alors

$$
\langle y|v(x) \rangle = \prod_{i=1}^n \langle y_i|u_i(x_i) \rangle = \prod_{i=1}^n \langle u_i^*(y_i)|x_i \rangle = \langle w(y)|x \rangle ,
$$

ce qui prouve notre assertion.

Soient $E$ et $F$ des espaces hilbertiens, $u \in \mathcal{L}(E ; F)$ et $n$ un entier positif. Si l’on fait $u_1 = ... = u_n = u$ dans la formule (12), on obtient le résultat que l’application linéaire continue $\hat{T}^n(u^*)$ de $\hat{T}^n(F)$ dans $\hat{T}^n(E)$ est l’adjoint de l’application linéaire continue $\hat{T}^n(u)$ de $\hat{T}^n(E)$ dans $\hat{T}^n(F)$. Les formules

$$
\hat{S}^n(u)^* = \hat{S}^n(u^*) , \quad \hat{\Lambda}^n(u)^* = \hat{\Lambda}^n(u^*)
$$

s’établissent de manière analogue à la formule (12), compte tenu de la définition du produit scalaire dans $\hat{S}^n(E)$ (V, p. 30, formule (15)) et dans $\hat{\Lambda}^n(E)$ (V, p. 34, formule (26)).

#### Remarque 1 {#evt-v-s4-n1-rem-1 .statement}

Supposons l’espace hilbertien $E$ non réduit à 0. Identifions $\mathcal{L}(K ; E)$ à $E$ par l’application $u \mapsto u(1)$; autrement dit, le vecteur $x$ de $E$ est identifié à l’application $\lambda \mapsto \lambda.x$ de $K$ dans $E$. Alors l’adjoint de $x$ est l’application $x^*: E \to K$ donnée par $x^*(y) = \langle x|y \rangle$. Autrement dit, $x \mapsto x^*$ est l’application semi-linéaire canonique de $E$ sur son dual (V, p.15).

De même, identifions le nombre $\lambda \in K$ à l’endomorphisme $\lambda .1_E$ de E. Alors $\lambda^*$ n’est autre que le conjugué de $\lambda$.

Avec ces identifications, on peut définir un produit $t_1 \ldots t_n$ où chaque $t_i$ est, soit un nombre dans K, soit un vecteur dans E, soit une forme linéaire appartenant à $E'$, soit un élément de $\mathcal{L}(E)$, pourvu qu’il n’y ait jamais deux facteurs consécutifs $t_i$ et $t_{i+1}$ de l’un des types suivants :

• $xy$ où $x, y$ sont tous deux dans E, ou tous deux dans $E'$;
• $xA$ ou $Ax'$ avec $A \in \mathcal{L}(E)$, $x \in E$ et $x' \in E'$.

On a les règles de calcul suivantes :
a) associativité ;
b) tout élément de K commute à tous les autres facteurs ;
c) on a $(t_1 \ldots t_n)^* = t_n^* \ldots t_1^*$; autrement dit, l’adjoint d’un produit est le produit des adjoints pris dans l’ordre opposé. On a aussi $t^{**} = t$.

Par exemple, soient $x, y$ dans E et A dans $\mathcal{L}(E)$. Alors $x^*y$ représente le produit scalaire $\langle x|y \rangle$ et $x^*Ay$ représente le produit scalaire $\langle x|Ay \rangle$. On a également $(A^*x)^* = x^*A^{**} = x^*A$, d’où $(A^*x)^*y = x^*Ay$, ce qui s’interprète en

$$
\langle A^*x|y \rangle = \langle x|Ay \rangle
$$

conformément à la définition de l’adjoint. On remarquera que $yx^*$ est l’endomorphisme $z \mapsto y \langle x|z \rangle$ de E, car $yx^*z$ s’interprète par l’associativité comme $y(x^*z)$, c’est-à-dire $y.\langle x|z \rangle$.

A la suite de Dirac $^1$, il est d’usage dans la plupart des ouvrages de Physique Mathématique de représenter les éléments de E par des symboles tels que $|x\rangle$, ceux de $E'$ par $\langle t|$. Le produit scalaire s’écrit $\langle x|y \rangle = \langle x|.|y \rangle$ et la première règle d’interdiction dans les produits exclut les combinaisons de signes $|$ et $|<$, par exemple $|x\rangle |y\rangle$.

#### Proposition 3 {#evt-v-s4-prop-3 .statement}

Soient E et F deux espaces hilbertiens et $u \in \mathcal{L}(E; F)$. Les conditions suivantes sont équivalentes :

(i) $u$ est un isomorphisme d’espaces vectoriels topologiques, d’inverse égal à $u^*$;
(ii) $u$ est surjectif et $u^*u = 1_E$;
(iii) $u$ est injectif et $uu^* = 1_F$;
(iv) $u$ est un isomorphisme d’espaces normés ;
(v) $u$ est un isomorphisme d’espaces hilbertiens.

La condition (i) signifie que l’on a $u^*u = 1_E$ et $uu^* = 1_F$. L’équivalence de (i), (ii) et (iii) résulte alors de E, II, p. 18, prop. 8. On a déjà noté l’équivalence de (iv) et (v) (V, p. 5). Enfin, la relation $u^*u = 1_E$ équivaut à $\langle x|u^*u(y)\rangle = \langle x|y\rangle$, c’est-à-dire à $\langle u(x)|u(y)\rangle = \langle x|y\rangle$ pour $x, y$ dans E, et entraîne évidemment que $u$ est injectif ; ceci prouve l’équivalence de (ii) et (v).

On appelle aussi opérateur unitaire dans E tout automorphisme de l’espace hilbertien E, autrement dit, tout $u \in \mathcal{L}(E)$ satisfaisant à $uu^* = u^*u = 1_E$.

#### Remarque 2 {#evt-v-s4-n1-rem-2 .statement}

La relation $u^*u = 1_E$ ne caractérise pas les automorphismes de l’espace hilbertien E. Par exemple, soit $E = \ell^2(\mathbf{N})$ et soit $u$ défini par $u(x)_n = x_{n-1}$ pour $n \geqslant 1$ et $u(x)_0 = 0$. On a $\|u(x)\| = \|x\|$ pour tout $x \in E$, c’est-à-dire $u^*u = 1_E$, mais $u$ n’est pas surjectif.

#### Remarque 3 {#evt-v-s4-n1-rem-3 .statement}

La définition (1) de l’adjoint $u^*$ s’écrit encore $\langle y|u(x)\rangle = \langle u^*(y)|x\rangle$, ou, d’après V, p. 15,

$$
\langle u(x), y^*\rangle = \langle x, (u^*(y))^*\rangle .
$$

$^1$ Voir P. A. M. DIRAC, Quantum mechanics, Oxford University Press, New York, 1935.

Mais on a aussi $\langle u(x), y^* \rangle = \langle x, {}^t u(y^*) \rangle$, d'où l'expression de l'adjoint à l'aide du transposé

$$
(u^*(y))^* = {}^t u(y^*) .
$$

### 2. Applications linéaires partiellement isométriques

#### Définition 2 {#evt-v-s4-def-2 .statement}

Soient E et F deux espaces hilbertiens et $u \in \mathcal{L}(E ; F)$. On appelle sous-espace initial de u l'orthogonal du noyau de u dans E et sous-espace final de u l'adhérence de l'image de u dans F. On appelle orthoprojecteur initial (resp. final) de u l'orthoprojecteur de E (resp. F) sur le sous-espace initial (resp. final) de u.

Soit P le sous-espace initial de u. Comme E est somme directe de P et du noyau de u, on a $u(P) = u(E)$.

#### Proposition 4 {#evt-v-s4-prop-4 .statement}

(i) Le sous-espace initial (resp. final) de $u^*$ est égal au sous-espace final (resp. initial) de u.

(ii) Supposons que l'on ait E = F. Soient M un sous-espace vectoriel fermé de E et $M^\circ$ son orthogonal. Les relations $u(M) \subset M$ et $u^*(M^\circ) \subset M^\circ$ sont équivalentes.

Soit Q = $\overline{u(E)}$ le sous-espace final de u. L'orthogonal Q$^\circ$ de Q dans F se compose des vecteurs y tels que l'on ait $\langle u(x)|y \rangle = 0$ pour tout $x \in E$; ceci équivaut à $\langle x|u^*(y) \rangle = 0$ pour tout $x \in E$, donc à $u^*(y) = 0$. On a donc Q$^\circ$ = Ker $u^*$, donc Q est le sous-espace initial de $u^*$. Comme u est l'adjoint de $u^*$, le sous-espace final de $u^*$ est aussi le sous-espace initial de u. D'où (i).

La relation $u(M) \subset M$ signifie que $u(M)$ est orthogonal à $M^\circ$, et la relation $u^*(M^\circ) \subset M^\circ$ que $u^*(M^\circ)$ est orthogonal à M. Or on a $\langle u(x)|y \rangle = \overline{\langle u^*(y)|x \rangle}$ pour $x \in M$ et $y \in M^\circ$, d'où (ii).

On peut aussi ramener la prop. 4 aux propriétés générales des transposées (II, p. 51, cor. 2) à l'aide de la remarque 3 de V, p. 40.

#### Définition 3 {#evt-v-s4-def-3 .statement}

Soient E et F deux espaces hilbertiens. On dit qu'une application $u \in \mathcal{L}(E ; F)$ est partiellement isométrique si l'on a $\|u(x)\| = \|x\|$ pour tout x appartenant au sous-espace initial de u.

Soit $u \in \mathcal{L}(E ; F)$ de noyau N et d'image I. Dire que u est partiellement isométrique revient à dire que l'application linéaire $\tilde{u} : E/N \to I$ déduite de u est isométrique (V, p. 13). Alors le sous-espace I de F est complet, donc fermé, et c'est le sous-espace final de u. Par suite, u induit un isomorphisme d'espaces hilbertiens du sous-espace initial de u sur son sous-espace final.

#### Proposition 5 {#evt-v-s4-prop-5 .statement}

Soit $u \in \mathcal{L}(E ; F)$ de sous-espace initial P et de sous-espace final Q. On note p (resp. q) l'orthoprojecteur initial (resp. final) de u. Supposons u partiellement isométrique.

(i) L'application $u^* \in \mathcal{L}(F ; E)$ est partiellement isométrique, de sous-espace initial Q et de sous-espace final P. L'isomorphisme de P sur Q induit par u est alors réciproque de l'isomorphisme de Q sur P induit par $u^*$.

(ii) *On a* $u^*u = p$ *et* $uu^* = q$.

Compte tenu de la prop. 4 (i), l’assertion (i) est une conséquence de (ii).

Prouvons (ii). Comme P contient l’image de $u^*$, l’application $u^*u$ applique E dans P. Soient $x \in E$ et $y \in P$; on a

$$
\langle u^*u(x)|y \rangle = \langle u(x)|u(y) \rangle .
$$

Si $x$ appartient à P, on a $\langle u(x)|u(y) \rangle = \langle x|y \rangle$ par définition d’une application partiellement isométrique ; si $x$ appartient au noyau N de $u$, on a $u(x) = 0$, d’où $\langle u(x)|u(y) \rangle = 0$ et $\langle x|y \rangle = 0$ car N et P sont orthogonaux. Comme on a $E = P \oplus N$, on a dans tous les cas $\langle u^*u(x) - x|y \rangle = 0$ donc $u^*u$ est l’orthoprojecteur $p$ de E sur P. La démonstration de $uu^* = q$ s’en déduit en échangeant $u$ et $u^*$.

#### Proposition 6 {#evt-v-s4-prop-6 .statement}

*Pour tout* $u \in \mathcal{L}(E; F)$, *les conditions suivantes sont équivalentes* :

(i) *u est partiellement isométrique* ;
(ii) *$u^*$ est partiellement isométrique* ;
(iii) *$u^*u$ est un orthoprojecteur* ;
(iv) *$uu^*$ est un orthoprojecteur* ;
(v) *$uu^*u = u$* ;
(vi) *$u^*uu^* = u^*$*.

D’après la prop. 5, (i) équivaut à (ii).

(i) $\Rightarrow$ (v) : Supposons $u$ partiellement isométrique. Alors $u^*u$ est l’orthoprojecteur initial de $u$ d’après la prop. 5. Pour tout $x \in E$, $u^*u(x) - x$ appartient donc au noyau de $u$, d’où $uu^*u(x) = u(x)$.

(v) $\Rightarrow$ (iii) : Supposons que l’on ait $uu^*u = u$, et posons $p = u^*u$; on a $p = p^*$ et $p^2 = p$. Soit M (resp. N) l’image (resp. le noyau) de $p$. Pour $x \in M$ et $y \in N$, on a $\langle x|y \rangle = \langle p(x)|y \rangle = \langle x|p^*(y) \rangle = \langle x|p(y) \rangle = 0$. Comme M et N sont orthogonaux, $p$ est l’orthoprojecteur de E sur M.

(iii) $\Rightarrow$ (i) : Supposons que $p = u^*u$ soit un orthoprojecteur, d’image M et de noyau N. Pour tout $x \in E$, on a

$$
\|u(x)\|^2 = \langle u^*u(x)|x \rangle = \langle p(x)|x \rangle .
$$

On a donc $u(x) = 0$ pour $x \in N$ et $\|u(x)\| = \|x\|$ pour $x \in M$, donc $u$ est partiellement isométrique de noyau N et de sous-espace initial M.

On a donc prouvé l’équivalence de (i), (iii) et (v). Remplaçant $u$ par $u^*$, on en déduit celle des conditions (ii), (iv) et (vi). D’où la prop. 6.

### 3. Endomorphismes normaux

#### Définition 4 {#evt-v-s4-def-4 .statement}

*Soient* E *un espace hilbertien et* $u \in \mathcal{L}(E)$. *On dit que* u *est normal s’il commute à son adjoint* $u^*$.

Par exemple, tout automorphisme $u$ de l’espace hilbertien E est normal puisque l’on a $uu^* = u^*u = 1_E$.

#### Proposition 7 {#evt-v-s4-prop-7 .statement}

Pour que $u \in \mathcal{L}(E)$ soit normal, il faut et il suffit que l’on ait $\|u(x)\| = \|u^*(x)\|$ pour tout $x \in E$.

Définissons une forme hermitienne $\Phi$ sur $E$ par

$$
\Phi(x, y) = \langle uu^*(x)|y \rangle - \langle u^*u(x)|y \rangle .
$$

Pour que $u$ soit normal, il faut et il suffit que l’on ait $\Phi = 0$. D’après les formules de polarisation (V, p. 2), ceci équivaut à $\Phi(x, x) = 0$ pour tout $x \in E$, d’où la proposition car on a

$$
\Phi(x, x) = \|u^*(x)\|^2 - \|u(x)\|^2 .
$$

#### Proposition 8 {#evt-v-s4-prop-8 .statement}

Supposons que $u \in \mathcal{L}(E)$ soit normal. Soient $N$ le noyau de $u$ et $M$ l’orthogonal de $N$ dans $E$; soient $m$ et $n$ deux entiers positifs tels que $m + n \geqslant 1$. Alors $N$ est le noyau de $u^m(u^*)^n$ et $M$ est à la fois le sous-espace initial et le sous-espace final de $u^m(u^*)^n$. En particulier, $M$ est à la fois le sous-espace initial et le sous-espace final de $u$ et de $u^*$, et il est stable par $u$ et $u^*$.

La prop. 7 montre que $u$ et $u^*$ ont même noyau $N$. D’après la prop. 4, (ii) de V, p. 41, le sous-espace $M$ de $E$ est stable par $u$ et $u^*$ puisqu’il en est ainsi de $N = M^\circ$; comme on a $M \cap N = \{0\}$, les endomorphismes de $M$ induits par $u$ et $u^*$ sont injectifs. Posons $v = u^m(u^*)^n$; ce qui précède montre que la restriction de $v$ à $M$ (resp. $N$) est injective (resp. nulle), donc $N$ est le noyau de $v$. Par suite, $M = N^\circ$ est le sous-espace initial de $v$. D’après la prop. 4, (i) de V, p. 41, le sous-espace final de $v$ est égal au sous-espace initial de $v^*$. Mais on a $v^* = u^n(u^*)^m$ et le sous-espace initial de $v^*$ est donc égal à $M$ d’après ce qui précède.

#### Corollaire {#evt-v-s4-n3-cor-1 .statement}

Soit $\lambda \in K$. Les sous-espaces suivants de $E$ sont égaux :

a) le sous-espace propre de $u$ relatif à $\lambda$;
b) le sous-espace propre de $u^*$ relatif à $\overline{\lambda}$;
c) le sous-espace primaire de $u$ relatif à $\lambda$ (autrement dit, d’après LIE, VII, § 1, no 1, l’ensemble des vecteurs $x$ de $E$ pour lesquels il existe un entier $n \geqslant 0$ tel que $(u - \lambda \cdot 1_E)^n(x) = 0$);
d) le sous-espace primaire de $u^*$ relatif à $\overline{\lambda}$.

Il est clair que $w = u - \lambda \cdot 1_E$ est un endomorphisme normal de $E$, donc les endomorphismes $w, w^* = u^* - \overline{\lambda} \cdot 1_E, w^n$ et $(w^*)^n$ de $E$ ont le même noyau d’après la prop. 8.

### 4. Endomorphismes hermitiens

#### Définition 5 {#evt-v-s4-def-5 .statement}

Soient $E$ un espace hilbertien et $u \in \mathcal{L}(E)$. On dit que $u$ est hermitien si l’on a $u^* = u$.

On note $\mathscr{H}(E)$ l’ensemble des éléments hermitiens de $\mathcal{L}(E)$; c’est un sous-espace vectoriel de l’espace vectoriel $\mathcal{L}(E)_{[\mathbf{R}]}$ sur $\mathbf{R}$ déduit de $\mathcal{L}(E)$ par restriction des scalaires.

A tout $u \in \mathcal{L}(E)$, on a associé (V, p. 16, cor. 2) la forme sesquilinéaire $\Phi_u : (x, y) \mapsto \langle x | u(y) \rangle$ sur $E \times E$. On a

$$
\Phi_{u^*}(x, y) = \overline{\Phi_u(y, x)} \quad (x, y \text{ dans } E);
$$

par suite, $u$ est hermitien si et seulement si la forme $\Phi_u$ est hermitienne. Lorsque $K = \mathbf{C}$, il revient au même de supposer que $\Phi_u(x, x) = \langle x | u(x) \rangle$ est réel pour tout $x \in E$ (V, p. 2, Remarque).

Soit $u \in \mathcal{L}(E)$. On a vu (V, p. 16, cor. 2) que la norme de $u$ se calcule par la formule

$$
\|u\| = \sup_{\|x\| \leq 1, \|y\| \leq 1} |\Phi_u(x, y)| .
$$

Lorsque $u$ est hermitien, on a le résultat suivant :

#### Proposition 9 {#evt-v-s4-prop-9 .statement}

Pour tout endomorphisme hermitien $u$ de $E$, on a

$$
\|u\| = \sup_{\|x\| \leq 1} |\langle x | u(x) \rangle| .
$$

Posons $\Phi = \Phi_u$ et $c = \sup_{\|x\| \leq 1} |\Phi(x, x)|$, d'où évidemment $c \leq \|u\|$. Soient $x, y$ dans $E$ tels que $\|x\| \leq 1, \|y\| \leq 1$. On a

$$
\Phi(x + y, x + y) = \Phi(x, x) + \Phi(y, y) + 2 \Re \Phi(x, y),
$$

d'où

$$
4 \Re \Phi(x, y) = \Phi(x + y, x + y) - \Phi(x - y, x - y);
$$

par ailleurs, on a $|\Phi(t, t)| \leq c \|t\|^2$ pour tout $t \in E$, d'où

$$
4 |\Re \Phi(x, y)| \leq c (\|x + y\|^2 + \|x - y\|^2) = 2c (\|x\|^2 + \|y\|^2) \leq 4c .
$$

Soit $a = \Phi(x, y)$; il existe un nombre complexe $\lambda$ de valeur absolue 1 tel que $\lambda a = |a|$. Remplaçant $y$ par $\lambda y$ dans l'inégalité précédente, on obtient $|\Phi(x, y)| \leq c$. D'après (15), on a donc $\|u\| \leq c$, d'où la prop. 9.    C.Q.F.D.

Tout endomorphisme hermitien est évidemment normal. Réciproquement :

#### Proposition 10 {#evt-v-s4-prop-10 .statement}

On suppose $K = \mathbf{C}$. Soit $u \in \mathcal{L}(E)$. Il existe alors un couple $(h_1, h_2)$ d'endomorphismes hermitiens de $E$, et un seul, tel que $u = h_1 + ih_2$. Pour que $u$ soit normal, il faut et il suffit que $h_1$ et $h_2$ commutent.

En effet, la relation « $u = h_1 + ih_2,\ h_1^* = h_1,\ h_2^* = h_2$ » équivaut à

$$
\langle h_1 = \frac{1}{2} (u + u^*) \text{ et } h_2 = \frac{i}{2} (u^* - u) \rangle.
$$

De plus, on a alors $h_1 h_2 - h_2 h_1 = \frac{i}{2} (uu^* - u^*u)$, d'où la prop. 10.

#### Proposition 11 {#evt-v-s4-prop-11 .statement}

Soit $p \in \mathcal{L}(E)$. Pour que $p$ soit l'orthoprojecteur de $E$ sur un sous-espace vectoriel fermé de $E$, il faut et il suffit que l'on ait $p^2 = p = p^*$.

Alors E est somme directe topologique de M et N. Pour que p soit un orthoprojecteur, il faut et il suffit que M soit orthogonal à N, c'est-à-dire que l'on ait il faut et il suffit que M soit orthogonal à N, c'est-à-dire que l'on ait $\langle p(x)|y - p(y) \rangle = 0$ quels que soient x, y dans E. Cette dernière relation équivaut à $p = p^*p$. Elle entraîne $p^* = (p^*p)^* = p^*p = p$; réciproquement si $p^* = p$, on a $p = p^2 = p^*p$.

### 5. Endomorphismes positifs

#### Définition 6 {#evt-v-s4-def-6 .statement}

Soient E un espace hilbertien et $u \in \mathcal{L}(E)$. On dit que u est positif, ce que l'on note $u \geqslant 0$, si u est hermitien et si l'on a $\langle x|u(x) \rangle \geqslant 0$ pour tout $x \in E$.

Lorsque K est égal à C, la relation
$$
\langle x|u(x) \rangle \geqslant 0 \text{ pour tout } x \in E
$$
entraîne que u est hermitien (V, p. 2, Remarque), donc positif.

On note $\mathcal{L}_+(E)$ l'ensemble des éléments positifs de $\mathcal{L}(E)$; c'est un cône convexe pointé saillant de l'espace vectoriel réel $\mathcal{L}(E)_{[\mathbf{R}]}$ sous-jacent à $\mathcal{L}(E)$. Pour que u soit positif, il faut et il suffit que la forme sesquilinéaire $\Phi_u$ sur $E \times E$ associée à u soit hermitienne positive. Étant donnés u et v dans $\mathcal{L}(E)$, la relation $u - v \geqslant 0$ se note encore $u \geqslant v$ ou $v \leqslant u$; c'est une relation d'ordre sur $\mathcal{L}(E)_{[\mathbf{R}]}$ compatible avec sa structure d'espace vectoriel réel.

#### Proposition 12 {#evt-v-s4-prop-12 .statement}

Soit u un élément hermitien (resp. positif) de $\mathcal{L}(E)$ et soit v une application linéaire continue de E dans un espace hilbertien F. Alors $vuv^*$ est un élément hermitien (resp. positif) de $\mathcal{L}(F)$.

On a en effet $(vuv^*)^* = v^{**}u^*v^* = vuv^*$. D'autre part, si $u \geqslant 0$, on a
$$
\langle y|vuv^*(y) \rangle = \langle v^*(y)|u(v^*(y)) \rangle \geqslant 0
$$
pour tout $y \in F$, d'où $vuv^* \geqslant 0$.

La prop. 12 montre en particulier que $vv^*$ est positif pour tout $v \in \mathcal{L}(E; F)$. Plus particulièrement, un orthoprojecteur p satisfait à $p = p^2 = pp^*$, donc est positif.

#### Remarque 1 {#evt-v-s4-n5-rem-1 .statement}

Pour tout u hermitien dans $\mathcal{L}(E)$, posons $m(u) = \inf_{\|x\|=1} \langle x|u(x) \rangle$,
$M(u) = \sup_{\|x\|=1} \langle x|u(x) \rangle$. Si E n'est pas réduit à 0, $m(u)$ et $M(u)$ sont finis ; de plus,
$M(u)$ est le plus petit nombre réel $\lambda$ tel que $u \leqslant \lambda .1_E$ et $m(u)$ le plus grand nombre réel $\mu$ tel que $u \geqslant \mu .1_E$. On a évidemment $m(-u) = -M(u)$ et $M(-u) = -m(u)$.
Il est clair que l'on a
$$
\sup(|m(u)|, |M(u)|) = \sup_{\|x\|=1} |\langle x|u(x) \rangle|
$$
et la prop. 9 (V, p. 44) entraîne donc (pour $E \neq \{0\}$)
$$
(17) \quad \|u\| = \sup(|m(u)|, |M(u)|) .
$$

\* Pour une autre démonstration de cette formule lorsque K = C, voir la prop. 14 de TS, I, § 6, no 8. \*

#### Remarque 2 {#evt-v-s4-n5-rem-2 .statement}

Soient M et N deux sous-espaces vectoriels fermés de E, et $p_M$ (resp. $p_N$) l’orthoprojecteur de E sur M (resp. N). *On a* $M \subset N$ *si et seulement si* $p_M \leq p_N$. En effet, on a $p_M^* p_M = p_M$ d’où

$$
\|p_M(x)\|^2 = \langle p_M(x)|p_M(x) \rangle = \langle x|p_M^* p_M(x) \rangle = \langle x|p_M(x) \rangle
$$

pour tout $x \in E$. La relation $p_M \leq p_N$ équivaut donc à « $\|p_M(x)\| \leq \|p_N(x)\|$ pour tout $x \in E$ ». Si $M \subset N$, on a $p_M = p_M p_N$ d’où $\|p_M(x)\| \leq \|p_N(x)\|$ puisque $\|p_M\| \leq 1$. Réciproquement, si l’on a $\|p_M(x)\| \leq \|p_N(x)\|$ pour tout $x \in E$, le noyau de $p_M$ contient le noyau de $p_N$, c’est-à-dire que l’on a $M^\circ \supset N^\circ$, d’où finalement $M \subset N$.

#### Proposition 13 {#evt-v-s4-prop-13 .statement}

*Soit* $\mathcal{H}(E)$ *l’ensemble des endomorphismes continus hermitiens de l’espace hilbertien* E. *Soit* $\mathcal{F}$ *une partie non vide, filtrante croissante et majorée de* $\mathcal{H}(E)$.

(i) *L’ensemble* $\mathcal{F}$ *admet une borne supérieure* $u_0$ *dans* $\mathcal{H}(E)$; *on a*

$$
\langle x|u_0(x) \rangle = \sup_{u \in \mathcal{F}} \langle x|u(x) \rangle \quad \text{pour tout } x \in E .
$$

(ii) *Le filtre des sections de* $\mathcal{F}$ *converge vers* $u_0$ *dans l’espace* $\mathcal{L}(E)$ *muni de la topologie de la convergence simple*.

Soit $\Sigma$ le filtre des sections de $\mathcal{F}$; pour tout $u \in \mathcal{H}(E)$, soit $\Phi_u$ la forme hermitienne continue sur E définie par

$$
\Phi_u(x, y) = \langle x|u(y) \rangle .
$$

Posons aussi

$$
\Psi_u(x) = \Phi_u(x, x)
$$

pour $u \in \mathcal{H}(E)$ et $x \in E$. D’après les formules de polarisation (V, p. 2), on a

(19) $$ 4\Phi_u(x, y) = \Psi_u(x + y) - \Psi_u(x - y) $$ si $K = \mathbf{R}$

(20) $$ 4\Phi_u(x, y) = \Psi_u(x + y) - \Psi_u(x - y) - i\Psi_u(x + iy) + i\Psi_u(x - iy) $$ si $K = \mathbf{C}$.

Pour tout $x \in E$, l’application $u \mapsto \Psi_u(x)$ de $\mathcal{H}(E)$ dans $\mathbf{R}$ est croissante et bornée, donc admet une limite selon $\Sigma$. D’après les formules précédentes, la limite

$$
\lim_{u, \Sigma} \Phi_u(x, y) = \Phi(x, y)
$$

existe pour tout couple $(x, y)$ d’éléments de E. Il est clair que $\Phi$ est une forme hermitienne sur E. Si $v_1 \in \mathcal{F}$ et $v_2$ est un majorant de $\mathcal{F}$, les formes hermitiennes $f_1 = \Phi - \Phi_{v_1}$ et $f_2 = \Phi_{v_2} - \Phi$ sont positives ; il existe un nombre réel $M \geq 0$ tel que $f_1(x, x) + f_2(x, x) = \Phi_{v_2 - v_1}(x, x) \leq M \|x\|^2$, d’où

$$
f_1(x, x) \leq M \|x\|^2 , \quad f_2(x, x) \leq M \|x\|^2 \quad (x \in E) ;
$$

par suite, les semi-normes $x \mapsto f_i(x, x)^{1/2}$ sont continues sur E. Comme $f_2 - f_1 = \Phi_{v_2} + \Phi_{v_1} - 2\Phi$, on en déduit que $x \mapsto \Phi(x, x)$ est une fonction continue sur E, et vu les formules (19) et (20) que $\Phi$ est continue sur $E \times E$. Il existe donc (V, p. 16, cor. 2) un élément $u_0$ de $\mathcal{H}(E)$ tel que $\Phi = \Phi_{u_0}$. La formule (18) est évidemment satisfaite, donc $u_0$ est la borne supérieure de $\mathcal{F}$ dans $\mathcal{H}(E)$. Ceci prouve (i).

On a par construction

(21) $\lim_{u,\Sigma} \langle x|(u_0 - u)(x)\rangle = 0$ pour tout $x \in E$.

Soit $v_1 \in \mathcal{F}$; étant donné $u \in \mathcal{F}$ tel que $u \geq v_1$, posons $v = u_0 - u$. Si l’on applique l’inégalité de Cauchy-Schwarz à la forme hermitienne positive $\Phi_v$ sur $E$, on obtient

$$
\|v(x)\|^4 = |\Phi_v(v(x), x)|^2 \leq \Phi_v(v(x), v(x)) \cdot \Phi_v(x, x)
= \langle v(x)|v^2(x)\rangle \langle x|v(x)\rangle \leq \|v\|^3 \|x\|^2 \langle x|v(x)\rangle
\leq \|u_0 - v_1\|^3 \|x\|^2 \langle x|v(x)\rangle,
$$

car on a $\|v\| \leq \|u_0 - v_1\|$ en vertu de V, p. 44, prop. 9. D’après (21), on a donc $\lim_{u,\Sigma} \|(u_0 - u)(x)\| = 0$ pour tout $x \in E$, d’où l’assertion (ii). C.Q.F.D.

La prop. 13 s’applique en particulier au cas d’une suite $(u_n)_{n \in \mathbf{N}}$ croissante et majorée d’éléments de $\mathcal{H}(E)$. Il existe alors un élément $v$ de $\mathcal{H}(E)$ caractérisé par

$$
\langle x|v(x)\rangle = \lim_{n \to \infty} \langle x|u_n(x)\rangle = \sup_{n \in \mathbf{N}} \langle x|u_n(x)\rangle \quad (x \in E),
$$

et l’on a $v(x) = \lim_{n \to \infty} u_n(x)$ pour tout $x \in E$. De plus, $v$ est la borne supérieure de l’ensemble des $u_n$ dans $\mathcal{H}(E)$.

### 6. Trace d’un endomorphisme

Soient $E$ et $F$ deux espaces hilbertiens. Conformément aux conventions de V, p. 40, on note $ba^*$, pour $a$ dans $E$ et $b$ dans $F$, l’application linéaire continue $x \mapsto b \langle a|x\rangle$ de $E$ dans $F$.

#### Lemme 1 {#evt-v-s4-lem-1 .statement}

Il existe un isomorphisme $\theta$ de l’espace vectoriel $F \otimes E'$ sur l’espace $\mathcal{L}_f(E; F)$ des applications linéaires continues de rang fini de $E$ dans $F$, caractérisé par $\theta(b \otimes a^*) = ba^*$ pour $a \in E, b \in F$.

D’après A, II, p. 77, il existe une application linéaire injective $\theta$ de $F \otimes E'$ dans $\mathcal{L}(E; F)$ et une seule qui transforme $b \otimes a'$ en l’application linéaire $x \mapsto ba'(x)$ pour $a' \in E', b \in F$. On a évidemment $\theta(b \otimes a^*) = ba^*$, et l’image de $\theta$ est contenue dans $\mathcal{L}_f(E; F)$. Par ailleurs, soit $u \in \mathcal{L}_f(E; F)$ et soit $(e_1, ..., e_n)$ une base orthonormale de l’image de $u$ dans $F$. Posons $f_i = u^*(e_i)$ pour $1 \leq i \leq n$. Pour tout $x \in E$, on a

$$
u(x) = \sum_{i=1}^n \langle e_i|u(x)\rangle \cdot e_i = \sum_{i=1}^n \langle f_i|x\rangle \cdot e_i,
$$

d’où $u = \sum_{i=1}^n e_i f_i^* = \theta(\sum_{i=1}^n e_i \otimes f_i^*)$. Donc l’image de $\theta$ est égale à $\mathcal{L}_f(E; F)$.

On suppose désormais que l’on a $E = F$, et l’on pose $\mathcal{L}_f(E) = \mathcal{L}_f(E ; E)$. D’après le lemme 1, il existe une forme linéaire $\tau$ sur $\mathcal{L}_f(E)$, et une seule, telle que $\tau(\theta(a \otimes a')) = a'(a)$ pour $a \in E, a' \in E'$; autrement dit, on a

$$
\tau(ba^*) = \langle a|b \rangle \quad \text{pour } a, b \text{ dans } E .
$$

Lorsque $E$ est de dimension finie, on a $\mathcal{L}_f(E) = \mathcal{L}(E)$ et $\tau(u)$ est la trace de l’endomorphisme $u$ de $E$ (A, II, p. 78).

#### Lemme 2 {#evt-v-s4-lem-2 .statement}

*Soit* $(e_i)_{i \in I}$ *une base orthonormale de* $E$. *On a*

$$
\tau(u) = \sum_{i \in I} \langle e_i|u(e_i) \rangle
$$

*pour tout* $u \in \mathcal{L}_f(E)$.

Il suffit d’examiner le cas où $u = ba^*$ avec $a, b$ dans $E$. On a alors

$$
\langle e_i|u(e_i) \rangle = e_i^* b . a^* e_i = \overline{\langle e_i|a \rangle} \langle e_i|b \rangle .
$$

Le lemme 2 résulte alors de la formule (22) et de la formule (3) de V, p. 22.

#### Lemme 3 {#evt-v-s4-lem-3 .statement}

*Soient* $u$ *un endomorphisme continu et positif de* $E$, *et* $\mathcal{F}$ *l’ensemble des orthoprojecteurs de rang fini dans* $E$. *Pour toute base orthonormale* $(e_i)_{i \in I}$ *de* $E$, *on a* (dans $\overline{\mathbf{R}}_+$) *l’égalité*

$$
\sum_{i \in I} \langle e_i|u(e_i) \rangle = \sup_{p \in \mathcal{F}} \tau(pup) .
$$

Pour toute partie finie $J$ de $I$, posons $p_J = \sum_{i \in J} e_i e_i^*$; c’est l’orthoprojecteur de $E$ sur le sous-espace vectoriel engendré par les vecteurs $e_i$ pour $i$ parcourant $J$. On a

$$
p_J up_J = \sum_{i \in J, j \in J} \langle e_i|u(e_j) \rangle e_i e_j^* ,
$$

d’où $\tau(p_J up_J) = \sum_{i \in J} \langle e_i|u(e_i) \rangle$. On a $p_J \in \mathcal{F}$, d’où

$$
\sum_{i \in J} \langle e_i|u(e_i) \rangle \leq \sup_{p \in \mathcal{F}} \tau(pup) ;
$$

on en déduit

$$
\sum_{i \in I} \langle e_i|u(e_i) \rangle = \sup_J \sum_{i \in J} \langle e_i|u(e_i) \rangle \leq \sup_{p \in \mathcal{F}} \tau(pup) .
$$

Soit $v$ un endomorphisme continu et positif de rang fini dans $E$ et soit $p \in \mathcal{F}$. D’après le th. 2 de V, p. 23, il existe une base orthonormale $(f_\alpha)_{\alpha \in A}$ de $E$ et une partie finie $B$ de $A$ telle que $(f_\alpha)_{\alpha \in B}$ soit une base orthonormale de l’image de $p$. On a donc $p = \sum_{\alpha \in B} f_\alpha f_\alpha^*$, d’où comme plus haut la relation $\tau(pvp) = \sum_{\alpha \in B} \langle f_\alpha|v(f_\alpha) \rangle$. On a

$$
\tau(v) = \sum_{\alpha \in A} \langle f_\alpha|v(f_\alpha) \rangle \text{ d’après le lemme 2 (V, p. 48), d’où la formule}
$$

$$
\sum_{\alpha \in B} \langle f_\alpha|v(f_\alpha) \rangle \leq \tau(v) .
$$

Appliquons cette inégalité au cas où $v = p_J u p_J$ et où J est une partie finie de I. On en déduit l’inégalité

$$
\sum_{\alpha \in B} \langle p_J(f_\alpha)|u p_J(f_\alpha) \rangle \leq \sum_{i \in J} \langle e_i|u(e_i) \rangle .
$$

Pour tout $x \in E$, on a $p_J(x) = \sum_{i \in J} \langle e_i|x \rangle e_i$, d’où $x = \lim_j p_J(x)$ selon l’ensemble ordonné filtrant des parties finies J de I. Passant à la limite sur J dans (23), on obtient

$$
\tau(pup) = \sum_{\alpha \in B} \langle f_\alpha|u(f_\alpha) \rangle \leq \sum_{i \in I} \langle e_i|u(e_i) \rangle ,
$$

ce qui achève de prouver le lemme 3.

#### Définition 7 {#evt-v-s4-def-7 .statement}

*Soit u un endomorphisme continu et positif de l’espace hilbertien E. On pose*

$$
\operatorname{Tr}(u) = \sup_{p \in \mathcal{F}} \tau(pup)
$$

(borne supérieure dans $\overline{\mathbf{R}}_+$), *où $\mathcal{F}$ est l’ensemble des orthoprojecteurs de rang fini dans E. On dit que $\operatorname{Tr}(u)$ est la trace de u*.

Soient $p$ l’orthoprojecteur de E sur un sous-espace vectoriel F de dimension finie de E, et soit $(x_1, ..., x_m)$ une base orthonormale de F. On a établi la relation

$$
\tau(pup) = \sum_{i=1}^m \langle x_i|u(x_i) \rangle . \text{ Par suite, on peut définir la trace par la formule}
$$

$$
\operatorname{Tr}(u) = \sup_{x_1, ..., x_m} \sum_{i=1}^m \langle x_i|u(x_i) \rangle ,
$$

où $(x_1, ..., x_m)$ parcourt l’ensemble des suites orthonormales finies de vecteurs de E.

D’après le lemme 3 (V, p. 48), on a

$$
\operatorname{Tr}(u) = \sum_{i \in I} \langle e_i|u(e_i) \rangle
$$

pour toute base orthonormale $(e_i)_{i \in I}$ de E. De là, on déduit

$$
\operatorname{Tr}(u + v) = \operatorname{Tr}(u) + \operatorname{Tr}(v)
$$
$$
\operatorname{Tr}(\lambda u) = \lambda \cdot \operatorname{Tr}(u)
$$

quels que soient les endomorphismes continus et positifs $u$ et $v$ de E et le nombre réel $\lambda \geq 0$ (on fait la convention $0.(+\infty) = 0$ dans (27)). Soit $\varphi$ un isomorphisme de E sur un espace hilbertien F ; comme $\varphi$ transforme toute base orthonormale de E en une base orthonormale de F, on déduit de (25) la relation

$$
\operatorname{Tr}(\varphi u \varphi^{-1}) = \operatorname{Tr}(u) .
$$

Soit $(u_\alpha)_{\alpha \in A}$ une famille non vide, filtrante croissante et majorée d’endomorphismes continus et positifs de E ; posons $u = \sup_\alpha u_\alpha$, d’où $\langle x|u(x) \rangle = \sup_\alpha \langle x|u_\alpha(x) \rangle$ pour tout $x \in E$ (V, p. 46, prop. 13). On a $\operatorname{Tr}(u) = \sup_{J \subset I} \sum_{i \in J} \langle e_i | u(e_i) \rangle$, où J parcourt l’ensemble des parties finies de I, d’où aussitôt

$$
\operatorname{Tr}(u) = \sup_\alpha \operatorname{Tr}(u_\alpha) \quad \text{pour} \quad u = \sup_\alpha u_\alpha .
$$

Soit $p_F$ l’orthoprojecteur de E sur un sous-espace hilbertien F ; il existe une base orthonormale $(e_i)_{i \in I}$ de E et une partie J de I, telles que $(e_i)_{i \in J}$ soit une base orthonormale de F. On a $\operatorname{Tr}(p_F u p_F) = \sum_{i \in J} \langle e_i | u(e_i) \rangle$. Cette formule a deux conséquences : tout d’abord, on a $\operatorname{Tr}(p_F u p_F) \leq \operatorname{Tr}(u)$; puis prenant $u = 1_E$, on obtient

$$
\operatorname{Tr}(p_F) = \begin{cases}
\dim F & \text{si } F \text{ est de dimension finie} \\
+ \infty & \text{sinon} .
\end{cases}
$$

#### Définition 8 {#evt-v-s4-def-8 .statement}

Soit E un espace hilbertien complexe. On note $\mathcal{L}^1(E)$ le sous-espace vectoriel de $\mathcal{L}(E)$ engendré par l’ensemble des endomorphismes continus, positifs et de trace finie de E.

D’après la formule (25) de V, p. 49, la trace s’étend en une forme linéaire sur $\mathcal{L}^1(E)$, notée encore Tr, et satisfaisant à la relation $\operatorname{Tr}(u) = \sum_{i \in I} \langle e_i | u(e_i) \rangle$ pour tout $u$ dans $\mathcal{L}^1(E)$ et toute base orthonormale $(e_i)_{i \in I}$ de E. Pour tout $u \in \mathcal{L}^1(E)$, on a $u^* \in \mathcal{L}^1(E)$ et $\operatorname{Tr}(u^*) = \overline{\operatorname{Tr}(u)}$. La formule (28) de V, p. 49 s’étend au cas où $u$ appartient à $\mathcal{L}^1(E)$. Soit F un sous-espace hilbertien de E ; d’après la formule (30), l’orthoprojecteur $p_F$ appartient à $\mathcal{L}^1(E)$ si et seulement si F est de dimension finie. Quels que soient $a$ et $b$ dans E, on a $4ab^* = \sum_{\varepsilon^4 = 1} \varepsilon(a + \varepsilon b)(a + \varepsilon b)^*$ et $cc^*$ est un opérateur positif de trace finie pour tout $c \in E$; par suite, si $u$ est un endomorphisme continu de rang fini de E, on a $u \in \mathcal{L}^1(E)$ et $\operatorname{Tr}(u) = \tau(u)$.

Soit E un espace hilbertien réel, et soit $E_{(c)}$ son complexifié (V, p. 5). Identifions E à un sous-ensemble de $E_{(c)}$. Alors $\mathcal{L}(E)$ s’identifie au sous-espace vectoriel réel de $\mathcal{L}(E_{(c)})$ formé des applications linéaires continues $u$ de $E_{(c)}$ dans $E_{(c)}$ telles que $u(E) \subset E$. On posera dans ce cas $\mathcal{L}^1(E) = \mathcal{L}(E) \cap \mathcal{L}^1(E_{(c)})$. Pour tout $u \in \mathcal{L}^1(E)$, la trace $\operatorname{Tr}(u)$ est réelle et égale à $\operatorname{Tr}(u^*)$. Les formules (25) et (28) sont encore valables, on a $\mathcal{L}_f(E) \subset \mathcal{L}^1(E)$ et $\operatorname{Tr}(u) = \tau(u)$ pour tout $u \in \mathcal{L}_f(E)$. Enfin, un sous-espace vectoriel fermé F de E est de dimension finie si et seulement si $p_F$ appartient à $\mathcal{L}^1(E)$.

\* Remarque 1. — Nous définirons ultérieurement la notion d’application nucléaire d’un espace de Banach E dans un espace de Banach F. On montrera alors que $\mathcal{L}^1(E)$ se compose des applications nucléaires de E dans E, que E soit un espace hilbertien réel ou complexe. \*

#### Proposition 14 {#evt-v-s4-prop-14 .statement}

Soient $E_1, \ldots, E_n$ des espaces hilbertiens, $E = E_1 \hat{\otimes}_2 \cdots \hat{\otimes}_2 E_n$, et $u_i$ un endomorphisme continu de $E_i$ pour $1 \leq i \leq n$. Si $u_1, \ldots, u_n$ sont positifs, il en est de même de $u = u_1 \hat{\otimes}_2 \cdots \hat{\otimes}_2 u_n$ et l’on a

$$
\operatorname{Tr}(u) = \prod_{i=1}^n \operatorname{Tr}(u_i) .
$$

Si l’on a $u_i \in \mathcal{L}^1(E_i)$ pour $1 \leq i \leq n$, on a $u \in \mathcal{L}^1(E)$ et la formule (31) est encore valable dans ce cas.

Procédant par récurrence sur $n$, on se ramène aussitôt au cas $n = 2$.

Pour $i = 1, 2$, définissons une forme sesquilinéaire $\Phi_i$ sur $E_i$ par la formule $\Phi_i(x, y) = \langle x|u_i(y) \rangle$ pour $x, y$ dans $E_i$. Si $u_1$ et $u_2$ sont positifs, les formes $\Phi_1$ et $\Phi_2$ sont hermitiennes et positives. D’après la prop. 1 de V, p. 25, il existe une forme hermitienne positive $\Phi$ sur l’espace vectoriel $E_1 \otimes E_2$ telle que

$$
\Phi(x_1 \otimes x_2, y_1 \otimes y_2) = \Phi_1(x_1, y_1) \cdot \Phi_2(x_2, y_2)
$$

pour $x_1, y_1$ dans $E_1$ et $x_2, y_2$ dans $E_2$. On vérifie aussitôt que l’on a la relation $\Phi(z, t) = \langle z|u(t) \rangle$ pour $z$ et $t$ dans $E_1 \otimes E_2$. Comme $\Phi$ est positive, on a donc $\langle z|u(z) \rangle \geq 0$ pour tout $z$ dans $E_1 \otimes E_2$. Comme $u$ est continu et que $E_1 \otimes E_2$ est dense dans l’espace hilbertien $E = E_1 \hat{\otimes}_2 E_2$, on conclut que $u$ est un endomorphisme continu et positif de $E$.

Soient $(e_i)_{i \in I}$ une base orthonormale de $E_1$ et $(f_j)_{j \in J}$ une base orthonormale de $E_2$; alors la famille $(e_i \otimes f_j)_{i \in I, j \in J}$ est une base orthonormale de $E$ et l’on a donc

$$
\begin{align*}
\operatorname{Tr}(u) &= \sum_{i \in I} \sum_{j \in J} \langle e_i \otimes f_j|u(e_i \otimes f_j) \rangle \\
&= \sum_{i \in I} \sum_{j \in J} \langle e_i|u_1(e_i) \rangle \cdot \langle f_j|u_2(f_j) \rangle \\
&= \operatorname{Tr}(u_1) \cdot \operatorname{Tr}(u_2) .
\end{align*}
$$

En particulier, si $u_1$ et $u_2$ sont des endomorphismes positifs de trace finie, il en est de même de $u$. Par linéarité, on déduit de là que $u$ appartient à $\mathcal{L}^1(E)$ lorsque $K = \mathbf{C}$ et que $u_i$ appartient à $\mathcal{L}^1(E_i)$ pour $i = 1, 2$; la formule (31) s’étend à ce cas par linéarité. Enfin, le cas où $K = \mathbf{R}$ et $u_i \in \mathcal{L}^1(E_i)$ se ramène au cas complexe par extension des scalaires.

#### Remarque 2 {#evt-v-s4-n6-rem-2 .statement}

Soit $E$ un espace hilbertien, somme hilbertienne d’une famille $(E_i)_{i \in I}$ de sous-espaces hilbertiens. Soit $u$ un élément de $\mathcal{L}(E)$ tel que $u(E_i) \subset E_i$ pour tout $i \in I$; soit $u_i$ l’élément de $\mathcal{L}(E_i)$ qui coïncide avec $u$ sur $E_i$. On a alors $\operatorname{Tr}(u) = \sum_{i \in I} \operatorname{Tr}(u_i)$ lorsque $u$ est positif, ou appartient à $\mathcal{L}^1(E)$ : cette relation se déduit de la formule (25) de V, p. 49 appliquée à une base orthonormale de $E$ réunion de bases orthonormales de chacun des $E_i$.

### 7. Applications de Hilbert-Schmidt

#### Définition 9 {#evt-v-s4-def-9 .statement}

Soient $E$ et $F$ deux espaces hilbertiens. On appelle application de Hilbert-Schmidt de $E$ dans $F$ toute application linéaire continue $u : E \to F$ telle que la trace de l’endomorphisme positif $u^*u$ de $E$ soit finie. L’ensemble des applications de Hilbert-Schmidt de $E$ dans $F$ se note $\mathcal{L}^2(E ; F)$.

Lorsque $E = F$, on écrit $\mathcal{L}^2(E)$ pour $\mathcal{L}^2(E ; E)$.

Pour tout $u \in \mathcal{L}(E; F)$, on pose $\|u\|_2 = \operatorname{Tr}(u^*u)^{1/2}$, de sorte que $u$ appartient à $\mathcal{L}^2(E; F)$ si et seulement si $\|u\|_2$ est fini. D’après la définition de la trace, on a

$$
\|u\|_2^2 = \sup_{x_1, \ldots, x_m} \sum_{i=1}^m \|u(x_i)\|^2
$$

où $(x_1, \ldots, x_m)$ parcourt l’ensemble des suites orthonormales finies dans E. Comme on peut prendre en particulier $m = 1$ dans la formule (32), on a

$$
\|u\| \leq \|u\|_2 \quad (u \in \mathcal{L}(E; F)) .
$$

Soient $(e_i)_{i \in I}$ une base orthonormale de E et $(f_j)_{j \in J}$ une base orthonormale de F. D’après la formule (25) de V, p. 49 et la relation de Parseval (V, p. 22), on a

$$
\|u\|_2^2 = \sum_{i \in I} \|u(e_i)\|^2 = \sum_{i,j} |\langle f_j | u(e_i) \rangle|^2 .
$$

Comme on a $|\langle f_j | u(e_i) \rangle| = |\langle e_i | u^*(f_j) \rangle|$, la formule (34) entraîne

$$
\|u^*\|_2 = \|u\|_2 ;
$$

par suite, l’adjoint d’une application de Hilbert-Schmidt est une application de Hilbert-Schmidt. Soient $E_1, F_1$ des espaces hilbertiens et $v : E_1 \to E, w : F \to F_1$ des applications linéaires continues. De (32), on déduit aussitôt

$$
\|wu\|_2 \leq \|w\| \cdot \|u\|_2 .
$$

D’après (35), (36) et la relation $uv = (v^*u^*)^*$, on obtient

$$
\|uv\|_2 \leq \|u\|_2 \|v\| .
$$

En particulier, si $u$ appartient à $\mathcal{L}^2(E; F)$, alors $wuw$ appartient à $\mathcal{L}^2(E_1; F_1)$.

#### Théorème 1 {#evt-v-s4-thm-1 .statement}

*Soient E et F deux espaces hilbertiens.*

(i) *L’ensemble $\mathcal{L}^2(E; F)$ est un sous-espace vectoriel de $\mathcal{L}(E; F)$ et $u \mapsto \|u\|_2$ est une norme hilbertienne (V, p. 6) sur $\mathcal{L}^2(E; F)$.*

(ii) *L’isomorphisme $\theta$ de $F \otimes E'$ sur $\mathcal{L}_f(E; F)$ caractérisé par $\theta(y \otimes x^*) = yx^*$ se prolonge en un isomorphisme $\hat{\theta}$ de $F \otimes_2 E'$ sur $\mathcal{L}^2(E; F)$. En particulier, $\mathcal{L}_f(E; F)$ est dense dans $\mathcal{L}^2(E; F)$.*

Soit $(e_i)_{i \in I}$ (resp. $(f_j)_{j \in J}$) une base orthonormale de E (resp. F). Pour tout $u \in \mathcal{L}(E; F)$, soit $\Lambda(u)$ la matrice de $u$ par rapport aux bases orthonormales choisies pour E et F (V, p. 22). On note $\|a\|_2$ la norme d’un élément $a$ de l’espace hilbertien $\ell^2(J \times I)$. D’après la formule (34), $\Lambda$ est une application de $\mathcal{L}^2(E; F)$ dans $\ell^2(J \times I)$ telle que $\|\Lambda(u)\|_2 = \|u\|_2$; il est clair que $\Lambda$ est injective. Pour prouver (i), il suffit donc de montrer que $\Lambda$ est surjective. Soit $a = (a_{ji})$ un élément de $\ell^2(J \times I)$; d’après l’inégalité de Cauchy-Schwarz, on a

$$
|\sum_{j,i} \overline{\eta_j} a_{ji} \xi_i|^2 \leq \sum_{j,i} |a_{ji}|^2 \sum_{j,i} |\overline{\eta_j} \xi_i|^2 = \|a\|_2^2 \|\xi\|^2 \|\eta\|^2
$$

quels que soient $\xi = (\xi_i)$ dans $\ell^2(I)$ et $\eta = (\eta_j)$ dans $\ell^2(J)$. Il existe donc une forme sesquilinéaire continue $\Phi$ sur $F \times E$ telle que $\Phi(y, x) = \sum_{j,i} \overline{\eta}_j a_{ji} \xi_i$ pour $x = \sum_i \xi_i e_i$ dans $E$ et $y = \sum_j \eta_j f_j$ dans $F$. Soit $u \in \mathcal{L}(E; F)$ tel que $\Phi(y, x) = \langle y|u(x) \rangle$ (V, p. 16, cor. 2). On a

$$
a_{ji} = \Phi(f_j, e_i) = \langle f_j|u(e_i) \rangle \quad \text{pour} \quad i \in I, j \in J,
$$

d'où $a = \Lambda(u)$.

Comme $\Lambda$ est un isomorphisme d'espaces hilbertiens de $\mathcal{L}^2(E; F)$ sur $\ell^2(J \times I)$ et que $(f_j \otimes e_i^*)$ est une base orthonormale de $F \hat{\otimes}_2 E'$, il existe un isomorphisme $\hat{\theta}$ de $F \hat{\otimes}_2 E'$ sur $\mathcal{L}^2(E; F)$ tel que

$$
\langle f_j|\hat{\theta}(t)\,e_i \rangle = \langle f_j \otimes e_i^*|t \rangle
$$

quels que soient $i \in I, j \in J$ et $t \in F \hat{\otimes}_2 E'$. En particulier pour $t = y \otimes x^*$, on trouve

$$
\langle f_j|\hat{\theta}(y \otimes x^*)\,e_i \rangle = \langle f_j \otimes e_i^*|y \otimes x^* \rangle = \langle f_j|y \rangle \langle x|e_i \rangle = \langle f_j|yx^*e_i \rangle
$$

d'où $\hat{\theta}(y \otimes x^*) = yx^*$. Ceci prouve (ii). C.Q.F.D.

#### Exemple 1 {#evt-v-s4-n7-exa-1 .statement}

Soient I et J deux ensembles. D'après la démonstration ci-dessus, pour qu'une application $u$ de $\ell^2(I)$ dans $\ell^2(J)$ soit de Hilbert-Schmidt, il faut et il suffit qu'il existe une matrice $(a_{ji})$ dans $\ell^2(J \times I)$ telle que l'on ait $u(\xi)_j = \sum_{i \in I} a_{ji} \xi_i$ pour tout $\xi = (\xi_i)$ dans $\ell^2(I)$.

#### Exemple 2 {#evt-v-s4-n7-exa-2 .statement}

\* Soient X et Y deux espaces topologiques séparés, munis respectivement de mesures positives $\mu$ et $\nu$. On peut montrer que les applications de Hilbert-Schmidt de $\mathcal{L}^2(X)$ dans $\mathcal{L}^2(Y)$ correspondent bijectivement aux classes de fonctions de carré intégrable dans $Y \times X$ : à la classe de la fonction $N \in \mathcal{L}^2(Y \times X, \nu \otimes \mu)$ correspond l'application $u_N$ donnée par

$$
(u_N f)(y) = \int_X N(y, x) f(x) \, d\mu(x)
$$

pour $\nu$-presque tout $y \in Y$ et $f \in \mathcal{L}^2(X, \mu)$. On a

$$
\|u_N\|^2_2 = \int_X \int_Y |N(y, x)|^2 \, d\mu(x) \, d\nu(y) \cdot *
$$

#### Remarque 1 {#evt-v-s4-n7-rem-1 .statement}

Supposons $K = \mathbf{C}$. Soient $u$ et $v$ dans $\mathcal{L}^2(E; F)$. On a la relation $4u^*v = \sum_{\varepsilon^4 = 1} \overline{\varepsilon}(u + \varepsilon v)^*(u + \varepsilon v)$, donc $u^*v$ appartient à $\mathcal{L}^1(E)$. Le produit scalaire dans l'espace hilbertien $\mathcal{L}^2(E; F)$ est donné par

$$
\langle u|v \rangle = \operatorname{Tr}(u^*v)
$$

car cette formule définit une forme hermitienne sur $\mathcal{L}^2(E; F)$ et l'on a $\langle u|u \rangle = \|u\|^2_2$.

Si $u \in \mathcal{L}^2(E ; F)$ et $v \in \mathcal{L}^2(F ; E)$, alors $vu$ appartient à $\mathcal{L}^1(E)$ et $uv$ à $\mathcal{L}^1(F)$ d’après ce qui précède ; en outre on a

$$
\text{Tr}(uv) = \text{Tr}(vu) .
$$

Par linéarité et continuité, il suffit en effet de vérifier cette formule lorsque $u = y_1 x_1^*$ et $v = x_2 y_2^*$ (avec $x_1, x_2$ dans $E$, $y_1, y_2$ dans $F$) ; mais alors $uv$ est l’application $y \mapsto y_1 \langle x_1 | x_2 \rangle \langle y_2 | y \rangle$ et $vu$ l’application $x \mapsto x_2 \langle y_2 | y_1 \rangle \langle x_1 | x \rangle$, et (42) résulte de la formule (22) de V, p. 48.

Par suite, si $u_1, u_2$ sont deux éléments de $\mathcal{L}^2(E ; F)$, on a, dans l’espace hilbertien $\mathcal{L}^2(F ; E)$,

$$
\langle u_1^* | u_2^* \rangle = \text{Tr}(u_1 u_2^*) = \text{Tr}(u_2^* u_1) = \langle u_2 | u_1 \rangle = \overline{\langle u_1 | u_2 \rangle} ;
$$

autrement dit, $u \mapsto u^*$ est un isomorphisme de l’espace hilbertien $\mathcal{L}^2(E ; F)$ sur le conjugué (V, p. 6) de l’espace hilbertien $\mathcal{L}^2(F ; E)$. Si on identifie ce conjugué au dual de $\mathcal{L}^2(F ; E)$ (V, p. 15), on voit que $\mathcal{L}^2(E ; F)$ s’identifie au dual de $\mathcal{L}^2(F ; E)$, la forme bilinéaire canonique $(v, u) \mapsto \langle v, u \rangle$ s’identifiant à $(v, u) \mapsto \text{Tr}(vu)$.

#### Remarque 2 {#evt-v-s4-n7-rem-2 .statement}

Supposons $K = \mathbf{R}$. On laisse au lecteur le soin de vérifier que les formules (40) et (41) sont encore valables, et de montrer que $\mathcal{L}^2(E ; F)$ s’identifie au dual de $\mathcal{L}^2(F ; E)$ au moyen de la forme bilinéaire $(u, v) \mapsto \text{Tr}(uv)$.

### 8. Diagonalisation des applications de Hilbert-Schmidt

#### Théorème 2 {#evt-v-s4-thm-2 .statement}

Soient $E$ et $F$ deux espaces hilbertiens et $u$ une application de Hilbert-Schmidt de $E$ dans $F$. Il existe une base orthonormale $(e_i)_{i \in I}$ de $E$ transformée par $u$ en une famille orthogonale dans $F$.

On note $B$ la boule unité (fermée) de $E$, qu’on munit de la topologie affaiblie ; c’est un espace compact (V, p. 17). On pose $Q(x) = \|u(x)\|^2$ pour tout $x \in B$. Enfin, on note $P$ l’ensemble des vecteurs $x$ de $E$ satisfaisant à la propriété suivante :

(H) Pour tout $y \in E$ orthogonal à $x$, l’élément $u(y)$ de $F$ est orthogonal à $u(x)$.

#### Lemme 4 {#evt-v-s4-lem-4 .statement}

La fonction $Q : B \to \mathbf{R}$ est continue.

Soit $(f_j)_{j \in J}$ une base orthonormale de $F$. Posons $\lambda_j = \|u^*(f_j)\|^2$ pour tout $j \in J$. Comme $u$ appartient à $\mathcal{L}^2(E ; F)$, on a $u^* \in \mathcal{L}^2(F ; E)$, d’où $\sum_j \lambda_j < + \infty$. Par ailleurs, on a

$$
Q(x) = \|u(x)\|^2 = \sum_j |\langle u^*(f_j) | x \rangle|^2
$$

d’après la relation de Parseval (V, p. 22) et la définition de l’adjoint (V, p. 38). Pour tout $x \in B$, on a $|\langle u^*(f_j) | x \rangle|^2 \leq \lambda_j$ d’après l’inégalité de Cauchy-Schwarz ; par suite, la convergence de la somme dans la formule (43) est uniforme sur $B$, d’où le lemme 4 (TG, X, p. 9).

#### Lemme 5 {#evt-v-s4-lem-5 .statement}

Soit $E_1$ un sous-espace vectoriel fermé de $E$, stable par $u^*u$. Si $E_1 \neq \{0\}$, il existe dans $E_1 \cap P$ un vecteur de norme 1.

Comme B est faiblement compacte, il en est de même du sous-espace faiblement fermé $B \cap E_1$ de B. Il existe donc (TG, IV, p. 27) un point $x_0$ de $B \cap E_1$ tel que $Q(x_0) \geq Q(x)$ pour tout $x \in B \cap E_1$. Si $Q(x_0) = 0$, on a $Q(x) = 0$ d'où $u(x) = 0$ pour tout $x \in B \cap E_1$. On a alors $E_1 \subset P$, d'où le lemme 5 dans ce cas.

Supposons que l'on ait $Q(x_0) > 0$, d'où $x_0 \neq 0$. Comme le vecteur $\|x_0\|^{-1} \cdot x_0$ appartient à $B \cap E_1$, on a

$$
Q(x_0) \geq Q(\|x_0\|^{-1} \cdot x_0) = Q(x_0)/\|x_0\|^2
$$

d'où $\|x_0\| = 1$. Prouvons que $x_0$ appartient à $P$; soit donc $y \in E$ orthogonal à $x_0$. Il s'agit de prouver que $u(y)$ est orthogonal à $u(x_0)$. Or $y$ est somme d'un vecteur de $E_1$ et d'un vecteur orthogonal à $E_1$, tous deux orthogonaux à $x_0$ (car on a $x_0 \in E_1$) ; il suffit donc de considérer les deux cas suivants :

a) $y$ est orthogonal à $E_1$ : comme $E_1$ est stable par $u^*u$, on a $u^*u(x_0) \in E_1$, d'où $0 = \langle y|u^*u(x_0)\rangle = \langle u(y)|u(x_0)\rangle$.

b) $y$ appartient à $E_1$ : pour tout $t \in \mathbf{R}$, le vecteur $x(t) = (x_0 + ty)/\|x_0 + ty\|$ appartient à $B \cap E_1$. On a $Q(x(t)) = f(t)/g(t)$ avec

$$
f(t) = \|u(x_0)\|^2 + 2t \Re \langle u(x_0)|u(y)\rangle + t^2 \|u(y)\|^2 \\
g(t) = 1 + t^2 \|y\|^2 .
$$

Vu la définition de $x_0$, on a $Q(x(0)) \geq Q(x(t))$ pour tout $t$ réel, donc $\frac{d}{dt} Q(x(t))$ s'annule pour $t = 0$. Or on a $f(0) = \|u(x_0)\|^2, g(0) = 1, f'(0) = 2 \Re \langle u(x_0)|u(y)\rangle, g'(0) = 0$. Comme on a

$$
\frac{d}{dt} Q(x(t)) = \frac{f'(t) g(t) - f(t) g'(t)}{g(t)^2} ,
$$

on en conclut $f'(0) = 0$, c'est-à-dire $\Re \langle u(x_0)|u(y)\rangle = 0$. Lorsque $K = \mathbf{R}$, $u(x_0)$ est donc orthogonal à $u(y)$; lorsque $K = \mathbf{C}$, le vecteur $iy$ appartient à $E_1$ et est orthogonal à $x_0$, d'où $\Im \langle u(x_0)|u(y)\rangle = - \Re \langle u(x_0)|u(iy)\rangle = 0$, et finalement $u(x_0)$ est orthogonal à $u(y)$. Ceci prouve le lemme 5.

Prouvons le th. 2. Par application du th. 1 de E, III, p. 35, on voit comme dans V, p. 23, qu'il existe un ensemble S maximal parmi les parties orthonormales de E contenues dans P. Soit $E_1$ l'ensemble des vecteurs de E orthogonaux à S. Soit $y \in E_1$; si $x \in S$, les vecteurs $x$ et $y$ sont orthogonaux, et comme on a $S \subset P$, on en déduit que $u(x)$ et $u(y)$ sont orthogonaux ; on a donc

$$
\langle x|u^*u(y)\rangle = \langle u(x)|u(y)\rangle = 0
$$

et $u^*u(y)$ est orthogonal à S. Donc $E_1$ est stable par $u^*u$. Si l'on avait $E_1 \neq \{0\}$, il existerait dans $E_1 \cap P$ un vecteur $x$ de norme 1 (lemme 5) et $S \cup \{x\}$ serait une partie orthonormale de E, contenue dans P. Ceci contredit le caractère maximal de S. On a donc $E_1 = \{0\}$ et S est une base orthonormale de E.

#### Corollaire 1 {#evt-v-s4-lem-5-cor-1 .statement}

Soit v un endomorphisme continu, positif et de trace finie de l’espace hilbertien E. Il existe une base orthonormale $(e_i)_{i\in I}$ de E et une famille sommable de nombres réels positifs $(\lambda_i)_{i\in I}$ telles que $v(e_i) = \lambda_i e_i$ pour tout $i \in I$.

Posons $\Phi(x, y) = \langle x|v(y)\rangle$ pour $x, y$ dans E. Alors $\Phi$ est une forme hermitienne positive sur E. Il existe donc (V, p. 8, corollaire) un espace hilbertien F et une application linéaire continue $u$ de E dans F tels que $\Phi(x, y) = \langle u(x)|u(y)\rangle$ pour $x, y$ dans E. Autrement dit, on a $v = u^*u$. En vertu de la déf. 9 (V, p. 51), $u$ est une application de Hilbert-Schmidt de E dans F. D’après le th. 2, il existe une base orthonormale $(e_i)_{i\in I}$ de E telle que les vecteurs $u(e_i)$ soient deux à deux orthogonaux. Soit $i \in I$; pour tout $j \neq i$ dans I, on a donc
$$
\langle e_j|v(e_i)\rangle = \langle u(e_j)|u(e_i)\rangle = 0
$$
donc $v(e_i)$ est proportionnel à $e_i$, de la forme $\lambda_i e_i$. On a $\lambda_i = \langle e_i|v(e_i)\rangle$, donc
$$
\lambda_i \geqslant 0 \quad \text{et} \quad \sum_{i\in I} \lambda_i = \operatorname{Tr}(v) < +\infty .
$$

#### Corollaire 2 {#evt-v-s4-lem-5-cor-2 .statement}

Soit E un espace hilbertien. On a $\mathcal{L}^1(E) \subset \mathcal{L}^2(E)$.

Le cas réel se ramenant au cas complexe par extension des scalaires, nous pouvons supposer que l’on a $\mathbf{K} = \mathbf{C}$.

Comme $\mathcal{L}^2(E)$ est un sous-espace vectoriel de $\mathcal{L}(E)$, il suffit de prouver que tout endomorphisme continu et positif de trace finie $v$ de E appartient à $\mathcal{L}^2(E)$. Avec les notations du cor. 1, on a
$$
\sum_{i\in I} \|v(e_i)\|^2 = \sum_{i\in I} \lambda_i^2 \leq (\sum_i \lambda_i)^2 < +\infty .
$$

#### Corollaire 3 {#evt-v-s4-lem-5-cor-3 .statement}

Soit v un endomorphisme continu, positif et de trace finie de l’espace hilbertien E. Il existe un endomorphisme de Hilbert-Schmidt positif w de E tel que $v = w^2$ et que $v$ commute à $w$.

Avec les notations du cor. 1, il suffit de considérer l’endomorphisme $w$ qui transforme le vecteur $\sum_{i\in I} \xi_i e_i$ en le vecteur $\sum_i \lambda_i^{1/2} \xi_i e_i$.

#### Remarque {#evt-v-s4-n8-rem-1 .statement}

Avec les notations du th. 2, soit J l’ensemble des $i \in I$ tels que $u(e_i) \neq 0$. Pour tout $i \in J$, posons $\hat{\lambda}_i = \|u(e_i)\|$ et $f_i = \hat{\lambda}_i^{-1} u(e_i)$. Alors $(e_i)_{i\in J}$ (resp. $(f_i)_{i\in J}$) est une base orthonormale du sous-espace initial (resp. final) de $u$, on a $u(e_i) = \lambda_i f_i$ pour tout $i \in J$ et $\sum_{i\in J} \lambda_i^2 = \|u\|_2^2$ est fini.

### 9. Trace d’une forme quadratique par rapport à une autre

Dans ce numéro, on note E un espace vectoriel réel et Q, H deux formes quadratiques positives sur E. Il existe deux formes bilinéaires symétriques $(x, y) \mapsto \langle x|y\rangle_Q$ et $(x, y) \mapsto \langle x|y\rangle_H$ sur $E \times E$, caractérisées par
$$
Q(x) = \langle x|x\rangle_Q , \quad H(x) = \langle x|x\rangle_H
$$
pour tout $x \in E$.

On appelle trace de Q par rapport à H, et l’on note Tr(Q/H) le nombre réel positif, fini ou non, défini comme suit :

a) S’il existe $x \in E$ avec $H(x) = 0$ et $Q(x) \neq 0$, on pose $\operatorname{Tr}(Q/H) = +\infty$.

b) Dans le cas contraire, $\operatorname{Tr}(Q/H)$ est la borne supérieure de l’ensemble des nombres de la forme $\sum_{i=1}^{m} Q(x_i)$, où $(x_1, \ldots, x_m)$ parcourt l’ensemble des suites finies d’éléments de E telles que $\langle x_i | x_j \rangle_H = \delta_{ij}$ (symbole de Kronecker).

#### Remarque 1 {#evt-v-s4-n9-rem-1 .statement}

Pour tout sous-espace F de E, notons $Q_F$ la restriction de Q à F et $H_F$ celle de H. On a $\operatorname{Tr}(Q_F/H_F) \leq \operatorname{Tr}(Q/H)$ et $\operatorname{Tr}(Q/H)$ est la borne supérieure de l’ensemble des nombres $\operatorname{Tr}(Q_F/H_F)$ où F parcourt l’ensemble des sous-espaces vectoriels de dimension finie de E.

#### Remarque 2 {#evt-v-s4-n9-rem-2 .statement}

Soient $E_1$ un espace vectoriel réel, $Q_1$ et $H_1$ deux formes quadratiques positives sur $E_1$ et $\pi : E \to E_1$ une application linéaire surjective. Si $Q = Q_1 \circ \pi$ et $H = H_1 \circ \pi$, on a $\operatorname{Tr}(Q/H) = \operatorname{Tr}(Q_1/H_1)$.

#### Proposition 15 {#evt-v-s4-prop-15 .statement}

*On suppose qu’il existe une structure d’espace hilbertien réel sur E telle que* $H(x) = \|x\|^2$ *pour tout* $x \in E$. *Pour que* $\operatorname{Tr}(Q/H)$ *soit fini, il faut et il suffit qu’il existe un endomorphisme continu et positif u de trace finie de E, tel que l’on ait* $Q(x) = \langle x | u(x) \rangle$ *pour tout* $x \in E$; *cet endomorphisme u est unique*, et l’on a

$$
\operatorname{Tr}(u) = \operatorname{Tr}(Q/H) = \sum_{i \in I} Q(e_i)
$$

pour toute base orthonormale $(e_i)_{i \in I}$ de E.

Supposons que $\operatorname{Tr}(Q/H)$ soit fini. Pour tout $x \in E$ de norme 1, on a $H(x) = 1$, d’où $Q(x) \leq \operatorname{Tr}(Q/H)$. On a donc $Q(x) \leq \operatorname{Tr}(Q/H) \cdot \|x\|^2$ pour tout $x \in E$, d’où

$$
|\langle x | y \rangle_Q| \leq Q(x)^{1/2} Q(y)^{1/2} \leq \operatorname{Tr}(Q|H) \cdot \|x\| \cdot \|y\|
$$

d’après l’inégalité de Cauchy-Schwarz. Par suite, la forme bilinéaire $(x, y) \mapsto \langle x | y \rangle_Q$ sur $E \times E$ est continue. Il existe donc (V, p. 16, cor. 2) une application $u \in \mathcal{L}(E)$ telle que $\langle x | y \rangle_Q = \langle x | u(y) \rangle$. On a $\langle x | y \rangle_Q = \langle y | x \rangle_Q$ pour $x, y$ dans $E$, donc $u$ est hermitien ; on a $\langle x | u(x) \rangle = Q(x) \geq 0$, donc $u$ est positif.

Réciproquement, soit $u$ un endomorphisme continu et positif de $E$ tel que $Q(x) = \langle x | u(x) \rangle$ pour tout $x \in E$. On a

$$
\langle x | u(y) \rangle = \frac{1}{2}(Q(x + y) - Q(x) - Q(y)) = \langle x | y \rangle_Q,
$$

d’où l’unicité de $u$. D’après la formule (24 bis) (V, p. 49), on a

$$
\operatorname{Tr}(u) = \sup_{x_1, \ldots, x_m} \sum_{i=1}^m \langle x_i | u(x_i) \rangle = \sup_{x_1, \ldots, x_m} \sum_{i=1}^m Q(x_i),
$$

où $(x_1, \ldots, x_m)$ parcourt l’ensemble des suites orthonormales finies d’éléments de E. On a donc $\operatorname{Tr}(u) = \operatorname{Tr}(Q/H)$ d’après la définition de $\operatorname{Tr}(Q/H)$. Enfin, pour toute base orthonormale $(e_i)_{i \in I}$ de E, on a $\operatorname{Tr}(u) = \sum_{i \in I} \langle e_i | u(e_i) \rangle$ d’après la formule (25) de V, p. 49, d’où $\operatorname{Tr}(u) = \sum_{i \in I} Q(e_i)$.

C.Q.F.D.

#### Remarque 3 {#evt-v-s4-n9-rem-3 .statement}

Soient E et F deux espaces hilbertiens et v une application linéaire, non nécessairement continue, de E dans F. Posons H(x) = \|x\|^2 et Q(x) = \|v(x)\|^2 pour tout x \in E. Il résulte de la prop. 15 que v est de Hilbert-Schmidt si et seulement si Tr(Q/H) est fini, et l’on a alors Tr(Q/H) = \|v\|_2^2.

#### Remarque 4 {#evt-v-s4-n9-rem-4 .statement}

Supposons E de dimension finie. Lorsque la forme quadratique H est inversible, la prop. 15 s’applique. Soit (e_1, ..., e_n) une base de E. Posons q_{ij} = \langle e_i | e_j \rangle_Q et h_{ij} = \langle e_i | e_j \rangle_H et introduisons les matrices q = (q_{ij}) et h = (h_{ij}). Soit u l’endomorphisme de E tel que Q(x) = \langle x | u(x) \rangle_H pour tout x \in E. On a

$$
\langle x | y \rangle_Q = \langle x | u(y) \rangle_H \quad (x, y \in E),
$$

et par suite la matrice de u par rapport à la base (e_1, ..., e_n) de E est égale à h^{-1} q. D’après la prop. 15, on a donc

(45)
$$
\operatorname{Tr}(Q/H) = \operatorname{Tr}(h^{-1} q) = \operatorname{Tr}(qh^{-1}).
$$

Si la base (e_1, ..., e_n) est orthonormale pour H, alors h est la matrice unité d’ordre n, et l’on a

$$
\operatorname{Tr}(Q/H) = \operatorname{Tr}(q) = \sum_{i=1}^n Q(e_i);
$$

on retrouve donc la formule (44) dans ce cas.

Supposons maintenant que la forme quadratique H ne soit pas inversible. Soit N le noyau de H, et soit \pi l’application canonique de E sur E/N. Il existe une forme quadratique inversible H_1 sur E/N telle que H = H_1 \circ \pi. Soit (e_1, ..., e_m) une suite d’éléments de E telle que la suite (\pi(e_1), ..., \pi(e_m)) soit une base de E/N, orthonormale pour H_1. Soit (e_{m+1}, ..., e_n) une base de N. Alors (e_1, ..., e_n) est une base de E, et l’on a

(46)
$$
H(\xi_1 e_1 + \cdots + \xi_n e_n) = \xi_1^2 + \cdots + \xi_m^2
$$

quels que soient les nombres réels \xi_1, ..., \xi_n.

Supposons que pour tout x \in E, la relation H(x) = 0 entraîne Q(x) = 0 ; autrement dit, supposons qu’il existe une forme quadratique Q_1 sur E/N telle que Q = Q_1 \circ \pi. D’après la remarque 2 et la prop. 15, on a

(47)
$$
\operatorname{Tr}(Q/H) = Q(e_1) + \cdots + Q(e_m).
$$

Exercises

## EXERCICES {#evt-v-s4-exercises}

See the [exercises for § 4](exercises/s4/).
