---
book: ac
book_title: Commutative Algebra
chapter: VIII
chapter_title: DIMENSION
section: 2
section_title: Dimension des algèbres
lang: fr
source: ac-viii-ix-fr
book_pages: AC VIII.13-AC VIII.23
pdf_pages: 0017-0027, 0088-0090
extraction: ocr
subsections:
    - "no": 1
      title: Dimension et platitude
      page: 13
      pdf_page: 17
    - "no": 2
      title: Dimension d’une algèbre de type fini
      page: 16
      pdf_page: 20
    - "no": 3
      title: Dimension d’une algèbre entière
      page: 0
      pdf_page: 21
    - "no": 4
      title: Algèbres de type fini sur un corps
      page: 19
      pdf_page: 23
statements: 32
exercises: 18
content_sha256: adc2a4e954a088d296502eb1f4f4669ae89dd263f74cfb2153cbce9b5d909848
---

## § 2. DIMENSION DES ALGÈBRES

### 1. Dimension et platitude

Soit $\rho : A \to B$ un homomorphisme d’anneaux. On note (PM) la condition suivante :
(PM) Il existe un B-module N fidèlement plat sur A tel que, pour tout idéal premier q de B, on ait $N \otimes_B \kappa(q) \neq 0$.

#### Remarque 1 {#ac-viii-s2-n1-rem-1 .statement}

La condition (PM) est satisfaite lorsqu’il existe un B-module de type fini, fidèlement plat sur A et de support égal à Spec(B). C’est le cas, en particulier, si le A-module B est fidèlement plat.

#### Remarque 2 {#ac-viii-s2-n1-rem-2 .statement}

L’existence d’un B-module N fidèlement plat sur A implique l’injectivité de ρ (I, § 3, n° 5, prop. 8), et la surjectivité de l’application “ρ : Spec(B) → Spec(A) (II, § 2, n° 5, cor. 4 à la prop. 11).

#### Remarque 3 {#ac-viii-s2-n1-rem-3 .statement}

Supposons que ρ : A → B soit un homomorphisme local d’anneaux locaux et qu’il existe un B-module N plat sur A et tel que N ⊗_B κ(q) ≠ 0 pour tout idéal premier q de B. Alors N est fidèlement plat sur A et ρ jouit donc de la propriété (PM) : en effet on a N/m_B N = N ⊗_B κ(m_B) ≠ 0, donc N ≠ m_B N et a fortiori N ≠ m_A N, et la conclusion résulte de la prop. 1 de I, § 3, n° 1.

#### Proposition 1 {#ac-viii-s2-prop-1 .statement}

Soit ρ : A → B un homomorphisme d’anneaux satisfaisant à la condition (PM).

a) Soit h : A → A′ un homomorphisme d’anneaux. Alors l’homomorphisme ρ′ : A′ → A′ ⊗_A B déduit de ρ satisfait à la condition (PM).

b) Soient q un idéal premier de B et p = ρ^{-1}(q). L’homomorphisme canonique ρ_q : A_p → B_q satisfait à la condition (PM).

c) Soient q un idéal premier de B et p = ρ^{-1}(q). Pour tout idéal premier p′ de A contenu dans p, il existe un idéal premier q′ de B au-dessus de p′ et contenu dans q.

Soit N un B-module fidèlement plat sur A et tel que N ⊗_B κ(q) ≠ 0 pour tout idéal premier q de B.

Démontrons a). Le A′-module N′ = A′ ⊗_A N est fidèlement plat (I, § 3, n° 3, prop. 5); soient q′ un idéal premier de B′ = A′ ⊗_A B et q son image réciproque dans B. On a des isomorphismes

$$ N' \otimes_{B'} \kappa(q') \to N \otimes_B \kappa(q') \to (N \otimes_B \kappa(q)) \otimes_{\kappa(q)} \kappa(q'); $$

comme on a N ⊗_B κ(q) ≠ 0, on a aussi N′ ⊗_{B′} κ(q′) ≠ 0.

Démontrons b). D’après les prop. 13 et 14 de II, § 3, n° 4, le A_p-modulé N_q est plat. D’autre part, soit b′ un idéal premier de B_q ; il est de la forme bB_q où b est un idéal premier de B contenu dans q (II, § 3, n° 1, prop. 3); on a N ⊗_B κ(b) ≠ 0 vu l’hypothèse faite sur N, et comme N_q ⊗_{B_q} κ(b′) est isomorphe à N ⊗_B κ(b′), on a N_q ⊗_{B_q} κ(b′) ≠ 0. La remarque 3 permet de conclure.

Démontrons c). L’homomorphisme local ρ_q : A_p → B_q déduit de ρ satisfait à la condition (PM) d’après b). L’application Spec(B_q) → Spec(A_p) est donc surjective (remarque 2), ce qu’on voulait démontrer.

#### Corollaire {#ac-viii-s2-n1-cor-1 .statement}

Soit F une partie fermée de Spec(A). Si Y est une composante irréductible de l’image réciproque de F par l’application “ρ : Spec(B) → Spec(A), alors l’adhérence de “ρ(Y) est une composante irréductible de F.

Soient en effet a un idéal de A tel que F = V(a) et q l’idéal premier de B tel que Y = V(q). L’image réciproque par “ρ de F est la partie V(ρ(a)B) de Spec(B) et l’adhérence de “ρ(Y) est la partie fermée irréductible V(ρ^{-1}(q)) de Spec(A).

