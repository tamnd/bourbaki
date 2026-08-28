---
book: ac
book_title: Commutative Algebra
chapter: III
chapter_title: Graduations, filtrations et topologies
section: 2
section_title: Généralités sur les anneaux et modules filtrés
lang: fr
source: ac-i-iv-fr
pdf_pages: 0190-0233, 0279-0290
extraction: ocr
subsections:
    - "no": 1
      title: Anneaux et modules filtrés.
      page: 0
      pdf_page: 190
    - "no": 2
      title: Fonction d’ordre.
      page: 0
      pdf_page: 194
    - "no": 3
      title: Module gradué associé à un module filtré.
      page: 0
      pdf_page: 195
    - "no": 4
      title: Homomorphismes compatibles avec les filtrations.
      page: 0
      pdf_page: 199
    - "no": 5
      title: Topologie définie par une filtration.
      page: 0
      pdf_page: 201
    - "no": 6
      title: Modules filtrés complets.
      page: 0
      pdf_page: 204
    - "no": 7
      title: Propriétés de compacité linéaire des modules filtrés complets.
      page: 0
      pdf_page: 208
    - "no": 8
      title: Relèvement d’homomorphismes de modules gradués associés.
      page: 0
      pdf_page: 209
    - "no": 9
      title: Relèvement de familles d’éléments d’un module gradué associé.
      page: 0
      pdf_page: 213
    - "no": 10
      title: 'Application : exemples d’anneaux noethériens.'
      page: 0
      pdf_page: 217
    - "no": 11
      title: Anneaux m-adiques complets et limites projectives.
      page: 0
      pdf_page: 220
    - "no": 12
      title: Séparé complété d'un module filtré.
      page: 0
      pdf_page: 222
    - "no": 13
      title: Séparé complété d’un anneau semi-local.
      page: 0
      pdf_page: 228
statements: 68
exercises: 31
content_sha256: dfff54cb43c75cb89d327982a34ad5f57bfe1d61524bd4073f17f7ca7f31972f
---

## § 2. Généralités sur les anneaux et modules filtrés.

### 1. Anneaux et modules filtrés.

#### Définition 1 {#ac-iii-s2-def-1 .statement}

On appelle filtration croissante (resp. décroissante) sur un groupe $G$ une suite croissante (resp. décroissante) $(G_n)_{n \in \mathbf{Z}}$ de sous-groupes de $G$.

On appelle groupe filtré un groupe muni d’une filtration.

Si $(G_n)_{n \in \mathbf{Z}}$ est une filtration croissante (resp. décroissante) sur un groupe $G$ et si l’on pose $G'_n = G_{-n}$, il est clair que $(G'_n)_{n \in \mathbf{Z}}$ est une filtration décroissante (resp. croissante) sur $G$. On peut donc se borner à étudier les filtrations décroissantes, et lorsque nous parlerons désormais de filtration, il s’agira d’une filtration décroissante, sauf mention expresse du contraire.

Étant donnée une filtration décroissante $(G_n)_{n \in \mathbf{Z}}$ sur un groupe $G$, il est clair que $\bigcap_{n \in \mathbf{Z}} G_n$ et $\bigcup_{n \in \mathbf{Z}} G_n$ sont des sous-groupes de G ; on dit que la filtration est séparée si $\bigcap_{n \in \mathbf{Z}} G_n$ est réduit à l’élément neutre, exhaustive si $\bigcup_{n \in \mathbf{Z}} G_n = G$.

#### Définition 2 {#ac-iii-s2-def-2 .statement}

Etant donné un anneau A, on dit qu’une filtration $(A_n)_{n \in \mathbf{Z}}$ sur le groupe additif A est compatible avec la structure d’anneau de A si l’on a
(1) $A_m A_n \subset A_{m+n}$ pour $m \in \mathbf{Z}, n \in \mathbf{Z}$
(2) $1 \in A_0$.

L’anneau A, muni de cette filtration, est alors appelé anneau filtré.

Les conditions (1) et (2) montrent que $A_0$ est un sous-anneau de A, et les $A_n$ des $A_0$-modules (à gauche et à droite). L’ensemble $B = \bigcup_{n \in \mathbf{Z}} A_n$ est un sous-anneau de A, et l’ensemble $\mathfrak{n} = \bigcap_{n \in \mathbf{Z}} A_n$ un idéal bilatère de B : en effet, si $x \in \mathfrak{n}$ et $a \in A_p$, pour tout $k \in \mathbf{Z}$ on a $x \in A_{k-p}$, d’où $ax \in A_k$ et $xa \in A_k$ par (1) ; par suite $ax \in \mathfrak{n}$ et $xa \in \mathfrak{n}$.

Un cas particulier important est celui où $A_0 = A$ ; alors $A_n = A$ pour $n \leq 0$ et tous les $A_n$ sont des idéaux bilatères de A.

#### Définition 3 {#ac-iii-s2-def-3 .statement}

Soient A un anneau filtré, $(A_n)_{n \in \mathbf{Z}}$ sa filtration, E un A-module. On dit qu’une filtration $(E_n)_{n \in \mathbf{Z}}$ sur E est compatible avec sa structure de module sur l’anneau filtré A, si l’on a
(3) $A_m E_n \subset E_{m+n}$ pour $m \in \mathbf{Z}, n \in \mathbf{Z}$.

Le A-module E, muni de cette filtration, est appelé module filtré.

Les $E_n$ sont tous des $A_0$-modules ; si $B = \bigcup_{n \in \mathbf{Z}} A_n$, il est clair que $\bigcup_{n \in \mathbf{Z}} E_n$ est un B-module, et il en est de même de $\bigcap_{n \in \mathbf{Z}} E_n$, par le même raisonnement que ci-dessus pour $\bigcap_{n \in \mathbf{Z}} A_n$. Lorsque $A_0 = A$, tous les $E_n$ sont des sous-modules de E.

#### Exemple 1 {#ac-iii-s2-n1-exa-1 .statement}

Soit $A$ un anneau gradué de type $\mathbf{Z}$; pour tout $i \in \mathbf{Z}$, soit $A_{(i)}$ le sous-groupe des éléments homogènes de degré $i$ dans $A$. Posons $A_n = \sum_{i \geq n} A_{(i)}$; alors il est immédiat que $(A_n)$ est une filtration décroissante, exhaustive et séparée, compatible avec la structure d’anneau de $A$; on dit que cette filtration est associée à la graduation $(A_{(i)})_{i \in \mathbf{Z}}$ et que l’anneau filtré $A$ est associé à l’anneau gradué $A$ donné.

Soit maintenant $E$ un module gradué de type $\mathbf{Z}$ sur l’anneau gradué $A$ et pour tout $i \in \mathbf{Z}$, soit $E_{(i)}$ le sous-groupe des éléments homogènes de degré $i$ de $E$. Posons $E_n = \sum_{i \geq n} E_{(i)}$; alors $(E_n)$ est une filtration décroissante, exhaustive et séparée, compatible avec la structure de module de $E$ sur l’anneau filtré $A$; on dit que cette filtration est associée à la graduation $(E_{(i)})_{i \in \mathbf{Z}}$ et que le module filtré $E$ est associé au module gradué $E$ donné.

#### Exemple 2 {#ac-iii-s2-n1-exa-2 .statement}

Soient $A$ un anneau filtré, $(A_n)_{n \in \mathbf{Z}}$ sa filtration, $E$ un $A$-module. Posons $E_n = A_n E$; il résulte de (1) que l’on a

$$
A_m E_n = A_m A_n E \subset A_{m+n} E = E_{m+n},
$$

et de (2) que $E_0 = E$; donc $(E_n)$ est une filtration exhaustive compatible avec la structure de $A$-module de $E$. On dit que cette filtration sur $E$ est déduite de la filtration donnée $(A_n)$ sur $A$; on notera qu’elle n’est pas nécessairement séparée, même si $(A_n)$ est séparée et si $E$ et les $A_n$ sont des $A$-modules de type fini (cf. § 3, exerc. 2 ; voir cependant § 3, n° 3, prop. 6 et n° 2, cor. de la prop. 4).

#### Exemple 3 {#ac-iii-s2-n1-exa-3 .statement}

Soient $A$ un anneau, $m$ un idéal bilatère de $A$. Posons $A_n = m^n$ pour $n \geq 0$, $A_n = A$ pour $n < 0$; il est immédiat que $(A_n)$ est une filtration exhaustive sur $A$, dite filtration $m$-adique. Soit $E$ un $A$-module ; on appelle filtration $m$-adique sur $E$ la filtration $(E_n)$ déduite de la filtration $m$-adique de $A$; autrement dit, on a $E_n = m^n E$ pour $n \geq 0$ et $E_n = E$ pour $n < 0$.

Si $A$ est commutatif et $B$ une $A$-algèbre, $n = mB$ est un idéal bilatère de $B$, et pour tout $B$-module $F$, on a $n^k F = m^k F$, donc la filtration $n$-adique sur $F$ coïncide avec la filtration $m$-adique (lorsque $F$ est considéré comme $A$-module).

#### Exemple 4 {#ac-iii-s2-n1-exa-4 .statement}

Si A est un anneau filtré, $(A_n)$ sa filtration, le A-module à gauche $A_s$ est un A-module filtré pour la filtration $(A_n)$. Il est clair d’autre part que $(A_n)$ est une filtration compatible avec la structure d’anneau de l’anneau opposé $A^0$, et $A_d$ est un $A^0$-module (à gauche) filtré pour la filtration $(A_n)$.

#### Exemple 5 {#ac-iii-s2-n1-exa-5 .statement}

Sur un anneau A, les ensembles $A_n$ tels que $A_n = 0$ pour $n > 0$, $A_n = A$ pour $n \leq 0$ forment une filtration dite *triviale*, associée (*Exemple 1*) à la graduation triviale de A ; sur un A-module E, toute filtration $(E_n)$ formée de sous-A-modules est alors compatible avec la structure de module de E sur l’anneau filtré A. On peut donc dire que tout groupe commutatif filtré G est un $\mathbf{Z}$-module filtré, lorsque $\mathbf{Z}$ est muni de la filtration triviale.

Soient G un groupe filtré, $(G_n)_{n \in \mathbf{Z}}$ sa filtration ; il est clair que pour tout sous-groupe H de G, $(H \cap G_n)_{n \in \mathbf{Z}}$ est une filtration, dite *induite* par celle de G ; elle est exhaustive (resp. séparée) si celle de G l’est. De même, si H est un sous-groupe *distingué* de G, la famille $((H.G_n)/H)_{n \in \mathbf{Z}}$ est une filtration sur le groupe $G/H$, dite *quotient* par H de la filtration de G ; elle est exhaustive si $(G_n)$ l’est. Si $G'$ est un second groupe filtré, $(G'_n)_{n \in \mathbf{Z}}$ sa filtration, $(G_n \times G'_n)$ est une filtration sur $G \times G'$ dite *produit* des filtrations de G et $G'$, qui est exhaustive (resp. séparée) si $(G_n)$ et $(G'_n)$ le sont.

Soit maintenant A un anneau filtré et soit $(A_n)$ sa filtration ; sur tout sous-anneau B de A, il est clair que la filtration induite par celle de A est compatible avec la structure d’anneau de B. Si b est un idéal bilatère de A, la filtration quotient de celle de A sur $A/b$ est compatible avec la structure de cet anneau, car on a $(A_n + b)(A_m + b) \subset A_{n+m} + b$. Si $A'$ est un second anneau filtré, la filtration produit sur $A \times A'$ est compatible avec la structure de cet anneau.

Soit enfin E un A-module filtré et soit $(E_n)$ sa filtration ; sur tout sous-module F de E, la filtration induite par celle de E est compatible avec la structure de A-module de F, et sur le module quotient $E/F$, la filtration quotient de celle de E est compatible avec la structure de A-module, car on a

$$
A_n(F + E_m) \subset F + A_nE_m \subset F + E_{m+n}.
$$

On notera que si la filtration de E est déduite de celle de A (Exemple 2), il en est de même de la filtration quotient sur E/F, mais non en général de la filtration induite sur F (exerc. 1 ; voir cependant § 3, n° 2, th. 2).

Si E' est un second A-module filtré, la filtration produit sur E × E' est compatible avec la structure de A-module. Si les filtrations de E et E' sont déduites de celle de A (Exemple 2), il en est de même de leur filtration produit.

### 2. Fonction d’ordre.

Soient A un anneau filtré, E un A-module filtré, (E_n) la filtration de E. Pour tout x ∈ E, on désigne par υ(x) la borne supérieure dans \overline{\mathbf{R}} de l’ensemble des entiers n ∈ \mathbf{Z} tels que x ∈ E_n. On a donc les équivalences suivantes :

$$
\begin{cases}
υ(x) = -∞ & \Leftrightarrow \quad x \notin \bigcup_{n \in \mathbf{Z}} E_n \\
υ(x) = p & \Leftrightarrow \quad x \in E_p \text{ et } x \notin E_{p+1} \\
υ(x) = +∞ & \Leftrightarrow \quad x \in \bigcap_{n \in \mathbf{Z}} E_n
\end{cases}
$$

On dit que l’application υ : E → \overline{\mathbf{R}} est la fonction d’ordre du module filtré E. La connaissance de υ entraîne celle des E_n, car E_n est l’ensemble des x ∈ E tels que υ(x) ≥ n ; le fait que les E_n sont des sous-groupes additifs de E se traduit par la relation

$$
υ(x - y) \geq \inf (\upsilon(x), \upsilon(y)).
$$

La définition précédente s’applique en particulier au A-module filtré A_s ; soit ω sa fonction d’ordre. Il résulte de la formule (3) du n° 1 que pour a ∈ A et x ∈ E, on a

$$
υ(ax) \geq ω(a) + υ(x)
$$

lorsque le second membre est défini ; en particulier, pour a ∈ A et b ∈ A, on a

$$
ω(ab) \geq ω(a) + ω(b)
$$

lorsque le second membre est défini.

On définit de la même manière la fonction d’ordre sur un groupe filtré G non nécessairement commutatif ; la relation correspondant à (5) s’écrit alors

