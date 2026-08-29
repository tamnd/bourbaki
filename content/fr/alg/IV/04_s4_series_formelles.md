---
book: alg
book_title: Algebra
chapter: IV
chapter_title: Polynômes et fractions rationnelles
section: 4
section_title: SÉRIES FORMELLES
lang: fr
source: alg-iv-vii-fr
book_pages: A IV.23-A IV.39, A IV.85-A IV.87
pdf_pages: 0030-0046, 0092-0094
extraction: ocr
subsections:
    - "no": 1
      title: Définition des séries formelles. Ordre
      page: 23
      pdf_page: 30
    - "no": 2
      title: Topologie sur l’ensemble des séries formelles. Familles sommables
      page: 24
      pdf_page: 31
    - "no": 3
      title: Substitutions
      page: 26
      pdf_page: 33
    - "no": 4
      title: Séries formelles inversibles
      page: 28
      pdf_page: 35
    - "no": 5
      title: Formule de Taylor pour les séries formelles
      page: 29
      pdf_page: 36
    - "no": 6
      title: Dérivations de l’algèbre des séries formelles
      page: 30
      pdf_page: 37
    - "no": 7
      title: Résolution des équations dans un anneau de séries formelles
      page: 33
      pdf_page: 40
    - "no": 8
      title: Séries formelles sur un anneau intègre
      page: 36
      pdf_page: 43
    - "no": 9
      title: Corps des fractions de l’anneau des séries formelles en une indéterminée sur un corps
      page: 36
      pdf_page: 43
    - "no": 10
      title: Exponentielle et logarithme
      page: 37
      pdf_page: 44
statements: 24
exercises: 8
content_sha256: 0c46b750a29c2ad670a2b596182d9340c14975df566b95df8921355b0f8baac5
---

## § 4. SÉRIES FORMELLES

### 1. Définition des séries formelles. Ordre

Soit I un ensemble. Rappelons (III, p. 27 et 28) que l’algèbre large du monoïde $\mathbf{N}^{(I)}$ sur A s’appelle l’algèbre des séries formelles par rapport aux indéterminées $X_i$ ($i \in I$) (ou en les indéterminées $X_i$) à coefficients dans A. Elle se note $A[[X_i]]_{i \in I}$ ou $A[[\{X_i\}_{i \in I}]]$, ou encore $A[[X]]$ en notant $X$ la famille $(X_i)_{i \in I}$ : dans ce paragraphe, nous utiliserons surtout la notation $A[[I]]$. Il est parfois commode de désigner l’image canonique dans $A[[I]]$ de l’élément $i$ de I par un symbole différent de $X_i$, par exemple $Y_i, Z_i, T_i, \ldots$; les conventions utilisées dans ce cas sont analogues à celles des polynômes (IV, p. 1). L’algèbre $A[[I]]$ se désigne alors par $A[[Y_i]]_{i \in I}$, ou $A[[Y]]$, etc.

Lorsque I est un ensemble fini à $p$ éléments, on dit encore que $A[[I]]$ est une algèbre de séries formelles en $p$ indéterminées. Ces algèbres sont toutes isomorphes pour $p$ fixé. Une algèbre de séries formelles à 1, 2, ... indéterminées peut ainsi se noter $A[[X]], A[[U, V]], \ldots$, l’ensemble d’indices I étant non spécifié.

Une série formelle $u$ s’écrit conventionnellement $u = \sum_{v \in \mathbf{N}^{(I)}} \alpha_v X^v$ (cf. IV, p. 1).

Les $\alpha_v$ sont les coefficients de $u$; une infinité d’entre eux peuvent être $\neq 0$. Les $\alpha_v X^v$ s’appellent les termes de $u$; pour que $u$ soit un polynôme, il faut et il suffit que $u$ ne possède qu’un nombre fini de termes $\neq 0$. Les termes $\alpha_v X^v$ tels que $|v| = p$ s’appellent les termes de degré total $p$. La série formelle $u_p = \sum_{|v|=p} \alpha_v X^v$ s’appelle la composante homogène de degré $p$ de $u$ (c’est un polynôme lorsque I est fini); $u_0$ s’identifie à un élément de A dit encore terme constant de $u$. On dit que $u$ est homogène de degré $p$ si $u = u_p$. Si $u, v \in A[[I]]$ et $w = uv$, on a

$$
w_p = \sum_{q+r=p} u_q v_r
$$

pour tout entier $p \geqslant 0$.

Rappelons (III, p. 29) que l’ordre $\omega(u)$ d’une série formelle $u \neq 0$ est le plus petit des entiers $p$ tels que $u_p \neq 0$. On convient d’adjoindre à $\mathbf{Z}$ un élément noté $\infty$, et de prolonger la relation d’ordre et l’addition de $\mathbf{Z}$ à $\mathbf{Z} \cup \{ \infty \}$ par les conventions

$$
n < \infty, \quad \infty + \infty = \infty, \quad \infty + n = n + \infty = \infty
$$

pour tout $n \in \mathbf{Z}$. On pose alors $\omega(0) = \infty$. Avec ces conventions, on a les relations

$$
\begin{align*}
\omega(u + v) &\geq \inf(\omega(u), \omega(v)) \\
\omega(u + v) &= \inf(\omega(u), \omega(v)) \quad \text{si} \quad \omega(u) \neq \omega(v) \\
\omega(uv) &\geq \omega(u) + \omega(v)
\end{align*}
$$

quelles que soient les séries formelles $u$ et $v$ dans $A[[I]]$.

Rappelons (III, p. 29) que pour toute partie $J$ de $I$, on identifie $A[[I]]$ à $A[[I - J]] [[J]]$, ce qui permet de définir l’ordre $\omega_J(u)$ d’une série formelle par rapport aux $X_j$ ($j \in J$), la composante homogène de $u$ par rapport aux $X_j$ ($j \in J$), etc.

Soit $\varphi$ un homomorphisme de $A$ dans un anneau $B$. On prolonge $\varphi$ en un homomorphisme $\overline{\varphi}$ de $A[[I]]$ dans $B[[I]]$ en faisant correspondre à toute série formelle $u = \sum_v \alpha_v X^v$ la série formelle $\sum_v \varphi(\alpha_v) X^v$; on dit que cette dernière est obtenue en appliquant $\varphi$ aux coefficients de la série formelle $u$. On écrit parfois $^\varphi u$ pour $\overline{\varphi}(u)$.

En particulier, si $A$ est un sous-anneau de $B$, et si $\varphi$ est l’injection canonique de $A$ dans $B$, l’homomorphisme $\overline{\varphi}$ de $A[[I]]$ dans $B[[I]]$ est injectif ; nous identifierons en général $A[[I]]$ par $\overline{\varphi}$ à un sous-anneau de $B[[I]]$.

### 2. Topologie sur l’ensemble des séries formelles. Familles sommables

Par définition, l’ensemble $A[[I]]$ n’est autre que l’ensemble produit $A^{N^{(I)}}$. Sauf mention expresse du contraire, on munira $A$ de la topologie discrète et $A[[I]]$ de la topologie produit (TG, I, p. 24) qu’on appelle la topologie canonique. Muni de l’addition et de la topologie discrète, $A$ est un groupe topologique séparé et complet ; par suite, pour l’addition, $A[[I]]$ est un groupe topologique séparé et complet (TG, III, p. 17 et 21 et TG, II, p. 17). De plus, l’algèbre $A[(X_i)_{i \in I}]$ des polynômes est dense dans $A[[I]]$ (TG, III, p. 17, prop. 25), et l’on peut donc considérer $A[[I]]$ comme le complété de $A[(X_i)_{i \in I}]$.

Pour tout $\beta \in N^{(I)}$, soit $S_\beta$ l’ensemble des multiindices $v$ tels que $v \leq \beta$, et soit $a_\beta$ l’ensemble des séries formelles $u = \sum_v \alpha_v X^v$ telles que $\alpha_v = 0$ pour $v \in S_\beta$. Il est clair que $S_\beta$ est une partie finie de $N^{(I)}$, et que toute partie finie de $N^{(I)}$ est contenue dans un ensemble de la forme $S_\beta$. Par suite, la famille $(a_\beta)_{\beta \in N^{(I)}}$ est un système fondamental de voisinages de 0 dans $A[[I]]$. Les ensembles $a_\beta$ sont des idéaux de $A[[I]]$, donc (TG, III, p. 49) $A[[I]]$ est un anneau topologique.

