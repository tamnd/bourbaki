---
book: ac
book_title: Commutative Algebra
chapter: I
chapter_title: Modules plats
section: 2
section_title: Modules plats
lang: fr
source: ac-i-iv-fr
pdf_pages: 0020-0042, 0058-0065
extraction: ocr
subsections:
    - "no": 1
      title: Rappel sur les produits tensoriels.
      page: 0
      pdf_page: 20
    - "no": 2
      title: '*Modules M-plats*.'
      page: 0
      pdf_page: 21
    - "no": 3
      title: Modules plats.
      page: 0
      pdf_page: 24
    - "no": 4
      title: Exemples de modules plats.
      page: 0
      pdf_page: 26
    - "no": 5
      title: Platitude des modules quotients.
      page: 0
      pdf_page: 28
    - "no": 6
      title: Propriétés d’intersection.
      page: 0
      pdf_page: 30
    - "no": 7
      title: Produits tensoriels de modules plats.
      page: 0
      pdf_page: 32
    - "no": 8
      title: Modules de présentation finie.
      page: 0
      pdf_page: 33
    - "no": 9
      title: '*Extension des scalaires dans les modules d’homomorphismes.*'
      page: 0
      pdf_page: 35
    - "no": 10
      title: '*Extension des scalaires : cas des anneaux commutatifs.*'
      page: 0
      pdf_page: 36
    - "no": 11
      title: Interprétation de la platitude en termes de relations (*).
      page: 0
      pdf_page: 39
statements: 41
exercises: 24
content_sha256: af91402a2ec2c2ed81a7bff1a5e8ce758f4c5169ec4ecce1812964a448251d8c
---

## § 2. Modules plats (*)

### 1. Rappel sur les produits tensoriels.

Soient $A$ un anneau, $E$ un $A$-module à droite, $M$ un $A$-module à gauche. On a défini en Alg., chap. II, 3e éd., § 3, n° 1, le produit tensoriel $E \otimes_A M$, qui est un $\mathbf{Z}$-module. Si $E'$ (resp. $M'$) est un $A$-module à droite (resp. à gauche) et $u : E \to E'$ (resp. $\varphi : M \to M'$) un homomorphisme, on a aussi défini (loc. cit., n° 2) un $\mathbf{Z}$-homomorphisme

$$
u \otimes \varphi : E \otimes_A M \to E' \otimes_A M'.
$$

#### Lemme 1 {#ac-i-s2-lem-1 .statement}

Soit $M' \xrightarrow{\varphi} M \xrightarrow{w} M'' \to 0$ une suite exacte de $A$-modules à gauche, et soit $E$ un $A$-module à droite. La suite

$$
E \otimes_A M' \xrightarrow{1 \otimes \varphi} E \otimes_A M \xrightarrow{1 \otimes w} E'' \otimes_A M \longrightarrow 0
$$

est alors une suite exacte de groupes commutatifs.

(*) Signalons aux lecteurs déjà au courant de l’Algèbre homologique qu’ils trouveront au § 4 d’autres caractérisations des modules plats.

C’est le cor. de la prop. 5 d’Alg., chap. II, 3e éd., § 3, n° 6.

On en conclut que pour tout homomorphisme $u : M \to N$ de A-modules à gauche, $E \otimes_A (\mathrm{Coker}\ u)$ s’identifie canoniquement à $\mathrm{Coker}\ (1_E \otimes u)$, comme le montre le lemme 1 appliqué à la suite exacte
$$
M \xrightarrow{u} N \to \mathrm{Coker}\ u \to 0.
$$

Les notations étant celles du lemme 1, on sait (loc. cit.) que si $\nu$ est injectif, c’est-à-dire si la suite $0 \to M' \xrightarrow{\nu} M \xrightarrow{\nu} M'' \to 0$ est exacte, il n’en résulte pas nécessairement que $1_E \otimes \nu$ soit injectif et l’on ne peut donc pas en général identifier $E \otimes_A M'$ à un sous-groupe de $E \otimes_A M$. Rappelons toutefois (Alg., chap. II, 3e éd., § 3, n° 7, cor. 5 de la prop. 7) le résultat suivant :

#### Lemme 2 {#ac-i-s2-lem-2 .statement}

*Si $\nu : M' \to M$ est injectif et si $\nu(M')$ est facteur direct de $M$, l’homomorphisme $1_E \otimes \nu$ est injectif, et son image est facteur direct de $E \otimes_A M$.*

### 2. *Modules M-plats*.

#### Définition 1 {#ac-i-s2-def-1 .statement}

*Soient $A$ un anneau, $E$ un $A$-module à droite et $M$ un $A$-module à gauche. On dit que $E$ est plat pour $M$ (ou $M$-plat) si, pour tout $A$-module à gauche $M'$ et tout homomorphisme injectif $\nu : M' \to M$, l’homomorphisme $1_E \otimes \nu : E \otimes_A M' \to E \otimes_A M$ est injectif.*

On définit de même, pour tout $A$-module à droite $N$, la notion de *module à gauche $N$-plat*. Dire qu’un $A$-module à droite $E$ est plat pour un $A$-module à gauche $M$ équivaut à dire que $E$, considéré comme $A^0$-module à gauche (on rappelle que $A^0$ désigne l’anneau opposé de $A$), est plat pour le $A^0$-module à droite $M$.

#### Lemme 3 {#ac-i-s2-lem-3 .statement}

