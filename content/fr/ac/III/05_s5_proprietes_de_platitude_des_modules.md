---
book: ac
book_title: Commutative Algebra
chapter: III
chapter_title: Graduations, filtrations et topologies
section: 5
section_title: Propriétés de platitude des modules filtrés
lang: fr
source: ac-i-iv-fr
pdf_pages: 0271-0277, 0303-0304
extraction: ocr
subsections:
    - "no": 1
      title: Modules idéalement séparés.
      page: 0
      pdf_page: 271
    - "no": 2
      title: Énoncé du critère de platitude.
      page: 0
      pdf_page: 271
    - "no": 3
      title: Démonstration du critère de platitude.
      page: 0
      pdf_page: 272
    - "no": 4
      title: Applications.
      page: 0
      pdf_page: 275
statements: 11
exercises: 8
content_sha256: 027647b256ef4b582d8f1e7c8248bf63f20a78764e2ce2f372c52dc1ce8df431
---

## § 5. Propriétés de platitude des modules filtrés.

### 1. Modules idéalement séparés.

#### Définition 1 {#ac-iii-s5-def-1 .statement}

Soient $A$ un anneau commutatif, $\mathfrak{J}$ un idéal de $A$. On dit qu’un $A$-module $M$ est idéalement séparé pour $\mathfrak{J}$ (ou simplement idéalement séparé s’il n’en résulte pas de confusion) si, pour tout idéal $a$ de type fini de $A$, le $A$-module $a \otimes_A M$ est séparé pour la topologie $\mathfrak{J}$-adique.

Faisant $a = A$ dans cette définition, on voit déjà que $M$ est nécessairement séparé pour la topologie $\mathfrak{J}$-adique.

#### Exemple 1 {#ac-iii-s5-n1-exa-1 .statement}

Si $A$ est noethérien, et si $\mathfrak{J}$ est contenu dans le radical de $A$ (autrement dit si $A$ est un anneau de Zariski pour la topologie $\mathfrak{J}$-adique), tout $A$-module de type fini est idéalement séparé ($\S$ 3, no 3, prop. 6).

#### Exemple 2 {#ac-iii-s5-n1-exa-2 .statement}

Toute somme directe de modules idéalement séparés est un module idéalement séparé, en vertu des relations
$$
\mathfrak{J}^n(a \otimes_A \bigoplus_{\lambda \in L} M_\lambda) = \mathfrak{J}^n \bigoplus_{\lambda \in L} (a \otimes_A M_\lambda) = \bigoplus_{\lambda \in L} \mathfrak{J}^n(a \otimes_A M_\lambda).
$$

#### Exemple 3 {#ac-iii-s5-n1-exa-3 .statement}

Si un $A$-module $M$ est plat et séparé pour la topologie $\mathfrak{J}$-adique il est idéalement séparé, car $a \otimes_A M$ s’identifie alors à un sous-module de $M$, et la topologie $\mathfrak{J}$-adique sur $a \otimes_A M$ est plus fine que la topologie induite sur $a \otimes_A M$ par la topologie $\mathfrak{J}$-adique de $M$, qui est séparée par hypothèse.

### 2. Énoncé du critère de platitude.

Soient $A$ un anneau, $\mathfrak{J}$ un idéal bilatère de $A$, $M$ un $A$-module à gauche, $\mathrm{gr}(A)$ et $\mathrm{gr}(M)$ l’anneau gradué et le $\mathrm{gr}(A)$-module gradué associés respectivement à l’anneau $A$ et au module $M$ munis des filtrations $\mathfrak{J}$-adiques ($\S$ 2, no 3). On a vu (loc. cit.) qu’on a pour tout entier $n \geqslant 0$ un homomorphisme surjectif de $\mathbf{Z}$-modules
$$
\gamma_n : (\mathfrak{J}^n/\mathfrak{J}^{n+1}) \otimes_{A/\mathfrak{J}} (M/\mathfrak{J}M) \to \mathfrak{J}^n M/\mathfrak{J}^{n+1} M
$$
et un homomorphisme gradué de degré 0 de $\mathrm{gr}(A)$-modules gradués
$$
\gamma_M : \mathrm{gr}(A) \otimes_{\mathrm{gr}_0(A)} \mathrm{gr}_0(M) \to \mathrm{gr}(M)
$$