Il s’agit de prouver que si q est minimal parmi les idéaux premiers de B contenant $\rho(a)$, alors $\rho^{-1}(q)$ est minimal parmi les idéaux premiers de A contenant a. Dans le cas contraire, il existerait un idéal premier $p'$ de A avec $a \subset p' \subset \rho^{-1}(q)$ et $p' \neq \rho^{-1}(q)$; d’après la prop. 1, c), il existerait un idéal premier $q'$ de B tel que $q' \subset q$ et $p' = \rho^{-1}(q')$, d’où $\rho(a) \subset q' \subset q$ et $q' \neq q$ contrairement à l’hypothèse faite sur q.

#### Proposition 2 {#ac-viii-s2-prop-2 .statement}

Soit $\rho : A \to B$ un homomorphisme d’anneaux non nuls possédant la propriété (PM). On a l’inégalité

(1)
$$
\dim(B) \geq \dim(A) + \inf_{m \in S} \dim(B/mB)
$$
où S est l’ensemble des idéaux maximaux de A.

On sait que l’on a $\dim(A) = \sup_{m \in S} \dim(A_m)$ (\S 1, no 3, prop. 8). Il suffit donc d’établir l’inégalité

(2)
$$
\dim(B) \geq \dim(A_m) + \dim(B/mB)
$$
pour tout idéal maximal m de A. Autrement dit, il s’agit de prouver l’inégalité

(3)
$$
\dim(B) \geq n + r
$$
si $p_0 \subset ... \subset p_n$ est une chaîne d’idéaux premiers de A contenus dans m et $\overline{q}_0 \subset ... \subset \overline{q}_r$ une chaîne d’idéaux premiers de B/mB. Pour $0 \leq i \leq r$, il existe un idéal premier $q_{n+i}$ de B au-dessus de m tel que $\overline{q}_i = q_{n+i}/mB$, et $q_n \subset ... \subset q_{n+r}$ est une chaîne d’idéaux premiers de B. Posons $p'_i = p_i$ pour $0 \leq i \leq n-1$ et $p'_n = m$, de sorte que $p'_0 \subset ... \subset p'_n$ est une chaîne d’idéaux premiers de A et que $q_n$ est au-dessus de $p'_n$. Si $q_i$ est un idéal premier de B au-dessus de $p'_i$ ($1 \leq i \leq n$), la prop. 1, c) prouve qu’il existe un idéal premier $q_{i-1}$ de B au-dessus de $p'_{i-1}$ et contenu dans $q_i$. Par récurrence descendante, on construit donc une chaîne $q_0 \subset ... \subset q_n$ d’idéaux premiers de B telle que $q_i$ soit au-dessus de $p_i$ pour $0 \leq i \leq n$. Comme $q_0 \subset ... \subset q_{n+r}$ est une chaîne d’idéaux premiers de B, on a prouvé l’inégalité (3).

#### Remarque 4 {#ac-viii-s2-n1-rem-4 .statement}

Soit $\rho : A \to B$ un homomorphisme local d’anneaux locaux noethériens satisfaisant à la condition (PM). On verra plus loin (\S 3, no 4, prop. 7) qu’on a dans ce cas égalité dans (1). Dans le cas général il peut y avoir inégalité stricte (p. 84, exercice 1).

#### Corollaire {#ac-viii-s2-n1-cor-2 .statement}

Pour tout idéal a de A, on a $\mathrm{ht}(a) \leq \mathrm{ht}(\rho(a)B)$.

Soient q un idéal premier de B contenant $\rho(a)B$, et $p = \rho^{-1}(q)$. D’après la prop. 1, l’homomorphisme local $\rho_q : A_p \to B_q$ déduit de $\rho$ satisfait à (PM), et l’on a donc $\dim(A_p) \leq \dim(B_q)$ d’après la prop. 2. D’après la prop. 7 du \S 7, no 3, on a $\mathrm{ht}(a) \leq \dim(A_p)$ puisque p contient a, d’où $\mathrm{ht}(a) \leq \dim(B_q)$ pour tout idéal premier q de B contenant $\rho(a)B$. Le corollaire résulte alors de loc. cit.

#### Lemme 1 {#ac-viii-s2-lem-1 .statement}

Soient $\rho : A \to B$ un homomorphisme d’anneaux et p un idéal premier de A. L’application continue $^a h : \mathrm{Spec}(B \otimes_A \kappa(p)) \to \mathrm{Spec}(B)$, associée à l’homomorphisme canonique $h : B \to B \otimes_A \kappa(p)$, *induit un homéomorphisme de* $\mathrm{Spec}(B \otimes_A \kappa(p))$ *sur le sous-espace* $(\alpha\rho)^{-1}(p)$ *de* $\mathrm{Spec}(B)$ *formé des idéaux premiers de* $B$ *au-dessus de* $p$.

L’homomorphisme $h$ est composé de l’homomorphisme de passage au quotient de $B$ dans $B/\rho(p)$ $B$ et de l’homomorphisme canonique de $B/\rho(p)$ $B$ dans son anneau de fractions $(\rho(A - p))^{-1}(B/\rho(p) \ B)$. D’après la remarque et le corollaire à la prop. 13 de II, § 4, no 3, $^a h$ induit donc un homéomorphisme de $\mathrm{Spec}(B \otimes_A \kappa(p))$ sur le sous-espace de $\mathrm{Spec}(B)$ formé des idéaux premiers $q$ de $B$ qui contiennent $\rho(p)$ et sont disjoints de $\rho(A - p)$, c’est-à-dire qui sont au-dessus de $p$.

