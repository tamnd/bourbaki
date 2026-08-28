---
book: ac
book_title: Commutative Algebra
chapter: I
chapter_title: Modules plats
section: 3
section_title: Modules fidèlement plats
lang: fr
source: ac-i-iv-fr
pdf_pages: 0042-0053, 0065-0066
extraction: ocr
subsections:
    - "no": 1
      title: '**Définition des modules fidèlement plats.**'
      page: 0
      pdf_page: 42
    - "no": 2
      title: Produit tensoriel de modules fidèlement plats.
      page: 0
      pdf_page: 45
    - "no": 3
      title: Changement d’anneau.
      page: 0
      pdf_page: 46
    - "no": 4
      title: Restriction des scalaires.
      page: 0
      pdf_page: 47
    - "no": 5
      title: Anneaux fidèlement plats.
      page: 0
      pdf_page: 48
    - "no": 6
      title: Anneaux fidèlement plats et conditions de finitude.
      page: 0
      pdf_page: 50
    - "no": 7
      title: Équations linéaires sur un anneau fidèlement plat.
      page: 0
      pdf_page: 52
statements: 23
exercises: 10
content_sha256: 4b5cda87ad52435cdd5b6839e30e09b7ccd28fca67c332897a6b360a304421ca
---

## § 3. Modules fidèlement plats

### 1. **Définition des modules fidèlement plats.**

#### Proposition 1 {#ac-i-s3-prop-1 .statement}

*Soit E un A-module à droite. Les quatre propriétés suivantes sont équivalentes :*

a) *Pour qu’une suite* $N' \xrightarrow{v} N \xrightarrow{w} N''$ *de A-modules à gauche soit exacte, il faut et il suffit que la suite*

$$
E \otimes_A N' \xrightarrow{1 \otimes v} E \otimes_A N \xrightarrow{1 \otimes w} E \otimes_A N''
$$
*soit exacte*.

b) *E est plat, et pour tout A-module à gauche N, la relation* $E \otimes_A N = 0$ *entraîne* $N = 0$.

c) *E est plat, et pour tout homomorphisme* $\varphi : N' \to N$ *de A-modules à gauche, la relation* $1_E \otimes \varphi = 0$ *entraîne* $\varphi = 0$.

d) *E est plat, et pour tout idéal à gauche maximal* $m$ *de A, on a* $E \neq Em$.

Pour simplifier l’écriture, nous poserons $T(Q) = E \otimes_A Q$ pour tout A-module à gauche Q, et $T(\varphi) = 1_E \otimes \varphi$ pour tout homomorphisme $\varphi$ de A-modules à gauche.

Nous allons d’abord prouver l’équivalence de $a$, $b$ et $c$.

Prouvons que $a$ implique $b$. Si $a$ est vérifiée, il est clair que E est plat ($§\ 2$, no 3, prop. 1). D’autre part, soit N un A-module à gauche tel que $T(N) = 0$, et considérons la suite $0 \to N \to 0$; l’hypothèse $T(N) = 0$ signifie que la suite $0 \to T(N) \to 0$ est exacte. Par $a$, la suite $0 \to N \to 0$ est exacte, d’où $N = 0$.

Montrons que $b$ implique $c$. Supposons $b$ vérifiée, et soient $\varphi : N' \to N$ un homomorphisme, I son image. Comme l’image de $T(\varphi)$ s’identifie à $T(I)$ ($§\ 2$, no 3, Remarque 2), l’hypothèse $T(\varphi) = 0$ entraîne $T(I) = 0$, donc $I = 0$ d’après $b$ et par suite $\varphi = 0$.

Démontrons que $c$ entraîne $a$. Supposons donc $c$ vérifiée et considérons une suite

$$(1)$$
$$
N' \xrightarrow{\varphi} N \xrightarrow{\omega} N''
$$

d’homomorphismes de A-modules à gauche, et la suite correspondante