dant la restriction à $\mathrm{gr}_n(A) \otimes_{\mathrm{gr}_0(A)} \mathrm{gr}_0(M)$ est $\gamma_n$ pour tout $n$, et qui est par suite surjectif.

#### Théorème 1 {#ac-iii-s5-thm-1 .statement}

Soient $A$ un anneau commutatif, $\mathfrak{J}$ un idéal de $A$, $M$ un $A$-module. Considérons les propriétés suivantes :
(i) $M$ est un $A$-module plat.
(ii) $\mathrm{Tor}_1^A(N, M) = 0$ pour tout $A$-module $N$ annulé par $\mathfrak{J}$.
(iii) $M/\mathfrak{J}M$ est un $(A/\mathfrak{J})$-module plat et l’application canonique $\mathfrak{J} \otimes_A M \to \mathfrak{J}M$ est bijective (cette dernière condition étant équivalente à $\mathrm{Tor}_1^A(A/\mathfrak{J}, M) = 0$ en vertu de la relation $\mathrm{Tor}_1^A(A, M) = 0$ et de la suite exacte $\mathrm{Tor}_1^A(A, M) \to \mathrm{Tor}_1^A(A/\mathfrak{J}, M) \to \mathfrak{J} \otimes_A M \to M$).
(iv) $M/\mathfrak{J}M$ est un $(A/\mathfrak{J})$-module plat, et l’homomorphisme canonique $\gamma_M : \mathrm{gr}(A) \otimes_{\mathrm{gr}_0(A)} \mathrm{gr}_0(M) \to \mathrm{gr}(M)$, est bijectif (propriété (GR) du § 2, no 8).
(v) Pour tout $n \geq 1$, $M/\mathfrak{J}^nM$ est un $(A/\mathfrak{J}^n)$-module plat.
Alors on a (i) $\Rightarrow$ (ii) $\Leftrightarrow$ (iii) $\Rightarrow$ (iv) $\Leftrightarrow$ (v).
Si en outre $\mathfrak{J}$ est nilpotent, ou si $A$ est noethérien et $M$ idéalement séparé, les propriétés (i), (ii), (iii), (iv) et (v) sont équivalentes.

#### Remarque {#ac-iii-s5-n2-rem-1 .statement}

Lorsque $A/\mathfrak{J}$ est un corps (cas fréquent dans les applications) la condition « $M/\mathfrak{J}M$ est un $(A/\mathfrak{J})$-module plat » est automatiquement vérifiée pour tout $A$-module $M$, ce qui simplifie l’énoncé des propriétés (iii) et (iv) ; en outre, dans ce cas, la propriété (v) équivaut à dire que $M/\mathfrak{J}^nM$ est un $(A/\mathfrak{J}^n)$-module libre pour tout entier $n \geq 1$ (chap. II, § 3, no 2, cor. 2 de la prop. 5).

### 3. Démonstration du critère de platitude.

A) Les implications (i) $\Rightarrow$ (ii) $\Leftrightarrow$ (iii).
L’implication (i) $\Rightarrow$ (ii) est immédiate (chap. I, § 4). L’équivalence (ii) $\Leftrightarrow$ (iii) est un cas particulier du chap. I, § 4, prop. 2, appliquée à $R = A, S = A/\mathfrak{J}, F = M, E = N$, en tenant compte de ce que la donnée d’une structure de $(A/\mathfrak{J})$-module sur $N$ équivaut à la donnée d’une structure de $A$-module pour laquelle $N$ est annulé par $\mathfrak{J}$.

Remarque 1). — La condition (ii) est aussi équivalente à la suivante :