#### Remarque 5 {#ac-viii-s2-n1-rem-5 .statement}

D’après la prop. 2 et le lemme 1, on a donc, sous les hypothèses de la prop. 2, l’inégalité
$$
\dim(\mathrm{Spec}(B)) \geq \dim(\mathrm{Spec}(A)) + \inf_{p \in \mathrm{Spec}(A)} \dim(\alpha\rho^{-1}(p)) .
$$

### 2. Dimension d’une algèbre de type fini

#### Proposition 3 {#ac-viii-s2-prop-3 .statement}

*Soit* $\rho : A \to B$ *un homomorphisme d’anneaux*. *Posons*
$n = \sup_{p \in \mathrm{Spec}(A)} \dim(B \otimes_A \kappa(p))$. *On a l’inégalité*
$$
\dim(B) + 1 \leq (\dim(A) + 1).(n + 1) .
$$

On peut supposer $\dim(A) \neq -\infty$ et $n < +\infty$. Soit $q_0 \subset ... \subset q_m$ une chaîne d’idéaux premiers de $B$; posons $p_i = \rho^{-1}(q_i)$. La suite des $p_i$ est croissante, donc l’ensemble de ses valeurs est de cardinal $\leq \dim(A) + 1$. Pour chaque $p \in \mathrm{Spec}(A)$, l’ensemble des $q_j$ tels que $p_j = p$ est une chaîne de la partie $^a\rho^{-1}(p)$ de $\mathrm{Spec}(B)$, donc est de cardinal inférieur à $\dim(B \otimes_A \kappa(p)) + 1$ (no 1, lemme 1), et par conséquent à $(n + 1)$. Il en résulte que $m + 1 \leq (\dim(A) + 1)(n + 1)$, d’où la proposition.

#### Remarque 1 {#ac-viii-s2-n2-rem-1 .statement}

Si les anneaux $A$ et $B$ sont noethériens, nous verrons ci-dessous (§ 3, no 4, cor. 2 à la prop. 7) qu’on a l’inégalité $\dim(B) \leq \dim(A) + n$, plus forte que celle de la prop. 3.

#### Corollaire 1 {#ac-viii-s2-prop-3-cor-1 .statement}

*Supposons qu’on ait* $\dim(A) < +\infty$ *et qu’il existe un entier* $n$ *tel que* $\dim(B \otimes_A \kappa(p)) \leq n$ *pour tout* $p \in \mathrm{Spec}(A)$. *Alors on a* $\dim(B) < +\infty$.

#### Corollaire 2 {#ac-viii-s2-prop-3-cor-2 .statement}

*Soient* $A$ *un anneau et* $B = A[X]$ *l’anneau des polynômes en une indéterminée à coefficients dans* $A$. *On a* :
$$
1 + \dim(A) \leq \dim(B) \leq 1 + 2\dim(A) .
$$

La première inégalité a déjà été démontrée (§ 1, no 3, exemple 4). Démontrons la seconde. Pour tout idéal premier $p$ de $A$, l’anneau $B \otimes_A \kappa(p)$, isomorphe à $\kappa(p)[X]$, est principal et n’est pas un corps, donc est de dimension 1 (§ 1, no 3, exemple 2), et l’inégalité résulte de la prop. 3.

Cependant, quels que soient les entiers n et q avec n + 1 ≤ q ≤ 2n + 1, il existe un anneau A de dimension n tel que dim(A[X]) = q (voir p. 84, exerc. 7).

#### Corollaire 3 {#ac-viii-s2-prop-3-cor-3 .statement}

Si A est de dimension finie, toute A-algèbre non nulle de type fini est de dimension finie.

On déduit en effet du cor. 2, par récurrence sur n, que l’anneau A[T₁, ..., Tₙ] est de dimension finie si A est de dimension finie ; a fortiori, tout quotient non nul de A[T₁, ..., Tₙ] est de dimension finie (§ 1, no 3, prop. 6).

### 3. Dimension d’une algèbre entière

#### Lemme 2 {#ac-viii-s2-lem-2 .statement}

Soit ρ : A → B un homomorphisme d’anneaux tel que, pour tout idéal premier p de A, la κ(p)-algèbre B ⊗ₓₐ κ(p) soit entière (V, § 1, no 1, déf. 2). Soient q et q’ deux idéaux premiers de B tels que q ⊂ q’ et q ≠ q’. Alors ρ⁻¹(q) ≠ ρ⁻¹(q’).

En effet, si q et q’ sont au-dessus d’un même idéal premier p de A, on a dim(B ⊗ₓₐ κ(p)) ≥ 1 d’après le lemme 1 du no 1, ce qui contredit le fait que dim(B ⊗ₓₐ κ(p)) ≤ 0 (§ 1, no 3, exemple 6).

#### Théorème 1 {#ac-viii-s2-thm-1 .statement}

Soit ρ : A → B un homomorphisme d’anneaux faisant de B une A-algèbre entière.

a) Soit M un A-module de type fini. Alors on a dim_B(M ⊗ₓₐ B) ≤ dim_A(M). En particulier, on a dim(B) ≤ dim(A). Si l’application “ρ : Spec(B) → Spec(A) est surjective, par exemple (V, § 2, no 1, th. 1) si ρ est injectif, on a dim_B(M ⊗ₓₐ B) = dim_A(M), et en particulier dim(B) = dim(A).

