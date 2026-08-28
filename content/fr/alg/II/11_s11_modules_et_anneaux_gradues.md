---
book: alg
book_title: Algebra
chapter: II
chapter_title: ALGÈBRE LINÉAIRE
section: 11
section_title: Modules et anneaux gradués
lang: fr
source: alg-i-iii-fr
pdf_pages: 0340-0353, 0386-0387
extraction: ocr
subsections:
    - "no": 1
      title: Groupes commutatifs gradués
      page: 0
      pdf_page: 340
    - "no": 2
      title: Anneaux et modules gradués
      page: 164
      pdf_page: 341
    - "no": 3
      title: Sous-modules gradués
      page: 0
      pdf_page: 344
    - "no": 4
      title: Cas d’un groupe des degrés ordonné
      page: 170
      pdf_page: 347
    - "no": 5
      title: Produit tensoriel gradué de modules gradués
      page: 173
      pdf_page: 350
    - "no": 6
      title: Modules gradués d’homomorphismes gradués
      page: 174
      pdf_page: 351
statements: 34
exercises: 1
content_sha256: b47e2f7501b600faa17f06a2c6b1c731b715b6679f70aecc6250626bcea6a495
---

## § 11. MODULES ET ANNEAUX GRADUÉS

A partir du n° 2 de ce paragraphe, Δ désignera un monoïde (I, p. 12) commutatif, noté additivement, ayant un élément neutre noté 0.

### 1. Groupes commutatifs gradués

Nous allons traduire dans un autre langage les définitions relatives aux sommes directes (II, p. 17).

#### Définition 1 {#alg-ii-s11-def-1 .statement}

Étant donnés un groupe commutatif G noté additivement et un ensemble Δ, on appelle graduation de type Δ sur G une famille $(G_\lambda)_{\lambda \in \Delta}$ de sous-groupes de G, dont G est somme directe. L’ensemble G, muni de la structure définie par sa loi de groupe et sa graduation, est appelé groupe (commutatif) gradué de type Δ.

On dit que Δ est l’ensemble des degrés de G. On dit qu’un élément $x \in G$ est homogène s’il appartient à un des $G_\lambda$, homogène de degré λ si $x \in G_\lambda$. L’élément 0 est donc homogène de tous les degrés ; mais si $x \neq 0$ est homogène, il appartient à un seul des $G_\lambda$ ; l’indice λ tel que $x \in G_\lambda$ est alors appelé le degré de x (ou quelquefois le poids de x) et se note parfois $\operatorname{deg}(x)$. Tout $y \in G$ s’écrit d’une seule manière comme somme $\sum_\lambda y_\lambda$ d’éléments homogènes, avec $y_\lambda \in G_\lambda$ ; on dit que $y_\lambda$ est la composante homogène de degré λ (ou simplement la composante de degré λ) de y. Lorsqu’on utilise le mot « poids » au lieu de « degré », on remplace l’adjectif « homogène » par « isobare ».

#### Exemple 1 {#alg-ii-s11-n1-exa-1 .statement}

Étant donnés un monoïde commutatif Δ quelconque (ayant un élément neutre 0) et un groupe commutatif quelconque G, on définit une graduation $(G_\lambda)_{\lambda \in \Delta}$ sur G en prenant $G_0 = G$ et $G_\lambda = \{0\}$ pour $\lambda \neq 0$ ; cette graduation est dite triviale.

#### Exemple 2 {#alg-ii-s11-n1-exa-2 .statement}

Soient Δ, Δ’ deux ensembles, ρ une application de Δ dans Δ’. Soit $(G_\lambda)_{\lambda \in \Delta}$ une graduation de type Δ sur un groupe commutatif G ; pour $\mu \in \Delta'$, soit $G'_\mu$ la somme des $G_\lambda$ tels que $\rho(\lambda) = \mu$ ; il est clair que $(G'_\mu)_{\mu \in \Delta'}$ est une graduation de type Δ’ sur G, dite déduite de $(G_\lambda)$ au moyen de l’application ρ.

Lorsque Δ est un groupe commutatif, noté additivement, et ρ l’application $\lambda \mapsto -\lambda$ de Δ sur lui-même, on dit que $(G'_\mu)$ est la graduation opposée de $(G_\lambda)$.

#### Exemple 3 {#alg-ii-s11-n1-exa-3 .statement}

Si $\Delta = \Delta_1 \times \Delta_2$ est un produit de deux ensembles, on dit qu’une graduation de type Δ est une bigraduation de types $\Delta_1, \Delta_2$. Pour tout $\lambda \in \Delta_1$, posons $G'_\lambda = \bigoplus_{\mu \in \Delta_2} G_{\lambda \mu}$, et pour tout $\mu \in \Delta_2$, posons $G''_\mu = \bigoplus_{\lambda \in \Delta_1} G_{\lambda \mu}$ ; il est clair que $(G'_\lambda)_{\lambda \in \Delta_1}$ est une graduation de type $\Delta_1$ et $(G''_\mu)_{\mu \in \Delta_2}$ une graduation de type $\Delta_2$ sur G ; on dit que ces graduations sont les graduations partielles déduites de la bigraduation $(G_{\lambda \mu})$. On notera que l’on a $G_{\lambda \mu} = G'_\lambda \cap G''_\mu$ ; inversement, si $(G'_\lambda)_{\lambda \in \Delta_1}$ et $(G''_\mu)_{\mu \in \Delta_2}$ sont deux graduations sur G telles que G soit somme directe des

G_{\lambda,\mu} = G'_\lambda \cap G''_\mu, ces sous-groupes forment une bigraduation de types $\Delta_1, \Delta_2$ sur G, dont $(G'_\lambda)$ et $(G''_\mu)$ sont les graduations partielles. Nous laissons au lecteur le soin de généraliser au cas où $\Delta$ est un produit fini d’ensembles.

#### Exemple 4 {#alg-ii-s11-n1-exa-4 .statement}

Soient $\Delta_0$ un monoïde commutatif noté additivement, ayant un élément neutre noté 0 ; soit I un ensemble quelconque, et désignons par $\Delta_0^{(I)} = \Delta$ le sous-monoïde du produit $\Delta_0^I$ formé des familles $(\lambda_i)_{i \in I}$ de support fini. Soit $\rho : \Delta \to \Delta_0$ l’homomorphisme (codiagonal) surjectif de $\Delta$ dans $\Delta_0$ défini par $\rho((\lambda_i)) = \sum_{i \in I} \lambda_i$. De toute graduation de type $\Delta$ on déduit au moyen de $\rho$ une graduation de type $\Delta_0$ (*Exemple 2*) ; on dit que c’est la *graduation totale* associée à la « multigraduation » donnée de type $\Delta$.

Les définitions et exemples de ce n° s’étendent aussitôt au cas où G est un groupe *non nécessairement commutatif* ; il faut simplement remplacer partout la notion de somme directe par celle de « somme restreinte » (II, p. 15, *Remarque*). On notera que dans ce cas les $G_\lambda$ sont des sous-groupes distingués de G et que pour $\lambda \neq \mu$, tout élément de $G_\lambda$ est permutable à tout élément de $G_\mu$.

### 2. Anneaux et modules gradués

#### Définition 2 {#alg-ii-s11-def-2 .statement}

Étant donnés un anneau $\mathbf{A}$ et une graduation $(\mathbf{A}_\lambda)$ de type $\Delta$ sur le groupe additif $\mathbf{A}$, on dit que cette graduation est compatible avec la structure d’anneau de $\mathbf{A}$ si l’on a

(1)
$$
\mathbf{A}_\lambda \mathbf{A}_\mu \subset \mathbf{A}_{\lambda+\mu} \quad \text{quels que soient } \lambda, \mu \text{ dans } \Delta.
$$

L’anneau $\mathbf{A}$, muni de cette graduation, est alors appelé anneau gradué de type $\Delta$.