$$(2)$$
$$
T(N') \xrightarrow{T(\varphi)} T(N) \xrightarrow{T(\omega)} T(N'')
$$

Si la suite (1) est exacte, il en est de même de (2), puisque E est plat ($§\ 2$, no 3, prop. 1). Inversement, si (2) est exacte, on a d’abord $T(\omega \circ \varphi) = T(\omega) \circ T(\varphi) = 0$, donc $\omega \circ \varphi = 0$ par hypothèse. Posons $I = \varphi(N')$ et $K = \omega^{-1}(0)$; on a $I \subset K$ d’après ce qui précède. Considérons la suite exacte

$$
0 \to I \xrightarrow{i} K \xrightarrow{p} K/I \to 0
$$

$i$ et $p$ étant les applications canoniques. Comme E est plat, la suite

$$
0 \to T(I) \xrightarrow{T(i)} T(K) \xrightarrow{T(p)} T(K/I) \to 0
$$

est exacte, autrement dit, $T(K/I)$ est isomorphe à $T(K)/T(I)$, qui est 0 par hypothèse, puisque $T(I)$ (resp. $T(K)$) s’identifie à l’image de $T(\varphi)$ (resp. au noyau de $T(\omega)$) ($§\ 2$, no 3, Remarque 2). Mais la relation $T(p) = 0$ entraîne $p = 0$ par hypothèse, donc on a $K = I$, ce qui prouve que la suite (1) est exacte.

Démontrons enfin l’équivalence de $b$ et $d$. Si $b$ est vérifiée, on a $E/E_m = E \otimes_A (A_s/m) \neq 0$ puisque $A_s/m \neq 0$; d’où $d$. Inversement, supposons $d$ vérifiée; tout idéal à gauche $a \neq A$ de A est contenu dans un idéal à gauche maximal $m$ (Alg., chap. I, § 8, n° 7, th. 2), donc l’hypothèse E ≠ Em entraîne E ≠ Ea, autrement dit E ⊗_A (A_s/a) ≠ 0. En d’autres termes, pour tout A-module à gauche monogène N ≠ 0, on a T(N) ≠ 0. Si maintenant N est un A-module à gauche ≠ 0 quelconque, il contient un sous-module monogène N′ ≠ 0 ; puisque E est plat, T(N′) s’identifie à un sous-groupe de T(N) ; on vient de voir que T(N′) ≠ 0, donc T(N) ≠ 0.

C. Q. F. D.

#### Définition 1 {#ac-i-s3-def-1 .statement}

On dit qu’un A-module à droite E est fidèlement plat s’il vérifie les quatre propriétés équivalentes de la prop. 1.

On définit de même les A-modules à gauche fidèlement plats ; il est clair que pour qu’un A-module à gauche E soit fidèlement plat, il faut et il suffit que E, considéré comme A^0-module à droite, soit fidèlement plat.

#### Remarque {#ac-i-s3-n1-rem-1 .statement}

Si E est un A-module fidèlement plat, E est un A-module fidèle : en effet, si un élément a ∈ A est tel que xa = 0 pour tout x ∈ E, l’homothétie h : b → ba dans A est telle que 1_E ⊗ h = 0 ; d’où h = 0 par la propriété c) de la prop. 1, c’est-à-dire a = 0 puisque A possède un élément unité.

#### Exemple 1 {#ac-i-s3-n1-exa-1 .statement}

La somme directe d’un module plat et d’un module fidèlement plat est un module fidèlement plat en vertu de la propriété d) de la prop. 1 et du § 2, n° 3, prop. 2.

#### Exemple 2 {#ac-i-s3-n1-exa-2 .statement}

Comme A_s est fidèlement plat en vertu du critère d) de la prop. 1 et du § 2, n° 4, Exemple 1, il résulte de 1) que tout module libre non réduit à 0 est fidèlement plat. Par contre, il existe des facteurs directs non nuls de modules libres (autrement dit, des modules projectifs non nuls) qui sont fidèles et ne sont pas fidèlement plats (exerc. 2).

#### Exemple 3 {#ac-i-s3-n1-exa-3 .statement}