b) Soient b un idéal de B et a = ρ⁻¹(b) son image réciproque dans A. On a ht(b) ≤ ht(a) et dim(B/b) = dim(A/a). Si “ρ : Spec B → Spec A est surjective, on a ht(aB) ≤ ht(a) pour tout idéal a de A.

c) Supposons B finie sur A et soit N un B-module de type fini. Alors on a dim_B(N) = dim_A(N). En particulier, on a dim(B) = dim_A(B).

Démontrons a). D’après la prop. 5 de V, § 1, no 1, la κ(p)-algèbre B ⊗ₓₐ κ(p) est entière pour tout idéal premier p de A. Soit q₀ ⊂ ... ⊂ qₘ une chaîne d’idéaux premiers de B ; d’après le lemme 2, les idéaux pᵢ = ρ⁻¹(qᵢ) sont deux à deux distincts, donc p₀ ⊂ ... ⊂ pₘ est une chaîne d’idéaux premiers de A, d’où m ≤ dim(A). On a donc dim(B) ≤ dim(A).

Supposons maintenant que l’application “ρ soit surjective. Soit p₀ ⊂ ... ⊂ pₙ une chaîne d’idéaux premiers de A ; il existe donc un idéal premier q₀ de B au-dessus de p₀. D’après le cor. 2 au premier théorème d’existence (V, § 2, no 1, th. 1), on peut construire, par récurrence sur n, une chaîne q₀ ⊂ ... ⊂ qₙ d’idéaux premiers de B telle que qᵢ soit au-dessus de pᵢ pour 0 ≤ i ≤ n. On a donc n ≤ dim(B) et par suite dim(A) ≤ dim(B).

Cela démontre $a$ dans le cas où $M = A$. Dans le cas général, notons $a$ l’annulateur de $M$, de sorte que le support de $M$ s’identifie à $\operatorname{Spec}(A/a)$, et qu’on a $\dim_A(M) = \dim(A/a)$. D’après II, § 4, no 4, prop. 19, le support de $M \otimes_A B$ est l’image réciproque par $^a\rho$ du support de $M$, donc s’identifie à $\operatorname{Spec}(B/\rho(a) B)$, et on a $\dim_B(M \otimes_A B) = \dim(B/\rho(a) B)$. Il reste à remarquer que l’homomorphisme $\rho': A/a \to B/\rho(a) B$ déduit de $\rho$ fait de $B/\rho(a) B$ une $(A/a)$-algèbre entière, et que “$\rho'$ est surjectif lorsque $^a\rho$ l’est.

Démontrons $b$. D’après la prop. 7 du § 1, no 3, il suffit de prouver que $\operatorname{ht}(b) \leq \dim(A_p)$ pour tout idéal premier $p$ de $A$ contenant $a$; soit $p$ un tel idéal. D’après V, § 2, no 1, cor. 2 au th. 1, il existe un idéal premier $q$ de $B$ au-dessus de $p$ et contenant $b$, et on a $\operatorname{ht}(b) \leq \dim(B_q)$ d’après la prop. 7 du § 1, no 3.

Or $B_q$ s’identifie à un anneau de fractions de la $A_p$-algèbre entière $B \otimes_A A_p$, d’où
$$
\dim(B_q) \leq \dim(B \otimes_A A_p) \leq \dim(A_p)
$$
d’après la prop. 6 du § 1, no 3 et l’assertion $a$ ci-dessus. On a ainsi prouvé l’inégalité $\operatorname{ht}(b) \leq \operatorname{ht}(a)$. Par ailleurs, l’homomorphisme de $A/a$ dans $B/b$ déduit de $\rho$ est injectif et fait de $B/b$ une $(A/a)$-algèbre entière; on a donc $\dim(B/b) = \dim(A/a)$ d’après $a$. Supposons “$\rho$ surjective et soient $a$ un idéal de $A$ et $p$ un idéal premier de $A$ contenant $a$. Il existe par hypothèse un idéal premier $q$ de $B$ au-dessus de $p$. On a $aB \subset q$, d’où $\operatorname{ht}(aB) \leq \operatorname{ht}(q) \leq \operatorname{ht}(p)$ d’après ce qui précède. Passant à la borne inférieure, on obtient $\operatorname{ht}(aB) \leq \operatorname{ht}(a)$.

Enfin, $c$ résulte de $b$ appliqué à l’annulateur $b$ de $N$.

#### Théorème 2 {#ac-viii-s2-thm-2 .statement}

Soient $A$ un anneau intégralement clos, et $B$ un anneau contenant $A$, entier sur $A$. On suppose que $B$ est un $A$-module sans torsion. Pour tout idéal $a$ de $A$, on a $\operatorname{ht}(a) = \operatorname{ht}(aB)$. Soient $b$ un idéal de $B$ et $a = b \cap A$; on a alors $\operatorname{ht}(a) = \operatorname{ht}(b)$.

