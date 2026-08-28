---
book: ac
book_title: Commutative Algebra
chapter: IV
chapter_title: Idéaux premiers associés et décomposition primaire
section: 2
section_title: Décomposition primaire
lang: fr
source: ac-i-iv-fr
pdf_pages: 0313-0332, 0341-0351
extraction: ocr
subsections:
    - "no": 1
      title: Sous-modules primaires.
      page: 0
      pdf_page: 313
    - "no": 2
      title: Existence d’une décomposition primaire.
      page: 0
      pdf_page: 316
    - "no": 3
      title: Propriétés d'unicité dans la décomposition primaire.
      page: 0
      pdf_page: 317
    - "no": 4
      title: Localisation d'une décomposition primaire.
      page: 0
      pdf_page: 320
    - "no": 5
      title: Anneaux et modules de longueur finie.
      page: 0
      pdf_page: 321
    - "no": 6
      title: Décomposition primaire et extension des scalaires.
      page: 0
      pdf_page: 328
statements: 46
exercises: 35
content_sha256: 4ea40e4021993533ff69b55389fb0ebd11745db620820620f573e2bc08e81f83
---

## § 2. Décomposition primaire.

### 1. Sous-modules primaires.

#### Proposition 1 {#ac-iv-s2-prop-1 .statement}

Soient $A$ un anneau noethérien et $M$ un $A$-module.

Les conditions suivantes sont équivalentes :
a) $\mathrm{Ass}(M)$ est réduit à un seul élément.
b) On a $M \neq 0$, et toute homothétie de $M$ est, soit injective, soit presque nilpotente (§ 1, n° 4).

Si ces conditions sont remplies, et si $p$ est l'ensemble des $a \in A$ tels que l'homothétie $a_M$ soit presque nilpotente, on a $\mathrm{Ass}(M) = \{ p \}$.

Ceci résulte aussitôt du § 1, n° 4, cor. de la prop. 9 et n° 1, cor. 2 de la prop. 2.

#### Définition 1 {#ac-iv-s2-def-1 .statement}

Soient $A$ un anneau noethérien, $N$ un $A$-module, $Q$ un sous-module de $N$. Si le module $M = N/Q$ satisfait aux conditions de la prop. 1, on dit que Q est p-primaire par rapport à N (ou dans N).

Lorsque aucune confusion n’en résulte, on dit simplement que Q est « p-primaire » ou « primaire » ; il est clair que pour tout sous-module N' $\neq Q$ de N contenant Q, Q est p-primaire dans N'.

La définition 1 s’applique en particulier au cas N = A ; les sous-modules de N sont alors les idéaux de A, et on dit donc qu’un idéal q de A est primaire si Ass(A/q) a un seul élément, ou, ce qui revient au même, si A $\neq q$ et si tout diviseur de zéro dans l’anneau A/q est nilpotent. Si q est p-primaire, il résulte de la déf. 1 que p est la racine (chap. II, § 2, no 6) de l’idéal q.

#### Remarque {#ac-iv-s2-n1-rem-1 .statement}

Soit Q un sous-module p-primaire d’un A-module N. Si N/Q est de type fini, il existe un entier k > 0 tel que $p^k N \subset Q$, en vertu du § 1, no 4, prop. 9.

#### Exemple 1 {#ac-iv-s2-n1-exa-1 .statement}

Si p est un idéal premier de A, p est p-primaire (§ 1, no 1, prop. 1).

#### Exemple 2 {#ac-iv-s2-n1-exa-2 .statement}

Soit q un idéal de A tel qu’il existe un seul idéal premier m (nécessairement maximal) contenant q ; alors, si M est un A-module tel que qM $\neq M$, qM est m-primaire par rapport à M. En effet, tout élément de Ass(M/qM) contient q, donc est égal à m, et on a Ass(M/qM) $\neq \varnothing$ (§ 1, no 1, cor. 1 de la prop. 2). En particulier q est un idéal m-primaire dans A.

#### Exemple 3 {#ac-iv-s2-n1-exa-3 .statement}

Soit m un idéal maximal de A ; les idéaux m-primaires sont alors les idéaux q de A pour lesquels il existe un entier n $\geq 1$ tel que $m^n \subset q \subset m$. En effet, si $m^n \subset q \subset m$, m est le seul idéal premier contenant q (chap. II, § 1, no 1, cor. de la prop. 1), et la conclusion résulte de l’Exemple 2 ; réciproquement, si q est m-primaire, m est la racine de q, et il existe donc n $\geq 1$ tel que $m^n \subset q$ (chap. II, § 2, no 6, prop. 15).

#### Exemple 4 {#ac-iv-s2-n1-exa-4 .statement}

Dans un anneau principal A, les idéaux primaires sont (0) et les idéaux de la forme Ap^n, où p est un élément extrémal et n $\geq 1$ ; cela résulte aussitôt de l’Exemple 3.

#### Exemple 5 {#ac-iv-s2-n1-exa-5 .statement}

Les puissances d’un idéal premier quelconque ne sont pas nécessairement des idéaux primaires (exerc. 1). D’autre part, il existe des idéaux primaires qui ne sont pas des puissances d’idéaux premiers (exerc. 1).

#### Proposition 2 {#ac-iv-s2-prop-2 .statement}

Soient M un module sur un anneau noethérien A, p un idéal premier de A, et (Q_i)_{i \in I} une famille finie non vide de sous-modules de M, p-primaires par rapport à M. Alors $\bigcap_{i \in I} Q_i$ est p-primaire par rapport à M.

En effet, $M / (\bigcap_{i \in I} Q_i)$ est isomorphe à un sous-module $\neq 0$ de la somme directe $\bigoplus_{i \in I} (M / Q_i)$. Or, on a

$$
\operatorname{Ass} \left( \bigoplus_{i \in I} (M / Q_i) \right) = \bigcup_{i \in I} \operatorname{Ass}(M / Q_i) = \{ p \}
$$

(§ 1, n° 1, cor. 1 de la prop. 3.) Donc $\operatorname{Ass} \left( M / (\bigcap_{i \in I} Q_i) \right) = \{ p \}$
(§ 1, n° 1, prop. 3 et cor. 1 de la prop. 2).

#### Proposition 3 {#ac-iv-s2-prop-3 .statement}

Soient A un anneau noethérien, S une partie multiplicative de A, p un idéal premier de A, M un A-module, N un sous-module de M, et $i = i_M^S$ l’application canonique de M dans $S^{-1}M$.

(i) On suppose que $p \cap S \neq \varnothing$. Si N est p-primaire par rapport à M, on a $S^{-1}N = S^{-1}M$.