#### Lemme 1 {#alg-iv-s4-lem-1 .statement}

Soient $L$ un ensemble infini et $(u_\lambda)_{\lambda \in L}$ une famille d’éléments de $A[[I]]$. Posons $u_\lambda = \sum_v \alpha_{\lambda,v} X^v$ pour $\lambda \in L$. Les conditions suivantes sont équivalentes :

(i) La famille $(u_\lambda)_{\lambda \in L}$ est sommable (TG, III, p. 37) dans $A[[I]]$.
(ii) On a $\lim u_\lambda = 0$ selon le filtre des complémentaires des parties finies de $L$.
(iii) Pour tout $v \in N^{(I)}$, on a $\alpha_{\lambda,v} = 0$ sauf pour un nombre fini d’indices $\lambda \in L$.

Si ces conditions sont remplies, la série $u = \sum_{\lambda \in L} u_\lambda$ est égale à $\sum_v \alpha_v X^v$ avec $\alpha_v = \sum_{\lambda \in L} \alpha_{\lambda,v}$ pour tout $v \in \mathbf{N}^{(l)}$.

L’équivalence de (i) et (ii) résulte du cor. 2 de TG, III, p. 39.
L’équivalence de (ii) et (iii) résulte des propriétés des limites dans un espace produit (TG, I, p. 51, cor. 1).
La dernière assertion résulte de la prop. 4 de TG, III, p. 41.

Donnons quelques exemples de familles sommables.
a) Soit $u \in \mathbf{A}[[\mathbf{I}]]$ et soit $\alpha_v$ le coefficient de $X^v$ dans $u$. La famille $(\alpha_v X^v)_{v \in \mathbf{N}^{(l)}}$ est alors sommable de somme $u$ (ce qui justifie l’écriture $u = \sum_v \alpha_v X^v$).

b) Soit $u \in \mathbf{A}[[\mathbf{I}]]$; pour tout entier $p \geq 0$, soit $u_p$ la composante homogène de degré $p$ de $u$. Alors la famille $(u_p)_{p \in \mathbf{N}}$ est sommable et l’on a $u = \sum_{p \geq 0} u_p$.

c) Soit $(u_\lambda)_{\lambda \in L}$ une famille d’éléments de $\mathbf{A}[[\mathbf{I}]]$. On suppose que pour tout entier $n \geq 0$ l’ensemble des $\lambda \in L$ tels que $\omega(u_\lambda) < n$ est fini. Alors la famille $(u_\lambda)_{\lambda \in L}$ est sommable.

#### Remarque {#alg-iv-s4-n2-rem-1 .statement}

Supposons I fini. Pour tout entier $n \geq 0$, soit $b_n$ l’ensemble des séries formelles $u \in \mathbf{A}[[\mathbf{I}]]$ telles que $\omega(u) \geq n$. La suite $(b_n)_{n \geq 0}$ est un système fondamental de voisinages de 0 dans $\mathbf{A}[[\mathbf{I}]]$. Par suite, une famille d’éléments $u_\lambda$ de $\mathbf{A}[[\mathbf{I}]]$ ($\lambda \in L$) est sommable si et seulement si, pour tout $n \in \mathbf{N}$, l’ensemble des $\lambda \in L$ tels que $\omega(u_\lambda) < n$ est fini.

#### Proposition 1 {#alg-iv-s4-prop-1 .statement}

Soient $(u_\lambda)_{\lambda \in L}$ et $(v_\mu)_{\mu \in M}$ deux familles sommables d’éléments de $\mathbf{A}[[\mathbf{I}]]$. Alors la famille $(u_\lambda v_\mu)_{(\lambda, \mu) \in L \times M}$ est sommable et l’on a
$$
\sum_{(\lambda, \mu) \in L \times M} u_\lambda v_\mu = (\sum_{\lambda \in L} u_\lambda) (\sum_{\mu \in M} v_\mu).
$$
Soit $(\alpha_{\lambda,v})_{v \in \mathbf{N}^{(l)}}$ (resp. $(\beta_{\mu,v})_{v \in \mathbf{N}^{(l)}}$) la famille des coefficients de $u_\lambda$ (resp. $v_\mu$). Pour tout $v \in \mathbf{N}^{(l)}$, il n’existe qu’un nombre fini de couples $(v_1, v_2) \in \mathbf{N}^{(l)} \times \mathbf{N}^{(l)}$ tels que $v_1 + v_2 = v$, donc il n’existe qu’un nombre fini de couples $(\lambda, \mu) \in L \times M$ tels que le coefficient de $X^v$ dans $u_\lambda v_\mu$ soit $\neq 0$. Par suite, la famille $(u_\lambda v_\mu)_{(\lambda, \mu) \in L \times M}$ est sommable. La formule (2) résulte alors de l’associativité de la somme (TG, III, p. 40, formule (2)).

Dans $\mathbf{A}[[\mathbf{I}]]$, le produit est une loi de composition associative et commutative. On peut donc parler de famille multipliable d’éléments de $\mathbf{A}[[\mathbf{I}]]$, et de produit d’une famille multipliable (TG, III, p. 37, remarque 3).

#### Proposition 2 {#alg-iv-s4-prop-2 .statement}

Soit $(u_\lambda)_{\lambda \in L}$ une famille sommable d’éléments de $\mathbf{A}[[\mathbf{I}]]$.
(i) La famille $(1 + u_\lambda)_{\lambda \in L}$ est multipliable.
(ii) Soit $\mathfrak{F}$ l’ensemble des parties finies de $L$. Pour $M \in \mathfrak{F}$, posons $u_M = \prod_{\lambda \in M} u_\lambda$.

Alors la famille $(u_M)_{M \in \mathcal{F}}$ est sommable, et l’on a

$$
\sum_{M \in \mathcal{F}} u_M = \prod_{\lambda \in L} (1 + u_\lambda).
$$

Définissons les idéaux $a_\beta$ comme au début de ce numéro. Soit $\beta \in \mathbf{N}^{(1)}$. Il existe une partie finie $L_0$ de $L$ telle que l’on ait $u_\lambda \in a_\beta$ pour $\lambda \notin L_0$. Alors pour tout $M \in \mathcal{F}$ tel que $M \notin L_0$, on a $u_M \in a_\beta$. On en déduit que la famille $(u_M)_{M \in \mathcal{F}}$ est sommable. D’autre part, si $M_0$ est une partie finie de $L$, on a

$$
\sum_{M \subset M_0} u_M = \prod_{\lambda \in M_0} (1 + u_\lambda).
$$

Suivant l’ensemble ordonné filtrant $\mathcal{F}$, le membre de gauche a pour limite $\sum_{M \in \mathcal{F}} u_M$. Donc le membre de droite a pour limite $\sum_{M \in \mathcal{F}} u_M$, ce qui prouve à la fois (i) et (ii).

#### Proposition 3 {#alg-iv-s4-prop-3 .statement}

*Soient $u = \sum_v \alpha_v X^v \in A[[I]]$, et $m$ un entier $> 0$. Pour tout $n \in \mathbf{N}$, soit $(\alpha_{v,n})_{v \in \mathbf{N}^{(1)}}$ la famille des coefficients de $u^n$. Supposons que $\alpha_0^m = 0$. On a $\alpha_{v,n} = 0$ pour $n \geq |v| + m$.
Soient $v \in \mathbf{N}^{(1)}$ et $n \in \mathbf{N}$. On a*

$$
\alpha_{v,n} = \sum_{v(1) + \cdots + v(n) = v} \alpha_{v(1)} \cdots \alpha_{v(n)}.
$$