Soit $\rho$ l’application canonique de $A$ dans $B$. Soient $a$ un idéal de $A$. Si $a = A$, la première égalité est claire. Supposons $a \neq A$. Comme $\rho$ est injectif, $^a\rho$ est surjectif (V, § 2, no 1, th. 1). Par suite $aB \neq B$. Soit alors $q$ un idéal premier de $B$ contenant $aB$. Posons $p = q \cap A$. On a $a \subset p$, d’où $\operatorname{ht}(a) \leq \operatorname{ht}(p)$. Soit $p_0 \subset ... \subset p_n$ une chaîne d’idéaux premiers de $A$ avec $p_n = p$. D’après le deuxième théorème d’existence (V, § 2, no 4, th. 3), on construit par récurrence une chaîne $q_0 \subset ... \subset q_n$ d’idéaux premiers de $B$ telle que $q_n = q$ et $q_i$ soit au-dessus de $p_i$ pour $0 \leq i \leq n$. On a $n \leq \operatorname{ht}(q)$, d’où $\operatorname{ht}(a) \leq \operatorname{ht}(q)$. En passant à la borne inférieure on obtient $\operatorname{ht}(a) \leq \operatorname{ht}(aB)$ ($§ 1$, no 3, prop. 7). L’inégalité $\operatorname{ht}(aB) \leq \operatorname{ht}(a)$ résulte du th. 1, d’où la première égalité. Soit $b$ un idéal de $B$. Posons $a = \rho^{-1}(b)$. On a $aB \subset b$, d’où $\operatorname{ht}(a) = \operatorname{ht}(aB) \leq \operatorname{ht}(b)$. L’inégalité $\operatorname{ht}(b) \leq \operatorname{ht}(a)$ résulte du th. 1, d’où le théorème.

#### Remarque {#ac-viii-s2-n3-rem-1 .statement}

Soient $A$ un anneau intègre et $B$ un anneau contenant $A$, entier sur $A$. Soit $p$ un idéal premier de $A$ tel que la clôture intégrale de $A_p$ soit un anneau local. On peut démontrer que, pour tout idéal premier $q$ de $B$ au-dessus de $p$, on a $\operatorname{ht}(p) = \operatorname{ht}(q)$ (p. 85, exerc. 9) lorsque $B$ est intègre.

### 4. Algèbres de type fini sur un corps

Dans ce numéro, $k$ désigne un corps.

#### Lemme 3 {#ac-viii-s2-lem-3 .statement}

Soient $A$ une $k$-algèbre de type fini et $p_0 \subset ... \subset p_m$ une chaîne maximale d’idéaux premiers de $A$. Il existe un entier $n \geq m$, une suite $(x_1, ..., x_n)$ d’éléments de $A$, algébriquement libre sur $k$ (A, IV, p. 4), et telle que :
a) $A$ soit entier sur l’anneau $B = k[x_1, ..., x_n]$;
b) pour tout $j$ tel que $0 \leq j \leq m$, l’idéal $p_j \cap B$ soit engendré par les $x_k$ avec $1 \leq k \leq n - m + j$.

D’après le lemme de normalisation (V, § 3, no 1, th. 1), il existe un entier $n \geq 0$, une suite finie $(x_1, ..., x_n)$ d’éléments de $A$ algébriquement libre et une suite croissante $(h(j))_{0 \leq j \leq m}$ d’entiers $\leq n$ telle que l’idéal $p_j \cap B$ soit égal à l’idéal premier $q_j$ de $B$ engendré par les $x_k$ avec $1 \leq k \leq h(j)$, et que $A$ soit entier sur l’anneau $B$. Soit $j$ un entier tel que $0 \leq j < m$. Par passage aux quotients, on déduit de l’injection canonique de $B$ dans $A$ un homomorphisme injectif de $B/q_j$ dans $A/p_j$ qui fait de $A/p_j$ une $(B/q_j)$-algèbre finie. Comme l’anneau $B/q_j$ est isomorphe à une algèbre de polynômes en $n - h(j)$ indéterminées sur $k$, il est intégralement clos (V, § 1, no 3, cor. 3 de la prop. 13). D’après le th. 2 du no 3, on a donc

$$
1 = \mathrm{ht}(p_{j+1}/p_j) = \mathrm{ht}(q_{j+1}/q_j) \geq h(j+1) - h(j) .
$$

Il en résulte que l’on a $h(j+1) \leq h(j) + 1$ et $q_{j+1} \neq q_j$, d’où $h(j+1) = h(j) + 1$. Mais on a $h(m) = n$ puisque $q_m$ est maximal (V, § 2, no 1, prop. 1), d’où finalement $h(j) = n - m + j$.

#### Théorème 3 {#ac-viii-s2-thm-3 .statement}

Soit $A$ une $k$-algèbre de type fini.
a) Pour tout idéal premier minimal $p$ de $A$, toutes les chaînes maximales d’idéaux premiers de $A$ d’origine $p$ ont pour longueur l’entier $\deg.\mathrm{tr}_k \kappa(p)$.
b) L’anneau $A$ est caténaire et sa dimension est la borne supérieure des entiers $\deg.\mathrm{tr}_k \kappa(p)$, où $p$ parcourt les idéaux premiers minimaux de $A$.
c) Si $A$ est intègre, alors toutes les chaînes maximales d’idéaux premiers de $A$ ont la même longueur, et la dimension de $A$ est le degré de transcendance sur $k$ du corps des fractions de $A$.