(ii) On suppose que $p \cap S = \varnothing$. Pour que N soit p-primaire par rapport à M, il faut et il suffit que N soit de la forme $i(N')$, où $N'$ est un sous-$S^{-1}A$-module de $S^{-1}M$, $(S^{-1}p)$-primaire par rapport à $S^{-1}M$; on a alors $N' = S^{-1}N$.

(i) Si $p \cap S \neq \varnothing$, et si N est p-primaire par rapport à M, on a $\operatorname{Ass}_{S^{-1}A}(S^{-1}(M/N)) = \varnothing$ (§ 1, n° 2, cor. de la prop. 5), donc $S^{-1}(M/N) = 0$ (§ 1, n° 1, cor. 1 de la prop. 2), d’où $S^{-1}M / S^{-1}N = 0$.

(ii) Supposons $p \cap S = \varnothing$. Si N est p-primaire par rapport à M, on a $\operatorname{Ass}_{S^{-1}A}(S^{-1}(M/N)) = \{ S^{-1}p \}$ (§ 1, n° 2, cor. de la prop. 5), donc le sous-module $N' = S^{-1}N$ de $S^{-1}M$ est $(S^{-1}p)$-primaire ; en outre, si $s \in S$ et $m \in M$ sont tels que $sm \in N$, on a $m \in N$, car l’homothétie de rapport s dans $M/N$ est injective, d’où $N = i(N')$ (chap. II, § 2, n° 4, prop. 10). Réciproquement, soit $N'$ un sous-module de $S^{-1}M$, $(S^{-1}p)$-primaire par rapport à $S^{-1}M$; posons $N = i^{-1}(N')$; on a $N' = S^{-1}N$ (chap. II, § 2, no 4, prop. 10) et $\mathrm{Ass}_{S^{-1}A}(S^{-1}(M/N)) = \mathrm{Ass}_{S^{-1}A}((S^{-1}M)/N') = \{ S^{-1}p \}$. Comme l’application canonique $M/N \to S^{-1}(M/N)$ est injective, aucun idéal premier de $A$ associé à $M/N$ ne rencontre $S$ ($§ 1$, no 2, prop. 6); il en résulte que $\mathrm{Ass}(M/N) = \{ p \}$ ($§ 1$, no 2, cor. de la prop. 5), de sorte que $N$ est $p$-primaire par rapport à $M$.

### 2. Existence d’une décomposition primaire.

#### Définition 2 {#ac-iv-s2-def-2 .statement}

Soient $A$ un anneau noethérien, $M$ un $A$-module, $N$ un sous-module de $M$. On appelle décomposition primaire de $N$ dans $M$ une famille finie $(Q_i)_{i \in I}$ de sous-modules de $M$, primaires par rapport à $M$, et tels que $N = \bigcap_{i \in I} Q_i$.

#### Exemple {#ac-iv-s2-n2-exa-1 .statement}

Prenons $A = \mathbf{Z}$, $M = \mathbf{Z}$, $N = n\mathbf{Z}$ pour un entier $n > 0$. Si $n = p_1^{\alpha_1} ... p_k^{\alpha_k}$ est la décomposition de $n$ en facteurs premiers, $n\mathbf{Z} = (p_1^{\alpha_1}\mathbf{Z}) \cap ... \cap (p_k^{\alpha_k}\mathbf{Z})$ est une décomposition primaire de $n\mathbf{Z}$ dans $\mathbf{Z}$ d’après l’Exemple 4 du no 1.

Par abus de langage, on dit que la relation $N = \bigcap_{i \in I} Q_i$ est une décomposition primaire de $N$ dans $M$. Il revient au même de dire que $\{ 0 \} = \bigcap_{i \in I} (Q_i/N)$ est une décomposition primaire de $\{ 0 \}$ dans $M/N$. Si $(Q_i)_{i \in I}$ est une décomposition primaire de $N$ dans $M$, l’application canonique de $M/N$ dans $\bigoplus_{i \in I} (M/Q_i)$ est injective. Réciproquement soient $N$ un sous-module de $M$, et soit $f$ un homomorphisme injectif de $M/N$ dans une somme directe finie $P = \bigoplus_{i \in I} P_i$, où chaque ensemble $\mathrm{Ass}(P_i)$ est réduit à un seul élément $p_i$; soient $f_i$ l’homomorphisme $M/N \to P_i$ déduit par composition avec $f$ de la projection $P \to P_i$, et soit $Q_i/N$ le noyau de $f_i$; alors les $Q_i$ distincts de $M$ sont primaires par rapport à $M$ (no 1, déf. 1) et on a $N = \bigcap_{i \in I} Q_i$. En outre, on a $\mathrm{Ass}(M/N) \subset \bigcup_{i \in I} \{ p_i \}$ en vertu du $§ 1$, no 1, prop. 3.

#### Théorème 1 {#ac-iv-s2-thm-1 .statement}

Soit M un module de type fini sur un anneau noethérien, et soit N un sous-module de M. Il existe une décomposition primaire de N dans M de la forme

(1)
$$
N = \bigcap_{p \in \operatorname{Ass}(M/N)} Q(p)
$$
où, pour tout $p \in \operatorname{Ass}(M/N)$, $Q(p)$ est $p$-primaire par rapport à M.

Quitte à remplacer M par $M/N$, on peut supposer que $N = 0$. En vertu du § 1, no 4, cor. du th. 2, $\operatorname{Ass}(M)$ est fini ; en vertu du § 1, no 1, prop. 4, il existe, pour chaque $p \in \operatorname{Ass}(M)$, un sous-module $Q(p)$ de M tel que $\operatorname{Ass}(M/Q(p)) = \{ p \}$ et $\operatorname{Ass}(Q(p)) = \operatorname{Ass}(M) - \{ p \}$. Posons $P = \bigcap_{p \in \operatorname{Ass}(M)} Q(p)$; pour tout $p \in \operatorname{Ass}(M)$, on a $\operatorname{Ass}(P) \subset \operatorname{Ass}(Q(p))$, donc $\operatorname{Ass}(P) = \emptyset$, ce qui entraîne $P = 0$ ($§ 1$, no 1, cor. 1 de la prop. 2) et démontre donc le théorème.

### 3. Propriétés d'unicité dans la décomposition primaire.

#### Définition 3 {#ac-iv-s2-def-3 .statement}

Soient M un module sur un anneau noethérien, N un sous-module de M. On dit qu'une décomposition primaire $N = \bigcap_{i \in I} Q_i$ de N dans M est réduite si les conditions suivantes sont remplies :

a) il n'existe aucun indice $i \in I$ tel que $\bigcap_{j \neq i} Q_j \subset Q_i$;

b) si $\operatorname{Ass}(M/Q_i) = \{ p_i \}$, les $p_i$ ($i \in I$) sont deux à deux distincts.

