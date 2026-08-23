---
book: ac
book_title: Commutative Algebra
chapter: VIII
chapter_title: DIMENSION
section: 7
section_title: Multiplicités
lang: fr
source: ac-viii-ix-fr
book_pages: AC VIII.71-AC VIII.81, AC VIII.103-AC VIII.108
pdf_pages: 0075-0085, 0107-0112
extraction: ocr
subsections:
    - "no": 1
      title: Multiplicité d’un module relativement à un idéal
      page: 71
      pdf_page: 75
    - "no": 2
      title: Multiplicités et extensions plates
      page: 0
      pdf_page: 77
    - "no": 3
      title: Multiplicités et extensions finies
      page: 74
      pdf_page: 78
    - "no": 4
      title: Multiplicités et suites sécantes
      page: 76
      pdf_page: 80
    - "no": 5
      title: Éléments superficiels
      page: 0
      pdf_page: 81
statements: 28
exercises: 25
content_sha256: 4794bf4ee4b6265162c8cc3eb9ffeac0c403b80501305d4b3cde8113dd388e6d
---

## § 7. MULTIPLICITÉS

Dans tout ce paragraphe, on note $ A $ un anneau noethérien.

### 1. Multiplicité d’un module relativement à un idéal

Soient $ M $ un $ A $-module de type fini et $ q $ un idéal de $ A $ contenu dans le radical de $ A $ et tel que $ M/qM $ soit de longueur finie. Supposons $ M $ non réduit à 0 et posons $ d = \dim_A(M) $. D’après § 4, no 3, corollaire du th. 2 et no 4, remarque 2, il existe un unique entier $ e_q(M) > 0 $ tel que l’on ait, pour tout entier $ n \geqslant 1 $

$$
\operatorname{long}_A(M/q^{n+1}M) = e_q(M) \frac{n^d}{d!} + \beta_n n^{d-1}
$$

où $ \beta_n $ tend vers une limite lorsque $ n $ augmente indéfiniment.

#### Définition 1 {#ac-viii-s7-def-1 .statement}

L’entier $ e_q(M) $ s’appelle la multiplicité du A-module M relativement à l’idéal q.

On le note aussi $ e_q^A(M) $ lorsque l’on désire mentionner l’anneau A. Lorsque A est local d’idéal maximal m, on écrit $ e(M) $ ou $ e^A(M) $ pour $ e_m(M) $ ou $ e_m^A(M) $.

#### Remarque 1 {#ac-viii-s7-n1-rem-1 .statement}

Si q’ est un idéal de A contenu dans le radical de A et contenant q, on a $ e_{q'}(M) \leqslant e_q(M) $ et, si la filtration q’-adique de M est q-bonne, on a $ e_{q'}(M) = e_q(M) $ (§ 4, no 3, th. 2).
2) Si M est de longueur finie, on a $ e_q(M) = \operatorname{long}_A(M) $ (§ 4, no 3, remarque 3).
3) Si $ d > 0 $, on a

$$
\operatorname{long}_{A/q}(q^nM/q^{n+1}M) = e_q(M) \frac{n^{d-1}}{(d-1)!} + \alpha_n n^{d-2}
$$

où $ \alpha_n $ tend vers une limite lorsque $ n $ augmente indéfiniment (§ 4, no 3, corollaire au th. 2).
4) On peut ramener le calcul des multiplicités au cas où A est local puisque, d’après § 4, no 4, corollaire au th. 3, on a

$$
e_q(M) = \sum e_{q_m}(M_m)
$$

la sommation étant étendue aux idéaux maximaux m de A tels que

$$
m \in \operatorname{Supp}(M) \cap V(q) \quad \text{et} \quad \dim_{A_m}(M_m) = d .
$$

Il résulte des remarques 2 et 3 que $ e_q(M) $ ne dépend que du A/q-module gradué $ \operatorname{gr}_q(M) $. Par conséquent :

#### Proposition 1 {#ac-viii-s7-prop-1 .statement}

Soient $ \hat{A} $ et $ \hat{M} $ les complétés de A et M pour leurs topologies q-adiques ; alors $ e_q^A(M) = e_{q\hat{A}}(\hat{M}) $.

#### Proposition 2 {#ac-viii-s7-prop-2 .statement}

Supposons A local régulier (§ 5, no 1, déf. 1) ; on a $ e(A) = 1 $.
Cela résulte du th. 1 du § 5, no 2.

#### Remarque 5 {#ac-viii-s7-n1-rem-5 .statement}

On peut avoir $ e(A) = 1 $ sans que A soit régulier (p. 104, exerc. 5). En fait, un anneau local noethérien A est régulier si et seulement si $ \hat{A} $ est intègre et si l’on a $ e(A) = 1 $ (p. 108, exerc. 24).

#### Exemple {#ac-viii-s7-n1-exa-1 .statement}

