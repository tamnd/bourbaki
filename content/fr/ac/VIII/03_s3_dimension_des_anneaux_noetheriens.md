---
book: ac
book_title: Commutative Algebra
chapter: VIII
chapter_title: DIMENSION
section: 3
section_title: Dimension des anneaux noethériens
lang: fr
source: ac-viii-ix-fr
book_pages: AC VIII.86-AC VIII.87
pdf_pages: 0028-0041, 0090-0091
extraction: ocr
subsections:
    - "no": 1
      title: Dimension d’un anneau quotient
      page: 24
      pdf_page: 28
    - "no": 2
      title: Dimension et suites sécantes
      page: 26
      pdf_page: 30
    - "no": 3
      title: Premières applications
      page: 0
      pdf_page: 33
    - "no": 4
      title: Changements d’anneaux
      page: 32
      pdf_page: 36
    - "no": 5
      title: Construction de suites sécantes
      page: 36
      pdf_page: 40
statements: 37
exercises: 7
content_sha256: 9e96d959c56485cbedf2ef098047ed722bad9561960260f61af3c6f4793e2f70
---

## § 3. DIMENSION DES ANNEAUX NOETHÉRIENS

### 1. Dimension d’un anneau quotient

#### Proposition 1 {#ac-viii-s3-prop-1 .statement}

Soient $A$ un anneau intègre noethérien, $x$ un élément non nul de $A$ et $p$ un élément minimal de l’ensemble des idéaux premiers de $A$ contenant $x$. Alors $p$ est de hauteur 1.

Soit $q \subset p$ un idéal premier distinct de $p$. On a $x \notin q$ vu le caractère minimal de $p$. Comme $A$ est intègre, $A_p$ s’identifie à un sous-anneau de $A_q$; pour tout entier $n \geq 0$, on note $q_n$ l’idéal $q^n A_q \cap A_p$ de $A_p$. Le caractère minimal de $p$ signifie que l’anneau local $A_p / xA_p$ est de dimension 0 ; il est donc de longueur finie ($§ 1$, no 3, exemple 1), et il existe un entier $n_0 \geq 0$ tel que l’on ait

$$
q_n + xA_p = q_{n+1} + xA_p \quad \text{pour tout } n \geq n_0 .
$$

Fixons l’entier $n \geq n_0$. Étant donné $y \in q_n$, il existe $a \in A_p$ tel que $y - ax \in q_{n+1}$; on a alors $ax \in q_n$, d’où $a \in q_n$ puisque $x \notin q$, et finalement on a $y \in q_{n+1} + xq_n$. On a donc

$$
q_n = q_{n+1} + xq_n .
$$

Comme $x$ appartient à l’idéal maximal de l’anneau local noethérien $A_p$, le lemme de Nakayama montre que l’on a $q_n = q_{n+1}$. Comme on a $(qA_q)^n = q_n A_q$, on en conclut

$$
(qA_q)^n = (qA_q)^{n+1} \quad \text{pour tout } n \geq n_0 .
$$

Comme l’anneau $A_q$ est local et noethérien, on a $\bigcap_{n \geq 0} (qA_q)^n = \{0\}$ (III, § 3, no 2, corollaire de la prop. 5) d’où $(qA_q)^{n_0} = \{0\}$ et finalement l’idéal premier $qA_q$ de $A_q$ est réduit à 0. On a donc $q = \{0\}$, ce qui prouve que $p$ est de hauteur 1.

#### Proposition 2 {#ac-viii-s3-prop-2 .statement}

Soient $A$ un anneau noethérien, $m$ un entier positif et $a$ un idéal contenu dans le radical de $A$ et engendré par $m$ éléments. On a

$$
\dim(A/a) \leq \dim(A) \leq \dim(A/a) + m .
$$

L’inégalité $\dim(A/a) \leq \dim(A)$ résulte de la prop. 6 du § 1, no 3. Une récurrence immédiate sur $m$ montre qu’il suffit d’établir l’inégalité

$$
\dim(A) \leq \dim(A/xA) + 1
$$

pour tout élément $x$ du radical de $A$, c’est-à-dire de démontrer que l’on a $\dim(A/xA) \geq n - 1$ pour toute chaîne $p_0 \subset ... \subset p_n$ d’idéaux premiers de $A$, de longueur $n \geqslant 1$, et telle que $x \in p_n$. Il suffit de construire une chaîne $q_1 \subset ... \subset q_n$ d’idéaux premiers de $A$, avec $x \in q_1$ et cela résulte du lemme suivant :

#### Lemme 1 {#ac-viii-s3-lem-1 .statement}

Soient $A$ un anneau noethérien, $p_0 \subset ... \subset p_n$ une chaîne d’idéaux premiers de $A$ de longueur $n \geqslant 1$ et $x$ un élément de $p_n$. Il existe une chaîne $p'_0 \subset ... \subset p'_n$ avec $p'_0 = p_0$, $p'_n = p_n$ et $x \in p'_1$.

Raisonnons par récurrence sur $n$, le cas $n = 1$ étant trivial. Supposons donc que l’on ait $n \geqslant 2$ et que $x$ n’appartienne pas à $p_{n-1}$. Soit $p'_{n-1}$ un élément minimal de l’ensemble des idéaux premiers de $A$ contenus dans $p'_n = p_n$ et contenant $p_{n-2} + Ax$ (II, § 2, no 6, lemme 2). D’après la prop. 1, l’idéal $p'_{n-1}/p_{n-2}$ de l’anneau $A/p_{n-2}$ est de hauteur 1, et comme $p_{n-2} \subset p_{n-1} \subset p_n$ est une chaîne de longueur 2, il en est de même de $p_{n-2} \subset p'_{n-1} \subset p'_n$. On a $x \in p'_{n-1}$. L’hypothèse de récurrence appliquée à la chaîne $p_0 \subset p_1 \subset ... \subset p_{n-2} \subset p'_{n-1}$ montre qu’il existe une chaîne $p'_0 \subset p'_1 \subset ... \subset p'_{n-2} \subset p'_{n-1}$ avec $x \in p'_1$ et $p'_0 = p_0$. La chaîne
$$
p'_0 \subset p'_1 \subset ... \subset p'_{n-1} \subset p'_n
$$
satisfait aux conditions exigées.

#### Corollaire 1 {#ac-viii-s3-lem-1-cor-1 .statement}

a) Tout anneau local noethérien est de dimension finie. Plus généralement, tout anneau semi-local (II, § 3, no 5, déf. 4) noethérien non nul est de dimension finie.
b) Soit $A$ un anneau noethérien. Tout idéal de $A$, distinct de $A$, est de hauteur finie.
c) Toute suite décroissante d’idéaux premiers d’un anneau noethérien $A$ est stationnaire.

