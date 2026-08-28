---
book: ac
book_title: Commutative Algebra
chapter: VIII
chapter_title: DIMENSION
section: 6
section_title: Dimension des anneaux gradués
lang: fr
source: ac-viii-ix-fr
book_pages: AC VIII.62-AC VIII.71, AC VIII.99-AC VIII.103
pdf_pages: 0066-0075, 0103-0107
extraction: ocr
subsections:
    - "no": 1
      title: Anneau filtré associé à un anneau gradué
      page: 62
      pdf_page: 66
    - "no": 2
      title: Dimension et chaînes d’idéaux gradués
      page: 0
      pdf_page: 67
    - "no": 3
      title: Dimension des modules gradués
      page: 0
      pdf_page: 69
    - "no": 4
      title: Semi-continuité de la dimension
      page: 69
      pdf_page: 73
    - "no": 5
      title: Algèbres graduées régulières
      page: 70
      pdf_page: 74
statements: 27
exercises: 12
content_sha256: 0579a874882d9e7d3c1b38a078e814db3421c17202711fc74c4f641509ba64bf
---

## § 6. DIMENSION DES ANNEAUX GRADUÉS

Dans ce paragraphe, on désigne par H un anneau gradué de type $\mathbf{Z}$, à degrés positifs, et par $(H_n)_{n \in \mathbf{Z}}$ sa graduation ; ainsi, on a $H_n = \{0\}$ pour $n < 0$.

### 1. Anneau filtré associé à un anneau gradué

Pour tout $n \in \mathbf{Z}$, on pose $H_{\geq n} = \sum_{i \geq n} H_i$. On a $H = H_{\geq 0}$; les $H_{\geq n}$ sont des idéaux gradués de H. Notons S la partie multiplicative $1 + H_{\geq 1}$ formée des éléments de H dont la composante de degré 0 est égale à 1, et considérons l’anneau de fractions $S^{-1}H$. Identifions H à un sous-anneau de son complété $\hat{H} = \prod_{n} H_n$ (III, § 2, n° 12, exemple 1); comme les éléments de S sont inversibles dans $\hat{H}$ (III, § 2, n° 13, lemme 3), $S^{-1}H$ s’identifie à un sous-anneau de $\hat{H}$ contenant H. Pour $s \in S$ et $h \in H_{\geq n}$, l’élément $s^{-1}h - h$ de $\hat{H}$ appartient à $\prod_{i \geq n} H_i$; par conséquent on a $S^{-1}H_{\geq n} = (S^{-1}H) \cap \prod_{i \geq n} H_i$.

On en déduit :

#### Proposition 1 {#ac-viii-s6-prop-1 .statement}

a) Les idéaux $S^{-1}H_{\geq n}$ forment une filtration exhaustive et séparée de l’anneau $S^{-1}H$.

b) L’homomorphisme canonique de $H$ dans $S^{-1}H$ induit pour chaque $n$ un isomorphisme $u_n$ de $H_n$ sur $S^{-1}H_{\geq n}/S^{-1}H_{\geq n+1}$; les $u_n$ sont les composants homogènes d’un isomorphisme d’anneaux gradués de $H$ sur l’anneau gradué associé à $S^{-1}H$, filtré par les $S^{-1}H_{\geq n}$.

#### Remarque 1 {#ac-viii-s6-n1-rem-1 .statement}

Un élément $h/s$ de $S^{-1}H$ avec $h \in H, s \in S$, est inversible si et seulement si la composante de degré 0 de $h$ est inversible dans $H_0$. Par conséquent, si l’anneau $H_0$ est local, l’anneau $S^{-1}H$ est local et l’injection canonique $H_0 \to S^{-1}H$ induit un isomorphisme sur les corps résiduels.

#### Remarque 2 {#ac-viii-s6-n1-rem-2 .statement}

Supposons $H$ engendré par $H_0$ et $H_1$; alors pour tout $n$, on a $H_{n+1} = H_1.H_n$, donc $H_{\geq n+1} = H_1.H_{\geq n}$ et $S^{-1}H_{\geq n+1} = H_1.S^{-1}H_{\geq n}$. Par suite, la filtration $(S^{-1}H_{\geq n})$ de $S^{-1}H$ est la filtration $S^{-1}H_{\geq 1}$-adique.

#### Exemple 1 {#ac-viii-s6-n1-exa-1 .statement}

\* Soit $p$ un idéal premier gradué de $\mathbf{C}[X_0, ..., X_n]$ différent de l’idéal engendré par les $X_i$; soient $V$ la sous-variété algébrique de $\mathbf{P}^n(\mathbf{C})$ définie par $p$ et $C$ la sous-variété algébrique de $\mathbf{C}^{n+1}$ définie par $p$. Alors $C$ est le cône de base $V$, $H = \mathbf{C}[X_0, ..., X_n]/p$ est l’algèbre affine de $C$ et $S^{-1}H$ l’anneau local du cône $C$ en son sommet. \*
2) Soient $A$ un anneau local et $a$ un idéal de $A$ distinct de $A$. Alors $H = \bigoplus_n a^n/a^{n+1}$ est un anneau gradué tel que $H_0 = A/a$ soit local ; il est engendré par $H_0$ et $H_1$. L’anneau $S^{-1}H$ est donc local et la filtration $(S^{-1}H_{\geq n})$ est la filtration $S^{-1}H_{\geq 1}$-adique. On prendra garde qu’en général les anneaux $A$ et $S^{-1}H$ ne sont pas isomorphes. \* En particulier une variété algébrique n’est pas en général localement isomorphe au voisinage d’un point à son cône des tangentes en ce point. \*