Si $n \geq |v| + m$ et $v(1) + \cdots + v(n) = v$, on a $|v(1)| + \cdots + |v(n)| \leq n - m$. On a donc $v(r) = 0$ et par suite $\alpha_{v(r)} = \alpha_0$ pour au moins $m$ valeurs distinctes de $r$; on en déduit que $\alpha_{v(1)} \cdots \alpha_{v(n)} = 0$, d’où la proposition.

#### Corollaire {#alg-iv-s4-n2-cor-1 .statement}

*Soit $u \in A[[I]]$. Pour que l’on ait $\lim_{n \to \infty} u^n = 0$, il faut et il suffit que le terme constant de $u$ soit nilpotent.*
Soit $\alpha_0$ le terme constant de $u$. Le terme constant de $u^n$ est $\alpha_0^n$, donc la condition énoncée est nécessaire. Elle est suffisante d’après la prop. 3.

### 3. Substitutions

Soit E une A-algèbre. On dit qu’une topologie sur E est linéaire si elle est invariante par translation, et s’il existe un système fondamental de voisinages de 0 formé d’idéaux de E (TG, III, p. 5). La topologie de E est alors compatible avec sa structure de A-algèbre (A étant muni de la topologie discrète). Une A-algèbre munie d’une topologie linéaire s’appelle une A-algèbre linéairement topologisée.

#### Proposition 4 {#alg-iv-s4-prop-4 .statement}

*Soient I un ensemble, E une A-algèbre associative, commutative et unifière, linéairement topologisée, séparée et complète.*
(i) *Soit $\varphi$ un homomorphisme continu de $A[[I]]$ dans E et soit $x_i = \varphi(X_i)$. Alors :*
a) *pour tout $i \in I$, $x_i^n$ tend vers 0 quand $n$ tend vers $+\infty$;*

b) si $I$ est infini, $x_i$ tend vers 0 suivant le filtre des complémentaires des parties finies de $I$.

(ii) Soit $x = (x_i)_{i \in I}$ une famille d’éléments de $E$ satisfaisant aux conditions a) et b) de (i). Il existe alors un homomorphisme unifère continu $\varphi$ et un seul de $A[[I]]$ dans $E$ tel que $\varphi(X_i) = x_i$ pour tout $i \in I$.

Pour tout $i \in I$, $X_i^n$ tend évidemment vers 0 dans $A[[I]]$ quand $n$ tend vers $+ \infty$; d’autre part, si $I$ est infini, $X_i$ tend vers 0 suivant le filtre des complémentaires des parties finies de $I$. Cela prouve (i).

Soit $(x_i)_{i \in I}$ une famille d’éléments de $E$ satisfaisant aux conditions a) et b) de (i). Soit $\psi$ l’homomorphisme $u \mapsto u((x_i)_{i \in I})$ de $A[(X_i)_{i \in I}]$ dans $E$. soit $V$ un voisinage de 0 dans $E$ qui soit un idéal de $E$. Il existe d’après b) une partie finie $J$ de $I$ telle que $x_i \in V$ pour tout $i \in I - J$. Puis il existe d’après a) un entier $n \geqslant 0$ tel que l’on ait $x_i^n \in V$ pour tout $i \in J$. Soit $\beta$ l’élément de $\mathbf{N}^{(1)}$ tel que $\beta_i = n - 1$ pour $i \in J$ et $\beta_i = 0$ pour $i \in I - J$. Définissons l’idéal $a_\beta$ de $A[[I]]$ comme au début du no 2 (IV, p. 24). Alors

$$
u \in A[(X_i)_{i \in I}] \cap a_\beta \Rightarrow \psi(u) \in V .
$$

Cela prouve que $\psi$ est continu si l’on munit $A[(X_i)_{i \in I}]$ de la topologie induite par celle de $A[[I]]$. Comme $E$ est séparée et complète, $\psi$ se prolonge en un homomorphisme unifère continu $\varphi$ de $A[[I]]$ dans $E$. On a $\varphi(X_i) = \psi(X_i) = x_i$ pour tout $i \in I$. Enfin, soit $\varphi'$ un homomorphisme unifère continu de $A[[I]]$ dans $E$ tel que $\varphi'(X_i) = x_i$. On a $\varphi'(u) = \varphi(u)$ pour tout $u \in A[(X_i)_{i \in I}]$, donc $\varphi' = \varphi$ puisque $A[(X_i)_{i \in I}]$ est dense dans $A[[I]]$.

Conservons les notations précédentes. Si $u \in A[[I]]$, l’image de $u$ par $\varphi$ se note $u(x)$ ou $u((x_i)_{i \in I})$ (ou encore $u(x_1, ..., x_n)$ si $I = \{ 1, 2, ..., n \}$) et s’appelle l’élément de $E$ déduit par substitution des $x_i$ aux $X_i$ dans $u$, ou la valeur de $u$ pour les valeurs $x_i$ des $X_i$, ou encore la valeur de $u$ pour $X_i = x_i$. En particulier, on a $u = u((X_i)_{i \in I})$.

Soit $E'$ une $A$-algèbre associative, commutative et unifère, linéairement topologisée, séparée et complète. Soit $\lambda$ un homomorphisme unifère continu de $E$ dans $E'$. Soit $(x_i)_{i \in I}$ une famille d’éléments de $E$ satisfaisant aux conditions a) et b) de la prop. 4 (IV, p. 26). La famille $(\lambda(x_i))_{i \in I}$ satisfait auxdites conditions a) et b). On a, pour tout $u \in A[[I]]$,

$$
\lambda(u((x_i)_{i \in I})) = u((\lambda(x_i))_{i \in I}) ,
$$

car l’application $u \mapsto \lambda(u((x_i)_{i \in I}))$ est un homomorphisme unifère continu de $A[[I]]$ dans $E'$ qui transforme $X_i$ en $\lambda(x_i)$ pour tout $i \in I$.

Si $J$ et $K$ sont deux ensembles, nous noterons $A_{J,K}$ l’ensemble des familles $(g_j)_{j \in J}$ satisfaisant aux conditions suivantes :

(i) pour tout $j \in J$, $g_j$ est un élément de $A[[K]]$ dont le terme constant est nilpotent ;
(ii) si $J$ est infini, $g_j$ tend vers 0 selon le filtre des complémentaires des parties finies de $J$.

On notera que si J est fini, toute famille $(g_j)_{j\in J}$ de séries formelles sans terme constant dans $A[[K]]$ appartient à $A_{J,K}$.

Soit $(g_j)_{j\in J}$ dans $A_{J,K}$. D’après le cor. de la prop. 3 (IV, p. 26), on a $\lim_{n\to\infty} g_j^n = 0$ pour tout $j \in J$. Soit $f \in A[[J]]$; on peut donc substituer $g_j$ à la variable d’indice $j$ dans $f$ et l’on obtient une série formelle $f((g_j)_{j\in J})$ appartenant à $A[[K]]$. De plus, l’application $f \mapsto f((g_j)_{j\in J})$ est un homomorphisme continu de $A$-algèbres de $A[[J]]$ dans $A[[K]]$.

En particulier, si $J = \{1, ..., p\}$ et $f \in A[[X_1, ..., X_p]]$, on peut substituer à chaque $X_j$ une série formelle $g_j \in A[[K]]$ sans terme constant; le résultat de la substitution se note $f(g_1, ..., g_p)$.

Soit $x = (x_k)_{k\in K}$ une famille d’éléments de E satisfaisant aux conditions a) et b) de la prop. 4 (IV, p. 26). Appliquons (3) en prenant pour $\lambda$ l’homomorphisme $u \mapsto u(x)$ de $A[[K]]$ dans $E$; on obtient

$$
f((g_j)_{j\in J})(x) = f((g_j(x))_{j\in J}) .
$$

Soient $f = (f_i)_{i\in I} \in (A[[J]])^I$ et $g = (g_j)_{j\in J} \in A_{J,K}$. On note $f(g)$ ou $f \circ g$ l’élément $(f_i((g_j)_{j\in J}))_{i\in I}$ de $(A[[K]])^I$. Si $f \in A_{I,J}$, on a $f \circ g \in A_{I,K}$ puisque l’application $f \mapsto f((g_j)_{j\in J})$ de $A[[J]]$ dans $A[[K]]$ est continue.