a) Soient $A$ un anneau semi-local noethérien non nul et $a$ son radical ; l’anneau quotient $A/a$ est artinien et non nul, donc de dimension 0 ($§ 1$, no 3, exemple 1). Il existe un entier $m \geqslant 0$ tel que l’idéal $a$ de $A$ soit engendré par $m$ éléments ; on a donc $0 \leqslant \dim(A) \leqslant m$ d’après la prop. 2.
b) Soit $a \neq A$ un idéal de $A$, et soit $m$ un idéal maximal de $A$ contenant $a$. On a $0 \leqslant \mathrm{ht}(a) \leqslant \dim(A_m)$ d’après la prop. 7 du $§ 1$, no 3, et $A_m$ est un anneau local noethérien. Donc $\mathrm{ht}(a)$ est finie d’après a).
c) Toute suite strictement décroissante finie $(p_i)_{0 \leqslant i \leqslant n}$ d’idéaux premiers de $A$ définit une chaîne $p_n \subset ... \subset p_0$, d’où $n \leqslant \dim(A_{p_0}) < + \infty$. Il ne peut donc exister de suite strictement décroissante infinie d’idéaux premiers de $A$, d’où c).

#### Corollaire 2 {#ac-viii-s3-lem-1-cor-2 .statement}

Soit $A$ un anneau local noethérien.
a) Soit $x \in m_A$. Alors $\dim(A/xA)$ est égal à $\dim(A)$ ou à $\dim(A) - 1$. Pour que l’on ait $\dim(A/xA) = \dim(A) - 1$, il faut et il suffit que $x$ n’appartienne à aucun des idéaux premiers minimaux $p$ de $A$ tels que $\dim(A/p) = \dim(A)$, et il suffit que $x$ ne soit pas diviseur de 0 dans $A$.
b) Soit $a$ un idéal de $A$ distinct de $A$ tel que $\dim(A/a) < \dim(A)$. Il existe $x \in a$ tel que $\dim(A/xA) = \dim(A) - 1$.
c) Si $\dim(A) \geqslant 1$, il existe $x \in m_A$ tel que $\dim(A/xA) = \dim(A) - 1$.
D’après la prop. 2, $\dim(A/xA)$ est égal à $\dim(A)$ ou à $\dim(A) - 1$. Pour que l’on ait $\dim(A/xA) = \dim(A)$, il faut et il suffit qu’il existe une chaîne $p_0 \subset ... \subset p_n$ d’idéaux premiers de $A$ telle que $x \in p_0$ et $n = \dim(A)$, c’est-à-dire qu’il existe un idéal premier $p_0$ de $A$ contenant $x$ tel que $\dim(A/p_0) = \dim(A)$. Mais un tel idéal premier $p_0$ est nécessairement minimal, et tout élément de $p_0$ est donc diviseur de 0 dans $A$ (IV, § 1, no 1, cor. 3 de la prop. 2 et no 4, th. 2). Ceci prouve a).

Soient $\Phi$ l’ensemble des idéaux premiers minimaux de $A$, et $\Phi'$ l’ensemble des $p \in \Phi$ tels que $\dim(A/p) = \dim(A)$. On sait (II, § 4, no 3, cor. 3 de la prop. 14) que $\Phi$ est fini, donc $\Phi'$ est fini. Soit $a$ un idéal de $A$ tel que $\dim(A/a) < \dim(A)$. Pour tout $p \in \Phi'$, on a $\dim(A/a) < \dim(A/p)$, donc $a \not\subset p$. D’après la prop. 2 de II, § 1, no 1, il existe donc un élément $x$ de $a$ qui n’appartient à aucun des $p \in \Phi'$, et l’on a alors $\dim(A/xA) = \dim(A) - 1$ d’après a). Ceci prouve b).

L’assertion c) est le cas particulier $a = m_A$ de b).

### 2. Dimension et suites sécantes

Soient $A$ un anneau noethérien, $M$ un $A$-module de type fini, $S$ une partie du radical de $A$, $\mathfrak{S}$ l’idéal de $A$ engendré par $S$ et $a$ l’annulateur de $M$. On a

(6)
$$
\dim_A(M) = \dim(A/a) \leq \dim(A) ;
$$
donc, si $A$ est local, on a $\dim_A(M) < + \infty$. Par ailleurs, le support du $A$-module $M/SM$ est égal à $V(a + \mathfrak{S})$ d’après le corollaire de la prop. 18 de II, § 4, no 4, d’où

(7)
$$
\dim_A(M/SM) = \dim(A/(a + \mathfrak{S})) .
$$

Lorsque $S$ est finie, ou que $M$ n’est pas réduit à 0, on a l’inégalité

(8)
$$
\dim_A(M/SM) \leq \dim_A(M) \leq \mathrm{Card}(S) + \dim_A(M/SM) ;
$$
lorsque $S$ est finie, cela résulte de la prop. 2 du no 1 et des formules (6) et (7) ci-dessus, et le cas où $S$ est infinie est trivial.

#### Définition 1 {#ac-viii-s3-def-1 .statement}

Soient $A$ un anneau local noethérien, $M$ un $A$-module non nul de type fini et $S$ une partie de l’idéal maximal $m_A$ de $A$. On dit que $S$ est sécante pour $M$ si l’on a

(9)
$$
\dim_A(M) = \mathrm{Card}(S) + \dim_A(M/SM) .
$$

Si $S$ est sécante pour $M$, on a $\mathrm{Card}(S) \leq \dim_A(M)$, donc $S$ est finie. On dit qu’une famille $(x_i)_{i \in I}$ d’éléments de $m_A$ est sécante pour $M$ si l’on a

(10)
$$
\dim_A(M) = \mathrm{Card}(I) + \dim_A(M/\sum_{i \in I} x_i M) ,
$$
c’est-à-dire si $i \mapsto x_i$ est une bijection de $I$ sur une partie de $m_A$ sécante pour $M$.

On dit qu’un élément x de $m_A$ est sécant pour M si $\{ x \}$ est une partie sécante pour M, c’est-à-dire si l’on a
$$
\dim_A(M/xM) = \dim_A(M) - 1 .
$$

#### Remarque 1 {#ac-viii-s3-n2-rem-1 .statement}