(ii') Tor_1^A(N, M) = 0 pour tout A-module N annulé par une puissance de $\mathfrak{J}$.

En effet, il est clair que (ii') implique (ii). Réciproquement, si (ii) est vérifiée, on a en particulier Tor_1^A(\mathfrak{J}^n N/\mathfrak{J}^{n+1} N, M) = 0 pour tout n ; de la suite exacte

$$
0 \to \mathfrak{J}^{n+1} N \to \mathfrak{J}^n N \to \mathfrak{J}^n N/\mathfrak{J}^{n+1} N \to 0
$$

on déduit la suite exacte

$$
\text{Tor}_1^A(\mathfrak{J}^{n+1} N, M) \to \text{Tor}_1^A(\mathfrak{J}^n N, M) \to \text{Tor}_1^A(\mathfrak{J}^n N/\mathfrak{J}^{n+1} N, M),
$$

et comme il existe un entier m tel que $\mathfrak{J}^m N = 0$, on en déduit par récurrence descendante sur n que $\text{Tor}_1^A(\mathfrak{J}^n N, M) = 0$ pour tout $n \leq m$, et en particulier pour $n = 0$.

Il résulte de là que lorsque $\mathfrak{J}$ est nilpotent, (ii) $\Rightarrow$ (i), car (ii') signifie alors que $\text{Tor}_1^A(N, M) = 0$ pour tout A-module N, donc que M est plat (chap. I, § 4).

B) Démontrons la proposition suivante :

#### Proposition 1 {#ac-iii-s5-prop-1 .statement}

Soient A un anneau commutatif, $\mathfrak{J}$ un idéal de A, M un A-module. Les conditions suivantes sont équivalentes :
a) Pour tout $n \geq 1$, on a $\text{Tor}_1^A(A/\mathfrak{J}^n, M) = 0$.
b) Pour tout $n \geq 1$, l'homomorphisme canonique
$$
\theta_n : \mathfrak{J}^n \otimes_A M \to \mathfrak{J}^n M
$$
est bijectif.

En outre ces conditions entraînent :
c) L'homomorphisme canonique $\gamma_M : \mathrm{gr}(A) \otimes_{\mathrm{gr}_0(A)} \mathrm{gr}_0(M) \to \mathrm{gr}(M)$
est bijectif.

Réciproquement, si $\mathfrak{J}$ est nilpotent, c) entraîne a) et b).

L'équivalence de a) et b) résulte de la suite exacte

$$
0 = \text{Tor}_1^A(A, M) \to \text{Tor}_1^A(A/\mathfrak{J}^n, M) \to \mathfrak{J}^n \otimes_A M \to M.
$$

Considérons ensuite le diagramme

$$
\begin{array}{cccccc}
\mathfrak{J}^{n+1} \otimes_A M & \longrightarrow & \mathfrak{J}^n \otimes_A M & \longrightarrow & (\mathfrak{J}^n/\mathfrak{J}^{n+1}) \otimes_A (M/\mathfrak{J}M) & \longrightarrow 0 \\
\theta_{n+1} \downarrow & & \theta_n \downarrow & & \gamma_n \downarrow & \\
0 & \longrightarrow & \mathfrak{J}^{n+1} M & \longrightarrow & \mathfrak{J}^n M & \longrightarrow \mathrm{gr}_n(M) \longrightarrow 0
\end{array}
$$

où on note que $(\mathfrak{J}^n/\mathfrak{J}^{n+1}) \otimes_A (M/\mathfrak{J}M)$ s’identifie canoniquement avec $(\mathfrak{J}^n/\mathfrak{J}^{n+1}) \otimes_{A/\mathfrak{J}} (M/\mathfrak{J}M)$. Ce diagramme est commutatif par définition de $r_n$ et ses lignes sont exactes. Si b) est vérifiée, $\theta_n$ et $\theta_{n+1}$ sont bijectifs, et il en est donc de même de $r_n$ par définition d’un conoyau, donc b) entraîne c). Inversement, supposons $\mathfrak{J}$ nilpotent, et montrons que c) entraîne b); nous procéderons par récurrence descendante sur $n$, puisque $\mathfrak{J}^n \otimes_A M = \mathfrak{J}^n M = 0$ pour $n$ assez grand. Supposons donc que dans le diagramme (1), $r_n$ et $\theta_{n+1}$ soient bijectifs ; il en est alors de même de $\theta_n$ en vertu du chap. I, § 1, no 4, cor. 1 de la prop. 2.

C) *L’implication* (ii) $\Rightarrow$ (iv).

Si (ii) est vérifié, il en est de même de (ii’) en vertu de la *Remarque* 1); la prop. 1 montre donc que $r_m$ est un isomorphisme. D’autre part, on sait déjà que (ii) entraîne (iii), donc $M/\mathfrak{J}M$ est un $(A/\mathfrak{J})$-module plat, ce qui achève de prouver que (ii) entraîne (iv).