Soient $f \in (A[[J]])^I$, $g \in A_{J,K}$, $h \in A_{K,L}$. Alors $g \circ h \in A_{J,L}$ et, d’après (4), on a

$$
(f \circ g) \circ h = f \circ (g \circ h) .
$$

### 4. Séries formelles inversibles

#### Proposition 5 {#alg-iv-s4-prop-5 .statement}

Dans l’anneau $A[[T]]$ des séries formelles en une indéterminée, le polynôme $1 - T$ est inversible, et l’on a $(1 - T)^{-1} = \sum_{n=0}^{\infty} T^n$.

En effet,

$$(1 - T)(\sum_{n=0}^{\infty} T^n) = \sum_{n=0}^{\infty} T^n - \sum_{n=0}^{\infty} T^{n+1} = 1 .$$

#### Proposition 6 {#alg-iv-s4-prop-6 .statement}

Soit $u \in A[[I]]$. Pour que $u$ soit inversible dans $A[[I]]$, il faut et il suffit que son terme constant soit inversible dans $A$.

Supposons qu’il existe $v \in A[[I]]$ tel que $uv = 1$. Soient $\alpha, \beta$ les termes constants de $u$ et $v$. On a $\alpha \beta = 1$, donc $\alpha$ est inversible.

Réciproquement, supposons que le terme constant $\alpha$ de $u$ soit inversible. Il existe donc une série formelle $t \in A[[I]]$ telle que $u = \alpha(1 - t)$ et $\omega(t) > 0$. Or, il existe un homomorphisme d’anneaux $\varphi : A[[T]] \to A[[I]]$ tel que $\varphi(T) = t$, et $1 - T$ est inversible dans $A[[T]]$ (prop. 5). Par suite, $1 - t$ est inversible dans $A[[I]]$ et il en est donc de même de $u$.

#### Remarque {#alg-iv-s4-n4-rem-1 .statement}

Soit $\mathcal{M}$ l’ensemble des séries formelles de terme constant égal à 1. D’après la prop. 6, $\mathcal{M}$ est un groupe commutatif pour la multiplication ; le groupe multiplicatif de $A[[I]]$ est produit direct de $\mathcal{M}$ et du groupe multiplicatif de $A$. Nous munirons $\mathcal{M}$ de la topologie induite par celle de $A[[I]]$. Pour tout $\beta \in \mathbf{N}^{(l)}$, on a défini dans IV, p. 24, l’idéal $a_\beta$ de $A[[I]]$ ; alors $1 + a_\beta$ est un sous-groupe de $\mathcal{M}$, et la famille $(1 + a_\beta)$ est un système fondamental de voisinages de 1 dans $\mathcal{M}$. Comme la multiplication dans $\mathcal{M}$ est continue, on voit que $\mathcal{M}$ est un groupe topologique (TG, III, p. 5) ; autrement dit, *l’application* $f \mapsto f^{-1}$ *est continue dans* $\mathcal{M}$.

Soient $K$ un corps commutatif et $\mathfrak{D}$ le sous-anneau du corps des fractions rationnelles $K((X_i)_{i \in I})$ formé des fractions rationnelles dans lesquelles l’élément 0 de $K^1$ est substituable. Soit $f \in \mathfrak{D}$. On a $f = \frac{u}{v}$ où $u$ et $v$ sont des polynômes tels que le terme constant de $v$ soit $\neq 0$. Donc $v$ est inversible dans $K[[I]]$. On vérifie aussitôt que l’élément $uv^{-1}$ de $K[[I]]$ ne dépend que de $f$ ; on dit que la série formelle $uv^{-1}$ est le *développement à l’origine de la fraction rationnelle* $\frac{u}{v}$. L’application $f \mapsto uv^{-1}$ est un homomorphisme injectif de $\mathfrak{D}$ dans $K[[I]]$ ; on identifie souvent $\mathfrak{D}$ à son image par cette application.

### 5. Formule de Taylor pour les séries formelles

Soient $X = (X_i)_{i \in I}$ et $Y = (Y_i)_{i \in I}$ deux familles d’indéterminées relatives au même ensemble d’indices $I$. On note $X + Y$ la famille $(X_i + Y_i)_{i \in I}$ de séries formelles dans $A[[X, Y]]$. Il est clair qu’on peut substituer $X_i + Y_i$ à $X_i$ dans une série formelle $u \in A[[X]]$, le résultat étant noté $u(X + Y)$. Pour tout $v \in \mathbf{N}^{(l)}$, on note $\Delta^v u$ le coefficient de $Y^v$ dans la série formelle $u(X + Y)$ considérée comme appartenant à $A[[X]] [[Y]]$ (III, p. 29). Autrement dit, on a

$$
u(X + Y) = \sum_v \Delta^v u(X) \cdot Y^v \quad (u \in A[[X]]) .
$$

En substituant $(0, X)$ à $(X, Y)$, on obtient

$$
u(X) = \sum_v \Delta^v u(0) \cdot X^v ;
$$

autrement dit, le terme constant de $\Delta^v u$ est le coefficient de $X^v$ dans $u$. L’application $u \mapsto u(X + Y)$ de $A[[X]]$ dans $A[[X, Y]]$ étant continue, les applications $u \mapsto \Delta^v u$ de $A[[X]]$ dans lui-même sont continues.

Comme dans le cas des polynômes (IV, p. 7), on démontre les formules

$$
\Delta^\sigma(uv) = \sum_{v + \rho = \sigma} \Delta^v(u) \ \Delta^\rho(v) ,
$$
$$
\Delta^\rho \Delta^\sigma u = \frac{(\rho + \sigma)!}{\rho! \ \sigma!} \Delta^{\rho + \sigma} u .
$$

La formule du binôme (I, p. 94, cor. 2) donne la valeur suivante pour $\Delta^\nu u$ lorsque $u = \sum_\lambda \alpha_\lambda X^\lambda$

$$
\Delta^\nu u = \sum_\lambda \alpha_{\lambda + \nu} \frac{(\lambda + \nu)!}{\lambda! \nu!} X^\lambda .
$$

Considérons en particulier le cas $\nu = \varepsilon_i$, c’est-à-dire $\nu_i = 1, \nu_j = 0$ pour $j \neq i$. On pose $D_i u = \Delta^{\varepsilon_i} u$; autrement dit, $D_i u$ est le coefficient de $Y_i$ dans $u(X + Y)$. D’après (10), on a donc

$$
D_i u = \sum_\lambda (\lambda_i + 1) \alpha_{\lambda + \varepsilon_i} X^\lambda ;
$$

en particulier, on a $D_i(X_i) = 1$ et $D_i(X_j) = 0$ pour $j \neq i$. La formule (8) montre que $D_i$ est une dérivation de $A[[X]]$, et de (9) on déduit la relation

$$
D^\nu u = \nu! \Delta^\nu u
$$

comme dans le cas des polynômes (IV, p. 8) (on a posé $D^\nu = \prod_{i \in I} D_i^{\nu_i}$ pour $\nu = (\nu_i)_{i \in I}$ dans $\mathbf{N}^{(I)}$). Lorsque $A$ est une $\mathbf{Q}$-algèbre, les formules (6), (7) et (12) entraînent les « formules de Taylor » :

$$
u(X + Y) = \sum_\nu \frac{1}{\nu!} D^\nu u(X) \cdot Y^\nu ,
$$
$$
u(X) = \sum_\nu \frac{1}{\nu!} D^\nu u(0) \cdot X^\nu .
$$

#### Remarque 1 {#alg-iv-s4-n5-rem-1 .statement}

On dit souvent que $D_i u$ est la *dérivée partielle de u par rapport à $X_i$* ; on emploie aussi les notations $D_{X_i} u, \frac{\partial u}{\partial X_i}$ et $u'_{X_i}$. Pour une seule indéterminée $X$, l’unique dérivée partielle $Du$ (notée aussi $\frac{du}{dX}$ ou $u'$) est appelée la *dérivée de u*.

#### Remarque 2 {#alg-iv-s4-n5-rem-2 .statement}