Il résulte des formules (6) et (7) que S est sécante pour M si et seulement si elle est sécante pour $A/\alpha$, où $\alpha$ est l’annulateur de M.
2) Soient S et S’ deux parties disjointes de $m_A$. Pour que $S \cup S'$ soit sécante pour M, il faut et il suffit que S soit sécante pour M et S’ sécante pour $M' = M/SM$. Cela résulte de l’inégalité (8) et de la formule
$$
\text{Card}(S \cup S') + \dim_A(M/(SM + S'M)) - \dim_A(M) =
= (\text{Card}(S) + \dim_A(M/SM) - \dim_A(M)) +
+ (\text{Card}(S') + \dim_A(M'/S'M') - \dim_A(M')) .
$$
3) Soient $x \in m_A$ et $n \geq 1$ un entier. Il est immédiat que les modules $M/xM$ et $M/x^nM$ ont même support, donc même dimension. Par suite, x est sécant pour M si et seulement si $x^n$ est sécant pour M. De là et de la remarque 2, on déduit aussitôt le résultat suivant : soient $x_1, ..., x_r$ des éléments de $m_A$ et $n_1, ..., n_r$ des entiers $> 0$; alors la suite $(x_1, ..., x_r)$ est sécante pour M si et seulement si la suite $(x_1^{n_1}, ..., x_r^{n_r})$ est sécante pour M.

#### Proposition 3 {#ac-viii-s3-prop-3 .statement}

Soient A un anneau local noethérien et M un A-module non nul de type fini. Pour qu’un élément x de $m_A$ soit sécant pour M, il faut et il suffit qu’il n’appartienne à aucun des éléments minimaux $p$ de $\mathrm{Supp}(M)$ tels que $\dim(A/p) = \dim_A(M)$, et il suffit que l’homothétie $x_M$ de rapport x dans M soit injective.
Soit $\alpha$ l’annulateur de M. Dire que x est sécant pour M signifie que x est sécant pour $A/\alpha$, le support de M se compose des idéaux premiers $p$ de A tels que $\alpha \subset p$ et si $x_M$ est injective, l’image de x dans $A/\alpha$ n’est pas diviseur de 0 dans $A/\alpha$. La prop. 3 résulte alors du cor. 2 de la prop. 2 du no 1 appliqué à l’anneau $A/\alpha$.

#### Corollaire {#ac-viii-s3-n2-cor-1 .statement}

Toute suite d’éléments de $m_A$ qui est complètement sécante pour M (A, X, p. 157, déf. 2) est sécante pour M.
Soit $(x_1, ..., x_r)$ une suite d’éléments de $m_A$ qui est complètement sécante pour M. Posons $M_0 = M$ et par récurrence $M_i = M_{i-1}/x_i M_{i-1}$ pour $1 \leq i \leq r$. D’après le cor. 1 de A, X, p. 160, l’homothétie de rapport $x_i$ dans $M_{i-1}$ est injective, d’où $\dim_A(M_i) = \dim_A(M_{i-1}) - 1$ (pour $1 \leq i \leq r$) (prop. 3). On a donc
$$
\dim_A(M) = r + \dim_A(M/(x_1M + \cdots + x_rM)) ,
$$
donc la suite $(x_1, ..., x_r)$ est sécante pour M.

#### Remarque 4 {#ac-viii-s3-n2-rem-4 .statement}

Il n’est pas vrai en général qu’une suite sécante pour M soit complètement sécante pour M (p. 87, exerc. 6). Nous étudierons plus tard les modules sur un anneau local noethérien pour lesquels toute suite sécante est complètement sécante.

#### Théorème 1 {#ac-viii-s3-thm-1 .statement}

Soient $A$ un anneau local noethérien, $M$ un $A$-module non nul de type fini et $S$ une partie de l’idéal maximal $m_A$ de $A$.

a) Si $M/SM$ est de longueur finie, on a $\mathrm{Card}(S) \geqslant \dim_A(M)$; si $S$ est sécante pour $M$, on a $\mathrm{Card}(S) \leqslant \dim_A(M)$.

b) Toute partie sécante pour $M$ est contenue dans une partie sécante pour $M$ maximale.

c) Les propriétés suivantes sont équivalentes :
(i) $S$ est une partie sécante pour $M$ maximale ;
(ii) $S$ est une partie sécante pour $M$ et $\mathrm{Card}(S) = \dim_A(M)$;
(iii) $M/SM$ est de longueur finie et $\mathrm{Card}(S) = \dim_A(M)$;
(iv) $S$ est une partie sécante pour $M$ et $M/SM$ est de longueur finie.

Comme on a $S \subset m_A$, le lemme de Nakayama montre que l’on a $M/SM \neq \{0\}$, d’où $\dim_A(M/SM) \geqslant 0$ avec égalité si et seulement si $M/SM$ est de longueur finie. L’assertion a) résulte alors des formules (8) et (9), ainsi que l’équivalence des propriétés (ii), (iii) et (iv).

L’assertion b) résulte du fait que le cardinal de toute partie de $m_A$ sécante pour $M$ est majorée par l’entier $\dim_A(M)$.

D’après a), toute partie sécante pour $M$, de cardinal égal à $\dim_A(M)$, est maximale. Il reste à prouver que, si $S$ est sécante pour $M$ et si $\mathrm{Card}(S) < \dim_A(M)$, alors $S$ n’est pas maximale. Soient $a$ l’annulateur de $M$, et $B$ l’anneau local noethérien $A/(a + SA)$. D’après le cor. 2 de la prop. 2 du no 1, il existe un élément $x$ de $m_A$ tel que $\dim(B/xB) = \dim(B) - 1$ d’où $x \notin S$. D’après la remarque 2, la partie $S \cup \{x\}$ de $m_A$ est sécante pour $A/a$, donc pour $M$ d’après la remarque 1.

#### Corollaire {#ac-viii-s3-n2-cor-2 .statement}

La dimension de $M$ est le plus petit des entiers $d \geqslant 0$ pour lesquels il existe une suite $(x_1, ..., x_d)$ d’éléments de $m_A$ telle que le $A$-module $M / \sum_{i=1}^d x_i M$ soit de longueur finie.

Comme $\varnothing$ est une partie sécante pour $M$, le th. 1, b) démontre l’existence d’une suite sécante pour $M$ maximale, soit $(x_1, ..., x_d)$. Mais alors on a $d = \dim_A(M)$ et le $A$-module $M / \sum_{i=1}^d x_i M$ est de longueur finie d’après la propriété (iii) du th. 1, c). Réciproquement si $(x'_1, ..., x'_{d'})$ est une suite d’éléments de $m_A$ telle que le $A$-module $M / \sum_{j=1}^{d'} x'_j M$ soit de longueur finie, on a $d' \geqslant \dim_A(M)$ d’après le th. 1, a).

Rappelons (III, § 3, no 2, déf. 1) qu’un idéal $q$ d’un anneau local noethérien $A$ est un idéal de définition de $A$ si les topologies $q$-adique et $m_A$-adique de $A$ coïncident.

#### Lemme 2 {#ac-viii-s3-lem-2 .statement}