#### Proposition 1 {#alg-ii-s11-prop-1 .statement}

Si tout élément de $\Delta$ est simplifiable et si $(\mathbf{A}_\lambda)$ est une graduation de type $\Delta$ compatible avec la structure d’un anneau $\mathbf{A}$, $\mathbf{A}_0$ est un sous-anneau de $\mathbf{A}$ (et en particulier on a $1 \in \mathbf{A}_0$).

Comme $\mathbf{A}_0 \mathbf{A}_0 \subset \mathbf{A}_0$ par définition, il suffit de prouver que $1 \in \mathbf{A}_0$. Soit $1 = \sum_{\lambda \in \Delta} e_\lambda$ la décomposition de 1 en ses composantes homogènes. Si $x \in \mathbf{A}_\mu$, on a $x = x.1 = \sum_{\lambda \in \Delta} x e_\lambda$; comparant les composantes de degré $\mu$, on obtient (puisque la relation $\mu + \lambda = \mu$ entraîne $\lambda = 0$) $x = x e_0$. Cette relation, étant vraie pour tout élément homogène de $\mathbf{A}$, est vraie pour tout $x \in \mathbf{A}$; en particulier $1 = 1.e_0 = e_0 \in \mathbf{A}_0$.

#### Définition 3 {#alg-ii-s11-def-3 .statement}

Soient $\mathbf{A}$ un anneau gradué de type $\Delta$, $(\mathbf{A}_\lambda)$ sa graduation, $\mathbf{M}$ un $\mathbf{A}$-module à gauche (resp. à droite) ; on dit qu’une graduation $(\mathbf{M}_\lambda)$ de type $\Delta$ sur le groupe additif $\mathbf{M}$ est compatible avec la structure de $\mathbf{A}$-module de $\mathbf{M}$ si l’on a

(2)
$$
\mathbf{A}_\lambda \mathbf{M}_\mu \subset \mathbf{M}_{\lambda+\mu} \quad \text{(resp. } \mathbf{M}_\mu \mathbf{A}_\lambda \subset \mathbf{M}_{\lambda+\mu})
$$
quels que soient $\lambda, \mu$ dans $\Delta$. Le module $\mathbf{M}$, muni de cette graduation, est alors appelé module gradué à gauche (resp. à droite) de type $\Delta$ sur l’anneau gradué $\mathbf{A}$.

Lorsque les éléments de $\Delta$ sont simplifiables, il résulte de (2) et de la prop. 1 que les $M_\lambda$ sont des $A_0$-modules.

Il est clair que si $A$ est un anneau gradué de type $\Delta$, le $A$-module à gauche $A_s$ (resp. le $A$-module à droite $A_d$) est gradué de type $\Delta$.

#### Exemple 1 {#alg-ii-s11-n2-exa-1 .statement}

Sur un anneau quelconque $A$, la graduation triviale de type $\Delta$ est compatible avec la structure d’anneau. Si $A$ est gradué par la graduation triviale, pour qu’une graduation $(M_\lambda)$ de type $\Delta$ sur un $A$-module $M$ soit compatible avec la structure de $A$-module, il faut et il suffit que les $M_\lambda$ soient des *sous-modules* de $M$.

#### Exemple 2 {#alg-ii-s11-n2-exa-2 .statement}

Soient $A$ un anneau gradué de type $\Delta$, $M$ un $A$-module gradué de type $\Delta$, $\rho$ un homomorphisme de $\Delta$ dans un monoïde commutatif $\Delta'$ dont l’élément neutre est noté 0. Alors $A$ est un anneau gradué de type $\Delta'$ et $M$ un $A$-module gradué de type $\Delta'$ pour les graduations de type $\Delta'$ déduites de $\rho$ et des graduations de type $\Delta$ sur $A$ et $M$ par le procédé de II, p. 163, *Exemple 2*: cela résulte aussitôt de la relation $\rho(\lambda + \mu) = \rho(\lambda) + \rho(\mu)$.

En particulier, si $\Delta = \Delta_1 \times \Delta_2$ est un produit de deux monoïdes commutatifs, les projections $pr_1$ et $pr_2$ sont des homomorphismes et les graduations correspondantes ne sont autres que les *graduations partielles* déduites des graduations de type $\Delta$ (II, p. 163, *Exemple 3*); ces graduations partielles sont donc compatibles avec la structure d’anneau de $A$ et la structure de module de $M$.

De même, si $\Delta = \Delta_0^{(I)}$ (où $\Delta_0$ est un monoïde commutatif ayant un élément neutre noté 0), la *graduation totale* (II, p. 164, *Exemple 4*) de type $\Delta_0$ déduite de la graduation de type $\Delta$ de $A$ (resp. $M$) au moyen de l’homomorphisme codiagonal est compatible avec la structure d’anneau de $A$ (resp. avec la structure de module de $M$).

#### Exemple 3 {#alg-ii-s11-n2-exa-3 .statement}

Soient $A$ un anneau gradué de type $\Delta$, $M$ un $A$-module gradué de type $\Delta$, $\lambda_0$ un élément de $\Delta$; pour tout $\lambda \in \Delta$, soit $M'_\lambda = M_{\lambda + \lambda_0}$, et soit $M'$ le $\mathbf{Z}$-module $\bigoplus_{\lambda \in \Delta} M'_\lambda$. Comme $A_\lambda M'_\mu \subset M_{\lambda + \mu + \lambda_0} = M'_{\lambda + \mu}$, $M'$ est un $A$-module et les $M'_\lambda$ forment sur $M'$ une graduation de type $\Delta$ compatible avec la structure de $A$-module de $M'$; on dit que le $A$-module gradué $M'$ de type $\Delta$ ainsi défini est obtenu par *décalage de $\lambda_0$* de la graduation de $M$, et on le note $M(\lambda_0)$. Lorsque $\Delta$ est un *groupe*, le $A$-module sous-jacent au $A$-module gradué $M'$ s’identifie à $M$.

#### Exemple 4 {#alg-ii-s11-n2-exa-4 .statement}

Soit $B$ un anneau commutatif. L’anneau de polynômes $B[X]$ à une indéterminée est gradué de type $\mathbf{N}$ par les sous-groupes $BX^n$ ($n \geqslant 0$) (cf. III, p. 25, et IV).*

#### Exemple 5 {#alg-ii-s11-n2-exa-5 .statement}

Soient $B$ un anneau commutatif, $E$ un $B$-module, $Q$ une forme quadratique sur $E$, $C(Q)$ l’algèbre de Clifford de $Q$ (cf. IX, § 9). Les sous-B-modules $C^+(Q)$ et $C^-(Q)$ forment sur $C(Q)$ une graduation de type $\mathbf{Z}/2\mathbf{Z}$ compatible avec la structure d’anneau de $C(Q)$.*

type $\mathbf{Z}^n$; lorsqu’on parle d’anneaux ou de modules *gradués* (resp. *bigradués*, *trigradués*, etc.) sans préciser de quel type, il est sous-entendu qu’il s’agit de graduations de type $\mathbf{Z}$ (resp. $\mathbf{Z}^2, \mathbf{Z}^3$, etc.); on dit aussi qu’un anneau (resp. module) gradué de type $\mathbf{N}$ est un anneau (resp. module) *gradué à degrés positifs*.

2) Les $\mathbf{Z}$-modules gradués de type $\Delta$, lorsque $\mathbf{Z}$ est muni de la graduation triviale, ne sont autres que les groupes commutatifs gradués (dont l’ensemble des degrés est un monoïde commutatif) de II, p. 163, déf. 1.

#### Définition 4 {#alg-ii-s11-def-4 .statement}

