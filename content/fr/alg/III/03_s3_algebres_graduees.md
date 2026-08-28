---
book: alg
book_title: Algebra
chapter: III
chapter_title: ALGÈBRES TENSORIELLES, ALGÈBRES EXTÉRIEURES, ALGÈBRES SYMÉTRIQUES
section: 3
section_title: Algèbres graduées
lang: fr
source: alg-i-iii-fr
book_pages: A III.30-A III.33, A III.183
pdf_pages: 0417-0420, 0570-0570
extraction: ocr
subsections:
    - "no": 1
      title: Algèbres graduées
      page: 30
      pdf_page: 417
    - "no": 2
      title: Sous-algèbres graduées, idéaux gradués d’une algèbre graduée
      page: 32
      pdf_page: 419
    - "no": 3
      title: Limites inductives d’algèbres graduées
      page: 32
      pdf_page: 419
statements: 6
exercises: 1
content_sha256: 6f21229504e496b104498446d4de3ebeae83d02b31cb596d657fcf1f1e55bbfb
---

## § 3. ALGÈBRES GRADUÉES

Les graduations dont il sera question dans ce paragraphe auront pour ensemble de degrés un monoïde commutatif noté additivement et dont l’élément neutre est noté 0.

### 1. Algèbres graduées

#### Définition 1 {#alg-iii-s3-def-1 .statement}

Soient $\Delta$ un monoïde commutatif, $A$ un anneau commutatif gradué de type $\Delta$ (II, p. 164), $(A_\lambda)_{\lambda \in \Delta}$ sa graduation, $E$ une $A$-algèbre. On dit qu’une graduation $(E_\lambda)_{\lambda \in \Delta}$ de type $\Delta$ sur le groupe additif $E$ est compatible avec la structure de $A$-algèbre de $E$ si elle est compatible à la fois avec la structure de $A$-module et avec la structure d’anneau de $E$, autrement dit, si l’on a, quels que soient $\lambda, \mu$ dans $\Delta$,

(1)
$$
A_\lambda E_\mu \subset E_{\lambda + \mu}
$$
(2)
$$
E_\lambda E_\mu \subset E_{\lambda + \mu}.
$$

La $A$-algèbre $E$, munie de cette graduation, est alors appelée algèbre graduée de type $\Delta$ sur l’anneau gradué $A$.

Lorsque la graduation de $A$ est *triviale* (c’est-à-dire (II, p. 163) que $A_0 = A$, $A_\lambda = \{0\}$ pour $\lambda \neq 0$), la condition (1) signifie que les $E_\lambda$ sont des *sous-A-modules* de $E$. Ceci conduit à définir la notion d’algèbre graduée de type $\Delta$ sur un anneau commutatif $A$ *non gradué*: on munit $A$ de la graduation triviale de type $\Delta$ et on applique la définition précédente.

Lorsque nous considérerons des $A$-algèbres graduées $E$ ayant un élément unité $e$, il sera toujours sous-entendu que $e$ est *de degré* 0 (cf. III, p. 183, exerc. 1).

On en conclut que si un élément inversible $x \in E$ est *homogène* et de degré $p$, son inverse $x^{-1}$ est *homogène* et de degré $-p$: il suffit en effet de décomposer $x^{-1}$ en somme d’éléments homogènes dans les relations $x^{-1}x = xx^{-1} = e$.

Soient $E$ et $E'$ deux algèbres graduées de type $\Delta$ sur un anneau gradué $A$ de type $\Delta$. On dit qu’un homomorphisme $u : E \to E'$ de $A$-algèbres est un *homomorphisme d’algèbres graduées* si on a $u(E_\lambda) \subset E'_\lambda$ pour tout $\lambda \in \Delta$ (en désignant par $(E_\lambda)$ et $(E'_\lambda)$ les graduations respectives de $E$ et $E'$); lorsque $E$ et $E'$ sont associatives et unifères, et que $u$ est unifère, cette condition signifie que $u$ est un homomorphisme d’anneaux gradués (II, p. 166).

Soit $E$ une $A$-algèbre graduée de type $\mathbf{N}$. On identifie $E$ à une $A$-algèbre graduée de type $\mathbf{Z}$, en convenant que $E_n = \{0\}$ pour $n < 0$.

#### Remarque {#alg-iii-s3-n1-rem-1 .statement}

La définition 1 peut encore s’interpréter en disant que E est un A-module gradué et que l’application A-linéaire