Soient $A$ un anneau local noethérien et $q$ un idéal de $A$. Les conditions suivantes sont équivalentes :

(i) $q$ est un idéal de définition de $A$;
(ii) il existe un entier $n \geqslant 0$ tel que $m_A^n \subset q \subset m_A$;

(iii) on a q ≠ A et A/q est un A-module de longueur finie ;
(iv) V(q) est égal à { m_A } (autrement dit, m_A est le seul idéal premier de A contenant q).

En effet, l’équivalence de (i), (ii) et (iv) a été démontrée en III, § 2, n° 5, et l’équivalence de (i) et (iii) résulte de IV, § 2, n° 5, cor. 2 à la prop. 9.

Le corollaire du th. 1 permet donc d’énoncer le scholie suivant :

#### Scholie {#ac-viii-s3-n2-sch-1 .statement}

La dimension d’un anneau local noethérien A est le plus petit des entiers d ≥ 0 pour lesquels il existe un idéal de définition de A engendré par d éléments.

### 3. Premières applications

Soient A un anneau noethérien, V = Spec(A) son spectre. Dans ce numéro, on appelle hypersurface dans V toute partie de la forme $^1 V(x)$ avec $x \in A$.

#### Proposition 4 {#ac-viii-s3-prop-4 .statement}

Soient X une partie fermée de V, et $H_1, ..., H_m$ des hypersurfaces dans V. Posons $X' = X \cap H_1 \cap ... \cap H_m$.

a) Pour toute partie fermée Y de V contenue dans X', on a

$$
\operatorname{codim}(Y, X') \geq \operatorname{codim}(Y, X) - m .
$$

b) On a $\operatorname{codim}(Z, X) \leq m$ pour toute composante irréductible Z de X'. Si X' est non vide, on a $\operatorname{codim}(X', X) \leq m$.

c) Si Z est une partie fermée irréductible de V contenue dans X telle que $\operatorname{codim}(Z, X) \leq m$, il existe des hypersurfaces $H'_1, ..., H'_m$ telles que Z soit une composante irréductible de $X \cap H'_1 \cap ... \cap H'_m$.

Soient α un idéal de A et $x_1, ..., x_m$ des éléments de A tels que $X = V(\alpha)$ et $H_i = V(x_i)$ pour $1 \leq i \leq m$. Soit Z une partie fermée irréductible de V contenue dans X ; il existe un idéal premier p de A contenant α et tel que $Z = V(p)$.

Supposons d’abord que Z soit contenue dans X' et notons $\xi_i$ l’image de $x_i$ dans l’anneau local noethérien $B = A_p/\alpha A_p$. D’après la prop. 7, b) du § 1, n° 3, on a

$$
\operatorname{codim}(Z, X) = \dim(B), \quad \operatorname{codim}(Z, X') = \dim(B/(\xi_1 B + \cdots + \xi_m B)) .
$$

D’après la prop. 2 du n° 1, on a donc

(11)
$$
\operatorname{codim}(Z, X') \geq \operatorname{codim}(Z, X) - m .
$$

Si Z est une composante irréductible de X', on a $\operatorname{codim}(Z, X') = 0$, d’où $\operatorname{codim}(Z, X) \leq m$; ceci prouve b). On prouve a) en prenant dans les deux membres de (11) la borne inférieure sur l’ensemble des composantes irréductibles Z de Y.

1 Rappelons que $V(x)$ se compose des idéaux premiers de A contenant x.

Réciproquement, supposons qu’on ait codim(Z, X) $\leq m$, c’est-à-dire dim(B) $\leq m$. Comme tout élément de $A_p$ est le produit d’un élément inversible de $A_p$ par l’image d’un élément de A, le scholie du n° 2 démontre l’existence d’éléments $x'_1, ..., x'_m$ de A dont les images dans B engendrent un idéal de définition de B. Posons $H'_i = V(x'_i)$ pour $1 \leq i \leq m$. Il est clair que Z est une composante irréductible de $X \cap H'_1 \cap ... \cap H'_m$.

#### Corollaire 1 {#ac-viii-s3-prop-4-cor-1 .statement}

Soit H une hypersurface non vide dans V. La codimension de H dans V est égale à 0 ou 1.

On a codim(H, V) = 1 si et seulement si H ne contient aucune composante irréductible de V. S’il en est ainsi, toutes les composantes irréductibles de H sont de codimension 1 dans V.

Pour toute composante irréductible Z de H, on a

$$
0 \leq \operatorname{codim}(Z, V) \leq 1
$$

d’après la prop. 4, b), et l’on a codim(Z, V) = 0 si et seulement si Z est une composante irréductible de V. On a par définition

$$
\operatorname{codim}(H, V) = \inf_Z \operatorname{codim}(Z, V)
$$

où Z parcourt l’ensemble des composantes irréductibles de H. Le cor. 1 résulte aussitôt de ces remarques.

#### Corollaire 2 {#ac-viii-s3-prop-4-cor-2 .statement}

Soient X une partie fermée irréductible de V et H une hypersurface dans V. Trois cas seulement sont possibles :

1) on a $X \subset H$;
2) l’ensemble $X \cap H$ est non vide et chacune de ses composantes irréductibles Z satisfait à $\operatorname{codim}(Z, X) = 1$;
3) l’ensemble $X \cap H$ est vide.

Supposons $X' = X \cap H$ non vide et distinct de X ; toute composante irréductible Z de $X'$ est distincte de X et satisfait à $\operatorname{codim}(Z, X) \leq 1$ d’après la prop. 4, b). Le cor. 2 résulte aussitôt de là.

#### Corollaire 3 {#ac-viii-s3-prop-4-cor-3 .statement}

Si A est factoriel (VII, § 3, n° 3, prop. 2), les idéaux premiers de hauteur 1 de A sont les idéaux principaux engendrés par les éléments extrémaux de A. Si de plus A est local, on a $\dim(A/p) = \dim(A) - 1$ pour tout idéal premier $p$ de hauteur 1 de A.

Soit x un élément extrémal de A. Alors Ax est un idéal premier car x est extrémal, de hauteur 1 car A est intègre (n° 1, prop. 1). Soit p un idéal premier de hauteur 1 de A. Alors $V(p)$ est une composante irréductible d’une hypersurface $V(Ax)$ pour un x convenable (prop. 4, c)). Soit $x = \prod_i y_i^{n_i}$ une décomposition de x en produits d’éléments extrémaux tels que $y_i$ et $y_j$ soient étrangers si $i \neq j$. Les composantes irréductibles de $V(Ax)$ sont les $V(Ay_i)$. Donc $p = Ay_i$ pour un i convenable. La dernière assertion résulte du cor. 2 à la prop. 2 du n° 1.