*Soient A, A' deux anneaux gradués de même type $\Delta$, $(A_\lambda), (A'_\lambda)$ leurs graduations respectives. On dit qu’un homomorphisme d’anneaux $h : A \to A'$ est gradué si l’on a $h(A_\lambda) \subset A'_\lambda$ pour tout $\lambda \in \Delta$.

Soient $M, M'$ deux modules gradués de type $\Delta$ sur un anneau gradué $A$ de type $\Delta$. Soient $u : M \to M'$ un $A$-homomorphisme et $\delta$ un élément de $\Delta$; on dit que $u$ est gradué de degré $\delta$ si l’on a $u(M_\lambda) \subset M_{\lambda + \delta}$ pour tout $\lambda \in \Delta$.

Soient $A$ un anneau gradué de type $\Delta$, $A'$ un anneau gradué de type $\Delta'$, $\rho : \Delta \to \Delta'$ un homomorphisme. On dit qu’un homomorphisme d’anneaux $h : A \to A'$ est *gradué* si $h$ est un homomorphisme gradué d’anneaux gradués de type $\Delta'$, lorsque l’on munit $A$ de la graduation de type $\Delta'$ déduite de sa graduation de type $\Delta$ au moyen de $\rho$ (II, p. 163, *Exemple 2*); cela signifie donc que $h(A_\lambda) \subset A'_{\rho(\lambda)}$ pour tout $\lambda \in \Delta$.

On dit qu’un $A$-homomorphisme $u : M \to M'$ est *gradué* s’il existe $\delta \in \Delta$ tel que $u$ soit gradué de degré $\delta$. Si $u \neq 0$ et si tout élément de $\Delta$ est *simplifiable*, le degré $\delta$ de $u$ est alors déterminé de façon *unique*.

Si $h : A \to A', h' : A' \to A''$ sont deux homomorphismes gradués d’anneaux gradués de type $\Delta$, il en est de même de $h' \circ h : A \to A''$; pour qu’une application $h : A \to A'$ soit un *isomorphisme* d’anneaux gradués, il faut et il suffit que $h$ soit bijective et que $h$ et l’application réciproque $h'$ soient des homomorphismes gradués; il suffit d’ailleurs pour cela que $h$ soit un homomorphisme gradué bijectif. On voit donc qu’on peut prendre pour *morphismes* de l’espèce de structure d’anneau gradué de type $\Delta$ les homomorphismes gradués (E, IV, p. 11).

De même, si $u : M \to M'$ et $u' : M' \to M''$ sont deux homomorphismes gradués de $A$-modules gradués de type $\Delta$, de degrés respectifs $\delta$ et $\delta'$, $u' \circ u : M \to M''$ est un homomorphisme gradué de degré $\delta + \delta'$. Si $\delta$ admet un opposé $-\delta$ dans $\Delta$ et si $u : M \to M'$ est un homomorphisme gradué bijectif de degré $\delta$, l’application réciproque $u' : M' \to M$ est un homomorphisme gradué bijectif de degré $-\delta$. On en conclut comme ci-dessus qu’on peut prendre pour *morphismes* de l’espèce de structure de $A$-module gradué de type $\Delta$ les *homomorphismes gradués de degré* 0. Mais un homomorphisme gradué bijectif $u : M \to N$ de degré $\neq 0$ n’est pas un isomorphisme de $A$-modules gradués si $M$ et $N$ ne sont pas réduits à 0 et si les éléments de $\Delta$ sont simplifiables.

#### Exemple 6 {#alg-ii-s11-n2-exa-6 .statement}

Si $M$ est un $A$-module gradué, $M(\lambda_0)$ un $A$-module gradué obtenu par décalage (II, p. 165, *Exemple 3*), l’application $\mathbf{Z}$-linéaire de $M(\lambda_0)$ dans $M$ qui coïncide avec l’injection canonique dans chaque $M_{\lambda + \lambda_0}$, est un homomorphisme gradué de degré $\lambda_0$ (qui est bijectif lorsque $\Delta$ est un *groupe*).

#### Exemple 7 {#alg-ii-s11-n2-exa-7 .statement}

Si $a$ est un élément homogène de degré $\delta$ appartenant au centre de $A$, l’homothétie $x \mapsto ax$ d’un $A$-module gradué quelconque $M$ est un homomorphisme gradué de degré $\delta$.

Remarque 3). — On dit qu’un $A$-module gradué $M$ est un $A$-module gradué libre s’il existe une base $(m_i)_{i \in I}$ de $M$ formée d’éléments *homogènes*. Supposons qu’il en soit ainsi et que $\Delta$ soit un *groupe* commutatif; soit $\lambda_i$ le degré de $m_i$, et considérons pour chaque $i$ le $A$-module décalé $A(-\lambda_i)$ (II, p. 165, *Exemple 3*); si on désigne par $e_i$ l’élément 1 de $A$, considéré comme élément *de degré* $\lambda_i$ dans $A(-\lambda_i)$, l’application $A$-linéaire $u : \bigoplus_{i \in I} A(-\lambda_i) \to M$ telle que $u(e_i) = m_i$ pour tout $i$, est un *isomorphisme de $A$-modules gradués*.

Supposant toujours que $\Delta$ est un groupe commutatif, soient maintenant $N$ un $A$-module gradué, $(n_i)_{i \in I}$ un système de générateurs *homogènes* de $N$, et supposons que $n_i$ soit de degré $\mu_i$. Alors l’application $A$-linéaire $v : \bigoplus_{i \in I} A(-\mu_i) \to N$ telle que $u(e_i) = n_i$ pour tout $i$ est un *homomorphisme surjectif de degré 0 de $A$-modules gradués*. Si $N$ est un $A$-module gradué *de type fini*, il y a toujours un système fini de générateurs homogènes de $N$, et on aura donc un homomorphisme surjectif du type précédent avec $I$ *finit*.

### 3. Sous-modules gradués

#### Proposition 2 {#alg-ii-s11-prop-2 .statement}

Soient $A$ un anneau gradué de type $\Delta$, $M$ un $A$-module gradué de *type* $\Delta$, $(M_\lambda)$ sa graduation, $N$ un sous-$A$-module de $M$. Les propriétés suivantes sont équivalentes:

a) $N$ est somme de la famille $(N \cap M_\lambda)_{\lambda \in \Delta}$.
b) *Les composantes homogènes de tout élément de $N$ appartiennent à $N$*.
c) $N$ est engendré *par des éléments homogènes*.

Tout élément de $N$ s’écrivant d’une seule manière comme somme d’éléments des $M_\lambda$, il est immédiat que a) et b) sont équivalentes et que a) entraîne c). Montrons que c) implique b). Soit donc $(x_i)_{i \in I}$ une famille de générateurs homogènes $\neq 0$ de $N$, et soit $\delta(i)$ le degré de $x_i$. Tout élément de $N$ s’écrit $\sum_i a_i x_i$ avec $a_i \in A$; si $a_{i,\lambda}$ est la composante de degré $\lambda$ de $a_i$, la conclusion résulte de la relation

$$
\sum_{i \in I} \left( \sum_{\mu \in \Delta} a_{i,\mu} x_i \right) = \sum_{\lambda \in \Delta} \left( \sum_{\mu + \delta(i) = \lambda} a_{i,\mu} x_i \right).
$$

Remarque 1). — Avec les notations précédentes, la relation $\sum_{i \in I} a_i x_i = 0$ est donc équivalente au système de relations $\sum_{\mu + \delta(i) = \lambda} a_{i,\mu} x_i = 0$. Lorsque $\Delta$ est un groupe, ces relations s’écrivent $\sum_{i \in I} a_{i,\lambda - \delta(i)} x_i = 0$.

Lorsqu’un sous-module N de M vérifie les propriétés équivalentes énoncées dans la prop. 2, il est clair que les $N \cap M_\lambda$ forment une graduation compatible avec la structure de A-module de N, appelée graduation induite par celle de M; on dit que N, muni de cette graduation, est un sous-module gradué de M.

