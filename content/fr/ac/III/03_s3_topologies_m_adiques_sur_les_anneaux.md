---
book: ac
book_title: Commutative Algebra
chapter: III
chapter_title: Graduations, filtrations et topologies
section: 3
section_title: Topologies m-adiques sur les anneaux nœthériens
lang: fr
source: ac-i-iv-fr
pdf_pages: 0233-0250, 0290-0299
extraction: ocr
subsections:
    - "no": 1
      title: Bonnes filtrations.
      page: 0
      pdf_page: 233
    - "no": 2
      title: Topologies $m$-adiques sur les anneaux noethériens.
      page: 0
      pdf_page: 238
    - "no": 3
      title: Anneaux de Zariski.
      page: 0
      pdf_page: 240
    - "no": 4
      title: Séparé complété d'un anneau noethérien.
      page: 0
      pdf_page: 242
    - "no": 5
      title: Complété d’un anneau de Zariski.
      page: 0
      pdf_page: 246
statements: 37
exercises: 9
content_sha256: a930a57cc68133a0752ad2e45fbd56a9286b0b1dd65838fcb468772bac7cd2fb
---

## § 3. Topologies $m$-adiques sur les anneaux nœthériens.

Toutes les filtrations considérées dans ce paragraphe sont supposées exhaustives.

### 1. Bonnes filtrations.

Soient $A$ un anneau commutatif filtré, $E$ un $A$-module filtré, $(A_n)$ et $(E_n)$ les filtrations respectives de $A$ et de $E$; supposons que $A_0 = A$. Dans l’anneau de polynômes $A[X]$, l’ensemble
$$
A' = \sum_{n \geq 0} A_n X^n
$$
est une sous-$A$-algèbre graduée de type $\mathbf{N}$; le sous-groupe
$$
E' = \sum_{n \geq 0} E_n \otimes_A A X^n
$$
de $E \otimes_A A[X]$ est un $A'$-module gradué de type $\mathbf{N}$, puisque
$$
A_m X^m (E_n \otimes_A A X^n) \subset (A_m E_n \otimes_A A X^{m+n}) \subset E_{m+n} \otimes_A A X^{m+n}.
$$

#### Définition 1 {#ac-iii-s3-def-1 .statement}

Soient $A$ un anneau commutatif, $m$ un idéal de $A$, $E$ un $A$-module, $(E_n)$ une filtration sur le groupe additif $E$, formée de sous-modules de $E$. On dit que la filtration $(E_n)$ est $m$-bonne si :
1° $m E_n \subset E_{n+1}$ pour tout $n \in \mathbf{Z}$;
2° il existe un entier $n_0$ tel que $m E_n = E_{n+1}$ pour $n \geq n_0$.

On a alors, par récurrence sur $q$, $m^q E_n = E_{n+q}$ pour $n \geq n_0$, $q \geq 1$. On notera que la condition $1^\circ$ signifie que la filtration $(E_n)$ est compatible avec la structure de $A$-module de $E$, quand on munit $A$ de la filtration $m$-adique. Il est clair que sur tout $A$-module $E$, la filtration $m$-adique est $m$-bonne. Si une filtration sur un $A$-module $E$ est $m$-bonne, la filtration quotient sur tout module quotient de $E$ est $m$-bonne.

#### Théorème 1 {#ac-iii-s3-thm-1 .statement}

*Soient $A$ un anneau commutatif, $m$ un idéal de $A$, $E$ un $A$-module, $(E_n)$ une filtration du groupe additif $E$, formée de sous-$A$-modules de type fini. On suppose que $m E_n \subset E_{n+1}$ pour tout $n$. Soit $A'$ la sous-algèbre graduée $\sum_{n \geq 0} m^n X^n$ de $A[X]$, $E'$ le $A'$-module gradué $\sum_{n \geq 0} E_n \otimes_A A X^n$. Les deux conditions suivantes sont équivalentes :

a) *La filtration* $(E_n)$ *est* $m$*-bonne*.

b) $E'$ *est un* $A'$*-module de type fini*.

Supposons que $m E_{n-1} = E_n$ pour $n > n_0 \geq 0$. Pour $i \leq n_0$, soit $(e_{ij})_{1 \leq j \leq r_i}$ un système fini de générateurs du $A$-module $E_i$. Comme le $A$-module $E_n \otimes_A A X^n$ est engendré par les éléments $e_{nj} \otimes X^n$ pour $0 \leq n \leq n_0$, et est égal à $m^{n-n_0} E_{n_0} \otimes_A A X^n$ pour $n > n_0$, le $A'$-module $E'$ est engendré par les éléments $e_{nj} \otimes X^n$ pour $0 \leq n \leq n_0$ et $1 \leq j \leq r_n$; il est donc bien de type fini.

Réciproquement, si $E'$ est un $A'$-module de type fini, il est engendré par une famille finie d’éléments de la forme $e_k \otimes X^{n(k)}$, où $e_k \in E_{n(k)}$. Soit $n_0$ le plus grand des entiers $n(k)$. Pour $n \geq n_0$ et $f \in E_n$, on a donc $f \otimes X^n = \sum_k t_k (e_k \otimes X^{n(k)})$ avec $t_k \in A'$; remplaçant au besoin $t_k$ par son composant homogène de degré $n - n(k)$, on peut supposer que $t_k = a_k X^{n-n(k)}$ avec $a_k \in m^{n-n(k)}$. Comme l’unique élément $X^n$ forme une base du $A$-module $A X^n$, l’égalité $f \otimes X^n = (\sum_k a_k e_k) \otimes X^n$ entraîne $f = \sum_k a_k e_k$. On a donc $E_n \subset m^{n-n_0} E_{n_0}$; l’inclusion opposée étant évidente, on a

$$
E_n = m^{n-n_0} E_{n_0},
$$

d’où $E_n = m E_{n-1}$ pour $n > n_0$.

C. Q. F. D.

#### Lemme 1 {#ac-iii-s3-lem-1 .statement}

Soient $A$ un anneau commutatif noethérien, $m$ un idéal de $A$. Alors le sous-anneau $A' = \sum_{n \geq 0} m^n X^n$ de $A[X]$ est noethérien.

En effet $A'$ est une $A$-algèbre engendrée par $mX$; comme $A$ est noethérien, $mX$ est un $A$-module de type fini, et la conclusion résulte donc du § 2, no 10, cor. 3 du th. 2.

#### Proposition 1 {#ac-iii-s3-prop-1 .statement}

Soient $A$ un anneau commutatif noethérien, $m$ un idéal de $A$; on munit $A$ de la filtration $m$-adique. Soient $E, F$ deux $A$-modules filtrés, $j : F \to E$ un homomorphisme injectif compatible avec les filtrations. Si $E$ est de type fini et si sa filtration est $m$-bonne, alors $F$ est de type fini et sa filtration est $m$-bonne.