#### Remarque 1 {#ac-viii-s3-n3-rem-1 .statement}

Supposons que A soit un anneau local, noethérien et intègre de dimension d ; soit x un élément non nul de m_A et soit H = V(x). D’après le cor. 2 de la prop. 4, toute composante irréductible de H est de codimension 1 dans X, donc de dimension $\leq d - 1$ ($§ 1$, no 2, prop. 3). D’après le cor. 2 de la prop. 2 du no 1, H est de dimension $d - 1$ et l’une de ces composantes est donc de dimension $d - 1$; toutes le sont si A est caténaire. Cependant, il se peut en général qu’il existe une composante irréductible de H de dimension < $d - 1$ (cf. p. 87, exerc. 7).

#### Remarque 2 {#ac-viii-s3-n3-rem-2 .statement}

Soient $x_1, ..., x_n$ des éléments de A, et posons $H_i = V(x_i)$ pour $1 \leq i \leq n$. Supposons qu’il existe un A-module M de type fini de support $V = \mathrm{Spec}(A)$, tel que $(x_1, ..., x_n)$ soit une suite complètement sécante pour M. Alors toute composante irréductible de $H_1 \cap ... \cap H_n$ est de codimension n dans V : cela résulte facilement du corollaire de la prop. 3 du no 2.

#### Remarque 3 {#ac-viii-s3-n3-rem-3 .statement}

Si l’idéal $\alpha$ de l’anneau noethérien A est engendré par m éléments, on a $\mathrm{ht}(\alpha) \leq m$. Cela résulte aussitôt de la prop. 4.

#### Proposition 5 {#ac-viii-s3-prop-5 .statement}

Soient A un anneau noethérien et $p \subset q$ une chaîne non saturée d’idéaux premiers de A. L’ensemble E des idéaux premiers r de A tels que $p \subset r \subset q$ soit une chaîne est infini. On a $\bigcup_{r \in E} r = q$ et $\bigcap_{r \in E} r = p$.

Quitte à remplacer A par $A/p$, on se ramène au cas où $p = \{0\}$.

D’après le lemme 1 du no 1, on a $q = \bigcup_{r \in E} r$, et la prop. 2 de II, $§ 1$, no 1 montre que E est infini.

Soit $y \neq 0$ un élément de $\bigcap_{r \in E} r$. La hauteur de q est finie (no 1, cor. 1 de la prop. 2), et l’on a $\mathrm{ht}(q) \geq 2$ par hypothèse. Il existe donc un idéal premier $q' \subset q$ de hauteur 2. La première partie de la démonstration appliquée à $q'$ montre que l’ensemble E’ des idéaux premiers de hauteur 1 contenus dans $q'$ est infini ; chacun de ces idéaux contient y par hypothèse. Or l’anneau local noethérien $B = A_{q'}/yA_{q'}$ est de dimension 1 d’après le cor. 2 de la prop. 2 du no 1. Pour tout $r \in E'$, l’idéal premier $r/yA_{q'}$ de B est donc minimal ; par suite, l’anneau noethérien B a une infinité d’idéaux premiers minimaux, ce qui est absurde (II, $§ 4$, no 3, cor. 3 de la prop. 14). On a donc $\bigcap_{r \in E} r = \{0\}$.

#### Proposition 6 {#ac-viii-s3-prop-6 .statement}

Soient A un anneau noethérien de dimension $\geq 2$, et h un entier tel que $0 < h < \dim(A)$.

a) A possède une infinité d’idéaux premiers de hauteur h.

b) Si A est de dimension finie, il possède une infinité d’idéaux premiers p tels que $\mathrm{ht}(p) = h$ et $\dim(A/p) = \dim(A) - h$.

Comme la dimension de A est la borne supérieure des hauteurs des idéaux premiers de A ($§ 1$, no 3, prop. 8), que tout idéal premier de A est de hauteur finie (no 1, cor. 1 de la prop. 2) et que $h < \dim(A)$, il existe un entier $n > h$ et un idéal premier p de hauteur n, donc une chaîne $p_0 \subset ... \subset p_n = p$ d’idéaux premiers de longueur n. On a $\mathrm{ht}(p_i) = i$ pour $0 \leq i \leq n$, d’où $\mathrm{ht}(r) = h$ pour tout idéal premier r de A tel que $p_{h-1} \subset r \subset p_{h+1}$ soit une chaîne. L’ensemble E de ces idéaux est infini d’après la prop. 5, d’où a).

Si $A$ est de dimension finie, on peut supposer qu’on a $n = \dim(A)$ dans ce qui précède. Pour tout idéal $r \in E$, on a $\mathrm{ht}(r) = h$, d’où $\dim(A/r) \leq n - h$, et comme $r \subset p_{h+1} \subset ... \subset p_n$ est une chaîne de longueur $n - h$, on a $\dim(A/r) = n - h$.

Il existe des anneaux intègres non noethériens de dimension 2 ne possédant qu’un seul idéal premier de hauteur 1, par exemple l’anneau d’une valuation de hauteur 2 (VI, § 4, no 4, prop. 5).

### 4. Changements d’anneaux

#### Proposition 7 {#ac-viii-s3-prop-7 .statement}

Soient $\rho : A \to B$ un homomorphisme local d’anneaux locaux noethériens, $M$ un $A$-module de type fini et $N$ un $B$-module de type fini. Posons $\overline{B} = B \otimes_A \kappa_A = B/\rho(m_A).B$ et $\overline{N} = N \otimes_B \overline{B} = N/\rho(m_A).N$. On a

$$
\dim_B(M \otimes_A N) \leq \dim_A(M) + \dim_B(\overline{N}),
$$

et il y a égalité si $N$ est plat sur $A$.

On peut supposer $M$ et $N$ non nuls. D’après le corollaire du th. 1 (no 2), il existe une partie $S$ (resp. $T$) de $m_A$ (resp. $m_B$) telle que $\mathrm{Card}(S) = \dim_A(M)$ (resp. $\mathrm{Card}(T) = \dim_{\overline{B}}(\overline{N})$) et que $M/SM$ soit un $A$-module de longueur finie (resp. $\overline{N}/T\overline{N}$ soit un $B$-module de longueur finie). On a $\rho(S) \subset m_B$. Soit $E$ le $B$-module $M \otimes_A N$; le $B$-module $E/(\rho(S).E + T.E)$ est isomorphe à $M/SM \otimes_A N/TN$, donc est de longueur finie : d’après les prop. 18 et 19 de II, § 4, no 4, on a