#### Corollaire 1 {#alg-ii-s11-prop-2-cor-1 .statement}

Si N est un sous-module gradué de M et si $(x_i)$ est un système générateur de N, les composantes homogènes des $x_i$ forment un système générateur de N.

#### Corollaire 2 {#alg-ii-s11-prop-2-cor-2 .statement}

Si N est un sous-module gradué de type fini de M, N admet un système générateur fini formé d’éléments homogènes.

Il suffit d’appliquer le cor. 1 en remarquant qu’un élément de M n’a qu’un nombre fini de composantes homogènes $\neq 0$.

Un sous-module gradué de $A_s$ (resp. $A_d$) est appelé idéal à gauche (resp. à droite) gradué de l’anneau gradué A. Pour tout sous-anneau B de A on a $(B \cap A_\lambda)(B \cap A_\mu) \subset B \cap A_{\lambda+\mu}$; si B est un sous-$\mathbf{Z}$-module gradué de A, la graduation induite sur B par celle de A est donc compatible avec la structure d’anneau de B; on dit alors que B est un sous-anneau gradué de A.

Il est clair que si N (resp. B) est un sous-A-module gradué de M (resp. un sous-anneau gradué de A), l’injection canonique $N \to M$ (resp. $B \to A$) est un homomorphisme gradué de modules de degré 0 (resp. un homomorphisme gradué d’anneaux).

Si N est un sous-module gradué d’un A-module gradué M et $(M_\lambda)_{\lambda \in \Delta}$ la graduation de M, les sous-modules $(M_\lambda + N)/N$ de $M/N$ forment une graduation compatible avec la structure de ce module quotient. En effet, si $N_\lambda = M_\lambda \cap N$, $(M_\lambda + N)/N$ s’identifie à $M_\lambda/N_\lambda$, et il résulte de II, p. 167, prop. 2 et II, p. 14, formule (26), que $M/N$ est leur somme directe. En outre, on a $A_\lambda(M_\mu + N) \subset A_\lambda M_\mu + N \subset M_{\lambda+\mu} + N$, donc $A_\lambda((M_\mu + N)/N) \subset (M_{\lambda+\mu} + N)/N$, ce qui établit notre assertion. On dit que la graduation $((M_\lambda + N)/N)_{\lambda \in \Delta}$ est la graduation quotient de celle de M par N, et le module quotient $M/N$, muni de cette graduation, s’appelle le module gradué quotient de M par le sous-module gradué N; l’homomorphisme canonique $M \to M/N$ est un homomorphisme gradué de degré 0 pour cette graduation.

Si $b$ est un idéal bilatère gradué de A, la graduation quotient sur $A/b$ est compatible avec la structure d’anneau de $A/b$; l’anneau $A/b$, muni de cette graduation, s’appelle l’anneau gradué quotient de A par $b$; l’homomorphisme canonique $A \to A/b$ est un homomorphisme d’anneaux gradués pour cette graduation.

#### Proposition 3 {#alg-ii-s11-prop-3 .statement}

Soient A un anneau gradué de type $\Delta$, M et N deux A-modules gradués de type $\Delta$, $u : M \to N$ un A-homomorphisme gradué de degré $\delta$. Alors:
(i) $\operatorname{Im}(u)$ est un sous-module gradué de N.

(ii) Si $\delta$ est un élément simplifiable de $\Delta$, $\mathrm{Ker}(u)$ est un sous-module gradué de $M$.
(iii) Si $\delta = 0$, la bijection $M / \mathrm{Ker}(u) \to \mathrm{Im}(u)$ canoniquement associée à $u$ est un isomorphisme de modules gradués.

L’assertion (i) découle aussitôt des définitions et de la prop. 2, c) (II, p. 167). Si $x$ est un élément de $M$ tel que $u(x) = 0$ et si $x = \sum_{\lambda} x_{\lambda}$ est sa décomposition en composantes homogènes (où $x_{\lambda}$ est de degré $\lambda$), on a $\sum_{\lambda} u(x_{\lambda}) = u(x) = 0$ et $u(x_{\lambda})$ est de degré $\lambda + \delta$; si $\delta$ est simplifiable, la relation $\lambda + \delta = \mu + \delta$ entraîne $\lambda = \mu$, donc les $u(x_{\lambda})$ sont les composantes homogènes de $u(x)$, et on a nécessairement $u(x_{\lambda}) = 0$ pour tout $\lambda \in \Delta$, ce qui prouve (ii). La bijection $v : M / \mathrm{Ker}(u) \to \mathrm{Im}(u)$ canoniquement associée à $u$ est alors un homomorphisme gradué de degré $\delta$, comme il résulte de la définition de la graduation quotient; d’où (iii) lorsque $\delta = 0$.

#### Corollaire {#alg-ii-s11-n3-cor-1 .statement}

Soient $A, B$ deux anneaux gradués de type $\Delta$, $u : A \to B$ un homomorphisme gradué d’anneaux gradués. Alors $\mathrm{Im}(u)$ est un sous-anneau gradué de $B$, $\mathrm{Ker}(u)$ un idéal bilatère gradué de $A$, et la bijection $A / \mathrm{Ker}(u) \to \mathrm{Im}(u)$ canoniquement associée à $u$ est un isomorphisme d’anneaux gradués.

Il suffit d’appliquer la prop. 3 à $u$ considéré comme homomorphisme de degré 0 de $\mathbf{Z}$-modules gradués.

#### Proposition 4 {#alg-ii-s11-prop-4 .statement}

Soient $A$ un anneau gradué de type $\Delta$, $M$ un $A$-module gradué de type $\Delta$.
(i) Toute somme et toute intersection de sous-modules gradués de $M$ est un sous-module gradué.
(ii) Si $x$ est un élément homogène de $M$, de degré $\mu$ simplifiable dans $\Delta$, l’annulateur de $x$ est un idéal à gauche gradué de $A$.
(iii) Si tous les éléments de $\Delta$ sont simplifiables, l’annulateur d’un sous-module gradué de $M$ est un idéal bilatère gradué de $A$.

Si $(N_i)$ est une famille de sous-modules gradués de $M$, la propriété c) de la prop. 2 (II, p. 167) montre que la somme des $N_i$ est engendrée par des éléments homogènes, et la propriété b) de la prop. 2 (II, p. 167) prouve que les composantes homogènes de tout élément de $\bigcap_i N_i$ appartiennent à $\bigcap_i N_i$; d’où (i).

Pour démontrer (ii), il suffit de remarquer que $\mathrm{Ann}(x)$ est le noyau de l’homomorphisme $a \mapsto ax$ du $A$-module $A_s$ dans $M$ et que cet homomorphisme est gradué de degré $\mu$; la conclusion résulte de la prop. 3, (ii). Enfin (iii) est conséquence de (i) et (ii), car l’annulateur d’un sous-module gradué $N$ de $M$ est l’intersection des annulateurs des éléments homogènes de $N$, en vertu de la prop. 2 de II, p. 167.

Remarque 2). — Soient $M$ un $A$-module gradué, $E$ un sous-module de $M$; il résulte de la prop. 4, (i) qu’il existe un plus grand sous-module gradué $N'$ de $M$ contenu dans $E$ et un plus petit sous-module gradué $N''$ de $M$ contenant $E$; $N'$ est l’ensemble des $x \in E$ dont toutes les composantes homogènes appartiennent à $E$, et $N''$ est le sous-module de $M$ engendré par les composantes homogènes d’un système générateur de $E$.

#### Proposition 5 {#alg-ii-s11-prop-5 .statement}

*Soit $A$ un anneau gradué de type $\Delta$. Si tout élément de $\Delta$ est simplifiable, alors, pour tout élément homogène $a \in A$, le commutant de $a$ dans $A$ (I, p. 7) est un sous-anneau gradué de $A$.*