De toute décomposition primaire $N = \bigcap_{i \in I} Q_i$ de N dans M, on déduit une décomposition primaire réduite de N dans M, de la façon suivante : soit J un élément minimal de l'ensemble des parties $I'$ de I telles que $N = \bigcap_{i \in I'} Q_i$. Il est clair que $(Q_i)_{i \in J}$ vérifie la condition a). Soit alors $\Phi$ l'ensemble des $p_i$ pour $i \in J$; pour tout $p \in \Phi$, soit $H(p)$ l'ensemble des $i \in J$ tels que $p_i = p$, et soit
$$
Q(p) = \bigcap_{i \in H(p)} Q_i ;
$$
il résulte de la prop. 2 du no 1 que $Q(p)$ est p-primaire par rapport à M ; on a en outre $N = \bigcap_{p \in \Phi} Q(p)$ et la famille $(Q(p))_{p \in \Phi}$ est donc une décomposition primaire réduite de N dans M.

Nous allons voir que la décomposition primaire définie dans la démonstration du th. 1 du no 2 est réduite ; cela résulte de la proposition suivante :

#### Proposition 4 {#ac-iv-s2-prop-4 .statement}

*Soient M un module sur un anneau noethérien, N un sous-module de M, $N = \bigcap_{i \in I} Q_i$ une décomposition primaire de N dans M, et pour tout $i \in I$, soit $\{ p_i \} = \operatorname{Ass}(M/Q_i)$. Pour que cette décomposition soit réduite, il faut et il suffit que les $p_i$ soient deux à deux distincts et appartiennent à $\operatorname{Ass}(M/N)$ ; on a alors*

$$
\text{(2)} \qquad \operatorname{Ass}(M/N) = \bigcup_{i \in I} \{ p_i \}
$$

$$
\text{(3)} \qquad \operatorname{Ass}(Q_i/N) = \bigcup_{j \neq i} \{ p_j \} \text{ pour tout } i \in I.
$$

Si la condition de l'énoncé est vérifiée, on ne peut avoir $N = \bigcap_{j \neq i} Q_j$, car on en déduirait $\operatorname{Ass}(M/N) \subset \bigcup_{j \neq i} \{ p_j \}$ (§ 1, no 1, cor. 2 de la prop. 3) contrairement à l'hypothèse ; la décomposition primaire $(Q_i)_{i \in I}$ de N est donc bien réduite. Inversement, on a toujours $\operatorname{Ass}(M/N) \subset \bigcup_{i \in I} \{ p_i \}$ (§ 1, no 1, cor. 2 de la prop. 3) ; d'autre part, pour tout $i \in I$, posons $P_i = \bigcap_{j \neq i} Q_j$; on a $P_i \cap Q_i = N$ et $P_i \neq N$ si $(Q_i)_{i \in I}$ est réduite, donc $P_i/N$ est non nul et est isomorphe au sous-module $(P_i + Q_i)/Q_i$ de $M/Q_i$, d'où $\{ p_i \} = \operatorname{Ass}(P_i/N)$ (§ 1, no 1, prop. 3 et cor. 1 de la prop. 2) ; comme $P_i/N \subset M/N$, on a $p_i \in \operatorname{Ass}(M/N)$, ce qui achève de prouver la nécessité de la condition de l'énoncé et la formule (2). Enfin, comme $N = \bigcap_{j \neq i} (Q_j \cap Q_i)$, on a $\operatorname{Ass}(Q_i/N) \subset \bigcup_{j \neq i} \operatorname{Ass}(Q_i/(Q_j \cap Q_i))$ (§ 1, no 1, cor. 2 de la prop. 3);

mais $Q_i/(Q_j \cap Q_i)$ est isomorphe au sous-module $(Q_i + Q_j)/Q_j$ de $M/Q_j$, donc $\operatorname{Ass}(Q_i/(Q_j \cap Q_i)) \subset \{ p_j \}$, et $\operatorname{Ass}(Q_i/N) \subset \bigcup_{j \neq i} \{ p_j \}$; compte tenu de (2) et de la prop. 3 du § 1, n° 1, on obtient bien la formule (3).

#### Corollaire {#ac-iv-s2-n3-cor-1 .statement}

*Soient A un anneau noethérien, M un A-module, N un sous-module de M, $(Q_i)_{i \in I}$ une décomposition primaire de N dans M. On a alors Card(I) $\geqslant$ Card($\operatorname{Ass}(M/N)$) ; pour que $(Q_i)_{i \in I}$ soit une décomposition primaire réduite, il faut et il suffit que Card(I) = Card($\operatorname{Ass}(M/N)$).*

Il résulte des remarques précédant la prop. 4 qu’il existe une décomposition primaire réduite $(R_j)_{j \in J}$ de N dans M telle que Card(J) $\leqslant$ Card(I) ; la première assertion résulte donc de la seconde, et cette dernière est une conséquence de la prop. 4.

#### Proposition 5 {#ac-iv-s2-prop-5 .statement}

*Soient A un anneau noethérien, M un A-module, N un sous-module de M, $N = \bigcap_{i \in I} Q_i$ une décomposition primaire réduite de N dans M, et pour tout $i \in I$, soit $\{ p_i \} = \operatorname{Ass}(M/Q_i)$. Si $p_i$ est un élément minimal de $\operatorname{Ass}(M/N)$, $Q_i$ est égal au saturé de N relativement à $p_i$ (chap. II, § 2, n° 4) (cf. exerc. 2).

On peut évidemment se borner au cas où $N = 0$, en remplaçant au besoin M par $M/N$. Si $p_i$ est minimal dans $\operatorname{Ass}(M)$, l’ensemble des éléments de $\operatorname{Ass}(M)$ qui ne rencontrent pas $A - p_i$ est réduit à $p_i$ ; la proposition résulte alors de la formule (3) ci-dessus, et du § 1, n° 2, prop. 6, le noyau de l’application canonique $M \to M_{p_i}$ étant égal au saturé de 0 relativement à $p_i$ (chap. II, § 2, n° 4).

#### Remarque {#ac-iv-s2-n3-rem-1 .statement}

Les idéaux premiers $p_i \in \operatorname{Ass}(M/N)$ qui ne sont pas des éléments minimaux de cet ensemble sont parfois appelés les idéaux premiers *immergés* associés à $M/N$ ; lorsque $M/N$ est de type fini, pour que $p_0 \in \operatorname{Ass}(M/N)$ soit immergé, il faut et il suffit que $V(p_0)$ *ne soit pas* une composante irréductible de $\operatorname{Supp}(M/N)$ (chap. II, § 4, n° 3, cor. 2 de la prop. 14) ; si $(Q(p))_{p \in \operatorname{Ass}(M/N)}$ et $(Q'(p))_{p \in \operatorname{Ass}(M/N)}$ sont deux décompositions primaires réduites de

N dans M, il peut se faire alors que Q'(p_0) \neq Q(p_0) (exerc. 24 c); on peut toutefois définir une décomposition primaire réduite canonique de N dans M, en imposant aux sous-modules primaires qui y figurent des conditions supplémentaires (exerc. 4).

### 4. Localisation d'une décomposition primaire.

Étant donné un sous-module N d'un module M sur un anneau noethérien A, nous désignerons pour simplifier par D_I(M/N), dans ce n°, l'ensemble des décompositions primaires réduites de N dans M dont l'ensemble d'indices est I (équipotent à Ass(M/N)).

#### Proposition 6 {#ac-iv-s2-prop-6 .statement}

Soient A un anneau noethérien, M un A-module, N un sous-module de M, I = Ass(M/N). Soient S une partie multiplicative de A, J la partie de I formée des indices i tels que S \cap p_i = \emptyset. Soit N' le saturé de N pour S dans M. Alors :

(i) Si (Q_i)_{i \in I} est un élément de D_I(M/N), la famille (Q_i)_{i \in J} est un élément de D_J(M/N'), et la famille (S^{-1}Q_i)_{i \in J} un élément de D_J(S^{-1}M/S^{-1}N).

(ii) L'application (Q_i)_{i \in J} \to (S^{-1}Q_i)_{i \in J} est une bijection de D_J(M/N') sur D_J(S^{-1}M/S^{-1}N).

(iii) Si (Q_i)_{i \in J} est un élément de D_J(M/N') et (R_i)_{i \in I} un élément de D_I(M/N), la famille (T_i)_{i \in I}, telle que T_i = Q_i pour i \in J et T_i = R_i pour i \in I - J, est un élément de D_I(M/N).

(i) On sait (n° 1, prop. 3) que pour i \in J, S^{-1}Q_i est primaire pour S^{-1}p_i et que pour i \in I - J, S^{-1}Q_i = S^{-1}M; comme S^{-1}N = \bigcap_{i \in I} S^{-1}Q_i (chap. II, § 2, n° 4), on a aussi S^{-1}N = \bigcap_{i \in J} S^{-1}Q_i. Les S^{-1}p_i pour i \in J sont deux à deux distincts et leur ensemble est Ass(S^{-1}M/S^{-1}N) (§ 1, n° 2, cor. de la prop. 5); donc (prop. 4) (S^{-1}Q_i)_{i \in J} est une décomposition primaire réduite de S^{-1}N. En outre, on a Q_i = (i_M^s)^{-1}(S^{-1}Q_i) (n° 1, prop. 3), donc N' = (i_M^s)^{-1}(S^{-1}N) = \bigcap_{i \in J} Q_i, et (Q_i)_{i \in J} est évidemment une décomposition primaire réduite de N' dans M.

(ii) Comme S^{-1}N' = S^{-1}N, on peut remplacer N par N', c'est-à-dire supposer que J = I. Soit (P_i)_{i \in I} une décomposition primaire réduite de $S^{-1}N$ dans $S^{-1}M$, et posons $Q_i = (i_M^s)^{-1}(P_i)$; il résulte du no 1, prop. 3, que $Q_i$ est primaire pour $p_i$ ($i \in I$) et $(Q_i)_{i \in I}$ est donc une décomposition primaire réduite de $N$ dans $M$ en vertu du no 3, cor. de la prop. 4. Enfin, comme pour tout $i \in I$ et tout sous-module $Q'_i$ de $M$ qui est $p_i$-primaire par rapport à $M$, on a $Q'_i = (i_M^s)^{-1}(S^{-1}Q'_i)$ en vertu du no 1, prop. 3 et de l’hypothèse $J = I$, on voit que l’on a défini deux applications $D_I(M/N) \to D_I(S^{-1}M/S^{-1}N)$ et $D_I(S^{-1}M/S^{-1}N) \to D_I(M/N)$ dont les composées sont les identités dans $D_I(M/N)$ et $D_I(S^{-1}M/S^{-1}N)$, ce qui prouve (ii).

(iii) En vertu de (i), on a $N' = \bigcap_{i \in J} R_t$, d’où $N = N' \cap \bigcap_{i \in I-J} R_t = (\bigcap_{i \in J} Q_i) \cap (\bigcap_{i \in I-J} R_t)$, et il résulte aussitôt du no 3, cor. de la prop. 4, que cette décomposition primaire est réduite.

#### Corollaire {#ac-iv-s2-n4-cor-1 .statement}

Les applications $D_I(M/N) \to D_J(M/N')$ et $D_I(M/N) \to D_J(S^{-1}M/S^{-1}N)$ définies dans la prop. 6, (i), sont surjectives.

En effet, la prop. 6, (iii) montre que l’application $D_I(M/N) \to D_J(M/N')$ est surjective, et la prop. 6 (ii) montre alors que l’application $D_I(M/N) \to D_J(S^{-1}M/S^{-1}N)$ est surjective.

### 5. Anneaux et modules de longueur finie.

Si un $A$-module $M$ est de longueur finie, nous noterons cette longueur $\operatorname{long}_A(M)$ ou $\operatorname{long}(M)$. Rappelons que tout anneau artinien est noethérien (*Alg.*, chap. VIII, § 6, no 5, cor. 3 de la prop. 12) et que tout module de type fini sur un anneau artinien est de longueur finie (*loc. cit.*, cor. 1 de la prop. 12). En outre, tout anneau artinien intègre est un corps (*Alg.*, chap. VIII, § 6, no 4, prop. 9).

#### Proposition 7 {#ac-iv-s2-prop-7 .statement}

Soit $M$ un module de type fini sur un anneau noethérien $A$. Les propriétés suivantes sont équivalentes :
a) $M$ est de longueur finie.
b) Tout idéal $p \in \operatorname{Ass}(M)$ est un idéal maximal de $A$.
c) Tout idéal $p \in \operatorname{Supp}(M)$ est un idéal maximal de $A$.
Soit $(M_t)_{0 \leq t \leq n}$ une suite de composition de $M$ telle que, pour 0 \leq i \leq n - 1, M_i / M_{i+1} soit isomorphe à $A/p_i$, où $p_i$ est premier ($§ 1$, no 4, th. 1). Si $M$ est de longueur finie, il en est de même de chacun des $A$-modules $A/p_i$, ce qui implique que chacun des anneaux $A/p_i$ est artinien ; mais comme $A/p_i$ est intègre, c'est alors un corps, autrement dit $p_i$ est maximal ; on en conclut que a) implique b) ($§ 1$, no 4, th. 2). La condition b) entraîne c) en vertu du $§ 1$, no 3, prop. 7. Enfin, si tous les idéaux de $\mathrm{Supp}(M)$ sont maximaux, il en est de même des $p_i$ ($§ 1$, no 4, th. 2), donc les $A/p_i$ sont des $A$-modules simples, et $M$ est de longueur finie, ce qui achève la démonstration.

#### Corollaire 1 {#ac-iv-s2-prop-7-cor-1 .statement}

*Pour tout module de longueur finie $M$ sur un anneau noethérien $A$, on a $\mathrm{Ass}(M) = \mathrm{Supp}(M)$*.

En effet, tout élément de $\mathrm{Supp}(M)$ est alors minimal dans $\mathrm{Supp}(M)$ et la conclusion résulte du $§ 1$, no 3, cor. 1 de la prop. 7.

#### Corollaire 2 {#ac-iv-s2-prop-7-cor-2 .statement}

*Soient $M$ un module de type fini sur un anneau noethérien $A$, et $p$ un idéal premier de $A$. Pour que $M_p$ soit un $A_p$-module de longueur finie non nulle, il faut et il suffit que $p$ soit un élément minimal de $\mathrm{Ass}(M)$*.

En vertu du $§ 1$, no 2, cor. de la prop. 5, $\mathrm{Ass}_{A_p}(M_p)$ est l'ensemble des idéaux $q_p$, où $q$ parcourt l'ensemble des idéaux de $\mathrm{Ass}(M)$ qui sont contenus dans $p$. D'autre part, $p_p$ est l'unique idéal maximal de $A_p$; en vertu de la prop. 7, pour que $M_p$ soit un $A_p$-module de longueur finie, il faut et il suffit qu'aucun élément de $\mathrm{Ass}(M)$ ne soit strictement contenu dans $p$. D'autre part, pour que $M_p \neq 0$, il faut et il suffit par définition que $p \in \mathrm{Supp}(M)$ (chap. II, $§ 4$, no 4), c'est-à-dire que $p$ contienne un élément de $\mathrm{Ass}(M)$ ($§ 1$, no 3, prop. 7). Ceci démontre le corollaire.

#### Remarque 1 {#ac-iv-s2-n5-rem-1 .statement}

Soit $M$ un module de type fini sur un anneau noethérien $A$; soit $(M_i)_{0 \leq i \leq n}$ une suite de composition de $M$ telle que pour $0 \leq i \leq n - 1$, $M_i / M_{i+1}$ soit isomorphe à $A/p_i$, où $p_i$ est un idéal premier de $A$ ($§ 1$, no 4, th. 1). Si $p$ est un élément minimal de $\mathrm{Ass}(M)$, la longueur $\mathrm{long}_{A_p}(M_p)$ est égale au *nombre des indices $i$ tels que $p_i = p$*. En effet, les $(M_i)_p$ forment une suite de composition de $M_p$, et $(M_i)_p / (M_{i+1})_p$ est isomorphe à $(A/p_i)_p$, donc à $\{0\}$ si $p_i \neq p$ (puisque $p$ est minimal dans l'ensemble des $p_i$ en vertu du $§ 1$, no 4, th. 2) et à $(A/p)_p$ qui est un corps, si $p_i = p$.

#### Proposition 8 {#ac-iv-s2-prop-8 .statement}

Soit M un module de longueur finie sur un anneau noethérien A.

(i) Il n’existe qu’une seule décomposition primaire de {0} par rapport à M indexée par Ass(M) (nécessairement réduite) ; soit {0} = $\bigcap_{p \in \operatorname{Ass}(M)} Q(p)$ cette décomposition, où Q(p) est p-primaire par rapport à M.

(ii) Il existe un entier $n_0$ tel que pour tout $n \geq n_0$ et tout $p \in \operatorname{Ass}(M)$, on ait $Q(p) = p^n M$.

(iii) Pour tout $p \in \operatorname{Ass}(M)$, l’application canonique de M dans $M_p$ est surjective et son noyau est $Q(p)$.

(iv) L’injection canonique de M dans $\bigoplus_{p \in \operatorname{Ass}(M)} (M/Q(p))$ est bijective.

Comme tout élément $p \in \operatorname{Ass}(M)$ est minimal dans $\operatorname{Ass}(M)$ (prop. 7), l’assertion (i) résulte du no 3, prop. 5. Comme M est de type fini, il existe $n_0$ tel que l’on ait $p^n M \subset Q(p)$ pour tout $p \in \operatorname{Ass}(M)$ et tout $n \geq n_0$ (no 1, Remarque) ; mais comme $p$ est un idéal maximal, $p^n M$ est p-primaire par rapport à M (no 1, Exemples 2 et 3), et comme $\bigcap_{p \in \operatorname{Ass}(M)} p^n M = \{0\}$, il résulte de (i) que l’on a nécessairement $p^n M = Q(p)$ pour tout $p \in \operatorname{Ass}(M)$ ; d’où (ii). Comme les $p^n$, pour $p \in \operatorname{Ass}(M)$, sont deux à deux étrangers (chap. II, § 1, no 2, prop. 3), l’application canonique $M \to \bigoplus_{p \in \operatorname{Ass}(M)} (M/p^n M)$ est surjective (chap. II, § 1, no 2, prop. 6) d’où (iv). On a $\operatorname{Ass}(Q(p)) = \operatorname{Ass}(M) - \{p\}$ et $\operatorname{Ass}(M/Q(p)) = \{p\}$ (no 3, prop. 4) ; comme les éléments de $\operatorname{Ass}(M)$ sont des idéaux maximaux, $p$ est le seul élément de $\operatorname{Ass}(M)$ qui ne rencontre pas $A - p$ ; $Q(p)$ est donc le noyau de l’application canonique $j : M \to M_p$ ($§ 1$, no 2, prop. 6). Si $s \in A - p$, l’homothétie de $M/Q(p)$ de rapport $s$ est injective, en vertu de la relation $\operatorname{Ass}(M/Q(p)) = \{p\}$ (no 1, prop. 1) ; puisque $M/Q(p)$ est artiniens, cette homothétie est bijective (Alg., chap. VIII, § 2, no 2, lemme 3). L’application canonique $M \to M/Q(p)$ s’écrit donc $f \circ j$ où $f : M_p \to M/Q(p)$ est un $A$-homomorphisme (chap. II, § 2, no 2, prop. 3) ; comme $\operatorname{Ker}(j) = \operatorname{Ker}(f \circ j) = Q(p)$, $f$ est injectif ; on en conclut que $j$ est surjectif et $f$ bijectif.

#### Corollaire {#ac-iv-s2-n5-cor-1 .statement}

Si M est un module de longueur finie sur un anneau noethérien A, on a

$$
\text{long}_A(M) = \sum_{p \in \operatorname{Ass}(M)} \text{long}_{A_p}(M_p).
$$

Cela résultera de la prop. 8, (iv) si l’on prouve que $\text{long}_A(M/Q(p)) = \text{long}_{A_p}(M_p)$. Or, il résulte de la prop. 1 du n° 1 que pour tout $s \in A - p$, l’homothétie de rapport s dans $M/Q(p)$ est injective ; l’homothétie de rapport s dans tout sous-module R de $M/Q(p)$ est donc injective, et comme R est artinien elle est bijective (*Alg.*, chap. VIII, § 2, n° 2, lemme 3) ; on en conclut que les sous-A-modules de $M/Q(p)$ sont les images par la bijection $f : M_p \to M/Q(p)$ des sous-$A_p$-modules de $M_p$ (chap. II, § 2, n° 3), d’où notre assertion.

#### Proposition 9 {#ac-iv-s2-prop-9 .statement}

Soit A un anneau noethérien. Les conditions suivantes sont équivalentes :

a) A est artinien.
b) Tous les idéaux premiers de A sont des idéaux maximaux.
c) Tous les éléments de $\operatorname{Ass}(A)$ sont des idéaux maximaux.