La formule (9) montre que les endomorphismes $\Delta^p$ du $A$-module $A[[X]]$ commutent deux à deux. Il en est donc de même des endomorphismes $D_i$.

#### Remarque 3 {#alg-iv-s4-n5-rem-3 .statement}

Si $u \in A[(X_i)_{i \in I}]$ est un polynôme, les polynômes $\Delta^p u$ et $D_i u$ définis dans IV, p. 6 et 7, coïncident avec les séries formelles désignées ici par le même symbole.

### 6. Dérivations de l’algèbre des séries formelles

Soient I un ensemble, E une $A$-algèbre associative, commutative et unifière, linéairement topologisée, séparée et complète, et $x = (x_i)_{i \in I}$ une famille d’éléments de E satisfaisant aux conditions a) et b) de la prop. 4 (IV, p. 26). Soit $\varphi$ l’homomorphisme continu $u \mapsto u(x)$ de $A[[I]]$ dans E ; il munit E d’une structure de $A[[I]]$-module. D’après III, p. 118, une $A$-dérivation D de $A[[I]]$ dans le $A[[I]]$-module E est donc une application A-linéaire $D : A[[I]] \to E$ satisfaisant à la relation
$$
(15) \quad D(uv) = u(x).D(v) + D(u).v(x)
$$
pour $u, v$ dans $A[[I]]$.

#### Proposition 7 {#alg-iv-s4-prop-7 .statement}

*Soit* $(y_i)_{i \in I}$ *une famille d’éléments de* $E$. *Lorsque* $I$ *est infini, on suppose que* $y_i$ *tend vers* $0$ *selon le filtre des complémentaires des parties finies de* $I$. *Il existe alors une unique* $A$-*dérivation continue* $D$ *de* $A[[I]]$ *dans le* $A[[I]]$*-module* $E$, *telle que* $D(X_i) = y_i$ *pour tout* $i \in I$. *On a*
$$
(16) \quad D(u) = \sum_{i \in I} (D_iu)(x).y_i \quad (u \in A[[I]]) .
$$

Comme $0$ admet dans $E$ un système fondamental de voisinages formé d’idéaux, la famille $((D_iu)(x).y_i)_{i \in I}$ est sommable dans $E$ pour tout $u \in A[[I]]$ (TG, III, p. 39, cor. 2). La formule (16) définit donc une application $A$-linéaire $D : A[[I]] \to E$. On laisse au lecteur le soin de vérifier que $D$ est une dérivation continue.

Soit $D_1$ une $A$-dérivation continue de $A[[I]]$ dans $E$, telle que $D_1(X_i) = y_i$ pour tout $i \in I$. Le noyau de la dérivation continue $D - D_1$ est une sous-algèbre fermée $B$ de $A[[I]]$ contenant 1 et les indéterminées $X_i$. Comme l’algèbre des polynômes $A[(X_i)_{i \in I}]$ est dense dans $A[[I]]$, on a $B = A[[I]]$, d’où $D_1 = D$.

#### Corollaire 1 {#alg-iv-s4-prop-7-cor-1 .statement}

*Soit* $\Delta$ *une dérivation continue de la* $A$*-algèbre* $E$. *Pour toute série formelle* $u \in A[[I]]$, *la famille* $((D_iu)(x).\Delta x_i)_{i \in I}$ *est sommable et l’on a*
$$
(17) \quad \Delta(u(x)) = \sum_{i \in I} (D_iu)(x).\Delta x_i .
$$

Cela résulte de la prop. 7 car l’application $u \mapsto \Delta(u(x))$ est une dérivation continue de $A[[I]]$ dans le $A[[I]]$*-module* $E$.

#### Corollaire 2 {#alg-iv-s4-prop-7-cor-2 .statement}

*La dérivation* $D_i$ *est l’unique dérivation continue de la* $A$*-algèbre* $A[[I]]$ *telle que*
$$
(18) \quad D_i(X_i) = 1 , \quad D_i(X_j) = 0 \quad \text{pour } j \neq i .
$$

Cela résulte du corollaire 1.

#### Corollaire 3 {#alg-iv-s4-prop-7-cor-3 .statement}

*Soient* $f \in A[[X_1, ..., X_p]]$ *et* $g_i \in A[[Y_1, ..., Y_q]]$ *pour* $1 \leq i \leq p$. *Supposons que, pour* $1 \leq i \leq p$, *le terme constant de* $g_i$ *soit nul*. *Posons* $h = f(g_1, ..., g_p)$. *Alors, pour* $1 \leq j \leq q$, *on a*
$$
(19) \quad \frac{\partial h}{\partial Y_j} = \sum_{i=1}^p D_i f(g_1, ..., g_p) \cdot \frac{\partial g_i}{\partial Y_j} .
$$

C’est le cas particulier $E = A[[Y_1, ..., Y_q]]$, $x_i = g_i$ et $\Delta = \partial / \partial Y_j$ du cor. 1.

#### Proposition 8 {#alg-iv-s4-prop-8 .statement}

Soit $X = (X_i)_{i \in I}$ une famille finie d’indéterminées.

(i) Toute dérivation de l’anneau de séries formelles $A[[X]]$ est continue.

(ii) Toute dérivation de l’anneau de polynômes $A[X]$ dans l’anneau de séries formelles $A[[X]]$ se prolonge de manière unique en une dérivation de l’anneau $A[[X]]$.

(iii) La famille $(D_i)_{i \in I}$ est une base du $A[[X]]$-module des $A$-dérivations de $A[[X]]$ dans lui-même.

Soit $b_n$ l’ensemble des séries formelles d’ordre $\geq n$. Il est clair que $b_n$ est un idéal de l’anneau $A[[X]]$, engendré par les monômes de degré $n$. Par suite $b_n$ se compose des sommes finies de produits de $n$ séries formelles sans terme constant ; si $D$ est une dérivation de $A[[X]]$, on a

$$
D(f_1 \ldots f_n) = \sum_{i=1}^n f_1 \ldots f_{i-1} D(f_i) f_{i+1} \ldots f_n,
$$

d’où immédiatement $Db_n \subset b_{n-1}$ pour $n \geq 1$. Comme la suite $(b_n)_{n \geq 0}$ est un système fondamental de voisinages de 0 dans $A[[X]]$ (IV, p. 25, remarque), $D$ est continue, d’où (i).

Soit $\Delta$ une dérivation de $A[X]$ dans $A[[X]]$. Raisonnant comme précédemment, on montre que $\Delta(h)$ appartient à $b_{n-1}$ pour tout polynôme $h$ homogène de degré $n \geq 1$. Soit alors $u \in A[[X]]$ et soit $u_n$ la composante homogène de degré $n$ de $u$. Comme on a $\Delta(u_n) \in b_{n-1}$ pour $n \geq 1$, la famille $(\Delta(u_n))_{n \geq 0}$ est sommable dans $A[[X]]$ et l’on définit une application $D$ de $A[[X]]$ dans lui-même par

$$
D(u) = \sum_{n \geq 0} \Delta(u_n).
$$

On a $D(b_n) \subset b_{n-1}$, donc $D$ est un endomorphisme continu du groupe additif de $A[[X]]$. L’application $\Phi : (u, v) \mapsto D(uv) - uD(v) - D(u)v$ de $A[[X]] \times A[[X]]$ dans $A[[X]]$ est continue et nulle sur $A[X] \times A[X]$. Comme $A[X]$ est dense dans $A[[X]]$, on a $\Phi = 0$; autrement dit, $D$ est une dérivation de $A[[X]]$ dans $A[[X]]$, prolongeant $\Delta$.

Enfin, $A[X]$ est dense dans $A[[X]]$, et toute dérivation dans $A[[X]]$ est continue, d’après (i) ; par suite, il existe un unique prolongement de $\Delta$ en une dérivation de $A[[X]]$. Ceci prouve (ii).

Prouvons enfin (iii). La formule (18) (IV, p. 31) montre que la famille $(D_i)_{i \in I}$ est linéairement indépendante sur $A[[X]]$. La formule (16) (IV, p. 31), appliquée au cas $E = A[[X]]$, prouve que toute $A$-dérivation est une combinaison linéaire des dérivations $D_i$ à coefficients dans $A[[X]]$.