### 2. Dimension et chaînes d’idéaux gradués

Dans ce numéro, nous noterons dimgr(H) la borne supérieure des longueurs des chaînes d’idéaux premiers gradués de $H$; de même, si $p$ est un idéal premier gradué de $H$, nous noterons htgr(p) la borne supérieure des longueurs des chaînes d’idéaux premiers gradués de $H$ dont $p$ est le plus grand élément. Si $p$ est un idéal premier gradué de $H$, on a $p \cap S = \varnothing$; sinon, en effet $p$ contiendrait un élément dont la composante de degré 0 serait égale à 1, donc contiendrait 1 puisqu’il est gradué. L’application $p \mapsto S^{-1}p$ de l’ensemble des idéaux premiers gradués de $H$ dans l’ensemble des idéaux premiers de $S^{-1}H$ est donc injective et croissante (II, § 2, no 5, prop. 11); par conséquent, compte tenu du § 1, no 3, prop. 6 et corollaire à la prop. 7, on a :

#### Proposition 2 {#ac-viii-s6-prop-2 .statement}

a) On a $\dim_{\mathrm{gr}}(H) \leq \dim(S^{-1}H) \leq \dim(H)$.
b) Pour tout idéal premier gradué $p$ de $H$, on a $\operatorname{ht}_{\mathrm{gr}}(p) \leq \operatorname{ht}(S^{-1}p) = \operatorname{ht}(p)$.

Pour tout idéal $a$ de $H$, notons $a^{\mathrm{gr}}$ le plus grand idéal gradué contenu dans $a$; on a $a^{\mathrm{gr}} = \sum_n (a \cap H_n)$.

#### Lemme 1 {#ac-viii-s6-lem-1 .statement}

a) Si $p$ est un idéal premier de $H$, $p^{gr}$ est un idéal premier.

b) Tout élément maximal de l’ensemble des idéaux gradués de $H$ distincts de $H$ est un idéal maximal de $H$ qui contient $H_{\geq 1}$.

c) Tout idéal premier minimal de $H$ est gradué.

a) Cela résulte de III, § 1, n° 4, prop. 4.

b) Soit $m$ un idéal gradué de $H$ distinct de $H$. Alors on a
$$
m \subset (m \cap H_0) + H_{\geq 1} \neq H.
$$
Si $m$ est maximal, alors on a $m = m_0 + H_{\geq 1}$, où $m_0$ est un idéal maximal de $H_0$, d’où $b$.

c) Soit $p$ un idéal premier minimal de $H$. Comme $p^{gr}$ est premier d’après $a$ et contenu dans $p$, on a $p = p^{gr}$, d’où $c$.

#### Lemme 2 {#ac-viii-s6-lem-2 .statement}

Soient $p$ et $q$ des idéaux premiers de $H$ tels que $q \subset p$ et $q \neq p$. Si $q^{gr} = p^{gr}$, alors $q$ est gradué, $p$ ne l’est pas et $ht(p/q) = 1$.

\* Remarque 1. — Reprenons les notations de l’exemple 1 du n° 1. Le lemme 2 implique que, si deux sous-variétés irréductibles $Y$ et $Z$ de $\mathbf{C}^{n+1}$ ont le même cône projetant et si $Z \subset Y$ et $Z \neq Y$, alors $Y$ est le cône projetant de $Z$, et $Z$ est de codimension 1 dans $Y$. \*

Remplaçant $H$ par $H/q^{gr}$ on se ramène au cas où $q^{gr} = \{0\}$. Alors $H$ est intègre (lemme 1, $a$), $p^{gr} = 0$, et il s’agit de prouver que $ht(p) \leq 1$ : cela entraînera en effet que $ht(q) = 0$, donc que $q = \{0\}$. Puisque $p^{gr} = \{0\}$, on a $p \cap H_n = \{0\}$ pour tout $n$, et $p$ est disjoint de la partie multiplicative $T = \bigcup (H_n - \{0\})$. L’anneau $H_p$ est donc isomorphe à un anneau de fractions de $T^{-1}H$, et l’on a donc
$$
ht(p) = \dim(H_p) \leq \dim(T^{-1}H)
$$
(§ 1, n° 3, prop. 6 et 7). Mais, d’après le lemme 4 de V, § 1, n° 8, $T^{-1}H$ est un corps ou est isomorphe à un anneau $K[X, X^{-1}]$, où $K$ est un corps ; on a donc $\dim(T^{-1}H) \leq 1$ et $ht(p) \leq 1$, ce qu’on voulait démontrer.

#### Proposition 3 {#ac-viii-s6-prop-3 .statement}