Si ces conditions sont satisfaites, A n’a qu’un nombre fini d’idéaux premiers, qui sont tous maximaux et associés au A-module A ; de plus, A est un anneau semi-local, et son radical est nilpotent.

En effet, dire que A est artinien équivaut à dire que A est un A-module de longueur finie ; donc a) et c) sont équivalentes en vertu de la prop. 7. Il est clair que b) implique c). Enfin a) implique b) puisque tout anneau artinien intègre est un corps. Les propriétés a,) b), c) sont donc équivalentes.

Supposons-les vérifiées. Comme tout idéal premier de A appartient à $\operatorname{Supp}(A)$ et que tout élément de $\operatorname{Supp}(A)$ contient un élément de $\operatorname{Ass}(A)$ (§ 1, n° 3, prop. 7), il résulte de c) que $\operatorname{Ass}(A)$ est l’ensemble de tous les idéaux premiers de A ; donc A n’a qu’un nombre fini d’idéaux premiers, tous maximaux et associés au A-module A. Ceci implique évidemment que A est semi-local ; enfin, on sait que le radical d’un anneau artinien est nilpotent (*Alg.*, chap. VIII, § 6, n° 4, th. 3).

#### Remarque 2 {#ac-iv-s2-n5-rem-2 .statement}

Les conditions de la prop. 9, pour un anneau nœthérien $A$, entraînent que le spectre de $A$ est fini et discret, tout point de $\mathrm{Spec}(A)$ étant alors fermé (chap. II, § 4, no 3, cor. 6 de la prop. 11). Inversement, pour un anneau nœthérien $A$, dire que tout point de $\mathrm{Spec}(A)$ est fermé signifie que tout idéal premier de $A$ est maximal (*loc. cit.*), donc cette condition équivaut à celles de la prop. 9.