C.Q.F.D.

#### Proposition 9 {#alg-iv-s4-prop-9 .statement}

Soient $(u_\lambda)_{\lambda \in L}$ une famille sommable d’éléments sans terme constant de $A[[I]]$ et $D$ une dérivation continue de la $A$-algèbre $A[[I]]$. Posons $f = \prod_{\lambda \in L} (1 + u_\lambda)$ (IV, p. 25, prop. 2). Alors la famille $(Du_\lambda/(1 + u_\lambda))_{\lambda \in L}$ est sommable et l’on a

$$
D(f)/f = \sum_{\lambda \in L} D(u_\lambda)/(1 + u_\lambda).
$$

Si $g$ et $h$ sont deux éléments inversibles de $\mathbf{A}[[\mathbf{I}]]$, on a
$$
\mathbf{D}(gh) = h \cdot \mathbf{D}(g) + g \cdot \mathbf{D}(h)
$$
d’où, par division par $gh$,
$$(21)$$
$$
\mathbf{D}(gh)/gh = \mathbf{D}(g)/g + \mathbf{D}(h)/h .
$$
Pour toute partie finie $M$ de $L$, posons $f_M = \prod_{\lambda \in M} (1 + u_\lambda)$. On déduit de (21), par récurrence sur Card $M$, la relation
$$(22)$$
$$
\mathbf{D}(f_M)/f_M = \sum_{\lambda \in M} \mathbf{D}(u_\lambda)/(1 + u_\lambda) .
$$
La prop. 9 est donc prouvée lorsque $L$ est fini. Supposons désormais $L$ infini et notons $\mathfrak{F}$ l’ensemble ordonné filtrant des parties finies de $L$. On a $\lim_{\mathfrak{F}} f_M = f$, et par suite (IV, p. 29, remarque)
$$
\mathbf{D}(f)/f = \lim_{\mathfrak{F}} \mathbf{D}(f_M)/f_M .
$$
La prop. 9 résulte alors par passage à la limite de (22).

### 7. Résolution des équations dans un anneau de séries formelles

#### Lemme 2 {#alg-iv-s4-lem-2 .statement}

Soit $(g_i)_{i \in I}$ une famille d’éléments d’ordre $\geqslant 2$ dans $\mathbf{A}[[\mathbf{I}]]$. Lorsque $I$ est infini, on suppose que $g_i$ tend vers 0 selon le filtre des complémentaires des parties finies de $I$. Il existe alors un automorphisme $T$ de la $\mathbf{A}$-algèbre topologique $\mathbf{A}[[\mathbf{I}]]$, et un seul, tel que $T(X_i) = X_i + g_i$ pour tout $i \in I$. De plus, on a
$$(23)$$
$$
\omega(T(u) - u) \geqslant \omega(u) + 1
$$
pour tout $u \in \mathbf{A}[[\mathbf{I}]]$.

La série $f_i = X_i + g_i$ est sans terme constant, et lorsque $I$ est infini, $f_i$ tend vers 0 selon le filtre des complémentaires des parties finies de $I$. Par suite (IV, p. 26, prop. 4), il existe un endomorphisme continu $T$ de la $\mathbf{A}$-algèbre $\mathbf{A}[[\mathbf{I}]]$, et un seul, tel que $T(X_i) = f_i$ pour tout $i \in I$. Pour tout $v \in \mathbf{N}^{(I)}$, posons
$$
v_v = T(X^v) - X^v = \prod_{i \in I} (X_i + g_i)^{v(i)} - \prod_{i \in I} X_i^{v(i)} ;
$$
les relations $\omega(g_i) \geqslant 2$ entraînent $\omega(v_v) \geqslant |v| + 1$, et la relation (23) résulte aussitôt de là.

Montrons que $T$ est injectif. Soit $u \in \mathbf{A}[[\mathbf{I}]]$ tel que $T(u) = 0$; d’après (23), on a $\omega(u) \geqslant \omega(u) + 1$, ce qui est impossible si $u \neq 0$, car alors $\omega(u)$ serait un entier positif.

Pour toute série formelle $v$ dans $\mathbf{A}[[\mathbf{I}]]$, notons $H_n(v)$ sa composante homogène de degré $n$. Posons $S_0(v) = H_0(v)$ et définissons les applications continues $S_n : A[[I]] \to A[[I]]$ par l’équation de récurrence

$$
(24) \quad S_n(v) = H_n(v - T(\sum_{k=0}^{n-1} S_k(v))) \quad \text{pour } n \geq 1 .
$$

Posons $S(v) = \sum_{n \geq 0} S_n(v)$. Soit $v \in \mathbf{N}^{(l)}$ et soit $n = |v|$; le coefficient $S^v(v)$ de $X^v$ dans $S(v)$ est égal à celui de $X^v$ dans $S_n(v)$; comme $S_n$ est une application continue, l’application $S^v : A[[I]] \to A$ est continue. Vu la définition de la topologie produit sur $A[[I]] = A^{\mathbf{N}^{(l)}}$, l’application $S : A[[I]] \to A[[I]]$ est continue.

Nous allons prouver la relation $T(S(v)) = v$ pour tout $v \in A[[I]]$, ce qui achèvera de prouver le lemme. Soient $v \in A[[I]]$, $u_n = S_n(v)$ et $u = S(v)$. Soit $n$ un entier positif tel que l’on ait

$$
(25)_n \qquad \omega(v - T(u)) \geq n .
$$

On a $\omega(u - (u_0 + \cdots + u_{n-1})) \geq n$, d’où

$$
(26) \qquad \omega(T(u) - T(u_0 + \cdots + u_{n-1}) - u_n) \geq n + 1
$$

d’après (23). L’équation de récurrence (24) entraîne

$$
(27) \qquad u_n = H_n(v - T(u_0 + \cdots + u_{n-1})) .
$$

D’après (26), les séries formelles $v - T(u)$ et $v - T(u_0 + \cdots + u_{n-1}) - u_n$ ont même composante homogène de degré $n$, et cette composante est nulle d’après (27). On a donc $\omega(v - T(u)) \geq n + 1$, c’est-à-dire que $(25)_n$ entraîne $(25)_{n+1}$. Comme la formule $(25)_0$ est évidente, on a donc $\omega(v - T(u)) \geq n$ pour tout entier $n \geq 0$, d’où $v = T(u) = T(S(v))$.

C.Q.F.D.

Dans la suite de ce numéro, pour tout ensemble $I$, nous noterons $A\{I\}$ l’ensemble des familles $(f_i)_{i \in I}$ satisfaisant aux conditions suivantes :
(i) pour tout $i \in I$, $f_i$ est un élément de $A[[I]]$ sans terme constant ;
(ii) si $I$ est infini, $f_i$ tend vers 0 suivant le filtre des complémentaires des parties finies de $I$.

L’ensemble $A\{I\}$ est un monoïde pour la loi de composition $(f, g) \mapsto f \circ g$, avec $(X_i)_{i \in I}$ pour élément unité. L’ensemble des éléments inversibles de $A\{I\}$ est donc un groupe.

D’autre part, soit $E$ le monoïde des endomorphismes unifères continus de la $A$-algèbre $A[[I]]$ qui laissent stable l’idéal des séries formelles sans terme constant. Si $f \in A\{I\}$ et $g \in A[[I]]$, l’élément $g(f)$ est défini. Pour $f$ fixé, l’application $g \mapsto g(f)$ de $A[[I]]$ dans $A[[I]]$ est un élément $W_f$ de $E$. Si $f_1, f_2 \in A\{I\}$ et $g \in A[[I]]$, on a, d’après la formule (5) (IV, p. 28)

$$
W_{f_1 \circ f_2}(g) = g(f_1 \circ f_2) = g(f_1) \circ f_2 = W_{f_2}(W_{f_1}(g))
$$

donc $f \mapsto W_f$ est un homomorphisme du monoïde opposé à $A\{I\}$ dans E. D’après la prop. 4 (IV, p. 26 ), cet homomorphisme est bijectif.