On a par définition $ e_{q,r}(M) = r^d e_q(M) $ où $ d = \dim_A(M) $. Par conséquent, si A est local régulier, on a $ e_{m_A^r}(A) = r^d $. Par exemple, si A est un anneau de valuation discrète, on a $ e_q(A) = \operatorname{long}(A/q) $.

#### Proposition 3 {#ac-viii-s7-prop-3 .statement}

*Soit M un A-module de type fini, de dimension d ≥ 0. Soit Φ l’ensemble des éléments minimaux p de Supp(M) tels que dim(A/p) = d. Soit q un idéal de A, contenu dans le radical de A, et tel que M/qM soit de longueur finie. On a*

$$
e_q(M) = \sum_{p \in \Phi} \operatorname{long}_{A_p}(M_p).e_q(A/p).
$$

#### Corollaire {#ac-viii-s7-n1-cor-1 .statement}

*Supposons A semi-local et soit q un idéal de définition de A.
a) On a $ e_q(A) = \sum_p e_q(A/p) $, où p parcourt l’ensemble des idéaux premiers minimaux de A tels que $ \dim(A/p) = \dim(A) $.
b) Supposons A intègre et soit M un A-module de type fini tel que $ \dim_A(M) = \dim(A) $. Alors on a $ e_q(M) = \operatorname{rg}(M).e_q(A) $.*

### 2. Multiplicités et extensions plates

#### Proposition 4 {#ac-viii-s7-prop-4 .statement}

*Soit ρ : A → B un homomorphisme local d’anneaux locaux noethériens, et soit N un B-module de type fini, plat sur A, et tel que N ⊗_A κ_A soit un B-module de longueur finie. Si M est un A-module de type fini non nul et q un idéal de A distinct de A et tel que M/qM soit de longueur finie, alors (M ⊗_A N)/(qB)(M ⊗_A N) est un B-module de longueur finie, et l’on a*

$$
e_{q_B}^B(M ⊗_A N) = \operatorname{long}_B(N ⊗_A κ_A).e_q^A(M).
$$

Soit L un A-module de longueur finie r. Alors L possède une suite de Jordan-Hölder de longueur r, à quotients isomorphes à κ_A ; comme N est plat sur A, le B-module L ⊗_A N possède une suite de composition de longueur r, à quotients isomorphes à N ⊗_A κ_A, donc est de longueur r · long_B(N ⊗_A κ_A). Comme le B-module (M ⊗_A N)/(qB)^n(M ⊗_A N) est isomorphe à (M/q^nM) ⊗_A N pour tout n ∈ ℕ, la proposition résulte de la définition des multiplicités.

#### Corollaire {#ac-viii-s7-n2-cor-1 .statement}

*On suppose que B est plat sur A et que ρ(m_A) B = m_B. Alors*

$$
e_{q_B}^B(M ⊗_A B) = e_q^A(M).
$$

Cela s’applique notamment lorsque B est le complété \* ou l’hensélisé \* de A relativement à un idéal distinct de A, \* ou un gonflement de A, par exemple un hensélisé strict de A. \*

#### Exemple {#ac-viii-s7-n2-exa-1 .statement}

\* Soient X une variété algébrique complexe, $ \mathcal{O}_{X,x} $ l’anneau local de X en un point rationnel x, $ X^{an} $ l’espace analytique associé à X ; notons encore x le point de $ X^{an} $ correspondant à x, et soit $ \mathcal{O}_{X^{an},x} $ l’anneau local de $ X^{an} $ en x. Alors $ e(\mathcal{O}_{X^{an},x}) = e(\mathcal{O}_{X,x}) $. \*

### 3. Multiplicités et extensions finies

#### Proposition 5 {#ac-viii-s7-prop-5 .statement}

Supposons A semi-local et soit $ \rho : A \to B $ un homomorphisme d’anneaux faisant de B un A-module de type fini. Soit N un B-module non nul de type fini et soit q un idéal de A contenu dans le radical de A, et tel que $ N/qN $ soit de longueur finie. Parmi les idéaux maximaux de B (en nombre fini, d’après IV, § 2, no 5, cor. 3 à la prop. 9), notons $ m_1, ..., m_r $ ceux pour lesquels on a $ \dim_{B_{m_i}}(N_{m_i}) = \dim_B(N) $. Posons $ B_i = B_{m_i} $ et $ q_i = qB_i $ pour $ 1 \leq i \leq r $. Alors on a les égalités

$$
\dim_A(N) = \dim_B(N),
$$
$$
e_{qB}^B(N) = \sum_{i=1}^r e_{q_i}^{B_i}(N_{m_i}),
$$
$$
e_q^A(N) = \sum_{i=1}^r [B/m_i : A/\rho^{-1}(m_i)]\ e_{q_i}^{B_i}(N_{m_i}).
$$