Soit A un anneau principal. Pour qu’un A-module E soit fidèlement plat, il faut et il suffit qu’il soit sans torsion et que E ≠ Ep pour tout élément extrémal (Alg., chap. VII, § 1, n° 3) p de A ; cela résulte aussitôt du § 2, n° 4, prop. 3 et du critère d) de la prop. 1.

#### Exemple 4 {#ac-i-s3-n1-exa-4 .statement}

L’exemple 3) montre que le $\mathbf{Z}$-module $\mathbf{Q}$ est un module plat et fidèle, mais non fidèlement plat.

#### Proposition 2 {#ac-i-s3-prop-2 .statement}

Soient E un A-module à droite fidèlement plat, et u : N' → N un homomorphisme de A-modules à gauche. Pour que u soit injectif (resp. surjectif, bijectif), il faut et il suffit que $1_E \otimes u : E \otimes_A N' \to E \otimes_A N$ le soit.
C'est une conséquence immédiate du critère a) de la prop. 1.

#### Proposition 3 {#ac-i-s3-prop-3 .statement}

Soit $0 \to E' \to E \to E'' \to 0$ une suite exacte de A-modules à droite. On suppose que E' et E'' sont plats, et que l'un d'eux est fidèlement plat. Alors E est fidèlement plat.
On sait déjà que E est plat (§ 2, n° 5, prop. 5). On va vérifier que E possède la propriété b) de la prop. 1. Soit N un A-module à gauche. Comme E'' est plat, on a la suite exacte
$$
0 \to E' \otimes_A N \to E \otimes_A N \to E'' \otimes_A N \to 0
$$
(§ 2, n° 5, prop. 4). Si $E \otimes_A N = 0$, on en conclut que $E' \otimes_A N$ et $E'' \otimes_A N$ sont nuls ; comme l'un des modules E', E'' est fidèlement plat, cela entraîne $N = 0$.

### 2. Produit tensoriel de modules fidèlement plats.

#### Proposition 4 {#ac-i-s3-prop-4 .statement}

Soient R, S deux anneaux, E un R-module à droite, F un (R, S)-bimodule. On suppose que E est fidèlement plat. Alors, pour que F soit un S-module plat (resp. fidèlement plat), il faut et il suffit que $E \otimes_R F$ le soit.
1° Si F est plat, $E \otimes_R F$ est plat (§ 2, n° 7, prop. 8).
2° Supposons $E \otimes_R F$ plat, et soit $\nu : N' \to N$ un homomorphisme injectif de S-modules à gauche. L'homomorphisme $1_E \otimes 1_F \otimes \nu : E \otimes_R F \otimes_S N' \to E \otimes_R F \otimes_S N$ est alors injectif (§ 2, n° 3, prop. 1). On déduit du n° 1, prop. 2 que $1_F \otimes \nu : F \otimes_S N' \to F \otimes_S N$ est injectif ; donc F est un S-module plat (§ 2, n° 3, prop. 1).
3° Supposons F fidèlement plat, et soit N un S-module à gauche tel que $E \otimes_R F \otimes_S N = 0$. Puisque E est fidèlement plat, cela entraîne $F \otimes_S N = 0$, d'où $N = 0$ puisque F est fidèlement plat ; cela prouve que $E \otimes_R F$ est fidèlement plat.
4° Supposons $E \otimes_R F$ fidèlement plat, et soit N un S-module à gauche tel que $F \otimes_S N = 0$. On a $E \otimes_R F \otimes_S N = 0$, d'où $N = 0$, ce qui montre que F est fidèlement plat.

#### Corollaire {#ac-i-s3-n2-cor-1 .statement}

Soient C un anneau commutatif, E et F deux C-modules fidèlement plats. Alors le C-module $E \otimes_C F$ est fidèlement plat.

On applique la prop. 4 avec $R = S = C$.

### 3. Changement d’anneau.

#### Proposition 5 {#ac-i-s3-prop-5 .statement}