Supposons $A$ intègre et considérons une chaîne maximale $p_0 \subset ... \subset p_m$ d’idéaux premiers de $A$. On a $p_0 = 0$. On déduit alors du lemme 3 l’existence d’un homomorphisme injectif $\varphi : k[X_1, ..., X_m] \to A$ de $k$-algèbres qui fait de $A$ une $k[X_1, ..., X_m]$-algèbre finie. Par suite, le degré de transcendance sur $k$ du corps des fractions de $A$ est égal à $m$, d’où c). L’assertion a) résulte de l’assertion c) appliquée à l’anneau $A/p$ et l’assertion b) est une conséquence immédiate de a) et de la prop. 5 du § 1, no 2.

#### Corollaire 1 {#ac-viii-s2-thm-3-cor-1 .statement}

Soit $n$ un entier positif. On a

$$
\dim(k[X_1, ..., X_n]) = n .
$$

Pour qu’une k-algèbre A de type fini soit de dimension n, il faut et il suffit qu’il existe un k-homomorphisme injectif $\varphi : k[X_1, ..., X_n] \to A$ faisant de A une algèbre finie sur $k[X_1, ..., X_n]$.

Cela résulte du th. 3, du lemme de normalisation (V, § 3, no 1, th. 1) et du th. 1, a) du no 3.

#### Corollaire 2 {#ac-viii-s2-thm-3-cor-2 .statement}

Soit A une k-algèbre intègre de type fini. Pour tout idéal premier p de A, on a

$$
\operatorname{ht}(p) = \dim(A_p) = \dim(A) - \dim(A/p)
$$
$$
= \dim(A) - \deg.\operatorname{tr}_k\kappa(p).
$$

En particulier, on a $\operatorname{ht}(m) = \dim(A_m) = \dim(A)$ pour tout idéal maximal m de A.

Cela résulte du th. 3 et de la remarque 4 du § 1, no 3.

#### Corollaire 3 {#ac-viii-s2-thm-3-cor-3 .statement}

Soit A une k-algèbre de type fini et soit f un élément de A qui n’appartienne à aucun idéal premier minimal de A (par exemple un élément de A non diviseur de zéro, cf. IV, § 1, no 1, cor. 3 à la prop. 2 et no 3, cor. 1 à la prop. 7). On a $\dim(A) = \dim(A_f)$.

L’application $p \mapsto pA_f$ est une bijection de l’ensemble des idéaux premiers minimaux de A sur l’ensemble des idéaux premiers minimaux de $A_f$. Par ailleurs les anneaux $A/p$ et $A_f/pA_f = (A/p)_f$ ont même corps des fractions. Il suffit donc d’appliquer le th. 3, b).

#### Corollaire 4 {#ac-viii-s2-thm-3-cor-4 .statement}

Soient A une k-algèbre de type fini et p un idéal premier de A.

a) Pour que p soit maximal, il faut et il suffit que le corps des fractions de $A/p$ soit une extension finie de k.

b) Soit $f \in A - p$; l’idéal p est un idéal maximal de A si et seulement si $pA_f$ est un idéal maximal de $A_f$.

Si p est un idéal maximal de A, alors $A/p$ est un corps, donc un anneau de dimension 0 ; c’est une extension de type fini de k dont le degré de transcendance est 0 (th. 3, c)), c’est donc une extension finie de k. Réciproquement, si le corps des fractions de $A/p$ est une extension finie de k, on a $\dim(A/p) = 0$ donc p est maximal. L’assertion b) résulte de l’assertion a) compte tenu que $A/p$ et $A_f/pA_f$ ont même corps des fractions.

L’assertion a) du cor. 4 est une forme du théorème des zéros (V, § 3, no 3, prop. 1).

#### Corollaire 5 {#ac-viii-s2-thm-3-cor-5 .statement}

Soient A une k-algèbre de type fini, p un idéal premier de A et $(\mathfrak{p}_i)_{i \in I}$ la famille des idéaux premiers minimaux de A contenus dans p. On a :

$$
\dim_p(A) = \sup_{i \in I} \dim(A/\mathfrak{p}_i)
$$
$$
= \dim(A_p) + \dim(A/p)
$$
$$
= \dim(A_p) + \deg.\operatorname{tr}_k\kappa(p).
$$

On a $\dim_p(A) = \sup_{i \in I} \dim_{p/p_i}(A/p_i)$ (\S 1, n° 3, prop. 6). Mais, d’après le cor. 3, on a $\dim_{p/p_i}(A/p_i) = \dim(A/p_i)$, d’où la première égalité. D’après le cor. 2, on a $\dim(A/p_i) = \dim((A/p_i)_p) + \dim(A/p)$. La deuxième égalité du corollaire résulte donc du fait que $\dim(A_p) = \sup_{i \in I} \dim((A/p_i)_p)$ et la troisième du th. 3.

Ainsi $\dim_p(A)$ est la borne supérieure des longueurs des chaînes d’idéaux premiers de $A$ dont $p$ est un élément.

#### Corollaire 6 {#ac-viii-s2-thm-3-cor-6 .statement}

*Soit A une k-algèbre de type fini non réduite à 0, et soit n un entier $\geqslant 0$. Les conditions suivantes sont équivalentes :*

a) *Pour tout $p \in \operatorname{Ass}(A)$, on a $\dim(A/p) = n$.*

b) *Tout idéal premier associé à A est minimal et toutes les composantes irréductibles de Spec(A) sont de dimension n.*

c) *Il existe un k-homomorphisme injectif $\varphi : k[X_1, ..., X_n] \to A$ faisant de A un $k[X_1, ..., X_n]$-module de type fini sans torsion.*