(5') $\nu(yx^{-1}) = \nu(xy^{-1}) \geq \inf (\nu(x), \nu(y)).$

### 3. Module gradué associé à un module filtré.

Soient G un groupe commutatif (noté additivement), $(G_n)$ une filtration sur G. Posons

$$
\left\{
\begin{array}{ll}
\mathrm{gr}_n(G) = G_n/G_{n+1} & \text{pour } n \in \mathbf{Z} \\
\mathrm{gr}(G) = \bigoplus_{n \in \mathbf{Z}} \mathrm{gr}_n(G).
\end{array}
\right.
$$

Le groupe commutatif $\mathrm{gr}(G)$ est donc un groupe gradué de type $\mathbf{Z}$, dit groupe gradué associé au groupe filtré G, les éléments homogènes de degré $n$ de $\mathrm{gr}(G)$ étant ceux de $\mathrm{gr}_n(G)$.

Soient maintenant A un anneau filtré, $(A_n)$ sa filtration, E un A-module filtré, $(E_n)$ sa filtration. Quels que soient $p \in \mathbf{Z}, q \in \mathbf{Z}$, on définit une application

$$
\mathrm{gr}_p(A) \times \mathrm{gr}_q(E) \to \mathrm{gr}_{p+q}(E)
$$

de la façon suivante : étant donnés $\alpha \in \mathrm{gr}_p(A), \xi \in \mathrm{gr}_q(E)$, deux représentants $a, a'$ de $\alpha$, deux représentants $x, x'$ de $\xi$, on a $ax \in E_{p+q}, a'x' \in E_{p+q}$ et $ax \equiv a'x'$ (mod. $E_{p+q+1}$), car

$$
ax - a'x' = (a - a')x + a'(x - x')
$$

et $a - a' \in A_{p+1}$ et $x - x' \in E_{q+1}$, donc notre assertion résulte de la formule (3) du n° 1. On peut donc noter $\alpha\xi$ la classe dans

$$
E_{p+q}/E_{p+q+1} = \mathrm{gr}_{p+q}(E)
$$

du produit $ax$ d’un représentant quelconque $a \in \alpha$ et d’un représentant quelconque $x \in \xi$. Il est immédiat que l’application (9) est $\mathbf{Z}$-bilinéaire ; par linéarité, on en déduit une application $\mathbf{Z}$-bilinéaire

$$
\mathrm{gr}(A) \times \mathrm{gr}(E) \to \mathrm{gr}(E).
$$

Si on applique d’abord cette définition au cas où $E = A_s$, l’application (10) est une loi de composition interne sur $\mathrm{gr}(A)$, dont on vérifie aussitôt qu’elle est associative et possède un élément neutre, image canonique dans $\mathrm{gr}_0(A)$ de l’élément unité de

A ; elle définit donc sur gr(A) une structure d’anneau, et la graduation $(\mathrm{gr}_n(A))_{n \in \mathbf{Z}}$ est par définition compatible avec cette structure. On dit que l’anneau gradué gr(A) (de type $\mathbf{Z}$) ainsi défini est l’anneau gradué associé à l’anneau filtré A ; il est évidemment commutatif lorsque A est commutatif ; $\mathrm{gr}_0(A)$ est un sous-anneau de gr(A). L’application (10) est d’autre part une loi externe de gr(A)-module sur gr(E), les axiomes des modules étant trivialement vérifiés, et la graduation $(\mathrm{gr}_n(E))_{n \in \mathbf{Z}}$ sur gr(E) est évidemment compatible avec cette structure de module. On dit que le gr(A)-module gradué gr(E) (de type $\mathbf{Z}$) ainsi défini est le module gradué associé au A-module filtré E.

#### Exemple 1 {#ac-iii-s2-n3-exa-1 .statement}

Soient A un anneau commutatif, t un élément de A non diviseur de 0. Munissons A de la filtration (t)-adique (n° 1, Exemple 3). Alors l’anneau gradué associé gr(A) est canoniquement isomorphe à l’anneau de polynômes $A/(t))[X]$. En effet, on a $\mathrm{gr}_n(A) = 0$ pour $n < 0$, et par définition l’anneau $\mathrm{gr}_0(A)$ est l’anneau $A/(t)$. Notons maintenant qu’en vertu de l’hypothèse sur t la relation $at^n \equiv 0 \pmod{t^{n+1}}$ est équivalente à $a \equiv 0 \pmod{t}$; si $\tau$ est l’image canonique de t dans $\mathrm{gr}_1(A)$, tout élément de $\mathrm{gr}_n(A)$ s’écrit donc d’une manière et d’une seule sous la forme $\alpha \tau^n$ où $\alpha \in \mathrm{gr}_0(A)$; d’où notre assertion.

#### Exemple 2 {#ac-iii-s2-n3-exa-2 .statement}

Soient K un anneau commutatif, A l’anneau de séries formelles $K[[X_1, ..., X_r]]$ (Alg., chap. IV, § 5), m l’idéal de A dont les éléments sont les séries formelles sans terme constant. Munissons A de la filtration m-adique (n° 1, Exemple 3); si $M_1, ..., M_s$ sont les différents monômes en $X_1, ..., X_r$ de degré total $n-1$, il est clair que toute série formelle $u$ d’ordre total $\omega(u) \geq n$ (loc. cit., n° 2) s’écrit $\sum_{k=1}^s u_k M_k$, où les $u_k$ appartiennent à m; on voit donc que $m^n$ est l’ensemble des séries formelles $u$ telles que $\omega(u) \geq n$, ce qui montre que $\omega$ est la fonction d’ordre pour la filtration m-adique. Il est clair alors que pour toute série formelle $u \in m^n$, il existe un polynôme homogène de degré $n$ en les $X_i$ et un seul qui soit congru à $u$ mod. $m^{n+1}$, savoir la somme des termes de degré $n$ de $u$; on en conclut que gr(A) est canoniquement isomorphe à l’anneau de polynômes $K[X_1, ..., X_r]$.

#### Exemple 3 {#ac-iii-s2-n3-exa-3 .statement}

Plus généralement, soient A un anneau commutatif, b un idéal de A, et munissons A de la filtration b-adique. Si on pose B = gr_0(A), F = gr_1(A) = b/b^2, on sait (Alg., chap. III, 3e éd.) que l’application identique du B-module F sur lui-même se prolonge de façon unique en un homomorphisme u de l’algèbre symétrique S(F) de F dans la B-algèbre gr(A); il résulte de la définition de gr(A) que u est un homomorphisme surjectif d’algèbres graduées; en effet, pour n ≥ 1, tout élément de gr_n(A) est somme de classes mod. b^{n+1} d’éléments de la forme y = x_1x_2…x_n, où x_i ∈ b (1 ≤ i ≤ n); si ξ_i est la classe de x_i mod. b^2, il est clair que la classe de y mod. b^{n+1} est l’élément u(ξ_1)…u(ξ_n), d’où notre assertion. En particulier, tout système de générateurs du B-module F est un système de générateurs de la B-algèbre gr(A).

Si maintenant E est un A-module et que l’on munit E de la filtration b-adique, on voit de même que le gr(A)-module gradué gr(E) est engendré par gr_0(E) = E/bE. De façon plus précise, la restriction φ à gr(A) × gr_0(E) de la loi externe du gr(A)-module gr(E) est une application Z-bilinéaire de gr(A) × gr_0(E) dans gr(E); de plus gr(A) est un (gr_0(A), gr_0(A))-bimodule et gr_0(E) un gr_0(A)-module; on vérifie aussitôt que pour α ∈ gr(A), α_0 ∈ gr_0(A), ξ ∈ gr_0(E), on a φ(αα_0, ξ) = φ(α, α_0ξ), donc φ définit une application gr_0(A)-linéaire surjective

$$
γ_E : \mathrm{gr}(A) \otimes_{\mathrm{gr}_0(A)} \mathrm{gr}_0(E) \to \mathrm{gr}(E)
$$

dite canonique.

#### Exemple 4 {#ac-iii-s2-n3-exa-4 .statement}

Soient K un anneau commutatif, g une algèbre de Lie sur K, U l’algèbre enveloppante de g. On définit sur U une filtration croissante (U_n)_{n∈\mathbf{Z}} en prenant U_n = {0} pour n < 0, et en désignant par U_n, pour n ≥ 0, l’ensemble des éléments de U qui peuvent s’exprimer comme somme de produits d’au plus n éléments de g; on a U_0 = K, et gr(U) est une K-algèbre commutative (Gr. et alg. de Lie, chap. I, § 2, n° 6). L’application canonique de g dans gr_1(U) = U_1/U_0 se prolonge de façon unique en un homomorphisme h de l’algèbre symétrique S(g) du K-module g dans la K-algèbre gr(U); l’homomorphisme h est surjectif, et lorsque le K-module g est libre, h est bijectif (loc. cit., n° 7, th. 1).*

#### Exemple 5 {#ac-iii-s2-n3-exa-5 .statement}

Soient A un anneau gradué de type \mathbf{Z}, E un A-module gradué de type $\mathbf{Z}$; soit $A_{(i)}$ (resp. $E_{(i)}$) le sous-groupe des éléments homogènes de degré $i$ de $A$ (resp. $E$). Munissons $A$ et $E$ des filtrations associées à leurs graduations ($n^o 1$, Exemple 1) et notons $A'$ et $E'$ l’anneau filtré et le $A'$-module filtré ainsi obtenus. Alors il est immédiat que l’application $\mathbf{Z}$-linéaire $A \to \mathrm{gr}(A')$ qui transforme un élément de $A_{(n)}$ en son image canonique dans
$$
\mathrm{gr}_n(A) = (\bigoplus_{i \geq n} A_{(i)}) / (\bigoplus_{i \geq n+1} A_{(i)})
$$
est un isomorphisme d’anneaux gradués. On définit de même un isomorphisme canonique $E \to \mathrm{gr}(E')$ de $A$-modules gradués.

#### Proposition 1 {#ac-iii-s2-prop-1 .statement}

*Soient A un anneau filtré, $(A_n)_{n \in \mathbf{Z}}$ sa filtration, $\nu$ sa fonction d’ordre. Supposons que $\mathrm{gr}(A)$ soit un anneau sans diviseur de zéro. Alors, pour tout couple d’éléments $a, b$ de l’anneau $B = \bigcup_{n \in \mathbf{Z}} A_n$, on a $\nu(ab) = \nu(a) + \nu(b)$.*

Comme $n = \bigcap_{n \in \mathbf{Z}} A_n$ est un idéal bilatère de l’anneau $B$, la formule est vraie si $\nu(a)$ ou $\nu(b)$ est égal à $+ \infty$. Dans le cas contraire, $\nu(a) = r$ et $\nu(b) = s$ sont des entiers ; les classes $\alpha$ de $a$ mod.$A_{r+1}$ et $\beta$ de $b$ mod.$A_{s+1}$ sont $\neq 0$ par définition, d’où par hypothèse $\alpha \beta \neq 0$ dans $\mathrm{gr}(A)$, et par suite $ab \notin A_{r+s+1}$ ; comme $ab \in A_{r+s}$, on a $\nu(ab) = \nu(a) + \nu(b)$.

#### Corollaire {#ac-iii-s2-n3-cor-1 .statement}

*Soient A un anneau filtré, $(A_n)_{n \in \mathbf{Z}}$ sa filtration ; posons $B = \bigcup_{n \in \mathbf{Z}} A_n$, $n = \bigcap_{n \in \mathbf{Z}} A_n$. Si l’anneau $\mathrm{gr}(A)$ est sans diviseur de zéro, il en est de même de l’anneau $B/n$.*

En effet, si $a$ et $b$ sont des éléments de $B$ n’appartenant pas à $n$, on a $\nu(a) \neq + \infty$, $\nu(b) \neq + \infty$, d’où $\nu(ab) \neq + \infty$, et par suite $ab \notin n$.

On notera que l’anneau $A$ peut être un anneau intègre, la filtration $(A_n)$ exhaustive et séparée, sans que $\mathrm{gr}(A)$ soit un anneau intègre (exerc. 2).

#### Remarque {#ac-iii-s2-n3-rem-1 .statement}

Soit $G$ un groupe non nécessairement commutatif, muni d’une filtration $(G_n)_{n \in \mathbf{Z}}$ telle que $G_{n+1}$ soit *distingué* dans $G_n$ pour tout $n \in \mathbf{Z}$; posons encore $\mathrm{gr}_n(G) = G_n / G_{n+1}$. On appelle encore groupe gradué associé à $G$ et on note $\mathrm{gr}(G)$ le produit restreint de la famille $(\mathrm{gr}_n(G))_{n \in \mathbf{Z}}$, c'est-à-dire le sous-groupe du produit $\prod_{n \in \mathbf{Z}} \mathrm{gr}_n(G)$ formé des éléments $(\xi_n)$ dont toutes les composantes, sauf au plus un nombre fini, sont égales à l’élément neutre.

### 4. Homomorphismes compatibles avec les filtrations.

Soient $G, G'$ deux groupes commutatifs (notés additivement), $(G_n)$ une filtration sur $G$, $(G'_n)$ une filtration sur $G'$; on dit qu’un homomorphisme $h : G \to G'$ est compatible avec les filtrations de $G$ et $G'$ si l’on a $h(G_n) \subset G'_n$ pour tout $n \in \mathbf{Z}$. L’homomorphisme composé $G_n \xrightarrow{h|G_n} G'_n \to G'_n / G'_{n+1}$ est nul dans $G_{n+1}$, donc définit par passage aux quotients un homomorphisme $h_n : G_n / G_{n+1} \to G'_n / G'_{n+1}$; il y a par suite un homomorphisme de groupes additifs $\mathrm{gr}(h) : \mathrm{gr}(G) \to \mathrm{gr}(G')$ et un seul, tel que, pour tout $n \in \mathbf{Z}$, $\mathrm{gr}(h)$ coïncide avec $h_n$ dans $\mathrm{gr}_n(G) = G_n / G_{n+1}$. On dit que $\mathrm{gr}(h)$ est l’homomorphisme de groupes gradués associé à $h$. Si $G''$ est un troisième groupe filtré, et $h' : G' \to G''$ un homomorphisme compatible avec les filtrations, $h' \circ h$ est un homomorphisme compatible avec les filtrations, et on a

$$
\mathrm{gr}(h' \circ h) = \mathrm{gr}(h') \circ \mathrm{gr}(h).
$$

#### Proposition 2 {#ac-iii-s2-prop-2 .statement}

Soient $G$ un groupe commutatif filtré, $H$ un sous-groupe de $G$; on munit $H$ de la filtration induite et $G/H$ de la filtration quotient. Si $j : H \to G$ est l’injection canonique et $p : G \to G/H$ la surjection canonique, $j$ et $p$ sont compatibles avec les filtrations, et la suite

$$
\begin{array}{ccccccccc}
0 & \longrightarrow & \mathrm{gr}(H) & \xrightarrow{\mathrm{gr}(j)} & \mathrm{gr}(G) & \xrightarrow{\mathrm{gr}(p)} & \mathrm{gr}(G/H) & \longrightarrow & 0
\end{array}
$$

est exacte.

La première assertion est évidente ; si $(G_n)$ est la filtration de $G$, on a $(H \cap G_n) \cap G_{n+1} = H \cap G_{n+1}$, donc $\mathrm{gr}(j)$ est injective ; en outre l’application canonique $G_n \to (H + G_n)/H$ est surjective, donc il en est de même de $\mathrm{gr}(p)$, et on a $\mathrm{gr}(p) \circ \mathrm{gr}(j) = 0$ par

(12). Enfin, soit $\xi \in G_n/G_{n+1}$ dans le noyau de $\mathrm{gr}(p)$; il existe donc $x \in \xi$ tel que $x \in H + G_{n+1}$; mais comme $G_{n+1} \subset G_n$, on a
$$
G_n \cap (H + G_{n+1}) = (H \cap G_n) + G_{n+1},
$$
donc $x = y + z$ avec $y \in H \cap G_n$ et $z \in G_{n+1}$; cela prouve que $\xi$ est la classe mod. $G_{n+1}$ de $j(y)$, autrement dit appartient à l’image de $\mathrm{gr}(H)$ par $\mathrm{gr}(j)$.

On notera que si l’on a une suite exacte $0 \to G' \xrightarrow{u} G \xrightarrow{v} G'' \to 0$
de groupes commutatifs filtrés, où $u$ et $v$ sont compatibles avec les filtrations, la suite $0 \to \mathrm{gr}(G') \xrightarrow{\mathrm{gr}(u)} \mathrm{gr}(G) \xrightarrow{\mathrm{gr}(v)} \mathrm{gr}(G'') \to 0$ n’est pas nécessairement exacte (exerc. 4).

Si maintenant $A$ et $B$ sont deux anneaux filtrés, $h : A \to B$ un homomorphisme d’anneaux compatible avec les filtrations, on vérifie aussitôt que l’homomorphisme de groupes gradués $\mathrm{gr}(h) : \mathrm{gr}(A) \to \mathrm{gr}(B)$ est aussi un homomorphisme d’anneaux. En particulier, si $A'$ est un sous-anneau de $A$ muni de la filtration induite, $\mathrm{gr}(A')$ s’identifie canoniquement à un sous-anneau gradué de $\mathrm{gr}(A)$ (prop. 2); si $b$ est un idéal bilatère de $A$, et si $A/b$ est muni de la filtration quotient, $\mathrm{gr}(A/b)$ s’identifie canoniquement à l’anneau gradué quotient $\mathrm{gr}(A)/\mathrm{gr}(b)$ (prop. 2).

Enfin, soient $A$ un anneau filtré, $E, F$ deux $A$-modules filtrés, $u : E \to F$ un $A$-homomorphisme compatible avec les filtrations. Alors il est immédiat que $\mathrm{gr}(u) : \mathrm{gr}(E) \to \mathrm{gr}(F)$ est une application $\mathrm{gr}(A)$-linéaire, donc un homomorphisme homogène de degré 0 de $\mathrm{gr}(A)$-modules gradués. En outre, si $u' : E \to F$ est un second $A$-homomorphisme compatible avec les filtrations, il en est de même de $u + u'$, et on a
$$
\mathrm{gr}(u + u') = \mathrm{gr}(u) + \mathrm{gr}(u').
$$

#### Remarque 1 {#ac-iii-s2-n4-rem-1 .statement}

Il est clair que les homomorphismes d’anneaux filtrés (resp. de modules filtrés sur un anneau filtré donné $A$) compatibles avec les filtrations peuvent être pris comme morphismes pour la structure d’anneau filtré (resp. de $A$-module filtré) (Ens., chap. IV, § 2, no 1).

#### Remarque 2 {#ac-iii-s2-n4-rem-2 .statement}

Soient E et F deux modules sur un anneau filtré A, et munissons-les des filtrations déduites de la filtration (A_n) de A (n° 1, Exemple 2). Alors toute application A-linéaire u : E → F est compatible avec les filtrations, puisque u(A_nE) = A_nu(E) ⊂ A_nF.

#### Remarque 3 {#ac-iii-s2-n4-rem-3 .statement}

On notera qu’un homomorphisme u : E → F de A-modules filtrés, compatible avec les filtrations, peut être tel que gr(u) = 0 sans être nul ; il en est ainsi par exemple de l’endomorphisme x → nx du groupe additif $\mathbf{Z}$ muni de la filtration (n)-adique (pour un entier $n > 1$ quelconque). La relation gr(u) = gr(v) pour deux endomorphismes u, v de E dans F, compatibles avec les filtrations, n’entraîne donc pas nécessairement $u = v$.

#### Remarque 4 {#ac-iii-s2-n4-rem-4 .statement}

Les définitions du début de ce n° s’étendent immédiatement à deux groupes non nécessairement commutatifs G, G′, filtrés par des sous-groupes $G_n, G'_n$, tels que $G_{n+1}$ (resp. $G'_{n+1}$) soit distingué dans $G_n$ (resp. $G'_n$). La prop. 2 est encore valable en faisant la même hypothèse sur les $G_n$ et en supposant que H est distingué dans G, la démonstration étant inchangée aux notations près.

### 5. Topologie définie par une filtration.

Soit G un groupe filtré par une famille $(G_n)_{n \in \mathbf{Z}}$ de sous-groupes distingués de G. Il existe une topologie et une seule sur G compatible avec la structure de groupe et pour laquelle les $G_n$ constituent un système fondamental de voisinages de l’élément neutre e de G (Top. gén., chap. III, 3e éd., § 1, n° 2, Exemple) ; on l’appelle la topologie de G définie par la filtration $(G_n)$. Lorsqu’on utilisera des notions topologiques relatives à un groupe filtré, il s’agira, sauf mention expresse du contraire, de la topologie définie par la filtration. On notera que les $G_n$, étant des sous-groupes de G, sont à la fois ouverts et fermés (Top. gén., chap. III, 3e éd., § 2, n° 1, cor. de la prop. 4).

Comme chaque $G_n$ est distingué dans G, les entourages des structures uniformes droite et gauche de G coïncident ; on en déduit que G admet un groupe séparé complété $\widehat{G}$ (Top. gén., chap. III, 3e éd., § 3, n° 4, th. 1 et n° 1, prop. 2).

Pour tout partie M de G, l’adhérence de M dans G est égale à $\bigcap_{n \in \mathbf{Z}} (M . G_n) = \bigcap_{n \in \mathbf{Z}} (G_n . M)$ (Top. gén., chap. III, 3e éd., § 3, n° 1, formule (1)) ; en particulier $\bigcap_{n \in \mathbf{Z}} G_n$ est l’adhérence de $\{ e \}$; on voit donc que pour que la topologie de G soit séparée, il faut et il suffit que la filtration $(G_n)$ soit séparée. Pour que la topologie de G soit discrète, il faut et il suffit qu’il existe un $n \in \mathbf{Z}$ tel que $G_n = \{ e \}$ (auquel cas $G_m = \{ e \}$ pour $m \geq n$) ; on dit alors que la filtration $(G_n)$ est discrète.

Le groupe séparé associé à G étant $H = G / (\bigcap_{n \in \mathbf{Z}} G_n )$, les groupes gradués associés gr(G) et gr(H) (lorsque H est muni de la filtration quotient) s’identifient canoniquement.

Soient maintenant $G'$ un second groupe filtré, $u : G \to G'$ un homomorphisme compatible avec les filtrations ; la définition des topologies sur G et $G'$ montre aussitôt que $u$ est continu (*). Si H est un sous-groupe (resp. un sous-groupe distingué) de G, la topologie induite sur H par celle de G (resp. la topologie quotient par H de celle de G) est la topologie sur H (resp. G/H) définie par la filtration induite par celle de G (resp. quotient de celle de G). La topologie produit de celles de G et $G'$ est la topologie définie par le produit des filtrations de G et de $G'$.

Soit $\nu$ la fonction d’ordre (n° 2) de G. L’hypothèse sur les $G_n$ entraîne que $\nu(x y x^{-1}) = \nu(y)$, donc $\nu(x y^{-1}) = \nu(y x^{-1}) = \nu(x^{-1} y) = \nu(y^{-1} x)$ quels que soient x, y dans G. Soit $\rho$ un nombre réel tel que $0 < \rho < 1$ (on peut par exemple prendre $\rho = 1/e$) et posons $d(x, y) = \rho^{\nu(xy^{-1})}$ pour x, y dans G. On a $d(x, x) = 0$, $d(x, y) = d(y, x)$ et l’inégalité (5’) du n° 2 donne

$$
d(x, y) \leq \sup (d(x, z), d(y, z))
$$

pour x, y, z dans G, ce qui entraîne l’inégalité du triangle

$$
d(x, y) \leq d(x, z) + d(y, z).
$$

Donc d est un écart sur G, invariant par translation à droite et à gauche, et $G_n$ est l’ensemble des $x \in G$ tels que $d(e, x) \leq \rho^n$; la

(*) Nous employons dans tout ce chapitre les mots « homomorphisme continu » au sens de ce qui est appelé « représentation continue » dans Top. gén., chap. III, 3e éd., § 2, n° 8 ; le mot « homomorphisme » ne sera jamais employé au sens de Top. gén., chap. III, 3e éd., § 2, n° 8, déf. 1 ; nous utiliserons toujours pour cette notion le terme « morphisme strict » afin d’éviter toute confusion.

structure uniforme définie par $d$ est donc la structure uniforme du groupe topologique $G$. Si $G$ est séparé, $G$ est un espace topologique métrisable éparpillé (*Top. gén.*, chap. IX, 2\textsuperscript{e} éd., § 6, no 4); $d$ est une *distance* sur $G$ si de plus la filtration $(G_n)$ est exhaustive.

Étant donné un anneau topologique $A$, rappelons qu’on appelle *A-module topologique à gauche* un A-module $E$, muni d’une topologie compatible avec sa structure de groupe additif et tel que l’application $(a, x) \to ax$ de $A \times E$ dans $E$ soit continue (*Top. gén.*, chap. III, 3\textsuperscript{e} éd., § 6, no 6).

#### Proposition 3 {#ac-iii-s2-prop-3 .statement}

*Soient A un anneau filtré, $(A_n)$ sa filtration, B le sous-anneau $\bigcup_{n \in \mathbf{Z}} A_n$ de A, E un B-module filtré, $(E_n)$ sa filtration, F le sous-B-module $\bigcup_{n \in \mathbf{Z}} E_n$ de E. Alors l’application $(a, x) \to ax$ de $B \times F$ dans $F$ est continue.*

Soient en effet $a_0 \in B,\ x_0 \in F$; il existe par hypothèse des entiers $r,\ s$ tels que $a_0 \in A_r$ et $x_0 \in E_s$. La relation
$$
ax - a_0x_0 = (a - a_0)x_0 + a_0(x - x_0) + (a - a_0)(x - x_0)
$$
montre que si $a - a_0 \in A_i$ et $x - x_0 \in E_j$, $ax - a_0x_0$ appartient à $E_{i+s} + E_{j+r} + E_{i+j}$. Si donc on suppose donné un entier $n$, on aura $ax - a_0x_0 \in E_n$ pourvu que l’on ait $i \geq n - s,\ j \geq n - r$ et $i + j \geq n$, c’est-à dire dès que $i$ et $j$ sont assez grands.

#### Corollaire {#ac-iii-s2-n5-cor-1 .statement}

*L’anneau B est un anneau topologique et le B-module F un B-module topologique.*

La première assertion s’obtient en appliquant la prop. 3 à $F = B_s$.

On voit en particulier qu’un anneau filtré $A$ dont la filtration est *exhaustive* est un anneau topologique ; lorsqu’il en est ainsi, tout A-module filtré dont la filtration est *exhaustive* est un A-module topologique.

#### Proposition 4 {#ac-iii-s2-prop-4 .statement}

*Soient A un anneau commutatif filtré par une filtration exhaustive $(A_n)$, p un idéal de A. Supposons que l’idéal gr(p) = \bigoplus_{n \in \mathbf{Z}} (p \cap A_n)/(p \cap A_{n+1})\ de\ l'anneau\ gr(A)\ soit\ premier.
Alors l’adhérence de p dans A est un idéal premier.
On sait que l’anneau gr(A/p) est isomorphe à gr(A)/gr(p) (no 4, prop. 2), donc est intègre ; on en conclut que $A / \bigcap_{n \in \mathbf{Z}} (p + A_n)$ est intègre (no 3, cor. de la prop. 1). Donc l’adhérence $\bigcap_{n \in \mathbf{Z}} (p + A_n)$ de p est un idéal premier.

Soient A un anneau, m un idéal bilatère de A ; la topologie définie sur A par la filtration m-adique (no 1, Exemple 3) est dite topologie m-adique ; comme la filtration m-adique est exhaustive, A est un anneau topologique pour cette topologie (cor. de la prop. 3). De même, pour tout A-module E, on appelle topologie m-adique sur E la topologie définie par la filtration m-adique ; E est un A-module topologique pour cette topologie.

Soit m’ un second idéal bilatère de A ; pour que la topologie m’-adique sur A soit plus fine que la topologie m-adique, il faut et il suffit qu’il existe un entier n > 0 tel que ${m'}^n \subset m$ ; la condition est en effet nécessaire, et si elle est remplie, on a ${m'}^{hn} \subset m^h$ pour tout $h > 0$, donc la condition est suffisante. Lorsque A est un anneau commutatif noethérien, il revient au même de dire que l’on a $V(m) \subset V(m')$ dans le spectre premier de A (chap. II, § 4, no 3, cor. 2 de la prop. 11 et § 2, no 6, prop. 15).

### 6. Modules filtrés complets.

#### Proposition 5 {#ac-iii-s2-prop-5 .statement}

Soit G un groupe filtré, dont la filtration $(G_n)$ est formée de sous-groupes distingués de G. Les conditions suivantes sont équivalentes :
a) G est un groupe topologique complet.
b) Le groupe séparé associé $G' = G / (\bigcap_{n \in \mathbf{Z}} G_n)$ est complet.
c) Toute suite de Cauchy dans G est convergente.
Lorsque G est commutatif et noté additivement, ces conditions sont aussi équivalentes à la suivante :
d) Toute famille $(x_\lambda)_{\lambda \in \mathbf{L}}$ d’éléments de G’ qui converge vers 0.