Soit $\rho$ un homomorphisme d’un anneau A dans un anneau B. Si E est un A-module à droite fidèlement plat, le B-module à droite $\rho^*(E) = E_{(B)} = E \otimes_A B$ est fidèlement plat.

On applique la prop. 4 du n° 2 avec $R = A, S = F = B$, en remarquant que le B-module $B_d$ est fidèlement plat.

#### Corollaire {#ac-i-s3-n3-cor-1 .statement}

Si E est un A-module à droite fidèlement plat, et si $a$ est un idéal bilatère de A, le $(A/a)$-module à droite $E/Ea$ est fidèlement plat.

On applique la prop. 5 avec $B = A/a$, $\rho$ étant l’homomorphisme canonique.

#### Proposition 6 {#ac-i-s3-prop-6 .statement}

Soient A un anneau commutatif, B une algèbre sur A, $\rho : a \to a.1$ l’homomorphisme canonique de A dans B. Supposons que B soit un A-module fidèlement plat. Alors, pour qu’un A-module E soit plat (resp. fidèlement plat), il faut et il suffit que le B-module à droite $E_{(B)} = E \otimes_A B$ soit plat (resp. fidèlement plat).

1° Si E est plat (resp. fidèlement plat), $E_{(B)}$ est plat (resp. fidèlement plat) en vertu du § 2, n° 7, cor. 2 de la prop. 8 (resp. de la prop. 5).

2° Supposons que $E_{(B)}$ soit plat, et soit $\nu : N' \to N$ un homomorphisme injectif de A-modules. En vertu du § 2, n° 7, cor. 3, le A-module $E \otimes_A B$ est plat, donc l’homomorphisme $1_E \otimes 1_B \otimes \nu : E \otimes_A B \otimes_A N' \to E \otimes_A B \otimes_A N$ est injectif. Comme les structures de A-module à droite et de A-module à gauche sur B coïncident, cet homomorphisme s’identifie à

$$
1_E \otimes \nu \otimes 1_B : E \otimes_A N' \otimes_A B \to E \otimes_A N \otimes_A B.
$$

Comme B est un A-module fidèlement plat, on en déduit que

$1_E \otimes \varphi : E \otimes_A N' \to E \otimes_A N$ est injectif (n° 1, prop. 2), ce qui montre que E est plat.

3° Supposons enfin que $E_{(B)}$ soit fidèlement plat. Tout d’abord E est plat en vertu du 2°. Soit en outre N un A-module tel que $E \otimes_A N = 0$. On a alors $E \otimes_A N \otimes_A B = 0$, d’où, puisque les structures de A-module à droite et de A-module à gauche sur B coïncident, $E \otimes_A B \otimes_A N = 0$, ce qui s’écrit aussi $(E \otimes_A B) \otimes_B (B \otimes_A N) = 0$. Comme $E_{(B)}$ est un B-module fidèlement plat, cela entraîne $B \otimes_A N = 0$ (n° 1, prop. 1), d’où $N = 0$ puisque B est un A-module fidèlement plat (n° 1, prop. 1).

C. Q. F. D.

### 4. Restriction des scalaires.

#### Proposition 7 {#ac-i-s3-prop-7 .statement}

Soient A, B deux anneaux, $\rho$ un homomorphisme de A dans B. Soit E un B-module à droite fidèlement plat. Pour que $\rho_*(E)$ soit un A-module à droite plat (resp. fidèlement plat), il faut et il suffit que B soit un A-module à droite plat (resp. fidèlement plat).

On applique la prop. 4 du n° 2, en remplaçant R, S, E, F respectivement par B, A, E, B, la structure de A-module à droite de B étant définie par $\rho$ ; on voit ainsi que B est un A-module plat (resp. fidèlement plat) si et seulement si $E \otimes_B B = \rho_*(E)$ est un A-module plat (resp. fidèlement plat).

#### Remarque {#ac-i-s3-n4-rem-1 .statement}

1° La prop. 7 montre que pour que B soit un A-module fidèlement plat, il suffit qu’il existe un B-module fidèlement plat qui soit aussi un A-module fidèlement plat.