Supposons que $a$ soit de degré $\delta$; soit $b = \sum_{\lambda} b_{\lambda}$ un élément permutable à $a$, $b_{\lambda}$ étant la composante homogène de degré $\lambda$ de $b$ pour tout $\lambda \in \Delta$. On a par hypothèse $\sum_{\lambda} (ab_{\lambda} - b_{\lambda}a) = 0$ et $ab_{\lambda} - b_{\lambda}a$ est homogène de degré $\lambda + \delta$; comme $\delta$ est simplifiable, on en déduit que $ab_{\lambda} = b_{\lambda}a$ pour tout $\lambda$, ce qui prouve notre assertion.

#### Corollaire {#alg-ii-s11-n3-cor-2 .statement}

*Si tout élément de $\Delta$ est simplifiable, le commutant d’un sous-anneau gradué $B$ de $A$ (et en particulier le centre de $A$) est un sous-anneau gradué de $A$.*

C’est en effet l’intersection des commutants des éléments homogènes de $B$.

*Remarque 3).* — Un *système inductif* $(A_{\alpha}, \varphi_{\beta \alpha})$ *d’anneaux gradués de type* $\Delta$ (resp. un *système inductif* $(M_{\alpha}, f_{\beta \alpha})$ *de* $A_{\alpha}$*-modules gradués de type* $\Delta$) est un système inductif d’anneaux (resp. de $A_{\alpha}$*-modules) tel que chaque $A_{\alpha}$ (resp. $M_{\alpha}$) soit gradué de type $\Delta$ et que chaque $\varphi_{\beta \alpha}$ (resp. $f_{\beta \alpha}$) soit un *homomorphisme d’anneaux gradués* (resp. un $A_{\alpha}$*-homomorphisme de degré* $0$ *de modules gradués*). Si $(A_{\alpha}^{\lambda})_{\lambda \in \Delta}$ (resp. $(M_{\alpha}^{\lambda})_{\lambda \in \Delta}$) est la graduation de $A_{\alpha}$ (resp. $M_{\alpha}$) et si on pose $A = \lim_{\longrightarrow} A_{\alpha}$, $A^{\lambda} = \lim_{\longrightarrow} A_{\alpha}^{\lambda}$ (resp. $M = \lim_{\longrightarrow} M_{\alpha}$, $M^{\lambda} = \lim_{\longrightarrow} M_{\alpha}^{\lambda}$), il résulte de II, p. 91, prop. 5 que $(A^{\lambda})$ (resp. $(M^{\lambda})$) est une graduation de $A$ (resp. $M$), et il résulte de I, p. 115–117 que cette graduation est compatible avec la structure d’anneau de $A$ (resp. la structure de $A$*-module de $M$). On dit que l’anneau *gradué* $A$ (resp. le $A$*-module *gradué* $M$) est la *limite inductive* du système inductif d’anneaux gradués $(A_{\alpha}, \varphi_{\beta \alpha})$ (resp. de modules gradués $(M_{\alpha}, f_{\beta \alpha})$). Si $\varphi_{\alpha}: A_{\alpha} \to A$ (resp. $f_{\alpha}: M_{\alpha} \to M$) est l’application canonique, $\varphi_{\alpha}$ (resp. $f_{\alpha}$) est un homomorphisme d’anneaux gradués (resp. un homomorphisme de degré $0$ de $A_{\alpha}$*-modules gradués*).

### 4. Cas d’un groupe des degrés ordonné

Sur un groupe commutatif $\Delta$, noté additivement, on dit qu’une structure d’ordre (notée $\leqslant$) est *compatible* avec la structure de groupe si pour tout $\rho \in \Delta$, la relation $\lambda \leqslant \mu$ entraîne $\lambda + \rho \leqslant \mu + \rho$. Le groupe $\Delta$, muni de cette structure d’ordre, est alors appelé *groupe ordonné*. Nous étudierons en détail ces groupes dans VI, § 1; bornons-nous ici à remarquer que dans un tel groupe, la relation $\lambda > 0$ entraîne $\lambda + \mu > \mu$ pour tout $\mu$, car elle entraîne $\lambda + \mu \geqslant \mu$ par définition, et la relation $\xi + \mu = \mu$ équivaut à $\xi = 0$.

Soient $\Delta$ un groupe commutatif ordonné, $A$ un anneau gradué de type $\Delta$, $(A_{\lambda})$ sa graduation, et supposons que la relation $A_{\lambda} \neq \{0\}$ entraîne $\lambda \geqslant 0$; alors il résulte des définitions que $\mathfrak{J}_0 = \sum_{\lambda > 0} A_\lambda$ est un *idéal bilatère gradué* de $A$, en vertu de la remarque faite ci-dessus.

#### Proposition 6 {#alg-ii-s11-prop-6 .statement}

*Soient $\Delta$ un groupe commutatif ordonné, $A$ un anneau gradué de type $\Delta$, $(A_\lambda)$ sa graduation, $M$ un $A$-module gradué de type $\Delta$, $(M_\lambda)$ sa graduation. Supposons que la relation $A_\lambda \neq \{0\}$ implique $\lambda \geqslant 0$ et qu’il existe $\lambda_0$ tel que $M_{\lambda_0} \neq \{0\}$ et $M_\lambda = \{0\}$ pour $\lambda < \lambda_0$. Alors, si on pose $\mathfrak{J}_0 = \sum_{\lambda > 0} A_\lambda$, on a $\mathfrak{J}_0 M \neq M$.

Soit $x$ un élément non nul de $M_{\lambda_0}$; supposons que l’on ait $x \in \mathfrak{J}_0 M$. Alors $x = \sum_i a_i x_i$ où les $a_i$ sont des éléments homogènes $\neq 0$ de $\mathfrak{J}_0$, les $x_i$ des éléments homogènes $\neq 0$ de $M$, avec $\deg(x) = \deg(a_i) + \deg(x_i)$ pour tout $i$ (II, p. 167). Mais, comme $\deg(a_i) > 0$, on aurait alors $\lambda_0 = \deg(a_i) + \deg(x_i) > \deg(x_i)$, ce qui contredit l’hypothèse.

#### Corollaire 1 {#alg-ii-s11-prop-6-cor-1 .statement}

*Les hypothèses sur $\Delta$ et $A$ étant celles de la prop. 6, si $M$ est un $A$-module gradué de type fini tel que $\mathfrak{J}_0 M = M$, on a $M = \{0\}$.

Supposons $M \neq \{0\}$. Soit $\lambda_0$ un élément minimal de l’ensemble des degrés d’un système générateur fini formé d’éléments homogènes $\neq 0$ de $M$; alors les hypothèses de la prop. 6 seraient vérifiées, ce qui implique contradiction.

#### Corollaire 2 {#alg-ii-s11-prop-6-cor-2 .statement}

*Les hypothèses sur $\Delta$ et $A$ étant celles de la prop. 6, soient $M$ un $A$-module gradué de type fini, $N$ un sous-module gradué de $M$ tel que $N + \mathfrak{J}_0 M = M$; alors on a $N = M$.

En effet, $M/N$ est un $A$-module gradué de type fini, et l’hypothèse entraîne que $\mathfrak{J}_0 . (M/N) = M/N$; donc $M/N = 0$.

#### Corollaire 3 {#alg-ii-s11-prop-6-cor-3 .statement}

*Les hypothèses sur $\Delta$ et $A$ étant celles de la prop. 6, soit $u : M \to N$ un homomorphisme gradué de $A$-modules à droite gradués, $N$ étant supposé de type fini. Si l’homomorphisme*

$$
u \otimes 1 : M \otimes_A (A/\mathfrak{J}_0) \to N \otimes_A (A/\mathfrak{J}_0)
$$

*est surjectif, alors $u$ est surjectif.*