Soit $p$ un idéal premier de $H$. Si $p \neq p^{gr}$, on a $ht(p^{gr}) = ht(p) - 1$.

D’après le lemme 1, $a$, l’idéal $p^{gr}$ est premier et contenu dans $p$, donc $ht(p^{gr}) \leq ht(p) - 1$. La proposition étant triviale lorsque $ht(p^{gr}) = + \infty$, on peut supposer $ht(p^{gr}) < + \infty$. Démontrons l’inégalité $ht(p) \leq ht(p^{gr}) + 1$ par récurrence sur $ht(p^{gr})$. Il suffit de prouver que, pour tout idéal premier $q$ contenu dans $p$ et distinct de $p$, on a $ht(q) \leq ht(p^{gr})$. Distinguons deux cas suivant que $q^{gr} \neq p^{gr}$ ou que $q^{gr} = p^{gr}$. Si $q^{gr} \neq p^{gr}$, alors on a $ht(q^{gr}) < ht(p^{gr})$; on a
$$
ht(q) \leq ht(q^{gr}) + 1,
$$
d’après l’hypothèse de récurrence si $q \neq q^{gr}$ et trivialement si $q = q^{gr}$; par conséquent, on a $ht(q) \leq ht(q^{gr}) + 1 \leq ht(p^{gr})$, ce qu’on voulait démontrer. Si $q^{gr} = p^{gr}$, alors on a $q = q^{gr}$ d’après le lemme 2, donc $ht(q) = ht(q^{gr}) \leq ht(p^{gr})$, d’où encore la conclusion voulue.

#### Théorème 1 {#ac-viii-s6-thm-1 .statement}

Supposons H noethérien.

a) Toute chaîne d’idéaux premiers gradués de H, saturée comme chaîne d’idéaux premiers gradués, est saturée comme chaîne d’idéaux premiers.

b) Pout tout idéal premier gradué p de H, on a htgr(p) = ht(S^{-1}p) = ht(p).

c) On a dimgr(H) = dim(S^{-1}H) = dim(H).

Pour démontrer a), il suffit de prouver que, si p et q sont deux idéaux premiers gradués distincts de H tels que q ⊂ p et que tout idéal premier gradué compris entre q et p soit égal à p ou à q, alors ht(p/q) = 1. En divisant par q, on se ramène au cas où q = {0}. Il s’agit donc de prouver que, si H est intègre, et si p est un idéal de H, minimal parmi les idéaux premiers gradués ≠ {0}, on a ht(p) = 1. Or, soit a un élément homogène non nul de p, et soit r un idéal premier de H tel que a ∈ r ⊂ p et minimal pour ces propriétés (II, § 2, no 6, lemme 2). Puisque r^{gr} est premier (lemme 1, a)) et non nul, on a r^{gr} = p, donc p = r. Comme H est intègre et noethérien, p est de hauteur 1 (§ 3, no 1, prop. 1), d’où a).

Démontrons b). Soit p un idéal premier gradué de H. On a

$$
\text{htgr}(p) \leq \text{ht}(S^{-1}p) \leq \text{ht}(p)
$$

(prop. 2); démontrons l’inégalité ht(p) ≤ htgr(p) par récurrence sur htgr(p). Si htgr(p) = 0, p est minimal parmi les idéaux premiers gradués, donc minimal (lemme 1, c)) et l’on a ht(p) = 0. Supposons que l’on ait htgr(p) > 0 et prouvons l’inégalité ht(q) ≤ htgr(p) − 1 pour tout idéal premier q contenu dans p et distinct de p. Distinguons deux cas. Si q est gradué, on conclut par l’hypothèse de récurrence. Si q n’est pas gradué, alors on a q^{gr} ≠ p, donc ht(q^{gr}) ≤ htgr(q^{gr}) d’après l’hypothèse de récurrence, d’où ht(q) ≤ htgr(q^{gr}) + 1 d’après la prop. 3 ; il reste à prouver l’inégalité htgr(q^{gr}) ≤ htgr(p) − 2 ; mais si l’on avait htgr(q^{gr}) = htgr(p) − 1, la chaîne q^{gr} ⊂ p serait saturée d’après a), ce qui n’est pas puisque q^{gr} ≠ q ≠ p.

Prouvons enfin c). On a dimgr(H) ≤ dim(S^{-1}H) ≤ dim(H) (prop. 2), et il reste à prouver dim(H) ≤ dimgr(H), ou encore ht(p) ≤ dimgr(H) pour tout idéal premier p de H. Soit donc p un idéal premier de H. Si p est gradué, on a ht(p) = htgr(p) ≤ dimgr(H). Si p n’est pas gradué, on a ht(p) = htgr(p^{gr}) + 1 d’après la prop. 3 ; soit m un idéal gradué maximal de H contenant p^{gr} ; d’après le lemme 1, b), m est maximal, donc distinct de p^{gr}, et l’on a htgr(p^{gr}) + 1 ≤ htgr(m) ≤ dimgr(H), d’où encore ht(p) ≤ dimgr(H). Cela achève la démonstration.