2° Soient A, B, C trois anneaux, $\rho : A \to B$, $\sigma : B \to C$ deux homomorphismes d’anneaux. La prop. 7 montre que si C est un B-module fidèlement plat et B un A-module fidèlement plat, alors C est un A-module fidèlement plat. Si C est un B-module fidèlement plat et un A-module fidèlement plat, alors B est un A-module fidèlement plat (les modules étant pris à droite, pour fixer les idées). Par contre B et C peuvent être des A-modules fidèlement plats sans que C soit un B-module fidèlement plat (exerc. 7).

### 5. Anneaux fidèlement plats.

#### Proposition 8 {#ac-i-s3-prop-8 .statement}

Soient A, B deux anneaux, $\rho$ un homomorphisme de A dans B. On suppose qu’il existe un B-module à droite E tel que $\rho_*(E)$ soit un A-module fidèlement plat. Alors :

(i) Pour tout A-module à gauche F, l’homomorphisme canonique $j : F \to F_{(B)} = B \otimes_A F$ (tel que $j(x) = 1 \otimes x$ pour $x \in F$) est injectif.

(ii) Pour tout idéal à gauche $a$ de A, on a $\rho^{-1}(Ba) = a$.

(iii) L’homomorphisme $\rho$ est injectif.

(iv) Pour tout idéal à gauche maximal $m$ de A, il existe un idéal à gauche maximal $n$ de B tel que $\rho^{-1}(n) = m$.

Démontrons (i). On sait (Alg., chap. II, 3e éd., § 5, no 2, cor. de la prop. 5) que pour tout B-module à droite M, le A-homomorphisme canonique $i : M \to \rho_*(M) \otimes_A B = \rho^*(\rho_*(M))$ défini par $i(y) = y \otimes 1$ est injectif et que le A-module $i(M)$ est facteur direct de $\rho_*(M) \otimes_A B$. Donc, pour tout A-module à gauche F,

$$
i \otimes 1_F : \rho_*(M) \otimes_A F \to \rho_*(M) \otimes_A B \otimes_A F
$$

est injectif (\S 2, no 1, lemme 2). Si on prend $M = E$, on en déduit (puisque $i \otimes 1_F = 1_M \otimes j$) que $j$ est injectif (no 1, prop. 2).

L’assertion (ii) résulte de (i) en prenant $F = A_s/a$, et (iii) résulte de (ii) en prenant $a = \{0\}$.

Enfin, si $m$ est un idéal à gauche maximal de A, on a $\rho^{-1}(Bm) = m$ en vertu de (ii), et par suite $Bm \neq B$. Il existe donc un idéal maximal à gauche $n$ de B contenant $Bm$ (Alg., chap. I, § 8, no 7, th. 2); on a $m \subset \rho^{-1}(n)$ et comme $\rho(1) \notin n$, 1 n’appartient pas à $\rho^{-1}(n)$. Par suite $\rho^{-1}(n) = m$.

Lorsque A et B vérifient les conditions de la prop. 8, on identifie d’ordinaire A à un sous-anneau de B au moyen de $\rho$.

#### Corollaire {#ac-i-s3-n5-cor-1 .statement}

Sous les hypothèses de la prop. 8, si B est noethérien (resp. artinien) à gauche, il en est de même de A.

En effet, si $(a_n)$ était une suite croissante (resp. décroissante) non stationnaire d’idéaux à gauche de A, la suite $(Ba_n)$ d’idéaux de B serait croissante (resp. décroissante) non stationnaire puisque $\rho^{-1}(Ba_n) = a_n$, contrairement à l’hypothèse.

*Remarque 1). — Lorsque A et B sont commutatifs, nous verrons au chap. II, § 2, n° 5, cor. 4 de la prop. 11, que l’hypothèse de la prop. 8 entraîne que pour tout idéal premier $p$ de A, il existe un idéal premier $q$ de B tel que $\rho^{-1}(q) = p$ (ou $p = A \cap q$ quand on identifie A à un sous-anneau de B).*