En effet, $u(M)$ est un sous-module gradué de $N$, et le $(A/\mathfrak{J}_0)$-module $(N/u(M)) \otimes_A (A/\mathfrak{J}_0)$ est isomorphe à $(N \otimes_A (A/\mathfrak{J}_0))/\mathrm{Im}(u \otimes 1)$ (II, p. 59, prop. 6). L’hypothèse entraîne donc $(N/u(M)) \otimes_A (A/\mathfrak{J}_0) = 0$, donc $N = u(M)$ en vertu du cor. 1.

#### Remarque {#alg-ii-s11-n4-rem-1 .statement}

Il résulte de la démonstration du cor. 1 que les cor. 1 et 2 (resp. le cor. 3) sont encore valables lorsqu’au lieu de supposer que $M$ (resp. $N$) est de type fini, on fait l’hypothèse suivante: il existe une partie $\Delta^+$ de $\Delta$ vérifiant les conditions suivantes:
$1^\circ$ pour $\lambda \notin \Delta^+$, on a $M_\lambda = \{0\}$ (resp. $N_\lambda = \{0\}$);
$2^\circ$ toute partie non vide de $\Delta^+$ possède un plus petit élément.
Ce sera le cas si $\Delta = \mathbf{Z}$ et si $M$ (resp. $N$) est un module gradué à degrés *positifs*.

#### Proposition 7 {#alg-ii-s11-prop-7 .statement}

*Supposons que $\Delta = \mathbf{Z}$. Les hypothèses sur $A$ et $M$ étant celles de la* prop. 6, on considère le $A_0$-module gradué $N = M / J_0 M$, et on suppose vérifiées les conditions suivantes:

(i) chacun des $N_\lambda$, considéré comme $A_0$-module, admet une base $(y_{i\lambda})_{i \in I_\lambda}$;
(ii) l’homomorphisme canonique $J_0 \otimes_A M \to M$ est injectif.

Alors $M$ est un $A$-module gradué libre (II, p. 167, Remarque 3), et de façon précise, si $x_{i\lambda}$ est un élément de $M_\lambda$ dont l’image dans $N_\lambda$ est $y_{i\lambda}$, la famille $(x_{i\lambda})_{(i, \lambda) \in I}$ (où $I$ est l’ensemble somme des $I_\lambda$) est une base de $M$.

On sait (II, p. 167, Remarque 3) qu’il y a un $A$-module gradué libre $L$ (de graduation $(L_\lambda)$) et un homomorphisme $p : L \to M$ de degré 0 tel que $p(e_{i\lambda}) = x_{i\lambda}$ pour tout $(i, \lambda) \in I$ (($e_{i\lambda}$)$_{(i, \lambda) \in I}$ étant une base de $L$ formée d’éléments homogènes $e_{i\lambda} \in L_\lambda$). Il résulte de la Remarque de II, p. 171, que $p$ est surjectif. Considérons le $A$-module gradué $R = \mathrm{Ker}(p)$, et notons que $R_\lambda = \{0\}$ pour $\lambda < \lambda_0$ par définition; il s’agit de prouver que $R = \{0\}$, et en vertu de la prop. 6 il suffira de montrer que l’on a $J_0 R = R$. Considérons le diagramme commutatif (II, p. 58, prop. 5).

$$
\begin{array}{ccccccccc}
J_0 \otimes R & \xrightarrow{1 \otimes j} & J_0 \otimes L & \xrightarrow{1 \otimes p} & J_0 \otimes M & \longrightarrow & 0 \\
\downarrow a & & \downarrow b & & \downarrow c & & \\
0 & \longrightarrow & R & \xrightarrow{j} & L & \xrightarrow{p} & M & \longrightarrow & 0
\end{array}
$$

où $j$ est l’injection canonique, $a, b, c$ les homomorphismes provenant de l’injection canonique $J_0 \to A$ (II, p. 55, prop. 4); il faut montrer que $a$ est surjectif. Notons que, comme $L$ est libre, $b$ est injectif (II, p. 63, cor. 6) et $c$ est injectif par hypothèse. Soit donc $t$ un élément de $R$, et soit $\bar{t}$ sa classe dans $R / J_0 R$; on a une suite exacte (II, p. 58, prop. 5 et II, p. 60, cor. 2)

$$
R / J_0 R \xrightarrow{\bar{j}} L / J_0 L \xrightarrow{\bar{p}} M / J_0 M \longrightarrow 0
$$