suivant le filtre $\mathfrak{F}$ des complémentaires des parties finies de $L$ est sommable dans $G'$.

Pour qu’un filtre sur $G$ soit un filtre de Cauchy (resp. un filtre convergent), il faut et il suffit que son image par l’application canonique $G \to G'$ soit un filtre de Cauchy (resp. convergent). (*Top. gén.*, chap. II, 3e éd., § 3, no 1, prop. 4); d’où en premier lieu l’équivalence de a) et b); d’autre part, comme $G'$ est métrisable, l’équivalence de b) et c) résulte de la prop. 9 de *Top. gén.*, chap. IX, 2e éd., § 2, no 6.

Supposons maintenant $G$ commutatif. Supposons $G'$ complet, et soit $(x_\lambda)_{\lambda \in L}$ une famille d’éléments de $G'$ qui converge vers 0 suivant $\mathfrak{F}$. Pour tout voisinage $V'$ de 0 dans $G'$ qui est un sous-groupe de $G'$, il existe une partie finie $J$ de $L$ telle que la condition $\lambda \in L - J$ entraîne $x_\lambda \in V'$; on a donc $\sum_{\lambda \in H} x_\lambda \in V'$ pour toute partie finie $H$ de $L$ ne rencontrant pas $J$, ce qui montre que la famille $(x_\lambda)_{\lambda \in L}$ est sommable (*Top. gén.*, chap. III, 3e éd., § 5, no 2, th. 1).

Réciproquement, supposons vérifiée la condition d), et soit $(x_n)$ une suite de Cauchy dans $G'$; la famille $(x_{n+1} - x_n)$ est alors sommable, et en particulier la série de terme général $x_{n+1} - x_n$ est convergente, donc la suite $(x_n)$ est convergente.

Soit $G$ un groupe filtré dont la filtration $(G_n)$ est formée de sous-groupes distingués de $G$; les groupes quotients $G/G_n$ sont *discrets*, donc complets, puisque les $G_n$ sont ouverts dans $G$. Soit $f_n$ l’application canonique $G \to G/G_n$, et pour $m \leq n$, soit $f_{mn}$ l’application canonique $G/G_n \to G/G_m$; $(G/G_n, f_{mn})$ est un système projectif de groupes discrets ayant $\mathbf{Z}$ pour ensemble d’indices (*Top. gén.*, chap. III, 3e éd., § 7, no 3). Soit $\tilde{G}$ le groupe topologique limite projective de ce système projectif, et pour tout $n$, soit $g_n : \tilde{G} \to G/G_n$ l’application canonique; soit $f : G \to \tilde{G}$ la limite projective du système projectif d’applications $(f_n)$, telle que $f_n = g_n \circ f$ pour tout $n$; enfin, soit $j$ l’application canonique de $G$ dans son séparé complété $\hat{G}$; comme les $G/G_n$ sont complets, il existe un isomorphisme et un seul $i : \hat{G} \to \tilde{G}$ de groupes topologiques tel que $f = i \circ j$ (*loc. cit.*, cor. 1 de la prop. 2); nous dirons que c’est l’isomorphisme *canonique* de $\hat{G}$ sur $\tilde{G}$.

Soit $H$ un second groupe filtré dont la filtration $(H_n)$ est formée de sous-groupes distingués de $H$, et soit $u : G \to H$ un homomorphisme compatible avec les filtrations (no 4). Posons $\tilde{H} = \lim_{\leftarrow} H/H_n$; pour tout $n$, $u$ définit par passage aux quotients un homomorphisme $u_n : G/G_n \to H/H_n$, et les $u_n$ forment évidemment un système projectif d'applications ; posons $\tilde{u} = \lim_{\leftarrow} u_n$. Soient par ailleurs $\hat{H}$ le séparé complété de $H$, $\hat{u} : \hat{G} \to \hat{H}$ l'homomorphisme déduit de $u$ par passage aux séparés complétés ($Top. gén.$, chap. II, 3e éd., § 3, no 7, prop. 15). Il résulte aussitôt des définitions que lorsqu'on identifie $\hat{G}$ à $\tilde{G}$ et $\hat{H}$ à $\tilde{H}$ au moyen des isomorphismes canoniques, $\hat{u}$ s'identifie à $\tilde{u}$. On en conclut en particulier que si, pour tout $n$, $u_n$ est un isomorphisme, alors $\hat{u}$ est un isomorphisme de groupes topologiques.

Exemples de groupes et d'anneaux filtrés complets. — 1) Soit $G$ un groupe filtré complet. Tout sous-groupe fermé de $G$ muni de la filtration induite, est complet ($Top. gén.$, chap. II, 3e éd., § 3, no 4, prop. 8). Tout groupe quotient de $G$, muni de la filtration quotient, est complet ($Top. gén.$, chap. IX, 2e éd., § 3, no 1, Remarque 1).