La prop. 8 s’applique notamment lorsque B est lui-même un A-module fidèlement plat. Mais on a dans ce cas la proposition plus précise suivante :

#### Proposition 9 {#ac-i-s3-prop-9 .statement}

*Soient A, B deux anneaux, $\rho$ un homomorphisme de A dans B. Les cinq propriétés suivantes sont équivalentes :*

a) *Le A-module à droite B est fidèlement plat.*

b) *L’homomorphisme $\rho$ est injectif et le A-module à droite $B/\rho(A)$ est plat.*

c) *Le A-module à droite B est plat, et pour tout A-module à gauche F, l’homomorphisme canonique $x \to 1 \otimes x$ de F dans $B \otimes_A F$ est injectif.*

d) *Le A-module à droite B est plat, et pour tout idéal à gauche $a$ de A, on a $\rho^{-1}(Ba) = a$.*

e) *Le A-module à droite B est plat, et pour tout idéal à gauche maximal $m$ de A, il existe un idéal à gauche maximal $n$ de B tel que $\rho^{-1}(n) = m$.*

D’après la prop. 8, a) implique chacune des propriétés c), d), e). D’autre part, si e) est vérifiée, on a $Bm \neq B$ pour tout idéal à gauche maximal $m$ de A (puisqu’il existe un idéal à gauche maximal $n$ de B tel que $Bm \subset n$), et B est un A-module fidèlement plat par le critère d) du n° 1, prop. 1 ; donc e) entraîne a).

Nous allons maintenant prouver que c) $\Rightarrow$ d) $\Rightarrow$ b) $\Rightarrow$ a), ce qui achèvera la démonstration. En premier lieu, c) entraîne d), en prenant $F = A_s/a$ dans c). Si d) est vérifiée, en prenant $a = \{0\}$, on voit que $\rho$ est injectif ; il résulte de d) et du § 2, n° 6, cor. de la prop. 7, que $B/\rho(A)$ est un A-module à droite plat, donc d) entraîne b). Enfin, si b) est vérifiée, la prop. 3 du n° 1 appliquée à la suite exacte

$$
0 \to A_d \xrightarrow{\rho} B \to B/\rho(A) \to 0
$$

montre que B est un A-module à droite fidèlement plat, puisque $A_d$ est fidèlement plat.

C. Q. F. D.

*Remarque 2). — Lorsque A et B sont commutatifs, nous verrons au chap. II, § 2, n° 5, cor. 4 de la prop. 11 que les conditions de la prop. 9 sont équivalentes à la suivante :

f) B est un A-module plat, et pour tout idéal premier $p$ de A, il existe un idéal $q$ de B tel que $\rho^{-1}(q) = p.$*

Sous les conditions de la prop. 9, identifions A à un sous-anneau de B au moyen de $\rho$. La relation $\rho^{-1}(Ba) = a$ s’écrit alors $A \cap Ba = a$. D’autre part, si F est un A-module à gauche, on identifie F à son image dans $B \otimes_A F$ par l’application canonique $x \to 1 \otimes x$; si X est un sous-groupe additif de F, on note alors BX le sous-B-module à gauche de $B \otimes_A F$ engendré par X. Avec ces notations, on a :

#### Proposition 10 {#ac-i-s3-prop-10 .statement}