où $\bar{j}$ et $\bar{p}$ se déduisent de $j$ et $p$ par passage aux quotients, et $\bar{p}$ est par hypothèse une bijection; on a donc $\bar{j}(\bar{t}) = 0$, autrement dit $j(t) \in J_0 L$. Il y a donc un élément $z \in J_0 \otimes L$ tel que $j(t) = b(z)$; comme $p(b(z)) = 0$, on a $c((1 \otimes p)(z)) = 0$, et comme $c$ est injectif, $(1 \otimes p)(z) = 0$. Autrement dit, $z$ est l’image d’un élément $t' \in J_0 \otimes R$ par $1 \otimes j$, et on a alors $j(a(t')) = b(z) = j(t)$; comme $j$ est injectif, cela entraîne $t = a(t')$.

C.Q.F.D.

Nous montrerons plus tard (AC, II, § 3, n° 2, prop. 5) comment cette proposition peut s’étendre aux modules non gradués.

#### Lemme 1 {#alg-ii-s11-lem-1 .statement}

Pour qu’un groupe commutatif $\Delta$ soit tel qu’il existe sur $\Delta$ un ordre total compatible avec la structure de groupe de $\Delta$, il faut et il suffit que $\Delta$ soit sans torsion.

En effet, s’il existe une telle structure d’ordre sur $\Delta$ et si $\lambda > 0$, on a $\lambda + \mu > 0$ pour tout $\mu \geq 0$ et en particulier, par récurrence sur l’entier $n > 0$, $n.\lambda > 0$, ce qui prouve que $\Delta$ est sans torsion (puisque tout élément $\neq 0$ de $\Delta$ est, soit $> 0$, soit $< 0$). Inversement, si $\Delta$ est sans torsion, $\Delta$ est un sous-$\mathbf{Z}$-module d’un $\mathbf{Q}$-espace vectoriel (II, p. 117, cor. 1) qu’on peut supposer de la forme $\mathbf{Q}^{(I)}$; si on munit $I$ d’une structure de bon ordre (E, III, p. 20, th. 1) et $\mathbf{Q}$ de sa structure d’ordre usuelle, l’ensemble $\mathbf{Q}^{(1)}$, muni de l’ordre *lexicographique*, est totalement ordonné (E, III, p. 23); il est immédiat que cet ordre est compatible avec la structure de groupe additif de $\mathbf{Q}^{(1)}$.

C. Q.F.D.

#### Proposition 8 {#alg-ii-s11-prop-8 .statement}

*Soient $\Delta$ un groupe commutatif sans torsion, $A$ un anneau gradué de type $\Delta$. Si le produit dans $A$ de deux éléments homogènes $\neq 0$ est $\neq 0$, l’anneau $A$ n’a pas de diviseur de 0.*

Munissons $\Delta$ d’une structure d’ordre total compatible avec sa structure de groupe (lemme 1) et soient $x = \sum_{\lambda \in \Delta} x_\lambda, y = \sum_{\lambda \in \Delta} y_\lambda$ deux éléments non nuls de $A$ ($x_\lambda$ et $y_\lambda$ étant homogènes de degré $\lambda$ pour tout $\lambda \in \Delta$); soit $\alpha$ (resp. $\beta$) le plus grand des éléments $\lambda \in \Delta$ tels que $x_\lambda \neq 0$ (resp. $y_\lambda \neq 0$); il est immédiat que si $\lambda \neq \alpha$ ou $\mu \neq \beta$, ou bien $x_\lambda y_\mu = 0$ ou bien $\deg(x_\lambda y_\mu) < \alpha + \beta$; la composante homogène de degré $\alpha + \beta$ de $xy$ est donc $x_\alpha y_\beta$, qui n’est pas nul par hypothèse; d’où $xy \neq 0$.

### 5. Produit tensoriel gradué de modules gradués

Soient $\Delta$ un monoïde commutatif dont l’élément neutre est noté 0, $A$ un anneau gradué de type $\Delta$, $M$ (resp. $N$) un $A$-module à droite (resp. à gauche) gradué de type $\Delta$. Soit $(A_\lambda)$ (resp. $(M_\lambda), (N_\lambda)$) la graduation de $A$ (resp. $M, N$); le produit tensoriel $M \otimes_Z N$ des $\mathbf{Z}\text{-modules}$ $M$ et $N$ est somme directe des $M_\lambda \otimes_Z N_\mu$ (II, p. 61, prop. 7), donc ces derniers forment une *bigraduation* de types $\Delta, \Delta$ sur ce $\mathbf{Z}\text{-module}$. Considérons sur $M \otimes_Z N$ la *graduation totale* de type $\Delta$ associée à cette bigraduation (II, p. 164, *Exemple 4*); elle est formée des sous-$\mathbf{Z}$-modules $P_\lambda = \sum_{\mu + \nu = \lambda} (M_\mu \otimes_Z N_\nu)$. On sait que le $\mathbf{Z}\text{-module}$ $M \otimes_A N$ est quotient de $M \otimes_Z N$ par le sous-$\mathbf{Z}$-module $Q$ engendré par les éléments $(xa) \otimes y - x \otimes (ay)$, où $x \in M, y \in N$ et $a \in A$ (II, p. 51); si pour tout $\lambda \in \Delta$, $x_\lambda, y_\lambda, a_\lambda$ sont les composantes homogènes de degré $\lambda$ de $x, y, a$ respectivement, il est clair que $(xa) \otimes y - x \otimes (ay)$ est somme des éléments homogènes $(x_\lambda a_\nu) \otimes y_\mu - x_\lambda \otimes (a_\nu y_\mu)$, autrement dit $Q$ est un sous-$\mathbf{Z}$-module *gradué* de $M \otimes_Z N$ (II, p. 167, prop. 2), et le quotient $M \otimes_A N = (M \otimes_Z N)/Q$ est donc canoniquement muni d’une structure de $\mathbf{Z}\text{-module}$ gradué de type $\Delta$ (II, p. 168). En outre (II, p. 170, prop. 5), le *centre* $C$ de $A$ est un sous-anneau gradué de $A$; la graduation que nous venons de définir sur $M \otimes_A N$ est *compatible avec sa structure de module sur l’anneau gradué* $C$. En effet, $M \otimes_Z N$ est canoniquement muni de *deux* structures de $C$-module, pour lesquelles on a respectivement $c(x \otimes y) = (xc) \otimes y$ et $(x \otimes y)c = x \otimes (cy)$ pour $x \in M, y \in N, c \in C$ (II, p. 53); si $x \in M_\lambda, y \in N_\mu, c \in C \cap A_v$, les deux éléments $c(x \otimes y)$ et $(x \otimes y)c$ appartiennent à $(M \otimes_Z N)_{\lambda + \mu + v}$ et leur différence appartient à $Q$, donc leur image commune dans $M \otimes_A N$ appartient à $(M \otimes_A N)_{\lambda + \mu + v}$, ce qui établit notre assertion. Quand nous parlerons de $M \otimes_A N$ comme d’un C-module gradué, il s’agira toujours de la structure ainsi définie, sauf mention expresse du contraire. On notera que $(M \otimes_A N)_\lambda$ peut se définir comme le sous-groupe additif de $M \otimes_A N$ engendré par les $x_\mu \otimes y_\nu$, où $x_\mu \in M_\mu, y_\nu \in N_\nu$ et $\mu + \nu = \lambda$.

Soient $M'$ (resp. $N'$) un second A-module à droite (resp. à gauche) gradué, $u : M \to M', v : N \to N'$ des homomorphismes gradués de degrés respectifs $\alpha$ et $\beta$. Alors il résulte aussitôt de la remarque précédente que $u \otimes v$ est un homomorphisme (de C-modules) gradué de degré $\alpha + \beta$.

Lorsque A est commutatif, on définit de même une graduation (compatible avec la structure de A-module) sur le produit tensoriel d’un nombre fini quelconque de A-modules gradués; il est immédiat en outre que les isomorphismes d’associativité tels que $(M \otimes N) \otimes P \to M \otimes (N \otimes P)$ (II, p. 64, prop. 8) sont des isomorphismes de modules gradués.

#### Remarque {#alg-ii-s11-n5-rem-1 .statement}

Lorsque A est muni de la graduation triviale (II, p. 163, Exemple 1), $(M \otimes_A N)_\lambda$ est alors simplement la somme directe des sous-C-modules $M_\mu \otimes_A N_\nu$ de $M \otimes_A N$ tels que $\mu + \nu = \lambda$.

Soient $M$ (resp. $N$) un A-module à droite (resp. à gauche) gradué de type $\Delta$, P un $\mathbf{Z}$-module gradué de type $\Delta$, et soit $f$ une application $\mathbf{Z}$-bilinéaire de $M \times N$ dans P, vérifiant la condition (1) de II, p. 50, et telle en outre que l’on ait

$$
f(x_\lambda, y_\mu) \in P_{\lambda+\mu} \quad \text{pour } x \in M_\lambda, y \in N_\mu, \lambda, \mu \text{ dans } \Delta.
$$

On a alors $f(x, y) = g(x \otimes y)$ où $g : M \otimes_A N \to P$ est une application $\mathbf{Z}$-linéaire (II, p. 51, prop. 1), et il résulte de la condition précédente que $g$ est un homomorphisme gradué de degré 0 de $\mathbf{Z}$-modules.

Soit B un second anneau gradué de type $\Delta$, $\rho : A \to B$ un homomorphisme d’anneaux gradués (II, p. 166); alors $\rho_*(B_d)$ est un A-module à droite gradué de type $\Delta$. Si E est un A-module à gauche gradué de type $\Delta$, et si l’on munit $\rho_*(B_d) \otimes_A E$ de la structure de $\mathbf{Z}$-module gradué de type $\Delta$ définie ci-dessus, la structure canonique de B-module à gauche (II, p. 81) est compatible avec la graduation de $E_{(B)} = \rho^*(E) = \rho_*(B_d) \otimes_A E$. On dit que le B-module gradué ainsi obtenu est obtenu par extension à B de l’anneau des scalaires au moyen de $\rho$, et lorsqu’on parle de $E_{(B)}$ ou de $\rho^*(E)$ comme d’un B-module gradué, c’est toujours de cette structure qu’il s’agit sauf mention expresse du contraire.

### 6. Modules gradués d’homomorphismes gradués