La première égalité résulte de § 2, no 3, th. 1, c); la seconde résulte de la remarque 4 du no 1 (noter que $ m_i $ appartient à $ V(qB) $ pour $ 1 \leq i \leq r $ puisque $ \rho^{-1}(m_i) \supset q $ d’après V, § 2, no 1, prop. 1). Démontrons la troisième égalité. Soit E un B-module de longueur finie; on a

$$
\operatorname{long}_A(E) = \sum_m [B/m : A/\rho^{-1}(m)].\operatorname{long}_{B_m}(E_m),
$$

$ m $ parcourant l’ensemble des idéaux maximaux de B ; c’est en effet évident lorsque E est l’un des $ B/m $, et le cas général s’en déduit, puisque E possède une suite de composition dont les quotients sont isomorphes à des $ B/m $. Appliquant cette formule aux B-modules $ N/q^{n+1}N $, on en déduit l’égalité cherchée par définition des multiplicités.

#### Corollaire {#ac-viii-s7-n3-cor-1 .statement}

Si $ [B/m_i : A/\rho^{-1}(m_i)] = 1 $ pour tout i, on a $ e_q^A(N) = e_{qB}^B(N) $.

#### Lemme 1 {#ac-viii-s7-lem-1 .statement}

Soit $ \rho : A \to B $ un homomorphisme d’anneaux, et soit $ p $ un idéal premier de A. Considérons les deux propriétés suivantes :
(i) l’homomorphisme canonique $ \tilde{\rho} $ de $ A_p $ dans $ A_p \otimes_A B $ est bijectif;
(ii) il existe un seul idéal premier $ r $ de B au-dessus de $ p $ et l’homomorphisme canonique $ \rho_p $ de $ A_p $ dans $ B_r $ est bijectif.
On a (i) $ \Rightarrow $ (ii). Si $ p $ est minimal, ou bien si B est entier sur A, on a (i) $ \Leftrightarrow $ (ii) $ ^1 $.

1 Ce lemme reste valable lorsque l’anneau A n’est pas noethérien.

L’anneau $ A_p \otimes_A B $ s’identifie à l’anneau de fractions $ S^{-1}B $ de $ B $ défini par la partie multiplicative $ S = \rho(A - p) $ de $ B $. Les idéaux premiers de $ S^{-1}B $ sont donc les $ S^{-1}q $, où $ q $ est un idéal premier de $ B $ tel que $ \rho^{-1}(q) \subset p $; si $ q $ est un tel idéal, $ (S^{-1}B)_{S^{-1}q} $ s’identifie à $ B_q $ (II, § 2, no 5, prop. 11).

Si la condition (i) est satisfaite, il existe (V, § 2, no 1, lemme 1) un unique idéal premier $ r $ de $ B $ tel que $ \rho^{-1}(r) = p $. De plus, $ B_r $ s’identifie à l’anneau de fractions $ (S^{-1}B)_{S^{-1}r} $, donc aussi à $ (A_p)_s $, où $ s $ est l’image réciproque de $ S^{-1}r $ par l’isomorphisme $ \tilde{\rho}: A_p \to S^{-1}B $; or $ \tilde{\rho}^{-1}(S^{-1}r) = (A - p)^{-1}p = pA_p $, d’où (ii).

Inversement, supposons (ii) satisfaite, et soit $ r $ l’unique idéal premier de $ B $ au-dessus de $ p $. Puisque $ (S^{-1}B)_{S^{-1}r} $ s’identifie à $ B_r $, il suffit de prouver que $ S^{-1}B $ est local d’idéal maximal $ S^{-1}r $, c’est-à-dire que tout idéal premier $ q $ de $ B $ tel que $ \rho^{-1}(q) \subset p $ est contenu dans $ r $. Si $ p $ est minimal, on a $ \rho^{-1}(q) = p $, donc $ q = r $. Si $ B $ est entier sur $ A $, il existe d’après V, § 2, no 1, cor. 2 au th. 1, un idéal premier $ r' $ de $ B $ tel que $ q \subset r' $ et $ \rho^{-1}(r') = p $; on a nécessairement $ r' = r $, donc $ q \subset r $.

#### Lemme 2 {#ac-viii-s7-lem-2 .statement}

*Supposons $ A $ semi-local ; soit $ q $ un idéal de définition de $ A $, et soit $ \rho : A \to B $ un homomorphisme d’anneaux faisant de $ B $ un $ A $-module de type fini. Supposons que, pour tout idéal premier (nécessairement minimal) $ p $ de $ A $ tel que $ \dim(A/p) = \dim(A) $, il existe un unique idéal premier $ r $ de $ B $ au-dessus de $ p $ et que l’homomorphisme canonique $ \rho_p : A_p \to B_r $ soit bijectif. Alors on a $ \dim_A(B) = \dim(A) $ et $ e_q^A(B) = e_q^A(A) $.*

Soit $ \mathfrak{S}_A $ (resp. $ \mathfrak{S}_B $) l’ensemble des idéaux premiers $ p $ de $ A $ tels que

$$
\dim(A/p) = \dim(A) \quad (\text{resp. } \dim_A(B/pB) = \dim_A(B));
$$

on a $ \mathfrak{S}_A \neq \varnothing $. Soit $ p \in \mathfrak{S}_A $; il existe par hypothèse un idéal premier de $ B $ au-dessus de $ p $. On a alors $ \rho^{-1}(pB) = p $ (II, § 2, no 5, cor. 3 à la prop. 11), et

$$
\dim(A/p) = \dim(B/pB) = \dim_A(B/pB)
$$

d’après le th. 1, $ b) $ et $ c) $ du § 2, no 3. Par suite, on a