L’équivalence de a) et b) est immédiate. Montrons que a) implique c). D’après b), l’anneau A est dimension n et il existe donc (cor. 1) un k-homomorphisme injectif $\varphi : k[X_1, ..., X_n] \to A$ faisant de A un $k[X_1, ..., X_n]$-module de type fini. Pour tout idéal premier $p \in \operatorname{Ass}(A)$, l’anneau $A/p$ est alors entier sur $k[X_1, ..., X_n]$, et on a donc $n = \dim(A/p) = \dim(k[X_1, ..., X_n]/\varphi^{-1}(p))$ d’après le th. 1, a) du n° 3, d’où $\varphi^{-1}(p) = 0$. L’image par l’homomorphisme injectif $\varphi$ d’un élément non nul de $k[X_1, ..., X_n]$ n’est pas un diviseur de 0 dans A (IV, § 1, n° 1, cor. 3 à la prop. 2), d’où c).

Inversement, supposons la condition c) satisfaite. Pour tout idéal premier $p \in \operatorname{Ass}(A)$, l’homomorphisme $k[X_1, ..., X_n] \to A/p$ déduit de $\varphi$ est injectif (*loc. cit.*). On a donc $\dim(A/p) = n$ d’après le cor. 1.

#### Remarque 1 {#ac-viii-s2-n4-rem-1 .statement}

D’après le cor. 5, les conditions a), b), c) du cor. 6 impliquent qu’on a $\dim_p(A) = \dim(A)$ pour tout idéal premier $p$ de A.

#### Proposition 4 {#ac-viii-s2-prop-4 .statement}

*Soient A et B deux k-algèbres de type fini et $\rho : A \to B$ un homomorphisme d’algèbres. Supposons que A soit intègre et que le A-module B soit sans torsion, et notons K le corps des fractions de A. On a*

$$
\dim(B) = \dim(A) + \dim(B \otimes_A K).
$$

Supposons d’abord B intègre. L’algèbre $B \otimes_A K$ est alors un anneau de fractions de B défini par une partie multiplicative ne contenant pas 0. Elle a donc pour corps des fractions le corps des fractions L de B. D’après le th. 3, on a

$$
\dim(B) = \deg.\mathrm{tr}_k L,\quad \dim(A) = \deg.\mathrm{tr}_k K,
$$
$$
\dim(B \otimes_A K) = \deg.\mathrm{tr}_K L.
$$

Or on a, d’après le corollaire de A, V, p. 106

$$
\deg.\mathrm{tr}_k L = \deg.\mathrm{tr}_K L + \deg.\mathrm{tr}_k K,
$$

d’où le résultat dans ce cas.

Passons au cas général. Tout idéal premier minimal $p$ de $B$ est formé de diviseurs de zéro dans $B$, donc est au-dessus de l’idéal 0 de $A$. Il en résulte que l’application $p \mapsto p . (B \otimes_A K)$ est une bijection de l’ensemble des idéaux premiers minimaux de $B$ sur l’ensemble des idéaux premiers minimaux de $B \otimes_A K$. La proposition résulte donc de la première partie de la démonstration et de la prop. 6, c) du § 1, no 3.

#### Corollaire {#ac-viii-s2-n4-cor-1 .statement}

*Soit $\rho : A \to B$ un homomorphisme injectif de k-algèbres de type fini.* *On a* $\dim(A) \leq \dim(B)$.

En effet, soit $p$ un idéal premier minimal de $A$ tel que $\dim(A) = \dim(A/p)$. Il existe un idéal premier $q$ de $B$ au-dessus de $p$ (II, § 2, no 6, prop. 16). D’après la prop. 4 appliquée à $A/p$ et $B/q$, on a $\dim(A) = \dim(A/p) \leq \dim(B/q) \leq \dim(B)$, d’où le corollaire.

*Lemme 4. — Soient $A$ et $B$ deux k-algèbres intègres, $M$ un $A$-module sans torsion, $N$ un $B$-module sans torsion. Si l’anneau $A \otimes_k B$ est intègre, alors $M \otimes_k N$ est un module sans torsion sur $A \otimes_k B$.

Soit $K$ (resp. $L$) le corps des fractions de $A$ (resp. $B$). Il existe un ensemble $I$ (resp. $J$) tel que $M$ (resp. $N$) soit isomorphe à un sous-module de $K^{(I)}$ (resp. $L^{(J)}$). Le $(A \otimes_k B)$-module $M \otimes_k N$ est alors isomorphe à un sous-module de $K^{(I)} \otimes_k L^{(J)}$, qui est isomorphe à $(K \otimes_k L)^{(I \times J)}$. Comme $K \otimes_k L$ est un anneau de fractions de l’anneau intègre $A \otimes_k B$, c’est un module sans torsion sur $A \otimes_k B$, d’où le lemme.

*PROPOSITION 5. — Soient $k'$ une extension de $k$, $A$ une k-algèbre de type fini et $B$ une $k'$-algèbre de type fini.

a) *La $k'$-algèbre $A \otimes_k B$ est de type fini et on a*
$$
\dim(A \otimes_k B) = \dim(A) + \dim(B).
$$

b) *Soit $r$ un idéal premier de $A \otimes_k B$; notons $p$ (resp. $q$) l’image réciproque de $r$ dans $A$ (resp. $B$). On a*
$$
\dim_r(A \otimes_k B) = \dim_p(A) + \dim_q(B).
$$

