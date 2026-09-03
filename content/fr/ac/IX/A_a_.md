---
book: ac
book_title: Commutative Algebra
chapter: IX
chapter_title: ANNEAUX LOCAUX NOETHÉRIENS COMPLETS
section: 0
section_title: ""
appendix: true
lang: fr
source: ac-viii-ix-fr
book_pages: AC IX.37-AC IX.42
pdf_pages: 0149-0154, 0196-0204
extraction: ocr
subsections:
    - "no": 1
      title: Limite inductive d’anneaux locaux
      page: 37
      pdf_page: 149
    - "no": 2
      title: Gonflement d’un anneau local
      page: 37
      pdf_page: 149
    - "no": 3
      title: Existence des $p$-anneaux
      page: 41
      pdf_page: 153
statements: 13
exercises: 7
content_sha256: 98bbdb09a04c6ecf122abe20e179ba71aba6d2aa037d166e2a4c159f9f8f8b67
---

### APPENDICE

### 1. Limite inductive d’anneaux locaux

Soit I un ensemble préordonné non vide filtrant à droite et soit $(A_\alpha, \varphi_{\beta\alpha})$ un système inductif d’anneaux relatif à I. On suppose que, pour tout $\alpha \in I$, l’anneau $A_\alpha$ est local, d’idéal maximal $m_\alpha$, que les homomorphismes $\varphi_{\beta\alpha}$ sont locaux et plats, et qu’on a $\varphi_{\beta\alpha}(m_\alpha)$ $A_\beta = m_\beta$ pour $\beta \geq \alpha$. Notons A la limite inductive des $A_\alpha$, et pour tout $\alpha \in I$, soit $\varphi_\alpha : A_\alpha \to A$ l’homomorphisme canonique.

#### Proposition 1 {#ac-ix-a0-prop-1 .statement}

a) L’anneau A est local, d’idéal maximal $m = \lim \overrightarrow{m_\alpha}$. Pour tout $\alpha \in I$, l’homomorphisme $\varphi_\alpha$ est local et plat, et on a $\varphi_\alpha(m_\alpha)$ $A = m$.

b) Si $A_\alpha$ est noethérien pour tout $\alpha \in A$, alors A est noethérien.

a) Posons $m = \lim \overrightarrow{m_\alpha}$; c’est un idéal de A. L’anneau quotient $A/m$ est limite inductive des corps $A_\alpha/m_\alpha$, donc est un corps (A, I, p. 116, prop. 3). Par ailleurs, tout élément de $A - m$ est inversible dans A : en effet, soit $x \in A - m$; il existe $\alpha \in I$ et $\xi \in A_\alpha$ tels que $x = \varphi_\alpha(\xi)$; on a $\xi \notin m_\alpha$, donc $\xi$ est inversible dans $A_\alpha$ et x est inversible dans A. Par conséquent, A est un anneau local, d’idéal maximal m. Soit $\alpha \in I$. Des relations $\varphi_{\beta\alpha}(m_\alpha)$ $A_\beta = m_\beta$ pour $\beta \geq \alpha$, on déduit, par passage à la limite inductive, $\varphi_\alpha(m_\alpha)$ $A = m$; enfin, l’homomorphisme $\varphi_\alpha$ est plat d’après I, § 2, no 7, prop. 9.

b) Soient $\hat{A}$ l’anneau séparé complété de A pour la topologie $m$-adique et $\pi$ l’application canonique de A dans $\hat{A}$. Supposons les anneaux $A_\alpha$ noethériens. Fixons $\alpha \in I$ et prouvons que l’anneau $\hat{A}$ est noethérien et plat sur $A_\alpha$. Par hypothèse, $m_\alpha$ est un idéal de type fini de $A_\alpha$, donc $m = \varphi_\alpha(m_\alpha)$. A est un idéal de type fini de A. Il s’ensuit que l’idéal maximal $\hat{m}$ de $\hat{A}$ est égal à $mA$ (III, § 2, no 12, cor. 2 à la prop. 16 et no 13, prop. 19), donc est de type fini. Par conséquent, l’anneau $\hat{A}$ est noethérien (loc. cit., no 10, cor. 5 au th. 2). D’autre part, pour tout $n \in \mathbf{N}$, le quotient $\hat{A}/\hat{m}^n$ est isomorphe à $A/m^n$ (loc. cit., n° 12, cor. 2 à la prop. 16 et formule (21)), ce qui signifie que $\hat{A}/\pi \circ \varphi_\alpha(m_\alpha^n)$ $\hat{A}$ est isomorphe à $A \otimes_A (A_\alpha/m_\alpha^n)$; puisque A est un $A_\alpha$-module plat, le $(A_\alpha/m_\alpha^n)$-module $\hat{A}/\pi \circ \varphi_\alpha(m_\alpha^n)$ $\hat{A}$ est plat pour tout $n \in \mathbf{N}$. D’après III, § 5, no 4, prop. 2, le $A_\alpha$-module $\hat{A}$ est idéalement séparé pour $m_\alpha$; d’après loc. cit., no 2, th. 1, le $A_\alpha$-module $\hat{A}$ est donc plat. Il en résulte par passage à la limite inductive que $\hat{A}$ est (fidèlement) plat sur A (I, § 2, no 7, prop. 9), donc que A est noethérien (I, § 3, no 5, corollaire à la prop. 8).