$$
m : E \otimes_A E \to E
$$

qui définit la multiplication dans E (III, p. 5) est homogène de degré 0 lorsqu’on munit $E \otimes_A E$ de sa graduation de type $\Delta$ (II, p. 173).

Définir une structure de A-algèbre graduée de type $\Delta$ sur l’anneau gradué A, ayant E pour A-module gradué sous-jacent, revient donc à définir, pour chaque couple $(\lambda, \mu)$ d’éléments de $\Delta$, une application $\mathbf{Z}$-bilinéaire $m_{\lambda \mu} : E_\lambda \times E_\mu \to E_{\lambda + \mu}$ telle que pour tout triplet d’indices $(\lambda, \mu, \nu)$ et pour $\alpha \in A_\lambda$, $x \in E_\mu$, $y \in E_\nu$, on ait $\alpha . m_{\mu, \nu}(x, y) = m_{\lambda + \mu, \nu}(\alpha x, y) = m_{\mu, \lambda + \nu}(x, \alpha y)$.

#### Exemple 1 {#alg-iii-s3-n1-exa-1 .statement}

Soit B un anneau gradué de type $\Delta$; si on munit B de sa structure canonique de $\mathbf{Z}$-algèbre (III, p. 2, Exemple 2), B est une A-algèbre graduée ($\mathbf{Z}$ étant muni de la graduation triviale).

#### Exemple 2 {#alg-iii-s3-n1-exa-2 .statement}

Soient A un anneau commutatif gradué de type $\Delta$, M un A-module gradué de type $\Delta$. Supposons que tous les éléments du monoïde $\Delta$ soient simplifiables, ce qui permet (II, p. 175) de définir sur $\mathrm{Homgr}_A(M, M) = \mathrm{Endgr}_A(M)$ une structure de A-module gradué de type $\Delta$; comme cette graduation est compatible avec la structure d’anneau de $\mathrm{Endgr}_A(M)$ (II, p. 175), elle définit sur la A-algèbre $\mathrm{Endgr}_A(M)$ une structure de A-algèbre graduée unifère.

#### Exemple 3 {#alg-iii-s3-n1-exa-3 .statement}

Algèbre d’un magma. Soient S un magma et soit $\varphi : S \to \Delta$ un homomorphisme. Pour tout $\lambda \in \Delta$, posons $S_\lambda = \varphi^{-1}(\lambda)$; on a alors $S_\lambda S_\mu \subset S_{\lambda + \mu}$. Soient A un anneau commutatif gradué de type $\Delta$, $(A_\lambda)_{\lambda \in \Delta}$ sa graduation; nous allons définir sur l’algèbre $E = A^{(S)}$ du magma S (III, p. 19) une structure de A-algèbre graduée. Pour cela, désignons par $E_\lambda$ le sous-groupe additif de E engendré par les éléments de la forme $\alpha . s$ tels que $\alpha \in A_\mu$, $s \in S_\nu$ et $\mu + \nu = \lambda$. Comme les $S_\lambda$ sont deux à deux disjoints, E est somme directe des $A_\mu S_\nu$, donc aussi somme directe des $E_\lambda$, et il est immédiat que les $E_\lambda$ vérifient les conditions (1) et (2) de III, p. 30 et définissent donc sur E la structure de A-algèbre graduée voulue. Si S admet un élément neutre $e$, on supposera en outre que $\varphi(e) = 0$. Un cas particulier est celui où la graduation de l’anneau A est triviale; alors $E_\lambda$ est le sous-A-module de E engendré par $S_\lambda$. Plus particulièrement, si l’on prend $S = \mathbf{N}^{(I)}$, $\Delta = \mathbf{N}$ et pour $\varphi$ l’application telle que $\varphi((n_i)) = \sum_{i \in I} n_i$, l’anneau A étant muni de la graduation triviale, on obtient ainsi sur l’algèbre de polynômes $A[X_i]_{i \in I}$ une graduation pour laquelle le degré d’un polynôme homogène $\neq 0$ est le degré total défini dans III, p. 26 (cf. III, p. 73).

Prenons maintenant pour S le monoïde libre Mo(B) d’un ensemble B (I, p. 79), et pour $\varphi$ l’homomorphisme $\mathrm{Mo}(B) \to \mathbf{N}$ qui à chaque mot associe sa longueur. On obtient ainsi une structure de A-algèbre graduée sur l’algèbre associative libre de l’ensemble B (III, p. 21; cf. III, p. 62).