#### Corollaire 1 {#ac-iv-s2-prop-9-cor-1 .statement}

*Tout anneau artinien $A$ est isomorphe au composé direct d'une famille finie d'anneaux artiniens locaux.*

En effet, il résulte de la prop. 9 et de la prop. 8, (iii) et (iv), que si $(\mathfrak{m}_i)_{1 \leq i \leq n}$ est la famille des idéaux maximaux de $A$, l'application canonique $A \to \prod_i A_{\mathfrak{m}_i}$ est bijective.

#### Remarque 3 {#ac-iv-s2-n5-rem-3 .statement}

Ce corollaire peut aussi se déduire du fait que $\mathrm{Spec}(A)$ est fini et discret, et du chap. II, § 4, no 3, prop. 15.

#### Corollaire 2 {#ac-iv-s2-prop-9-cor-2 .statement}

*Soient $A$ un anneau nœthérien, $m$ un idéal de $A$. Les conditions suivantes sont équivalentes :*

a) $A$ est un anneau semi-local, et $m$ un idéal de définition de $A$.

b) $A$ est un anneau de Zariski pour la topologie $m$-adique, et $A/m$ est artinien.

En effet, si a) est vérifiée, $A$ est un anneau de Zariski pour la topologie $m$-adique (chap. III, § 3, no 3, *Exemple 3*) ; de plus, comme par hypothèse $m$ contient une puissance du radical $r$ de $A$, tout idéal premier de $A$ qui contient $m$ contient aussi $r$ (chap. II, § 1, no 1, prop. 1) ; il est par suite maximal, puisque $r$ est intersection finie d'idéaux maximaux (*loc. cit.*) ; la prop. 9 montre donc que $A/m$ est artinien. Réciproquement, si b) est vérifiée, tout idéal maximal $p$ de $A$ contient le radical de $A$, donc contient $m$ (chap. III, § 3, no 3, prop. 6) ; comme $A/m$ est artinien, les idéaux $p/m$ sont en nombre fini (prop. 9), donc $A$ n'a qu'un nombre fini d'idéaux maximaux, ce qui entraîne qu'il est semi-local.