$$
\begin{align*}
\mathrm{Supp}(M/SM \otimes_A N/TN) &= \mathrm{Supp}(N/TN) \cap {}^a\rho^{-1}(\mathrm{Supp}(M/SM)) \\
&= \mathrm{Supp}(N/TN) \cap {}^a\rho^{-1}(\mathrm{Supp}(\kappa_A)) \\
&= \mathrm{Supp}(N/TN \otimes_A \kappa_A) = \mathrm{Supp}(\overline{N}/T\overline{N}) = \{m_B\}.
\end{align*}
$$

Il en résulte, d’après le th. 1, que l’on a l’inégalité

$$
\dim_B(E) \leq \mathrm{Card}(S) + \mathrm{Card}(T) = \dim_A(M) + \dim_{\overline{B}}(\overline{N}).
$$

Supposons maintenant $N$ plat sur $A$, et montrons qu’il y a égalité dans la formule (12). Soit $a$ (resp. $b$) l’annulateur de $M$ (resp. $N$). D’après les prop. 18 et 19 de II, § 4, no 4, on a

$$
\begin{align*}
\mathrm{Supp}(E) &= \mathrm{Supp}(N) \cap {}^a\rho^{-1}(\mathrm{Supp}(M)) \\
&= V(b) \cap {}^a\rho^{-1}(V(a)) = V(b + \rho(a).B).
\end{align*}
$$

On a par suite

$$
\dim_B(M \otimes_A N) = \dim(B/(b + \rho(a).B))
$$

et aussi

$$
\dim_A(M) + \dim_{\overline{B}}(\overline{N}) = \dim(A/a) + \dim(B/(b + \rho(m_A).B)).
$$

$$
\dim(B') \geq \dim(A') + \dim(B'/\rho'(\mathfrak{m}_{A'}).B')
$$

et comme l’anneau $B'/\rho'(\mathfrak{m}_{A'}).B'$ est isomorphe à $B/(b + \rho(\mathfrak{m}_A).B)$, notre assertion résulte des formules (13), (14) et (15).

#### Corollaire 1 {#ac-viii-s3-prop-7-cor-1 .statement}

*Soit $\rho : A \to B$ un homomorphisme local d’anneaux locaux noethériens.*

*a)* *On a*

$$
\dim(B) \leq \dim(A) + \dim(B \otimes_A \kappa_A)
$$

*avec égalité si $\rho$ fait de $B$ un $A$-module plat.*

*b)* *Supposons que $\rho$ fasse de $B$ un $A$-module plat, et soit $S$ une partie de $\mathfrak{m}_A$. Alors $S$ est sécante pour $A$ si et seulement si $\rho(S)$ est sécante pour $B$.*

L’assertion *a)* est le cas particulier $M = A, N = B$ de la prop. 7.
Prouvons *b)*. Sous les hypothèses faites, on a

$$
\dim(B) = \dim(A) + \dim(\overline{B})
$$

avec $\overline{B} = B \otimes_A \kappa_A = B/\rho(\mathfrak{m}_A).B$. Comme $\rho$ est injectif (I, § 3, no 5, prop. 9), on a

$$
\mathrm{Card}(\rho(S)) = \mathrm{Card}(S).
$$

Enfin $B' = B/\rho(S).B$ est un module plat sur $A' = A/SA$, d’où

$$
\dim(B/\rho(S).B) = \dim(A/SA) + \dim(\overline{B})
$$

car $B'/\rho(\mathfrak{m}_{A'}).B'$ est isomorphe à $\overline{B}$. Notre assertion résulte aussitôt des formules (17), (18) et (19).

#### Corollaire 2 {#ac-viii-s3-prop-7-cor-2 .statement}

*Soit $\rho : A \to B$ un homomorphisme d’anneaux noethériens. On a*

$$
\dim(B) \leq \dim(A) + \sup_{p \in \mathrm{Spec}(A)} \dim(B \otimes_A \kappa(p)).
$$

Soient $q$ un idéal premier de $B$ et $p = \rho^{-1}(q)$. D’après le cor. 1, on a $\dim(B_q) \leq \dim(A_p) + \dim(B_q \otimes_A \kappa(p))$. On en déduit (prop. 6, *b*) du § 1, no 3) l’inégalité $\dim(B_q) \leq \dim(A) + \dim(B \otimes_A \kappa(p))$, et on conclut par la prop. 8 du § 1, no 3.

#### Corollaire 3 {#ac-viii-s3-prop-7-cor-3 .statement}

Soient $A$ un anneau noethérien et $n$ un entier $\geqslant 0$. On a

$$
\dim(A[X_1, ..., X_n]) = \dim(A) + n .
$$

Posons $B = A[X_1, ..., X_n]$. Pour tout idéal premier $p$ de $A$, l’anneau $B \otimes_A \kappa(p)$ est un anneau de polynômes à $n$ variables sur un corps, donc est de dimension $n$ ($§ 2$, no 4, cor. 1 au th. 3). D’après le cor. 2, on a $\dim(B) \leqslant \dim(A) + n$; l’inégalité inverse résulte de l’exemple 4 du $§ 1$, no 3.

#### Corollaire 4 {#ac-viii-s3-prop-7-cor-4 .statement}

Soient $\rho : A \to B$ un homomorphisme d’anneaux noethériens, et $a$ un idéal de $A$. On a l’inégalité

$$
\text{ht}(\rho(a).B) \leqslant \text{ht}(a)
$$

si l’application $^a\rho : \mathrm{Spec}(B) \to \mathrm{Spec}(A)$ est surjective. Si $B$ est un $A$-module fidèlement plat, on a $\text{ht}(\rho(a).B) = \text{ht}(a)$.

Si $B$ est fidèlement plat sur $A$, alors $^a\rho$ est surjective (II, $§ 2$, no 5, cor. 4 à la prop. 11) et l’on a $\text{ht}(a) \leqslant \text{ht}(\rho(a).B)$ ($§ 2$, no 1, corollaire de la prop. 2).

Il reste donc à prouver l’inégalité (20) sous l’hypothèse que $^a\rho$ est surjective. Soit $p$ un idéal premier de $A$ tel que $a \subset p$ et $\text{ht}(a) = \text{ht}(p)$ ($§ 1$, no 3, prop. 7). Posons $\overline{B} = B \otimes_A \kappa(p)$ et notons $h$ l’homomorphisme canonique de $B$ dans $\overline{B}$. Si $X = {}^a\rho^{-1}(p)$ est l’ensemble non vide des idéaux premiers de $B$ au-dessus de $p$, on sait ($§ 2$, no 1, lemme 1) que l’application $^ah$ est un homéomorphisme de $\mathrm{Spec}(\overline{B})$ sur le sous-espace $X$ de $\mathrm{Spec}(B)$. Soit $q$ l’image par $^ah$ d’un idéal premier minimal de $\overline{B}$; on a $\dim(B_q \otimes_A \kappa(p)) = 0$ et le cor. 1 entraîne l’inégalité $\dim(B_q) \leqslant \dim(A_p) = \text{ht}(p) = \text{ht}(a)$, finalement