Comme $F$ est isomorphe à un sous-module de $E$, il est de type fini puisque $A$ est noethérien et $E$ de type fini. Soient $(E_n), (F_n)$ les filtrations respectives de $E$ et $F$, qui sont formées de sous-modules de type fini ; gardons les notations du lemme 1 et posons $E' = \sum_{n \geq 0} E_n \otimes_A AX^n, \quad F' = \sum_{n \geq 0} F_n \otimes_A AX^n$; comme par hypothèse $F_n$ est isomorphe à un sous-module de $E_n$, on voit que $F'$ est isomorphe à un sous-module de $E'$. En vertu du th. 1, $E'$ est un $A'$-module de type fini, donc il en est de même de $F'$ puisque $A'$ est noethérien (lemme 1). D'où la conclusion en vertu du th. 1.

#### Corollaire 1 (lemme d’Artin-Rees) {#ac-iii-s3-prop-1-cor-1 .statement}

Soient $A$ un anneau commutatif noethérien, $m$ un idéal de $A$, $E$ un $A$-module de type fini, $F$ un sous-module de $E$. La filtration induite sur $F$ par la filtration $m$-adique de $E$ est $m$-bonne.

En d’autres termes, il existe un entier $n_0$ tel que l’on ait
$$
m((m^n E) \cap F) = (m^{n+1} E) \cap F
$$
pour tout $n \geq n_0$.

#### Corollaire 2 {#ac-iii-s3-prop-1-cor-2 .statement}

Soient $A$ un anneau commutatif noethérien, $a, b$ deux idéaux de $A$. Il existe un entier $h > 0$ tel que $a^h \cap b \subset ab$.

En effet, il existe $n$ tel que $a^{n+1} \cap b = a(a^n \cap b) \subset ab$ en vertu du cor. 1 appliqué à $E = A, F = b$.

#### Corollaire 3 {#ac-iii-s3-prop-1-cor-3 .statement}

Soient $A$ un anneau commutatif noethérien, $m$ un idéal de $A$, $x$ un élément de $A$ non diviseur de $0$. Il existe un entier $k > 0$ tel que, pour tout $n \geq k$, la relation $xy \in m^n$ entraîne $y \in m^{n-k}$.

En effet, le cor. 1 appliqué à $E = A$, $F = Ax$, montre qu’il existe $k$ tel que, pour tout $n \geq k$, on ait $m^n \cap Ax = m^{n-k}(m^k \cap Ax)$. Donc, si $xy \in m^n$, on a $xy \in m^n \cap Ax \subset m^{n-k}x$, et comme $x$ n’est pas diviseur de $0$, on en déduit $y \in m^{n-k}$.

Avec la notation des transporteurs (chap. I, § 2, no 10), la conclusion du cor. 3 s’écrit
$$
(2) \quad m^n : Ax \subset m^{n-k}.
$$

#### Corollaire 4 {#ac-iii-s3-prop-1-cor-4 .statement}

Soient $A$ un anneau commutatif noethérien, $m$ un idéal de $A$, $E$ un $A$-module de type fini, $(E_n)$ et $(E'_n)$ deux filtrations formées de sous-modules de $E$. On suppose que les filtrations $(E_n)$ et $(E'_n)$ sont compatibles avec la structure de $A$-module de $E$, quand on munit $A$ de la filtration $m$-adique. Si la filtration $(E_n)$ est $m$-bonne et si $E'_n \subset E_n$ pour tout $n \in \mathbf{Z}$, la filtration $(E'_n)$ est $m$-bonne.

C’est un cas particulier de la prop. 1.

#### Lemme 2 {#ac-iii-s3-lem-2 .statement}

Soient $A, B$ deux anneaux commutatifs noethériens, $\varphi : A \to B$ un homomorphisme d’anneaux, $E$ un $A$-module de type fini, $F$ un $B$-module de type fini. Alors $\mathrm{Hom}_A(E, \varphi_*(F))$ est un $B$-module de type fini.

En effet, il existe par hypothèse un $A$-homomorphisme surjectif $\varphi : A^n \to E$; l’application $u \to u \circ \varphi$ de $\mathrm{Hom}_A(E, \varphi_*(F))$ dans $\mathrm{Hom}_A(A^n, \varphi_*(F))$ est donc injective, et comme $B$ est noethérien, il suffit de prouver que $\mathrm{Hom}_A(A^n, \varphi_*(F))$ est un $B$-module de type fini ; ce qui est immédiat puisqu’il est isomorphe à $F^n$.

#### Proposition 2 {#ac-iii-s3-prop-2 .statement}

Soient $A$ un anneau commutatif noethérien, $m$ un idéal de $A$, $E, F$ deux $A$-modules de type fini. Si $(F_n)$ est une filtration $m$-bonne sur $F$, les sous-modules $\mathrm{Hom}_A(E, F_n)$ forment une filtration $m$-bonne du $A$-module $\mathrm{Hom}_A(E, F)$.

Comme on a $m^k F_n \subset F_{n+k}$ pour $n \in \mathbf{Z}$, $k \geq 0$, on a aussi
$$
m^k \mathrm{Hom}_A(E, F_n) \subset \mathrm{Hom}_A(E, F_{n+k});
$$
la famille $(\mathrm{Hom}_A(E, F_n))_{n \in \mathbf{Z}}$ est donc une filtration sur $\mathrm{Hom}_A(E, F)$, compatible avec sa structure de module sur l’anneau $A$ filtré parla filtration m-adique. Puisque E est de type fini, il existe un entier r > 0 et un A-homomorphisme surjectif u : Ar → E, qui définit un A-homomorphisme injectif

$$
\varphi = \operatorname{Hom}(u, 1_F) : \operatorname{Hom}_A(E, F) \to \operatorname{Hom}_A(A^r, F);
$$

il est clair que $\varphi$ est compatible avec les filtrations ($\operatorname{Hom}_A(E, F_n)$) et ($\operatorname{Hom}_A(A^r, F_n)$). Comme $\operatorname{Hom}_A(E, F)$ et $\operatorname{Hom}_A(A^r, F)$ sont de type fini (lemme 2), il suffit, en vertu de la prop. 1, de montrer que la filtration ($\operatorname{Hom}_A(A^r, F_n)$) est m-bonne ; mais cela est immédiat en vertu de l’existence de l’isomorphisme canonique $\operatorname{Hom}_A(A^r, F_n) \to F_n^r$ et du fait que la relation $mF_n = F_{n+1}$ entraîne $m(F_n^r) = (mF_n)^r = F_{n+1}^r$ (*Alg.*, chap. II, 3e éd., § 3, no 7, *Remarque*).