2) Soit $A$ un anneau commutatif filtré, dont nous désignons par $(a_n)_{n \in \mathbf{Z}}$ la filtration ; soit $A'$ l'anneau de séries formelles $A[[X_1, ..., X_s]]$. Pour tout $e = (e_1, ..., e_s) \in \mathbf{N}^s$, nous poserons
$$
|e| = \sum_{i=1}^s e_i, \quad X^e = \prod_{i=1}^s X_i^{e_i},
$$
de sorte que tout élément $P \in A'$ peut s'écrire d'une seule manière $P = \sum_{e \in \mathbf{N}^s} \alpha_{e,P} X^e$ avec $\alpha_{e,P} \in A$.
Pour tout $n \in \mathbf{Z}$, désignons par $a'_n$ l'ensemble des $P \in A'$ tels que $\alpha_{e,P} \in a_{n-|e|}$ pour tout $e \in \mathbf{N}^s$ ; il est clair que $a'_n$ est un sous-groupe additif de $A'$ ; d'autre part, si $P \in a'_n$ et $Q \in a'_m$ on a, pour $e \in \mathbf{N}^s$,
$$
\alpha_{e,PQ} = \sum_{e'+e''=e} \alpha_{e',Q} \alpha_{e'',P}
$$
et la relation $e'+e''=e$ entraîne $\alpha_{e',Q} \alpha_{e'',P} \in a_{m-|e'|} a_{n-|e''|} \subset a_{m+n-|e|}$, ce qui prouve que $(a'_n)_{n \in \mathbf{Z}}$ est une filtration compatible avec la structure d'anneau de $A'$ (car on a évidemment $1 \in a'_0$). Lorsqu'on parlera désormais de $A'$ comme d'un anneau filtré, il s'agira touno 6 GÉNÉRALITÉS SUR ANNEAUX ET MODULES FILTRÉS 209
jours, sauf mention expressé du contraire, de la filtration $(\alpha'_n)$.
Il est clair que $\bigcap_{n \in \mathbf{Z}} \alpha'_n$ est l’ensemble des séries formelles dont tous les coefficients appartiennent à $\bigcap_{n \in \mathbf{Z}} \alpha_n$; donc, si $A$ est séparé, il en est de même de $A'$. Si $\alpha_0 = A$, on a $\alpha'_0 = A'$.

#### Proposition 6 {#ac-iii-s2-prop-6 .statement}

Les notations étant comme ci-dessus, supposons que $\alpha_0 = A$, et désignons par $h$ l’application $P \to (\alpha_{e,P})_{e \in \mathbf{N}^s}$.
Alors $h$ est un isomorphisme du groupe additif topologique $A'$ sur le groupe additif topologique $A^{\mathbf{N}^s}$. L’anneau de polynômes $A[X_1, ..., X_s]$ est dense dans $A'$; si $A$ est complet, il en est de même de $A'$.

Il est clair que $h$ est bijective ; $V_n = h(\alpha'_n)$ est l’ensemble des $(a_e) \in A^{\mathbf{N}^s}$ tels que $a_e \in \alpha_{n-|e|}$ pour tout $e \in \mathbf{N}^s$ tel que $|e| \leq n$; comme ces éléments $e$ sont en nombre fini, $V_n$ est un voisinage de 0 dans $A^{\mathbf{N}^s}$. Inversement, si $V$ est un voisinage de 0 dans $A^{\mathbf{N}^s}$, il y a une partie finie $E$ de $\mathbf{N}^s$ et un entier $v$ tel que les conditions $a_e \in \alpha_v$ pour tout $e \in E$ entraînent $(a_e) \in V$; si donc $n$ est le plus grand des entiers $v + |e|$ pour $e \in E$, on a $h(\alpha'_n) \subset V$, ce qui prouve la première assertion de la prop. 6. De plus, $n$ et $E$ étant définis comme ci-dessus, on a $h(P - \sum_{e \in E} \alpha_{e,P} X^e) \in V$ pour tout $P \in A'$, ce qui montre que $A[X_1, ..., X_s]$ est dense dans $A'$. La dernière assertion résulte de la première et du fait qu’un produit d’espaces complets est complet.

Soit $m$ un idéal de $A$ et supposons que $(\alpha_n)$ soit la filtration $m\text{-adique}$; alors, si $n$ est l’idéal de $A'$ engendré par $m$ et les $X_i$ ($1 \leq i \leq s$), la filtration $(\alpha'_n)$ est la filtration $n\text{-adique}$. En effet, il est clair que pour tout $k \geq 0$, $n^k$ est engendré par les éléments $aX^e$ tels que $a \in m^{k-|e|}$ pour tout $e \in \mathbf{N}^s$ tel que $|e| \leq k$, d’où $n^k \subset \alpha'_k$. Prouvons inversement que $\alpha'_k \subset n^k$. Pour tout $P \in \alpha'_k$, on a $P = P' + P''$, avec $P' = \sum_{|e| < k} \alpha_{e,P} X^e$, $P'' = \sum_{|e| \geq k} \alpha_{e,P} X^e$. Il est clair que l’on peut écrire $P'' = \sum_{|e|=k} X^e Q_e$, où les $Q_e$ sont des éléments de $A'$, d’où $P'' \in n^k$; par ailleurs, il est clair que $\alpha_{e,P} X^e \in n^k$ pour tout $e \in \mathbf{N}^s$, d’où $P' \in n^k$. On a donc bien $n^k = \alpha'_k$.

#### Corollaire {#ac-iii-s2-n6-cor-1 .statement}

Soient $A$ un anneau commutatif,
$$
A' = A[[X_1, ..., X_s]]
$$
l’anneau de séries formelles à s indéterminées sur $A$, $\mathfrak{n}$ l’idéal de $A'$ formé des séries formelles sans terme constant. L’anneau $A'$ est séparé et complet pour la topologie $\mathfrak{n}$-adique, et l’anneau de polynômes $A[X_1, ..., X_s]$ est partout dense dans $A'$.

Il suffit d’appliquer ce qui vient d’être dit au cas $m = \{0\}$.

### 7. Propriétés de compacité linéaire des modules filtrés complets.

Rappelons que si $E$ est un $A$-module, on appelle partie affine (ou variété linéaire affine) de $E$ toute partie $F$ qui est vide ou de la forme $a + M$, où $a \in E$ et $M$ est un sous-module de $E$, appelé direction de $F$ (Alg., chap. II, 3e éd., § 9, nos 1 et 3).

#### Proposition 7 {#ac-iii-s2-prop-7 .statement}

Soient $A$ un anneau filtré, $E$ un $A$-module filtré, $(E_n)$ la filtration de $E$; on suppose que $E_0 = E$, que les $E_n$ sont des sous-modules de $E$, que les $A$-modules $E/E_n$ sont artiniens, et enfin que le groupe topologique $E$ est séparé et complet. Alors l’intersection d’une suite décroissante de parties affines fermées non vides de $E$ est non vide.

On a vu au no 6 que $E$, étant séparé et complet, s’identifie à $\tilde{E} = \lim_{\leftarrow} E/E_n$. Soit $(W_p)$ une suite décroissante de parties affines fermées non vides de $E$, et pour tout $n \geq 0$, soit $W_{p,n}$ l’image canonique de $W_p$ dans $E/E_n$; nous allons construire une suite $x = (x_n) \in \tilde{E}$ telle que $x_n \in W_{p,n}$ pour tout $p$ et tout $n$; on aura donc $x \in W_p + E_n$ pour tout $p$ et tout $n$, et comme les $W_p$ sont fermés, $x \in W_p$ pour tout $p$ (no 5), ce qui démontrera la proposition.

Comme $E/E_0 = 0$, nous prendrons $x_0 = 0$. Supposons définis les $x_i$ pour $0 \leq i \leq n - 1$, et soit $W'_{p,n}$ l’ensemble des éléments de $W_{p,n}$ dont l’image canonique dans $E/E_{n-1}$ est $x_{n-1}$; comme $x_{n-1} \in W_{p,n-1}$ et que $W_{p,n-1}$ est l’image canonique de $W_{p,n}$, $W'_{p,n}$ n’est pas vide, et est évidemment une partie affine de $E/E_n$; en outre la suite $(W'_{p,n})_{p \in \mathbf{N}}$ est décroissante. Comme $E/E_n$ est artinien, cette suite est stationnaire (sans quoi la suite des sousmodules de $E/E_n$ qui sont les directions des $W'_{p,n}$, serait strictement décroissante, ce qui est absurde). Il suffit alors de prendre pour $x_n$ un élément de $\bigcap_{p \in \mathbf{N}} W'_{p,n}$ et la construction de $(x_n)$ peut donc se faire par récurrence.

#### Proposition 8 {#ac-iii-s2-prop-8 .statement}

*On suppose que A et E vérifient les hypothèses de la prop. 7. Soit $(F_p)$ une suite décroissante de sous-modules fermés de E tels que $\bigcap_p F_p = 0$. Alors, pour tout voisinage V de 0 dans E, il existe $p$ tel que $F_p \subset V$ (autrement dit, la base de filtre $(F_p)$ converge vers 0).

On peut supposer que V est l’un des $E_n$, auquel cas $E/V$ est artinien. Posons $F'_p = (F_p + V)/V$; comme les $F'_p$ forment une suite décroissante de sous-modules de $E/V$, il existe un entier $j$ tel que $F'_p = F'_j$ pour tout $p \geq j$. Nous allons voir que $F'_j = \{0\}$, ce qui achèvera la démonstration. Soit $x \in F'_j$, et soit $W_p$ l’ensemble des éléments de $F_p$ dont l’image dans $E/V$ est $x$ ($p \geq j$); par définition de $j$, les $W_p$ sont des parties affines fermées *non vides* de E, et on a évidemment $W_{p+1} \subset W_p$; il résulte donc de la prop. 7 qu’il existe un élément $y$ appartenant à tous les $W_p$. Comme $W_p \subset F_p$ et que $\bigcap_{p \in \mathbf{N}} F_p = \{0\}$, on a $y = 0$; puisque $x$ est l’image canonique de $y$ dans $E/V$, on a bien $x = 0$ (cf. exerc. 15 à 21).

### 8. Relèvement d’homomorphismes de modules gradués associés.

#### Théorème 1 {#ac-iii-s2-thm-1 .statement}

*Soient X, Y deux groupes filtrés dont les filtrations $(X_n)$, $(Y_n)$ sont formées de sous-groupes distingués ; soit $u : X \to Y$ un homomorphisme compatible avec les filtrations.

(i) *Supposons la filtration $(X_n)$ exhaustive.* Pour que $\mathrm{gr}(u)$ soit *injectif*, il faut et il suffit que $\bar{u}^{-1}(Y_n) = X_n$ pour tout $n \in \mathbf{Z}$.

(ii) *Supposons vérifiée l’une des hypothèses suivantes :* $\alpha)$ X est complet et Y séparé ; $\beta)$ Y est discret. *Alors, pour que $\mathrm{gr}(u)$ soit surjectif*, il faut et il suffit que $Y_n = u(X_n)$ pour tout $n \in \mathbf{Z}$.*

(i) Dire que l’application gr_n(u) est injective signifie que l’on a

$$
X_n \cap \bar{u}^{-1}(Y_{n+1}) \subset X_{n+1}.
$$

C’est évidemment le cas si $\bar{u}^{-1}(Y_{n+1}) = X_{n+1}$. Inversement, si on a $X_n \cap \bar{u}^{-1}(Y_{n+1}) \subset X_{n+1}$ pour tout $n$, on en déduit, par récurrence sur $k$, que $X_{n-k} \cap \bar{u}^{-1}(Y_{n+1}) \subset X_{n+1}$ pour tout $n \in \mathbf{Z}$ et tout $k \geq 0$. Comme la filtration $(X_n)$ est exhaustive, on voit que, pour tout $n$, $X$ est réunion des $X_{n-k}$ ($k \geq 0$), donc $\bar{u}^{-1}(Y_{n+1}) \subset X_{n+1}$ pour tout $n$ et on a par hypothèse $X_{n+1} \subset \bar{u}^{-1}(Y_{n+1})$, ce qui achève la démonstration.

(ii) Dire que l’application gr_n(u) est surjective signifie que l’on a

$$
Y_n = u(X_n) Y_{n+1}.
$$

C’est évidemment le cas si $Y_n = u(X_n)$. Réciproquement, supposons que $Y_n = u(X_n) Y_{n+1}$ pour tout $n \in \mathbf{Z}$. Soient $n$ un entier, $y$ un élément de $Y_n$; on va définir une suite $(x_k)_{k \geq 0}$ d’éléments de $X_n$ telle que l’on ait $x_k \in X_n,\ x_{k+1} \equiv x_k \pmod{X_{n+k}}$ et $u(x_k) \equiv y \pmod{Y_{n+k}}$ pour tout $k \geq 0$. Nous prendrons $x_0$ égal à l’élément neutre de $X$, ce qui donne bien $u(x_0) \equiv y \pmod{Y_n}$. Supposons construit un $x_k \in X_n$ tel que $u(x_k) \equiv y \pmod{Y_{n+k}}$; on a $(u(x_k))^{-1} y \in Y_{n+k}$; l’hypothèse entraîne qu’il existe $t \in X_{n+k}$ tel que $u(t) \equiv (u(x_k))^{-1} y \pmod{Y_{n+k+1}}$, donc $u(x_{kt}) \equiv y \pmod{Y_{n+k+1}}$; il suffit de prendre $x_{k+1} = x_{kt}$ pour poursuivre la récurrence. Cela étant, si $Y$ est discret, il existe un $k \geq 0$ tel que $Y_{n+k} = \{ e' \}$ (élément neutre de $Y$), d’où $u(x_k) = y$, et on a donc dans ce cas prouvé que $u(X_n) = Y_n$ pour tout $n$. Supposons maintenant $X$ complet et $Y$ séparé. Comme $x_h^{-1} x_k \in X_{n+k}$ pour $h \geq k \geq 0$, $(x_k)$ est une suite de Cauchy dans $X_n$; comme $X_n$ est fermé dans $X$, donc complet, cette suite a au moins une limite $x$ dans $X_n$. En vertu de la continuité de $u$, $u(x)$ est l’unique limite de la suite $(u(x_k))$ dans $Y$, $Y$ étant séparé. Mais les relations $u(x_k) \equiv y \pmod{Y_{n+k+1}}$ montrent que $y$ est aussi limite de cette suite, d’où $u(x) = y$ et on a encore prouvé que $u(X_n) = Y_n$.

C. Q. F. D.

#### Corollaire 1 {#ac-iii-s2-thm-1-cor-1 .statement}

Supposons que $X$ soit séparé et sa filtration exhaustive. Alors, si gr(u) est injectif, $u$ est injectif.

Soient $e, e'$ les éléments neutres de $X$ et $Y$ respectivement. On a
$$
u^{-1}(e') \subset \bigcap_n u^{-1}(Y_n) = \bigcap_n X_n = \{ e \}
$$
par hypothèse, d'où le corollaire.

#### Corollaire 2 {#ac-iii-s2-thm-1-cor-2 .statement}

Supposons vérifiée l'une des hypothèses suivantes :
$\alpha)$ $X$ est complet, $Y$ est séparé et sa filtration est exhaustive ;
$\beta)$ $Y$ est discret et sa filtration est exhaustive.
Alors, si $\mathrm{gr}(u)$ est surjectif, $u$ est surjectif.
En effet, on a alors $Y = \bigcup_n Y_n = \bigcup_n u(X_n) \subset u(X)$.

#### Corollaire 3 {#ac-iii-s2-thm-1-cor-3 .statement}

Supposons $X$ et $Y$ séparés, les filtrations de $X$ et $Y$ exhaustives et $X$ complet. Alors, si $\mathrm{gr}(u)$ est bijectif, $u$ est bijectif.

Soient $A$ un anneau local, $m$ son idéal maximal, $M$ un $A$-module ; munissons $A$ et $M$ des filtrations $m$-adiques et soient $\mathrm{gr}(A)$ et $\mathrm{gr}(M)$ l'anneau gradué et le $\mathrm{gr}(A)$-module gradué associés à $A$ et $M$. On a vu (n° 3, Exemple 3) que l'application canonique (11) est toujours surjective ; nous allons considérer la propriété suivante de $M$ :

(GR) L'application canonique
$$
\gamma_M : \mathrm{gr}(A) \otimes_{\mathrm{gr}_0(A)} \mathrm{gr}_0(M) \to \mathrm{gr}(M)
$$
est bijective.

#### Proposition 9 {#ac-iii-s2-prop-9 .statement}

Soient $A$ un anneau local, $m$ son idéal maximal, $M, N$ deux $A$-modules, $u : N \to M$ un $A$-homomorphisme. On munit $M$ et $N$ des filtrations $m$-adiques, et on suppose que : $1^\circ$ $M$ vérifie la propriété (GR) ; $2^\circ$ $\mathrm{gr}_0(u) : \mathrm{gr}_0(N) \to \mathrm{gr}_0(M)$ est injectif. Alors $\mathrm{gr}(u) : \mathrm{gr}(N) \to \mathrm{gr}(M)$ est injectif, $N$ et $P = \mathrm{Coker}\,(u)$ vérifient la propriété (GR), et on a $m^n N = \overline{u}^{-1}(m^n M)$ pour tout entier $n > 0$.

On vérifie aussitôt que le diagramme

$$
\begin{array}{ccc}
\mathrm{gr}(A) \otimes_{\mathrm{gr}_0(A)} \mathrm{gr}_0(N) & \xrightarrow{1 \otimes \mathrm{gr}_0(u)} & \mathrm{gr}(A) \otimes_{\mathrm{gr}_0(A)} \mathrm{gr}_0(M) \\
\gamma_N \downarrow & & \downarrow \gamma_M \\
\mathrm{gr}(N) & \xrightarrow{\mathrm{gr}(u)} & \mathrm{gr}(M)
\end{array}
$$