$$
\dim_A(B) \geq \dim_A(B/pB) = \dim(A/p) = \dim(A) \geq \dim_A(B).
$$

Cela implique $ \mathfrak{S}_A \subset \mathfrak{S}_B $ et $ \dim(A) = \dim_A(B) $. Inversement, si $ p \in \mathfrak{S}_B $, on a les inégalités

$$
\dim_A(B/pB) = \dim_A(B) = \dim(A) \geq \dim(A/p) \geq \dim_A(B/pB),
$$

d’où $ p \in \mathfrak{S}_A $ et $ \mathfrak{S}_B = \mathfrak{S}_A $. D’après la prop. 3 du no 1 et son corollaire, on a

$$
e_q^A(A) = \sum_{p \in \mathfrak{S}_A} e_q^A(A/p) \quad \text{et} \quad e_q^A(B) = \sum_{p \in \mathfrak{S}_B} \operatorname{long}_{A_p}(A_p \otimes_A B) e_q^A(A/p);
$$

d’après le lemme 1, on a $ \operatorname{long}_{A_p}(A_p \otimes_A B) = 1 $ pour tout $ p \in \mathfrak{S}_A $, d’où $ e_q^A(A) = e_q^A(B) $.

#### Proposition 6 {#ac-viii-s7-prop-6 .statement}

*Supposons $ A $ semi-local et réduit ; soit $ q $ un idéal de définition de $ A $; soit $ A' $ l’anneau total des fractions de $ A $, et soit $ B $ une sous-A-algèbre finie de $ A' $. Alors $ B $ est semi-local et $ qB $ en est un idéal de définition. Supposons que, pour tout idéal maximal m de B tel que dim(B_m) = dim(B), on ait [B/m : A/(A ∩ m)] = 1. Alors on a $ e_q^A(A) = e_{q_B}^B(B) $.

D’après IV, § 2, n° 5, cor. 3 de la prop. 9, B est semi-local d’idéal de définition qB. On a $ e_{q_B}^B(B) = e_q^A(B) $ d’après le corollaire à la prop. 5. Comme A′ s’identifie à $ \prod_p A_p $ où p parcourt l’ensemble des idéaux premiers minimaux de A (IV, § 2, n° 5, prop. 10), l’application canonique $ A_p \to A_p \otimes_A B $ est bijective pour tout idéal premier minimal p de A. Il résulte alors des lemmes 1 et 2 que $ e_q^A(B) = e_q^A(A) $, d’où la proposition.

#### Exemple {#ac-viii-s7-n3-exa-1 .statement}

Soit k un corps de caractéristique $ \neq 2 $ et prenons pour A l’anneau local $ k[[X, Y]]/(X^2 + Y^2) $ de corps résiduel k. Prenons $ B = k[[X, T]]/(T^2 + 1) $ où $ T = Y/X $. Distinguons deux cas : si — 1 est le carré d’un élément i de k, B possède deux idéaux maximaux engendrés respectivement par {X, T + i} et {X, T − i}, ils sont de corps résiduel k, et l’on a $ e_{m_A}^A(A) = e_{m_{AB}}^B(B) = 2 $. Si — 1 n’est pas un carré dans k, B possède un unique idéal maximal (X) de corps résiduel $ k[T]/(T^2 + 1) $, et l’on a $ e_{m_A}^A(A) = 2,\ e_{m_{AB}}^B(B) = 1 $.

### 4. Multiplicités et suites sécantes

#### Proposition 7 {#ac-viii-s7-prop-7 .statement}

Supposons A local. Soit s un entier $ \geq 1 $ et, pour $ 1 \leq i \leq s $, soient $ \delta_i $ un entier $ > 0 $, $ x_i $ un élément de $ m_A^{\delta_i} $, et $ \xi_i $ sa classe dans $ m_A^{\delta_i}/m_A^{\delta_i+1} $. On suppose que $ (x_1, ..., x_s) $ est une suite sécante pour A. Notons x l’idéal de A engendré par $ (x_1, ..., x_s) $. Alors on a $ e(A/x) \geq \delta_1 ... \delta_s \cdot e(A) $ avec égalité si $ (\xi_1, ..., \xi_s) $ est une suite complètement sécante pour gr(A).