*Pour qu’un $A$-module à droite $E$ soit $M$-plat, il suffit que pour tout sous-module de type fini $M'$ de $M$, l’homomorphisme canonique $1_E \otimes j : E \otimes_A M' \to E \otimes_A M$ ( $j$ étant l’injection canonique $M' \to M$) soit injectif.*

En effet, supposons cette condition vérifiée et soit N un sous-module quelconque de M. Supposons que l’image canonique dans $E \otimes_A M$ d’un élément $z = \sum_i x_i \otimes y_i \in E \otimes_A N$ ($x_i \in E,\ y_i \in N$) soit nulle, et soit $M'$ le sous-module de type fini de N engendré par les $y_i$; comme par hypothèse l’application composée $E \otimes_A M' \to E \otimes_A N \to E \otimes_A M$ est injective, la somme $z' = \sum_i x_i \otimes y_i$, considérée comme élément de $E \otimes_A M'$, est nulle. Comme $z$ est l’image de $z'$, on a aussi $z = 0$, d’où le lemme.

#### Lemme 4 {#ac-i-s2-lem-4 .statement}

*Soient E un A-module à droite et M un A-module à gauche tel que E soit M-plat. Si N est, soit un sous-module, soit un module quotient de M, alors E est N-plat.*

Le cas où N est un sous-module est facile, car si N’ est un sous-module de N, l’homomorphisme composé

$$
E \otimes_A N' \to E \otimes_A N \to E \otimes_A M
$$

est injectif, donc il en est de même de $E \otimes_A N' \to E \otimes_A N$. Supposons donc que N soit un module quotient de M, c’est-à-dire qu’il existe une suite exacte $0 \to R \xrightarrow{i} M \xrightarrow{p} N \to 0$. Soient N’ un sous-module de N, et $M' = p^{-1}(N')$. Notons $i'$ l’application de R dans M’ ayant même graphe que $i$, $p'$ la surjection $M' \to N'$, ayant même graphe que la restriction de $p$ à $M'$, $r$ l’application identique de R sur R, $m$ l’injection canonique $M' \to M$, $n$ l’injection canonique $N' \to N$. Le diagramme

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & R & \xrightarrow{i'} & M' & \xrightarrow{p'} & N' & \longrightarrow & 0 \\
& & r \downarrow & & m \downarrow & & n \downarrow & & \\
0 & \longrightarrow & R & \xrightarrow{i} & M & \xrightarrow{p} & N & \longrightarrow & 0
\end{array}
$$

est commutatif, et ses lignes sont exactes.

Pour simplifier l’écriture, posons $T(Q) = E \otimes_A Q$ pour tout A-module à gauche Q et $T(\varphi) = 1_E \otimes \varphi$ pour tout homomorphisme $\varphi$ de A-modules à gauche. Le diagramme

$$
\begin{array}{ccccccccc}
T(R) & \xrightarrow{T(i')} & T(M') & \xrightarrow{T(p')} & T(N') & \longrightarrow & 0 \\
T(r) \downarrow & & T(m) \downarrow & & T(n) \downarrow & & \\
T(R) & \xrightarrow{T(i)} & T(M) & \xrightarrow{T(p)} & T(N) & \longrightarrow & 0
\end{array}
$$

est commutatif, et ses lignes sont exactes en vertu du no 1, lemme 1.

n° 2

De plus, puisque E est M-plat, l’homomorphisme T(m) est injectif. Comme T(r) et T(p') sont surjectifs, il résulte du § 1, n° 4, cor. 2 de la prop. 2, que T(n) est injectif, ce qui démontre le lemme.

#### Lemme 5 {#ac-i-s2-lem-5 .statement}

Soit $(M_i)_{i \in I}$ une famille de A-modules à gauche, $M = \bigoplus_{i \in I} M_i$ leur somme directe, et E un A-module à droite. Si, pour tout $i \in I$, E est plat pour $M_i$, alors E est plat pour M.

a) Supposons d’abord que $I = \{1, 2\}$, et soit $M'$ un sous-module de $M = M_1 \oplus M_2$, $M_1$ et $M_2$ étant canoniquement identifiés à des sous-modules de M. Désignons par $M'_1$ l’intersection $M' \cap M_1$, par $M'_2$ l’image de $M'$ dans $M_2$ par la projection canonique $p$ de M sur $M_2$. On a un diagramme

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & M'_1 & \xrightarrow{i'} & M' & \xrightarrow{p'} & M'_2 & \longrightarrow & 0 \\
& & v_1 \downarrow & & v \downarrow & & v_2 \downarrow & & \\
0 & \longrightarrow & M_1 & \xrightarrow{i} & M & \xrightarrow{p} & M_2 & \longrightarrow & 0
\end{array}
$$

où $v_1$, $v$, $v_2$, $i$, $i'$ sont les injections canoniques et $p'$ l’application ayant même graphe que la restriction de $p$ à $M'$, qui est surjective. On vérifie aussitôt que ce diagramme est commutatif et que ses lignes sont exactes. Les notations T(Q) et T($v$) ayant le même sens que dans la démonstration du lemme 4, on a un diagramme commutatif

$$
\begin{array}{ccccc}
T(M'_1) & \xrightarrow{T(i')} & T(M') & \xrightarrow{T(p')} & T(M'_2) \\
T(v_1) \downarrow & & T(v) \downarrow & & T(v_2) \downarrow \\
T(M_1) & \xrightarrow{T(i)} & T(M) & \xrightarrow{T(p)} & T(M_2)
\end{array}
$$

En vertu du lemme 1 du n° 1, les deux lignes de ce diagramme sont exactes ; comme E est plat pour $M_1$ et $M_2$, $T(v_1)$ et $T(v_2)$ sont injectifs ; en outre, en vertu du lemme 2 du n° 1, $T(i)$ est injectif. Le cor. 1 de la prop. 2 du § 1, n° 4 montre alors que $T(v)$ est injectif et par suite E est M-plat.

b) Si I est un ensemble fini à n éléments, on procède par récurrence sur n en utilisant a).

c) Dans le cas général, soit $M'$ un sous-module de type fini de M. Il existe alors une partie finie J de l’ensemble d’indices I telle que $M'$ soit contenu dans la somme directe $M_J = \bigoplus_{i \in J} M_i$. En vertu de b), E est plat pour $M_J$ ; l’homomorphisme canonique

E \otimes_A M' \to E \otimes_A M_j est donc injectif. D’autre part, comme M_j est facteur direct de M, l’homomorphisme canonique E \otimes_A M_j \to E \otimes_A M est injectif (n° 1, lemme 2). Par composition, on en déduit que E \otimes_A M' \to E \otimes_A M est injectif, et E est plat pour M en vertu du lemme 3.

### 3. Modules plats.

#### Proposition 1 {#ac-i-s2-prop-1 .statement}

Soit E un A-module à droite. Les trois propriétés suivantes sont équivalentes :

a) E est plat pour A_s (autrement dit, pour tout idéal à gauche a de A, l’homomorphisme canonique E \otimes_A a \to E \otimes_A A_s = E est injectif).

b) E est M-plat pour tout A-module à gauche M.

c) Pour toute suite exacte de A-modules à gauche et d’homomorphismes

$$
M' \xrightarrow{\nu} M \xrightarrow{\omega} M''
$$

la suite

$$
E \otimes_A M' \xrightarrow{1 \otimes \nu} E \otimes_A M \xrightarrow{1 \otimes \omega} E \otimes_A M''
$$

est exacte.

Il est immédiat que b) entraîne a). Inversement supposons a) vérifiée ; en vertu du n° 2, lemme 5, E est plat pour tout A-module à gauche libre ; comme tout A-module à gauche est isomorphe à un quotient d’un module libre (Alg., chap. II, 3e éd., § 1, n° 11, prop. 20), il résulte du n° 2, lemme 4 que E est plat pour M.

Montrons que c) implique b). Si \nu : M' \to M est un homomorphisme injectif, la suite 0 \to M' \xrightarrow{\nu} M est exacte ; en vertu de c), la suite 0 \to E \otimes_A M' \xrightarrow{1 \otimes \nu} E \otimes_A M est exacte ; cela signifie que 1 \otimes \nu est injectif, autrement dit que E est M-plat.

Enfin, l’implication b) \Rightarrow c) est la conséquence du lemme plus précis suivant :

#### Lemme 6 {#ac-i-s2-lem-6 .statement}

Si M' \xrightarrow{\nu} M \xrightarrow{\omega} M'' est une suite exacte de A-modules à gauche et si E est un A-module à droite plat pour M'', la suite

$$
E \otimes_A M' \xrightarrow{1 \otimes \nu} E \otimes_A M \xrightarrow{1 \otimes \omega} E \otimes_A M''
$$

est exacte.

Utilisons les notations T(Q) et T(φ) avec le même sens que dans la démonstration du lemme 4 du n° 2. Posons M''_i = ω(M) et soient i : M''_i → M'' l’injection canonique et p l’application de M dans M''_i ayant même graphe que ω. La suite M' → M → M''_i → 0 étant exacte, il résulte du n° 1, lemme 1 que la suite