est commutatif. Comme $\mathrm{gr}_0(A) = A/m$ est un corps, l’hypothèse entraîne que $1 \otimes \mathrm{gr}_0(u)$ est injectif ; comme par hypothèse $\gamma_M$ est injectif, il en est de même de $\gamma_M \circ (1 \otimes \mathrm{gr}_0(u))$. Ceci entraîne d’abord que $\gamma_N$ est injectif, donc bijectif, et ensuite que $\mathrm{gr}(u)$ est injectif. La formule $\tilde{u}^1(m^n M) = m^n N$ est alors conséquence du th. 1, (i).

En outre, posons $N' = u(N)$, et soit $j : N' \to M$ l’injection canonique. Si $p : M \to P = M/N'$ est l’homomorphisme canonique, alors, dans le diagramme commutatif

$$
\begin{array}{ccccccccc}
\mathrm{gr}(A) \otimes \mathrm{gr}_0(N') & \xrightarrow{1 \otimes \mathrm{gr}_0(j)} & \mathrm{gr}(A) \otimes \mathrm{gr}_0(M) & \xrightarrow{1 \otimes \mathrm{gr}_0(p)} & \mathrm{gr}(A) \otimes \mathrm{gr}_0(P) & \to & 0 \\
\gamma_{N'} \downarrow & & \gamma_M \downarrow & & \gamma_P \downarrow & & \\
\mathrm{gr}(N') & \xrightarrow{\mathrm{gr}(j)} & \mathrm{gr}(M) & \xrightarrow{\mathrm{gr}(p)} & \mathrm{gr}(P) & \longrightarrow & 0
\end{array}
$$

la ligne du bas est exacte (n° 4, prop. 2), et il en est de même de la ligne du haut, en vertu de la prop. 2 du n° 4 et du fait que $\mathrm{gr}_0(A)$ est un corps. D’ailleurs, $\mathrm{gr}(j)$ est injectif (n° 4, prop. 2), donc $\mathrm{gr}_0(j)$ est injectif. La première partie du raisonnement, appliquée à $j$, montre que $\gamma_{N'}$ est bijectif ; comme il en est de même de $\gamma_M$ par hypothèse, on en conclut que $\gamma_P$ est bijectif (chap. I, § 1, n° 4, cor. 2 de la prop. 2).

#### Corollaire {#ac-iii-s2-n8-cor-1 .statement}

Sous les hypothèses de la prop. 9, si on suppose en outre $N$ séparé pour la filtration m-adique, alors $u$ est injectif.

En effet, cela résulte de ce que $\mathrm{gr}(u)$ est injectif (cor. 1 du th. 1).

*Remarque. — Supposons vérifiées les hypothèses de la prop. 9, et en outre l’une des conditions suivantes :
1° $m$ est nilpotent ;
2° $A$ est noethérien, et $P$ idéalement séparé (cf. § 5, n° 1) ; alors $P$ est un $A$-module plat. Cela résulte en effet de ce que $\gamma_P$ est bijectif et du § 5, n° 2, th. 1, (iv), puisque $A/m$ est un corps.*

### 9. Relèvement de familles d’éléments d’un module gradué associé.

Soient $A$ un anneau commutatif filtré, $(A_n)_{n \in \mathbf{Z}}$ sa filtration, $C$ un sous-anneau de $A_0$ tel que $C \cap A_1 = \{0\}$. La restriction à $C$ de l’application canonique $A_0 \to A_0/A_1 = \mathrm{gr}_0(A)$ est alors injective, ce qui permet d’identifier $C$ à un sous-anneau de $\mathrm{gr}_0(A)$; c’est ce que nous ferons d’ordinaire en pareil cas. Si $A_1 \neq A_0$ et si $K$ est un sous-corps quelconque de $A_0$, on a $K \cap A_1 = \{0\}$ puisque $K \cap A_1$ est un idéal de $K$ ne contenant pas 1 ; on peut donc identifier $K$ à un sous-corps de $\mathrm{gr}_0(A)$.

#### Proposition 10 {#ac-iii-s2-prop-10 .statement}

Soient $A$ un anneau commutatif filtré, $(A_n)$ sa filtration ; on suppose qu’il existe un sous-anneau $C$ de $A_0$ tel que $C \cap A_1 = \{0\}$ et on identifie $C$ à un sous-anneau de $\mathrm{gr}_0(A)$. Soit $(x_i)_{1 \leq i \leq q}$ une famille finie d’éléments de $A$ ; supposons que $x_i \in A_{n_i}$ pour $1 \leq i \leq q$, et soit $\xi_i$ la classe de $x_i$ dans $\mathrm{gr}_{n_i}(A)$ pour $1 \leq i \leq q$.

(i) Si la famille $(\xi_i)$ d’éléments de $\mathrm{gr}(A)$ est algébriquement libre sur $C$, la famille $(x_i)$ est algébriquement libre sur $C$.

(ii) Si la filtration de $A$ est exhaustive et discrète et si $(\xi_i)$ est un système de générateurs de la $C$-algèbre $\mathrm{gr}(A)$, alors $(x_i)$ est un système de générateurs de la $C$-algèbre $A$.

Soit $A'$ l’algèbre de polynômes $C[X_1, ..., X_q]$ sur $C$ ; munissons $A'$ de la graduation $(A'_n)$ de type $\mathbf{Z}$ pour laquelle $A'_n$ est l’ensemble des combinaisons $C$-linéaires des monômes $X_1^{s(1)} ... X_q^{s(q)}$ tels que $\sum_{i=1}^q n_i s(i) = n$. Soit $u$ l’homomorphisme $f \to f(x_1, ..., x_q)$ de la $C$-algèbre $A'$ dans la $C$-algèbre $A$ ; par définition, on a $u(A'_n) \subset A_n$ pour tout $n \in \mathbf{Z}$, donc $u$ est compatible avec les filtrations ($A'$ étant muni de sa structure d’anneau filtré associé à sa structure d’anneau gradué, cf. no 1, Exemple 1). Cela étant, l’hypothèse de (i) signifie que $\mathrm{gr}(u) : A' = \mathrm{gr}(A') \to \mathrm{gr}(A)$ est injectif ; comme la filtration de $A'$ est exhaustive et séparée, on peut appliquer le cor. 1 du th. 1 du no 8, et $u$ est injectif, ce qui démontre la conclusion de (i). De même l’hypothèse (ii) sur les $(\xi_i)$ signifie que $\mathrm{gr}(u)$ est surjectif ; comme $A$ est discret et que sa filtration est exhaustive, on peut appliquer le cor. 2 du th. 1 du n° 8 et $u$ est surjectif, ce qui prouve la conclusion de (ii).

#### Proposition 11 {#ac-iii-s2-prop-11 .statement}

*Soient A un anneau commutatif filtré, séparé et complet, C un sous-anneau de $A_0$ tel que $C \cap A_1 = \{0\}$, $(x_i)_{1 \leq i \leq q}$ une famille finie d’éléments de A telle que $x_i \in A_{n_i}$ avec $n_i > 0$ pour $1 \leq i \leq q$; soit $\xi_i$ la classe de $x_i$ dans $\mathrm{gr}_{n_i}(A)$ pour $1 \leq i \leq q$.

(i) *Il existe un C-homomorphisme et un seul $\nu$ de l’algèbre de séries formelles $A'' = C[[X_1, ..., X_q]]$ dans A tel que $\nu(X_i) = x_i$ pour $1 \leq i \leq q$.

(ii) *Si la famille $(\xi_i)$ est algébriquement libre sur C, l’homomorphisme $\nu$ est injectif.

(iii) *Si la filtration de A est exhaustive et si la famille $(\xi_i)$ est un système de générateurs de la C-algèbre $\mathrm{gr}(A)$, l’homomorphisme $\nu$ est surjectif.

Comme $n_i \geq 1$ pour tout $i$, on a $\sum_{i=1}^q n_i s(i) \geq \sum_{i=1}^q s(i)$ pour tout monôme $X_1^{s(1)} ... X_q^{s(q)}$, et d’autre part $\sum_{i=1}^q n_i s(i) \leq r \cdot \sum_{i=1}^q s(i)$ si $r$ est le plus grand des $n_i$. Si l’on désigne par $A''_n$ l’ensemble des séries formelles dont les termes non nuls $a_s X_1^{s(1)} ... X_q^{s(q)}$ sont tels que $\sum_{i=1}^q n_i s(i) \geq n$, il résulte du n° 6, cor. de la prop. 6 que $A''$ est séparé et complet pour la filtration exhaustive ($A''_n$) et que $A' = C[X_1, ..., X_q]$ est dense dans $A''$; en outre l’homomorphisme $u$ défini dans la démonstration de la prop. 10 est *continu* dans $A'$ et se prolonge donc de façon unique en un homomorphisme continu $\nu : A'' \to A$, puisque A est séparé et complet (*Top. gén.*, chap. III, 3e éd.; § 3, n° 3, prop. 5), ce qui démontre (i); en outre, on a $\mathrm{gr}(A'') = \mathrm{gr}(A')$ et $\mathrm{gr}(\nu) = \mathrm{gr}(u)$; (ii) et (iii) résultent donc respectivement des cor. 1 et 2 du th. 1 du n° 8, vu les hypothèses sur A.

On exprime parfois la conclusion de (ii) (resp. (iii)) dans le corollaire en disant que la famille $(x_i)$ est *formellement libre sur C* (resp. est un *système formel de générateurs* de A).

#### Proposition 12 {#ac-iii-s2-prop-12 .statement}

Soient A un anneau filtré, E un A-module filtré, (A_n) et (E_n) les filtrations respectives de A et E. On suppose A complet, et la filtration (E_n) exhaustive et séparée. Soit (x_i)_{i \in I} une famille finie d’éléments de E et, pour tout i \in I, soit n(i) un entier tel que x_i \in E_{n(i)} ; soit enfin \xi_i la classe de x_i dans gr_{n(i)}(E). Alors, si (\xi_i) est un système de générateurs du gr(A)-module gr(E), (x_i) est un système de générateurs du A-module E.

Dans le A-module L = A_s^I, désignons par L_n l’ensemble des (a_i) tels que a_i \in A_{n-n(i)} pour tout i \in I ; si p et q sont le plus petit et le plus grand des n(i), on a A_{n-q}^I \supset L_n \supset A_{n-p}^I, et la topologie définie sur L par la filtration (L_n) est la même que la topologie produit ; donc L est un A-module filtré complet. Comme L est libre, il existe une application A-linéaire u : L \to E telle que u((a_i)) = \sum_{i \in I} a_i x_i, et elle est évidemment compatible avec les filtrations ; nous devons prouver que u est surjective, et pour cela, il suffit, en vertu du cor. 2 du th. 1, no 8, de montrer que gr(u) : gr(L) \to gr(E) est surjective, ou encore que, pour tout x \in E_n, il existe une famille (a_i) telle que a_i \in A_{n-n(i)} pour tout i \in I et x \equiv \sum_{i \in I} a_i x_i \pmod{E_{n+1}}. Soit \xi la classe de x dans gr_n(E) ; puisque les \xi_i engendrent le gr(A)-module gr(E), il existe des \alpha_i \in gr(A) tels que \xi = \sum_{i \in I} \alpha_i \xi_i, et on peut supposer que \alpha_i \in gr_{n-n(i)}(A), en remplaçant au besoin \alpha_i par sa composante homogène de degré n - n(i). Alors \alpha_i est l’image d’un élément a_i \in A_{n-n(i)}, et la famille (a_i) possède la propriété requise.

#### Corollaire 1 {#ac-iii-s2-prop-12-cor-1 .statement}

Soient A un anneau filtré complet, E un A-module filtré dont la filtration est exhaustive et séparée. Si gr(E) est un gr(A)-module de type fini (resp. noethérien), alors E est un A-module de type fini (resp. noethérien).

Si gr(E) est de type fini, il a un système fini de générateurs homogènes, et la prop. 12 montre que E est de type fini. Supposons maintenant gr(E) noethérien, et soit F un sous-module de E ; la filtration induite sur F par celle de E est exhaustive et séparée et gr(F) s’identifie à un sous-gr(A)-module de gr(E) (no 4, prop. 2), donc est de type fini par hypothèse ; on en conclut que F est un A-module de type fini, donc E est noethérien.

#### Corollaire 2 {#ac-iii-s2-prop-12-cor-2 .statement}

Soit $A$ un anneau filtré séparé et complet, dont la filtration est exhaustive. Si $\mathrm{gr}(A)$ est un anneau noethérien à gauche, il en est de même de $A$.

Il suffit d’appliquer le cor. 1 à $E = A_s$.

#### Corollaire 3 {#ac-iii-s2-prop-12-cor-3 .statement}

Soient $A$ un anneau filtré complet, $(A_n)$ sa filtration, $E$ un $A$-module filtré séparé, $(E_n)$ sa filtration, $F$ un sous-module de type fini de $E$; on suppose $A_0 = A$ et $E_0 = E$.

(i) Si, pour tout $k \geqslant 0$, on a $E_k = E_{k+1} + A_k F$, alors $F = E$.

(ii) Si on suppose de plus que la filtration de $E$ est déduite de celle de $A$ (no 1, Exemple 2), la relation $E = E_1 + F$ entraîne $F = E$.

Soient $\xi_i$ ($1 \leqslant i \leqslant n$) les classes mod. $E_1$ d’un système fini de générateurs de $F$. Il résulte de l’hypothèse faite que pour tout $k \geqslant 0$, tout élément de $\mathrm{gr}_k(E)$ se met sous la forme $\sum_{i=1}^n \alpha_i \xi_i$ avec $\alpha_i \in \mathrm{gr}(A)$; les $\xi_i$ engendrent donc le $\mathrm{gr}(A)$-module $\mathrm{gr}(E)$, ce qui démontre (i), en vertu de la prop. 12. Si la filtration de $E$ est déduite de celle de $A$, la relation $E = E_1 + F$, entraîne $E_k = A_k E = A_k E_1 + A_k F = A_k A_1 E + A_k F \subset A_{k+1} E + A_k F = E_{k+1} + A_k F \subset E_k$, d’où (ii).

#### Proposition 13 {#ac-iii-s2-prop-13 .statement}

Soient $A$ un anneau, $m$ un idéal bilatère de $A$ contenu dans le radical de $A$, $E$ un $A$-module. On munit $A$ et $E$ des filtrations $m$-adiques (no 1, Exemple 3). On suppose que l’une des conditions suivantes est vérifiée :

a) $E$ est un $A$-module de type fini et $A$ est séparé ;
b) $m$ est nilpotent.

Pour que $E$ soit un $A$-module libre, il faut et il suffit que $E/mE$ soit un $(A/m)$-module libre et que $E$ vérifie la propriété (GR) (no 8).

Si $E$ est un $A$-module libre, et $(e_\lambda)$ une base de $E$, $m^k E$ est somme directe des sous-modules $m^k e_\lambda$ de $E$ pour tout $k \geqslant 0$ (Alg., chap. II, 3e éd., § 3, no 7, Remarque) ; par suite $m^k E/m^{k+1} E$ s’identifie à la somme directe des $m^k e_\lambda / m^{k+1} e_\lambda$ (Alg., chap. II, 3e éd., § 1, no 6, prop. 7). On en déduit d’abord (pour $k = 0$) que les classes $1 \otimes e_\lambda$ des $e_\lambda$ dans $E/mE = (A/m) \otimes_A E$ forment une base du $(A/m)$-module $E/mE$, puis que l’application canonique

$$
(m^k/m^{k+1}) \otimes_A (E/mE) \to m^k E/m^{k+1} E
$$

est bijective pour tout $k \geq 0$; donc $\gamma_E$ est bijective. On notera que cette partie de la démonstration n’utilise pas la condition a) ni b).

Supposons inversement vérifiées les conditions de l’énoncé, et soit $(x_i)_{i \in I}$ une famille d’éléments de $E$ dont les classes mod. $mE$ forment une base du $(A/m)$-module $E/mE$; soient $L$ le $A$-module libre $A_s^{(I)}$, $(f_i)_{i \in I}$ sa base canonique, et $u : L \to E$ l’application $A$-linéaire telle que $u(f_i) = x_i$ pour tout $i \in I$. Les hypothèses entraînent déjà que $u$ est surjective (chap. II, § 3, n° 2, cor. 1 de la prop. 4), et il reste à prouver que $u$ est injective. Or, chacune des hypothèses $a), b)$ entraîne que $A$ est séparé, donc il en est de même de $L$ muni de la filtration $m$-adique, puisque $m^kL = (m^k)^{(I)}$ (\emph{Alg.}, chap. II, 3e éd., § 3, n° 7, *Remarque*), et gr$(L)$ s’identifie à gr$(A) \otimes_{A/m} (L/mL)$ d’après la première partie de la démonstration ; l’homomorphisme $u$ est compatible avec les filtrations et on peut écrire $\operatorname{gr}(u) = \gamma_E \circ \varphi$ où $\varphi$ est la bijection de gr$(L)$ sur gr$(A) \otimes_{A/m} (E/mE)$ appliquant la classe de $f_i$ mod. $mM$ sur $1 \otimes \bar{x}_i$, où $\bar{x}_i$ est la classe de $x_i$ mod. $mE$. L’hypothèse entraîne donc que gr$(u)$ est injectif et on conclut à l’aide du cor. 1 du th. 1, n° 8.

### 10. Application : exemples d’anneaux noethériens.

#### Lemme 1 {#ac-iii-s2-lem-1 .statement}

Soit $A$ un anneau gradué de type $\mathbf{Z}$, dont la graduation $(A_n)$ est telle que $A_n = 0$ pour tout $n < 0$, ou $A_n = 0$ pour tout $n > 0$. Soit $M$ un $A$-module gradué de type $\mathbf{Z}$. Pour que $M$ soit un $A$-module noethérien, il faut et il suffit que tout sous-module gradué de $M$ soit de type fini.

Comme $n \to -n$ est un automorphisme du groupe $\mathbf{Z}$, on peut se borner au cas où $A_n = 0$ pour tout $n > 0$. Désignons par $A'$ et $M'$ l’anneau $A$ et le module $M$ munis des filtrations associées à leurs graduations respectives (n° 1, *Exemple 1*), qui sont exhaustives et séparées ; l’hypothèse sur $A$ entraîne que $A'$ est discret, donc complet. Si $E$ est un sous-$A$-module de $M$, le $A'$-module filtré $E'$ obtenu en munissant $E$ de la filtration induite est séparé et sa filtration est exhaustive ; en outre $\operatorname{gr}(E')$ s’identifie à un sous-$A$-module gradué de $M = \operatorname{gr}(M')$, donc est de type fini par hypothèse. La conclusion résulte donc du cor. 1 de la prop. 12 du n° 9.

#### Théorème 2 {#ac-iii-s2-thm-2 .statement}

Soient $A$ un anneau gradué de type $\mathbf{N}$, $M$ un $A$-module gradué de type $\mathbf{N}$, $(A_n)$ et $(M_n)$ leurs graduations respectives. On suppose qu’il existe un élément $a \in A_1$ tel que $A_n = A_0 a^n$ et $M_n = a^n M_0$ pour tout $n > 0$. Alors, si $M_0$ est un $A_0$-module noethérien, $M$ est un $A$-module noethérien.

En vertu du lemme 1, il suffit de prouver que tout sous-module gradué $N$ de $M$ est de type fini. Pour tout $r \geqslant 0$, soit $N_r = N \cap M_r$ et soit $L_r$ l’ensemble des $m \in M_0$ tels que $a^r m \in N_r$. Comme $a^r A_0 \subset A_r = A_0 a^r$ on a $a^r A_0 L_r \subset A_0 a^r L_r \subset A_0 N_r \subset N_r$, donc les $L_r$ sont des sous-$A_0$-modules de $M_0$; en outre on a
$$
aN_r \subset N \cap aM_r = N \cap M_{r+1} = N_{r+1},
$$
donc la suite $(L_r)_{r \geqslant 0}$ est croissante. L’hypothèse entraîne qu’il existe un entier $n \geqslant 0$ tel que $L_r = L_n$ pour $r \geqslant n$. Pour chacun des $r \leqslant n$, soit $(m_{r,s})_{1 \leqslant s \leqslant k_r}$ un système de générateurs du $A_0$-module $L_r$. On va prouver que les éléments $a^r m_{r,s}$ pour $1 \leqslant s \leqslant k_r$, $0 \leqslant r \leqslant n$ forment un système de générateurs du $A$-module $N$. Comme $M_r = a^r M_0$ pour tout $r$, on a $N_r = a^r L_r$ pour tout $r$, par définition de $L_r$. Pour $r \leqslant n$, on a donc
$$
N_r = a^r L_r = \sum_{s=1}^{k_r} a^r A_0 m_{rs} \subset \sum_{s=1}^{k_r} A_0 a^r m_{rs},
$$
et pour $r > n$
$$
N_r = a^r L_n = \sum_{s=1}^{k_n} a^r A_0 m_{n,s} \subset \sum_{s=1}^{k_n} A_0 a^r m_{n,s} \subset \sum_{s=1}^{k_n} A_0 a^{r-n} (a^n m_{n,s})
$$
ce qui achève la démonstration (cf. exerc. 10).

#### Corollaire 1 (théorème de Hilbert) {#ac-iii-s2-thm-2-cor-1 .statement}

Pour tout anneau commutatif noethérien $C$, l’anneau de polynômes $C[X]$ est noethérien (cf. exerc. 10).

#### Corollaire 2 {#ac-iii-s2-thm-2-cor-2 .statement}

Pour tout anneau commutatif noethérien $C$ et tout entier $n > 0$, l’anneau de polynômes $C[X_1, \ldots, X_n]$ est noethérien.

Cela résulte du cor. 1 par récurrence sur $n$.

#### Corollaire 3 {#ac-iii-s2-thm-2-cor-3 .statement}

Si C est un anneau commutatif noethérien, toute C-algèbre commutative de type fini est un anneau noethérien.
En effet, une telle algèbre est isomorphe à un quotient d'une algèbre de polynômes $C[X_1, ..., X_n]$ ($§ 1,$ no 1).

#### Corollaire 4 {#ac-iii-s2-thm-2-cor-4 .statement}

Soit A un anneau commutatif gradué de type $\mathbf{N}$, et soit $(A_n)$ sa graduation. Pour que A soit noethérien, il faut et il suffit que $A_0$ soit noethérien et que A soit une $A_0$-algèbre de type fini.
La condition est suffisante en vertu du cor. 3. Inversement, supposons A noethérien ; $m = \sum_{n \geq 1} A_n$, qui est un idéal de A, est donc de type fini ; par suite A est une $A_0$-algèbre de type fini ($§ 1,$ no 2, cor. de la prop. 1) ; d'autre part $A_0$, qui est isomorphe à $A/m$, est un anneau noethérien.

#### Corollaire 5 {#ac-iii-s2-thm-2-cor-5 .statement}

Soient A un anneau commutatif, m un idéal de A tel que $A/m$ soit noethérien, que $m/m^2$ soit un $(A/m)$-module de type fini et que A soit séparé et complet pour la topologie m-adique. Alors gr(A) et A sont noethériens.
En effet, gr(A) est une $(A/m)$-algèbre engendrée par $m/m^2$ (no 3, Exemple 3), donc l'anneau gr(A) est noethérien en vertu du cor. 3. On en déduit que A lui-même est noethérien (no 9, cor. 2 de la prop. 12).

#### Corollaire 6 {#ac-iii-s2-thm-2-cor-6 .statement}

Pour tout anneau commutatif noethérien C et tout entier $n > 0$, l'anneau de séries formelles $C[[X_1, ..., X_n]]$ est noethérien.
Cela résulte du cor. 5 et du no 6, cor. de la prop. 6, car si m est l'idéal de $A = C[[X_1, ..., X_n]]$ formé des séries formelles sans terme constant, $A/m$ est isomorphe à C et $m/m^2$ au C-module $C^n$.

#### Remarque 1 {#ac-iii-s2-n10-rem-1 .statement}

Les corollaires 2, 3 et 6 s'appliquent en particulier lorsque C est un corps commutatif.

#### Remarque 2 {#ac-iii-s2-n10-rem-2 .statement}

Soit g une algèbre de Lie sur un anneau commutatif noethérien C, et supposons que g soit un C-module de type fini. Munissons l'algèbre enveloppante U de g de la filtration croissante $(U_n)$ définie au no 3, Exemple 4. Pour la topologie correspondante, U est discret, donc séparé et complet ; l’anneau gradué associé gr(U) est une C-algèbre de type fini, étant un quotient de l’algèbre symétrique S(g), donc gr(U) est un anneau nœthérien (cor. 3) et on en déduit que U est un anneau nœthérien à gauche et à droite (no 9, cor. 2 de la prop. 12).*

### 11. Anneaux m-adiques complets et limites projectives.

On a vu au no 6 que si A est un anneau commutatif et m un idéal de A tel que A soit séparé et complet pour la topologie m-adique, alors l’anneau topologique A s’identifie canoniquement à la limite projective des anneaux discrets $A_i = A/m^{i+1}$ ($i \in \mathbf{N}$) pour les applications canoniques $h_{ij} : A/m^{j+1} \to A/m^{i+1}$ ($i \leq j$) ; on notera que $h_{ij}$ est surjectif et que, si $n_{ij}$ est son noyau, on a
$$
n_{ij} = m^{i+1}/m^{j+1} = (m/m^{j+1})^{i+1} = (n_{0j})^{i+1};
$$
en particulier $(n_{0j})^{j+1} = 0$. Réciproquement :

#### Proposition 14 {#ac-iii-s2-prop-14 .statement}

Soit $(A_i, h_{ij})$ un système projectif d’anneaux commutatifs discrets, dont l’ensemble d’indices est $\mathbf{N}$, et soit $(M_i, u_{ij})$ un système projectif de modules sur le système projectif d’anneaux $(A_i, h_{ij})$. On désigne par $n_j$ le noyau de $h_{0j} : A_j \to A_0$, et on pose $A = \lim_{\leftarrow} A_i, M = \lim_{\leftarrow} M_i$. On suppose que :
a) pour tout $i \in \mathbf{N}$, $h_{ii}$ est l’application identique de $A_i$, et pour $i \leq j$, $h_{ij}$ et $u_{ij}$ sont surjectifs ;
b) pour $i \leq j$, les noyaux de $h_{ij}$ et $u_{ij}$ sont $n_j^{i+1}$ et $n_j^{i+1}M_j$ respectivement.