$$
\text{ht}(\rho(a).B) \leqslant \text{ht}(q) = \dim(B_q) \leqslant \dim(A_p) = \text{ht}(p) = \text{ht}(a),
$$

d’où le corollaire.

#### Proposition 8 {#ac-viii-s3-prop-8 .statement}

Soient $A$ un anneau noethérien, $a$ un idéal de $A$, $M$ un $A$-module de type fini, $\hat{A}$ et $\hat{M}$ les séparés complétés de $A$ et $M$ respectivement pour la topologie $a$-adique.

a) Soient $m$ un idéal premier de $A$ contenant $a$ et $\hat{m} = m\hat{A}$. Alors $\hat{m}$ est un idéal premier de $\hat{A}$ et on a $\dim_{\hat{A}_{\hat{m}}}(\hat{M}_{\hat{m}}) = \dim_{A_m}(M_m)$.

b) On a $\dim_{\hat{A}}(\hat{M}) = \sup_m \dim_{A_m}(M_m)$, où $m$ parcourt l’ensemble des idéaux premiers (resp. maximaux) de $A$ contenant $a$. En particulier, on a $\dim_{\hat{A}}(\hat{M}) \leqslant \dim_A(M)$.

a) Puisque $\hat{A}/\hat{m}$ s’identifie à $A/m$, $\hat{m}$ est un idéal premier de $\hat{A}$. D’après le th. 3 de III, $§ 3$, no 4, $\hat{A}$ est plat sur $A$, donc $\hat{A}_{\hat{m}}$ est plat sur $A_m$. Par ailleurs l’application canonique de $A$ dans $\hat{A}$ induit un isomorphisme de $A/a$ sur $\hat{A}/a\hat{A}$, donc aussi un isomorphisme de $A_m/mA_m$ sur $\hat{A}_{\hat{m}}/m\hat{A}_{\hat{m}}$. On conclut en appliquant la prop. 7 aux anneaux $A_m$ et $\hat{A}_{\hat{m}}$ et aux modules $M_m$ et $\hat{A}_{\hat{m}}$ car $M_m \otimes_{A_m} \hat{A}_{\hat{m}}$ est isomorphe à $\hat{M}_{\hat{m}}$ (III, loc. cit. et prop. 8).

b) D’après la prop. 8 de III, $§ 3$, no 4, l’application $m \mapsto \hat{m}$ est une bijection de l’ensemble des idéaux maximaux de $A$ contenant $a$ sur l’ensemble des idéaux maximaux de $\hat{A}$. L’assertion b) résulte de là et de la prop. 9 du $§ 1$, no 4.

#### Corollaire 1 {#ac-viii-s3-prop-8-cor-1 .statement}

Soit $A$ un anneau de Zariski (III, $§ 3$, no 3, déf. 2). Pour tout $A$-module $M$ de type fini, on a $\dim_{\hat{A}}(\hat{M}) = \dim_A(M)$.

En effet, la topologie de $A$ est la topologie $a$-adique, où $a$ est un idéal contenu dans le radical de $A$ (*loc. cit.*), c’est-à-dire contenu dans tout idéal maximal $m$ de $A$. Il suffit donc d’appliquer l’assertion b) de la prop. 8.

#### Corollaire 2 {#ac-viii-s3-prop-8-cor-2 .statement}

Soient $A$ un anneau noethérien, $a$ un idéal de $A$, et $\hat{A}$ le séparé complété de $A$ pour la topologie $a$-adique. On a $\dim(\hat{A}) \leqslant \dim(A)$, avec égalité lorsque $A$ est local et $a$ distinct de $A$.

#### Corollaire 3 {#ac-viii-s3-prop-8-cor-3 .statement}

Soient $A$ un anneau noethérien et $n$ un entier $\geqslant 0$. On a

$$
\dim(A[[X_1, ..., X_n]]) = \dim(A) + n .
$$

L’anneau $A[[X_1, ..., X_n]]$ est le séparé complété de l’anneau de polynômes $A[X_1, ..., X_n]$ pour la topologie $a$-adique, où $a$ est l’idéal engendré par $X_1, ..., X_n$; on a donc

$$
\dim(A[[X_1, ..., X_n]]) \leqslant \dim(A[X_1, ..., X_n])
$$

d’après le cor. 2. On a par ailleurs

$$
\dim(A[X_1, ..., X_n]) = \dim(A) + n
$$

d’après le cor. 3 de la prop. 7. Enfin, on a

$$
\dim(A) + n \leqslant \dim(A[[X_1, ..., X_n]])
$$

d’après l’exemple 4 du $§ 1$, no 3.

#### Remarque 1 {#ac-viii-s3-n4-rem-1 .statement}

Soient $A$ un anneau noethérien et $a$ un idéal de $A$. Supposons $A$ séparé et complet pour la topologie $a$-adique, et considérons l’anneau $R = A \{ X_1, ..., X_n \}$ des séries formelles restreintes (III, $§ 4$, no 2, déf. 2). On a $\dim(R) = \dim(A) + n$. En effet, $R$ est le complété de l’anneau $B = A[X_1, ..., X_n]$ pour la topologie $aB$-adique, d’où $\dim(R) \leqslant \dim(A[X_1, ..., X_n]) = \dim(A) + n$. L’inégalité inverse se démontre comme dans le cas des séries formelles.

#### Remarque 2 {#ac-viii-s3-n4-rem-2 .statement}

Soient $A$ un anneau local noethérien, identifié à un sous-anneau de son complété $\hat{A}$, et $B$ un sous-anneau de $\hat{A}$ contenant $A$. Supposons que $B$ soit local noethérien et que l’on ait $m_A B = m_B$. Alors, l’injection canonique de $A$ dans $B$ s’étend en un isomorphisme de $\hat{A}$ sur le complété $\hat{B}$ de $B$ (III, $§ 3$, no 5, prop. 11), d’où $\dim(B) = \dim(A)$ (cor. 2 à la prop. 8). Ceci s’applique notamment à la situation suivante. \* Soient $k$ un corps valué complet non discret, $A$ l’anneau local de l’anneau de polynômes $k[X_1, ..., X_n]$ en l’idéal premier engendré par $X_1, ..., X_n$, et $B$ l’anneau des séries convergentes en $X_1, ..., X_n$ à coefficients dans $k$. Alors les hypothèses précédentes sont satisfaites, et par conséquent on a $\dim(B) = n$.*