Soient B un anneau et A un sous-anneau de B tel que B soit un A-module à droite fidèlement plat. Soient F un A-module à gauche, F', F'' deux sous-modules de F. Alors :
(i) L’application canonique $B \otimes_A F' \to B \otimes_A F$ induit un isomorphisme de $B \otimes_A F'$ sur $BF'$.
(ii) On a $F \cap BF' = F'$.
(iii) On a $B(F' + F'') = BF' + BF''$.
(iv) On a $B(F' \cap F'') = BF' \cap BF''$.

En effet, comme B est un A-module à droite plat, l’application canonique $B \otimes_A F' \to B \otimes_A F$ est injective ; compte tenu des identifications faites, son image est $BF'$, ce qui démontre (i). L’assertion (ii) résulte du § 2, n° 6, prop. 7, appliquée avec $E = B$, $E' = A$, et compte tenu des formules $A \otimes_A F = F$ et $A \otimes_A F' = F'$. L’assertion (iii) est triviale, et (iv) résulte du § 2, n° 6, prop. 6.

### 6. Anneaux fidèlement plats et conditions de finitude.

#### Proposition 11 {#ac-i-s3-prop-11 .statement}

Soient B un anneau et A un sous-anneau de B tel que B soit un A-module à droite fidèlement plat. Pour qu’un

A-module à gauche F soit de type fini (resp. de présentation finie), il faut et il suffit que le B-module $B \otimes_A F$ soit de type fini (resp. de présentation finie).

1° Sans hypothèse sur B, il est clair que si F est un A-module à gauche de type fini, $B \otimes_A F$ est un B-module à gauche de type fini. Inversement, si $B \otimes_A F$ est un B-module de type fini, il est engendré par un nombre fini d’éléments de la forme $1 \otimes x_i$ avec $x_i \in F$; si M est le sous-A-module de F engendré par les $x_i$, et j l’injection canonique $M \to F$, $1_B \otimes j : B \otimes_A M \to B \otimes_A F$ est un homomorphisme surjectif, donc j est surjectif (n° 1, prop. 2), ce qui prouve que F est de type fini.

2° Si F admet une présentation finie, il en est de même de $B \otimes_A F$ sans hypothèse sur B (\S 2, n° 8). Reste à prouver que si $B \otimes_A F$ admet une présentation finie, il en est de même de F. On sait déjà par 1° que F est de type fini, donc il existe un homomorphisme surjectif $u : L \to F$, où L est un A-module libre de type fini. Soit R le noyau de u, de sorte que $B \otimes_A R$ s’identifie au noyau de l’homomorphisme surjectif $1_B \otimes u : B \otimes_A L \to B \otimes_A F$ (\S 2, n° 3, Remarque 2). Comme $B \otimes_A F$ admet une présentation finie par hypothèse, on en conclut (\S 2, n° 8, lemme 9) que $B \otimes_A R$ est de type fini ; il résulte alors de 1° que R est un A-module de type fini, et par suite F admet une présentation finie.

#### Proposition 12 {#ac-i-s3-prop-12 .statement}

Soient B un anneau et A un sous-anneau commutatif du centre de B tel que B soit un A-module fidèlement plat. Pour qu’un A-module F soit projectif et de type fini, il faut et il suffit que $B \otimes_A F$ soit un B-module à gauche projectif de type fini.

La condition est évidemment nécessaire sans hypothèses sur A ni B (Alg., chap. II, 3e éd., § 5, n° 1, cor. de la prop. 4); prouvons qu’elle est suffisante. Un module projectif de type fini admettant une présentation finie (\S 2, n° 8, lemme 8), l’hypothèse entraîne que F admet une présentation finie en vertu de la prop. 11, donc, pour tout A-module M on a un isomorphisme canonique

$$
\omega : B \otimes_A \operatorname{Hom}_A(F, M) \to \operatorname{Hom}_B(B \otimes_A F, B \otimes_A M)
$$

(§ 2, no 10, prop. 11). Soit alors $\varphi : M \to M''$ un homomorphisme surjectif de A-modules et considérons le diagramme commutatif

$$
\begin{array}{ccc}
B \otimes_A \mathrm{Hom}_A(F, M) & \xrightarrow{\omega} & \mathrm{Hom}_B(B \otimes_A F, B \otimes_A M) \\
\downarrow_{1_B \otimes \mathrm{Hom}(1_F, \varphi)} & & \downarrow_{\mathrm{Hom}(1_B \otimes_F, 1_B \otimes \varphi)} \\
B \otimes_A \mathrm{Hom}_A(F, M'') & \xrightarrow{\omega} & \mathrm{Hom}_B(B \otimes_A F, B \otimes_A M'')
\end{array}
$$

Comme $1_B \otimes \varphi$ est surjectif, et que $B \otimes_A F$ est supposé projectif, $\mathrm{Hom}(1_B \otimes_F, 1_B \otimes \varphi)$ est surjectif (Alg., chap. II, 3e éd., § 2, no 2, prop. 4), et il en est donc de même de $1_B \otimes \mathrm{Hom}(1_F, \varphi)$. Mais comme B est un A-module fidèlement plat, $\mathrm{Hom}(1_F, \varphi)$ est lui-même surjectif (no 1, prop. 2), donc F est un A-module projectif (Alg., chap. II, 3e éd., § 2, no 2, prop. 4).

### 7. Équations linéaires sur un anneau fidèlement plat.

Soient B un anneau, A un sous-anneau de B. Nous dirons que le couple (A, B) a la propriété d’extension linéaire s’il vérifie la condition suivante :

(E) Toute solution $(y_k)_{1 \leq k \leq n}$, formée d’éléments de B, d’un système d’équations linéaires

$$
\sum_{k=1}^n y_k c_{ki} = d_i \quad (1 \leq i \leq m)
$$
dont les coefficients $c_{ki}$ et les seconds membres $d_i$ appartiennent à A, est de la forme
$$
y_k = x_k + \sum_{j=1}^p b_j z_{jk} \quad (1 \leq k \leq n)
$$
où $(x_k)$ est une solution de (3) formée d’éléments de A, les $b_j$ appartiennent à B et chacun des $(z_{jk})_{1 \leq k \leq n}$ est une solution du système linéaire homogène associé à (3), formée d’éléments de A.

#### Proposition 13 {#ac-i-s3-prop-13 .statement}

Soit A un sous-anneau d’un anneau B. Pour que le couple (A, B) vérifie la propriété d’extension linéaire, il faut et il suffit que B soit un A-module à droite fidèlement plat.

La condition est suffisante. En effet, comme B est un A-module plat, toute solution à éléments dans B du système linéaire homogène associé à (3) est combinaison linéaire à coefficients dans B de solutions formées d’éléments de A (§ 2, no 11, cor. 2 de la prop. 13). Tout revient donc à prouver que l’existence d’une solution de (3) à éléments dans B entraîne l’existence d’une solution à éléments dans A. Or si on pose $c_k = (c_{ki})_{1 \leq i \leq m} \in A_s^m$, $d = (d_i) \in A_s^m$, le système (3) équivaut à l’équation $\sum_{k=1}^n y_k \otimes c_k = 1 \otimes d$ dans $B \otimes_A A_s^m = B_s^m$. Autrement dit, si M est le sous-A-module de $A_s^m$ engendré par les $c_k (1 \leq k \leq n)$, l’existence de la solution $(y_k)$ de (3) équivaut (avec les identifications faites au no 5) à la relation $d \in BM \cap A_s^m$; mais comme $BM \cap A_s^m = M$ (no 5, prop. 10, (ii)), elle entraîne $d \in M$, c’est-à-dire l’existence d’une solution $(x_k)$ du système (3) à éléments dans A.

La condition est nécessaire. Supposons en effet que (A, B) vérifie la propriété d’extension linéaire ; on sait déjà que B est un A-module à droite plat (§ 2, no 11, cor. 2 de la prop. 13) ; prouvons que pour tout idéal à gauche $\alpha$ de A, on a $B \alpha \cap A = \alpha$, ce qui démontrera que B est un A-module à droite fidèlement plat (no 5, prop. 9, d)). Or, soit $x \in B \alpha \cap A$; il existe par hypothèse des $y_i \in B$ et des $a_i \in \alpha$ tels que $\sum_i y_i a_i = x$; la propriété (E) appliquée à cette équation linéaire à coefficients et second membre dans A montre qu’il existe des $x_i \in A$ tels que $x = \sum_i x_i a_i$, donc $x \in \alpha$.

C. Q. F. D.

## EXERCICES {#ac-i-s3-exercises}

See the [exercises for § 3](exercises/s3/).