#### Corollaire 3 {#ac-iv-s2-prop-9-cor-3 .statement}

*Soient $A, A'$ deux anneaux, $h$ un homomorphisme de $A$ dans $A'$. On suppose que $A$ est semi-local et nœthérien, et que $A'$ est un $A$-module de type fini. Alors l'anneau $A'$ est semi-local et noethérien ; si m est un idéal de définition de A, mA' est un idéal de définition de A'.

En effet, on sait que A' est un anneau de Zariski pour la topologie mA'-adique (chap. III, § 3, no 3, prop. 7). Comme A/m est artinien (cor. 2) et que A'/mA' est un (A/m)-module de type fini, A'/mA' est un anneau artinien, donc A' est semi-local et mA' est un idéal de définition de A' (cor. 2).

#### Corollaire 4 {#ac-iv-s2-prop-9-cor-4 .statement}

Soient A un anneau noethérien, semi-local et complet, m un idéal de définition de A, E un A-module de type fini, (F_n) une suite décroissante de sous-modules de E telle que $\bigcap_n F_n = 0$. Alors, pour tout $p > 0$, il existe $n > 0$ tel que $F_n \subset m^p E$.

Comme A est un anneau de Zariski, E est séparé et les F_n sont fermés pour la topologie m-adique. D'autre part, E est complet (chap. III, § 2, no 12, cor. 1 de la prop. 16). Enfin, E/m^pE est un module de type fini sur l'anneau A/m^p, qui est artinien (cor. 2); par suite E/m^pE est un (A/m^p)-module artinien, donc un A-module artinien. Le corollaire résulte alors du chap. III, § 2, no 7, prop. 8.

#### Corollaire 5 {#ac-iv-s2-prop-9-cor-5 .statement}

Dans un anneau noethérien, semi-local et complet, toute suite décroissante d'idéaux dont l'intersection est 0 est une base de filtre qui converge vers 0.

Il suffit d'appliquer le cor. 4 au A-module A.

#### Proposition 10 {#ac-iv-s2-prop-10 .statement}

Soient A un anneau noethérien, $p_1, ..., p_n$ les idéaux premiers associés au A-module A, avec $p_i \neq p_j$ pour $i \neq j$.

(i) L'ensemble $S = \bigcap_{i=1}^n (A - p_i)$ est l'ensemble des éléments non diviseurs de 0 dans A.

(ii) Si tous les $p_i$ sont des éléments minimaux de Ass(A), l'anneau total de fractions $S^{-1}A$ de A est artinien.

(iii) Si l'anneau A est réduit, tous les $p_i$ sont des éléments minimaux de Ass(A) (et par suite sont les éléments minimaux de Spec(A)), et chacun des $A_{p_i}$ est un corps; pour chaque indice i, l'homomorphisme canonique $S^{-1}A \to A_{p_i}$ (chap. II, § 2, no 1, cor. 1 de la prop. 2) est surjectif et son noyau est $S^{-1}p_i$; enfin l’homomorphisme canonique de $S^{-1}A$ dans $\prod_{i=1}^n (S^{-1}A/S^{-1}p_i)$ est bijectif.

Le fait que S est l’ensemble des éléments non diviseurs de 0 de A a déjà été vu ($§ 1$, n° 1, cor. 3 de la prop. 2). Les idéaux premiers de $S^{-1}A$ sont de la forme $S^{-1}p$, où p est un idéal premier de A contenu dans $\bigcup_{i=1}^n p_i$ (chap. II, $§ 2$, n° 5, prop. 10), c’est-à-dire contenu dans un des $p_i$ (chap. II, $§ 1$, n° 1, prop. 2). Si $p_i$ est un élément minimal de Ass(A), c’est un élément minimal de Spec(A) ($§ 1$, n° 3, cor. de la prop. 7); si chacun des $p_i$ est un élément minimal de Ass(A), on voit donc que les idéaux premiers de $S^{-1}A$ sont les $S^{-1}p_i$, et ils sont donc tous maximaux, ce qui montre que $S^{-1}A$ est artinien (prop. 9).

Supposons enfin que l’anneau A soit réduit. On a alors
$$
\bigcap_{i=1}^n p_i = \{0\} \quad (§ 1, \text{n}° 3, \text{cor. 2 de la prop. 7}).
$$
On en déduit que
$$
\{0\} = \bigcap_{i=1}^n p_i
$$
est une décomposition primaire réduite de l’idéal $\{0\}$ (n° 3, cor. de la prop. 4); en particulier, aucun des $p_i$ ne peut contenir un $p_j$ d’indice $j \neq i$, et par suite les $p_i$ sont tous des éléments minimaux de Ass(A). L’anneau $S^{-1}A$ est donc artinien d’après (ii). Les $S^{-1}p_i$ sont des idéaux premiers associés au $S^{-1}A$-module $S^{-1}A$ ($§ 1$, n° 2, cor. de la prop. 5) et on a $\{0\} = S^{-1}\left(\bigcap_{i=1}^n p_i\right) = \bigcap_{i=1}^n S^{-1}p_i$ (chap. II, $§ 2$, n° 4); comme les $S^{-1}p_i$ sont deux à deux distincts, $(S^{-1}p_i)_{1 \leq i \leq n}$ est une décomposition primaire réduite de $\{0\}$ dans $S^{-1}A$ (n° 3, cor. de la prop. 4). La prop. 8 montre alors que l’homomorphisme canonique $g_i : S^{-1}A \to (S^{-1}A)_{p_i}$ est surjectif et de noyau $S^{-1}p_i$, et que l’homomorphisme canonique $S^{-1}A \to \prod_{i=1}^n (S^{-1}A/S^{-1}p_i)$ est bijectif. On sait d’ailleurs que l’homomorphisme canonique $S^{-1}A \to A_{p_i}$ est composé de $g_i$ et d’un isomorphisme $(S^{-1}A)_{S^{-1}p_i} \to A_{p_i}$ (chap. II, $§ 2$, n° 3, prop. 7). Enfin, il résulte de la prop. 8 que $(S^{-1}A)_{S^{-1}p_i}$ est isomorphe à $S^{-1}A/S^{-1}p_i$, donc est un corps puisque $S^{-1}p_i$ est un idéal maximal.

### 6. Décomposition primaire et extension des scalaires.

Dans ce n°, on désigne par A et B deux anneaux et on considère un homomorphisme d’anneaux $\rho : A \to B$, qui fait de B une A-algèbre ; rappelons que pour tout B-module F, $\rho_*(F)$ est le groupe commutatif F muni de la structure de A-module définie par $a.y = \rho(a)y$ pour $a \in A,\ y \in F$.

#### Lemme 1 {#ac-iv-s2-lem-1 .statement}