#### Remarque 2 {#ac-viii-s6-n2-rem-2 .statement}

Il existe des anneaux gradués non noethériens H tels que dimgr(H) < dim(H) (p. 99, exercice 1).

### 3. Dimension des modules gradués

Dans ce numéro, on note M un H-module gradué (de type $\mathbf{Z}$).
Alors S^{-1}M est un S^{-1}H-module, et si l’on pose $M_{\geq n} = \bigoplus_{i \geq n} M_i$, on voit comme au no 1 que la suite des ensembles $S^{-1}M_{\geq n}$ est une filtration exhaustive et séparée sur

$S^{-1}M$ et que l’application canonique $M \to S^{-1}M$ induit un isomorphisme de $M$ sur le module gradué $\bigoplus_n S^{-1}M_{\geq n}/S^{-1}M_{\geq n+1}$.

#### Lemme 3 {#ac-viii-s6-lem-3 .statement}

Supposons $H$ engendré par $H_0 \cup H_1$ et $M$ engendré par $\bigoplus_{i \leq n_0} M_i$ pour un entier $n_0$ convenable. Alors la filtration $(S^{-1}M_{\geq n})$ sur $S^{-1}M$ est bonne pour l’idéal $S^{-1}H_{\geq 1}$ de $S^{-1}H$.

On a, pour $n \geq n_0$, $M_{\geq n+1} = H_1 \cdot M_{\geq n}$, donc $S^{-1}M_{\geq n+1} = H_1 \cdot S^{-1}M_{\geq n} = S^{-1}H_{\geq 1} \cdot S^{-1}M_{\geq n}$.

#### Proposition 4 {#ac-viii-s6-prop-4 .statement}

Supposons $H$ noethérien et $M$ de type fini. Alors $\dim_H(M) = \dim_{S^{-1}H}(S^{-1}M)$.

Soit a l’annulateur du $H$-module $M$ ; c’est un idéal gradué de $H$. Comme $M$ est un $H$-module de type fini, l’annulateur du $S^{-1}H$-module $S^{-1}M$ est l’idéal $S^{-1}\alpha$ de $S^{-1}H$. On a $\dim_H(M) = \dim(H/\alpha)$ et $\dim_{S^{-1}H}(S^{-1}M) = \dim(S^{-1}H/S^{-1}\alpha)$. La prop. 4 résulte alors du th. 1, c) du n° 2 appliqué à l’anneau gradué $H/\alpha$.

#### Proposition 5 {#ac-viii-s6-prop-5 .statement}

Supposons $H_0$ local et artinien, $H$ engendré par $H_0 \cup H_1$, $H_1$ de type fini comme $H_0$-module, $M$ non nul et de type fini comme $H$-module. Alors $M_n$ est un $H_0$-module de longueur finie pour chaque $n$, et il existe $Q(T) \in \mathbf{Z}[T, T^{-1}]$ tel que $Q(1) > 0$ et que l’on ait dans l’anneau $\mathbf{Z}((T))$

$$
\sum_{n \in \mathbf{Z}} \operatorname{long}_{H_0}(M_n) \cdot T^n = (1 - T)^{-d} \cdot Q(T),
$$

avec $d = \dim_H(M)$.

L’anneau $S^{-1}H$ est local et noethérien (n° 1, remarque 1), le $S^{-1}H$-module $S^{-1}M$ est non nul de type fini, et de dimension $d = \dim_H(M)$ (prop. 4). Par ailleurs, $S^{-1}H_{\geq 1}$ est un idéal de définition de $S^{-1}H$ (§ 3, n° 2, lemme 2) et $S^{-1}M_{\geq n}$ est une filtration $S^{-1}H_{\geq 1}$-bonne sur $S^{-1}M$ (lemme 3). Enfin, on a $\operatorname{long}_{S^{-1}H} S^{-1}M_{\geq n}/S^{-1}M_{\geq n+1} = \operatorname{long}_{H_0}(M_n)$ pour tout $n$. Il suffit donc d’appliquer les th. 2 et 3 du § 4 (n°s 3 et 4).

#### Remarque {#ac-viii-s6-n3-rem-1 .statement}

A l’exception de la détermination de l’entier $d$, la prop. 5 résulte directement du th. 1 du § 4, n° 2.

#### Corollaire {#ac-viii-s6-n3-cor-1 .statement}

Soient $A$ un anneau local noethérien et $q$ un idéal de définition de $A$. Alors on a $\dim(A) = \dim(\operatorname{gr}_q(A))$.

Appliquant la prop. 5 au cas $M = H = \operatorname{gr}_q(A)$, on obtient la relation

$$
\sum_{n \geq 0} \operatorname{long}_{A/q}(q^n/q^{n+1}) \cdot T^n = (1 - T)^{-d} Q(T)
$$

avec $d = \dim(\operatorname{gr}_q(A))$ et $Q(1) \neq 0$. On a $d = \dim(A)$ d’après le th. 3 du § 4, n° 4, d’où le corollaire.

#### Proposition 6 {#ac-viii-s6-prop-6 .statement}

Supposons $H_0$ local et artinien, $H$ de type fini comme $H_0$-algèbre et $M$ de type fini comme $H$-module.