### 2. Gonflement d’un anneau local

Soit A un anneau local.

On note A]X[ l’anneau local de l’anneau de polynômes A[X] en l’idéal premier $m_A A[X]$. C’est un anneau local d’idéal maximal $m_A A[X]$, l’homomorphisme canonique $A \to A[X]$ est local et plat, et le corps résiduel de $A[X]$ est l’extension pure de $\kappa_A$ engendrée par la classe de $X$.

#### Lemme 1 {#ac-ix-a0-lem-1 .statement}

Soit $P \in A[X]$ un polynôme unitaire dont l’image $\overline{P}$ dans $\kappa_A[X]$ est irréductible. Alors la $A$-algèbre $B = A[X]/(P)$ est locale et finie sur $A$, d’idéal maximal $m_A B$, l’homomorphisme canonique $\rho : A \to B$ est local et plat, l’extension résiduelle $\kappa_A \to \kappa_B$ est algébrique et engendrée par la classe $x$ de $X$, et le polynôme minimal de $x$ sur $\kappa_A$ est $\overline{P}$.

Comme le polynôme $P$ est unitaire, le $A$-module $B$ est libre de type fini (A, IV, p. 10). L’anneau $B/m_A B$ s’identifie à $\kappa_A[X]/(\overline{P})$, donc est un corps ; l’idéal $m_A B$ est donc maximal. Soit $q$ un idéal maximal de $B$ ; alors l’idéal $\rho^{-1}(q)$ est maximal (V, § 2, no 1, prop. 1) ; on a donc $\rho^{-1}(q) = m_A$, d’où $q \supset m_A B$ et enfin $q = m_A B$. Ainsi l’anneau $B$ est local. Le lemme 1 en résulte aussitôt.

#### Définition 1 {#ac-ix-a0-def-1 .statement}

Soit $A$ un anneau local. On dit qu’une $A$-algèbre $B$ est un gonflement élémentaire de $A$ si $B$ est isomorphe à la $A$-algèbre $A[X]$, ou bien s’il existe un polynôme unitaire $P$ de $A[X]$, d’image irréductible dans $\kappa_A[X]$, tel que $B$ soit isomorphe à la $A$-algèbre $A[X]/(P)$.

Soit $B$ un gonflement élémentaire de $A$. De ce qui précède résultent les propriétés suivantes :

a) L’anneau $B$ est local et l’homomorphisme canonique de $A$ dans $B$ est local et plat, et en particulier injectif (I, § 3, no 5, prop. 8).

b) Le corps résiduel $\kappa_B$ de $B$ est une extension monogène du corps résiduel $\kappa_A$ de $A$. Si $\kappa_A$ est de degré fini $d$ sur $\kappa_A$, alors $B$ est un $A$-module libre de rang $d$.

c) On a $m_B = m_A B$. En particulier, si $A$ est un corps, il en est de même de $B$. Une extension de corps est un gonflement élémentaire si et seulement si elle est monogène.

d) Si $A$ est noethérien, il en est de même de $B$.

#### Définition 2 {#ac-ix-a0-def-2 .statement}

Soit $A$ un anneau local. On dit qu’une $A$-algèbre $B$ est un gonflement de $A$ s’il existe un ensemble bien ordonné $\Lambda$ ayant un plus grand élément $\omega$, et une famille croissante $(B_\lambda)_{\lambda \in \Lambda}$ de sous-algèbres de $B$ satisfaisant aux conditions suivantes :

a) On a $B_\omega = B$ et l’anneau $B_\lambda$ est local pour tout $\lambda \in \Lambda$.

b) Si $\alpha$ est le plus petit élément de $\Lambda$, la $A$-algèbre $B_\alpha$ est isomorphe à $A$.