Soient A un anneau noethérien, p un idéal premier de A, E un A-module dont l’annulateur contient une puissance de p et tel que $\operatorname{Ass}(E) = \{p\}$, F un B-module tel que $\rho_*(F)$ soit un A-module plat. La condition $\mathfrak{P} \in \operatorname{Ass}_B(E \otimes_A F)$ entraîne alors $\rho^{-1}(\mathfrak{P}) = p$.

Si $n$ est tel que $p^nE = 0$, on a $p^nB \subset \operatorname{Ann}(E \otimes_A F)$, d’où $p^nB \subset \mathfrak{P}$, ce qui entraîne $p^n \subset \rho^{-1}(\mathfrak{P})$ et par suite $p \subset \rho^{-1}(\mathfrak{P})$ puisque $\rho^{-1}(\mathfrak{P})$ est premier. Par ailleurs, si $a \in A - p$, l’homothétie $h$ de rapport $a$ dans E est injective (§ 1, n° 1, cor. 2 de la prop. 2) ; comme $h \otimes 1_F$ est l’homothétie $h'$ de rapport $\rho(a)$ dans $E \otimes_A F$ et que $\rho_*(F)$ est plat, $h'$ est injective (chap. I, § 2, n° 2, déf. 1) ; ceci prouve que $\rho(a) \notin \mathfrak{P}$, d’où $\rho^{-1}(\mathfrak{P}) = p$.

#### Théorème 2 {#ac-iv-s2-thm-2 .statement}

Soient $\rho : A \to B$ un homomorphisme d’anneaux, E un A-module, F un B-module tel que $\rho_*(F)$ soit un A-module plat. On a alors

$$
\operatorname{Ass}_B(E \otimes_A F) \supset \bigcup_{p \in \operatorname{Ass}_A(E)} \operatorname{Ass}_B(F/pF).
$$

Lorsque A est noethérien, les deux membres de (5) sont égaux.
Soit $p \in \operatorname{Ass}_A(E)$; par définition, il existe une suite exacte
$$
0 \to A/p \to E.
$$
Puisque F est un A-module plat, on en déduit une suite exacte
$$
0 \to F/pF \to E \otimes_A F
$$
d’où $\operatorname{Ass}_B(F/pF) \subset \operatorname{Ass}_B(E \otimes_A F)$, ce qui prouve l’inclusion (5).

Supposons maintenant A nœthérien et démontrons l’inclusion opposée.

On procédera par étapes :

(i) Supposons d’abord que E soit un A-module de type fini et que Ass_A(E) soit réduit à un seul élément p. En vertu du § 1, no 4, th. 1, il existe une suite de composition (E_i)_{0 \leq i \leq n} de E telle que E_i/E_{i+1} soit isomorphe à A/p_i, où p_i est un idéal premier de A ; en outre (§ 1, no 4, th. 2 et no 3, prop. 7) tous les p_i contiennent p. Comme F est un A-module plat, les E_i \otimes_A F forment une suite de composition de E \otimes_A F et (E_i \otimes_A F)/(E_{i+1} \otimes_A F) s’identifie à (A/p_i) \otimes_A F = F/p_i F. En vertu du § 1, no 1, prop. 3, on a donc

$$
\operatorname{Ass}_B(E \otimes_A F) \subset \bigcup_{i=0}^{n-1} \operatorname{Ass}_B(F/p_i F).
$$

On sait que E est annulé par une puissance de p (no 1, Remarque) ; le lemme 1 montre donc que pour tout $\mathfrak{P} \in \operatorname{Ass}_B(E \otimes_A F)$, on a $\rho^{-1}(\mathfrak{P}) = p$. Comme F/p_i F est isomorphe à (A/p_i) \otimes_A F, on a $\rho^{-1}(\mathfrak{P}') = p_i$ pour tout $\mathfrak{P}' \in \operatorname{Ass}_B(F/p_i F)$ en vertu du lemme 1, d’où $\operatorname{Ass}_B(E \otimes_A F) \cap \operatorname{Ass}(F/p_i F) = \emptyset$ si $p_i \neq p$, ce qui démontre le théorème dans le cas considéré.

(ii) Supposons seulement que E soit un A-module de type fini. Soient $p_i$ (1 \leq i \leq n) les éléments de Ass_A(E), et soit $\{0\} = \bigcap_{i=1}^n Q_i$ une décomposition primaire réduite correspondante (no 3) ; E est donc isomorphe à un sous-module de la somme directe des $E_i = E/Q_i$, et comme F est un A-module plat, $E \otimes_A F$ est isomorphe à un sous-module de la somme directe des B-modules $E_i \otimes_A F$. On en déduit (§ 1, no 1, prop. 3 et cor. 1 de la prop. 3)

$$
\operatorname{Ass}_B(E \otimes_A F) \subset \bigcup_{i=1}^n \operatorname{Ass}_B(E_i \otimes_A F).
$$

Mais $E_i$ est un A-module de type fini tel que Ass_A(E_i) soit réduit à un seul élément $p_i$ (no 1, déf. 1). En vertu de (i), on a $\operatorname{Ass}_B(E_i \otimes_A F) = \operatorname{Ass}_B(F/p_i F)$, d’où le théorème dans ce cas.

(iii) Cas général. Le B-module $E \otimes_A F$ est réunion des sous-modules $E' \otimes_A F$, $E'$ parcourant l’ensemble des sous-modules de type fini du A-module E. Si $\mathfrak{P}$ appartient à $\mathrm{Ass}_B(E \otimes_A F)$, il existe donc un sous-module de type fini $E'$ de E tel que $\mathfrak{P} \in \mathrm{Ass}_B(E' \otimes_A F)$. D’après (ii), il existe $p \in \mathrm{Ass}_A(E')$ tel que $\mathfrak{P} \in \mathrm{Ass}_B(F/pF)$; comme $\mathrm{Ass}_A(E') \subset \mathrm{Ass}_A(E)$, cela achève la démonstration du th. 2.

#### Corollaire 1 {#ac-iv-s2-thm-2-cor-1 .statement}

*Si A est noethérien et si $\mathfrak{P} \in \mathrm{Ass}_B(E \otimes_A F)$, on a $\rho^{-1}(\mathfrak{P}) \in \mathrm{Ass}_A(E)$ et $\rho^{-1}(\mathfrak{P})$ est le seul idéal premier $p$ de A tel que $\mathfrak{P} \in \mathrm{Ass}_B(F/pF)$.*
Cela résulte du th. 2 et du lemme 1 appliqué au cas où $E = A/p$.

#### Corollaire 2 {#ac-iv-s2-thm-2-cor-2 .statement}

*On suppose que A et B sont noethériens et que E est un A-module plat. Soient $p$ un idéal premier de A, $Q \subset E$ un sous-module $p$-primaire, $\mathfrak{P}$ un idéal premier de B. Pour que $Q \otimes_A B$ soit un sous-module $\mathfrak{P}$-primaire de $E \otimes_A B$, il faut et il suffit que $pB$ soit un idéal $\mathfrak{P}$-primaire de B.*
Appliquons le th. 2 au A-module $E/Q$ et au B-module B ; on a $\mathrm{Ass}_A(E/Q) = \{ p \}$ et $(E/Q) \otimes_A B$ est isomorphe à $(E \otimes_A B)/(Q \otimes_A B)$, donc $\mathrm{Ass}_B((E \otimes_A B)/(Q \otimes_A B)) = \mathrm{Ass}_B(B/pB)$. Dire que $Q \otimes_A B$ est $\mathfrak{P}$-primaire dans $E \otimes_A B$ signifie donc que $\mathrm{Ass}_B(B/pB)$ est réduit à $\mathfrak{P}$, d’où le corollaire.