*Remarque* 2). — La prop. 1 montre que lorsque $\mathfrak{J}$ est nilpotent, (iv) entraîne (iii); compte tenu de la *Remarque* 1), on a donc prouvé dans ce cas que (i), (ii), (iii) et (iv) sont équivalentes.

D) *L’équivalence* (iv) $\Leftrightarrow$ (v).

Pour tout $n \geqslant 1$, $M/\mathfrak{J}^n M$ est canoniquement muni d’une structure de $(A/\mathfrak{J}^n)$-module. Si on le filtre par la filtration $(\mathfrak{J}/\mathfrak{J}^n)$-adique, il est immédiat que $\mathrm{gr}_m(M/\mathfrak{J}^n M) = \mathrm{gr}_m(M)$ si $m < n$, et $\mathrm{gr}_m(M/\mathfrak{J}^n M) = 0$ si $m \geqslant n$. Pour tout $k \geqslant 1$, posons $A_k = A/\mathfrak{J}^k$, $\mathfrak{J}_k = \mathfrak{J}/\mathfrak{J}^k$, $M_k = M/\mathfrak{J}^k M$; notons (iv)_k (resp. (v)_k) l’assertion déduite de (iv) (resp. (v)) en remplaçant $A$, $\mathfrak{J}$, $M$ par $A_k$, $\mathfrak{J}_k$, $M_k$. Il résulte de ce qu’on vient de dire que (iv) équivaut à « pour tout $k \geqslant 1$, (iv)_k », et il est évident que (v) équivaut à « pour tout $k \geqslant 1$, (v)_k ». Il suffira donc d’établir l’équivalence (iv)_k $\Leftrightarrow$ (v)_k pour tout $k$, ou encore de démontrer que (iv) $\Leftrightarrow$ (v) lorsque $\mathfrak{J}$ est *nilpotent*. Or (*Remarque* 2) on a vu que dans ce cas (iv) équivaut à (i). Comme $M/\mathfrak{J}^n M$ est isomorphe à $M \otimes_A (A/\mathfrak{J}^n)$, (i) entraîne (v) (chap. I, § 2, no 7, cor. 2 de la prop. 8); par ailleurs il est clair que (v) entraîne alors (i). Nous avons donc démontré l’équivalence

(iv) $\Leftrightarrow$ (v) dans tous les cas, et aussi celle de toutes les propriétés du théorème dans le cas où $\mathfrak{J}$ est nilpotent.

E) L’implication (v) $\Rightarrow$ (i) lorsque $A$ est noethérien et $M$ idéalement séparé.

Il suffit de prouver que pour tout idéal $a$ de $A$, l’application canonique $j : a \otimes_A M \to M$ est injective (chap. I, § 2, no 3, prop. 1). Soit $x \in \mathrm{Ker}\, j$; comme $a \otimes_A M$ est séparé pour la topologie $\mathfrak{J}$-adique, il suffit de voir que pour tout entier $n > 0$, on a $x \in \mathfrak{J}^n(a \otimes_A M)$. Soit $f : \mathfrak{J}^n a \to a$ l’injection canonique ; il suffit de montrer que $x \in \mathrm{Im}(f \otimes 1_M)$; en effet, si $b \in \mathfrak{J}^n$, $a \in a$ et $m \in M$, l’image par $f \otimes 1_M$ de l’élément $(ba) \otimes m$ de $(\mathfrak{J}^n a) \otimes_A M$ est l’élément $(ba) \otimes m = b(a \otimes m)$ de $a \otimes_A M$, donc $\mathrm{Im}(f \otimes 1_M) \subset \mathfrak{J}^n(a \otimes_A M)$. En vertu du th. de Krull (§ 3, no 2, th. 2), il existe un entier $k$ tel que $a_k = a \cap \mathfrak{J}^k \subset \mathfrak{J}^n a$; si $i : a_k \to a$ est l’injection canonique, il suffira donc de montrer que $x \in \mathrm{Im}(i \otimes 1_M)$. Or, en désignant par $p : a \to a/a_k$ et $h : a/a_k \to A/\mathfrak{J}^k$ les applications canoniques, on a un diagramme commutatif