#### Proposition 3 {#ac-iii-s3-prop-3 .statement}

*Soient A un anneau noethérien, m un idéal de A tel que A soit séparé et complet pour la topologie m-adique. Soit E un A-module filtré sur l’anneau filtré A, la filtration (E_n) de E étant telle que E_0 = E, et que E soit séparé pour la topologie définie par (E_n). Alors les conditions suivantes sont équivalentes* :

a) *E est un A-module de type fini et (E_n) est une filtration m-bonne*.

b) *gr(E) est un gr(A)-module de type fini*.

c) *Pour tout n \geqslant 0, gr_n(E) est un A-module de type fini, et il existe n_0 tel que pour n \geqslant n_0 l’homomorphisme canonique*

$$
\operatorname{gr}_1(A) \otimes_A \operatorname{gr}_n(E) \to \operatorname{gr}_{n+1}(E)
$$

*soit surjectif*.

Il résulte aussitôt des définitions que a) implique c). Le fait que b) entraîne c) est conséquence du § 1, no 3, lemme 1 ; inversement, si c) est vérifiée, il est clair que gr(E) est engendré, en tant que gr(A)-module, par la somme des gr_p(E) pour p \leqslant n_0, donc admet par hypothèse un système fini de générateurs. Reste à prouver que c) implique a) ; comme les gr_n(E) sont de type fini et que E_0 = E, il est clair d’abord, par récurrence sur n, que E/E_n est un A-module de type fini pour tout n ; il suffira donc de prouver que pour n > n_0, E_n est un A-module de type fini et que l’on a mE_n = E_{n+1}. Or, considérons le A-module E_{n+1} muni de la filtration exhaustive et séparée des E_{n+k} (k \geqslant 1) ; on a mE_n \subset E_{n+1} ;

l’hypothèse c) entraîne que l’image de mE_n dans gr_{n+1}(E) = E_{n+1}/E_{n+2} est égale à gr_{n+1}(E) et engendre le gr(A)-module gradué gr(E_{n+1}). Comme gr_{n+1}(E) est par hypothèse un A-module de type fini, il résulte du § 2, no 9, prop. 12 que mE_n = E_{n+1} et que E_{n+1} est un A-module de type fini.

### 2. Topologies $m$-adiques sur les anneaux noethériens.

#### Proposition 4 {#ac-iii-s3-prop-4 .statement}

Soient A un anneau commutatif noethérien, $m$ un idéal de A, E un A-module de type fini. Toutes les filtrations $m$-bonnes sur E définissent la même topologie (savoir la topologie $m$-adique).

Soit $(E_n)$ une filtration $m$-bonne sur E. Comme cette filtration est exhaustive, tout élément de E appartient à un des $E_n$, et comme E est de type fini et les $E_n$ des A-modules, il existe un entier $n_1$ tel que $E_{n_1} = E$. Soit d’autre part $n_0$ tel que $mE_n = E_{n+1}$ pour $n \geq n_0$; pour $n > n_0 - n_1$, on a donc $m^n E \subset E_{n+n_1} = m^{n+n_1-n_0} E_{n_0} \subset m^{n+n_1-n_0} E$, ce qui démontre la proposition.

#### Théorème 2 (Krull) {#ac-iii-s3-thm-2 .statement}

Soient A un anneau commutatif noethérien, $m$ un idéal de A, E un A-module de type fini, F un sous-module de E. Alors la topologie $m$-adique de F est induite par la topologie $m$-adique de E.

En effet, il résulte du no 1, prop. 1, que la filtration induite sur F par la filtration $m$-adique de E est $m$-bonne, et la conclusion découle alors de la prop. 4.

#### Corollaire {#ac-iii-s3-n2-cor-1 .statement}

Soient A un anneau commutatif noethérien, $m$ un idéal de A, E un A-module, F un A-module de type fini. Toute application A-linéaire $u : E \to F$ est un morphisme strict (Top. gén., chap. III, 3e éd., § 2, no 8) pour les topologies $m$-adiques.

En effet, comme $u(m^n E) = m^n u(E)$, $u$ est un morphisme strict de E sur $u(E)$ pour les topologies $m$-adiques sur ces deux modules, et la topologie $m$-adique sur $u(E)$ est induite par la topologie $m$-adique sur F en vertu du th. 2.

#### Proposition 5 {#ac-iii-s3-prop-5 .statement}

Soient A un anneau commutatif nœthérien, m un idéal de A, E un A-module de type fini. L’adhérence $\bigcap_{n=1}^{\infty} m^n E$ de $\{0\}$ dans E pour la topologie m-adique est l’ensemble des $x \in E$ pour lesquels il existe un élément $m \in m$ tel que $(1 - m)x = 0$.

En effet, si $x = mx$ avec $m \in m$, on a $x = m^n x \in m^n E$ pour tout entier $n \geq 0$, donc $x \in F = \bigcap_{n=0}^{\infty} m^n E$. Inversement, si $x \in F$, $Ax$ est contenu dans l’intersection des voisinages de 0 dans E ; il résulte alors du th. 2 que la topologie m-adique sur $Ax$, qui est induite par celle de E, est la topologie la moins fine ; comme $mx$ est par définition un voisinage de 0 pour cette topologie, on a $mx = Ax$, donc il existe $m \in m$ tel que $x = mx$.

#### Corollaire (Krull) {#ac-iii-s3-n2-cor-2 .statement}

Soient A un anneau commutatif nœthérien, m un idéal de A. L’idéal $\bigcap_{n=1}^{\infty} m^n$ est l’ensemble des éléments $x \in A$ pour lesquels il existe un $m \in m$ tel que $(1 - m)x = 0$. En particulier, pour que $\bigcap_{n=1}^{\infty} m^n = \{0\}$, il faut et il suffit qu’aucun élément de $1 + m$ ne soit diviseur de zéro dans A.

Il suffit d’appliquer la prop. 5 à $E = A_s$.

#### Remarque {#ac-iii-s3-n2-rem-1 .statement}

L’hypothèse que A est nœthérien est essentielle dans ce corollaire. Par exemple, soit A l’anneau des applications indéfiniment différentiables de $\mathbf{R}$ dans lui-même, et soit m l’idéal (maximal) de A formé des fonctions $f$ telles que $f(0) = 0$. Il est immédiat que $\bigcap_{n=0}^{\infty} m^n$ est l’ensemble des fonctions $f$ telles que $f^{(n)}(0) = 0$ pour tout $n \geq 0$, et il existe de telles fonctions telles que $f(x) \neq 0$ pour tout $x \neq 0$, par exemple la fonction $f$ définie par $f(x) = e^{-1/x^2}$ pour $x \neq 0$ et $f(0) = 0$.