Posons $n = \dim(A)$ et $m = \dim(B)$. Il existe d’après le cor. 1 au th. 3 des homomorphismes injectifs d’algèbres $\varphi : k[X_1, ..., X_n] \to A$ et $\psi : k'[Y_1, ..., Y_m] \to B$ faisant respectivement de $A$ et $B$ des algèbres finies sur $k[X_1, ..., X_n]$ et $k'[Y_1, ..., Y_m]$. L’homomorphisme $\varphi \otimes \psi$ est alors injectif et fait de $A \otimes_k B$ une algèbre finie sur la $k'$-algèbre $k[X_1, ..., X_n] \otimes_k k'[Y_1, ..., Y_m]$ qui s’identifie à $k'[X_1, ..., X_n, Y_1, ..., Y_m]$. On a donc $\dim(A \otimes_k B) = n + m$ d’après le cor. 1 au th. 3, ce qui prouve a).

Remarquons que lorsque $A$ et $B$ sont intègres, $A \otimes_k B$ est un $k'[X_1, ..., X_n, Y_1, ..., Y_m]$-module sans torsion d’après le lemme 4 et qu’on a donc
$$
\dim_r(A \otimes_k B) = n + m = \dim(A) + \dim(B)
$$
pour tout idéal premier $r$ de $A \otimes_k B$ d’après la remarque 1.

Prouvons maintenant b). Soit $r_0$ un idéal premier minimal de $A \otimes_k B$ contenu dans $r$, et notons $p_0$ (resp. $q_0$) l’image réciproque de $r_0$ dans $A$ (resp. $B$). L’anneau

(A \otimes_k B)/r_0 est isomorphe à un quotient de l’anneau (A/p_0) \otimes_k (B/q_0). On a donc, d’après $a$,

$$
\dim((A \otimes_k B)/r_0) \leq \dim(A/p_0) + \dim(B/q_0).
$$

Appliquant le cor. 5 au th. 3, on en déduit l’inégalité

$$
\dim_r(A \otimes_k B) \leq \dim_p(A) + \dim_q(B).
$$

Inversement, soit $p_0$ (resp. $q_0$) un idéal premier minimal de A (resp. B) contenu dans $p$ (resp. q). D’après la remarque faite ci-dessus, on a

$$
\dim(A/p_0) + \dim(B/q_0) = \dim_{\overline{r}}((A/p_0) \otimes_k (B/q_0))
$$

où $\overline{r}$ est l’image de r par la surjection canonique $A \otimes_k B \to (A/p_0) \otimes_k (B/q_0)$. Le second membre de l’égalité précédente est évidemment inférieur à $\dim_r(A \otimes_k B)$. Appliquant le cor. 5 au th. 3, on en déduit l’inégalité

$$
\dim_p(A) + \dim_q(B) \leq \dim_r(A \otimes_k B),
$$

ce qui achève la démonstration.

#### Corollaire {#ac-viii-s2-n4-cor-2 .statement}

*Soient A une k-algèbre de type fini, k' une extension de k, et A' la k'-algèbre A \otimes_k k'.*

a) *On a* $\dim(A') = \dim(A)$.

b) *Soient p' un idéal premier de A' et p son image réciproque dans A ; on a* $\dim_{p'}(A') = \dim_p(A)$.

c) *Soient p' un idéal premier minimal de A' et p son image réciproque dans A. Alors p est minimal et l’on a* $\dim(A'/p') = \dim(A/p)$.

Les assertions a) et b) se déduisent de la prop. 5 en y prenant $B = k'$. Démontrons c). L’idéal p est minimal (n° 1, prop. 1) et l’on a

$$
\dim(A'/p') = \dim_{p'}(A') = \dim_p(A) = \dim(A/p).
$$

#### Remarque 2 {#ac-viii-s2-n4-rem-2 .statement}

*Supposons l’extension k' de k radicielle. Alors l’application canonique $f : \mathrm{Spec}(A') \to \mathrm{Spec}(A)$ est un homéomorphisme.*

Soit en effet $p \in \mathrm{Spec}(A)$. D’après le lemme 1 du n° 1, l’espace $f^{-1}(\{p\})$ est homéomorphe à $\mathrm{Spec}(\kappa(p) \otimes_k k')$. Or l’ensemble a des éléments nilpotents de $\kappa(p) \otimes_k k'$ est un idéal premier (A, V, p. 134, corollaire) et l’anneau quotient $(\kappa(p) \otimes_k k')/a$, intègre et entier sur $\kappa(p)$, est un corps (A, V, p. 16, cor. 1 et p. 10, prop. 1). Par conséquent $f^{-1}(\{p\})$ est réduit à un élément. Il en résulte que l’application $f$ est une bijection croissante de $\mathrm{Spec}(A')$ sur $\mathrm{Spec}(A)$, ces deux ensembles étant ordonnés par l’inclusion des idéaux premiers, donc induit une bijection entre les parties fermées irréductibles de $\mathrm{Spec}(A)$ sur celles de $\mathrm{Spec}(A')$. Comme les parties fermées de $\mathrm{Spec}(A)$ (resp. $\mathrm{Spec}(A')$) sont les réunions finies de parties fermées irréductibles, $f$ est un homéomorphisme.

Pour une généralisation, voir l’exerc. 24, p. 98.

## EXERCICES {#ac-viii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