$$
\begin{array}{ccccc}
a_k \otimes_A M & \xrightarrow{i \otimes 1_M} & a \otimes_A M & \xrightarrow{p \otimes 1_M} & (a/a_k) \otimes_A M \to 0 \\
& & j \downarrow & & h \otimes 1_M \downarrow \\
& & M & \longrightarrow & (A/\mathfrak{J}^k) \otimes_A M
\end{array}
$$

dans lequel la première ligne est exacte. Il suffit de prouver que $x \in \mathrm{Ker}(p \otimes 1_M)$ et comme $x \in \mathrm{Ker}\, j$ par hypothèse, il suffira de voir que l’application $h \otimes 1_M$ est injective. Or, elle s’écrit aussi (Alg., chap. II, 3e éd., § 3, no 6, cor. 3 de la prop. 6)

$$
h \otimes 1_{M/\mathfrak{J}^k_M} : (a/a_k) \otimes_{A/\mathfrak{J}^k} (M/\mathfrak{J}^k M) \to M/\mathfrak{J}^k M
$$

et comme $h$ est injective et que, d’après (v), $M/\mathfrak{J}^k M$ est un $(A/\mathfrak{J}^k)$-module plat, cela achève la démonstration.

### 4. Applications.

#### Proposition 2 {#ac-iii-s5-prop-2 .statement}

Soient $A$ un anneau commutatif, $\mathfrak{J}$ un idéal de $A$, $B$ une $A$-algèbre commutative noethérienne telle que $\mathfrak{J}B$ soit contenu dans le radical de $B$. Alors tout $B$-module de type fini $M$ est un $A$-module idéalement séparé pour $\mathfrak{J}$.

Nous allons voir plus généralement que pour tout A-module de type fini N, $N \otimes_A M$ est séparé pour la topologie $\mathfrak{J}$-adique. En effet, $N_{(B)} = N \otimes_A B$ est un B-module de type fini, et le B-module $N \otimes_A M$ s’identifie canoniquement à $N_{(B)} \otimes_B M$ en vertu de l’associativité du produit tensoriel. Soit $\mathfrak{L}$ le radical de B ; comme $\mathfrak{J}B \subset \mathfrak{L}$, la topologie $\mathfrak{J}$-adique sur $N \otimes_A M$ est ainsi identifiée à une topologie plus fine que la topologie $\mathfrak{L}$-adique de $N_{(B)} \otimes_B M$ ; mais cette dernière topologie est séparée puisque $N_{(B)} \otimes_B M$ est un B-module de type fini (n° 1, Exemple 1), d’où la conclusion.

#### Proposition 3 {#ac-iii-s5-prop-3 .statement}

Soient A un anneau commutatif, B une A-algèbre commutative, $\mathfrak{J}$ un idéal de A, M un B-module. On suppose que B est un anneau noethérien et un A-module plat, et que M est idéalement séparé pour $\mathfrak{J}B$. Les conditions suivantes sont équivalentes :

a) M est un B-module plat.
b) M est un A-module plat et $M/\mathfrak{J}M = M/(\mathfrak{J}B)M$ est un $(B/\mathfrak{J}B)$-module plat.

Si en outre l’homomorphisme canonique $A/\mathfrak{J} \to B/\mathfrak{J}B$ est bijectif, les conditions a) et b) sont aussi équivalentes à :
c) M est un A-module plat.

La condition a) entraîne b) en vertu du chap. I, § 2, n° 7, cor. 2 et 3 à la prop. 8 et du fait que $M/\mathfrak{J}M$ est isomorphe à $M \otimes_B (B/\mathfrak{J}B)$. Supposons la condition b) satisfaite ; pour montrer que M est un B-module plat, nous allons appliquer le th. 1 du n° 2, avec A remplacé par B et $\mathfrak{J}$ par $\mathfrak{J}B$. Il suffira donc de montrer que l’application canonique $f : \mathfrak{J}B \otimes_B M \to \mathfrak{J}M$ est injective. Soient $f_1$ l’application canonique $\mathfrak{J} \otimes_A B \to \mathfrak{J}B$ et $f_2$ l’isomorphisme canonique $\mathfrak{J} \otimes_A M \to (\mathfrak{J} \otimes_A B) \otimes_B M$ ; $f \circ (f_1 \otimes 1_M) \circ f_2$ est l’application canonique $f' : \mathfrak{J} \otimes_A M \to \mathfrak{J}M$, comme on le vérifie facilement. Or $f'$ est un isomorphisme puisque M est un A-module plat, tandis que $f_1$ est un isomorphisme parce que B est plat sur A ; $f$ est donc un isomorphisme.