Posons $ B = A/x $, et considérons les séries formelles

$$
H_A = \sum_{n \geq 0} \operatorname{long}(m_A^n/m_A^{n+1}) \cdot T^n, \quad H_B = \sum_{n \geq 0} \operatorname{long}(m_B^n/m_B^{n+1}) \cdot T^n
$$

et $ H_B^{(s)} = (1 - T)^{-s} H_B $. D’après la prop. 6 du § 4, n° 5, on a dans $ \mathbf{Z}[[T]] $, l’inégalité

$$
H_B^{(s)} \geq \left( \prod_{i=1}^s \frac{1 - T^{\delta_i}}{1 - T} \right) H_A,
$$

et il y a égalité lorsque la suite $ (\xi_1, ..., \xi_s) $ est complètement sécante. Mais

$$
R(T) = \prod_{i=1}^s \frac{1 - T^{\delta_i}}{1 - T}
$$

est un polynôme de $ \mathbf{Z}[T] $ tel que $ R(1) = \delta_1 ... \delta_s $. Posons $ \dim(A) = d $; on a $ \dim(B) = d - s $. D’après le th. 2 du § 4, n° 3, il existe des éléments $ R_A $ et $ R_B $ de $ \mathbf{Z}[T, T^{-1}] $ tels que

$$
H_A = (1 - T)^{-d} R_A(T), \quad R_A(1) = e(A),
$$
$$
H_B = (1 - T)^{-d+s} R_B(T), \quad R_B(1) = e(A/x).
$$

Donc on a
$$
(1 - T)^{-d} R_B(T) = H_B^{(s)} \geq \left( \prod_{i=1}^s \frac{1 - T^{\delta_i}}{1 - T} \right) H_A = (1 - T)^{-d} R(T) \, R_A(T),
$$
et l’égalité a lieu si la suite $(\xi_1, ..., \xi_s)$ est complètement sécante. On conclut par le lemme 2 du § 4, no 1.

#### Remarque {#ac-viii-s7-n4-rem-1 .statement}

On peut montrer réciproquement (*cf.* p. 103, exerc. 4) que si A est régulier et $e(A/x) = \delta_1 ... \delta_s$, alors la suite $(\xi_1, ..., \xi_s)$ est complètement sécante.

#### Exemple {#ac-viii-s7-n4-exa-1 .statement}

Prenons pour A un anneau de séries formelles $k[[X_1, ..., X_n]]$ sur un corps $k$; soient $F_1, ..., F_s$ des éléments de A, à l’idéal qu’ils engendrent et B = A/a. Notons $P_1, ..., P_s \in k[X_1, ..., X_n]$ les formes initiales des séries $F_1, ..., F_s$ et $\delta_1, ..., \delta_s$ leurs degrés respectifs. Si la suite $F_1, ..., F_s$ est sécante dans A, on a $e(B) \geq \delta_1 ... \delta_s$; si la suite $P_1, ..., P_s$ est complètement sécante dans l’anneau $k[X_1, ..., X_n]$, on a $e(B) = \delta_1 ... \delta_s$.

Considérons par exemple l’anneau $B = k[[X, Y]]/a$, où a est engendré par $X^2 + Y^3$ et $X^2 + Y^4$; l’inégalité précédente donne $e(B) \geq 4$; en remarquant que a est engendré par les éléments $X^2 + Y^3$ et $Y^4 - Y^3$, pour lesquels la suite des formes initiales est complètement sécante, on obtient $e(B) = 6$.

### 5. Éléments superficiels

Dans ce numéro on note q un idéal de A contenu dans le radical de A, et M un A-module non nul de type fini tel que $M/qM$ soit de longueur finie.

#### Proposition 8 {#ac-viii-s7-prop-8 .statement}

Soient $\delta > 0$ un entier, x un élément de $q^\delta$, $\xi$ sa classe dans $\mathrm{gr}_\delta(A) = q^\delta/q^{\delta+1}$ et $\varphi$ la multiplication par $\xi$ dans le gr(A)-module gr(M).

a) La dimension du A-module $M/xM$ est égale à $\dim_A(M)$ ou à $\dim_A(M) - 1$. Dans le deuxième cas, on a $e_q(M/xM) \geq \delta e_q(M)$.