c) Soit $\nu \neq \alpha$ dans $\Lambda$ et soit $S_\nu$ l’ensemble des $\lambda \in \Lambda$ tels que $\lambda < \nu$. Si $S_\nu$ n’a pas de plus grand élément, on a $B_\nu = \bigcup_{\lambda \in S_\nu} B_\lambda$; si $S_\nu$ a un plus grand élément $\mu$, alors $B_\nu$ est un gonflement élémentaire de $B_\mu$.

Soient $B$ un anneau et $\rho : A \to B$ un homomorphisme d’anneaux. On dit que $\rho$ est un gonflement (resp. un gonflement élémentaire) si la $A$-algèbre définie par $\rho$ a cette propriété. S’il en est ainsi, $\rho$ est injectif.

#### Exemple 1 {#ac-ix-a0-n2-exa-1 .statement}

Toute extension de corps est un gonflement. Soit en effet K une extension d’un corps k. Munissons K d’un bon ordre pour lequel 0 est le plus grand élément, et pour $\lambda \in K$, soit $K_\lambda$ la sous-$k$-extension de K engendrée par les éléments $\beta$ de K tels que $\beta < \lambda$. La vérification des conditions a), b), c), pour $k, K$ et la famille $(K_\lambda)_{\lambda \in K}$, est immédiate.

#### Exemple 2 {#ac-ix-a0-n2-exa-2 .statement}

Soient A un anneau local, et I un ensemble d’indices. Notons $A[(X_i)_{i \in I}]$ l’anneau local de l’anneau de polynômes $A[(X_i)_{i \in I}]$ en l’idéal premier $m_A A[(X_i)_{i \in I}]$. La A-algèbre $A[(X_i)_{i \in I}]$ est un gonflement de A. En effet, munissons l’ensemble I d’un bon ordre ; soit $\Lambda$ l’ensemble bien ordonné obtenu en adjoignant à I un plus grand élément $\omega$. Pour $i \in I$, identifions $A[(X_j)_{j < i}]$ à une sous-algèbre $B_i$ de $B = A[(X_i)_{i \in I}]$, et posons $B_\omega = B$. La famille $(B_\lambda)_{\lambda \in \Lambda}$ satisfait aux conditions a), b), c).

#### Remarque {#ac-ix-a0-n2-rem-1 .statement}

Avec les notations de la déf. 2, l’anneau $B_\mu$ est un gonflement de $B_\lambda$ lorsque $\lambda \leq \mu$.

#### Proposition 2 {#ac-ix-a0-prop-2 .statement}

Soient A un anneau local et B un gonflement de A.

a) L’anneau B est local et l’on a $m_A B = m_B$.

b) La A-algèbre B est fidèlement plate.

c) L’homomorphisme canonique

$$
\gamma_B : \operatorname{gr}(A) \otimes_{\kappa_A} \kappa_B \to \operatorname{gr}(B)
$$

est bijectif.

d) Si A est noethérien, il en est de même de B et les séries de Hilbert-Samuel (VIII, § 4, no 3) de A et B sont égales.

Soit $(B_\lambda)_{\lambda \in \Lambda}$ une famille de sous-algèbres de B satisfaisant aux conditions a), b) et c) de la déf. 2.

Soit $\Lambda'$ l’ensemble des indices $\lambda \in \Lambda$ tels que, pour tout $\mu \leq \lambda$ dans $\Lambda$, la A-algèbre $B_\mu$ soit locale et fidèlement plate, et qu’on ait $m_{B_\mu} = m_A B_\mu$. Supposons qu’on ait $\Lambda' \neq \Lambda$ et soit $v$ le plus petit élément de $\Lambda - \Lambda'$. On a $\alpha \in \Lambda'$, d’où $v \neq \alpha$. Or $S_v$ est contenu dans $\Lambda'$. Si $S_v$ n’a pas de plus grand élément, on a $B_v = \bigcup_{\lambda \in S_v} B_\lambda$ et $v$ appartient à $\Lambda'$ d’après la prop. 1 du no 1. Si $S_v$ a un plus grand élément $\mu$, on a $\mu \in \Lambda'$ et $B_v$ est un gonflement élémentaire de $B_\mu$ : on a encore $v \in \Lambda'$ d’après les remarques qui suivent la déf. 1, d’où une contradiction.

Lorsque A est noethérien, on prouve de manière analogue que l’ensemble $\Lambda''$ des indices $\lambda \in \Lambda$ tels que l’anneau $B_\lambda$ soit noethérien est égal à $\Lambda$.

On a donc $\omega \in \Lambda'$, d’où les assertions a) et b). Lorsque A est noethérien, on a $\omega \in \Lambda''$, donc $B = B_\omega$ est noethérien.

L’assertion c) résulte de a); b), et du th. 1 de III, § 5, no 2. Supposons A (donc B) noethérien ; comme on a