a) Soient $a_1, ..., a_n$ des éléments de $H$, homogènes de degrés $> 0$, et soit $\varphi$ l’homomorphisme (de $H_0$-algèbres) de $H_0[X_1, ..., X_n]$ dans $H$ qui transforme $X_i$ en $a_i$ pour $1 \leq i \leq n$. Le $S^{-1}H$-module $S^{-1}M / \sum_{i=1}^n (a_i/1).S^{-1}M$ est de longueur finie si et seulement si $\varphi_*(M)$ est un module de type fini sur $H_0[X_1, ..., X_n]$.

b) Il existe une famille $(a_1, ..., a_d)$ d’éléments de $H$, tous homogènes d’un même degré $> 0$, avec $d = \dim_H(M)$, et telle que $(a_1/1, ..., a_d/1)$ soit une suite sécante maximale pour le $S^{-1}H$-module $S^{-1}M$. Si de plus $H$ est engendré par $H_1$ comme $H_0$-algèbre, et si le corps résiduel de $H_0$ est infini, on peut prendre les $a_i$ de degré 1.

a) Posons $N = M / \sum_{i=1}^n a_i M$. On a $\dim_H(N) = \dim_{S^{-1}H}(S^{-1}N)$ d’après la prop. 4. Par suite, le $S^{-1}H$-module $S^{-1}N$ est de longueur finie si et seulement si le $H$-module $N$ est de longueur finie, c’est-à-dire si et seulement si $N$ est un $H_0$-module de type fini. Si $\varphi_*(M)$ est le module sur $H_0[X_1, ..., X_n]$ déduit de $M$ par l’homomorphisme $\varphi : H_0[X_1, ..., X_n] \to M$, on a $N = \varphi_*(M)/\sum_{i=1}^n X_i \cdot \varphi_*(M)$. Par suite (A, II, p. 171, cor. 3 et remarque) $\varphi_*(M)$ est un module de type fini sur $H_0[X_1, ..., X_n]$ si et seulement si $N$ est un $H_0$-module de type fini. Ceci prouve a).

Pour prouver b), nous établirons d’abord un lemme.

#### Lemme 4 {#ac-viii-s6-lem-4 .statement}

Soit $b$ un élément de $H$, homogène de degré $> 0$, et n’appartenant à aucun des éléments minimaux $p$ de $\mathrm{Supp}(M)$, tels que $\dim(H/p) = \dim_H(M)$. On a alors $\dim_H(M/bM) = \dim_H(M) - 1$.

Posons $d = \dim_H(M)$. D’après la définition de $b$, on a $\dim_H(M/bM) < d$. D’après la prop. 4, on a
$$
\dim_H(M/bM) = \dim_{S^{-1}H}(S^{-1}M/(b/1).S^{-1}M)
$$
et la formule (8) du § 3, no 2 fournit l’inégalité
$$
\dim_{S^{-1}H}(S^{-1}M/(b/1).S^{-1}M) \geq \dim_{S^{-1}H}(S^{-1}M) - 1 .
$$
Enfin, on a
$$
\dim_{S^{-1}H}(S^{-1}M) = \dim_H(M) = d
$$
d’après la prop. 4. On a donc $\dim_H(M/bM) \geq d - 1$, d’où le lemme 4.

Reprenons la démonstration de la prop. 6, b). On peut supposer $\dim_H(M) > 0$. Remarquons que tout élément minimal de $\mathrm{Supp}(M)$ est gradué (appliquer le lemme 1 du no 2 au quotient de $H$ par l’annulateur de $M$). D’après la prop. 8 de III, § 1, no 4, il existe donc un élément homogène $b$ de $H$, de degré $> 0$, n’appartenant à aucun des éléments minimaux $p$ de $\mathrm{Supp}(M)$ tels que $\dim(H/p) = \dim_H(M)$. D’après le lemme 4, on a $\dim_H(M/bM) = \dim_H(M) - 1$. Supposons de plus $H$ engendrée par $H_1$ comme $H_0$-algèbre et le corps résiduel $k$ de $H_0$ infini. Pour tout élément minimal $p$ de $\mathrm{Supp}(M)$, tel que $\dim(H/p) = \dim_H(M)$, considérons le sous-espace vectoriel $V_p = (p \cap H_1) \otimes_{H_0} k$ du $k$-espace vectoriel $V = H_1 \otimes_{H_0} k$. Si on avait $V_p = V$, on aurait $\mathfrak{p} \cap H_1 = H_1$ (II, § 3, n° 2, prop. 4), d’où $H_1 \subset \mathfrak{p}$ et $\dim_H(M) = \dim(H/\mathfrak{p}) \leq \dim(H/H_{\geq 1}) = 0$, ce qui n’est pas. Puisque $k$ est supposé infini, la réunion des $V_p$ est distincte de $V$; si $b \in H_1$ est tel que $b \otimes 1$ n’appartient à aucun des $V_p$, on a $\dim(M/bM) = \dim_H(M) - 1$.