$$
T(M') \xrightarrow{T(\varphi)} T(M) \xrightarrow{T(p)} T(M''_i) \to 0
$$

est exacte. Par ailleurs, comme E est M''-plat, l’application T(i) : T(M''_i) → T(M'') est injective, et comme T(i) ∘ T(p) = T(ω), la suite

$$
T(M') \xrightarrow{T(\varphi)} T(M) \xrightarrow{T(\omega)} T(M'')
$$

est exacte (§ 1, n° 3).

#### Définition 2 {#ac-i-s2-def-2 .statement}

On dit qu’un A-module à droite E est plat s’il vérifie les propriétés équivalentes de la prop. 1.

On définit de même les A-modules à gauche plats. Dire qu’un A-module à droite E est plat équivaut à dire que E, considéré comme A^0-module à gauche, est plat.

#### Remarque 1 {#ac-i-s2-n3-rem-1 .statement}

En vertu du n° 2, lemme 3, pour qu’un A-module à droite E soit plat, il faut et il suffit que, pour tout idéal à gauche α de A, de type fini, l’application canonique E ⊗_A α → E (prop. 1) d’image Ea, soit injective.

#### Remarque 2 {#ac-i-s2-n3-rem-2 .statement}

Soit E un A-module à droite plat. Si M’ est un sous-module d’un A-module à gauche M, l’injection canonique E ⊗_A M’ → E ⊗_A M permet d’identifier E ⊗_A M’ à un sous-groupe de E ⊗_A M. Ceci étant, soient N un A-module à gauche, u : M → N un homomorphisme, K = Ker u, I = Im u. La considération de la suite exacte.

$$
0 \to K \to M \xrightarrow{u} N
$$

montre aussitôt (prop. 1) que E ⊗_A (Ker u) s’identifie à Ker (1_E ⊗ u). D’autre part, en notant u’ l’homomorphisme surjectif M → I ayant même graphe que u, et i l’injection canonique I → N, 1_E ⊗ u’ est surjectif (n° 1, lemme 1) et 1_E ⊗ i est injectif puisque E est plat. Comme 1_E ⊗ u = (1_E ⊗ i) ∘ (1_E ⊗ u’), E ⊗_A (Im u) s’identifie à Im (1_E ⊗ u).

#### Proposition 2 {#ac-i-s2-prop-2 .statement}

(i) Soit $(E_i)_{i \in I}$ une famille de $A$-modules à droite. Pour que $E = \bigoplus_{i \in I} E_i$ soit plat, il faut et il suffit que chacun des $E_i$ soit plat.

(ii) Soient $I$ un ensemble ordonné, $(E_\alpha, f_{\beta \alpha})$ un système inductif de $A$-modules à droite ($Alg.$, chap. II, 3e éd., § 6, no 6). Si chacun des $E_\alpha$ est plat, alors $E = \lim_{\rightarrow} E_\alpha$ est plat.

Soit $M' \to M$ un homomorphisme injectif de $A$-modules à gauche.

(i) Pour que l’homomorphisme somme directe
$$
\bigoplus_{i \in I} (E_i \otimes_A M') \to \bigoplus_{i \in I} (E_i \otimes_A M)
$$
soit injectif, il faut et il suffit que chacun des homomorphismes $E_i \otimes_A M' \to E_i \otimes_A M$ le soit ($Alg.$, chap. II, 3e éd., § 1, no 6, cor. 1 de la prop. 7), ce qui démontre (i), puisque $\bigoplus_{i \in I} (E_i \otimes_A M)$ s’identifie canoniquement à $E \otimes_A M$ ($Alg.$, chap. II, 3e éd., § 3, no 7, prop. 7).

(ii) Par hypothèse, chacune des suites
$$
0 \to E_\alpha \otimes_A M' \to E_\alpha \otimes_A M
$$
est exacte ; il en est donc de même de la suite
$$
0 \to E \otimes_A M' \to E \otimes_A M
$$
puisque le passage à la limite inductive commute avec le produit tensoriel ($Alg.$, chap. II, 3e éd., § 6, no 7, prop. 12) et conserve l’exactitude ($ibid.$, § 6, no 6, prop. 8).

### 4. Exemples de modules plats.

1) Pour tout anneau $A$, il est clair que $A_d$ est un $A$-module plat ($Alg.$, chap. II, 3e éd., § 3, no 4, prop. 4). Il résulte alors de la prop. 2, (i), du no 3 que tout $A$-module à droite libre, et plus généralement tout $A$-module à droite *projectif* ($Alg.$, chap. II, 3e éd., § 2, no 2) est un $A$-module plat.

2) Si $A$ est un anneau *semi-simple* ($Alg.$, chap. VIII, § 5, no 1, déf. 1) tout $A$-module à droite $E$ est semi-simple, donc somme directe de modules simples ; comme chacun de ces derniers est

*3) Aux chap. II et III, nous étudierons en détail deux exemples importants de A-modules plats : les anneaux de fractions $S^{-1}A$ et les séparés complétés $\hat{A}$ de A pour les topologies $\mathfrak{J}$-adiques.*

#### Proposition 3 {#ac-i-s2-prop-3 .statement}

*Soient A un anneau, E un A-module à droite.

(i) *Supposons que E soit plat. Pour tout élément a de A qui n’est pas diviseur à droite de 0 (*), les relations $x \in E,\ xa = 0$ entraînent $x = 0$.

(ii) *On suppose que A est un anneau commutatif intègre dans lequel tout idéal de type fini est principal (par exemple un anneau principal (Alg., chap. VII, § 1, no 1)). Alors, pour que E soit plat, il faut et il suffit que E soit sans torsion.

Prouvons (i). Soit $\varphi : A_s \to A_s$ l’homomorphisme $t \to ta$ de A-modules à gauche ; l’hypothèse signifie que $\varphi$ est injectif. Comme E est plat, l’homomorphisme $1_E \otimes \varphi : E \otimes_A A_s \to E \otimes_A A_s$ est aussi injectif. Lorsque l’on identifie canoniquement $E \otimes_A A_s$ à E, $1_E \otimes \varphi$ devient l’endomorphisme $x \to xa$ de E. Donc la relation $xa = 0$ entraîne $x = 0$.

Prouvons (ii). D’après (i), si E est plat, E est sans torsion. Inversement, soit E un A-module sans torsion ; vérifions que, pour tout idéal de type fini $a$ de A, l’homomorphisme canonique $E \otimes_A a \to E$ est injectif (no 3, Remarque 1). Cette assertion est évidente si $a = (0)$ ; sinon, on a par hypothèse $a = Aa$ avec $a \in A$ et $a \neq 0$, et $t \to ta$ est alors un isomorphisme $\varphi$ de A sur $a$ ; notant $i$ l’injection canonique $a \to A$, $i \circ \varphi$ est l’homothétie de rapport $a$ dans A. Alors $1_E \otimes (i \circ \varphi)$ est l’homothétie de rapport $a$ dans E, et est injective puisque E est supposé sans torsion. Or, on a $1_E \otimes (i \circ \varphi) = (1_E \otimes i) \circ (1_E \otimes \varphi)$ ; comme $1_E \otimes \varphi$ est un isomorphisme, $1_E \otimes i$ est injective, ce qui achève la démonstration.

(*) Rappelons qu’un *diviseur à droite* (resp. *à gauche*) de 0 dans un anneau A est un élément $b \in A$ tel que l’application $x \to xb$ (resp. $x \to bx$) ne soit pas injective.

#### Exemple {#ac-i-s2-n4-exa-1 .statement}

Appliquant la prop. 3 à l’anneau $\mathbf{Z}$, on voit que $\mathbf{Q}$ est un $\mathbf{Z}$-module plat, mais que $\mathbf{Z}/n\mathbf{Z}$ (pour $n \geq 2$) n’est pas un $\mathbf{Z}$-module plat.

### 5. Platitude des modules quotients.

#### Proposition 4 {#ac-i-s2-prop-4 .statement}

Soit E un A-module à droite. Les trois propriétés suivantes sont équivalentes :
a) E est plat.
b) Pour toute suite exacte de A-modules à droite de la forme
(1)
$$
0 \to G \xrightarrow{v} H \xrightarrow{w} E \to 0
$$
et tout A-module à gauche F, la suite
(2)
$$
0 \longrightarrow G \otimes_A F \xrightarrow{v \otimes 1} H \otimes_A F \xrightarrow{w \otimes 1} E \otimes_A F \longrightarrow 0
$$
est exacte.
c) Il existe une suite exacte (1), où H est plat, telle que la suite (2) soit exacte pour tout A-module à gauche F de la forme $A_s/\alpha$, où $\alpha$ est un idéal à gauche de type fini de A.