$$
[m_B^n / m_B^{n+1} : \kappa_B] = [m_A^n / m_A^{n+1} : \kappa_A]
$$

pour tout $n \in \mathbf{N}$, les séries de Hilbert-Samuel de A et B sont égales.

#### Corollaire {#ac-ix-a0-n2-cor-1 .statement}

Supposons A noethérien.
a) On a dim(A) = dim(B).
b) Supposons A régulier, et soit $(x_1, ..., x_n)$ un système de coordonnées de A. Alors B est régulier et la suite $(x_1 1_B, ..., x_n 1_B)$ est un système de coordonnées de B.
Cela résulte de la prop. 1 de VIII, § 5, no 1.

#### Proposition 3 {#ac-ix-a0-prop-3 .statement}

Soient A, B, C trois anneaux locaux et $u : A \to B, v : B \to C$ deux gonflements. Alors $v \circ u$ est un gonflement.
Soient $(B_\lambda)_{\lambda \in \Lambda}$ et $(C_\mu)_{\mu \in M}$ des familles de sous-A-algèbres de B et de sous-B-algèbres de C respectivement, ayant les propriétés a), b), c) de la déf. 2. Sur l’ensemble N somme de $\Lambda$ et M, considérons la relation d’ordre induisant sur $\Lambda$ et M les ordres donnés et telle qu’on ait $\lambda < \mu$ pour $\lambda \in \Lambda, \mu \in M$. C’est une relation de bon ordre. Pour $\lambda \in \Lambda \subset N$, posons $C_\lambda = v(B_\lambda)$. Alors la famille $(C_v)_{v \in N}$ satisfait aux conditions a), b), c) de la déf. 1 relativement à la A-algèbre C.

#### Théorème 1 {#ac-ix-a0-thm-1 .statement}

Soient $f : A \to A'$ un homomorphisme local surjectif d’anneaux locaux et $B'$ un gonflement de $A'$. Il existe un gonflement B de A et un isomorphisme de A-algèbres de $B \otimes_A A'$ sur $B'$.
A) Supposons que $B'$ soit un gonflement élémentaire de $A'$. Distinguons deux cas :
1) Si $B'$ est finie sur $A'$, choisissons un isomorphisme de $A'-algèbres$ $\varphi : A'[X]/(P') \to B'$, où $P' \in A'[X]$ est un polynôme unitaire d’image irréductible dans $\kappa_{A'}[X]$. Choisissons un polynôme unitaire $P \in A[X]$ dont l’image dans $A'[X]$ est $P'$. Il est nécessairement irréductible modulo l’idéal maximal de A. Posons alors $B = A[X]/(P)$. La A-algèbre B est un gonflement élémentaire de A et $\varphi$ induit un isomorphisme de A-algèbres de $B \otimes_A A'$ sur $B'$.
2) Si $B'$ n’est pas finie sur $A'$, choisissons un isomorphisme de $A'-algèbres$ $\psi : A'[X] \to B'$. Posons $B = A[X][$. La A-algèbre B est un gonflement élémentaire de A, et $B \otimes_A A'$ est canoniquement isomorphe à $A'[X][$. Par suite $\psi$ induit un isomorphisme de A-algèbres de $B \otimes_A A'$ sur $B'$.
B) Passons au cas général. Soit $(B'_\lambda)_{\lambda \in \Lambda}$ une famille de sous-A'-algèbres de $B'$ ayant relativement à $A'$ et $B'$ les propriétés a), b), c) de la déf. 2. Nous allons définir par récurrence transfinie un système inductif $(\tilde{B}_\lambda, i_{\mu \lambda})$ relatif à $\Lambda$ d’anneaux locaux et d’homomorphismes locaux injectifs, et des isomorphismes $u_\lambda : \tilde{B}_\lambda \otimes_A A' \to B'_\lambda$ tels que, pour $\lambda \leq \mu$, $u_\mu \circ (i_{\mu \lambda} \otimes \mathrm{Id}_{A'}) \circ u_\lambda^{-1}$ soit l’injection canonique de $B'_\lambda$ dans $B'_{\mu}$.
Si $\alpha$ est le plus petit élément de $\Lambda$, on pose $\tilde{B}_\alpha = A, i_{\alpha \alpha} = \mathrm{Id}_A$ et on prend pour $u_\alpha$ l’isomorphisme canonique $A \otimes_A A' \to A'$.
Soit $\nu \in \Lambda$, et supposons $\tilde{B}_\lambda, u_\lambda$ et $i_{\mu \lambda}$ construits lorsque $\lambda \leq \mu < \nu$. Soit $S_\nu$ l’ensemble des éléments $\varepsilon$ de $\Lambda$ tels que $\varepsilon < \nu$. Si $S_\nu$ n’a pas de plus grand élément, on prend pour $\tilde{B}_\nu$ la limite inductive des $\tilde{B}_\lambda$ pour $\lambda \in S_\nu$, pour $u_\nu$ l’isomorphisme composé $\tilde{B}_\nu \otimes_A A' \to \lim (\tilde{B}_\lambda \otimes_A A') \to \lim B'_\lambda \to B'_\nu$, et pour $i_{\nu \lambda}$, lorsque $\lambda \in S_\nu$, l’application canonique de $\tilde{B}_\lambda$ dans $\tilde{B}_\nu$. Si $S_\nu$ a un plus grand élément $\mu$, alors $B'_\nu$ est un gonflement élémentaire de $B'_{\mu}$. D’après A), il existe un gonflement élémentaire i_{v\mu}: \tilde{B}_{\mu} \to \tilde{B}_{v} et un isomorphisme de $\tilde{B}_{\mu}$-algèbres de $\tilde{B}_{v} \otimes_{\tilde{B}_{\mu}} B'_{\mu}$ sur $B'_{v}$. Prenons pour $u_{v}$ l’isomorphisme de A-algèbres composé
$$
\tilde{B}_{v} \otimes_{A} A' \to \tilde{B}_{v} \otimes_{\tilde{B}_{\mu}} (\tilde{B}_{\mu} \otimes_{A} A') \to \tilde{B}_{v} \otimes_{\tilde{B}_{\mu}} B'_{\mu} \to B'_{v}
$$
et pour $i_{v\lambda}$, lorsque $\lambda \in S_{v}$, l’homomorphisme $i_{v\mu} \circ i_{\mu\lambda}$.