Alors :
(i) A est un anneau topologique séparé et complet, M est un A-module topologique séparé et complet, et les applications canoniques $h_i : A \to A_i, u_i : M \to M_i$ sont surjectives.
(ii) Si $M_0$ est un $A_0$-module de type fini, M est un A-module de type fini ; plus précisément, toute partie finie S de M telle que $u_0(S)$ engendre $M_0$ est un système de générateurs de M.

Les assertions de (i) résultent de Top. gén., chap. II, 3e éd., § 3, no 5, cor. de la prop. 10 et cor. 1 du th. 1.

Pour tout $i \in \mathbf{N}$, posons $m_{i+1} = \mathrm{Ker}(h_i), N_{i+1} = \mathrm{Ker}(u_i)$; on a donc $m_{i+1} = \lim_{\leftarrow k \geq 0} h_{t, i+k}(0) = \lim_{\leftarrow k} n_{i+k}^{i+1}$ et $N_{i+1} = \lim_{\leftarrow k} n_{i+k}^{i+1} M_{i+k}$; comme $h_{i+k}$ et $u_{i+k}$ sont surjectifs, on a

(16) $$
h_{i+k}(m_{i+1}) = n_{i+k}^{i+1}, \quad u_{i+k}(N_{i+1}) = n_{i+k}^{i+1} M_{i+k}.
$$

Montrons que l’on a $m_i N_j \subset N_{i+j}$ pour $i \geq 1$ et $j \geq 1$, ce qui revient à prouver que $u_{i+j-1}(m_i N_j) = 0$; or $u_{i+j-1}(m_i N_j) = h_{i+j-1}(m_i) u_{i+j-1}(N_j)$ est égal à $n_{i+j-1}^i(n_{i+j-1}^j M_{i+j-1}) = 0$, car, pour tout $k \geq 0$, $n_k^{k+1}$, qui est le noyau de $h_{kk}$, est égal à 0. On voit de même que $m_i m_j \subset m_{i+j}$. Si on pose, pour $i \leq 0$, $m_i = A$ et $N_i = M$, $(m_i)_{i \in \mathbf{Z}}$ est une filtration de $A$ et $(N_i)_{i \in \mathbf{Z}}$ une filtration de $M$ compatible avec la filtration de $A$; les topologies de $A$ et de $M$ sont évidemment celles définies par ces filtrations. Cela étant, soit $a$ un idéal de $A$ tel que $h_1(a) = n_1$, et désignons par $M'$ le sous-module de $M$ engendré par $S$; on va montrer que

(17) $$
N_i = a^i M' + N_{i+1} \text{ pour } i \geq 0.
$$

Posons $a_i = h_i(a)$, $M'_i = u_i(M')$; il suffit de montrer que $u_i(N_i) = a_i^i M'_i$. C’est vrai si $i = 0$, car $N_0 = M$ et $M'_0 = M_0$ par hypothèse. Si $i \geq 1$, on a $u_i(N_i) = n_i^i M_i$ par (16). Comme $h_{1i}$ est surjectif et que $h_{0i} = h_{01} \circ h_{1i}$, $h_{1i}$ applique le noyau $n_i$ de $h_{0i}$ sur le noyau $n_1$ de $h_{01}$, et $n_i = \overline{h_{1i}}(n_1)$; on a $h_{1i}(a_i) = h_1(a) = n_1 = h_{1i}(n_i)$, et comme le noyau de $h_{1i}$ est $n_i^2$, on a $n_i \subset a_i + n_i^2$ et $a_i \subset n_i$, d’où $n_i = a_i + n_i^2$. Par ailleurs on a $u_{0i}(M'_i) = u_0(M') = M_0 = u_{0i}(M_i)$ et comme $\operatorname{Ker}(u_{0i}) = n_i M_i$, $M_i = M'_i + n_i M_i$; d’où

$$
n_i^i M_i = (a_i + n_i^2)^i (M'_i + n_i M_i).
$$

Or, on a $a_i^k n_i^{i+1-k} \subset n_i^{i+1} = 0$ pour $0 \leq k \leq i$; il en résulte bien que $u_i(N_i) = n_i^i M_i = a_i^i M'_i$, ce qui prouve (17).

Par ailleurs on a $m_1 = \overline{h_1}(n_1)$, d’où $a \subset m_1$ et par suite $a^i \subset m_1^i \subset m_i$, d’où $N_i \subset m_i M' + N_{i+1}$; d’autre part on a évidemment $m_i M \subset N_i$, donc $N_i = m_i M' + N_{i+1}$ pour tout $i \geq 0$; il résulte alors du cor. 3 de la prop. 12 du n° 9 que l’on a $M' = M$, ce qui achève la démonstration.

#### Corollaire 1 {#ac-iii-s2-prop-14-cor-1 .statement}

Les notations et hypothèses étant celles de la prop. 14, supposons de plus que $M_0$ soit un $A_0$-module de type fini et que l'idéal $n_1$ de $A_1$ soit de type fini. Soit $m_1$ le noyau de $h_0$; les topologies de $A$ et de $M$ sont alors les topologies $m_1$-adiques sur cet anneau et ce module respectivement; d'une façon précise, pour tout $i \geqslant 0$, les noyaux de $h_i$ et de $u_i$ sont $m_1^{i+1}$ et $m_1^{i+1}M$ respectivement; de plus $m_1/m_1^2$ est un $A$-module de type fini.

Conservons les notations de la démonstration de la prop. 14 ; les hypothèses permettent ici de supposer que l'idéal $a$ est de type fini. Soit $i \geqslant 0$ un entier quelconque ; pour tout $j \geqslant 0$, on a, d'après (17), $N_{i+j} = a^j(a^iM) + N_{i+j+1} \subset m_j(a^iM) + N_{i+j+1}$; réciproquement, $m_j(a^iM) \subset m_jm_iM \subset m_{i+j}M \subset N_{i+j}$, d'où

$$
N_{i+j} = m_j(a^iM) + N_{i+j+1}.
$$

Comme $a$ et $M$ sont des $A$-modules de type fini, il en est de même de $a^iM$. Appliquant le cor. 3 de la prop. 12 du no 9 au module $N_i$ muni de la filtration $(N_{ij})_{j \in \mathbf{Z}}$ définie par $N_{ij} = N_i$ si $j < 0$, $N_{ij} = N_{i+j}$ si $j \geqslant 0$, il vient $N_i = a^iM$, d'où $N_i \subset m_1^iM$. Mais on a aussi $m_1^iM \subset m_iM \subset N_i$, d'où $N_i = m_1^iM$. Appliquant ceci au cas où $M_i = A_i$, $u_{ij} = h_{ij}$, il vient $m_i = m_1^i$. De plus, on a $m_1 = a + m_1^2$ en vertu de (17), ce qui démontre la dernière assertion du corollaire.

#### Corollaire 2 {#ac-iii-s2-prop-14-cor-2 .statement}

Les hypothèses étant celles du cor. 1, pour que $A$ soit noethérien, il faut et il suffit que $A_0$ le soit.

La condition est nécessaire puisque $A_0$ est isomorphe à un quotient de $A$; elle est suffisante en vertu du no 10, cor. 5 du th. 2.

### 12. Séparé complété d'un module filtré.

Soient $G$ un groupe filtré dont la filtration $(G_n)$ est formée de sous-groupes distingués de $G$; nous avons déjà rappelé (no 6) que le séparé complété $\hat{G}$ du groupe topologique $G$ s'identifie canoniquement à la limite projective $\lim_{\leftarrow} G/G_n$ des groupes discrets $G/G_n$, l'homomorphisme canonique $i : G \to \hat{G}$ ayant pour image le groupe séparé associé à $G$ (partout dense dans $\hat{G}$) et pour noyau l'adhérence $\bigcap G_n$ de $\{0\}$ dans $G$. Le séparé complété $\hat{G}_n$ du sous-groupe $G_n$ de $G$ s'identifie à l'adhérence de $i(G_n)$ dans $\hat{G}$ ($Top.$)

gén., chap. II, 3e éd., § 3, n° 9, cor. 1 de la prop. 18), et puisque $G_n$ est fermé dans $G$, on a