b) Supposons que l’on ait $\dim_A(M) \geq 1$ et que le noyau de $\varphi$ soit de longueur finie sur $A/q$. Alors on a $\dim_A(M/xM) = \dim_A(M) - 1$. De plus :
(i) Si $\dim_A(M) > 1$, on a $e_q(M/xM) = \delta e_q(M)$.
(ii) Si $\dim_A(M) = 1$, on a pour tout entier $n \geq 0$
$$
n \delta e_q(M) \leq \mathrm{long}_A(M/x^nM) \leq n \delta e_q(M) + \mathrm{long}_{A/q}(\mathrm{Ker}\ \varphi^n),
$$
où $\varphi^n$ est le n-ième itéré de l’endomorphisme $\varphi$, et
$$
\delta e_q(M) = e_{xA}(M) \leq \mathrm{long}_A(M/xM).
$$

Posons $M'' = M/xM$; considérons les séries de Hilbert-Samuel $H_M = H_{M,q}$ et $H_{M''} = H_{M'',q}$, ainsi que la série de Poincaré $P(T) = \sum_{n \geq 0} \mathrm{long}_{A/q}(\mathrm{Ker}\ \varphi_n) \cdot T^n$. D’après § 4, no 3, th. 2 et no 4, remarque 2, on a
$$
H_M(T) = (1 - T)^{-d} R_M(T), \quad H_{M''}(T) = (1 - T)^{-d''} R_{M''}(T),
$$

avec $ d = \dim_A(M) $, $ d'' = \dim_A(M'') $, $ R_M $ et $ R_{M''} $ dans $ \mathbf{Z}[T] $, $ R_M(1) = e_q(M) $, $ R_{M''}(1) = e_q(M'') $. D’après le lemme 6 du § 4, n° 5, on a dans $ \mathbf{Z}((T)) $ les inégalités

$$
(1 - T^\delta) H_M^{(1)} \leq H_{M''}^{(1)} \leq (1 - T^\delta) H_M^{(1)} + T^\delta P^{(1)} .
$$

Posant $ R(T) = (1 - T^\delta)/(1 - T) = 1 + T + \cdots + T^{\delta-1} $, cela s’écrit aussi

(1) $$ (1 - T)^{-d} R(T) R_M(T) \leq (1 - T)^{-d''-1} R_{M''}(T) \leq $$
$$ \leq (1 - T)^{-d} R(T) R_M(T) + (1 - T)^{-1} T^\delta P(T) . $$

D’après le lemme 2 du § 4, n° 1, la première inégalité (1) implique soit $ d'' \geq d $, soit $ d'' = d - 1 $ et $ R(1) R_M(1) \leq R_{M''}(1) $, c’est-à-dire $ \delta e_q(M) \leq e_q(M'') $. Cela démontre $ a) $, puisque $ d'' \leq d $.

Sous l’hypothèse de $ b) $, on a $ P(T) \in \mathbf{Z}[T] $ et $ P(1) = \operatorname{long}_A(\operatorname{Ker} \varphi) $. La seconde inégalité (1) s’écrit

$$
(1 - T)^{-d''-1} R_{M''}(T) \leq (1 - T)^{-d}(R(T) R_M(T) + T^\delta (1 - T)^{d-1} P(T)) .
$$

Supposons qu’on ait $ d > 1 $; alors le lemme 2 du § 4, n° 1 entraîne $ d'' + 1 \leq d $, d’où $ d'' = d - 1 $ d’après la partie $ a) $ de la démonstration; on a alors

$$
R_{M''}(1) \leq R(1). R_M(1)
$$

(loc. cit.), d’où (i).

Supposons maintenant $ d = 1 $. D’après loc. cit., on a $ d'' = 0 $ et

$$
R_{M''}(1) \leq R(1). R_M(1) + P(1) .
$$

Par conséquent, $ M'' $ est de longueur finie égale à $ e_q(M'') = R_{M''}(1) $ et l’on obtient

(2) $$ \delta e_q(M) \leq \operatorname{long}_A(M/xM) \leq \delta e_q(M) + \operatorname{long}_A(\operatorname{Ker} \varphi) . $$

Soit $ n \geq 1 $ un entier. Remplaçons $ x $ par $ x^n $ dans (2); on a donc

(3) $$ n \delta e_q(M) \leq \operatorname{long}_A(M/x^nM) \leq n \delta e_q(M) + \operatorname{long}_A(\operatorname{Ker} \varphi^n) . $$

Il est immédiat que les sous-modules $ \operatorname{Ker} \varphi^n $ du gr(A)-module noethérien gr(M) forment une suite croissante donc stationnaire et que chacun d’eux est de longueur finie sur $ A/q $. Divisant par $ n \geq 1 $ dans l’inégalité (3) et faisant tendre $ n $ vers $ + \infty $, on trouve $ e_{xA}(M) = \delta e_q(M) $ par définition de $ e_{xA}(M) $.

#### Lemme 3 {#ac-viii-s7-lem-3 .statement}