Posons alors $B = \tilde{B}_{\omega}$ et, pour tout $\lambda \in \Lambda$, notons $B_{\lambda}$ l’image de $\tilde{B}_{\lambda}$ par l’injection canonique $\tilde{B}_{\lambda} \to B$. La famille $(B_{\lambda})_{\lambda \in \Lambda}$ satisfait aux conditions a), b), c) de la déf. 2, et B est un gonflement de A. D’autre part, l’homomorphisme $u_{\omega}$ est un A’-isomorphisme de $B \otimes_{A} A'$ dans $B'$.

#### Corollaire {#ac-ix-a0-n2-cor-2 .statement}

Soient A un anneau local et K une extension de son corps résiduel $\kappa_{A}$. Il existe un anneau local B et un gonflement $A \to B$ tels que la $\kappa_{A}$-algèbre $\kappa_{B}$ soit isomorphe à K.

En effet, l’homomorphisme $\kappa_{A} \to K$ est un gonflement (exemple 1). Appliquant le th. 1 avec $A' = \kappa_{A}$ et $B' = K$, on obtient l’existence d’un gonflement B de A et d’un A-isomorphisme de $B/m_{A}B$ sur K, d’où le corollaire.

### 3. Existence des $p$-anneaux

#### Proposition 4 {#ac-ix-a0-prop-4 .statement}

Soient p un nombre premier, k un corps de caractéristique p, et soit n un entier $\geq 1$, ou $+ \infty$. Il existe un $p$-anneau ($\S$ 2, no 1, déf. 1) de longueur n dont le corps résiduel est isomorphe à k.

On peut considérer k comme une extension du corps résiduel $\mathbf{Z}/p\mathbf{Z}$ de l’anneau local $\mathbf{Z}_{(p)}$. D’après le corollaire du th. 1, il existe un anneau local B, gonflement de $\mathbf{Z}_{(p)}$, tel que $\kappa_{B}$ soit isomorphe à k. L’anneau local $\mathbf{Z}_{(p)}$ est régulier et $\{ p \}$ est un système de coordonnées de $\mathbf{Z}_{(p)}$. D’après le corollaire de la prop. 2 du no 2, l’anneau B est régulier et $\{ pl_{B} \}$ est un système de coordonnées de B. Autrement dit, B est un anneau de valuation discrète, d’idéal maximal $pB$. Le complété C de B est alors un $p$-anneau de longueur infinie et le corps résiduel $\kappa_{C}$ est isomorphe à $\kappa_{B}$, donc à k. De plus, pour tout entier $n \geq 1$, $C/p^{n}C$ est un $p$-anneau de longueur n, de corps résiduel isomorphe à $\kappa_{C}$, donc à k.

Exercises

## EXERCICES {#ac-ix-a0-exercises}

See the [exercises for Appendix 0](exercises/a0/).