Montrons d’abord que a) implique b). Le A-module à gauche F est isomorphe à un quotient d’un module libre (Alg., chap. II, 3e éd., § 1, no 11, prop. 20); autrement dit, on a une suite exacte
$$
0 \to R \xrightarrow{i} L \xrightarrow{p} F \to 0
$$
où L est libre. Considérons le diagramme
(3)
$$
\begin{array}{ccc}
G \otimes R & \xrightarrow{v \otimes 1_R} & H \otimes R \xrightarrow{w \otimes 1_R} E \otimes R \\
\downarrow_{1_G \otimes i} & & \downarrow_{1_H \otimes i} \downarrow_{1_E \otimes i} \\
G \otimes L & \longrightarrow & H \otimes L \longrightarrow E \otimes L \\
\downarrow_{1_G \otimes p} & & \downarrow_{v \otimes 1_L} \downarrow_{w \otimes 1_L} \\
G \otimes F & \xrightarrow{v \otimes 1_F} & H \otimes F
\end{array}
$$
Il est immédiat que ce diagramme est commutatif, et ses lignes et colonnes sont exactes en vertu du no 1, lemme 1; en outre, comme $1_G \otimes p$ et $1_H \otimes p$ sont surjectifs (no 1, lemme 1), on a $G \otimes F = \mathrm{Coker}\,(1_G \otimes i)$, $H \otimes F = \mathrm{Coker}\,(1_H \otimes i)$; $w \otimes 1_R$ est surjectif (no 1, lemme 1); enfin, comme L est libre, donc plat, $v \otimes 1_L$ est injectif. On peut donc appliquer le diagramme du serpent (§ 1, n° 4, prop. 2, (iii)) qui prouve l’existence d’une suite exacte

(4) $\mathrm{Ker}\,(1_H \otimes i) \longrightarrow \mathrm{Ker}\,(1_E \otimes i) \xrightarrow{d} G \otimes F \xrightarrow{\nu \otimes 1_F} H \otimes F.$

Cela étant, si E est plat, $1_E \otimes i$ est injectif, autrement dit $\mathrm{Ker}\,(1_E \otimes i) = 0$, et la suite exacte (4) montre que $\nu \otimes 1_F$ est injectif, donc la suite (2) est exacte (compte tenu du n° 1, lemme 1).

Comme b) implique évidemment c), il nous reste à prouver que c) entraîne a). Considérons le diagramme (3) dans le cas $R = a$, $L = A_s$, $F = A_s/a$, et appliquons la suite exacte (4). Par hypothèse, $\nu \otimes 1_F$ est injectif, donc $\mathrm{Im}\,(d) = 0$; en outre, comme H est plat, on a $\mathrm{Ker}\,(1_H \otimes i) = 0$; l’exactitude de la suite (4) entraîne donc $\mathrm{Ker}\,(1_E \otimes i) = 0$, autrement dit $1_E \otimes i$ est injectif et cela prouve que E est plat (n° 3, Remarque 1).

#### Proposition 5 {#ac-i-s2-prop-5 .statement}

Soit $0 \to E' \xrightarrow{v} E \xrightarrow{w} E'' \to 0$ une suite exacte de A-modules à droite. Supposons que $E''$ soit plat. Alors, pour que E soit plat, il faut et il suffit que $E'$ soit plat.

Soit $u : F' \to F$ un homomorphisme injectif de A-modules à gauche. Considérons le diagramme

$$
\begin{array}{ccc}
E' \otimes F' & \xrightarrow{\nu \otimes 1_{F'}} & E \otimes F' \\
1_{E'} \otimes u \downarrow & & 1_E \otimes u \downarrow \\
E' \otimes F & \xrightarrow{\nu \otimes 1_F} & E \otimes F \\
& & w \otimes 1_F \downarrow \\
& & E'' \otimes F
\end{array}
$$

Il est commutatif et ses lignes sont exactes (n° 1, lemme 1). Puisque $E''$ est plat, $1_{E''} \otimes u$ est injectif ; en outre, la prop. 4 prouve que $\nu \otimes 1_{F'}$ et $\nu \otimes 1_F$ sont injectifs. Cela étant, si E est plat, $1_E \otimes u$ est injectif, donc aussi $(1_E \otimes u) \circ (\nu \otimes 1_{F'}) = (\nu \otimes 1_F) \circ (1_{E'} \otimes u)$; on en conclut que $1_{E'} \otimes u$ est injectif, et par suite $E'$ est plat. Réciproquement, si $E'$ est plat, $1_{E'} \otimes u$ est injectif ; on conclut alors du § 1, n° 4, cor. 1 de la prop. 2, que $1_E \otimes u$ est injectif, et par suite E est plat.

#### Remarque 1 {#ac-i-s2-n5-rem-1 .statement}

Il peut se faire que E et $E'$ soient plats sans que $E''$ le soit, comme le montre l’exemple des $\mathbf{Z}$-modules $E = \mathbf{Z},\ E' = n\mathbf{Z},\ E'' = \mathbf{Z}/n\mathbf{Z}\ (n \geq 2)$.

#### Remarque 2 {#ac-i-s2-n5-rem-2 .statement}

Un sous-module d’un module plat n’est pas nécessairement un module plat (exerc. 3).

### 6. Propriétés d’intersection.

#### Lemme 7 {#ac-i-s2-lem-7 .statement}

Soient E un A-module à droite, F un A-module à gauche, F’, F'' deux sous-modules de F tels que F = F' + F''. Alors l’intersection des images canoniques de E ⊗ F’ et E ⊗ F'' dans E ⊗ F est égale à l’image canonique de E ⊗ (F' ∩ F'').

Considérons en effet le diagramme

$$
\begin{array}{ccccccc}
0 & \to & F' \cap F'' & \longrightarrow & F' & \longrightarrow & F'/(F' \cap F'') \to 0 \\
& & \downarrow & & \downarrow & & i \downarrow \\
0 & \longrightarrow & F'' & \longrightarrow & F' + F'' & \to & (F' + F'')/F'' \to 0
\end{array}
$$

où les flèches non spécifiées sont les injections et surjections canoniques et j est l’isomorphisme canonique défini dans (Alg., chap. I, § 6, no 13, th. 6). Ce diagramme est commutatif et ses lignes sont exactes. On en déduit (puisque F = F' + F'') un diagramme commutatif

$$
\begin{array}{ccc}
E \otimes (F' \cap F'') & \to & E \otimes F' \to E \otimes (F'/(F' \cap F'')) \\
\downarrow & & \downarrow \\
E \otimes F'' & \longrightarrow & E \otimes F \longrightarrow E \otimes (F/F'')
\end{array}
$$

Les lignes de ce diagramme sont exactes (no 1, lemme 1) et $1_E \otimes j$ est un isomorphisme. Notre assertion est alors un cas particulier du § 1, no 4, prop. 1, (i). (Cf. exerc. 5.)

#### Proposition 6 {#ac-i-s2-prop-6 .statement}

Soient E un A-module à droite et F un A-module à gauche tels que E soit plat pour F. Pour tout sous-module F’ de F, notons $\varphi(F')$ l’image de $E \otimes F'$ par l’application canonique de $E \otimes F'$ dans $E \otimes F$ (qui est injective en vertu de la déf. 1 du no 2). Alors, si F’, F'' sont deux sous-modules de F, on a

$$
\varphi(F' \cap F'') = \varphi(F') \cap \varphi(F'').
$$

En effet, comme E est plat pour F, $\varphi(F' + F'')$ s’identifie à $E \otimes (F' + F'')$, et les sous-modules $\varphi(F')$, $\varphi(F'')$ et $\varphi(F' \cap F'')$ s’identifient aux images canoniques de $E \otimes F'$, $E \otimes F''$ et $E \otimes (F' \cap F'')$ dans $E \otimes (F' + F'')$ respectivement. La prop. 6 résulte alors du lemme 7.

n° 6

#### Remarque 1 {#ac-i-s2-n6-rem-1 .statement}

Les hypothèses étant celles de la prop. 6, on identifie d’ordinaire $E \otimes F'$ à $\varphi(F')$ pour tout sous-module $F'$ de $F$, ce qui donne la formule

$$
E \otimes_A (F' \cap F'') = (E \otimes_A F') \cap (E \otimes_A F'').
$$

#### Proposition 7 {#ac-i-s2-prop-7 .statement}

Soient $E$ un $A$-module à droite, $E'$ un sous-module de $E$, $F$ un $A$-module à gauche et $F'$ un sous-module de $F$. Supposons que $E/E'$ ou $F/F'$ soit un module plat. Alors l’image canonique de $E' \otimes F'$ dans $E \otimes F$ est l’intersection des images canoniques de $E' \otimes F$ et de $E \otimes F'$ dans $E \otimes F$.

Supposons par exemple que $E/E'$ soit plat, et considérons le diagramme

$$
\begin{array}{ccc}
E' \otimes F' & \to & E \otimes F' \to (E/E') \otimes F' \\
\downarrow & & \downarrow \\
E' \otimes F & \to & E \otimes F \to (E/E') \otimes F
\end{array}
$$