#### Remarque {#ac-iv-s2-n6-rem-1 .statement}

Supposons A et B noethériens. Soit $\mathfrak{P}$ un idéal premier de B, et soit $p = \rho^{-1}(\mathfrak{P})$; posons $S = A - p$, et soit $k(p) = S^{-1}(A/p)$ le corps des fractions de $A/p$. Puisque $\mathfrak{P}$ contient $pB$, $\mathfrak{P}/pB$ est un idéal premier de $B/pB$. Si $\rho'$ est l’homomorphisme composé $A \xrightarrow{\rho} B \to B/pB$, on sait qu’on identifie $S^{-1}(B/pB)$ à l’anneau $(\rho'(S))^{-1}(B/pB)$ et $\mathfrak{P}' = S^{-1}(\mathfrak{P}/pB)$ à un idéal de cet anneau (chap. II, § 2, no 2, prop. 6) ; comme $\mathfrak{P}/pB$ ne rencontre pas $\rho'(S)$, $\mathfrak{P}'$ est un idéal premier de $S^{-1}(B/pB)$ (chap. II, § 2, no 5, prop. 11) ; par ailleurs on a des isomorphismes canoniques entre $S^{-1}(B/pB)$, $S^{-1}((A/p) \otimes_A B)$, et $(S^{-1}(A/p)) \otimes_A B = k(p) \otimes_A B$ ; de même $S^{-1}(F/pF)$ s’identifie canoniquement à $k(p) \otimes_A F$. Cela étant, sous les hypothèses du th. 2, *pour que $\mathfrak{P} \in \mathrm{Ass}_B(E \otimes_A F)$, il faut et il suffit que $p \in \mathrm{Ass}_A(E)$ et $\mathfrak{P}' \in \mathrm{Ass}_{k(p) \otimes_A B}(k(p) \otimes_A F)$*. En effet, en vertu du th. 2 et de son cor. 1, tout revient à voir que les conditions

$$
\langle \mathfrak{P} \in \mathrm{Ass}_B(F/pF) \rangle \quad \text{et} \quad \langle \mathfrak{P}' \in \mathrm{Ass}_{k(p) \otimes_A B}(k(p) \otimes_A F) \rangle
$$

sont équivalentes ; mais comme B est noethérien, cela résulte du § 1, n° 2, cor. de la prop. 5 et des identifications précédentes.

#### Proposition 11 {#ac-iv-s2-prop-11 .statement}

On suppose que A et B sont noethériens et que B est un A-module plat. Soient E un A-module, E' un sous-module de E tel que pour tout idéal $p \in \mathrm{Ass}_A(E/E')$, $pB$ soit un idéal premier de B ou soit égal à B. Soit $E' = \bigcap_{p \in \mathrm{Ass}(E/E')} Q(p)$ une décomposition primaire réduite de $E'$ dans E, $Q(p)$ étant $p$-primaire pour tout $p \in \mathrm{Ass}(E/E')$.

(i) Si $p \in \mathrm{Ass}(E/E')$ et si $pB = B$, on a $Q(p) \otimes_A B = E \otimes_A B$.

(ii) Si $p \in \mathrm{Ass}(E/E')$ et si $pB$ est premier, $Q(p) \otimes_A B$ est $pB$-primaire dans $E \otimes_A B$.

(iii) Si $\Phi$ est l'ensemble des $p \in \mathrm{Ass}(E/E')$ tels que $pB$ soit premier, on a $E' \otimes_A B = \bigcap_{p \in \Phi} (Q(p) \otimes_A B)$, et cette relation est une décomposition primaire réduite de $E' \otimes_A B$ dans $E \otimes_A B$.

Si $pB = B$, le th. 2 appliqué à $E/Q(p)$ et à B, montre que l'on a $\mathrm{Ass}_B((E/Q(p)) \otimes_A B) = \emptyset$ et comme B est noethérien et est un A-module plat, on en conclut ($§ 1$, n° 1, cor. 1 de la prop. 2) que $Q(p) \otimes_A B = E \otimes_A B$. L'assertion (ii) résulte du cor. 2 du th. 2, en prenant $\mathfrak{P} = pB$. Enfin la relation $E' \otimes_A B = \bigcap_{p \in \Phi} (Q(p) \otimes_A B)$ résulte de ce que B est un A-module plat (chap. I, $§ 2$, n° 6, prop. 6) ; comme $p = \overline{\rho}(pB)$ pour $p \in \Phi$ (lemme 1), on a $pB \neq p'B$ pour deux idéaux distincts $p, p'$ de l'ensemble $\Phi$; d'autre part, on a $\mathrm{Ass}((E \otimes_A B)/(E' \otimes_A B)) = \Phi$ en vertu du th. 2 ; on conclut du n° 3, prop. 4 que $E' \otimes_A B = \bigcap_{p \in \Phi} (Q(p) \otimes_A B)$ est une décomposition primaire réduite.

#### Corollaire {#ac-iv-s2-n6-cor-1 .statement}

Supposons que $pB$ soit premier pour tout $p \in \mathrm{Ass}_A(E/E')$. Alors, si $p_1, ..., p_n$ sont les éléments minimaux de $\mathrm{Ass}_A(E/E')$, les $p_iB$ sont les éléments minimaux de $\mathrm{Ass}_A((E \otimes_A B)/(E' \otimes_A B))$.

Il résulte en effet de la prop. 11 que l'on a dans ce cas $p_iB \neq p_jB$ pour $i \neq j$.

#### Exemple 1 {#ac-iv-s2-n6-exa-1 .statement}

Prenons $B = S^{-1}A$, où $S$ est une partie multiplicative de $A$; si $A$ est nœthérien, les hypothèses de la prop. 11 sont vérifiées, et on retrouve une partie de la prop. 6 du no 4.

#### Exemple 2 {#ac-iv-s2-n6-exa-2 .statement}

Soient $A$ un anneau nœthérien, $m$ un idéal de $A$, $B$ le séparé complété de $A$ pour la topologie $m$-adique; alors $B$ est un $A$-module plat et on peut appliquer à $F = B$ le th. 2 ; mais en général les hypothèses de la prop. 11 ne seront pas vérifiées pour les idéaux premiers de $A$ (chap. III, § 2, exerc. 15 b)).

#### Exemple 3 {#ac-iv-s2-n6-exa-3 .statement}

Soient $A$ un anneau nœthérien, $B$ l’algèbre de polynômes $A[X_1,...,X_n]$; $B$ est nœthérien et est un $A$-module libre, donc plat. En outre, si $p$ est un idéal premier de $A$, $B/pB$ est isomorphe à $(A/p)[X_1,...,X_n]$, qui est intègre, donc $pB$ est premier ; les hypothèses de la prop. 11 sont donc vérifiées pour tout $A$-module $E$ et tout sous-module $E'$ de $E$.

#### Exemple 4 {#ac-iv-s2-n6-exa-4 .statement}

Soient $A$ une algèbre de type fini sur un corps $k$, $K$ une extension de $k$, $B = A \otimes_k K$ l’algèbre sur $K$ obtenue par extension des scalaires ; $A$ et $B$ sont nœthériens et $B$ est un $A$-module libre, donc on peut appliquer le th. 2 à $F = B$. Dans certains cas (par exemple lorsque $k$ est algébriquement clos), on peut montrer que pour tout idéal premier $p$ de $A$, $pB$ est premier ou égal à $B$; nous reviendrons plus tard sur cet exemple.

## EXERCICES {#ac-iv-s2-exercises}

See the [exercises for § 2](exercises/s2/).