Soient $f = (f_i)_{i \in I} \in A\{I\}$, et $\sum_{j \in I} \alpha_{ij} X_j$ la composante homogène de degré 1 de $f_i$. Pour tout $j$ fixé dans I, on a $\alpha_{ij} = 0$ sauf pour un nombre fini d’indices $i$ d’après l’hypothèse (ii) ci-dessus. Si $(\lambda_i) \in A^{(I)}$, on a donc $(\sum_{j \in I} \alpha_{ij} \lambda_j) \in A^{(I)}$. Notons $T_f$ l’application A-linéaire $^1$

$$
(\lambda_i) \mapsto (\sum_{j \in I} \alpha_{ij} \lambda_j)
$$

de $A^{(I)}$ dans $A^{(I)}$. Si $g \in A\{I\}$, on vérifie aisément que

$$(28)$$
$$
T_{f \circ g} = T_f \circ T_g .
$$

**Proposition 10. — Soit $f \in A\{I\}$. Les conditions suivantes sont équivalentes :**

(i) $f$ est inversible dans $A\{I\}$ pour la loi $\circ$ :
(ii) $T_f$ est inversible dans l’anneau $\mathrm{End}(A^{(I)})$.

L’implication (i) $\Rightarrow$ (ii) résulte aussitôt de (28). Supposons $T_f$ inversible dans $\mathrm{End}(A^{(I)})$. Il existe $g = (g_i)_{i \in I} \in A\{I\}$ tel que chaque $g_i$ soit homogène de degré 1 et que $T_g \circ T_f$ soit l’application identique de $A^{(I)}$. Posons $h = g \circ f$; la formule (28) montre que $T_h$ est l’application identique de $A^{(I)}$, ce qui équivaut à $\omega(h_i - X_i) \geq 2$. D’après le lemme 2 de IV, p. 33, $h$ est donc inversible dans $A\{I\}$. Il est clair que $g$ est inversible dans $A\{I\}$. Donc $f$ est inversible dans $A\{I\}$.

**Corollaire. — Soient $f_i(Y_1, Y_2, ..., Y_q, X_1, X_2, ..., X_p)$ ($1 \leq i \leq q$) q séries formelles sans terme constant dans $A[[Y_1, ..., Y_q, X_1, ..., X_p]]$. Si le terme constant de la série formelle $D = \det \left( \frac{\partial f_i}{\partial Y_j} \right)$ est inversible dans $A$, il existe un système et un seul de q séries formelles sans terme constant $u_1(X_1, ..., X_p), ..., u_q(X_1, ..., X_p)$ telles que

$$(29)$$
$$
f_i(u_1, ..., u_q, X_1, ..., X_p) = 0 \quad (1 \leq i \leq q) .
$$

Posons $f_{q+1} = X_1, ..., f_{q+p} = X_p$, $f = (f_1, ..., f_{q+p})$. Alors $\det T_f$ est égal au terme constant de D, donc est inversible dans $A$; par suite $T_f$ est inversible. D’après la prop. 10, il existe des séries formelles sans terme constant

$$
g_1, ..., g_{q+p} \in A[[Y_1, ..., Y_q, X_1, ..., X_p]]
$$

telles que, posant

$$
g = (g_1, ..., g_{p+q}) , \quad 1_{p+q} = (Y_1, ..., Y_q, X_1, ..., X_p)
$$

on ait $f \circ g = g \circ f = 1_{p+q}$. La relation $f \circ g = 1_{p+q}$ donne en particulier

$$
g_{q+1} = X_1, ..., g_{q+p} = X_p .
$$

Donc

$$(30)$$
$$
f_i(g_1, ..., g_q, X_1, ..., X_p) = Y_i \quad (1 \leq i \leq q) .
$$

$^1$ On dit parfois que $T_f$ est l’application linéaire tangente à $f$.

Posons

(31) $$ u_i(X_1, ..., X_p) = g_i(0, ..., 0, X_1, ..., X_p) \quad (1 \leq i \leq q); $$

substituant 0 à chacun des $Y_i$ dans (30), on obtient la relation cherchée (29).

Réciproquement, supposons que les séries formelles $u_1, ..., u_q$ dans l’anneau $A[[X_1, ..., X_p]]$ satisfassent à la relation (29). La relation $g \circ f = 1_{p+q}$ entraîne

(32) $$ g_i(f_1, ..., f_q, X_1, ..., X_p) = Y_i \quad (1 \leq i \leq q); $$

substituant $u_i$ à $Y_i$ pour $1 \leq i \leq q$ dans (32), on obtient (31), d’où l’unicité de la solution du système (29).

### 8. Séries formelles sur un anneau intègre

#### Proposition 11 {#alg-iv-s4-prop-11 .statement}

Supposons A intègre.

(i) L’anneau $A[[I]]$ est intègre.

(ii) Si $u$ et $v$ sont des éléments non nuls de $A[[I]]$, on a $\omega(uv) = \omega(u) + \omega(v)$.

Pour tout $J \subset I$, soit $\varphi_J$ l’homomorphisme de $A[[I]]$ dans $A[[J]]$ obtenu en substituant, dans tout élément de $A[[I]]$, $X_i$ à $X_i$ pour $i \in J$ et 0 à $X_i$ pour $i \in I - J$. Soient $u, v$ des éléments non nuls de $A[[I]]$, $p = \omega(u)$ et $q = \omega(v)$. Il existe une partie finie $J$ de $I$ telle que
$$
\varphi_J(u) \neq 0,\ \varphi_J(v) \neq 0,\ \omega(\varphi_J(u)) = p,\ \omega(\varphi_J(v)) = q.
$$
Soit $a$ (resp. $b$) la composante homogène de degré $p$ (resp. $q$) de $\varphi_J(u)$ (resp. $\varphi_J(v)$). Comme $J$ est fini, $a$ et $b$ sont des polynômes. On a $a \neq 0, b \neq 0$, donc $ab \neq 0$ (IV, p. 9, prop. 8). Par suite, $\varphi_J(u) \varphi_J(v)$ est non nul et d’ordre $p + q$. Il en résulte que $uv \neq 0$ et que $\omega(uv) \leq p + q$. Enfin, il est clair que $\omega(uv) \geq p + q$.

### 9. Corps des fractions de l’anneau des séries formelles en une indéterminée sur un corps

Si K est un corps commutatif, on désigne par $K((X))$ le corps des fractions de l’anneau intègre $K[[X]]$.

#### Proposition 12 {#alg-iv-s4-prop-12 .statement}

Tout élément non nul $u$ de $K((X))$ s’écrit d’une seule manière sous la forme $u = X^k v$, où $k \in \mathbf{Z}$ et où $v$ est une série formelle en $X$ d’ordre 0.

Soit $u = w/t$, où $w, t$ sont des éléments non nuls de $K[[X]]$. On a $w = X^r w_1$, $t = X^s t_1$, où $r, s \in \mathbf{N}$ et où $w_1, t_1$ sont des séries formelles d’ordre 0, donc inversibles dans $K[[X]]$ (IV, p. 28, prop. 6). Alors $u = X^{r-s} w_1 t_1^{-1}$, et $w_1 t_1^{-1}$ est une série formelle d’ordre 0.

Démontrons l’unicité. Supposons $u = X^{k_1} v_1 = X^{k_2} v_2$ où $k_1, k_2 \in \mathbf{Z}$ et où $v_1, v_2$ sont des séries formelles d’ordre 0. Puisque $X^{k_1 - k_2} = v_2 v_1^{-1}$ est une série formelle d’ordre 0, on a $k_1 = k_2$, d’où $v_1 = v_2$, ce qui prouve l’assertion d’unicité de la proposition.

On dit que les éléments de $K((X))$ sont les séries formelles généralisées en $X$, à coefficients dans $K$, ou simplement les séries formelles si aucune confusion n’en résulte (les éléments de $K[[X]]$ sont alors appelés séries formelles à exposants positifs); si $u \neq 0$, l’entier $k$ défini dans la prop. 12 est encore appelé l’ordre de $u$ et noté $\omega(u)$ même s’il est $< 0$; on pose encore $\omega(0) = \infty$. On vérifie immédiatement que les relations