Soient $ R $ un anneau noethérien gradué à degrés $ \geq 0 $, $ E $ un $ R $-module gradué de type fini tel que $ E_n $ soit un $ R_0 $-module de longueur finie pour tout $ n \in \mathbf{Z} $.
Les conditions suivantes sont équivalentes :
(i) $ E $ est un $ R $-module de longueur finie ;
(ii) il existe un entier $ n_0 $ tel que $ E_n = 0 $ pour $ n \geq n_0 $ ;
(iii) tout idéal premier de $ R $ associé à $ E $ contient $ R_+ = \bigoplus_{n \geq 1} R_n $.

(i) ⇔ (ii) : c’est clair.
(iii) ⇒ (i) : soit $ p $ un idéal premier associé à E. Si (iii) est satisfaite, on a $ p = p_0 + R_+ $ où $ p_0 $ est un idéal premier de $ R_0 $, et le R-module $ R/p $ est isomorphe à $ R_0/p_0 $. D’après IV, § 3, no 1, corollaire de la prop. 1, le $ R_0 $-module $ R_0/p_0 $ est isomorphe à un sous-module d’un des $ E_k $, donc est de longueur finie. Par conséquent, $ R/p $ est de longueur finie. D’après IV, § 2, no 5, prop. 7, $ p $ est donc maximal. Vu l’arbitraire de $ p $, le R-module E est de longueur finie (loc. cit.).
(i) ⇒ (iii) : soit $ p $ un idéal premier associé à E. Alors $ p $ est gradué (IV, § 3, no 1, prop. 1) et maximal (IV, § 2, no 5, prop. 7), donc contient $ R_+ $ (§ 6, no 2, lemme 1).

#### Proposition 9 {#ac-viii-s7-prop-9 .statement}

Notons $ p_1, ..., p_r $ ceux des idéaux premiers de l’anneau gradué $ \mathrm{gr}(A) = \bigoplus_n (q^n/q^{n+1}) $ qui sont associés au module gradué $ \mathrm{gr}(M) = \bigoplus_n (q^n M/q^{n+1} M) $ et ne contiennent pas $ \mathrm{gr}_1(A) = q/q^2 $. Soient $ \delta $ un entier $ > 0 $, $ \xi $ un élément de $ \mathrm{gr}_\delta(A) $, et $ \varphi : \mathrm{gr}(M) \to \mathrm{gr}(M) $ l’homothétie de rapport $ \xi $ dans $ \mathrm{gr}(M) $. Pour que $ \varphi_n $ soit injective pour tout $ n $ assez grand, il faut et il suffit que $ \xi $ n’appartienne à aucun des $ p_i $.
En effet, les idéaux premiers associés au $ \mathrm{gr}(A) $-module $ \mathrm{Ker}\, \varphi $ sont ceux des idéaux premiers associés à $ \mathrm{gr}(M) $ qui contiennent $ \xi $ (IV, § 1, no 1, déf. 1). D’après le lemme 3, $ (\mathrm{Ker}\, \varphi)_n $ est nul pour $ n $ assez grand, si et seulement si ces idéaux contiennent tous $ \mathrm{gr}_+(A) $ (ou ce qui revient au même $ \mathrm{gr}_1(A) $), d’où la proposition.

#### Définition 2 {#ac-viii-s7-def-2 .statement}

Soient A un anneau noethérien, q un idéal de A contenu dans le radical de A et M un A-module de type fini tel que $ M/qM $ soit de longueur finie. Un élément x de A est dit superficiel pour M relativement à q s’il appartient à q et si, pour tout $ n $ assez grand, l’application $ q^n M/q^{n+1} M \to q^{n+1} M/q^{n+2} M $ induite par la multiplication par x est injective.

#### Remarque 1 {#ac-viii-s7-n5-rem-1 .statement}

Soit $ \delta $ un entier $ > 0 $. On dit parfois qu’un élément x de A est superficiel d’ordre $ \delta $ pour M relativement à q si $ x \in q^\delta $, et si, pour tout $ n $ assez grand, l’application $ q^n M/q^{n+1} M \to q^{n+\delta} M/q^{n+\delta+1} M $ induite par la multiplication par x est injective. Avec cette terminologie, les éléments superficiels au sens de la déf. 2 sont les éléments superficiels d’ordre 1.
2) Avec les notations de la prop. 9, x est superficiel d’ordre $ \delta $ si et seulement si sa classe $ \xi $ dans $ \mathrm{gr}_\delta(A) $ n’appartient à aucun des $ p_i $.
3) D’après III, § 1, no 4, prop. 8, il existe un élément homogène de $ \mathrm{gr}(A) $ de degré $ > 0 $ qui n’appartient à aucun des $ p_i $. Par conséquent, il existe un entier $ \delta > 0 $ et un élément superficiel d’ordre $ \delta $ pour M.
4) Supposons A local de corps résiduel k, et considérons l’application surjective canonique $ \lambda : q \to q \otimes_A k $. Elle est la composée des applications canoniques $ q \to q/q^2 $ et $ \bar{\lambda} : q/q^2 \to q \otimes_A k $. D’après le lemme de Nakayama, chacun des sous-espaces vectoriels $ V_i = \bar{\lambda}(p_i \cap (q/q^2)) $ de $ q \otimes_A k $ est distinct de $ q \otimes_A k $; si $ \alpha \in q \otimes_A k $ n’appartient à aucun des $ V_i $, alors $ \lambda^{-1}(\alpha) $ est formé d’éléments superficiels pour M (prop. 9). Si k est infini, la réunion des $ V_i $ est distincte de $ q \otimes_A k $ et il existe donc des éléments superficiels pour M.