### 5. Construction de suites sécantes

#### Proposition 9 {#ac-viii-s3-prop-9 .statement}

Soient $A$ un anneau noethérien, $M$ un $A$-module de type fini, $a$ une partie de $A$ stable par addition et multiplication, $q_1, ..., q_m$ des idéaux premiers de $A$ ne contenant pas $a$ et $r \geq 1$ un entier tel que

$$
\text{codim}(V(a) \cap \operatorname{Supp}(M), \operatorname{Supp}(M)) \geq r .
$$

Il existe une suite $(x_1, ..., x_r)$ d’éléments de $a$, n’appartenant à aucun des idéaux $q_1, ..., q_m$ et telle que la suite $(x_1/1, ..., x_r/1)$ d’éléments de $A_p$ soit sécante pour le $A_p$-module $M_p$, quel que soit l’idéal premier $p \in V(a) \cap \operatorname{Supp}(M)$.

Raisonnons par récurrence sur $r$. Supposons d’abord $r = 1$, et notons $\Phi$ l’ensemble (fini) des éléments minimaux de $\operatorname{Supp}(M)$. Raisonnons par l’absurde et supposons qu’il n’existe aucun élément $x_1$ de $a$ satisfaisant aux conditions de l’énoncé. Soit $x \in a$, n’appartenant pas à $q_1 \cup ... \cup q_m$. Il existe par hypothèse un élément $p$ de $V(a) \cap \operatorname{Supp}(M)$ tel que l’image $x/1$ de $x$ dans $A_p$ ne soit pas sécante pour $M_p$. Soit $\Psi$ l’ensemble des idéaux $q \in \Phi$ contenus dans $p$; alors les éléments minimaux de $\operatorname{Supp}(M_p)$ sont les idéaux premiers $qA_p$ de $A_p$, où $q$ parcourt $\Psi$. D’après la prop. 3 du n° 2, il existe donc un élément $q$ de $\Psi$ tel que $x/1 \in qA_p$, d’où $x \in q$. Autrement dit, on a $a \subset q_1 \cup ... \cup q_m \cup \bigcup_{q \in \Phi} q$. Comme on a $a \not\subset q_j$ pour $1 \leq j \leq m$, la prop. 2 de II, § 1, n° 1 démontre l’existence d’un élément $q$ de $\Phi$ contenant $a$, d’où

$$
V(q) \subset V(a) \cap \operatorname{Supp}(M) .
$$

Comme $V(a)$ contient une composante irréductible de $\operatorname{Supp}(M)$, ceci contredit l’hypothèse

$$
\text{codim}(V(a) \cap \operatorname{Supp}(M), \operatorname{Supp}(M)) \geq 1 .
$$

Supposons maintenant $r \geq 2$. D’après l’hypothèse de récurrence, on peut trouver une suite $(x_1, ..., x_{r-1})$ d’éléments de $a$, n’appartenant pas à $q_1 \cup ... \cup q_m$ et telle que, pour tout $p \in V(a) \cap \operatorname{Supp}(M)$, la suite $(x_1/1, ..., x_{r-1}/1)$ d’éléments de $A_p$ soit sécante pour $M_p$. Posons $N = M / \sum_{i=1}^{r-1} x_i M$. Il suffit de construire un élément $x_r$ de $a$ n’appartenant pas à $q_1 \cup ... \cup q_m$ et tel que, pour tout $p \in V(a) \cap \operatorname{Supp}(M)$, l’élément $x_r/1$ de $A_p$ soit sécant pour $N_p$. D’après la première partie de la démonstration, il suffit d’établir les deux relations

$$
V(a) \cap \operatorname{Supp}(M) = V(a) \cap \operatorname{Supp}(N) ,
$$
$$
\text{codim}(V(a) \cap \operatorname{Supp}(N), \operatorname{Supp}(N)) \geq 1 .
$$

Or on a

$$
\operatorname{Supp}(N) = V(x_1) \cap ... \cap V(x_{r-1}) \cap \operatorname{Supp}(M)
$$

$$
m = r - 1,\quad X = \operatorname{Supp}(M),\quad Y = V(\alpha) \cap \operatorname{Supp}(N),\quad H_i = V(x_i)
$$

d’où $X' = \operatorname{Supp}(N)$.

#### Corollaire 1 {#ac-viii-s3-prop-9-cor-1 .statement}

*Soient A un anneau noethérien, M un A-module de type fini, $p_1, ..., p_n, q_1, ..., q_m$ des idéaux premiers de A et r un entier $\geqslant 1$. On suppose qu’on a $p_i \not\subset q_j$ pour $1 \leqslant i \leqslant n$ et $1 \leqslant j \leqslant m$, et $\dim_{A_{p_i}}(M_{p_i}) \geqslant r$ pour $1 \leqslant i \leqslant n$. Il existe alors une suite $(x_1, ..., x_r)$ d’éléments de A appartenant à tous les $p_i$ et n’appartenant à aucun des $q_j$, telle que, pour $1 \leqslant i \leqslant n$, les images de $x_1, ..., x_r$ dans $A_{p_i}$ forment une suite sécante pour le module $M_{p_i}$.

Posons $\alpha = \bigcap_i p_i$. On a $M_{p_i} \neq \{0\}$, donc $p_i \in \operatorname{Supp}(M)$ pour $1 \leqslant i \leqslant n$, d’où $V(\alpha) \subset \operatorname{Supp}(M)$. On a

$$
\operatorname{codim}(V(\alpha) \cap \operatorname{Supp}(M), \operatorname{Supp}(M)) = \operatorname{codim}(V(\alpha), \operatorname{Supp}(M)) =
= \inf_i (\operatorname{codim}(V(p_i), \operatorname{Supp}(M))) = \inf_i \dim(M_{p_i}) \geqslant r
$$

(§ 1, n° 4, prop. 9), et l’on applique la prop. 9.

#### Corollaire 2 {#ac-viii-s3-prop-9-cor-2 .statement}

*Soient A un anneau local noethérien, M un A-module non nul de type fini et $\alpha$ une partie de $m_A$, stable par addition et multiplication et telle que $\operatorname{long}(M/\alpha M) < +\infty$. Il existe une partie de $\alpha$ qui est sécante maximale pour M.*

En effet, on a $V(\alpha) \cap \operatorname{Supp}(M) = \operatorname{Supp}(M/\alpha M) = \{m_A\}$ (§ 1, n° 4, remarque 1), donc $\operatorname{codim}(V(\alpha) \cap \operatorname{Supp}(M), \operatorname{Supp}(M)) = \dim(\operatorname{Supp}(M)) = \dim_A(M)$, et on applique la prop. 9.

## EXERCICES {#ac-viii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