Supposons dans ce numéro que le monoïde $\Delta$ soit un groupe. Soient A un anneau gradué de type $\Delta$, et M, N deux A-modules à gauche (par exemple) gradués de type $\Delta$. Désignons par $H_\lambda$ le groupe additif des homomorphismes gradués de degré $\lambda$ de M dans N (II, p. 166); dans le groupe additif $\mathrm{Hom}_A(M, N)$ de tous les homomorphismes de M dans N (pour les structures de A-module non gradué) la somme (pour $\lambda \in \Delta$) des $H_\lambda$ est directe. En effet, si on a une relation $\sum_{\lambda} u_{\lambda} = 0$ avec $u_{\lambda} \in H_{\lambda}$ pour tout $\lambda$, on en tire $\sum_{\lambda} u_{\lambda}(x_{\mu}) = 0$ pour tout $\mu$ et tout $x_{\mu} \in M_{\mu}$. Comme les éléments de $\Delta$ sont simplifiables, $u_{\lambda}(x_{\mu})$ est la composante homogène de degré $\lambda + \mu$ de $\sum_{\lambda} u_{\lambda}(x_{\mu})$; on a donc $u_{\lambda}(x_{\mu}) = 0$ pour tout couple $(\lambda, \mu)$ et tout $x_{\mu} \in M_{\mu}$, ce qui entraîne $u_{\lambda} = 0$ pour tout $\lambda \in \Delta$. Nous désignerons (dans ce paragraphe) par $\mathrm{Homgr}_{A}(M, N)$ le sous-groupe additif de $\mathrm{Hom}_{A}(M, N)$ somme des $H_{\lambda}$ et nous dirons que c’est le groupe additif des *homomorphismes de A-modules gradués* de $M$ dans $N$. Soit $C$ le centre de $A$, qui est un sous-anneau gradué (II, p. 170, corollaire); pour la structure canonique de $C$-module sur $\mathrm{Hom}_{A}(M, N)$ (II, p. 35, *Remarque 1*), $\mathrm{Homgr}_{A}(M, N)$ est un *sous-module* et la graduation $(H_{\lambda})$ est *compatible* avec la structure de $C$-module: en effet, si $c_{v} \in C \cap A_{v}$, $x_{\mu} \in M_{\mu}$ et $u_{\lambda} \in H_{\lambda}$, on a, par définition
$$
(c_{v}u_{\lambda})(x_{\mu}) = c_{v}.u_{\lambda}(x_{\mu}) \subset N_{\lambda+\mu+v},
$$
donc $c_{v}u_{\lambda} \in H_{\lambda+v}$.

Soient $M'$ et $N'$ deux $A$-modules à gauche gradués de type $\Delta$, $u': M' \to M$, $v': N \to N'$ des homomorphismes gradués de degrés respectifs $\alpha$ et $\beta$. Alors il est immédiat que $\mathrm{Hom}(u', v'): w \mapsto v' \circ w \circ u'$ applique $\mathrm{Homgr}_{A}(M, N)$ dans $\mathrm{Homgr}_{A}(M', N')$ et que sa restriction à $\mathrm{Homgr}_{A}(M, N)$ est un homomorphisme *gradué* dans $\mathrm{Homgr}_{A}(M', N')$, *de degré* $\alpha + \beta$.

En particulier $\mathrm{Homgr}_{A}(M, M)$ est un *sous-anneau gradué* de $\mathrm{End}_{A}(M)$, que l’on note $\mathrm{Endgr}_{A}(M)$.

#### Remarque {#alg-ii-s11-n6-rem-1 .statement}

Si $M$ et $N$ sont des $A$-modules à gauche gradués, $\mathrm{Homgr}_{A}(M, N)$ est en général distinct de $\mathrm{Hom}_{A}(M, N)$. Toutefois ces deux ensembles sont égaux lorsque $M$ est un $A$-module *de type fini*. En effet, $M$ est alors engendré par un nombre fini d’éléments homogènes $x_{i}$ ($1 \leq i \leq n$); soit $d(i)$ le degré de $x_{i}$; soit $u \in \mathrm{Hom}_{A}(M, N)$ et pour tout $\lambda \in \Delta$, désignons par $z_{i, \lambda}$ la composante homogène de degré $\lambda + d(i)$ de $u(x_{i})$. Montrons qu’il existe un homomorphisme $u_{\lambda}: M \to N$, tel que $u_{\lambda}(x_{i}) = z_{i, \lambda}$ pour tout $i$. Il suffit de prouver que si l’on a $\sum_{i} a_{i}x_{i} = 0$ avec $a_{i} \in A$ pour $1 \leq i \leq n$, il en résulte que $\sum_{i} a_{i}z_{i, \lambda} = 0$ pour tout $\lambda \in \Delta$ (II, p. 16, *Remarque*). On peut supposer que chaque $a_{i}$ est homogène de degré $d'(i)$ tel que $d(i) + d'(i) = \mu$ pour tout $i$ (II, p. 167, *Remarque 1*); on a alors $\sum_{i} a_{i}u(x_{i}) = 0$; prenant la composante homogène de degré $\lambda + \mu$ du premier membre, il vient $\sum_{i} a_{i}z_{i, \lambda} = 0$, d’où l’existence de l’homomorphisme $u_{\lambda}$; il est clair en outre que $u_{\lambda}$ est *gradué* de degré $\lambda$. Enfin, on a $u_{\lambda} = 0$ sauf pour un nombre fini de valeurs de $\lambda$, et $u = \sum_{\lambda} u_{\lambda}$ par définition, ce qui achève de prouver notre assertion.

En particulier, on a $\mathrm{Homgr}_{A}(A_{s}, M) = \mathrm{Hom}_{A}(A_{s}, M)$ pour tout $A$-module à gauche gradué $M$; en outre $\mathrm{Hom}_{A}(A_{s}, M)$ est muni d’une structure de *A-module à gauche gradué* (et non seulement de $C$-module gradué) et il est immédiat que pour cette structure, l’application canonique de M dans Hom_A(A_s, M) (II, p. 35, Remarque 2) est un isomorphisme de A-modules gradués.

De même, Homgr_A(M, A_s) est muni d’une structure de A-module à droite gradué (et non seulement de C-module gradué); on dit que c’est le dual gradué du A-module gradué M, et on le note M^{*gr}, ou simplement M* quand aucune confusion n’en résulte. Si u : M → N est un homomorphisme gradué de degré δ, il résulte de ce qui précède que la restriction à N^{*gr} de ^t u = Hom(u, 1_{A_s}) est un homomorphisme gradué u’ du dual gradué N^{*gr} dans le dual gradué M^{*gr}, de degré δ, dit transposé gradué de u.

On considère parfois sur le dual gradué M^{*gr} la graduation déduite de la précédente à l’aide de l’isomorphisme λ ↦ −λ de Δ (II, p. 163, Exemple 2) de sorte que l’on prend pour éléments homogènes de degré λ de M^{*gr} les formes linéaires graduées de degré −λ sur M (lorsque A est muni de la graduation triviale, ce seront les formes linéaires nulles dans les M_μ d’indice μ ≠ λ). Alors, si u : M → N est un homomorphisme gradué de degré δ, u’ devient un homomorphisme gradué de degré −δ.

Supposons A commutatif et gradué de type Δ, et soient M, N, P, Q quatre A-modules gradués de type Δ. On a alors des homomorphismes canoniques gradués de degré 0
(3) Homgr_A(M, Homgr_A(N, P)) → Homgr_A(M ⊗_A N, P)
(4) Homgr_A(M, N) ⊗_A P → Homgr_A(M, N ⊗_A P)
(5) Homgr_A(M, P) ⊗_A Homgr_A(N, Q) → Homgr_A(M ⊗_A N, P ⊗_A Q)
(les produits tensoriels étant munis des graduations définies dans II, p. 173) que l’on obtient par restriction des homomorphismes canoniques définis au § 4 (II, p. 74, 75 et 79); en effet, si u : M → Homgr_A(N, P) est gradué de degré δ, alors, pour tout x ∈ M_λ, u(x) est un homomorphisme gradué N → P de degré δ + λ, donc, pour y ∈ N_μ, on a u(x)(y) ∈ P_{δ+λ+μ}; si v : M ⊗_A N → P correspond canoniquement à u, on voit donc que v est un homomorphisme gradué de degré δ, d’où notre assertion concernant (3); on voit en outre que cet homomorphisme est bijectif. On raisonne de même pour (4) et (5).

Si on prend en particulier P = Q = A dans (5), on obtient un homomorphisme canonique gradué de degré 0
(6) M^{*gr} ⊗_A N^{*gr} → (M ⊗_A N)^{*gr}.

## EXERCICES {#alg-ii-s11-exercises}

See the [exercises for § 11](exercises/s11/).