$$
\begin{align*}
\omega(u + v) &\geq \inf(\omega(u), \omega(v)) \\
\omega(u + v) &= \inf(\omega(u), \omega(v)) \quad \text{si} \quad \omega(u) \neq \omega(v) \\
\omega(uv) &= \omega(u) + \omega(v)
\end{align*}
$$

sont encore valables pour les séries formelles généralisées. En particulier, si $u \neq 0$, on a $\omega(u^{-1}) = -\omega(u)$. \* Autrement dit (AC, VI, § 3, no 6, déf. 3), $\omega$ est une valuation discrète normée du corps $K((X))$. \*

Pour tout entier $n \in \mathbf{Z}$, soit $p_n$ l’ensemble des $u \in K((X))$ tels que $\omega(u) \geq n$. Alors $(p_n)_{n \in \mathbf{Z}}$ est une suite décroissante de sous-groupes du groupe additif $K((X))$, d’intersection 0 ; il existe donc une topologie sur $K((X))$, invariante par translation, pour laquelle $(p_n)_{n \in \mathbf{Z}}$ est un système fondamental de voisinages de 0 (TG, III, p. 5). On vérifie facilement que $K((X))$ est un corps topologique (TG, III, p. 54) et que $K[[X]]$ est un sous-espace ouvert et fermé de $K((X))$.

Soit $(\alpha_n)_{n \in \mathbf{Z}}$ une famille d’éléments de $K$; on suppose qu’il existe un entier $N$ tel que $\alpha_n = 0$ pour tout $n < N$. Alors la famille $(\alpha_n X^n)_{n \in \mathbf{Z}}$ est sommable dans $K((X))$ (TG, III, p. 39, cor. 2); posons $u = \sum_{n \in \mathbf{Z}} \alpha_n X^n$. Alors $u = 0$ si et seulement si l’on a $\alpha_n = 0$ pour tout $n$; sinon, l’ordre de $u$ est le plus petit entier $k$ tel que $\alpha_k \neq 0$. Enfin, tout élément de $K((X))$ s’écrit de manière unique sous la forme $\sum_{n \in \mathbf{Z}} \alpha_n X^n$, la suite $(\alpha_n)$ vérifiant $\alpha_{-n} = 0$ pour tout $n$ assez grand.

L’anneau $K[X]$ étant un sous-anneau de $K[[X]]$, toute fraction rationnelle $u/v \in K(X)$ ($u$ et $v$ sont des polynômes en $X$) peut être identifiée à la série formelle (généralisée) $uv^{-1}$ de $K((X))$, qu’on appelle son développement à l’origine ; le corps $K(X)$ est ainsi identifié à un sous-corps de $K((X))$.

### 10. Exponentielle et logarithme

On appelle série exponentielle l’élément $\sum_{n \geq 0} \frac{X^n}{n!}$ de $\mathbf{Q}[[X]]$. On la note $\exp X$ ou $e^X$.

#### Proposition 13 {#alg-iv-s4-prop-13 .statement}

Dans $\mathbf{Q}[[X, Y]]$, on a $e^{X+Y} = e^X e^Y$.

En effet, la formule du binôme donne

$$
\frac{(X + Y)^n}{n!} = \sum_{i+j=n} \frac{X^i}{i!} \frac{Y^j}{j!}.
$$

Donc
$$
e^X e^Y = \left( \sum_{i \geq 0} \frac{X^i}{i!} \right) \left( \sum_{j \geq 0} \frac{Y^j}{j!} \right) = \sum_{i,j \geq 0} \frac{X^i}{i!} \frac{Y^j}{j!} = \sum_{n \geq 0} \sum_{i+j=n} \frac{X^i}{i!} \frac{Y^j}{j!}
$$
$$
= \sum_{n \geq 0} \frac{(X+Y)^n}{n!} = e^{X+Y}.
$$

Définissons deux éléments $e(X), l(X)$ de $\mathbf{Q}[[X]]$ par

(33)
$$
e(X) = e^X - 1 = \sum_{n \geq 1} \frac{X^n}{n!}
$$

(34)
$$
l(X) = \sum_{n \geq 1} (-1)^{n-1} \frac{X^n}{n}.
$$

On a
(35)
$$
e(X+Y) = e(X) + e(Y) + e(X) e(Y)
$$
(36)
$$
\mathrm{D}(e^X) = \mathrm{D}(e(X)) = e^X
$$
(37)
$$
\mathrm{D}(l(X)) = \sum_{n \geq 0} (-X)^n = (1+X)^{-1}.
$$

#### Proposition 14 {#alg-iv-s4-prop-14 .statement}

*On a* $l(e(X)) = e(l(X)) = X$.

Les séries $l$ et $e$ sont sans terme constant, et leurs termes de degré 1 sont égaux à $X$. D’après la prop. 10 de IV, p. 35, il suffit de prouver la formule $l(e(X)) = X$. D’après les formules (36) et (37), et le cor. 3 de IV, p. 31, on a
$$
\mathrm{D}(l(e(X))) = (1 + e(X))^{-1} \mathrm{D}(e(X)) = (e^X)^{-1} e^X = 1
$$
d’où $l(e(X)) = X$.

Soit $K$ une $\mathbf{Q}$-algèbre. Les éléments de $K[[I]]$ sans terme constant forment pour l’addition un groupe commutatif $\mathcal{E}$. Les éléments de $K[[I]]$ de terme constant 1 forment pour la multiplication un groupe commutatif $\mathcal{M}$ (IV, p. 29). On peut définir, pour tout $f \in \mathcal{E}$, les éléments $e \circ f$ et $l \circ f$ de $\mathcal{E}$. D’après la prop. 14 ci-dessus, les applications $f \mapsto l \circ f$ et $f \mapsto e \circ f$ sont des permutations réciproques de $\mathcal{E}$. Elles sont évidemment continues. Comme on a $\exp X = e(X) + 1$, on voit que l’application exponentielle $f \mapsto \exp f = e \circ f + 1$ est une bijection bicontinue de $\mathcal{E}$ sur $\mathcal{M}$. D’après la formule (4) de IV, p. 28, et la prop. 13, on a $\exp(f+g) = (\exp f)(\exp g)$ si $f, g \in \mathcal{E}$. Donc l’exponentielle est un isomorphisme du groupe topologique $\mathcal{E}$ sur le groupe topologique $\mathcal{M}$.

L’isomorphisme réciproque de $\mathcal{M}$ sur $\mathcal{E}$ s’appelle le logarithme et se note $g \mapsto \log g$. On a donc $\log g = l(g-1)$ pour $g$ dans $\mathcal{M}$, et, en particulier
(38)
$$
\log(1+X) = l(X).
$$

Comme le logarithme est un homomorphisme de $\mathcal{M}$ dans $\mathcal{E}$, la formule

(1 + X)(1 + Y) = 1 + (X + Y + XY) entraîne

$$(39)$$
$$l(X) + l(Y) = l(X + Y + XY).$$

Soit $(u_\lambda)_{\lambda \in L}$ une famille sommable d’éléments de $E$. La famille $(\exp u_\lambda)_{\lambda \in L}$ est multipliable, et l’on a

$$(40)$$
$$\exp(\sum_{\lambda \in L} u_\lambda) = \prod_{\lambda \in L} \exp u_\lambda.$$

De même si $(f_\lambda)_{\lambda \in L}$ est une famille multipliable d’éléments de $M$, la famille $(\log f_\lambda)_{\lambda \in L}$ est sommable, et l’on a

$$(41)$$
$$\log(\prod_{\lambda \in L} f_\lambda) = \sum_{\lambda \in L} \log f_\lambda.$$

Soit $g \in M$, et soit D une dérivation continue de $K[[I]]$. On a $\log g = l(g - 1)$, donc, d’après le cor. 3 de IV, p. 31 et la formule (37), on a

$$(42)$$
$$D \log g = D(g)/g.$$

L’expression $D(g)/g$ est appelée la *dérivée logarithmique* de $g$ (relativement à D).

## EXERCICES {#alg-iv-s4-exercises}

See the [exercises for § 4](exercises/s4/).