$$
G_n = i(\hat{G}_n) = i(\hat{G}_n \cap i(G)).
$$

En outre, les $\hat{G}_n$ forment un système fondamental de voisinages de 0 dans $\hat{G}$ (Top. gén., chap. III, 3e éd., § 3, n° 4, prop. 7) et sont donc des sous-groupes ouverts distingués de $\hat{G}$ (Top. gén., chap. III, 3e éd., § 2, n° 3, prop. 8); la topologie de $\hat{G}$ est définie par la filtration $(\hat{G}_n)$, qui est toujours séparée par définition. Comme $i(G)$ est dense dans $\hat{G}$ et que $\hat{G}_n$ est ouvert, on a

$$
\hat{G} = i(G) \cdot \hat{G}_n
$$

et de même

$$
\hat{G}_{n-1} = i(G_{n-1}) \cdot \hat{G}_n.
$$

On déduit de (18) et (19) que la filtration $(\hat{G}_n)$ est exhaustive si et seulement si $(G_n)$ l’est.

Le second théorème d’isomorphie (Alg., chap. I, § 6, n° 13, th. 6 d)) et les formules (18), (19), (20) montrent que les homomorphismes canoniques

$$
G_{n-1}/G_n \to \hat{G}_{n-1}/\hat{G}_n, \quad G/G_n \to \hat{G}/\hat{G}_n,
$$

sont *bijectifs*, donc il en est de même de l’homomorphisme canonique

$$
\operatorname{gr}(G) \to \operatorname{gr}(\hat{G}).
$$

Soient maintenant $A$ un anneau filtré, $E$ un $A$-module filtré, $(A_n)$ et $(E_n)$ les filtrations respectives de $A$ et de $E$; nous supposons ces filtrations *exhaustives*, de sorte que pour les topologies correspondantes, $A$ est un anneau topologique et $E$ un $A$-module topologique (n° 5, prop. 3). On a alors défini (Top. gén., chap. III, 3e éd., § 6, nos 5 et 6) $\hat{A}$ comme anneau topologique et $\hat{E}$ comme $\hat{A}$-module topologique. Si $i : A \to \hat{A}$ est l’homomorphisme canonique, on a $i(A_m)i(A_n) \subset i(A_{m+n})$, d’où, en vertu de la continuité du produit dans $\hat{A}$,

$$
\hat{A}_m \hat{A}_n \subset \hat{A}_{m+n}
$$

puisque $\hat{A}_n$ est l’adhérence de $i(A_n)$ dans $\hat{A}$. On montre de même que
$$
\hat{A}_m \hat{E}_n \subset \hat{E}_{m+n};
$$
autrement dit :

#### Proposition 15 {#ac-iii-s2-prop-15 .statement}

*Soient A un anneau filtré, E un A-module filtré, les filtrations respectives $(A_n), (E_n)$ de A et de E étant exhaustives. Alors $(\hat{A}_n)$ est une filtration compatible avec la structure d’anneau de $\hat{A}$ et $(\hat{E}_n)$ une filtration compatible avec la structure de module de $\hat{E}$ sur l’anneau filtré $\hat{A}$; en outre ces filtrations sont exhaustives et définissent respectivement les topologies de $\hat{A}$ et de $\hat{E}$. Enfin, les applications canoniques $\operatorname{gr}(A) \to \operatorname{gr}(\hat{A})$ et $\operatorname{gr}(E) \to \operatorname{gr}(\hat{E})$ de $\mathbf{Z}$-modules gradués sont respectivement un isomorphisme d’anneaux gradués et un isomorphisme de $\operatorname{gr}(A)$-modules gradués.*

Dans ce qui suit, pour tout espace uniforme X, nous noterons $j_x$ l’application canonique de X dans son séparé complété $\hat{X}$, par $X_0 = j_x(X)$ le sous-espace uniforme de $\hat{X}$, qui est l’espace séparé associé à X. Rappelons que la topologie de X est l’image réciproque par $j_x$ de celle de $X_0$ (*Top. gén.*, chap. II, 3e éd., § 3, no 7, prop. 12). Rappelons aussi que pour toute application uniformément continue $f : X \to Y$, $\hat{f}$ désigne l’application uniformément continue de $\hat{X}$ dans $\hat{Y}$ telle que $\hat{f} \circ j_x = j_Y \circ f$ (*loc. cit.*, prop. 15); si X est un sous-espace uniforme de Y et $f$ l’injection canonique, $\hat{X}$ s’identifie à un sous-espace uniforme de $\hat{Y}$, et $\hat{f}$ à l’injection canonique de $\hat{X}$ dans $\hat{Y}$ (*loc. cit.*, no 9, cor. 1 de la prop. 18).

#### Lemme 2 {#ac-iii-s2-lem-2 .statement}

*Soit $X \xrightarrow{f} Y \xrightarrow{g} Z$ une suite exacte de morphismes stricts de groupes topologiques (*Alg.*, chap. II, 3e éd., § 1, no 4, Remarque). Supposons que X, Y, Z admettent des groupes séparés complétés, et que les éléments neutres de X, Y, Z admettent des systèmes fondamentaux dénombrables de voisinages. Alors $\hat{X} \xrightarrow{\hat{f}} \hat{Y} \xrightarrow{\hat{g}} \hat{Z}$ est une suite exacte de morphismes stricts.*
Soient $N_f, N_g$ les noyaux respectifs de $f$ et $g$; écrivons
$$
f = f_3 \circ f_2 \circ f_1
$$

où $f_1$ est l’application canonique $X \to X/N_f$, $f_2$ un isomorphisme de $X/N_f$ sur $N_g$ et $f_3$ l’injection canonique $N_g \to Y$. On sait déjà que $\hat{f}_2$ est un isomorphisme de $(X/N_f)^{\sim}$ sur $\hat{N}_g$, et on vient de rappeler que $\hat{f}_3$ est un morphisme strict injectif de $\hat{N}_g$ dans $\hat{Y}$; si on montre que $\hat{f}_1$ est un morphisme strict surjectif, il en résultera que $\hat{f}$ est un morphisme strict (*Top. gén.*, chap. III, 3e éd., § 2, n° 8, *Remarque 2*). Soit $g_1$ l’application canonique $Y \to Y/N_g$; si on montre que $\hat{g}_1$ est un morphisme strict surjectif de noyau $\hat{N}_g$, on verra comme ci-dessus que $\hat{g}$ est un morphisme strict et la suite $\hat{X} \xrightarrow{\hat{f}} \hat{Y} \xrightarrow{\hat{g}} \hat{Z}$ sera exacte. On est donc ramené à prouver que si $Y = X/N$ (où $N$ est un sous-groupe distingué de $X$) et $f : X \to Y$ l’application canonique, $\hat{f}$ est *un morphisme strict surjectif de noyau* $\hat{N}$.

Soit $f_0 : X_0 \to Y_0$ l’application qui coïncide avec $\hat{f}$ dans $X_0$; comme $j_X$ (resp. $j_Y$) est un morphisme strict surjectif de $X$ sur $X_0$ (resp. de $Y$ sur $Y_0$), $f_0$ est un morphisme strict surjectif (*Top. gén.*, chap. III, 3e éd., § 2, n° 8, *Remarque 3*). Or $X_0$ et $Y_0$ sont métrisables (*Top. gén.*, chap. IX, 2e éd., § 3, n° 1, prop. 1); il résulte alors de *Top. gén.*, chap. IX, 2e éd., § 3, n° 1, cor. 1 de la prop. 4 et lemme 1, que $\hat{f}_0 = \hat{f}$ est un morphisme strict surjectif et admet comme noyau l’adhérence $\hat{N}_0'$ *dans* $\hat{X}$ du noyau $N_0'$ de $f_0$. Il nous suffira donc de montrer que $\hat{N}_0' = \hat{N}$. Or $N_0'$ contient évidemment $N_0 = j_X(N)$; il suffira de prouver que $N_0'$ est contenu dans l’adhérence $\overline{N}_0$ de $N_0$ *dans* $X_0$. Or,

$$
U = j_X^{-1}(X_0 - \overline{N}_0) = X - j_X^{-1}(\overline{N}_0)
$$

est un ensemble ouvert dans $X$ qui ne rencontre pas $N$; comme $f$ est un morphisme strict surjectif, $V = f(U)$ est un ensemble ouvert dans $Y$ ne contenant pas l’élément neutre $e'$ de $Y$, donc ne rencontrant pas l’adhérence de $e'$; par suite $j_Y(V)$ ne contient pas l’élément neutre de $Y_0$. Mais $j_Y(V) = f_0(X_0 - \overline{N}_0)$, donc $N_0' \subset \overline{N}_0$, ce qui achève de prouver le lemme 2.

#### Proposition 16 {#ac-iii-s2-prop-16 .statement}

*Soient A un anneau filtré, ($A_n$) sa filtration, E un A-module, ($E_n$) la filtration sur E déduite de celle de A, formée des $E_n = A_n E$. On suppose la filtration ($A_n$) exhaustive et le* module E de type fini. Alors, si i : E → Ē est l’application canonique, on a, pour tout n ∈ Z,

$$
\hat{E}_n = \hat{A}_n \hat{E} = \hat{A}_n i(E) \quad \text{et} \quad \hat{E} = \hat{A}. i(E).
$$

En particulier $\hat{E}$ est un $\hat{A}$-module de type fini.

L’égalité $A_n E = E_n$ entraîne, en vertu de la continuité de la loi externe du $\hat{A}$-module $\hat{E}$, $\hat{A}_n \hat{E} \subset \hat{E}_n$, et on a évidemment $\hat{A}_n \hat{E} \supset \hat{A}_n i(E)$. Par hypothèse il existe un homomorphisme surjectif $u : L \to E$, où $L = A_s^I$, I étant un ensemble fini ; munissons L de la filtration produit, formée des $L_n = A_n^I$, qui définit sur L la topologie produit ; on a donc $\hat{L} = \hat{A}_s^I$ et $\hat{L}_n = \hat{A}_n^I$ (Top. gén., chap. II, 3e éd., § 3, no 9, cor. 2 de la prop. 18). Soient $j : L \to \hat{L}$ l’application canonique, $(e_i)_{i \in I}$ la base canonique de L ; pour qu’un élément $\sum_{i \in I} a_i j(e_i)$ (avec $a_i \in \hat{A}$ pour tout $i \in I$) appartenne à $\hat{L}_n$, il faut et il suffit que $a_i \in \hat{A}_n$ pour tout $i$; on a donc $\hat{L}_n = \hat{A}_n . j(L)$. Cela étant, on a par définition $u(L_n) = A_n E = E_n$, donc $u$ est un morphisme strict de L sur E (Top. gén., chap. III, 3e éd., § 2, no 8, prop. 24). Le lemme 2 montre alors que $\hat{u} : \hat{L} \to \hat{E}$ est un morphisme strict surjectif. Comme $\hat{L}_n$ est un sous-groupe ouvert de $\hat{L}$, $\hat{u}(\hat{L}_n)$ est un sous-groupe ouvert (donc fermé) de $\hat{E}$; mais $\hat{u}(\hat{L}_n) = \hat{A}_n \hat{u}(j(L)) = \hat{A}_n i(E)$, et comme $i(E_n) \subset A_n i(E) \subset \hat{A}_n i(E)$, on voit finalement que $\hat{E}_n \subset \hat{A}_n i(E) \subset \hat{A}_n \hat{E} \subset \hat{E}_n$, et par suite $\hat{E}_n = \hat{A}_n \hat{E} = \hat{A}_n i(E)$; faisant $n = 0$, on obtient la deuxième formule (25).

#### Corollaire 1 {#ac-iii-s2-prop-16-cor-1 .statement}

Sous les conditions de la prop. 16, si A est complet, il en est de même de E.

En effet, comme l’application canonique $A \to \hat{A}$ est alors surjective (no 6, prop. 5), on a $\hat{E} = i(E)$ d’après (25), et on conclut par la prop. 5 du no 6.

#### Corollaire 2 {#ac-iii-s2-prop-16-cor-2 .statement}

Soient A un anneau commutatif, m un idéal de A de type fini, $\hat{A}$ le séparé complété de A pour la topologie m-adique. On a alors $\widehat{m^n} = (\hat{m})^n = m^n . \hat{A}$ pour tout entier $n > 0$, et la topologie de $\hat{A}$ est la topologie $\hat{m}$-adique.

Posons $A_n = m^n$, qui est un idéal de type fini de $A$. La formule $m^p A_n = m^{n+p}$ montre que la topologie induite sur $A_n$ par la topologie $m$-adique coïncide avec la topologie $m$-adique du $A$-module $A_n$ (n° 1, Exemple 3). En vertu de la prop. 16 appliquée à $E = A_n$, on a $\widehat{A}_n = \widehat{A}.A_n$, autrement dit $\widehat{m^n} = m^n.\widehat{A}$. En particulier $\widehat{m} = m.\widehat{A}$, d'où
$$
(\widehat{m})^n = m^n.\widehat{A} = \widehat{A}.A_n
$$
(cf. exerc. 12).

Exemples de séparés complétés d’anneaux filtrés. — 1) Soit $A$ un anneau gradué de type $\mathbf{N}$, et soit $(A_n)_{n \geq 0}$ sa graduation ; munissons-le de la filtration associée qui est séparée et exhaustive (n° 1, Exemple 1). Le groupe additif $A$ s’identifie canoniquement à un sous-groupe de $B = \prod_{n \in \mathbf{N}} A_n$; si on munit $B$ de la topologie produit des topologies discrètes, la topologie induite sur $A$ est la topologie définie par la filtration de $A$; en outre $B$ est un groupe topologique complet, et $A$ est dense dans $B$ (Top. gén., chap. III, 3e éd., § 2, n° 9, prop. 25). Le groupe additif topologique $B$ s’identifie donc au complété $\widehat{A}$ du groupe additif séparé $A$, et il résulte de la prop. 15 qu’il est muni d’une structure d’anneau unique qui en fait le complété de l’anneau topologique $A$. Pour définir la multiplication dans cet anneau, on remarque que si l’on pose $A'_n = \sum_{i > n} A_i$, l’adhérence dans $B$ de l’idéal bilatère $A'_n$ est l’ensemble $B_n$ des $x = (x_i) \in B$ tels que $x_i = 0$ pour $i \leq n$. Soient alors $x = (x_i), y = (y_i)$ deux éléments de $B$, $z = (z_i)$ leur produit. On a, pour tout $n > 0$, $x \equiv x'_n$ (mod. $B_n$), $y \equiv y'_n$ (mod. $B_n$), où $x'_n = (x_i)_{0 \leq i \leq n}$, $y'_n = (y_i)_{0 \leq i < n}$, d’où $z \equiv x'_n y'_n$ (mod. $B_n$). Mais $x'_n$ et $y'_n$ appartiennent à $A$, et on voit donc que l’on a pour tout $n \in \mathbf{N}$
$$
z_n = \sum_{j=0}^n x_j y_{n-j}.
$$
En particulier, on retrouve le cor. de la prop. 6 du n° 6 : si $C$ est un anneau commutatif, le complété de l’anneau de polynômes $C[X_1, ..., X_r]$, muni de la filtration associée à sa graduation usuelle (par le degré total) s’identifie canoniquement à l’anneau de séries formelles $C[[X_1, ..., X_r]]$ (cf. Alg., chap. IV, § 5, n° 10).