Procédant par récurrence sur $d = \dim_H(M)$, on construit alors une suite $(b_1, ..., b_d)$ d’éléments de $H$, avec $b_i$ homogène de degré $n_i > 0$ et telle que $M / \sum_{i=1}^n b_i M$ soit un $H$-module de longueur finie. Si on suppose $H$ engendrée par $H_1$ comme $H_0$-algèbre et le corps résiduel de $H_0$ infini, on peut supposer $n_i = 1$ pour $i = 1, ..., d$. D’après la prop. 4, on a $\dim_{S^{-1}H}(S^{-1}M) = d$ et
$$
\dim_{S^{-1}H}(S^{-1}M / \sum_{i=1}^d (b_i/1).S^{-1}M) = 0 .
$$
Alors $(b_1/1, ..., b_d/1)$ est une suite sécante maximale pour le $S^{-1}H$-module $S^{-1}M$. Posons $a_i = b_i^{(n_1 ... n_d)/n_i}$ pour $1 \leq i \leq d$; alors les $a_i$ sont tous de même degré, et $(a_1/1, ..., a_d/1)$ est une suite sécante maximale pour $S^{-1}M$ (§ 3, n° 2, remarque 3).

#### Corollaire 1 {#ac-viii-s6-lem-4-cor-1 .statement}

*Supposons que $H_0$ soit un corps et que $H$ soit de type fini comme $H_0$-algèbre. Posons $n = \dim(H)$. Il existe des éléments homogènes $a_1, ..., a_n$ de $H$ tous de même degré $> 0$, tels que le $H_0$-homomorphisme $\varphi : H_0[X_1, ..., X_n] \to H$ défini par $\varphi(X_i) = a_i, i = 1, ..., n$, soit injectif et fasse de $H$ une $H_0[X_1, ..., X_n]$-algèbre finie. Si $H$ est engendrée par $H_1$ comme $H_0$-algèbre et si $H_0$ est infini, on peut supposer les $a_i$ de degré 1.*

Il existe d’après la prop. 6 un $H_0$-homomorphisme $\varphi$ de la forme indiquée qui fait de $H$ une $H_0[X_1, ..., X_n]$-algèbre finie. D’après le th. 1 du § 2, n° 3, on a alors
$$
\dim(H_0[X_1, ..., X_n]/(\mathrm{Ker}\ \varphi)) = \dim(H);
$$
comme on a
$$
\dim(H) = n = \dim(H_0[X_1, ..., X_n]),
$$
et que $H_0[X_1, ..., X_n]$ est intègre, ceci implique $\mathrm{Ker}\ \varphi = \{0\}$.

#### Remarque {#ac-viii-s6-n3-rem-2 .statement}

Soit $(h_1, ..., h_r)$ un système générateur fini du $H_0$-espace vectoriel $H_1$. Pour $\lambda = (\lambda_1, ..., \lambda_r) \in H_0^r$, posons $h_\lambda = \lambda_1 h_1 + \cdots + \lambda_r h_r$. Les démonstrations de la prop. 6 et du cor. 1 entraînent le résultat suivant : l’ensemble des éléments $(\lambda_1, ..., \lambda_n)$ de $(H_0^r)^n$ tels que les éléments $a_i = h_{\lambda_i} \in H_1$ satisfassent à la conclusion du cor. 1, contient le complémentaire de la réunion d’un nombre fini de sous-espaces vectoriels de $(H_0^r)^n$ distincts de l’espace entier.

#### Corollaire 2 {#ac-viii-s6-lem-4-cor-2 .statement}

*Soient $A$ un anneau local noethérien et $n \in \mathbf{N}$. Pour que l’on ait $\dim(A) \geq n$, il faut et il suffit que pour tout entier $r \geq 0$, on ait*
$$
[m_A^r/m_A^{r+1} : \kappa_A] \geq \binom{n+r-1}{n-1}, \quad \left( \text{resp. } \mathrm{long}_A(A/m_A^{r+1}) \geq \binom{n+r}{n} \right);
$$
*on a l’égalité pour tout $r$ si et seulement si $A$ est régulier de dimension $n$.*

La condition est suffisante (\S 4, n° 4, th. 3 et \S 5, n° 2, th. 1). Montrons qu’elle est nécessaire. Considérons l’anneau gradué gr(A) = gr_{m_A}(A); soit k une extension infinie du corps $\kappa_A$, et posons $H = k \otimes_{\kappa_A} \mathrm{gr}(A)$. L’anneau H est de dimension $\geq n$ (prop. 5 et son corollaire); on déduit donc du cor. 1 l’existence d’un homomorphisme gradué injectif de k-algèbres graduées $\varphi : H_0[X_1, ..., X_n] \to H$. On a par conséquent, pour tout entier $r \geq 0$,

$$
[\mathrm{gr}_r(A) : \kappa_A] = [H_r : H_0] \geq \binom{n + r - 1}{n - 1},
$$

et l’égalité pour tout $r$ implique la bijectivité de $\varphi$, donc la régularité de A (\S 5, n° 2, th. 1).

Les égalités

$$
\mathrm{long}_A(A/m_A^{r+1}) = \sum_{i=0}^r [\mathrm{gr}_i(A) : \kappa_A]
$$