Soit $\rho : A/\mathfrak{J} \to B/\mathfrak{J}B$ l’homomorphisme canonique ; la structure de $(A/\mathfrak{J})$-module de $M/\mathfrak{J}M$ déduite par $\rho$ de sa structure de $(B/\mathfrak{J}B)$-module est isomorphe à celle de $M \otimes_A (A/\mathfrak{J})$. Il en résulte que si M est un A-module plat, $M/\mathfrak{J}M$ est un $(A/\mathfrak{J})$-module plat, donc aussi un (B/\mathfrak{J}B)-module plat si $\rho$ est un isomorphisme ; on a ainsi prouvé que c) $\Rightarrow b)$ dans ce cas.

#### Corollaire {#ac-iii-s5-n4-cor-1 .statement}

*Soient A un anneau commutatif noethérien, $\mathfrak{J}$ un idéal de A, $\hat{A}$ le séparé complété de A pour la topologie $\mathfrak{J}$-adique, M un $\hat{A}$-module idéalement séparé pour $\mathfrak{J}\hat{A}$. Pour que M soit un A-module plat, il faut et il suffit que M soit un $\hat{A}$-module plat.*

On sait en effet que $\hat{A}$ est un anneau noethérien (\S 3, n° 4, prop. 8) et un A-module plat (\S 3, n° 4, th. 3), que $\mathfrak{J}\hat{A} = \hat{\mathfrak{J}}$ (\S 2, n° 12, prop. 16) et que l’homomorphisme canonique $A/\mathfrak{J} \to \hat{A}/\hat{\mathfrak{J}}$ est bijectif (\S 2, n° 12, prop. 15) ; on peut donc appliquer la prop. 3.

#### Proposition 4 {#ac-iii-s5-prop-4 .statement}

*Soient A et B deux anneaux commutatifs noethériens, $h : A \to B$ un homomorphisme d’anneaux, $\mathfrak{J}$ un idéal de A, $\mathfrak{L}$ un idéal de B contenant $\mathfrak{J}B$ et contenu dans le radical de B. Soient $\hat{A}$ le séparé complété de A pour la topologie $\mathfrak{J}$-adique, $\hat{B}$ le séparé complété de B pour la topologie $\mathfrak{L}$-adique ; $h$ est continu pour ces topologies et $\hat{h} : \hat{A} \to \hat{B}$ fait donc de $\hat{B}$ une $\hat{A}$-algèbre. Soient M un B-module de type fini, $\hat{M}$ son séparé complété pour la topologie $\mathfrak{L}$-adique ; les propriétés suivantes sont équivalentes :

a) M est un A-module plat.
b) $\hat{M}$ est un A-module plat.
c) $\hat{M}$ est un $\hat{A}$-module plat.

Comme B, muni de la topologie $\mathfrak{L}$-adique, est un anneau de Zariski, $\hat{B}$ est un B-module fidèlement plat (\S 3, n° 5, prop. 9) et $\hat{M}$ est canoniquement isomorphe à $M \otimes_B \hat{B}$ (\S 3, n° 4, th. 3) ; on vérifie aussitôt que cet isomorphisme canonique est un isomorphisme de la structure de A-module de $\hat{M}$ sur la structure de A-module de $M \otimes_B \hat{B}$ déduite de celle de M. Appliquons la prop. 4 du chap. I, \S 3, n° 2 avec R remplacé par B, S par A, E par $\hat{B}$, F par M ; on voit que pour que M soit un A-module plat, il faut et il suffit que $\hat{M}$ soit un A-module plat. Par ailleurs, $\hat{M}$ est un $\hat{B}$-module de type fini et $\mathfrak{J}\hat{B}$ est contenu dans $\hat{\mathfrak{L}} = \mathfrak{L}\hat{B}$, donc dans le radical de $\hat{B}$ (\S 3, n° 4, prop. 8) ; par suite $\hat{M}$ est un $\hat{A}$-module idéalement séparé pour $\mathfrak{J}\hat{A}$ (prop. 2). Les conditions b) et c) sont donc équivalentes en vertu du cor. de la prop. 3.*

## EXERCICES {#ac-iii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