### 2. Sous-algèbres graduées, idéaux gradués d’une algèbre graduée

Soit E une algèbre graduée de type Δ sur un anneau gradué A de type Δ. Si F est une sous-A-algèbre de E qui est un sous-A-module gradué, alors la graduation (F_λ) de F est compatible avec sa structure de A-algèbre, puisque F_λ = F ∩ E_λ ; on dit dans ce cas que F est une sous-algèbre graduée de E, et l’injection canonique F → E est un homomorphisme d’algèbres graduées.

De même, si a est un idéal à gauche (resp. à droite) de E qui soit un sous-A-module gradué, on a E_λ a_μ ⊂ a_{λ+μ} (resp. a_λ E_μ ⊂ a_{λ+μ}), puisque a_λ = a ∩ E_λ ; on dit alors que a est un idéal gradué de l’algèbre E. Si b est un idéal bilatère gradué de E, la graduation quotient sur le module E/b est compatible avec la structure d’algèbre de E/b, et l’homomorphisme canonique E → E/b est un homomorphisme d’algèbres graduées.

Si u : E → E' est un homomorphisme d’algèbres graduées, Im(u) est une sous-algèbre graduée de E', Ker(u) un idéal bilatère gradué de E, la bijection E/Ker(u) → Im(u) canoniquement associée à u étant un isomorphisme d’algèbres graduées.

#### Proposition 1 {#alg-iii-s3-prop-1 .statement}

Soient A un anneau commutatif gradué de type Δ, E une A-algèbre graduée de type Δ, S un ensemble d’éléments homogènes de E. Alors la sous-A-algèbre (resp. l’idéal à gauche, l’idéal à droite, l’idéal bilatère) engendrée par S (resp. engendré par S) est une sous-algèbre graduée (resp. un idéal gradué).

La sous-algèbre de E engendrée par S est le sous-A-module engendré par les produits finis d’éléments de S, qui sont homogènes; de même, l’idéal à gauche (resp. à droite) engendré par S est le sous-A-module engendré par les éléments de la forme u_1(u_2(...(u_n s))...) (resp. (...((s u_n) u_{n-1})...) u_2) u_1, où s ∈ S et les u_j ∈ E sont homogènes (n quelconque) et ces produits sont homogènes, d’où dans ce cas la conclusion en vertu de II, p. 167, prop. 2; enfin l’idéal bilatère engendré par S est la réunion de la suite (J_n)_{n ≥ 1}, où J_1 est l’idéal à gauche engendré par S, J_{2n} (resp. J_{2n+1}) l’idéal à droite (resp. à gauche) engendré par J_{2n-1} (resp. J_{2n}), ce qui termine la démonstration.

### 3. Limites inductives d’algèbres graduées

Soit (A_α, φ_{βα}) un système inductif filtrant d’anneaux commutatifs gradués de type Δ (II, p. 170, Remarque 3), et pour chaque α, soit E_α une A_α-algèbre graduée de type Δ; pour α ≤ β, soit f_{βα} : E_α → E_β un A_α-homomorphisme d’algèbres graduées, et supposons que l’on ait f_{γα} = f_{γβ} ◦ f_{βα} pour α ≤ β ≤ γ; nous dirons alors que (E_α, f_{βα}) est un système inductif filtrant d’algèbres graduées de type Δ sur le système inductif filtrant (A_α, φ_{βα}) d’anneaux commutatifs graduées de type Δ. On sait alors (II, p. 170) que E = lim → E_α est canoniquement muni d’une structure de module gradué de type Δ sur l’anneau gradué A = lim → A_α, et d’une multiplication telle que E^λ E^μ ⊂ E^{λ+μ} (en désignant par (E^λ) la graduation de E);

donc cette multiplication et la structure de A-module gradué de E définissent sur E une structure de A-\emph{algèbre graduée de type} $\Delta$; on dit que E, muni de cette structure, est la \emph{limite inductive} du système inductif $(E_\alpha,\ f_{\beta\alpha})$ d’algèbres graduées. Les homomorphismes canoniques $E_\alpha \to E$ sont alors des $A_\alpha$-homomorphismes d’algèbres graduées. En outre, si F est une A-algèbre graduée de type $\Delta$ et $(u_\alpha)$ un système inductif de $A_\alpha$-homomorphismes $u_\alpha : E_\alpha \to F$, $u = \lim u_\alpha$ est un A-homomorphisme d’algèbres graduées.

## EXERCICES {#alg-iii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