et

$$
\binom{n + r}{n} = \sum_{i=0}^r \binom{n + i - 1}{n - 1}
$$

impliquent alors les assertions analogues pour la fonction $r \mapsto \mathrm{long}_A(A/m_A^{r+1})$.

### 4. Semi-continuité de la dimension

#### Lemme 5 {#ac-viii-s6-lem-5 .statement}

Soient A un anneau, r son radical, $R = \bigoplus_{i \in \mathbf{Z}} R_i$ une A-algèbre graduée, $M = \bigoplus_{i \in \mathbf{Z}} M_i$ un R-module gradué. On suppose que chaque $M_i$ est un A-module de type fini et que $M/rM$ est un $R/rR$-module de type fini. Alors M est un R-module de type fini.

Soient $m_1, ..., m_n$ des éléments homogènes de M, dont les images dans $M/rM$ engendrent le $R/rR$-module $M/rM$. Soit N le sous-R-module (gradué) de M engendré par $\{ m_1, ..., m_n \}$. Pour tout $i \in \mathbf{Z}$, on a $M_i = N_i + rM_i$, donc $M_i = N_i$ (II, \S 3, n° 2, prop. 4); par suite on a $M = N$.

#### Lemme 6 {#ac-viii-s6-lem-6 .statement}

Soient $\rho : B \to C$ un homomorphisme d’anneaux et S une partie multiplicative de B. On suppose que C est une B-algèbre de type fini, et que $S^{-1}C$ est une $S^{-1}B$-algèbre finie. Il existe alors $f \in S$ tel que $C_f$ soit une $B_f$-algèbre finie.

Soit X un ensemble générateur fini de la B-algèbre C. Pour tout $x \in X$, l’image de x dans $S^{-1}C$ est entière sur $S^{-1}B$, et il existe par conséquent un entier $n(x) \geq 0$, des éléments $b_1(x), ..., b_{n(x)}(x) \in B$ et un élément $f(x) \in S$ tels que

$$
f(x)\ x^{n(x)} + b_1(x)\ x^{n(x)-1} + \cdots + b_{n(x)} = 0.
$$

Soit $f = \prod_{x \in X} f(x)$; l’image de tout élément x de X dans $C_f$ est entière sur $B_f$, donc $C_f$ est une $B_f$-algèbre finie (V, \S 1, n° 1, prop. 4).

#### Proposition 7 {#ac-viii-s6-prop-7 .statement}

Supposons que H soit une $H_0$-algèbre de type fini. Alors la fonction $p \mapsto \dim(H \otimes_{H_0} \kappa(p))$ est semi-continue supérieurement sur $\mathrm{Spec}(H_0)$.

Puisque H est de type fini comme $H_0$-algèbre, chaque $H_i$ est un $H_0$-module de type fini (III, § 1, no 2, corollaire à la prop. 1) et H est engendrée comme $H_0$-algèbre par $H_0 \oplus H_1 \oplus \cdots \oplus H_r$ pour un entier $r \geq 0$ convenable. Soit $p \in \mathrm{Spec}(H_0)$ et posons $\dim(H \otimes_{H_0} \kappa(p)) = n \geq 0$. D’après le corollaire 1 à la prop. 6, il existe des éléments $a_1, ..., a_n$ de H, tous homogènes de même degré $d > 0$, tels que le $\kappa(p)$-homomorphisme $\overline{\varphi} : \kappa(p)[X_1, ..., X_n] \to H \otimes_{H_0} \kappa(p)$ qui applique $X_i$ sur $a_i \otimes 1$ pour $1 \leq i \leq n$, fasse de $H \otimes_{H_0} \kappa(p)$ une $\kappa(p)[X_1, ..., X_n]$-algèbre finie. Notons $\varphi$ le $H_0$-homomorphisme de $H_0[X_1, ..., X_n] = R$ dans H qui applique $X_i$ sur $a_i$ pour $1 \leq i \leq n$. Si l’on pose, pour tout $m \in \mathbf{Z}$, $H'_m = \sum_{(m-1)d < i \leq md} H_i$, on obtient une graduation de type $\mathbf{Z}$ sur H, compatible avec la structure de R-module donnée par $\varphi$. Chaque $H'_m$ est de type fini sur $H_0$. D’après le lemme 5, $H_p$ est un $R_p$-module de type fini. D’après le lemme 6, il existe donc $f \in H_0 - p$ tel que $H_f$ soit un $R_f$-module de type fini. Pour tout $q \in \mathrm{Spec}(H_0)_f$, $H \otimes_{H_0} \kappa(q)$ est une $\kappa(q)[X_1, ..., X_n]$-algèbre finie, donc $\dim(H \otimes_{H_0} \kappa(q)) \leq n$ (\S 2, no 3, th. 1), ce qui achève la démonstration.

#### Remarque 1 {#ac-viii-s6-n4-rem-1 .statement}