#### Définition 1 {#ac-iii-s3-def-1-bis .statement}

Soit $A$ un anneau topologique. Si un idéal bilatère $m$ de $A$ est tel que la topologie donnée sur $A$ soit la topologie $m$-adique, on dit que $m$ est un idéal de définition de la topologie de $A$.

Soient $A$ un anneau commutatif noethérien, $m$ un idéal de $A$, $t$ sa racine (chap. II, § 2, no 6). Si $m'$ est un idéal de définition de la topologie $m$-adique, il existe un entier $n > 0$ tel que ${m'}^n \subset m$ ($§ 2,$ no 5), donc $m' \subset t$; inversement, puisque $A$ est noethérien, il existe un entier $k > 0$ tel que $t^k \subset m$ (chap. II, § 2, no 6, prop. 15), donc $t$ est le plus grand idéal de définition de la topologie $m$-adique.

### 3. Anneaux de Zariski.

#### Proposition 6 {#ac-iii-s3-prop-6 .statement}

Soient $A$ un anneau commutatif noethérien, $m$ un idéal de $A$. Les propriétés suivantes sont équivalentes :
a) $m$ est contenu dans le radical de $A$.
b) Tout $A$-module de type fini est séparé pour la topologie $m$-adique.
c) Pour tout $A$-module $E$ de type fini, tout sous-module de $E$ est fermé pour la topologie $m$-adique de $E$.
d) Tout idéal maximal de $A$ est fermé pour la topologie $m$-adique.

Montrons que a) implique b). Supposons $m$ contenu dans le radical de $A$ et soit $E$ un $A$-module de type fini. Si $x \in E$ et $m \in m$ sont tels que $(1 - m)x = 0$, on a $x = 0$, car $1 - m$ est inversible dans $A$. Donc (no 2, prop. 5) $E$ est séparé pour la topologie $m$-adique.

Prouvons que b) entraîne c). Supposons b) vérifiée. Soient $E$ un $A$-module de type fini, $F$ un sous-module de $A$. Alors $E/F$ est séparé pour la topologie $m$-adique, qui est la topologie quotient de la topologie $m$-adique de $E$; donc $F$ est fermé dans $E$.

Il est clair que c) implique d). Démontrons enfin que d) implique a). Il résulte de d) que pour tout idéal maximal $a$ de $A$, le $A$-module $A/a$ est séparé pour la topologie $m$-adique. Cela entraîne $m(A/a) \neq A/a$, sinon la topologie $m$-adique de $A/a$ serait la topologie la moins fine, et $A/a$ serait réduit à 0, ce qui est absurde puisque $A/a$ est un corps. L'image canonique de $m$ dans $A/a$ est donc un idéal de $A/a$ distinct de $A/a$, donc est réduite à 0; on a par suite $m \subset a$, ce qui montre que $m$ est contenu dans le radical de $A$.

#### Définition 2 {#ac-iii-s3-def-2 .statement}

On dit qu’un anneau topologique $A$ est un anneau de Zariski s’il est commutatif et nœthérien et s’il existe un idéal de définition $m$ pour la topologie de $A$, satisfaisant aux conditions équivalentes de la prop. 6.

Un anneau de Zariski $A$ est nécessairement séparé (prop. 6), et tout idéal de définition pour sa topologie est contenu dans le radical de $A$.

Exemples d’anneaux de Zariski. — 1) Soient $A$ un anneau commutatif nœthérien, $m$ un idéal de $A$. Si $A$ est séparé et complet pour la topologie $m$-adique, $A$ est un anneau de Zariski pour cette topologie, en vertu du § 2, n° 13, lemme 3.

2) Tout anneau quotient $A/b$ d’un anneau de Zariski est un anneau de Zariski, car il est nœthérien, et si $m$ est un idéal de définition de $A$, $m(A/b) = (m + b)/b$ est contenu dans le radical de $A/b$ (Alg., chap. VIII, § 6, n° 3, prop. 7).

3) Soient $A$ un anneau semi-local nœthérien, $r$ son radical. Alors $A$, muni de la topologie $r$-adique, est un anneau de Zariski. C’est toujours de cette topologie qu’il sera question (sauf mention expresse du contraire) quand on considérera un anneau semi-local nœthérien comme un anneau topologique.

#### Proposition 7 {#ac-iii-s3-prop-7 .statement}

Soient $A, A'$ deux anneaux commutatifs, $h : A \to A'$ un homomorphisme d’anneaux. On suppose que $A$ est nœthérien et que $A'$ est un $A$-module de type fini (pour la structure de module définie par $h$). Soit $m$ un idéal de $A$, et soit $m' = mA'$. Alors :

(i) Pour que la topologie $m'$-adique de $A'$ soit séparée, il faut et il suffit que les éléments de $1 + h(m)$ soient non diviseurs de 0 dans $A'$.

(ii) Si $A$, muni de la topologie $m$-adique, est un anneau de Zariski, alors $A'$, muni de la topologie $m'$-adique, est un anneau de Zariski.