où les flèches sont les homomorphismes canoniques. Ce diagramme est commutatif et ses lignes sont exactes (n° 1, lemme 1). Comme $E/E'$ est plat, $u$ est injectif. Notre assertion est alors un cas particulier du § 1, n° 4, prop. 1, (i).

#### Corollaire {#ac-i-s2-n6-cor-1 .statement}

Soient $E$ un $A$-module à droite, $E'$ un sous-module de $E$.

(i) Supposons que $E/E'$ soit plat. Alors, pour tout idéal à gauche $a$ de $A$, on a

$$
E'a = E' \cap Ea.
$$

(ii) Inversement, supposons que $E$ soit plat et que pour tout idéal à gauche de type fini $a$ de $A$, on ait la relation (5). Alors $E/E'$ est plat.

(i) Il suffit d’appliquer la prop. 7 au cas où $F = A_s, F' = a$.

(ii) Pour prouver que $E/E'$ est plat, appliquons le critère c) de la prop. 4 du n° 5 ; il faut donc établir que la suite

$$
0 \to E'/E'a \to E/Ea \to E/(E' + Ea) \to 0
$$

est exacte en $E'/E'a$ pour tout idéal à gauche $a$ de type fini de $A$. Or, c’est exactement ce qu’exprime la relation (5).

#### Remarque 2 {#ac-i-s2-n6-rem-2 .statement}

La conclusion de la prop. 7 reste vraie si l’on suppose seulement que E/E’ est plat pour F ou que F/F’ est plat pour E.

### 7. Produits tensoriels de modules plats.

Soient A, B deux anneaux, E un A-module à droite, F un (A, B)-bimodule (Alg., chap. II, 3e éd., § 1, no 14). Rappelons (Alg., chap. II, 3e éd., § 3, no 4) que E ⊗_A F est canoniquement muni d’une structure de B-module à droite, pour laquelle

$$(x \otimes y)b = x \otimes (yb)$$ pour $x \in E,\ y \in F,\ b \in B.$

#### Proposition 8 {#ac-i-s2-prop-8 .statement}

Soient A, B deux anneaux, E un A-module à droite, F un (A, B)-bimodule. Supposons que E soit plat, et que F soit plat en tant que B-module. Alors le B-module E ⊗_A F est plat.

Soient en effet G un B-module à gauche et G’ un sous-module de G. Puisque F est plat en tant que B-module à droite, l’homomorphisme canonique $F \otimes_B G' \to F \otimes_B G$ est injectif. Puisque E est plat, l’homomorphisme canonique

$$E \otimes_A (F \otimes_B G') \to E \otimes_A (F \otimes_B G)$$

est injectif. Comme $E \otimes_A (F \otimes_B G')$ et $E \otimes_A (F \otimes_B G)$ s’identifient canoniquement à $(E \otimes_A F) \otimes_B G'$ et $(E \otimes_A F) \otimes_B G$ respectivement (Alg., chap. II, 3e éd., § 3, no 8, prop. 8), l’homomorphisme canonique $(E \otimes_A F) \otimes_B G' \to (E \otimes_A F) \otimes_B G$ est injectif, ce qui prouve que $E \otimes_A F$ est un B-module plat.

#### Corollaire 1 {#ac-i-s2-prop-8-cor-1 .statement}

Soient C un anneau commutatif, E, F deux C-modules plats. Alors $E \otimes_C F$ est un C-module plat.

En effet, F est un (C, C)-bimodule et il suffit d’appliquer la prop. 8 avec $B = A = C$.

#### Corollaire 2 {#ac-i-s2-prop-8-cor-2 .statement}

Soit ρ un homomorphisme d’un anneau A dans un anneau B. Si E est un A-module à droite plat, le B-module à droite $ρ^*(E) = E_{(B)}$ obtenu par extension à B de l’anneau des scalaires (Alg., chap. II, 3e éd., § 5, no 1) est plat.

En effet, on a par définition $E_{(B)} = E \otimes_A B$, où B est considéré comme (A, B)-bimodule au moyen de ρ. Comme le B-module à droite B_d est plat, il suffit d’appliquer la prop. 8.

#### Corollaire 3 {#ac-i-s2-prop-8-cor-3 .statement}

Soient R, S deux anneaux, φ : R → S un homomorphisme d’anneaux. Si M est un S-module à droite plat et si φ_*(S_d) est un R-module à droite plat, alors φ_*(M) est un R-module à droite plat.

Rappelons que φ_*(M) est le R-module à droite défini par x.r = x.φ(r) pour tout x ∈ M et tout r ∈ R (Alg., chap. II, 3e éd., § 1, no 13). On applique alors la prop. 8 avec A = S, B = R, E = M et F = S, S étant muni de la structure de (S, R)-bimodule définie par φ ; le R-module à droite M ⊗_S S n’est autre alors que φ_*(M).

#### Proposition 9 {#ac-i-s2-prop-9 .statement}

Soient (A_α, f_{βα}) un système inductif filtrant d’anneaux, A = lim → A_α sa limite inductive, (E_α, g_{βα}) un système inductif de A_α-modules à droite ayant même ensemble d’indices, E = lim → E_α sa limite inductive, qui est un A-module à droite (Alg., chap. II, 3e éd., § 6, no 6). Si chacun des E_α est un A_α-module plat, E est un A-module plat.

En effet, soit E'_α = E_α ⊗_{A_α} A, où A est considéré comme A_α-module à gauche au moyen de l’homomorphisme canonique A_α → A ; on sait que le A-module à droite E est canoniquement isomorphe à lim → E'_α (loc. cit., cor. 2 de la prop. 12). Il résulte du cor. 2 de la prop. 8 que E'_α est un A-module à droite plat pour tout α, donc E est un A-module plat en vertu du no 3, prop. 2.

### 8. Modules de présentation finie.

Soit A un anneau. On appelle présentation (ou présentation de longueur 1) d’un A-module à gauche (resp. à droite) E une suite exacte

(6)
$$
L_1 \to L_0 \to E \to 0
$$
de A-modules à gauche (resp. à droite), où L_0 et L_1 sont libres.

Tout A-module E admet une présentation. On sait en effet (Alg., chap. II, 3e éd., § 1, no 11, prop. 20) qu’il existe un homomorphisme surjectif $u : L_0 \to E$, où $L_0$ est libre ; si $R$ est le noyau de $u$, il existe de même un homomorphisme surjectif $\varphi : L_1 \to R$ où $L_1$ est libre. Si l’on considère $\varphi$ comme un homomorphisme de $L_1$ dans $L_0$, la suite $L_1 \xrightarrow{\varphi} L_0 \xrightarrow{u} E \to 0$ est exacte par définition, d’où notre assertion.

Si $\rho : A \to B$ est un homomorphisme d’anneaux, toute présentation (6) de $E$ fournit une présentation de $E_{(B)} = E \otimes_A B$ :

$$
L_1 \otimes_A B \to L_0 \otimes_A B \to E \otimes_A B \to 0
$$

en vertu du no 1, lemme 1 et du fait que $L \otimes_A B$ est un $B$-module libre lorsque $L$ est libre.

On dit qu’une présentation (6) d’un module $E$ est *finie* si les modules libres $L_0$ et $L_1$ ont des bases finies. Il est clair que si la présentation (6) est finie, il en est de même de la présentation (7). On dit que $E$ est un *A-module de présentation finie* s’il admet une présentation finie.

#### Lemme 8 {#ac-i-s2-lem-8 .statement}

(i) *Tout module admettant une présentation finie est de type fini*.

(ii) *Si $A$ est un anneau noethérien à gauche, tout $A$-module à gauche de type fini admet une présentation finie*.

(iii) *Tout module projectif de type fini admet une présentation finie*.

L’assertion (i) résulte trivialement des définitions. Si $A$ est noethérien à gauche et s’il existe un homomorphisme surjectif $u : L_0 \to E$, où $L_0$ est un $A$-module à gauche libre ayant une base finie, le noyau $R$ de $u$ est de type fini (*Alg.*, chap. VIII, § 2, no 1, prop. 1 et no 3, prop. 7), donc il y a un homomorphisme surjectif $\varphi : L_1 \to R$ où $L_1$ est libre de base finie, et la suite exacte $L_1 \xrightarrow{\varphi} L_0 \xrightarrow{u} E \to 0$ est une présentation finie de $E$; d’où (ii).

Enfin, supposons que $E$ soit un module projectif de type fini ; il est alors facteur direct d’un module libre de type fini $L_0$ (*Alg.*, chap. II, 3e éd., § 2, no 2, cor. de la prop. 4) ; le noyau $R$ de l’homomorphisme surjectif $L_0 \to E$ est alors isomorphe à un quotient de $L_0$, donc est de type fini, et on termine comme ci-dessus.

#### Lemme 9 {#ac-i-s2-lem-9 .statement}

Soient $A$ un anneau, $E$ un $A$-module de présentation finie. Pour toute suite exacte

$$
0 \to F \xrightarrow{j} G \xrightarrow{p} E \to 0
$$

où $G$ est de type fini, le module $F$ est de type fini.

Soit $L_1 \xrightarrow{r} L_0 \xrightarrow{s} E \to 0$ une présentation finie ; si $(e_i)$ est une base de $L_0$, il existe pour chaque $i$ un élément $g_i \in G$ tel que $p(g_i) = s(e_i)$; l’homomorphisme $u : L_0 \to G$ tel que $u(e_i) = g_i$ pour tout $i$ est donc tel que $s = p \circ u$. Comme $s \circ r = 0$, on a $u(r(L_1)) \subset \mathrm{Ker}\, p$, et comme $\mathrm{Ker}\, p$ est isomorphe à $F$, on voit qu’il y a un homomorphisme $\varphi : L_1 \to F$ tel que le diagramme

$$
\begin{array}{ccc}
L_1 & \xrightarrow{r} & L_0 \xrightarrow{s} E \to 0 \\
v \downarrow & & u \downarrow \quad 1_E \downarrow \\
F & \xrightarrow{j} & G \xrightarrow{p} E \to 0
\end{array}
$$

soit commutatif. Comme $j$ est injectif et $s$ surjectif, on peut appliquer le diagramme du serpent ($§ 1$, no 4, prop. 2), autrement dit il y a une suite exacte

$$
0 = \mathrm{Ker}\, 1_E \xrightarrow{d} \mathrm{Coker}\, \varphi \to \mathrm{Coker}\, u \to \mathrm{Coker}\, 1_E = 0.
$$

Ceci montre que $\mathrm{Coker}\, \varphi$ est isomorphe à $G/u(L_0)$, qui est de type fini par hypothèse. On a en outre la suite exacte

$$
0 \to \varphi(L_1) \to F \to \mathrm{Coker}\, \varphi \to 0
$$

et comme $\varphi(L_1)$ et $\mathrm{Coker}\, \varphi$ sont de type fini, il en est de même de $F$ (*Alg.*, chap. II, 3e éd., $§ 1$, no 7, cor. 5 de la prop. 9).

### 9. *Extension des scalaires dans les modules d’homomorphismes.*

Soient $A$ et $B$ deux anneaux, $E$ un $A$-module à droite, $F$ un $B$-module à droite et $G$ un $(B, A)$-bimodule. Rappelons qu’on a défini (*Alg.*, chap. II, 3e éd., $§ 4$, no 2) un homomorphisme canonique de $\mathbf{Z}$-modules

$$(8)$$
$$
\nu : F \otimes_B \mathrm{Hom}_A(E, G) \to \mathrm{Hom}_A(E, F \otimes_B G)
$$

tel que, pour $y \in F$ et $u \in \mathrm{Hom}_A(E, G)$, $\nu(y \otimes u)$ soit l’application $A$-linéaire $x \to y \otimes u(x)$.

#### Proposition 10 {#ac-i-s2-prop-10 .statement}

Soient $A, B$ deux anneaux, $E$ un $A$-module à droite, $F$ un $B$-module à droite, $G$ un $(B, A)$-bimodule. Supposons que $F$ soit plat. Alors, si $E$ est de type fini (resp. de présentation finie) l’homomorphisme canonique (8) est injectif (resp. bijectif).

Considérons $A, B, F, G$ comme fixés, et, pour tout $A$-module à droite $E$, posons

$$
T(E) = F \otimes_B \mathrm{Hom}_A(E, G), \qquad T'(E) = \mathrm{Hom}_A(E, F \otimes_B G)
$$

et notons $\nu_E$ l’homomorphisme (8) ; pour tout homomorphisme $\varphi : E \to E'$ de $A$-modules à droite, posons $T(\varphi) = 1_F \otimes \mathrm{Hom}(\varphi, 1_G)$ et $T'(\varphi) = \mathrm{Hom}(\varphi, 1_F \otimes 1_G)$. Soit $L_1 \xrightarrow{\psi} L_0 \xrightarrow{\omega} E \to 0$ une présentation de $E$; nous supposons le module libre $L_0$ (resp. les modules libres $L_0$ et $L_1$) de type fini. On a le diagramme

$$
\begin{array}{ccccccc}
0 & \longrightarrow & T(E) & \xrightarrow{T(\omega)} & T(L_0) & \xrightarrow{T(\psi)} & T(L_1) \\
& & \nu_E \downarrow & & \nu_{L_0} \downarrow & & \nu_{L_1} \downarrow \\
0 & \longrightarrow & T'(E) & \xrightarrow{T'(\omega)} & T'(L_0) & \xrightarrow{T'(\psi)} & T'(L_1)
\end{array}
$$

qui est commutatif, et dont la seconde ligne est exacte ($Alg.$, chap. II, 3e éd., § 2, no 1, th. 1) ; en outre, la suite

$$
0 \to \mathrm{Hom}_A(E, G) \to \mathrm{Hom}_A(L_0, G) \to \mathrm{Hom}_A(L_1, G)
$$

est exacte (*loc. cit.*), et comme $F$ est *plat*, la première ligne de (9) est aussi une suite exacte (no 3, prop. 1). Cela étant, on sait que $\nu_{L_0}$ (resp. $\nu_{L_0}$ et $\nu_{L_1}$) est *bijectif* (resp. sont *bijectifs*) ($Alg.$, chap. II, 3e éd., § 4, no 2, prop. 2). Si on suppose seulement $\nu_{L_0}$ bijectif, il résulte de (9) que $\nu_{L_0} \circ T(\omega) = T'(\omega) \circ \nu_E$ est injectif, donc $\nu_E$ l’est aussi. Si on suppose que $\nu_{L_0}$ et $\nu_{L_1}$ sont tous deux bijectifs, on déduit du § 1, no 4, cor. 2, (ii) de la prop. 2 que $\nu_E$ est surjectif, et comme on vient de voir que $\nu_E$ est injectif, il est bijectif.

C. Q. F. D.

### 10. *Extension des scalaires : cas des anneaux commutatifs.*

Soient maintenant $A$ un anneau *commutatif*, $B$ un anneau, $\rho : A \to B$ un homomorphisme d’anneaux tel que $\rho(A)$ soit contenu dans le *centre* de $B$; autrement dit, $\rho$ définit sur $B$ une structure de *A-algèbre*. Pour tout $A$-module $E$, le $B$-module à droite $E_{(B)} = E \otimes_A B$ s’identifie alors à $B \otimes_A E$, les structures de $A$-mon° 10

dule de $\rho_*(B_s)$ et de $\rho_*(B_d)$ étant identiques par hypothèse. Rappelons que pour tout couple $(E, F)$ de $A$-modules, on a défini un $B$-homomorphisme canonique

(10)
$$
\omega : (\mathrm{Hom}_A(E, F))_{(B)} \to \mathrm{Hom}_B(E_{(B)}, F_{(B)})
$$
tel que pour $u \in \mathrm{Hom}_A(E, F)$, $\omega(u \otimes 1) = u \otimes 1_B$ (*Alg.*, chap. II, 3e éd., § 5, n° 3).

#### Proposition 11 {#ac-i-s2-prop-11 .statement}

*Soient $A$ un anneau commutatif, $B$ un anneau, $\rho$ un homomorphisme de $A$ dans le centre de $B$, $E$ et $F$ deux $A$-modules. On suppose que $B$ est un $A$-module plat, et que $E$ est de type fini (resp. de présentation finie). Alors l’homomorphisme canonique (10) est injectif (resp. bijectif).*

Comme $\omega$ est composé de l’isomorphisme canonique
$$
\mathrm{Hom}_A(E, B \otimes_A F) \to \mathrm{Hom}_B(E_{(B)}, F_{(B)})
$$
et de l’homomorphisme canonique (8)
$$
\nu : B \otimes_A \mathrm{Hom}_A(E, F) \to \mathrm{Hom}_A(E, B \otimes_A F)
$$
(*loc. cit.*), la proposition est conséquence de la prop. 10 du n° 9.

Supposons maintenant $A$ et $B$ commutatifs, et considérons trois $A$-modules, $E_1, E_2, E_3$ et une application $A$-bilinéaire $f : E_1 \times E_2 \to E_3$. Il existe alors une application $B$-bilinéaire et une seule $f_B : E_{1(B)} \times E_{2(B)} \to E_{3(B)}$ telle que $f_B(1 \otimes x_1, 1 \otimes x_2) = 1 \otimes f(x_1, x_2)$ quels que soient $x_1 \in E_1, x_2 \in E_2$ (*Alg.*, chap. IX, § 1, n° 4, prop. 1).

Dans l’énoncé qui suit, nous supposerons que $B$ est un $A$-module *plat* et, pour tout sous-module $E'$ d’un $E_i$ ($i = 1, 2, 3$), nous identifierons canoniquement $E'_{(B)}$ à son image dans $E_{i(B)}$ (n° 3, *Remarque* 2).

#### Proposition 12 {#ac-i-s2-prop-12 .statement}

*Soient $A, B$ des anneaux commutatifs, $\rho$ un homomorphisme de $A$ dans $B$, $E_1, E_2, E_3$ trois $A$-modules, $f : E_1 \times E_2 \to E_3$ une application $A$-bilinéaire,
$$
f_B : E_{1(B)} \times E_{2(B)} \to E_{3(B)}
$$
son extension. Considérons un sous-module $F_2$ de $E_2$, un sous-module $F_3$ de $E_3$, et notons $T$ le sous-module de $E_1$ formé des $x_1 \in E_1$ tels que f(x_1, x_2) \in F_3 \text{ pour tout } x_2 \in F_2. On suppose que B est un A-module plat, et que F_2 est de type fini. Alors T_{(u)} est l'ensemble des x'_1 \in E_{1(u)} tels que f_B(x'_1, x'_2) \in F_{3(u)} pour tout x'_2 \in F_{2(u)}.

Soit en effet p la surjection canonique E_3 \to E_3/F_3 ; à tout x_1 \in E_1 associons l'application A-linéaire x_2 \to p(f(x_1, x_2)) de F_2 dans E_3/F_3, que nous noterons g(x_1) ; donc g est un A-homomorphisme de E_1 dans Hom_A(F_2, E_3/F_3), et le noyau de g n'est autre que T. Puisque B est un A-module plat, on a la suite exacte

$$
0 \to T_{(u)} \to E_{1(u)} \xrightarrow{1 \otimes g} (\operatorname{Hom}_A(F_2, E_3/F_3))_{(u)}
$$

(n°3, prop. 1). En vertu de la prop. 11, l'homomorphisme canonique

$$
\omega : (\operatorname{Hom}_A(F_2, E_3/F_3))_{(u)} \to \operatorname{Hom}_B(F_{2(u)}, (E_3/F_3)_{(u)})
$$

est injectif. D'autre part, comme B est un A-module plat, (E_3/F_3)_{(u)} s'identifie canoniquement à E_{3(u)}/F_{3(u)} ; composant ω et 1 ⊗ g, on obtient un homomorphisme u, pour lequel la suite

$$
0 \to T_{(u)} \to E_{1(u)} \xrightarrow{u} \operatorname{Hom}_B(F_{2(u)}, E_{3(u)}/F_{3(u)})
$$

est exacte. Il résulte aussitôt des définitions que u(x'_1), pour x'_1 = 1 ⊗ x_1 \in E_{1(u)}, est l'application linéaire qui, à tout x'_2 \in F_{2(u)}, fait correspondre la classe mod. F_{3(u)} de f_B(x'_1, x'_2) ; par linéarité, cela est encore vrai pour tout x'_1 \in E_{1(u)} ; le noyau de u étant T_{(u)}, la proposition est démontrée.

#### Corollaire 1 {#ac-i-s2-prop-12-cor-1 .statement}

Soient A, B deux anneaux commutatifs, ρ : A → B un homomorphisme tel que B soit un A-module plat, E un A-module de présentation finie. Pour tout sous-module de type fini F de E, l'orthogonal de F_{(u)} dans le dual de E_{(u)} est égal à (F')_{(u)}, en désignant par F' l'orthogonal de F dans le dual E* de E.

Il résulte de la prop. 11 que (E*)_{(u)} est canoniquement isomorphe au dual (E_{(u)})* de E_{(u)}. Il suffit alors d'appliquer la prop. 12 à E_1 = E*, E_2 = E, E_3 = A, F_2 = F, F_3 = \{0\}, f étant la forme bilinéaire canonique sur E* × E.

#### Corollaire 2 {#ac-i-s2-prop-12-cor-2 .statement}

Soient A, B, deux anneaux commutatifs, ρ : A → B un homomorphisme tel que B soit un A-module plat. Alors, pour tout A-module de type fini E, l'annulateur de E_{(u)} est l'idéal aB de B, où a est l'annulateur de E dans A.

Il suffit d’appliquer la prop. 12 à $E_1 = A,\ E_2 = E_3 = E,\ F_2 = E,\ F_3 = \{0\}$.

#### Remarque {#ac-i-s2-n10-rem-1 .statement}

Lorsqu’il n’y a pas d’ambiguïté sur les modules $E_i$ et sur l’application bilinéaire $f$, on note parfois $F_3 : F_2$ le module désigné par T dans la prop. 12, et on l’appelle le transporteur de $F_2$ dans $F_3$. La conclusion de la prop. 12 s’écrit alors

(11)
$$
F_{3(B)} : F_{2(B)} = (F_3 : F_2)_{(B)}.
$$

Dans le cas particulier où les $E_i$ sont égaux à l’anneau $A$, $f$ étant la multiplication, et les $F_i$ des idéaux $a_i$, on obtient la formule des transporteurs

(12)
$$
B(a_3 : a_2) = Ba_3 : Ba_2
$$
valable lorsque B est un A-module plat et que $a_2$ est un idéal de type fini.

### 11. Interprétation de la platitude en termes de relations (*).

Dans tout ce no A désigne un anneau, E un A-module à droite et F un A-module à gauche.

Tout élément de $E \otimes_A F$ s’écrit, au moins d’une façon, sous la forme $z = \sum_{i=1}^n e_i \otimes f_i$ où $e_i \in E$ et $f_i \in F$. Le lemme suivant donne une condition pour qu’une telle somme soit nulle :

#### Lemme 10 {#ac-i-s2-lem-10 .statement}

Soient $(f_\lambda)_{\lambda \in L}$ une famille de générateurs de F, $(e_\lambda)_{\lambda \in L}$ une famille d’éléments de E, de support fini. Pour que $\sum_{\lambda \in L} e_\lambda \otimes f_\lambda = 0$, il faut et il suffit qu’il existe un ensemble fini J, une famille $(x_j)_{j \in J}$ d’éléments de E et une famille $(a_{j\lambda})$ ($j \in J,\ \lambda \in L$) d’éléments de A ayant les propriétés suivantes :
1° la famille $(a_{j\lambda})$ a un support fini ;
2° on a $\sum_{\lambda \in L} a_{j\lambda} f_\lambda = 0$ pour tout $j \in J$ ;
3° on a $e_\lambda = \sum_{j \in J} x_j a_{j\lambda}$ pour tout $\lambda \in L$.

(*) Les résultats de ce no ne seront pas utilisés dans le reste de ce chapitre, sauf au § 3, no 7.

En langage imagé, le système des $e_\lambda$ doit être combinaison linéaire à coefficients dans $E$ de systèmes d’éléments de $A$ qui sont des « relations entre les $f_\lambda$ ».

Considérons en effet le $A$-module libre $A_s^{(L)}$, sa base canonique $(u_\lambda)$ et l’homomorphisme $g : A_s^{(L)} \to F$ tel que $g(u_\lambda) = f_\lambda$ pour tout $\lambda \in L$; en notant $R$ le noyau de $g$, on a (puisque les $f_\lambda$ engendrent $F$) la suite exacte

$$
R \xrightarrow{i} A_s^{(L)} \xrightarrow{g} F \to 0
$$

où $i$ désigne l’injection canonique. En vertu du no 1, lemme 1, on en déduit la suite exacte

$$
E \otimes_A R \xrightarrow{1 \otimes i} E \otimes_A A_s^{(L)} \xrightarrow{1 \otimes g} E \otimes_A F \to 0.
$$

Or, $E \otimes_A A_s^{(L)}$ s’identifie canoniquement à $E^{(L)}$, une famille $e = (e_\lambda) \in E^{(L)}$ étant identifiée à $\sum_{\lambda} e_\lambda \otimes u_\lambda$ ($Alg.$, chap. II, 3e éd., § 3, no 7, cor. 1 de la prop. 7). Pour qu’une telle famille appartienne au noyau de $1_E \otimes g$, il faut et il suffit que $\sum_{\lambda \in L} e_\lambda \otimes f_\lambda = 0$ dans $E \otimes_A F$; compte tenu de la suite exacte (13), cela équivaut à dire que $e$ appartient à l’image de $1_E \otimes i$, c’est-à-dire que l’on a une relation de la forme

$$
\sum_{\lambda \in L} e_\lambda \otimes u_\lambda = \sum_{j \in J} x_j \otimes i(r_j)
$$

où $x_j \in E$, $r_j \in R$ et $J$ est fini. Si l’on pose $i(r_j) = \sum_{\lambda \in L} a_{j\lambda} u_\lambda$, l’hypothèse $r_j \in R$ se traduit par la relation $\sum_{\lambda \in L} a_{j\lambda} f_\lambda = 0$ pour tout $j \in J$; la relation (14) se traduit d’autre part par $e_\lambda = \sum_{j \in J} x_j a_{j\lambda}$ pour tout $\lambda \in L$ ($Alg.$, chap. II, 3e éd., § 3, no 7, cor. 1 de la prop. 7), ce qui achève la démonstration.

#### Proposition 13 {#ac-i-s2-prop-13 .statement}

*Pour que E soit plat pour F* (no 2, déf. 1), *il faut et il suffit que la condition suivante soit satisfaite*:

(R) *Si* $(e_i)_{i \in I}$ *et* $(f_i)_{i \in I}$ *sont deux familles finies d’éléments de E et de F respectivement, telles que* $\sum_{i \in I} e_i \otimes f_i = 0$ *dans* $E \otimes_A F$, *il existe un ensemble fini J, une famille* $(x_j)_{j \in J}$ *d’éléments de E, et une famille* $(a_{ji})$ *$(j \in J, i \in I)$* *d’éléments de A, ayant les propriétés suivantes* :

n° 11

1° on a $\sum_{i \in I} a_{ji} f_i = 0$ pour tout $j \in J$;
2° on a $e_i = \sum_{j \in J} x_j a_{ji}$ pour tout $i \in I$.

Supposons que E soit plat pour F. Soient $(e_i)$ et $(f_i)$ des familles finies d’éléments telles que $\sum_i e_i \otimes f_i = 0$ dans $E \otimes_A F$, et soit $F'$ le sous-module de F *engendré par les* $f_i$. Puisque l’application canonique $E \otimes_A F' \to E \otimes_A F$ est injective, on a aussi $\sum_i e_i \otimes f_i = 0$ *dans* $E \otimes_A F'$ et on peut alors appliquer le lemme 10 à E et à $F'$; on obtient ainsi les familles $(x_j)$ et $(a_{ji})$ vérifiant les conditions de (R).

Réciproquement, supposons vérifiée la condition (R). Soit $F'$ un sous-module de F, et soit $y = \sum_{i \in I} e_i \otimes f_i$ un élément du noyau de l’application canonique $E \otimes_A F' \to E \otimes_A F$. Puisque (R) est vérifiée, il existe des familles $(x_j)$ et $(a_{ji})$ vérifiant les conditions 1° et 2°. On en conclut que, dans $E \otimes_A F'$, on a

$$
y = \sum_{i,j} x_j a_{ji} \otimes f_i = \sum_{j \in J} (x_j \otimes \sum_{i \in I} a_{ji} f_i) = 0.
$$

Donc $E \otimes_A F' \to E \otimes_A F$ est injectif. C. Q. F. D.

#### Corollaire 1 {#ac-i-s2-prop-13-cor-1 .statement}

*Pour qu’un A-module à droite E soit plat, il faut et il suffit qu’il vérifie la condition suivante*:

(RP) *Si* $(e_i)_{i \in I}$ *et* $(b_i)_{i \in I}$ *sont deux familles finies d’éléments de* E *et de* A *respectivement telles que* $\sum_{i \in I} e_i b_i = 0$, *il existe un ensemble fini* J, *une famille* $(x_j)_{j \in J}$ *d’éléments de* E, *et une famille* $(a_{ji})$ (*j* $\in J, i \in I$) *d’éléments de* A *tels que* $\sum_{i \in I} a_{ji} b_i = 0$ *pour tout* $j \in J$ *et que* $e_i = \sum_{j \in J} x_j a_{ji}$ *pour tout* $i \in I$.

En effet, la condition (RP) n’est autre que la condition (R) de la prop. 13, appliquée au module $F = A_s$.

En termes imagés, (RP) s’énonce ainsi : toute « relation » entre les $b_i$, à coefficients dans E, est combinaison linéaire (à coefficients dans E) de « relations » entre les $b_i$ à coefficients dans A.

Considérons plus particulièrement un homomorphisme de A dans un anneau B, faisant de B un A-module à droite. On sait (n° 3, prop. 1) qu’il revient au même de dire que ce A-module est plat, ou qu’il est plat pour tout A-module à gauche $A_s^m$ ($m \geq 1$). Si on applique la condition (R) de la prop. 13 à $E = B, F = A_s^m$, on obtient la condition suivante :

#### Corollaire 2 {#ac-i-s2-prop-13-cor-2 .statement}

*Pour que l’anneau B soit un A-module à droite plat, il faut et il suffit qu’il vérifie la condition suivante :*
(RP') *Toute solution* $(y_k)_{1 \leq k \leq n}$, *formée d’éléments de B, d’un système d’équations linéaires et homogènes*

$$
\sum_{k=1}^n y_k c_{ki} = 0 \qquad (1 \leq i \leq m)
$$
*à coefficients* $c_{ki}$ *dans A, est combinaison linéaire*

$$
y_k = \sum_{j=1}^q b_j z_{jk} \qquad (1 \leq k \leq n)
$$
*à coefficients* $b_j \in B$, *de solutions* $(z_{jk})_{1 \leq k \leq n}$ *du système* (15), *formées d’éléments* $z_{jk}$ *de A*.

## EXERCICES {#ac-i-s2-exercises}

See the [exercises for § 2](exercises/s2/).