*2) Soit K un corps valué complet commutatif. Le complété de l’anneau des séries convergentes à r variables sur K s’identifie canoniquement à l’anneau de séries formelles K[[X₁,..., Xₙ]].*

3) Soit α un élément non nul et non inversible d’un anneau principal A ; la topologie (α)-adique sur A est encore appelée topologie α-adique ; elle est séparée, car l’intersection des idéaux (αⁿ) est réduite à 0 (Alg., chap. VII, § 1, no 3). On notera que le complété de A pour cette topologie n’est pas nécessairement un anneau intègre (cf. no 13, Remarque 3). L’anneau gradué associé gr(A) = gr(Ā) est canoniquement isomorphe à (A/(α))[X] (no 3, Exemple 1). Lorsque A = Z, le complété de Z pour la topologie n-adique (n > 1) se note Zₙ et ses éléments s’appellent les entiers n-adiques.

Tout élément de $\mathbf{Z}/n^k\mathbf{Z}$ admet un représentant et un seul de la forme $\sum_{i=0}^{k-1} a_i n^i$ avec $0 \leqslant a_i \leqslant n-1$ pour tout $i$; en outre, son image canonique dans $\mathbf{Z}/n^{k-1}\mathbf{Z}$ est la classe de $\sum_{i=0}^{k-2} a_i n^i$. Ces remarques, et le fait que $\mathbf{Z}_n$ s’identifie canoniquement à la limite projective $\lim_{\leftarrow k} \mathbf{Z}/n^k \mathbf{Z}$, montrent aussitôt que tout élément de $\mathbf{Z}_n$ peut s’écrire d’une seule manière sous la forme $\sum_{i=0}^{\infty} a_i n^i$ avec $0 \leqslant a_i < n$ et que réciproquement une telle série est convergente dans $\mathbf{Z}_n$.

### 13. Séparé complété d’un anneau semi-local.

#### Proposition 17 {#ac-iii-s2-prop-17 .statement}

Soient A un anneau commutatif, (mλ)λ∈L une famille d’idéaux de A, distincts de A, tels que mλ et mμ soient étrangers pour λ ≠ μ. Pour tout famille s = (s(λ))λ∈L d’entiers ≥ 0, à support fini, on pose $a_s = \bigcap_{λ∈L} m_s^{s(λ)}$ (égal au produit des m_s^{s(λ)} pour les λ tels que s(λ) ≠ 0 ; cf. chap. II, § 1, no 2, prop. 3 et 5) ; les a_s forment un système fondamental de voisinages de 0 pour une topologie C compatible avec la structure d’anneau de A ; soit Ā le séparé complété de A pour cette topologie. D’autre part, pour tout λ ∈ L, soit Aλ l’anneau A muni de la topologie mλ-adique, et soit Āλ son séparé complété. Si l’on désigne par $u : A \to \prod_{\lambda \in L} A_\lambda$ l’homomorphisme diagonal, $u$ est continu et l’homomorphisme correspondant $\hat{u}$:

$$
\hat{A} \to (\prod_{\lambda \in L} A_\lambda)^{\sim} = \prod_{\lambda \in L} \hat{A}_\lambda
$$

(Top. gén., chap. III, 3e éd., § 6, n° 5 et chap. II, 3e éd., § 3, n° 9, cor. 2 de la prop. 18) est un isomorphisme d’anneaux topologiques.

La première assertion résulte de Top. gén., chap. III, 3e éd., § 6, n° 3, Exemple 3. Posons $B = \prod_{\lambda \in L} A_\lambda$; comme la topologie de $A$ est plus fine que chacune des topologies $m_\lambda$-adiques, les applications $\mathrm{pr}_\lambda \circ u$ sont continues, donc $u$ est continu. De plus, $u(a_s)$ est l’intersection de la diagonale $\Delta$ de $B$ et de l’ensemble ouvert $\bigcap_{\lambda \in L} \mathrm{pr}_\lambda^{-1}(m^{s(\lambda)}_\lambda)$ de $B$; il en résulte que $u$ est un morphisme strict du groupe additif $A$ dans $B$, d’image $\Delta$. Or $\Delta$ est dense dans $B$. En effet, soit $b = (a_\lambda)_{\lambda \in L}$ un élément de $B$; tout voisinage de $b$ dans $B$ contient un ensemble de la forme $b + V$, où $V = \bigcap_{\lambda \in L} \mathrm{pr}_\lambda^{-1}(m^{s(\lambda)}_\lambda)$, pour une famille $s = (s(\lambda))_{\lambda \in L}$ à support fini d’entiers $\geqslant 0$. Comme les $m^{s(\lambda)}_\lambda$ sont deux à deux étrangers (chap. II, § 1, n° 2, prop. 3), il existe un $x \in A$ tel que $x \equiv a_\lambda$ (mod. $m^{s(\lambda)}_\lambda$) pour tout $\lambda$ (loc. cit., prop. 5), donc $(b + V) \cap \Delta \neq \varnothing$. Le complété séparé du groupe $B/\Delta$ est donc $\{0\}$; appliquant le lemme 2 du n° 12 aux suites exactes $0 \to A \xrightarrow{u} B, A \xrightarrow{u} B \to B/\Delta$, on voit que $\hat{u}$ est un isomorphisme de $\hat{A}$ sur $\hat{B}$.

#### Corollaire {#ac-iii-s2-n13-cor-1 .statement}

Soient $A$ un anneau principal, $P$ un système représentatif d’éléments extrémaux de $A$ (Alg., chap. VII, § 1, n° 3). La topologie sur $A$ pour laquelle les idéaux $\neq 0$ de $A$ forment un système fondamental de voisinages de $0$, qui est compatible avec la structure d’anneau de $A$, est séparée, et le complété de $A$ muni de cette topologie est canoniquement isomorphe au produit des complétés de $A$ pour les topologies $\pi$-adiques, où $\pi$ parcourt $P$.

Les idéaux principaux $(\pi)$ pour $\pi \in P$ sont en effet maximaux et deux à deux distincts, donc étrangers ; on a déjà vu (n° 12,

Exemple 3) que les topologies $\pi$-adiques sont séparées, donc il en est de même de la topologie définie dans l’énoncé de la prop. 17, qui est plus fine que chacune des topologies $\pi$-adiques.

Lorsqu’on applique le cor. de la prop. 17 à $A = \mathbf{Z}$, on désigne par $\hat{\mathbf{Z}}$ le complété de $\mathbf{Z}$ pour la topologie pour laquelle tous les idéaux $\neq 0$ de $\mathbf{Z}$ forment un système fondamental de voisinages de 0, anneau isomorphe au produit $\prod_{p \in P} \mathbf{Z}_p$ des anneaux d’entiers $p$-adiques ($P$ étant l’ensemble des nombres premiers).

#### Remarque 1 {#ac-iii-s2-n13-rem-1 .statement}

Il est clair que sous les conditions de la prop. 17, la topologie $\mathcal{G}$ est la borne supérieure des topologies $m_\lambda$-adiques sur $A$.

#### Remarque 2 {#ac-iii-s2-n13-rem-2 .statement}

Tout idéal fermé $a$ de $\prod_{\lambda \in L} \hat{A}_\lambda$ est identique au produit de ses projections $a_\lambda = \mathrm{pr}_\lambda(a)$, qui sont des idéaux fermés dans les $\hat{A}_\lambda$; en effet, $\hat{A}_\lambda$ s’identifie canoniquement à un idéal fermé $A'_\lambda$ de $\prod_{\lambda} \hat{A}_\lambda$ et $a_\lambda$ à $a \cap A'_\lambda$ (*Alg.*, chap. I, § 8, no 10, prop. 6), la somme des $a_\lambda$ est *dense* dans le produit $\prod_{\lambda} a_\lambda$ (*Top. gén.*, chap. III, 3e éd., § 2, no 9, prop. 25) et ce dernier est fermé dans $\prod_{\lambda} \hat{A}_\lambda$, d’où notre assertion.

#### Proposition 18 {#ac-iii-s2-prop-18 .statement}

Soient $A$ un anneau commutatif, $(m_i)_{1 \leq i \leq q}$ une famille finie d’idéaux maximaux distincts de $A$, $x$ l’idéal produit $m_1 m_2 \ldots m_q = m_1 \cap m_2 \cap \ldots \cap m_q$, $S$ la partie multiplicative $\bigcap_{i=1}^q (A - m_i)$. On munit $A$ de la topologie $x$-adique, l’anneau $B = S^{-1}A$ de la topologie $xB$-adique, chacun des anneaux locaux $A_{m_i}$ de la topologie $(m_i A_{m_i})$-adique. Soient $u : A \to B$, $v_i : B \to A_{m_i}$ les homomorphismes canoniques (chap. II, § 2, no 1, cor. 2 de la prop. 2), $v$ l’homomorphisme $(v_i) : B \to \prod_{i=1}^q A_{m_i}$. Les homomorphismes $u$ et $v$ sont continus, et les homomorphismes correspondants $\hat{u} : \hat{A} \to \hat{B}$ et $\hat{v} : \hat{B} \to \prod_{i=1}^q (A_{m_i})^\sim$ sont des isomorphismes d’anneaux topologiques.

On a $m_i \cap S = \varnothing$ pour $1 \leq i \leq q$, donc l’idéal $m'_i = m_i B$ de $B$ est maximal (chap. II, § 2, n° 5, prop. 11) et on a
$$
rB = m'_1 \cap m'_2 \cap \ldots \cap m'_q
$$
(chap. II, § 2, n° 4); enfin, on a $B_{m'_i} = A_{m_i}$ à un isomorphisme canonique près (chap. II, § 2, n° 5, prop. 11). Comme $\bar{u}^1(rB) = r$ et $\bar{\nu}_i(m_i A_{m_i}) \supset rB$, $u$ et $\nu$ sont continus. Il suffit donc de prouver que si $\omega = \nu \circ u : A \to \prod_{i=1}^q A_{m_i}$, $\hat{\omega}$ est un isomorphisme de $\hat{A}$ sur $\prod_{i=1}^q \hat{A}_{m_i}$, car ce résultat appliqué à $B$ et aux $m'_i$ montrera que $\hat{\nu}$ est un isomorphisme, et par suite aussi $\hat{u}$. Notons que tout produit de puissances des $m_i$ contient une puissance de $r$, donc la topologie $r$-adique est la borne supérieure des topologies $m_i$-adiques; en outre, si $A_t$ désigne l’anneau $A$ muni de la topologie $m_t$-adique, et $\varphi : A \to \prod_{i=1}^q A_i$ l’application diagonale, $\hat{\varphi} : \hat{A} \to \prod_{i=1}^q \hat{A}_i$ est un isomorphisme (prop. 17). Tout revient donc à prouver que si $u_t : A_t \to A_{m_i}$ est l’application canonique, $\hat{u}_t : \hat{A}_t \to \hat{A}_{m_i}$ est un isomorphisme. Or, pour tout $n$, l’application
$$
u_{i,n} : A/m_i^n \to A_{m_i}/m_i^n A_{m_i}
$$
déduite de $u_t$ par passage aux quotients est un isomorphisme (chap. II, § 3, n° 3, prop. 9); notre assertion résulte de ce que $\hat{A}_t$ (resp. $\hat{A}_{m_i}$) est la limite projective des anneaux discrets $A/m_i^n$ (resp. $A_{m_i}/m_i^n A_{m_i}$) (cf. n° 6).

Remarque 3). — On voit donc qu’un anneau intègre $A$ peut être tel que son séparé complété $\hat{A}$ admette des diviseurs de zéro non nuls.

#### Proposition 19 {#ac-iii-s2-prop-19 .statement}

Soient $A$ un anneau commutatif, $m$ un idéal maximal de $A$. Le séparé complété $\hat{A}$ de $A$ pour la topologie $m$-adique est un anneau local, dont l’idéal maximal est $\hat{m}$.

Si $a = \bigcap_{k \geq 1} m^k$, $\hat{A}$ est le complété de l’anneau séparé $A/a$ associé à $A$, et comme $m/a$ est maximal dans $A/a$, on peut supposer que $A$ est séparé pour la topologie $m$-adique. Comme $A/m$ et $\hat{A}/\hat{m}$ sont des anneaux isomorphes (no 12, formule (21)), $\hat{m}$ est maximal dans $\hat{A}$. Comme la topologie de $\hat{A}$ est définie par la filtration $(\hat{m}^n)^{\sim}$ (no 12), la proposition sera conséquence du lemme suivant :

#### Lemme 3 {#ac-iii-s2-lem-3 .statement}

*Soit $A$ un anneau topologique séparé et complet, dans lequel il existe un système fondamental $\mathcal{S}$ de voisinages de $0$ formé de sous-groupes additifs de $A$.

(i) *Pour tout $x \in A$ tel que $\lim_{n \to \infty} x^n = 0$, $1 - x$ est inversible dans $A$ et son inverse est égal à $\sum_{n=0}^{\infty} x^n$.

(ii) *Soit $a$ un idéal bilatère de $A$ tel que $\lim_{n \to \infty} x^n = 0$ pour tout $x \in a$. Pour qu’un élément $y$ de $A$ soit inversible, il faut et il suffit que sa classe mod. $a$ soit inversible dans $A/a$; en particulier $a$ est contenu dans le radical de $A$.

(i) Comme
$$
(1 - x)(1 + x + \cdots + x^n) = (1 + x + \cdots + x^n)(1 - x) = 1 - x^{n+1},
$$
tout revient à prouver que la série de terme général $x^n$ est convergente dans $A$; or, par hypothèse, pour tout voisinage $V \in \mathcal{S}$ de $0$ dans $A$, il existe un entier $p > 0$, tel que $x^n \in V$ pour $n \geq p$. On en conclut que $x^p + x^{p+1} + \cdots + x^q \in V$ pour tout $q \geq p$, et notre assertion résulte donc du critère de Cauchy (*Top. gén.*, chap. III, 3e éd., § 5, no 2, th. 1).

(ii) Supposons qu’il existe $y' \in A$ tel que $yy' \equiv 1$ (mod. $a$) et $y'y \equiv 1$ (mod. $a$). L’hypothèse sur $a$ entraîne, en vertu de (i), que $yy'$ et $y'y$ sont inversibles dans $A$, donc $y$ est inversible dans $A$. En particulier, tout $x \in a$ est tel que $1 - x$ soit inversible dans $A$, et comme $a$ est un idéal bilatère de $A$, il est contenu dans le radical de $A$ (*Alg.*, chap. VIII, § 6, no 3, th. 1).

Ce lemme étant établi, il suffit de l’appliquer à l’anneau topologique $\hat{A}$ et à l’idéal $\hat{m}$, car pour tout $x \in \hat{m}$, on a $x^n \in (\hat{m})^n \subset (\hat{m}^n)^{\sim}$ et la suite $(x^n)$ tend donc vers $0$.

Si on prend $A = \mathbf{Z}$, tout idéal maximal de $\mathbf{Z}$ est de la forme $p\mathbf{Z}$, où $p$ est premier. L’anneau des nombres $p$-adiques $\mathbf{Z}_p$ est donc un anneau local, dont $p\mathbf{Z}_p$ est l’idéal maximal (cor. 2 de la prop. 16), et dont le corps résiduel est isomorphe à $\mathbf{Z}/p\mathbf{Z} = \mathbf{F}_p$ et $\mathbf{Z}_{(p)}$, muni de la topologie $p\mathbf{Z}_{(p)}$-adique, s’identifie à un sous-anneau topologique de $\mathbf{Z}_p$, contenant $\mathbf{Z}$.

#### Corollaire {#ac-iii-s2-n13-cor-2 .statement}

Soient $A$ un anneau semi-local (chap. II, § 3, no 5), $m_i$ ses idéaux maximaux distincts ($1 \leq i \leq q$),
$$
r = m_1 \cap m_2 \cap \ldots \cap m_q
$$
son radical. Le séparé complété $\hat{A}$ de $A$ pour la topologie $r$-adique est un anneau semi-local, canoniquement isomorphe au produit
$$
\prod_{i=1}^q \hat{A}_{m_i},
$$
où $\hat{A}_{m_i}$ est l’anneau local séparé complété de l’anneau local $A_{m_i}$ pour la topologie $(m_i A_{m_i})$-adique.

## EXERCICES {#ac-iii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