(iii) Si $h$ est injectif (identifiant ainsi $A$ à un sous-anneau de $A'$) la topologie $m'$-adique de $A'$ induit sur $A$ la topologie $m$-adique.

Rappelons que la filtration $m'$-adique de $A'$ coïncide avec la filtration $m$-adique du $A$-module $A'$ ($\S 2$, n° 1, Exemple 3). L’assertion (i) est donc un cas particulier de la prop. 5 du n° 2, et l’assertion (iii) un cas particulier du th. 2 du n° 2. Démontrons enfin (ii). Supposons que A soit un anneau de Zariski pour la topologie m-adique, et soit E' un A'-module de type fini ; c'est aussi un A-module de type fini, et les filtrations m-adique et m'-adique sur E' coïncident ; donc E' est séparé pour la topologie m'-adique. Enfin le A-module A' est noethérien, donc l'anneau A' est noethérien, ce qui achève de prouver que A' est un anneau de Zariski.

### 4. Séparé complété d'un anneau noethérien.

Soient A un anneau commutatif, m un idéal de A, E un A-module ; notons $\hat{A}$ et $\hat{E}$ les séparés complétés respectifs de A et E pour les topologies m-adiques, et $j_E$ l'application canonique $E \to \hat{E}$. L'application A-bilinéaire $(a, x) \to aj_E(x)$ de $\hat{A} \times E$ dans $\hat{E}$ définit une application $\hat{A}$-linéaire $\alpha_E : \hat{A} \otimes_A E \to \hat{E}$, dite canonique. Soit $u : E \to F$ un homomorphisme de A-modules, et soit $\hat{u} : \hat{E} \to \hat{F}$ l'application qu'on en déduit par passage aux séparés complétés ; pour $a \in \hat{A}$, $x \in E$, on a
$$
\alpha_F(a \otimes u(x)) = aj_F(u(x)) = a \hat{u}(j_E(x)) = \hat{u}(\alpha_E(a \otimes x)),
$$
autrement dit, le diagramme

$$
\begin{array}{ccc}
\hat{A} \otimes_A E & \xrightarrow{1 \otimes u} & \hat{A} \otimes_A F \\
\alpha_E \downarrow & & \downarrow \alpha_F \\
\hat{E} & \xrightarrow{\hat{u}} & \hat{F}
\end{array}
$$

est commutatif. Enfin, il résulte du § 2, n° 12, prop. 16 que si E est de type fini, l'homomorphisme $\alpha_E$ est surjectif.

#### Théorème 3 {#ac-iii-s3-thm-3 .statement}

Soient A un anneau commutatif noethérien, m un idéal de A, E, F, G trois A-modules de type fini. Alors :
(i) Si $E \xrightarrow{u} F \xrightarrow{v} G$ est une suite exacte d'applications A-linéaires, la suite $\hat{E} \xrightarrow{\hat{u}} \hat{F} \xrightarrow{\hat{v}} \hat{G}$ qu'on en déduit par passage aux séparés complétés (pour les topologies m-adiques) est exacte.
(ii) L'application $\hat{A}$-linéaire canonique $\alpha_E : \hat{A} \otimes_A E \to \hat{E}$ est bijective.
(iii) Le A-module $\hat{A}$ est plat.

On a vu que $u$ et $v$ sont des morphismes stricts de groupes topologiques (no 2, cor. du th. 2). L’assertion (i) résulte donc du § 2, no 12, lemme 2. L’assertion (ii) est évidente lorsque $E = A$, et le cas où $E$ est un $A$-module libre de type fini se ramène aussitôt à celui-là. Dans le cas général, $E$ admet une présentation de type fini

$$
L \xrightarrow{u} L' \xrightarrow{v} E \to 0
$$

(chap. I, § 2, no 8, lemme 8). On en déduit le diagramme commutatif

$$
\begin{array}{cccccc}
\hat{A} \otimes_A L & \xrightarrow{1 \otimes u} & \hat{A} \otimes_A L' & \xrightarrow{1 \otimes v} & \hat{A} \otimes_A E & \longrightarrow 0 \\
\alpha_L \downarrow & & \downarrow \alpha_{L'} & & \downarrow \alpha_E & \\
\hat{L} & \xrightarrow{\hat{u}} & \hat{L}' & \xrightarrow{\hat{v}} & \hat{E} & \longrightarrow 0
\end{array}
$$

La première ligne est exacte (chap. I, § 2, no 1, lemme 1) et il en est de même de la seconde d’après (i). On sait déjà que $\alpha_E$ est surjectif ($\S 2$, no 12, prop. 16); d’autre part, comme $\alpha_L$ et $\alpha_{L'}$ sont bijectifs et $1 \otimes v$ surjectif, $\alpha_E$ est injectif en vertu du chap. I, § 1, no 4, cor. 2 de la prop. 2; ceci démontre (ii).

Il résulte alors de (i) et (ii) que si $a$ est un idéal de $A$ (nécessairement de type fini), l’application canonique $\hat{A} \otimes_A a \to \hat{A}$ est injective, étant composée de $\hat{a} \to \hat{A}$ et de $\alpha_E$, ce qui prouve que $\hat{A}$ est un $A$-module plat (chap. I, § 2, no 3, prop. 1).

C. Q. F. D.

Sous les conditions du th. 3, on identifie souvent $\hat{A} \otimes_A E$ à $\hat{E}$ au moyen de l’application canonique $\alpha_E$. Si $u : E \to F$ est un homomorphisme de $A$-modules de type fini, $\hat{u} : \hat{E} \to \hat{F}$ se trouve alors identifié à $1 \otimes u$ en vertu de la commutativité du diagramme (4).

#### Corollaire 1 {#ac-iii-s3-thm-3-cor-1 .statement}

*Soient A un anneau commutatif noethérien, m un idéal de A, E un A-module de type fini, F et G deux sous-modules de E. Munissons A, E, F et G des topologies m-adiques, et soit i l’application canonique de E dans $\hat{E}$. On a alors*:

$$
\hat{F} = \hat{A}.i(F), \quad (F + G)^{\sim} = \hat{F} + \hat{G}, \quad (F \cap G)^{\sim} = \hat{F} \cap \hat{G},
$$
$$
(F : G)^{\sim} = \hat{F} : \hat{G}.
$$

*En outre, si a et b sont deux idéaux de A, et si c = ab, on a $\hat{c} = \hat{a}\hat{b}$.*

En effet, en vertu du th. 3, $\hat{E}, \hat{F}, \hat{G}$ s’identifient canoniquement à $\hat{A} \otimes E, \hat{A} \otimes F, \hat{A} \otimes G$, ce qui démontre les deux premières formules. La troisième et la quatrième résultent respectivement du chap. I, § 2, no 6, prop. 6 et no 10, prop. 12. Enfin comme $\hat{a} = \hat{A}i(a), \hat{b} = \hat{A}i(b), \hat{c} = \hat{A}i(c)$, on a bien
$$
\hat{c} = \hat{A}i(ab) = \hat{A}i(a)i(b) = \hat{a}\hat{b}.
$$

#### Corollaire 2 {#ac-iii-s3-thm-3-cor-2 .statement}

*Soient A un anneau commutatif noethérien, m un idéal de A, $\hat{A}$ le séparé complété de A pour la topologie m-adique. Si un élément $a \in A$ est non diviseur de 0 dans A, son image canonique $a'$ dans $\hat{A}$ est non diviseur de 0 dans $\hat{A}$.

Comme $\hat{A}$ est un A-module plat, le corollaire est un cas particulier du chap. I, § 2, no 4, prop. 3, (i).

#### Corollaire 3 {#ac-iii-s3-thm-3-cor-3 .statement}

*Si A est un anneau commutatif noethérien, l’anneau de séries formelles $A[[X_1, ..., X_n]]$ est un A-module plat.

En effet c’est le complété de l’anneau de polynômes
$$
B = A[X_1, ..., X_n]
$$
pour la topologie m-adique, où m est l’ensemble des polynômes sans terme constant ($\S 2,$ no 12, *Exemple 1*); comme B est noethérien ($\S 2,$ no 10, cor. 2 du th. 2), $A[[X_1, ..., X_n]]$ est un B-module plat en vertu du th. 3, et comme B est un A-module libre, $A[[X_1, ..., X_n]]$ est un A-module plat (chap. I, § 2, no 7, cor. 3 de la prop. 8).

#### Proposition 8 {#ac-iii-s3-prop-8 .statement}

*Soient A un anneau commutatif noethérien, m un idéal de A, $\hat{A}$ le séparé complété de A pour la topologie m-adique, j l’application canonique de A dans $\hat{A}$. Alors :
(i) $\hat{A}$ est un anneau de Zariski et $\hat{m} = \hat{A}.j(m)$ est un idéal de définition de $\hat{A}$.
(ii) *L’application* $n \to \hat{n} = \hat{A}.j(n)$ *est une bijection de l’ensemble des idéaux maximaux de A contenant m sur l’ensemble des idéaux maximaux de $\hat{A}$, et $q \to \hat{j}(q)$ *est la bijection réciproque*.
(iii) *Soit n un idéal maximal de A contenant m. L’homomorphisme* $j' : A_n \to \hat{A}_{\hat{n}}$ *déduit de j est injectif ; si on identifie* $A_n$ *au moyen* de $j'$ à un sous-anneau de $\hat{A}_{\hat{n}}$, la topologie $(nA_n)$-adique de $A_n$ est induite par la topologie $\hat{n}$-adique de $\hat{A}_{\hat{n}}$, et $A_n$ est dense dans $\hat{A}_{\hat{n}}$ pour la topologie $\hat{n}$-adique.

Démontrons (i). Comme $m$ est un idéal de type fini, on a $(m^n)^{\sim} = (\hat{m})^n = m^n \hat{A}$ (\S 2, no 12, cor. 2 de la prop. 16) et la topologie de $\hat{A}$ est la topologie $\hat{m}$-adique. Comme $\hat{A}/\hat{m}$ est isomorphe à $A/m$, c'est un anneau nœthérien, et $\hat{m} = m \hat{A}$ est un $\hat{A}$-module de type fini, donc $\hat{A}$ est nœthérien (\S 2, no 10, cor. 5 du th. 2); enfin, comme $\hat{A}$ est séparé et complet pour la topologie $\hat{m}$-adique, $\hat{A}$ est un anneau de Zariski (no 3, Exemple 1).

L’assertion (ii) résulte aussitôt de ce que l’homomorphisme canonique $A/m \to \hat{A}/\hat{m}$ déduit de $j$ est bijectif et du fait que tout idéal maximal de $\hat{A}$ contient $\hat{m}$, puisque $\hat{A}$ est un anneau de Zariski et que le radical de $\hat{A}$ contient donc $\hat{m}$ (no 3, prop. 6).

Prouvons enfin (iii). Comme $n = j^{-1}(\hat{n})$, on a $j(A - n) \subset \hat{A} - \hat{n}$, et $j$ définit bien un homomorphisme $j' : A_n \to \hat{A}_{\hat{n}}$ (chap. II, \S 2, no 1, prop. 2). Montrons que $j'$ est injectif; soient $a \in A, s \in A - n$ tels que $j'(a/s) = j(a)/j(s) = 0$; il existe donc $s' \in \hat{A} - \hat{n}$ tel que $s'j(a) = 0$ (chap. II, \S 2, no 1, Remarque 3), et l’annulateur de $j(a)$ dans $\hat{A}$ n’est donc pas contenu dans $\hat{n}$. Or, si $b$ est l’annulateur de $a$ dans $A$, l’annulateur de $j(a)$ dans $\hat{A}$ est $\hat{b}$ (cor. 1 du th. 3); donc $b \notin n$, ce qui montre que $a/s = 0$.

En outre, on a un diagramme commutatif

$$
\begin{array}{ccc}
A/n^k & \longrightarrow & A_n/(nA_n)^k \\
\downarrow h & & \downarrow h' \\
\hat{A}/\hat{n}^k & \longrightarrow & \hat{A}_{\hat{n}}/(\hat{n}\hat{A}_{\hat{n}})^k
\end{array}
$$

où $h$ et $h'$ sont déduits de $j$ et $j'$ respectivement, et où les flèches horizontales sont les isomorphismes canoniques du chap. II, \S 3, no 3, prop. 9. Comme $n^k$ est un idéal ouvert de $A$ (puisqu’il contient $m^k$), $h$ est bijectif, donc il en est de même de $h'$. Ceci montre d’abord que $(nA_n)^k = {j'}^{-1}((\hat{n}\hat{A}_{\hat{n}})^k)$, donc la topologie de $A_n$ est induite par celle de $\hat{A}_{\hat{n}}$; en outre, on a $\hat{A}_{\hat{n}} = A_n + (\hat{n}\hat{A}_{\hat{n}})^k$ pour tout $k > 0$, donc $A_n$ est partout dense dans $\hat{A}_{\hat{n}}$.

C. Q. F. D.

#### Corollaire {#ac-iii-s3-n4-cor-1 .statement}

Soient $A$ un anneau local (resp. semi-local) noethérien, $m$ son radical. Alors $\hat{A}$ est un anneau local (resp. semi-local) noethérien dont le radical est $\hat{m}$.

En effet, $\hat{A}$ est noethérien en vertu de la prop. 8, (i), et le reste résulte de la prop. 8, (ii) et de la troisième formule du cor. 1 du th. 3.

### 5. Complété d’un anneau de Zariski.

#### Proposition 9 {#ac-iii-s3-prop-9 .statement}

Soient $\Lambda$ un anneau commutatif noethérien, $m$ un idéal de $\Lambda$; munissons $\Lambda$ de la topologie $m$-adique. Pour que $\hat{\Lambda}$ soit un $\Lambda$-module fidèlement plat, il faut et il suffit que $\Lambda$ soit un anneau de Zariski.

En effet, pour tout $\Lambda$-module de type fini $M$, l’application canonique $M \to M \otimes_{\Lambda} \hat{\Lambda}$ s’identifie à l’application canonique $M \to \hat{M}$ de $M$ dans son séparé complété pour la topologie $m$-adique (no 4, th. 3), et le noyau de cette application est donc l’adhérence de $\{0\}$ dans $M$ pour cette topologie. Comme on sait déjà que $\hat{\Lambda}$ est un $\Lambda$-module plat (no 4, th. 3), la proposition résulte de la caractérisation des modules fidèlement plats (chap. I, § 3, no 1, prop. 1 b)) et de la caractérisation des anneaux de Zariski (no 3, prop. 6).

Si $A$ est un anneau de Zariski et si $E$ est un $A$-module de type fini on peut (en vertu de la prop. 9) identifier $E$ à une partie de $\hat{E}$ au moyen de l’application canonique $j_e : E \to \hat{E}$. Avec cette identification :

#### Corollaire 1 {#ac-iii-s3-prop-9-cor-1 .statement}

Soient $A$ un anneau de Zariski, $E$ un $A$-module de type fini, $F$ un sous-module de $E$. Alors $F = \hat{F} \cap E = (\hat{A}F) \cap E$.

C’est un cas particulier du chap. I, § 3, no 5, prop. 10, (ii), et résulte aussi d’ailleurs du no 3, prop. 6.

#### Corollaire 2 {#ac-iii-s3-prop-9-cor-2 .statement}

Soient $A$ un anneau de Zariski, $E$ un $A$-module de type fini. Si $\hat{E}$ est un $\hat{A}$-module libre, $E$ est un $A$-module libre.

Soit $m$ un idéal de définition de $A$, qui est donc contenu dans le radical de $A$. Appliquons le critère du chap. II, § 3, no 2, prop. 5:

l’application canonique $j_E : E \to \hat{E}$ définit une bijection $i_{j_E} : E/mE \to \hat{E}/(mE)^{\sim}$; de même l’application canonique $j_A : A \to \hat{A}$ définit une bijection $i_A : A/m \to \hat{A}/\hat{m}$, qui est un isomorphisme d’anneaux. On a $(mE)^{\sim} = \hat{A}.mE = \hat{m}\hat{E}$ (no 4, th. 3), de sorte que $\hat{E}/(mE)^{\sim}$ est muni d’une structure de $(\hat{A}/\hat{m})$-module, donc (à l’aide de $i_A$) d’une structure de $(A/m)$-module. Il est immédiat que $i_E$ est $(A/m)$-linéaire, de sorte que c’est un isomorphisme de $(A/m)$-modules. Comme $\hat{E}/\hat{m}\hat{E}$ est un $(\hat{A}/\hat{m})$-module libre, $E/mE$ est un $(A/m)$-module libre.

Par ailleurs, soit $\varphi : m \otimes_A E \to E$ l’homomorphisme canonique; comme $(m \otimes_A E) \otimes_A \hat{A}$ s’identifie canoniquement à $\hat{m} \otimes_{\hat{A}} \hat{E}$ et $E \otimes_A \hat{A}$ à $\hat{E}$ (no 4, th. 3), l’hypothèse que $\hat{E}$ est un $\hat{A}$-module libre entraîne que l’homomorphisme $\varphi \otimes 1 : \hat{m} \otimes_{\hat{A}} \hat{E} \to \hat{E}$ est injectif. Comme $\hat{A}$ est un $A$-module fidèlement plat (prop. 9), on en conclut que $\varphi$ est injectif (chap. I, § 3, no 1, prop. 2) et les conditions d’application du critère précité sont bien remplies.

#### Corollaire 3 {#ac-iii-s3-prop-9-cor-3 .statement}

Soient $A$ un anneau de Zariski tel que $\hat{A}$ soit intègre, $a$ un idéal de $A$. Si l’idéal $a\hat{A}$ de $\hat{A}$ est principal, $a$ est principal.
C’est un cas particulier du cor. 2.

#### Corollaire 4 {#ac-iii-s3-prop-9-cor-4 .statement}

Soient $A$ un anneau de Zariski tel que $\hat{A}$ soit intègre, $L$ le corps des fractions de $\hat{A}$, $K \subset L$ le corps des fractions de $A$; on a $\hat{A} \cap K = A$.

Il est clair que $A \subset \hat{A} \cap K$; d’autre part, si $x \in \hat{A} \cap K$, on a $\hat{A}x \subset \hat{A}$, donc comme $\hat{A}x = \hat{A} \otimes_A (Ax)$ (no 4, th. 3) on a $\hat{A} \otimes_A ((Ax + A)/A) = 0$. Comme $\hat{A}$ est un $A$-module fidèlement plat (prop. 9), on en déduit $Ax \subset A$, d’où $x \in A$.

#### Corollaire 5 {#ac-iii-s3-prop-9-cor-5 .statement}

Soient $A$ un anneau commutatif nœthérien, $E, F$ deux $A$-modules de type fini, $u : E \to F$ un $A$-homomorphisme. Pour tout idéal maximal $m$ de $A$, notons $A(m)$ (resp. $E(m)$, $F(m)$) le séparé complété de $A$ (resp. $E, F$) pour la topologie $m$-adique, par $u(m) : E(m) \to F(m)$ l’homomorphisme correspondant à $u$. Pour que $u$ soit injectif (resp. surjectif, bijectif, nul), il faut et il suffit que $u(m)$ le soit pour tout idéal maximal $m$ de $A$.

On sait en effet que pour que $u$ soit injectif (resp. surjectif, bijectif, nul), il faut et il suffit que $u_m : E_m \to F_m$ le soit pour tout idéal maximal $m$ de $A$ (chap. II, § 3, no 3, th. 1). Notons maintenant que $A_m$ est un anneau local noethérien (chap. II, § 2, no 4, cor. 2 de la prop. 10), donc un anneau de Zariski, et il y a un isomorphisme canonique de $A$-algèbres $\hat{A}_m \to A(m)$ ($\S 2,$ no 13, prop. 18). D'autre part (début du no 4), on a un diagramme commutatif

$$
\begin{array}{ccc}
E_m \otimes_{A_m} A(m) & \longrightarrow & E \otimes_A A(m) \longrightarrow E(m) \\
u_m \otimes 1 \downarrow & & \downarrow u \otimes 1 \quad \downarrow u(m) \\
F_m \otimes_{A_m} A(m) & \longrightarrow & F \otimes_A A(m) \longrightarrow F(m)
\end{array}
$$

où les flèches horizontales de gauche proviennent de l’associativité du produit tensoriel et des isomorphismes $E_m \to E \otimes_A A_m$, $F_m \to F \otimes_A A_m$; comme $E$ et $F$ sont des $A$-modules de type fini, il résulte du no 4, th. 3, que les lignes horizontales de ce diagramme sont formées d’isomorphismes ; tout revient donc à montrer qu’il est équivalent que $u_m$ soit injectif (resp. surjectif, bijectif, nul) et que $u_m \otimes 1$ le soit. Mais cela résulte du fait que $\hat{A}_m$ (donc aussi $A(m)$) est un $A_m$-module fidèlement plat d’après la prop. 9 (chap. I, § 3, no 1, prop. 1 et 2).

#### Proposition 10 {#ac-iii-s3-prop-10 .statement}

*Soient $A, B$ deux anneaux de Zariski, $\hat{A}, \hat{B}$ leurs complétés, $f : A \to B$ un homomorphisme continu d’anneaux, $\hat{f} : \hat{A} \to \hat{B}$ l’homomorphisme déduit de $f$ par passage aux complétés ; si $\hat{f}$ est bijectif, le $A$-module $B$ est fidèlement plat.*

Comme $A$ et $B$ sont séparés, l’hypothèse que $\hat{f}$ est bijectif entraîne d’abord que $f$ est injectif. Identifiant (algébriquement) $A$ à $f(A)$ au moyen de $f$ et $\hat{A}$ à $\hat{B}$ au moyen de $\hat{f}$, on a donc les inclusions $A \subset B \subset \hat{A} = \hat{B}$; on sait que $\hat{A}$ est un $A$-module fidèlement plat et un $B$-module fidèlement plat (prop. 9); on en conclut que $B$ est un $A$-module fidèlement plat (chap. I, § 3, no 4, Remarque 2).

#### Proposition 11 {#ac-iii-s3-prop-11 .statement}

*Soient $A$ un anneau local noethérien, $m$ son idéal maximal, $\hat{A}$ son complété $m$-adique, $B$ un anneau tel que $A \subset B \subset \hat{A}$. Supposons que $B$ soit un anneau local noethérien dont l’idéal maximal $\mathfrak{n}$ vérifie la relation $\mathfrak{n} = mB$. On a alors*

$$
\mathfrak{n}^k = m^kB = \hat{m}^k \cap B
$$

pour tout $k \geqslant 1$, la topologie $n$-adique de $B$ est induite par la topologie $\hat{m}$-adique de $\hat{A}$, $B$ est un $A$-module fidèlement plat, et il y a un isomorphisme de $\hat{A}$ sur le complété $n$-adique $\hat{B}$ de $B$, qui prolonge l'injection canonique $A \to B$.

Il suffit de vérifier la relation $n^k = \hat{m}^k \cap B$, car $B$ étant dense dans $\hat{A}$ et la topologie $n$-adique induite par la topologie $\hat{m}$-adique, la dernière assertion résultera de Top. gén., chap. II, 3e éd., § 3, no 9, cor. 1 de la prop. 18, et l'avant-dernière de la prop. 10. L'injection $j_A : A \to \hat{A}$ (resp. $j_B : B \to \hat{A}$) définit par passage aux quotients un homomorphisme injectif $i_A : A/(\hat{m} \cap A) \to \hat{A}/\hat{m}$ (resp. $i_B : B/(\hat{m} \cap B) \to \hat{A}/\hat{m}$). On sait que $\hat{m} \cap A = m$ et que $i_A$ est bijectif, donc $i_B$ est bijectif, ce qui montre que $B/(\hat{m} \cap B)$ est un corps, donc que $\hat{m} \cap B$ est un idéal maximal de $B$, et par suite $\hat{m} \cap B = n$. Comme $\hat{A} = A + \hat{m}$, on a $B = A + n = A + mB$; par récurrence sur $k$, on en déduit que $B = A + m^kB = A + n^k$ pour tout $k > 1$. Comme on a $n^k \subset \hat{m}^k \cap B$, il suffit de montrer que $\hat{m}^k \cap B \subset n^k$; si $b \in \hat{m}^k \cap B$, on peut écrire $b = a + z$ avec $a \in A$, $z \in n^k$; d'où $a = b - z \in \hat{m}^k \cap A = m^k \subset n^k$, et $b \in n^k$.

*Un cas important où ceci s'applique est le suivant : B est l'anneau des séries entières à $n$ variables sur un corps valué complet K, qui convergent au voisinage de 0, A est l'anneau local

$$
K[X_1, ..., X_n]_p
$$

où $p$ est l'idéal maximal formé des polynômes sans terme constant, et $\hat{A}$ est l'anneau de séries formelles $K[[X_1, ..., X_n]]$*

#### Remarque {#ac-iii-s3-n5-rem-1 .statement}

Un anneau local B tel que $A \subset B \subset \hat{A}$, dont l'idéal maximal $n$ est égal à $mB$ et dont la topologie $n$-adique est induite par la topologie $\hat{m}$-adique de $\hat{A}$, n'est pas nécessairement noethérien (exerc. 14).

#### Proposition 12 {#ac-iii-s3-prop-12 .statement}

Soient A un anneau commutatif noethérien, $m$ un idéal de A, S la partie multiplicative $1 + m$ de A, E un A-module de type fini. Dans ces conditions :

(i) $S^{-1}A$ est un anneau de Zariski pour la topologie $(S^{-1}m)$-adique.

(ii) L'application canonique $f : E \to S^{-1}E$ est continue quand on munit E de la topologie $m$-adique et $S^{-1}E$ de la topologie $(S^{-1}m)$-adique, et $\hat{f} : \hat{E} \to (S^{-1}E)^{\sim}$ est un isomorphisme.

Tout élément de $1 + (S^{-1}\mathfrak{m})$ est de la forme
$$
1 + (m/(1 + m')) = (1 + m + m')/(1 + m)
$$
avec $m \in \mathfrak{m}$ et $m' \in \mathfrak{m}$; il est par suite inversible dans $S^{-1}A$, ce qui prouve que $S^{-1}\mathfrak{m}$ est contenu dans le radical de $S^{-1}A$; comme $S^{-1}A$ est noethérien (chap. II, § 2, no 4, cor. 2 de la prop. 10), $S^{-1}A$ est un anneau de Zariski pour la topologie $(S^{-1}\mathfrak{m})$-adique, ce qui prouve (i). Démontrons (ii). Pour tout $n > 0$, on a
$$
f((S^{-1}\mathfrak{m})^nE) = f(S^{-1}(m^nE)) = m^nE :
$$
en effet, il est clair tout d’abord que $f(m^nE) \subset S^{-1}m^nE$; inversement, soit $x$ un élément de $f(S^{-1}m^nE)$; il existe donc des éléments $m', m''$ de $\mathfrak{m}$ et un $x'' \in m^nE$ tels que $(1 + m')((1 + m'')x - x'') = 0$, d’où $(1 - m)x = x'$ avec $m = -(m' + m'' + m'm'') \in \mathfrak{m}$ et $x' = (1 + m')x'' \in m^nE$; on en conclut
$$
x = (1 + m + ... + m^{n-1})x' + m^n x \in m^nE.
$$
Ceci prouve que $f$ est un morphisme strict. De plus, le noyau de $f$, qui est l’ensemble des $x \in E$ pour lesquels il existe un $s \in S$ tel que $sx = 0$, est identique au noyau de l’application canonique $j : E \to \widehat{E}$ (no 2, prop. 5). Il y a donc un isomorphisme topologique $f_0 : j(E) \to f(E)$ tel que $f = f_0 \circ j$; comme $\widehat{j}$ est un isomorphisme topologique, tout revient à voir que $f(E)$ est dense dans $S^{-1}E$. Or tout élément de $S^{-1}E$ s’écrit $x/(1 - m)$ avec $m \in \mathfrak{m}$, et on vérifie aussitôt que
$$
x/(1 - m) \equiv ((1 + m + ... + m^{n-1})x)/1 \pmod{S^{-1}m^nE}
$$
ce qui achève la démonstration.

## EXERCICES {#ac-iii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