\* En géométrie algébrique, la prop. 7 implique que la dimension des fibres d’un morphisme projectif de variétés algébriques est semi-continue supérieurement. \*
2) Nous verrons plus tard que si $\rho : A \to B$ est un homomorphisme d’anneaux qui fasse de B une A-algèbre de type fini, la fonction $q \mapsto \dim_q(B \otimes_A \kappa(\rho^{-1}(q)))$ est semi-continue supérieurement sur $\mathrm{Spec}(B)$ (cf. p. 101, exerc. 10).

### 5. Algèbres graduées régulières

Dans ce numéro, on suppose que $H_0$ est un corps et que H est une $H_0$-algèbre de type fini.

On pose $H_+ = H_{\geq 1}$; c’est un idéal maximal de H. L’anneau $S^{-1}H$ s’identifie à l’anneau local $H_{H_+}$ de H en l’idéal $H_+$; son idéal maximal est $(H_+ )_{H_+} = S^{-1}H_+$, son corps résiduel s’identifie à $H_0$.

#### Proposition 8 {#ac-viii-s6-prop-8 .statement}

a) On a $\dim(H) \leq [H_+/H_+^2 : H_0]$.
b) Les conditions suivantes sont équivalentes :
(i) $\dim(H) = [H_+/H_+^2 : H_0]$;
(ii) l’anneau local noethérien $S^{-1}H$ est régulier ;
(iii) H est engendré comme $H_0$-algèbre par une famille d’éléments homogènes de degrés $> 0$, algébriquement indépendants sur $H_0$.
c) Supposons les conditions de b) satisfaites, et soient $a_1, ..., a_n \in H$ des éléments homogènes de degrés $> 0$. Les conditions suivantes sont équivalentes :
(i) les classes des $a_i$ forment une base du $H_0$-espace vectoriel $H_+/H_+^2$;
(ii) les $a_i/1$ forment un système de coordonnées de l’anneau local noethérien régulier $S^{-1}H$;

(iii) les $a_i$ sont algébriquement indépendants sur $H_0$ et engendrent $H$ comme $H_0$-algèbre.

On a $\dim(H) = \dim(S^{-1}H)$ (n° 2, th. 1), et $[H_+/H_+^2 : H_0] = [(S^{-1}H_+)/ (S^{-1}H_+)^2 : H_0]$ (II, § 3, n° 3, prop. 9); d’après le § 5, n° 1, cela entraîne $a$ et les équivalences (i) $\Leftrightarrow$ (ii) dans $b$ et $c$. Les deux implications (iii) $\Rightarrow$ (i) dans $b$ et $c$ sont triviales. Démontrons les implications (i) $\Rightarrow$ (iii). Supposons donc qu’on ait $\dim(H) = [H_+/H_+^2 : H_0]$ et soient $a_1, ..., a_n$ des éléments homogènes de $H$, de degrés $> 0$, dont les classes forment une base de $H_+/H_+^2$; considérons l’homomorphisme d’algèbres graduées $\varphi : H_0[X_1, ..., X_n] \to H$ qui envoie $X_i$ sur $a_i$. L’idéal $H_+$ de $H$ est engendré par les $a_i$ (A, II, p. 171, cor. 2 et remarque); par conséquent l’homomorphisme $\varphi$ est surjectif (III, § 1, n° 2, prop. 1). Mais on a

$$
\dim(H_0[X_1, ..., X_n]) = n = \dim(H) = \dim(H_0[X_1, ..., X_n]/(\mathrm{Ker}\, \varphi))
$$

(§ 2, n° 4, cor. 1 du th. 3), donc $\mathrm{Ker}\, \varphi = 0$ puisque $H_0[X_1, ..., X_n]$ est intègre. Cela implique les assertions (iii).

Sous les hypothèses de $b$, on dit que $H$ est une $H_0$-algèbre graduée régulière, ou une $H_0$-algèbre graduée de polynômes. Sous les hypothèses de $c$, on dit que les $a_i$ forment un système de coordonnées gradué de $H$.

#### Remarque 1 {#ac-viii-s6-n5-rem-1 .statement}

Avec les notations de $c$, soit $d_i$ le degré de $a_i$ ($1 \leq i \leq n$). Alors la série de Poincaré $P_H = \sum_{n \in \mathbf{Z}} [H_n : H_0]. T^n$ est égale à $\prod_i (1 - T^{d_i})^{-1}$ (§ 4, n° 2, exemple 1).
Par conséquent, si $H$ est une $H_0$-algèbre graduée de polynômes, on a

$$
P_H = \prod_n (1 - T^n)^{-\delta(n)}, \quad \text{avec} \quad \delta(n) = [(H_+/H_+^2)_n : H_0].
$$

#### Remarque 2 {#ac-viii-s6-n5-rem-2 .statement}

Inversement, le fait qu’il existe des entiers $d_i > 0$ tels que $P_H = \prod_i (1 - T^{d_i})^{-1}$ n’implique pas que $H$ soit une algèbre graduée de polynômes; par exemple, si $H$ est engendrée par un élément $X$ de degré 1 et un élément $Y$ de degré 2, soumis à la seule relation $X^2 = 0$, on a $P_H = (1 - T)^{-1}$.

## EXERCICES {#ac-viii-s6-exercises}

See the [exercises for § 6](exercises/s6/).