#### Théorème 1 {#ac-viii-s7-thm-1 .statement}

Soient $ A $ un anneau noethérien, $ q $ un idéal de $ A $ contenu dans le radical de $ A $ et $ M $ un $ A $-module de type fini tel que $ M/qM $ soit de longueur finie. Soit $ x_1, ..., x_m $ une suite finie d’éléments de $ q $. Posons $ x = Ax_1 + \cdots + Ax_m \subset q $.

a) On a $ \dim_A(M/xM) \geq \dim_A(M) - m $.

b) Si $ \dim_A(M/xM) = \dim_A(M) - m $, alors $ e_q(M/xM) \geq e_q(M) $.

c) Si $ m < \dim_A(M) $, et si pour $ i = 1, ..., m $, l’élément $ x_i $ de $ A $ est superficiel pour $ M/(x_1M + \cdots + x_{i-1}M) $ relativement à $ q $, alors on a

$$
\dim_A(M/xM) = \dim_A(M) - m \quad \text{et} \quad e_q(M/xM) = e_q(M) .
$$

d) Si $ m = \dim_A(M) $, et si, pour $ i = 1, ..., m $, l’élément $ x_i $ de $ A $ est superficiel pour $ M/(x_1M + \cdots + x_{i-1}M) $ relativement à $ q $, alors on a

$$
e_q(M) = e_x(M) \leq \operatorname{long}(M/xM) < + \infty .
$$

Les parties $ a), b), $ et $ c) $ résultent pour $ m = 1 $ de la prop. 8, et le cas général s’en déduit par récurrence. Supposons les hypothèses de $ d) $ satisfaites et posons $ x' = Ax_1 + \cdots + Ax_{m-1} $ et $ M' = M/x'M $ de sorte que $ M/xM $ s’identifie à $ M'/x_mM' $. Alors, d’après $ c) $, on a $ \dim_A(M') = 1 $ et $ e_q(M) = e_q(M') $. D’après la prop. 8, $ M/xM $ est de longueur finie et l’on a $ e_q(M') = e_{x_mA}(M') \leq \operatorname{long}(M/xM) $. Mais, puisque $ x_m^nM' = x^nM' $ pour tout $ n $, on a $ e_{x_mA}(M') = e_x(M') $. On a par ailleurs $ e_x(M') \geq e_x(M) $ : cela résulte de $ b) $ où l’on remplace $ m $ par $ m - 1 $, $ x $ par $ x' $ et $ q $ par $ x $. Par conséquent, on a

$$
e_x(M) \leq e_x(M') = e_{x_mA}(M') = e_q(M') = e_q(M) .
$$

Puisque $ x $ est contenu dans $ q $, cela implique $ e_x(M) = e_q(M) $ (n° 1, remarque 1), et achève la démonstration.

#### Corollaire {#ac-viii-s7-n5-cor-1 .statement}

Supposons $ A $ local, à corps résiduel infini, et posons $ d = \dim_A(M) $. Il existe une suite $ x_1, ..., x_d $ d’éléments de $ q $ tels que, en posant $ x = Ax_1 + \cdots + Ax_d $, on ait

$$
e_q(M) = e_x(M) \leq \operatorname{long}(M/xM) < + \infty .
$$

Cela résulte aussitôt du théorème et de la remarque 4.

#### Remarque 5 {#ac-viii-s7-n5-rem-5 .statement}

Dans la situation du corollaire précédent, on a

$$
e_q(M) = e_x(M) \leq \operatorname{long}(M/xM)
$$

et $ \operatorname{long}(M/qM) \leq \operatorname{long}(M/xM) $; les trois cas

$$
e_q(M) < \operatorname{long}(M/qM) , \quad e_q(M) = \operatorname{long}(M/qM) , \quad e_q(M) > \operatorname{long}(M/qM)
$$

sont possibles (p. 106, exerc. 16 et 17).

Exercises

## EXERCICES {#ac-viii-s7-exercises}

See the [exercises for § 7](exercises/s7/).
