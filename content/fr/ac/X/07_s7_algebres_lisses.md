---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 7
section_title: Algèbres lisses
lang: fr
source: ac-x-fr
book_pages: AC X.170-AC X.173
pdf_pages: 0082-0103, 0169-0172
extraction: ocr
subsections:
    - "no": 1
      title: Dérivations et relèvements d’homomorphismes
      page: 0
      pdf_page: 82
    - "no": 2
      title: Algèbres formellement lisses
      page: 84
      pdf_page: 83
    - "no": 3
      title: Exemples d’algèbres formellement lisses
      page: 87
      pdf_page: 86
    - "no": 4
      title: Relèvements d’homomorphismes dans les algèbres filtrées complètes
      page: 89
      pdf_page: 88
    - "no": 5
      title: Quotients formellement lisses d’algèbres
      page: 90
      pdf_page: 89
    - "no": 6
      title: Extension du corps de base dans les algèbres régulières (caractéristique non nulle)
      page: 0
      pdf_page: 91
    - "no": 7
      title: Un critère pour les algèbres locales formellement lisses
      page: 95
      pdf_page: 94
    - "no": 8
      title: Existence de rétractions pour les applications linéaires
      page: 0
      pdf_page: 96
    - "no": 9
      title: Le critère jacobien
      page: 98
      pdf_page: 97
    - "no": 10
      title: Algèbres lisses
      page: 102
      pdf_page: 101
statements: 39
exercises: 15
content_sha256: d68b9c7325c87d31bf9721e3dce35c4be0ff95e79d61fe0491564111f5babb1e
---

## § 7. ALGÈBRES LISSES

### 1. Dérivations et relèvements d’homomorphismes

Soient $k$ un anneau, $C$ une $k$-algèbre et $N$ un idéal de $C$ de carré nul. Notons $\pi : C \to C/N$ l’homomorphisme canonique ; puisque $N^2 = \{0\}$, la structure de $C$-module de $N$ provient d’une structure de $C/N$-module.

Soient $A$ une $k$-algèbre et $\varphi : A \to C/N$ un homomorphisme de $k$-algèbres. Munissons $N$ de la structure de $A$-module déduite de $\varphi$. On appelle *relèvement de $\varphi$* (à $C$) tout homomorphisme de $k$-algèbres $\tilde{\varphi} : A \to C$ tel que $\pi \circ \tilde{\varphi} = \varphi$. Soient $\tilde{\varphi}$ un tel relèvement, et $\delta$ une application de $A$ dans $N$ ; notons $\delta + \tilde{\varphi}$ l’application $x \mapsto \delta(x) + \tilde{\varphi}(x)$ de $A$ dans $C$.

#### Proposition 1 {#ac-x-s7-prop-1 .statement}

*Si $\varphi$ admet un relèvement, l’application $(\delta, \tilde{\varphi}) \mapsto \delta + \tilde{\varphi}$ définit une opération simplement transitive du groupe des $k$-dérivations de $A$ dans $N$ sur l’ensemble des relèvements de $\varphi$.*

Soit $\tilde{\varphi}_0 : A \to C$ un relèvement de $\varphi$. L’application $\delta \mapsto \delta + \tilde{\varphi}_0$ induit une bijection de l’ensemble des applications de $A$ dans $N$ sur l’ensemble des applications $\tilde{\varphi} : A \to C$ telles que $\pi \circ \tilde{\varphi} = \varphi$. Fixons $\delta$, et posons $\tilde{\varphi} = \delta + \tilde{\varphi}_0$. Pour que $\tilde{\varphi}$ soit un homomorphisme de $k$-algèbres, il faut et il suffit que $\delta$ soit une $k$-dérivation de $A$ dans $N$ : en effet, pour $x, y$ dans $A$ et $\lambda$ dans $k$, on a les relations

$$
\begin{align*}
\tilde{\varphi}(x + y) - \tilde{\varphi}(x) - \tilde{\varphi}(y) &= \delta(x + y) - \delta(x) - \delta(y) \\
\tilde{\varphi}(\lambda x) - \lambda \tilde{\varphi}(x) &= \delta(\lambda x) - \lambda \delta(x) \\
\tilde{\varphi}(xy) - \tilde{\varphi}(x)\tilde{\varphi}(y) &= \delta(xy) - \delta(x)\delta(y) - \delta(x)\tilde{\varphi}_0(y) - \tilde{\varphi}_0(x)\delta(y) \\
&= \delta(xy) - \varphi(x)\delta(y) - \varphi(y)\delta(x),
\end{align*}
$$

la dernière égalité résultant du fait que $N$ est de carré nul. La proposition en résulte.

#### Exemple {#ac-x-s7-n1-exa-1 .statement}

Soient $B$ une $k$-algèbre, $N$ un $B$-module. Munissons le $k$-module $B \oplus N$ de la structure de $k$-algèbre définie par $(b, x)(b', x') = (bb', bx' + b'x)$ (*cf.* A, III, p. 127), de sorte que $N$ est un idéal de carré nul de $B \oplus N$. Soit $\varphi : A \to B$ un homomorphisme de $k$-algèbres. Alors les relèvements de $\varphi$ à $B \oplus N$ sont les applications $x \mapsto (\varphi(x), \delta(x))$, où $\delta$ parcourt l’ensemble des $k$-dérivations de $A$ dans $N$ (*cf. loc. cit.*, prop. 12).

Soit $\Omega_k(A)$ le module des $k$-différentielles de l’anneau $A$, et soit $d : A \longrightarrow \Omega_k(A)$ la $k$-dérivation universelle (A, III, p. 133 et 134) ; rappelons (*loc. cit.*) que pour tout $A$-module $M$, l’application $v \mapsto v \circ d$ est un isomorphisme $A$-linéaire de $\mathrm{Hom}_A(\Omega_k(A), M)$ sur le $A$-module des $k$-dérivations de $A$ dans $M$.

Soit J un idéal de A. D’après A, III, p. 137, on a une suite exacte d’applications A/J-linéaires

$$
J/J^2 \xrightarrow{\bar{d}} (\Lambda/J) \otimes_A \Omega_k(\Lambda) \longrightarrow \Omega_k(A/J) \to 0,
$$

où $\bar{d}$ est l’homomorphisme déduit par passage aux quotients de la restriction de $d$ à J.

Notons $\rho : A \to A/J^2$ et $\pi : A/J^2 \to A/J$ les surjections canoniques. Soit $v : (A/J) \otimes_A \Omega_k(A) \longrightarrow J/J^2$ une application $k$-linéaire ; on lui associe une application $k$-linéaire $H_v : A \to A/J^2$ en posant $H_v(x) = \rho(x) - v(1 \otimes dx)$. Si $v$ est une rétraction de $\bar{d}$, $H_v$ s’annule sur J, donc induit par passage au quotient une application $k$-linéaire $h_v : A/J \to A/J^2$. D’autre part, étant donnée une application $k$-linéaire $h : A/J \to A/J^2$, notons $\psi_h : A/J \oplus J/J^2 \longrightarrow A/J^2$ l’application $(x, y) \mapsto h(x) + y$.

#### Proposition 2 {#ac-x-s7-prop-2 .statement}

Munissons le $k$-module $\Lambda/J \oplus J/J^2$ de la structure de $k$-algèbre définie dans l’exemple ci-dessus. Les applications $v \mapsto h_v$ et $h \mapsto \psi_h$ induisent des bijections entre les ensembles suivants :

(i) l’ensemble des rétractions $A/J$-linéaires $v$ de $\bar{d}$ ;
(ii) l’ensemble des homomorphismes de $k$-algèbres $h : A/J \to A/J^2$ tels que $\pi \circ h = \mathrm{Id}_{A/J}$ ;
(iii) l’ensemble des isomorphismes de $k$-algèbres $\psi : A/J \oplus J/J^2 \longrightarrow A/J^2$ tels que $\pi \circ \psi = \mathrm{pr}_1$ et $\psi(0, z) = z$ pour $z \in J/J^2$.

Appliquons la prop. 1 avec $C = A/J^2$ et $N = J/J^2$. Soit $\varphi : A \to A/J$ la surjection canonique ; l’homomorphisme $\rho$ est un relèvement de $\varphi$ à $A/J^2$. Le A-module $\mathrm{Hom}_{A/J}((A/J) \otimes_A \Omega_k(A), J/J^2)$ s’identifie à $\mathrm{Hom}_A(\Omega_k(A), J/J^2)$ ; d’après la prop. 1, l’application $v \mapsto H_v$ est une bijection de cet ensemble sur l’ensemble des relèvements de $\varphi$ à $A/J^2$. Pour $x \in J$, on a $1 \otimes dx = \bar{d}(\rho(x))$ ; pour que $H_v$ s’annule sur J, il faut et il suffit que $v \circ \bar{d}$ soit l’application identique de $J/J^2$. Cela prouve que l’application $v \mapsto h_v$ induit une bijection entre les deux premiers ensembles décrits dans l’énoncé.

L’application $h \mapsto \psi_h$ est une bijection de l’ensemble des homomorphismes $k$-linéaires de $A/J$ dans $A/J^2$ sur l’ensemble des homomorphismes $k$-linéaires $\psi : A/J \oplus J/J^2 \longrightarrow A/J^2$ tels que $\psi(0, z) = z$ pour $z \in J/J^2$ ; de plus pour qu’on ait $\pi \circ \psi_h = \mathrm{pr}_1$ il faut et il suffit qu’on ait $\pi \circ h = \mathrm{Id}_{A/J}$, c’est-à-dire $z \equiv h(\pi(z)) \pmod{J/J^2}$ pour tout $z \in A/J^2$. Supposons ces conditions vérifiées. Pour que $h$ soit un homomorphisme d’anneaux, il faut et il suffit qu’il en soit ainsi de $\psi_h$ ; de plus, l’homomorphisme $\psi_h$ est bijectif : l’application réciproque associe à un élément $z$ de $A/J^2$ le couple $(\pi(z), z - h(\pi(z)))$. Cela prouve que l’application $h \mapsto \psi_h$ induit une bijection entre les deux derniers ensembles décrits dans l’énoncé.

### 2. Algèbres formellement lisses

Soient $k$ un anneau et $A$ une $k$-algèbre linéairement topologisée (III, § 4, n° 2, déf. 1).

#### Définition 1 {#ac-x-s7-def-1 .statement}

On dit que $A$ est formellement lisse sur $k$, ou est une $k$-algèbre formellement lisse, si elle satisfait à la condition suivante : quels que soient la $k$-algèbre $C$ et l’idéal de carré nul $N$ de $C$, tout homomorphisme continu de $A$ dans la $k$-algèbre $C/N$, munie de la topologie discrète, se relève en un homomorphisme continu de $A$ dans la $k$-algèbre $C$, munie de la topologie discrète.

Rappelons qu’un homomorphisme de $A$ dans une $k$-algèbre munie de la topologie discrète est continu si et seulement si son noyau est ouvert.

Soient $k$ un anneau, $A$ une $k$-algèbre et $J$ un idéal de $A$. Munissons $A$ de la topologie $J$-adique. Soient $C$ une $k$-algèbre, $N$ un idéal de carré nul de $C$; munissons $C$ et $C/N$ de la topologie discrète. Soit $\varphi : A \to C/N$ un homomorphisme continu d’algèbres. Tout relèvement $\tilde{\varphi} : A \to C$ de $\varphi$ est continu : en effet il existe un entier $n$ tel que $\varphi(J^n)$ soit nul, et l’on a $\tilde{\varphi}(J^n) \subset N$, d’où $\tilde{\varphi}(J^{2n}) \subset N^2 = 0$. Il en résulte notamment que, si $A$ est formellement lisse pour la topologie $J$-adique, elle est aussi formellement lisse pour la topologie $J'$-adique pour tout idéal $J'$ contenant $J$.

Nous dirons qu’une $k$-algèbre $A$ est formellement lisse si elle est formellement lisse lorsqu’on la munit de la topologie discrète, c’est-à-dire de la topologie $(0)$-adique ; elle est alors formellement lisse pour la topologie $J$-adique quel que soit l’idéal $J$ de $A$.

#### Remarque 1 {#ac-x-s7-n2-rem-1 .statement}

Soient $k$ un anneau, $A$ une $k$-algèbre et $J$ un idéal de $A$. Si la $k$-algèbre $A/J$ est formellement lisse (pour la topologie discrète), l’application identique de $A/J$ admet un relèvement à $A/J^2$ ; par conséquent les ensembles décrits dans la prop. 2 sont non vides. En particulier, la suite

$$
0 \to J/J^2 \xrightarrow{\bar{d}} (A/J) \otimes_A \Omega_k(A) \longrightarrow \Omega_k(A/J) \to 0
$$

est exacte et scindée.

#### Remarque 2 {#ac-x-s7-n2-rem-2 .statement}

Soient $k$ un anneau, $A$ une $k$-algèbre linéairement topologisée formellement lisse, $M$ un $A$-module dont l’annulateur est ouvert dans $A$. Alors toute dérivation $\delta$ de $k$ dans $M$ se prolonge en une dérivation de $A$ dans $M$. En effet, posons $B = A/Ann(M)$ ; l’application $\lambda \mapsto (\lambda 1_B, \delta(\lambda))$ définit un homomorphisme d’anneaux de $k$ dans $B \oplus M$ (n° 1, exemple), c’est-à-dire une structure de $k$-algèbre sur $B \oplus M$. La surjection canonique $\varphi : A \to B$ est continue, donc admet un relèvement $\tilde{\varphi} : A \to B \oplus M$ ; d’après loc. cit., $pr_2 \circ \tilde{\varphi}$ est une dérivation de $A$ dans $M$ qui prolonge $\delta$.

#### Proposition 3 {#ac-x-s7-prop-3 .statement}

Soit $k$ un anneau.

a) Soient $A$ et $B$ des $k$-algèbres linéairement topologisées et $\rho : A \to B$ un homomorphisme continu de $k$-algèbres. Si $A$ est formellement lisse sur $k$ et $B$ formellement lisse sur $A$, alors $B$ est formellement lisse sur $k$.

b) La $k$-algèbre produit d’une famille finie de $k$-algèbres linéairement topologisées formellement lisses est formellement lisse.

c) Soient $A$ une $k$-algèbre linéairement topologisée, et $\hat{A}$ l’algèbre séparée complétée de $A$ ; pour que $A$ soit formellement lisse sur $k$, il faut et il suffit qu’il en soit ainsi de $\hat{A}$.

Soient C une $k$-algèbre, N un idéal de carré nul de C, et $\pi : C \to C/N$ la surjection canonique. Munissons C et C/N de la topologie discrète.

a) Soit $\psi : B \to C/N$ un homomorphisme continu de $k$-algèbres. Puisque A est formellement lisse sur $k$, il existe un homomorphisme continu de $k$-algèbres $\tilde{\varphi} : A \to C$ tel que $\pi \circ \tilde{\varphi} = \psi \circ \rho$.

$$
\begin{array}{ccc}
 & & C \\
 & \swarrow_{\tilde{\varphi}} & \\
A \xrightarrow{\rho} B \xrightarrow{\psi} C/N & & \downarrow^{\pi}
\end{array}
$$

Considérons C et C/N comme des A-algèbres à l’aide de $\tilde{\varphi}$, de sorte que $\psi$ est un homomorphisme de A-algèbres ; puisque B est formellement lisse sur A, il existe un homomorphisme continu de A-algèbres $\tilde{\psi} : B \to C$ tel que $\pi \circ \tilde{\psi} = \psi$, d’où a).

b) Il suffit de prouver que le produit de deux $k$-algèbres formellement lisses $A_1$ et $A_2$ est formellement lisse. Soit $\varphi : A_1 \times A_2 \to C/N$ un homomorphisme continu de $k$-algèbres. Posons $e_1 = \varphi(1,0)$, $e_2 = \varphi(0,1)$, de sorte que $e_1$ et $e_2$ sont des idempotents orthogonaux dans C/N. Notons $\varphi_1 : A_1 \to (C/N)e_1$ et $\varphi_2 : A_2 \to (C/N)e_2$ les applications définies par $\varphi_1(a_1) = \varphi(a_1,0)$ et $\varphi_2(a_2) = \varphi(0,a_2)$; ce sont des homomorphismes continus de $k$-algèbres, et l’on a $\varphi(a_1, a_2) = \varphi_1(a_1) + \varphi_2(a_2)$ pour tout $(a_1, a_2) \in A_1 \times A_2$. Il existe un élément idempotent $\tilde{e}_1$ de C tel que $\pi(\tilde{e}_1) = e_1$ (A, VIII, § 9, n° 4, prop. 7) ; posons $\tilde{e}_2 = 1 - \tilde{e}_1$, de sorte que $\pi(\tilde{e}_2) = e_2$. Pour $i = 1, 2$, l’homomorphisme $C\tilde{e}_i \to (C/N)e_i$ induit par $\pi$ est surjectif, de noyau $N\tilde{e}_i$; puisque la $k$-algèbre $A_i$ est formellement lisse, l’homomorphisme $\varphi_i$ admet un relèvement continu $\tilde{\varphi}_i$ à $C\tilde{e}_i$. L’application $(a_1, a_2) \mapsto \tilde{\varphi}_1(a_1) + \tilde{\varphi}_2(a_2)$ est un relèvement continu de $\varphi$ à C.

c) Notons $i : A \to \widehat{A}$ l’homomorphisme canonique. Pour tout anneau D, muni de la topologie discrète, l’application qui associe à un homomorphisme continu $f : \widehat{A} \to D$ l’homomorphisme continu $f \circ i : A \to D$ est bijective. L’assertion c) en résulte.

L’assertion c) de la proposition s’applique en particulier lorsque la topologie de $\Lambda$ est la topologie J-adique, où J est un idéal de type fini ; l’adhérence $\widehat{J}$ de J dans $\widehat{A}$ est alors égale à $JA$ et la topologie de $\widehat{A}$ est la topologie $\widehat{J}$-adique (III, § 2, n° 12, cor. 2 de la prop. 16). Par conséquent, il est équivalent de dire que A est formellement lisse pour la topologie J-adique ou que son séparé complété $\widehat{A}$ est formellement lisse pour la topologie J-adique.

#### Proposition 4 {#ac-x-s7-prop-4 .statement}

Soient k un anneau, A et B des $k$-algèbres, J un idéal de A, K un idéal de B.

a) Soient S une partie multiplicative de A et T une partie de k dont l’image dans A est contenue dans S. Si A est formellement lisse sur k pour la topologie J-adique, S $^1\Lambda$ est formellement lisse sur $T^{-1}k$ pour la topologie $S^{-1}J$-adique.

b) Soit $k'$ une $k$-algèbre. Si $A$ est formellement lisse sur $k$ pour la topologie $J$-adique, la $k'$-algèbre $A_{(k')}$ est formellement lisse sur $k'$ pour la topologie $JA_{(k')}$-adique.

c) Désignons par $I$ l’idéal de $A \otimes_k B$ engendré par les images de $J \otimes_k B$ et $A \otimes_k K$. Si $A$ et $B$ sont formellement lisses sur $k$ pour les topologies $J$-adique et $K$-adique respectivement, la $k$-algèbre $A \otimes_k B$ est formellement lisse pour la topologie $I$-adique.

a) Sous les hypothèses de a), soient $C$ une $T^{-1}k$-algèbre, $N$ un idéal de carré nul de $C$; munissons $C$ et $C/N$ de la topologie discrète et notons $\pi : C \to C/N$ la surjection canonique. Soit $\varphi : S^{-1}A \longrightarrow C/N$ un homomorphisme de $T^{-1}k$-algèbres, continu pour la topologie $S^{-1}J$-adique. Notons $i$ l’homomorphisme canonique de $A$ dans $S^{-1}A$. L’application $\varphi \circ i$ est un homomorphisme de $k$-algèbres, continu pour la topologie $J$-adique, donc admet un relèvement $\tilde{\varphi}_0 : A \to C$. Les éléments de $\tilde{\varphi}_0(S)$ sont inversibles modulo $N$, donc inversibles puisque $N$ est de carré nul. Par suite il existe un homomorphisme d’anneaux $\tilde{\varphi} : S^{-1}A \to C$ tel que $\tilde{\varphi} \circ i = \tilde{\varphi}_0$ (II, § 2, n° 1, prop. 1); d’après le cor. 3 de la prop. 2 de loc. cit., $\tilde{\varphi}$ est $T^{-1}k$-linéaire. On a $\pi \circ \tilde{\varphi} \circ i = \varphi \circ i$, d’où $\pi \circ \tilde{\varphi} = \varphi$ (loc. cit., prop. 1), de sorte que $\tilde{\varphi}$ est un relèvement de $\varphi$.

b) Plaçons-nous sous les hypothèses de b). Soient $C$ une $k'$-algèbre, $N$ un idéal de carré nul de $C$; munissons $C$ et $C/N$ de la topologie discrète. Soit $\varphi : A_{(k')} \longrightarrow C/N$ un homomorphisme de $k'$-algèbres, continu pour la topologie $JA_{(k')}$-adique. Notons $i : A \to A_{(k')}$ l’homomorphisme canonique. L’application $\varphi \circ i$ est un homomorphisme de $k$-algèbres de $A$ dans $C/N$, continu pour la topologie $J$-adique; si $A$ est formellement lisse sur $k$ pour la topologie $J$-adique, $\varphi \circ i$ admet un relèvement $\tilde{\psi} : A \to C$. L’homomorphisme de $k'$-algèbres $\tilde{\varphi} : A_{(k')} \longrightarrow C$ déduit de $\tilde{\psi}$ est un relèvement de $\varphi$.

c) Plaçons-nous sous les hypothèses de c). La $B$-algèbre $A \otimes_k B$ est formellement lisse pour la topologie $J(A \otimes_k B)$-adique d’après b), donc pour la topologie $I$-adique; de plus l’homomorphisme canonique $B \to A \otimes_k B$ est continu lorsqu’on munit $B$ de la topologie $K$-adique et $A \otimes_k B$ de la topologie $I$-adique. L’assertion c) résulte donc de la prop. 3, a).

### 3. Exemples d’algèbres formellement lisses

Soit $k$ un anneau.

1) Soit $P$ un $k$-module projectif. La $k$-algèbre symétrique $S_k(P)$ est formellement lisse pour la topologie discrète, et $a fortiori$ pour celle qui est définie par sa graduation. En effet, pour toute $k$-algèbre $C$ et tout idéal $N$ de $C$, les homomorphismes d’algèbres de $S_k(P)$ dans $C$ (resp. $C/N$) sont en correspondance bijective avec les applications $k$-linéaires de $P$ dans $C$ (resp. $C/N$), et l’application canonique $\mathrm{Hom}_k(P, C) \to \mathrm{Hom}_k(P, C/N)$ est surjective.

Par conséquent (prop. 3, c)), la $k$-algèbre $\hat{S}_k(P) = \prod_{n \geq 0} S_k^n(P)$ est formellement lisse (pour la topologie produit des topologies discrètes sur les $S_k^n(P)$) : en effet c’est la complétée de la $k$-algèbre $S_k(P)$ pour la topologie définie par la graduation.

2) Pour toute famille d’indéterminées $\mathbf{T} = (T_i)_{i \in I}$, la $k$-algèbre de polynômes $k[\mathbf{T}]$, et la $k$-algèbre de séries formelles $k[[\mathbf{T}]]$ munie de sa topologie canonique, sont formellement lisses ; cela résulte de l’exemple 1. Si $k$ est un corps, l’extension pure $k(\mathbf{T})$ est formellement lisse (n° 2, prop. 4 a)).

3) Soit $f \in k[T]$ un polynôme en une indéterminée. Dire que la $k$-algèbre $k[T]/(f)$ est formellement lisse, c’est dire que la propriété suivante est satisfaite : *pour toute $k$-algèbre $C$ et tout idéal de carré nul $N$ de $C$, toute racine de $f$ dans $C/N$ se relève en une racine de $f$ dans $C$*. Il en est ainsi lorsque $f$ et sa dérivée $f'$ engendrent l’idéal unité. En effet, soit $\alpha$ une racine de $f$ dans $C/N$ et soit $a$ un élément de $C$ relevant $\alpha$. Alors $f(a)$ appartient à $N$ et par conséquent $f'(a)$ est inversible dans $C$ ; l’élément $b = a - f'(a)^{-1} f(a)$ relève $\alpha$. Puisque $f'(a)^{-1} f(a)$ est de carré nul, on a

$$
f(b) = f(a) - f'(a) f'(a)^{-1} f(a) = 0 .
$$

**Théorème 1** (I. S. Cohen). *Soient $k$ un corps et $K$ une extension séparable de $k$. Alors $K$ est une $k$-algèbre formellement lisse.*

Soient $C$ une $k$-algèbre, $N$ un idéal de carré nul de $C$, $\pi : C \to C/N$ l’homomorphisme canonique et $\varphi : K \to C/N$ un homomorphisme de $k$-algèbres. Il s’agit de construire un relèvement de $\varphi$. Distinguons deux cas.

A) Supposons d’abord $k$ de caractéristique 0. Considérons les couples $(K', \tilde{\varphi}')$, où $K'$ est une sous-extension de $K$ et $\tilde{\varphi}' : K' \to C$ un relèvement de la restriction de $\varphi$ à $K'$. L’ensemble de ces couples, muni de l’ordre défini par la relation de prolongement, est inductif ; d’après le théorème de Zorn (E, III, p. 20, th. 2), il existe un couple $(K', \tilde{\varphi}')$ maximal. Prouvons que $K'$ est égal à $K$. Soit $x \in K - K'$. Si $x$ est transcendant sur $K'$, la $K'$-algèbre $K'(x)$ est formellement lisse (exemple 2). Si $x$ est algébrique sur $K'$, son polynôme minimal $f \in K'[T]$ est étranger à sa dérivée (A, V, p. 37, prop. 4), et $K'(x)$ s’identifie à la $K'$-algèbre $K'[T]/(f)$, donc est une $K'$-algèbre formellement lisse (exemple 3). Dans les deux cas, $K'(x)$ est formellement lisse sur $K'$, et il existe un prolongement de $\tilde{\varphi}'$ à $K'(x)$ qui relève la restriction de $\varphi$ à $K'(x)$, ce qui contredit le caractère maximal de $(K', \tilde{\varphi}')$.

B) Supposons $k$ de caractéristique $p \neq 0$. Considérons l’homomorphisme d’anneaux $F : C \to C$ tel que $F(x) = x^p$; on a $F(x) = 0$ pour $x \in N$, de sorte qu’il existe un unique homomorphisme d’anneaux $\lambda : C/N \to C$ tel que $\lambda \circ \pi = F$. On a $\pi(\lambda(\pi(x))) = \pi(x^p) = \pi(x)^p$; puisque $\pi$ est surjectif, on a donc $\pi(\lambda(z)) = z^p$ pour tout élément $z$ de $C/N$. Par ailleurs, notons $f : K \to K^p$ l’isomorphisme $y \mapsto y^p$ et $f^{-1} : K^p \to K$ l’isomorphisme réciproque. Soit $g : K^p \to C$ le composé de la suite d’homomorphismes d’anneaux

$$
\begin{array}{ccccccccc}
K^p & \xrightarrow{f^{-1}} & K & \xrightarrow{\varphi} & C/N & \xrightarrow{\lambda} & C .
\end{array}
$$

Pour tout $x \in K$, on a $g(x^p) = \lambda(\varphi(x))$. Puisque $\lambda(\alpha z) = \alpha^p \lambda(z)$ pour $\alpha \in k$ et $z \in C/N$, l’application $g$ est $k^p$-linéaire. Puisque l’extension $K$ de $k$ est séparable, $k(K^p)$ s’identifie à $k \otimes_{k^p} K^p$ (A, V, p. 119, remarque) ; il existe par conséquent un unique homomorphisme de $k$-algèbres $h : k(K^p) \to C$ qui coïncide avec $g$ dans $K^p$.

Soit $(a_i)_{i \in I}$ une $p$-base de $K$ sur $k(K^p)$ (A, V, p. 98, théorème 2) ; pour tout $i \in I$, choisissons un élément $b_i$ de $C$ tel que $\pi(b_i) = \varphi(a_i)$. On a $h(a_i^p) = g(a_i^p) = \lambda(\varphi(a_i)) = \lambda(\pi(b_i)) = b_i^p$ pour tout $i \in I$. D’après A, V, p. 94, remarque, il existe un homomorphisme de $k$-algèbres $\tilde{\varphi} : K \to C$, prolongeant $h$ et tel que $\tilde{\varphi}(a_i) = b_i$ pour tout $i$. On a $\pi(\tilde{\varphi}(a_i)) = \pi(b_i) = \varphi(a_i)$ pour tout $i$ et $\pi(\tilde{\varphi}(x^p)) = \pi(h(x^p)) = \pi(g(x^p)) = \pi(\lambda(\varphi(x))) = \varphi(x^p)$ pour tout $x \in K$. On a donc $\pi \circ \tilde{\varphi} = \varphi$, ce qui achève la démonstration.

#### Corollaire {#ac-x-s7-n3-cor-1 .statement}

Soient $k$ un corps, $K$ une extension séparable de $k$ et $A$ une $K$-algèbre linéairement topologisée. Si $A$ est formellement lisse sur $K$, elle est formellement lisse sur $k$.

Cela résulte du théorème et de la prop. 3 a) du n° 2.

#### Remarque 1 {#ac-x-s7-n3-rem-1 .statement}

Soit $k$ un corps. Toute $k$-algèbre étale (A, V, p. 28, déf. 1) est formellement lisse (*loc. cit.*, p. 34, th. 4, d) et n° 2, prop. 3, b)).

#### Remarque 2 {#ac-x-s7-n3-rem-2 .statement}

Nous verrons ci-dessous (cor. 2 du th. 2 du n° 5) qu’une extension de corps qui est formellement lisse est absolument régulière, donc séparable (§ 6, n° 4, exemple 2).

### 4. Relèvements d’homomorphismes dans les algèbres filtrées complètes

Soient $k$ un anneau, $C$ une $k$-algèbre, $(C_n)_{n \in \mathbf{Z}}$ une filtration décroissante de $C$, compatible avec la structure de $k$-algèbre et telle que $C_0 = C$ (III, § 2, n° 1). Supposons $C$ séparée et complète pour la topologie définie par cette filtration, de sorte que l’application canonique $C \to \varprojlim C/C_n$ est un homéomorphisme (*loc. cit.*, n° 6). Soit $m$ un entier $> 0$ ; notons $\pi : C \to C/C_m$ la surjection canonique.

#### Proposition 5 {#ac-x-s7-prop-5 .statement}

Soit $A$ une $k$-algèbre linéairement topologisée formellement lisse. Tout homomorphisme continu de $k$-algèbres $\varphi : \Lambda \to C/C_m$ admet un relèvement continu à $C$.

Pour tout entier $n > m$, notons $\pi_n : C/C_n \to C/C_{n-1}$ la surjection canonique. Puisque $C$ s’identifie à la limite projective des $C/C_n$, il revient au même de se donner un relèvement continu de $\varphi$ à $C$ ou une famille $(\varphi_n)_{n > m}$ d’homomorphismes continus de $k$-algèbres $\varphi_n : A \to C/C_n$, satisfaisant à $\pi_n \circ \varphi_n = \varphi_{n-1}$. Cela nous ramène, par récurrence sur $m$, à prouver l’énoncé lorsque $C_{m+1} = 0$. L’idéal $C_m$ est alors de carré nul (car $2m \geq m+1$), d’où la proposition puisque $A$ est formellement lisse.

#### Exemple {#ac-x-s7-n4-exa-1 .statement}

Soient $C$ une $k$-algèbre et $N$ un idéal nilpotent de $C$. La proposition s’applique à l’algèbre $C$ munie de la filtration $N$-adique. Si $A$ est une $k$-algèbre linéairement topologisée formellement lisse, on obtient que tout homomorphisme continu de $A$ dans la $k$-algèbre $C/N$, munie de la topologie discrète, se relève en un homomorphisme continu de $A$ dans la $k$-algèbre $C$, munie de la topologie discrète.

### 5. Quotients formellement lisses d’algèbres

#### Théorème 2 {#ac-x-s7-thm-2 .statement}

Soient k un anneau, A une k-algèbre et J un idéal de A tel que la k-algèbre A/J soit formellement lisse. Munissons A de la topologie J-adique. Les conditions suivantes sont équivalentes :

(i) la k-algèbre topologique A est formellement lisse ;
(ii) le $\Lambda/J$-module $J/J^2$ est projectif et l’homomorphisme canonique ($\S$ 5, n° 2)
$$
\beta : S_{A/J}(J/J^2) \to \mathrm{gr}_J(A)
$$
est bijectif ;
(iii) le $A/J$-module $J/J^2$ est projectif et il existe un isomorphisme de k-algèbres topologiques de l’algèbre séparée complétée de A sur l’algèbre complétée de l’algèbre graduée $S_{A/J}(J/J^2)$.

Si A est noethérien, ces conditions équivalent aussi à :

(iv) l’idéal J est complètement sécant.

Observons d’abord que (iii) implique (i) : en effet, sous les hypothèses de (iii), l’algèbre $S_{A/J}(J/J^2)$, munie de la topologie associée à sa graduation, est formellement lisse sur $A/J$ (n° 3, exemple 1), donc sur k (n° 2, prop. 3, a)) ; l’assertion (i) résulte alors de la prop. 3, c) du n° 2.

Notons $\hat{A}$ l’algèbre séparée complétée de A et $\hat{J}$ le séparé complété de J. L’homomorphisme canonique $i : A \to \hat{A}$ induit un isomorphisme $A/J \to \hat{A}/\hat{J}$ (III, § 2, n° 12, formule (21)). Soit $\varphi : A/J \to \hat{A}$ un relèvement de cet isomorphisme (n° 4, prop. 5). Notons $\lambda : \hat{J} \to J/J^2$ la surjection déduite de l’isomorphisme canonique $J/J^2 \to \hat{J}/\hat{J}^2$ (III, § 2, n° 12, formule (21)). Soient $a$ un élément de A, $\bar{a}$ sa classe dans $A/J$, et $z$ un élément de $\hat{J}$ ; on a $\varphi(\bar{a}) \equiv i(a) \pmod{\hat{J}}$, d’où $\varphi(\bar{a})z \equiv i(a)z \pmod{\hat{J}^2}$ et $\lambda(\varphi(\bar{a})z) = \lambda(i(a)z) = \bar{a}\lambda(z)$. En d’autres termes, $\lambda$ est A/J-linéaire lorsqu’on munit $\hat{J}$ de la structure de A/J-module déduite de $\varphi$.

Supposons que l’homomorphisme $\lambda$ admette une section A/J-linéaire $\sigma : J/J^2 \to \hat{J}$. Notons S la k-algèbre graduée $S_{A/J}(J/J^2)$ et $\hat{S}$ sa complétée. Soit
$$
\theta : S \to \hat{A}
$$
l’homomorphisme de k-algèbres tel que $\theta(x) = \varphi(x)$ pour $x$ dans $S^0 = A/J$, et $\theta(x) = \sigma(x)$ pour $x$ dans $S^1 = J/J^2$. Puisque $\theta$ applique $S^1$ dans $\hat{J}$, il applique $S^n$ dans $\hat{J}^n$ et se prolonge donc en un homomorphisme continu $\hat{\theta} : \hat{S} \to \hat{A}$. L’application $\mathrm{gr}_1(\theta) : J/J^2 \to \hat{J}/\hat{J}^2$ est la composée de $\sigma$ avec la surjection canonique $\hat{J} \to \hat{J}/\hat{J}^2$ ; puisque $\sigma$ est une section de $\lambda$, $\mathrm{gr}_1(\theta)$ coïncide avec l’isomorphisme canonique de $J/J^2$ sur $\hat{J}/\hat{J}^2$. Par suite $\mathrm{gr}(\theta) : S \to \mathrm{gr}_{\hat{J}}(\hat{A})$ est la composée de la surjection canonique $\beta$ avec l’isomorphisme canonique $\mathrm{gr}_J(A) \to \mathrm{gr}_{\hat{J}}(\hat{A})$ (III, § 2, n° 12, formule (22)).

Prouvons maintenant l’implication (ii) $\Rightarrow$ (iii). Sous l’hypothèse (ii), le A/J-module $J/J^2$ est projectif, donc $\lambda$ admet une section A/J-linéaire ; l’homomorphisme $\hat{\theta} : \hat{S} \to \hat{A}$ associé à cette section par la construction précédente induit par

Prouvons (i) ⇒ (ii). Supposons la k-algèbre topologique A formellement lisse. Prouvons d’abord que le A/J-module J/J^2 est projectif. Soient M un Λ/J-module et f : M → J/J^2 une application A/J-linéaire surjective ; il s’agit de démontrer que f admet une section Λ/J-linéaire.

Notons π : A/J^2 → A/J la surjection canonique. D’après la remarque 1 du n° 2, il existe un isomorphisme de k-algèbres ψ : A/J ⊕ J/J^2 → A/J^2 tel que π(ψ(y, z)) = y et ψ(0, z) = z pour y ∈ A/J, z ∈ J/J^2. Considérons la k-algèbre (A/J) ⊕ M (n° 1, exemple) et l’application u : (A/J) ⊕ M → A/J^2 telle que u(x, m) = ψ(x, f(m)). C’est un homomorphisme surjectif de k-algèbres, dont le noyau est le sous-module Ker f de M, donc est de carré nul. La surjection canonique ρ : A → A/J^2 est continue ; comme la k-algèbre topologique A est formellement lisse, il existe un homomorphisme de k-algèbres ŝ : A → (A/J)⊕M tel que u◦ŝ = ρ. Comme pr_1 = π◦ψ = π◦u, on a pr_1◦ŝ = π◦u◦ŝ = π◦ρ, de sorte que pr_1◦ŝ est la surjection canonique de A sur A/J. On a donc ŝ(J) ⊂ M et par conséquent ŝ(J^2) = 0, de sorte que ŝ induit une application A/J-linéaire s : J/J^2 → M. On a u◦ŝ = ρ et pr_2◦ψ^{-1}◦u(y, m) = f(m) pour y ∈ A/J et m ∈ M. Soient x ∈ J, et ū sa classe dans J/J^2 ; on a f(s(ū)) = f(pr_2(ŝ(x))) = pr_2(ψ^{-1}(ū)) = ū. Ainsi s est une section de f.

Il reste à prouver que l’homomorphisme β est injectif. Puisque le A/J-module J/J^2 est projectif, λ admet une section A/J-linéaire ; notons θ : S → Ā l’homomorphisme associé. L’homomorphisme gr(θ) s’identifie à β. Soit m un entier ; notons Σ_m la k-algèbre graduée quotient de S par l’idéal $\sum_{i>m} S^i$ et $\theta_m : \Sigma_m \to A/J^{m+1}$ l’homomorphisme déduit de θ. Le composé de θ_m avec la surjection canonique A/J^{m+1} → A/J est la projection canonique de Σ_m sur S^0 = A/J ; par suite le noyau de θ_m est un idéal nilpotent. D’après l’exemple du n° 4, il existe un relèvement ψ_m : A → Σ_m de la surjection canonique A → A/J^{m+1}. Comme le composé de ψ_m avec la projection canonique de Σ_m sur A/J est la surjection canonique, ψ_m(J) est formé d’éléments de degré > 0. Par passage aux gradués associés, on déduit de ψ_m une application k-linéaire graduée gr(ψ_m) : gr_J(A) → Σ_m telle que gr_m(θ)◦gr_m(ψ_m) = Id_{J^m/J^{m+1}}. Il en résulte que gr_m(θ), donc aussi β_m, est injectif, ce qui achève de prouver (ii).

Enfin, lorsque A est noethérien, les conditions (ii) et (iv) sont équivalentes (§ 5, n° 2, th. 1).

#### Corollaire 1 {#ac-x-s7-thm-2-cor-1 .statement}

Soient k un corps et A une k-algèbre locale noethérienne telle que l’extension κ_A de k soit séparable. Les conditions suivantes sont équivalentes :

(i) la k-algèbre A est formellement lisse pour la topologie m_A-adique ;
(ii) l’anneau A est régulier ;
(iii) la k-algèbre Λ est absolument régulière (§ 6, n° 4, déf. 1) ;
(iv) la k-algèbre Ā est isomorphe à κ_A[[T_1, ..., T_n]], avec n = dim A.

#### Corollaire 2 {#ac-x-s7-thm-2-cor-2 .statement}

Soient $k$ un corps, $A$ une $k$-algèbre noethérienne et $J$ un idéal de $A$ contenu dans le radical de $A$. Supposons la $k$-algèbre $A$ formellement lisse pour la topologie $J$-adique. Elle est alors absolument régulière.

Soient en effet $k'$ une extension finie de $k$ et $A'$ la $A$-algèbre $A_{(k')}$; il s’agit de prouver que, pour tout idéal maximal $m'$ de $A'$, l’anneau local noethérien $A'_{m'}$ est régulier. Or on a $JA' \subset m'$: en effet, l’image réciproque de $m'$ dans $A$ est un idéal maximal de $A$ (V, § 2, n° 1, prop. 1), donc contient $J$. La $k'$-algèbre $A'$ est formellement lisse pour la topologie $JA'$-adique (n° 2, prop. 4, b)), et la $k'$-algèbre $A'_{m'}$ est formellement lisse pour la topologie $JA'_{m'}$-adique (n° 2, prop. 4, a)), donc aussi pour la topologie $m'A'_{m'}$-adique. Soit $k_0$ le sous-corps premier de $k'$. Alors $A'_{m'}$ est formellement lisse sur $k_0$ pour la topologie $m'A'_{m'}$-adique (cor. du th. 1 du n° 3); comme $\kappa(m')$ est séparable sur $k_0$, l’anneau $A'_{m'}$ est régulier (cor. 1).

#### Corollaire 3 {#ac-x-s7-thm-2-cor-3 .statement}

Soient $k$ un anneau et $A$ une $k$-algèbre formellement lisse.

a) Le $A$-module $\Omega_k(A)$ est projectif.

b) Supposons que l’anneau $A \otimes_k A$ soit noethérien. Notons $\mu : A \otimes_k A \to A$ l’homomorphisme tel que $\mu(x \otimes y) = xy$; alors l’idéal $\mathrm{Ker}(\mu)$ est complètement sécant.

Les $k$-algèbres $A$ et $A \otimes_k A$ sont formellement lisses (n° 2, prop. 4, c)), et $A$ est isomorphe au quotient de $A \otimes_k A$ par le noyau $I$ de $\mu$. On a par définition $\Omega_k(A) = I/I^2$. Ainsi a) et b) résultent du th. 2.

### 6. Extension du corps de base dans les algèbres régulières (caractéristique non nulle)

Soient $k$ un anneau et $\rho : A \to B$ un homomorphisme de $k$-algèbres. On déduit de $\rho$ une application $A$-linéaire $\Omega(\rho) : \Omega_k(A) \to \Omega_k(B)$, et par suite une application $B$-linéaire $\Omega_0(\rho) : B \otimes_A \Omega_k(A) \to \Omega_k(B)$ (A, III, p. 135). Soient $T = (T_i)_{i \in I}$ une famille d’indéterminées, et $t = (t_i)_{i \in I}$ une famille d’éléments de $B$; pour tout polynôme $f = \sum_{\alpha \in \mathbf{N}^{(I)}} c_\alpha T^\alpha$ de $A[T]$, notons $d^\Lambda f(t)$ l’élément $\sum_\alpha t^\alpha \otimes dc_\alpha$ de $B \otimes_A \Omega_k(A)$.

#### Lemme 1 {#ac-x-s7-lem-1 .statement}

Supposons que la $A$-algèbre $B$ admette une famille génératrice $t = (t_i)_{i \in I}$, liée par des relateurs $f_\lambda \in A[T]$ ($\lambda \in \Lambda$). L’homomorphisme $B$-linéaire
$$
\psi : (B \otimes_A \Omega_k(A)) \oplus B^{(I)} \longrightarrow \Omega_k(B)
$$
défini par $\psi(\alpha, (b_i)) = \Omega_0(\rho)(\alpha) + \sum_{i \in I} b_i dt_i$, est surjectif; son noyau est engendré par les éléments $r_\lambda = \left( d^\Lambda f_\lambda(t), \left( \frac{\partial f_\lambda}{\partial T_i}(t) \right)_{i \in I} \right)$ pour $\lambda \in \Lambda$.

Considérons la suite de B-modules et d’applications B-linéaires

$$
B^{(\Lambda)} \xrightarrow{\varphi} (B \otimes_{\Lambda} \Omega_k(A)) \oplus B^{(1)} \xrightarrow{\psi} \Omega_k(B) \longrightarrow 0,
$$

où $\varphi$ est l’homomorphisme tel que $\varphi(e_\lambda) = n_\lambda$; il s’agit de démontrer que cette suite est exacte. D’après A, II, p. 36, th. 1, il suffit de prouver que, pour tout B-module M, la suite

$$
0 \to \mathrm{Hom}_B(\Omega_k(B), M) \xrightarrow{\mathrm{Hom}(\psi, 1)} \mathrm{Hom}_B((B \otimes_A \Omega_k(A)) \oplus B^{(1)}, M) \xrightarrow{\mathrm{Hom}(\varphi, 1)} \mathrm{Hom}_B(B^{(\Lambda)}, M)
$$

est exacte. Compte tenu de la propriété universelle du module des différentielles (A, III, p. 134), cette suite s’identifie à

$$
0 \to D_k(B, M) \xrightarrow{\psi'} D_k(A, M) \oplus M^1 \xrightarrow{\varphi'} M^\Lambda
$$

où $\psi'(D) = (D \circ \rho, (D(t_i)))$ et $\varphi'(\Delta, (m_i)) = (f^\Delta_\lambda(t) + \sum_i \frac{\partial f_\lambda}{\partial T_i}(t) m_i)_{\lambda \in \Lambda}$ (conformément à A, V, p. 121, pour tout polynôme $f = \sum_{\alpha \in \mathbf{N}^{(1)}} c_\alpha T^\alpha$ de $A[T]$, on note $f^\Delta(t)$ l’élément $\sum_\alpha t^\alpha \Delta(c_\alpha)$). Or l’exactitude de cette suite résulte de loc. cit., prop. 1, compte tenu de ce qu’une dérivation $D : B \to M$ est $k$-linéaire si et seulement s’il en est ainsi de $D \circ \rho$.

Soit A un anneau. Il existe une unique structure de $\mathbf{Z}$-algèbre sur A ; on note simplement $\Omega(\Lambda)$ le A-module $\Omega_{\mathbf{Z}}(A)$. Si $\rho : k \to A$ est un homomorphisme d’anneaux, on a une suite exacte canonique de A-modules (A, III, p. 136, prop. 21)

$$
A \otimes_k \Omega(k) \to \Omega(A) \to \Omega_k(A) \to 0.
$$

Supposons que A contienne un sous-corps, et soit P le sous-corps premier de A ; alors $\Omega(P)$ est nul et l’homomorphisme canonique de A-modules $\Omega(A) \to \Omega_P(A)$ est bijectif. Si en outre A est de caractéristique $p \neq 0$ (ce qui signifie par définition que $p$ est un nombre premier, que $p1_A = 0$ et $1_A \neq 0$), alors P s’identifie à $\mathbf{F}_p$. De plus, toute dérivation de A s’annule sur le sous-anneau $A^p$ ; pour tout sous-anneau $k$ de A contenu dans $A^p$ (et, en particulier, pour tout sous-corps parfait $k$ de A), l’application canonique $\Omega(A) \to \Omega_k(A)$ est bijective.

Soient A un anneau de caractéristique $p \neq 0$ et $(f_i)_{1 \leq i \leq n}$ une suite finie d’éléments de A. Notons $A_n$ l’anneau quotient de l’anneau de polynômes $A[T_1, \ldots, T_n]$ par l’idéal engendré par les polynômes $T_i^p - f_i$, pour $1 \leq i \leq n$.

#### Lemme 2 {#ac-x-s7-lem-2 .statement}

Supposons l’anneau A local et noethérien. Alors $A_n$ est local et noethérien. Les conditions suivantes sont équivalentes :

(i) $A_n$ est régulier ;
(ii) A est régulier et les éléments $1 \otimes df_i$ du $\kappa_A$-espace vectoriel $\kappa_A \otimes_A \Omega(A)$ sont linéairement indépendants.

A) Traitons d’abord le cas $n = 1$, en posant $T_1 = T$, $f_1 = f$. Notons $a$ la classe de $f$ dans $\kappa_A$ et distinguons deux cas, suivant que $a$ appartient ou non à $\kappa_A^p$. Si $a \notin \kappa_A^p$, alors le polynôme $T^p - a$ est irréductible dans $\kappa_A$ (A, V, p. 24, lemme 1) et $\kappa_A \otimes_A A_1$ est isomorphe au corps $\kappa_A[T]/(T^p - a)$. L’idéal $m_A A_1$ de $A_1$ est donc maximal, de sorte que l’anneau $A_1$ est local (V, § 2, n° 1, prop. 1). Si $A$ est régulier, $A_1$ est régulier (VIII, § 5, n° 1, prop. 1). D’après A, V, p. 99, prop. 6, l’élément $da$ de $\Omega(\kappa_A)$ n’est pas nul ; puisque c’est l’image par l’application canonique $\kappa_A \otimes_A \Omega(A) \to \Omega(\kappa_A)$ de $1 \otimes df$, ce dernier n’est pas nul. Cela démontre le lemme dans ce cas.

Supposons maintenant que $a$ appartienne à $\kappa_A^p$. Il existe donc un élément $g$ de $A$ tel que $f - g^p \in m_A$. Posons $h = f - g^p$. Puisque $T^p - f = (T - g)^p - h$, la $A$-algèbre $A_1$ est isomorphe à $A[T]/(T^p - h)$. D’après VIII, § 5, n° 4, prop. 4, l’anneau $A_1$ est local et, pour qu’il soit régulier, il faut et il suffit que $A$ soit régulier et que $h$ n’appartienne pas à $m_A^2$. Or, puisque $\kappa_A$ est formellement lisse sur le corps premier (n° 3, th. 1), l’application canonique

$$
\bar{d} : m_A / m_A^2 \to \kappa_A \otimes_A \Omega(A)
$$

est injective (n° 2, remarque 1) ; mais l’image par $\bar{d}$ de la classe de $h$ modulo $m_A^2$ est égale à $1 \otimes dh = 1 \otimes d(f - g^p) = 1 \otimes df$. Cela démontre le lemme dans ce deuxième cas et achève la preuve du cas $n = 1$.

B) Supposons $n > 1$. L’anneau $A_1$ est local et noethérien d’après le cas déjà traité. La $A_1$-algèbre $A_n$ s’identifie au quotient de $A_1[T_2, \ldots, T_n]$ par l’idéal engendré par les $T_i^p - f_i$, $i \geq 2$ ; d’après l’hypothèse de récurrence, c’est un anneau local et la condition (i) équivaut à la conjonction des deux suivantes :

(i') $A_1$ est régulier ;
(ii') les éléments $1 \otimes df_2, \ldots, 1 \otimes df_n$ du $\kappa_{A_1}$-espace vectoriel $\kappa_{A_1} \otimes_{A_1} \Omega(A_1)$ sont linéairement indépendants.

Mais (i') équivaut, comme on vient de le voir, à
(ii'') $A$ est régulier et l’élément $1 \otimes df_1$ du $\kappa_A$-espace vectoriel $\kappa_A \otimes_A \Omega(A)$ n’est pas nul.

D’après le lemme 1, l’homomorphisme canonique $A_1 \otimes_A \Omega(A) \to \Omega(A_1)$ induit un isomorphisme de $((A_1 \otimes_A \Omega(A))/A_1(1 \otimes df_1)) \oplus A_1$ sur $\Omega(A_1)$, et par suite un homomorphisme injectif de $(\kappa_{A_1} \otimes_A \Omega(A))/\kappa_{A_1}(1 \otimes df_1)$ dans $\kappa_{A_1} \otimes_{A_1} \Omega(A_1)$. Comme $\kappa_{A_1} \otimes_A \Omega(A)$ s’identifie à $\kappa_{A_1} \otimes_{\kappa_A} (\kappa_A \otimes_A \Omega(A))$, l’assertion (ii'') équivaut donc à :
(ii''') les éléments $1 \otimes df_2, \ldots, 1 \otimes df_n$ sont linéairement indépendants dans $(\kappa_A \otimes_A \Omega(A))/\kappa_A(1 \otimes df_1)$.

Mais la conjonction de (ii') et (ii'') équivaut à (ii), ce qui démontre le lemme.

#### Proposition 6 {#ac-x-s7-prop-6 .statement}

Soient $k$ un corps de caractéristique $p \neq 0$, $k'$ une extension radicielle de $k$, de degré fini et de hauteur $\leqslant 1$, et $A$ une $k$-algèbre locale régulière. Alors $A_{(k')}$ est un anneau local et les conditions suivantes sont équivalentes :

(i) l’anneau $A_{(k')}$ est régulier ;
(ii) l’application $\kappa_A$-linéaire

$$
\kappa_A \otimes_{{k'}^p} \Omega_{{k'}^p}({k'}^p) \longrightarrow \kappa_A \otimes_A \Omega(A)
$$

déduite de l’injection canonique ${k'}^p \to A$ est injective.

Soit en effet $(x_i)_{i \in I}$ une $p$-base finie de $k'$ sur $k$ (A, V, p. 98) ; pour tout $i \in I$, posons $f_i = x_i^p \in k$. La $k$-algèbre $k'$ s’identifie au quotient de $k[(T_i)_{i \in I}]$ par l’idéal engendré par les polynômes $T_i^p - f_i$, donc la $A$-algèbre $A_{(k')}$ au quotient de $A[(T_i)_{i \in I}]$ par l’idéal engendré par les polynômes $T_i^p - f_i 1_A$.

Par ailleurs, $(f_i)_{i \in I}$ est une $p$-base de ${k'}^p$ sur $k^p$, et le ${k'}^p$-espace vectoriel $\Omega_{k^p}({k'}^p)$ admet pour base la famille des $df_i$ (A, V, p. 97, th. 1). La prop. 6 résulte alors du lemme 2.

### 7. Un critère pour les algèbres locales formellement lisses

#### Proposition 7 {#ac-x-s7-prop-7 .statement}

Soient $k_0$ un anneau, $k$ une $k_0$-algèbre, $A$ une $k$-algèbre, $m$ un idéal maximal de $A$. On suppose que $k$ et $A/m$ sont formellement lisses sur $k_0$. Pour que $A$ soit formellement lisse sur $k$ pour la topologie $m$-adique, il faut et il suffit que les deux conditions suivantes soient réalisées :

(i) l’homomorphisme canonique $S_{A/m}(m/m^2) \to \mathrm{gr}_m(A)$ est bijectif ;
(ii) l’application $A/m$-linéaire

$$
\omega : A/m \otimes_k \Omega_{k_0}(k) \longrightarrow A/m \otimes_A \Omega_{k_0}(A)
$$

déduite de l’application canonique $k \to A$ est injective.

Notons $d_k : k \to \Omega_{k_0}(k)$ et $d_A : A \to \Omega_{k_0}(A)$ les $k_0$-dérivations universelles.

Supposons d’abord $A$ formellement lisse sur $k$ pour la topologie $m$-adique. Alors $A$ est formellement lisse sur $k_0$ pour la topologie $m$-adique (n° 2, prop. 3, a)), ce qui équivaut à (i) (n° 5, th. 2). Par ailleurs, la $k_0$-dérivation $\lambda \mapsto 1 \otimes d_k(\lambda)$ de $k$ dans $A/m \otimes_k \Omega_{k_0}(k)$ peut s’étendre en une $k_0$-dérivation de $A$ dans $A/m \otimes_k \Omega_{k_0}(k)$ (n° 2, remarque 2). Il existe donc une application $A$-linéaire $u : \Omega_{k_0}(A) \to A/m \otimes_k \Omega_{k_0}(k)$ telle que $u(d_A(\lambda 1_A)) = 1 \otimes d_k(\lambda)$ pour tout $\lambda \in k$. L’application $A/m$-linéaire $A/m \otimes_A \Omega_{k_0}(A) \longrightarrow A/m \otimes_k \Omega_{k_0}(k)$ déduite de $u$ est une rétraction de $\omega$, ce qui démontre (ii).

Supposons inversement les conditions (i) et (ii) satisfaites. Alors $A$ est formellement lisse sur $k_0$ pour la topologie $m$-adique (n° 5, th. 2) et le $A$-module $\Omega_{k_0}(A)$ est projectif (n° 5, cor. 3 du th. 2). Fixons un entier $r \geqslant 0$ et considérons l’application $A/m^r$-linéaire

$$
\omega_r : A/m^r \otimes_k \Omega_{k_0}(k) \longrightarrow A/m^r \otimes_A \Omega_{k_0}(A)
$$

déduite de l’application canonique $k \to A$. Soit $(\lambda_i)_{i \in I}$ une famille d’éléments de $k$ tels que les $d_k(\lambda_i)$ forment une base du $k$-espace vectoriel $\Omega_{k_0}(k)$ ; d’après (ii), les éléments $1 \otimes d_A(\lambda_i 1_A)$ sont linéairement indépendants dans $A/\mathfrak{m} \otimes_{\Lambda} \Omega_{k_0}(A)$. D’après II, § 3, n° 2, cor. 1 et 2 de la prop. 5, les $1 \otimes d_A(\lambda_i 1_A)$ forment une base d’un facteur direct du $A/\mathfrak{m}^r$-module $A/\mathfrak{m}^r \otimes_{\Lambda} \Omega_{k_0}(A)$. Il existe donc une application $A/\mathfrak{m}^r$-linéaire
$$
u_r : A/\mathfrak{m}^r \otimes_{\Lambda} \Omega_{k_0}(A) \longrightarrow A/\mathfrak{m}^r \otimes_k \Omega_{k_0}(k)
$$
telle que $u_r(1 \otimes d_A(\lambda_i 1_A)) = 1 \otimes d_k(\lambda_i)$ pour tout $i$, donc $u_r \circ \omega_r = \mathrm{Id}$.

Vérifions maintenant que $A$ est formellement lisse sur $k$ pour la topologie $\mathfrak{m}$-adique. Soient $C$ une $k$-algèbre, $N$ un idéal de carré nul de $C$, et $\pi : C \to C/N$ la surjection canonique ; munissons $C$ et $C/N$ de la topologie discrète. Soit $\varphi : A \to C/N$ un homomorphisme continu de $k$-algèbres. Puisque $A$ est formellement lisse sur $k_0$ pour la topologie $\mathfrak{m}$-adique, il existe un homomorphisme continu de $k_0$-algèbres $\tilde{\varphi}_0 : A \to C$ tel que $\pi \circ \tilde{\varphi}_0 = \varphi$. D’après la prop. 1 du n° 1, les homomorphismes de $k_0$-algèbres $\tilde{\varphi} : A \to C$ tels que $\pi \circ \tilde{\varphi} = \varphi$ sont les applications $x \mapsto v(d_A(x)) + \tilde{\varphi}_0(x)$, où $v$ parcourt $\mathrm{Hom}_{\Lambda}(\Omega_{k_0}(A), N)$. Il s’agit de choisir $v$ de façon que $\tilde{\varphi}$ soit un homomorphisme de $k$-algèbres. L’application $\lambda \mapsto \lambda 1_C - \tilde{\varphi}_0(\lambda 1_A)$ est une $k_0$-dérivation de $k$ dans $N$ (*loc. cit.*), donc peut s’écrire $h \circ d_k$ avec $h \in \mathrm{Hom}_k(\Omega_{k_0}(k), N)$.

Choisissons un entier $r$ tel que le noyau de $\varphi$ contienne $\mathfrak{m}^r$. Le $A$-module $N$ est annulé par $\mathfrak{m}^r$ et il suffit de prendre pour $v$ le composé de la suite d’homomorphismes
$$
\Omega_{k_0}(A) \longrightarrow A/\mathfrak{m}^r \otimes_{\Lambda} \Omega_{k_0}(A) \xrightarrow{u_r} A/\mathfrak{m}^r \otimes_k \Omega_{k_0}(k) \xrightarrow{h'} N ,
$$
où $h'$ est déduit de $h$. En effet, on a pour $\lambda \in k$ :
$$
v(d_A(\lambda 1_A)) = h'u_r(1 \otimes d_A(\lambda 1_A)) = h'(1 \otimes d_k(\lambda)) = h(d_k(\lambda)) = \lambda 1_C - \tilde{\varphi}_0(\lambda 1_A) .
$$

#### Remarque 1 {#ac-x-s7-n7-rem-1 .statement}

Lorsque $A$ est noethérien, la condition (i) signifie que l’anneau local $A_{\mathfrak{m}}$ est régulier (VIII, § 5, n° 2, th. 1).

#### Proposition 8 {#ac-x-s7-prop-8 .statement}

*Soient $k$ un corps et $A$ une $k$-algèbre locale noethérienne. Les conditions suivantes sont équivalentes* :

(i) *A est formellement lisse sur $k$ pour la topologie $\mathfrak{m}_A$-adique* ;
(ii) *A est régulière et l’application $\kappa_A$-linéaire*
$$
\omega : \kappa_A \otimes_k \Omega(k) \longrightarrow \kappa_A \otimes_{\Lambda} \Omega(A)
$$
*déduite de l’injection canonique $k \to A$ est injective* ;
(iii) *A est absolument régulière* ;
(iv) *pour toute extension radicielle $k'$ de $k$, de degré fini et de hauteur $\leqslant 1$, l’anneau local $A_{(k')}$ est régulier*.

(ii) $\Leftrightarrow$ (i) : il suffit d’appliquer la prop. 7 et la remarque 1 ci-dessus, en prenant pour $k_0$ le sous-corps premier de $k$; en effet, $k$ et $\kappa_A$ sont formellement lisses sur $k_0$ (n° 3, th. 1).
(i) $\Rightarrow$ (iii) : cela résulte du cor. 2 du th. 2 (n° 5).

Si k est de caractéristique 0, il résulte du cor. 1 du th. 2 (n° 5) que (iv) implique (i), d’où la proposition dans ce cas. Supposons k de caractéristique $p \neq 0$ et prouvons (iv) ⇒ (ii). Soit $k'$ une extension radicielle de k, de degré fini et de hauteur $\leq 1$. Si A et $A_{(k')}$ sont réguliers, l’application canonique $\kappa_A \otimes_{k'} \Omega_{k^p}({k'}^p) \longrightarrow \kappa_A \otimes_A \Omega(\Lambda)$ est injective (n° 6, prop. 6). D’après le th. 1, b) de A, V, p. 97, appliqué à l’extension k de $k^p$, le k-espace vectoriel $\Omega(k)$, qui coïncide avec $\Omega_{k^p}(k)$, est réunion filtrante croissante des sous-espaces $k \otimes_{{k'}^p} \Omega_{k^p}({k'}^p)$ où $k'$ décrit l’ensemble des extensions finies radicielles de k de hauteur $\leq 1$ contenues dans une clôture algébrique fixée de k. L’assertion (ii) en résulte.

#### Remarque 2 {#ac-x-s7-n7-rem-2 .statement}

Soient k un corps et A une k-algèbre telle que l’anneau $A_{(k')}$ soit régulier pour toute extension radicielle $k'$ de k, de degré fini et de hauteur $\leq 1$; alors A est absolument régulière. En effet, soit $k'$ une telle extension ; pour tout idéal maximal m de A, l’anneau $k' \otimes_k A_m$ s’identifie à un anneau de fractions de $A_{(k')}$, donc est régulier. D’après la prop. 8 ci-dessus et la prop. 6 du § 6, n° 4, l’algèbre A est absolument régulière.

### 8. Existence de rétractions pour les applications linéaires

#### Proposition 9 {#ac-x-s7-prop-9 .statement}

Soient A un anneau, M un A-module de type fini, N un A-module projectif et $u : M \to N$ une application A-linéaire.

a) Soit $\mathfrak{p}$ un idéal premier de A. Les conditions suivantes sont équivalentes :

(i) il existe $f \in A - \mathfrak{p}$ et $v \in \mathrm{Hom}_{A_f}(N_f, M_f)$ avec $v \circ u_f = \mathrm{Id}_{M_f}$;
(ii) il existe $v \in \mathrm{Hom}_{A_\mathfrak{p}}(N_\mathfrak{p}, M_\mathfrak{p})$ avec $v \circ u_\mathfrak{p} = \mathrm{Id}_{M_\mathfrak{p}}$;
(iii) l’application $\kappa(\mathfrak{p})\text{-linéaire } 1 \otimes u : \kappa(\mathfrak{p}) \otimes_A M \to \kappa(\mathfrak{p}) \otimes_A N$ est injective;
(iv) il existe un entier $m \geq 0$, des éléments $x_1, \ldots, x_m$ de M et des formes linéaires $y_1, \ldots, y_m$ sur N tels que les images des $x_i$ dans $M_\mathfrak{p}$ engendrent le $A_\mathfrak{p}$-module $M_\mathfrak{p}$ et que l’on ait $\det(<y_j, u(x_i)>)\notin \mathfrak{p}$;

Si la condition (iv) est vérifiée, on a $m = [\kappa(\mathfrak{p}) \otimes_A M : \kappa(\mathfrak{p})]$ et les éléments $1 \otimes x_i$ forment une base du $\kappa(\mathfrak{p})$-espace vectoriel $\kappa(\mathfrak{p}) \otimes_A M$.

b) L’ensemble U des idéaux premiers $\mathfrak{p}$ de A qui satisfont aux conditions de a) est un ouvert de Spec(A) et les conditions suivantes sont équivalentes :

(i) on a $U = \mathrm{Spec}(A)$;
(ii) U contient tous les idéaux maximaux de A ;
(iii) il existe $v \in \mathrm{Hom}_A(N, M)$ avec $v \circ u = \mathrm{Id}_M$;
(iv) u est injectif et Coker(u) est un A-module projectif.

Démontrons a).

(i) ⇒ (ii) ⇒ (iii) : ces implications sont claires.

(iii) ⇒ (iv) : posons $m = [\kappa(\mathfrak{p}) \otimes_A M : \kappa(\mathfrak{p})]$ et soit $(x_1, \ldots, x_m)$ une suite d’éléments de M telle que les éléments $1 \otimes x_i$ forment une base du $\kappa(\mathfrak{p})$-espace vectoriel $\kappa(\mathfrak{p}) \otimes_A M$. Les images des $x_i$ dans $M_\mathfrak{p}$ engendrent le $A_\mathfrak{p}$-module $M_\mathfrak{p}$ (lemme de Nakayama). Si la condition (iii) est satisfaite, les éléments $1 \otimes u(x_i)$ du $\kappa(\mathfrak{p})$-espace vectoriel $\kappa(\mathfrak{p}) \otimes_A N$ sont linéairement indépendants.

Il existe par ailleurs un A-module N', un ensemble I et un isomorphisme de A-modules $\theta : N \oplus N' \to A^{(I)}$, dont on déduit un isomorphisme de $\kappa(p)$-espaces vectoriels
$$
\overline{\theta} : (\kappa(p) \otimes_{\Lambda} N) \oplus (\kappa(p) \otimes_A N') \to \kappa(p)^{(I)} .
$$
Les éléments $t_i = \overline{\theta}(1 \otimes u(x_i), 0)$ de $\kappa(p)^{(I)}$ forment une famille libre finie. Il existe donc des éléments $\alpha_1, \ldots, \alpha_m$ de I tels que l’on ait $\det(\mathrm{pr}_{\alpha_j}(t_i)) \neq 0$; les formes linéaires $y_j : z \mapsto \mathrm{pr}_{\alpha_j}(\theta(z, 0))$ sur N conviennent.

Supposons la condition (iv) satisfaite. Notons $(a_{ij}) \in M_m(A)$ la matrice de coefficients $a_{ij} = <y_j, u(x_i)>$. Soit g un élément de $A - p$ tel que les images des $x_i$ engendrent le $\Lambda_g$-module $M_g$ (II, § 5, n° 1, prop. 2), et soit $f = g \det(a_{ij})$. Comme $\det(a_{ij})$ est inversible dans $A_f$, les images des éléments $u(x_i)$ dans $N_f$ sont linéairement indépendantes ; par suite les images des $x_i$ dans $M_f$ forment une base de ce $A_f$-module. Cela prouve la dernière assertion de a). Démontrons maintenant (i). Notons $w \in \mathrm{Hom}_A(N, M)$ l’application $z \mapsto \sum_j <y_j, z> x_j$. On a
$$
w \circ u(x_i) = \sum_j a_{ij} x_j ;
$$
comme les images des $x_i$ forment une base de $M_f$ et que la matrice $(a_{ij})$ est inversible dans $M_m(A_f)$, l’endomorphisme $(w \circ u)_f$ de $M_f$ est bijectif, et l’application $v = (w \circ u)_f^{-1} \circ w_f \in \mathrm{Hom}_{A_f}(N_f, M_f)$ vérifie la condition (i).

Démontrons b). Le fait que U soit ouvert résulte de la condition (i) de a).

(iii) $\Rightarrow$ (i) $\Rightarrow$ (ii) : c’est clair.

(iv) $\Rightarrow$ (iii) : sous les hypothèses de (iv), la suite $0 \to M \xrightarrow{u} N \longrightarrow \mathrm{Coker}(u) \to 0$ est exacte et scindée, d’où (iii).

(ii) $\Rightarrow$ (iv) : introduisons comme ci-dessus un isomorphisme de A-modules $\theta : N \oplus N' \to A^{(I)}$. Notons $u'$ l’application de M dans $A^{(I)}$ définie par $u'(x) = \theta(u(x), 0)$. Il existe une partie finie J de I telle que l’image de $u'$ soit contenue dans le sous-module $A^J$ de $A^{(I)}$. Notons $u'' : M \to \Lambda^J$ l’application déduite de $u'$. Sous l’hypothèse (ii), pour tout idéal maximal m de A, l’application $A_m$-linéaire $u'_m$ de $M_m$ dans $A_m^{(I)}$ admet une rétraction, et il en est donc de même de $u''_m$; ainsi $u''_m$ est injective et son image est facteur direct dans $A_m^J$, de sorte que son conoyau est un $A_m$-module projectif. Le A-module $\mathrm{Coker}(u'')$ est de présentation finie par construction ; il est donc projectif (II, § 5, n° 2, th. 1). L’homomorphisme $u''$ est injectif (II, § 3, n° 3, th. 1); par conséquent, $u$ est injectif. Le A-module $\mathrm{Coker}(u')$ est isomorphe, d’une part à $\mathrm{Coker}(u) \oplus N'$, d’autre part à $\mathrm{Coker}(u'') \oplus A^{(I-J)}$. Comme les A-modules $A^{(I-J)}$, $\mathrm{Coker}(u'')$ et $N'$ sont projectifs, il en est de même de $\mathrm{Coker}(u)$, ce qui achève de prouver (iv).

### 9. Le critère jacobien

Soient k un anneau, A une k-algèbre, J un idéal de A et $\bar{d} : J/J^2 \to \Lambda/J \otimes_A \Omega_k(A)$ l’application canonique. Pour chaque A/J-algèbre R, on note
$$
\bar{d}_R : R \otimes_{\Lambda/J} J/J^2 \longrightarrow R \otimes_A \Omega_k(A)
$$

l’application R-linéaire déduite de $\bar{d}$. Si la $k$-algèbre $A/J$ est formellement lisse, $\bar{d}$ possède une rétraction A-linéaire (n° 2, remarque 1) et $\bar{d}_R$ possède une rétraction R-linéaire pour tout R.

Plus généralement :

#### Lemme 3 {#ac-x-s7-lem-3 .statement}

Soit K un idéal de A contenant J. Supposons qu’il existe un entier m tel que $J \cap K^m$ soit contenu dans JK (cette condition est satisfaite si A est noethérienne). Si $A/J$ est formellement lisse sur k pour la topologie K/J-adique, l’application $\bar{d}_{A/K} : A/K \otimes_{A/J} J/J^2 \longrightarrow A/K \otimes_A \Omega_k(A)$ possède une rétraction A-linéaire.

Notons C la $k$-algèbre $A/(JK + K^m)$ ; l’idéal N = $(J + K^m)/(JK + K^m)$ de C est de carré nul et l’anneau quotient C/N s’identifie à $A/(J + K^m)$. Munissons C et C/N de la topologie discrète, et A/J de la topologie K/J-adique. L’homomorphisme canonique $A/J \to A/(J + K^m)$ est continu ; il possède donc un relèvement $\varphi : A/J \to A/(JK + K^m)$.

L’application $a \mapsto a1_C - \varphi(a1_{A/J})$ de A dans N est alors une $k$-dérivation (n° 1, prop. 1), donc s’écrit $a \mapsto u(da)$ avec $u \in \mathrm{Hom}_A(\Omega_k(A), N)$. Mais l’hypothèse $J \cap K^m \subset JK$ implique $J \cap (JK + K^m) = JK$, de sorte que l’application canonique $\psi : J/JK \to N$ est bijective ; il existe donc $v \in \mathrm{Hom}_{A/K}(A/K \otimes_A \Omega_k(A), J/JK)$ telle que, pour a dans A, on ait $a1_C = \varphi(a1_{A/J}) + \psi(v(1 \otimes da))$. Prenant a dans J, on voit que $v(1 \otimes da)$ est égal à la classe de a dans J/JK. Puisque $A/K \otimes_{A/J} J/J^2$ s’identifie à $J/JK$, $v$ est la rétraction cherchée.

Le fait que la condition sur K soit satisfaite lorsque l’algèbre A est noethérienne résulte de III, § 3, n° 1, cor. 2 de la prop. 1.

#### Lemme 4 {#ac-x-s7-lem-4 .statement}

Supposons que A soit formellement lisse sur k pour la topologie J-adique. Pour que $A/J$ soit formellement lisse sur k, il faut et il suffit que l’application canonique $\bar{d}$ possède une rétraction A-linéaire.

On sait déjà que si $A/J$ est formellement lisse sur $k$, l’application $\bar{d}$ admet une rétraction A-linéaire (n° 2, remarque 1). Inversement, supposons que $\bar{d}$ possède une rétraction A-linéaire. Soit $\pi : A/J^2 \to A/J$ la surjection canonique ; d’après la prop. 2 du n° 1, il existe un homomorphisme d’anneaux $h : A/J \to A/J^2$ tel que $\pi \circ h = \mathrm{Id}_{A/J}$. Soient C une $k$-algèbre, N un idéal de C de carré nul, et $\rho : C \to C/N$ la surjection canonique ; munissons C et C/N de la topologie discrète. Soit $u : A/J \to C/N$ un homomorphisme continu de $k$-algèbres. Puisque A est formellement lisse sur $k$ pour la topologie J-adique, il existe un homomorphisme de $k$-algèbres $v : A \to C$ rendant commutatif le diagramme

$$
\begin{array}{ccc}
A & \xrightarrow{v} & C \\
\downarrow & & \downarrow \rho \\
A/J & \xrightarrow{u} & C/N
\end{array}
$$

où les flèches verticales représentent les surjections canoniques. On a $v(J) \subset \mathbf{N}$, donc $v(J^2) \subset \mathbf{N}^2 = \{0\}$, et $v$ définit par passage aux quotients un homomorphisme $\bar{v} : A/J^2 \to C$ qui vérifie $\rho \circ \bar{v} = u \circ \pi$. Alors $\bar{v} \circ h$ est un relèvement de $u$ à $C$.

#### Théorème 3 {#ac-x-s7-thm-3 .statement}

Soient $k$ un anneau, $A$ une $k$-algèbre formellement lisse et $J$ un idéal de type fini de $A$; posons $B = A/J$.

a) Soit $\mathfrak{p}$ un idéal premier de $B$ et soit $q$ l’idéal (premier) de $A$ tel que $\mathfrak{p} = q/J$. Les conditions suivantes sont équivalentes :
(i) la $k$-algèbre $B_{\mathfrak{p}}$ est formellement lisse ;
(ii) il existe $f \in B - \mathfrak{p}$ tel que la $k$-algèbre $B_f$ soit formellement lisse ;
(iii) l’application $\kappa(\mathfrak{p})$-linéaire
$$
\bar{d}_{\kappa(\mathfrak{p})} : \kappa(\mathfrak{p}) \otimes_B J/J^2 \to \kappa(\mathfrak{p}) \otimes_A \Omega_k(\Lambda)
$$
est injective ;
(iv) il existe un entier $m \geqslant 0$, des éléments $f_1, \ldots, f_m$ de $J$, dont les images $(f_1)_q, \ldots, (f_m)_q$ engendrent l’idéal $J_q$, et des $k$-dérivations $D_1, \ldots, D_m$ de $A$ tels que $\det(D_j(f_i)) \notin q$.

b) L’ensemble des idéaux premiers $\mathfrak{p}$ de $B$ qui satisfont aux conditions équivalentes de a) est ouvert dans $\mathrm{Spec}(B)$. Pour que $B$ soit formellement lisse sur $k$, il faut et il suffit que tout idéal premier (resp. maximal) de $B$ satisfasse à ces conditions.

c) Supposons $A$ noethérien. Les conditions de a) équivalent aussi à :
(v) la $k$-algèbre $B_{\mathfrak{p}}$ est formellement lisse pour la topologie $\mathfrak{p}B_{\mathfrak{p}}$-adique.
De plus, sous les conditions de (iv), l’idéal $J_q$ est complètement sécant et la suite $((f_1)_q, \ldots, (f_m)_q)$ est complètement sécante pour $A_q$.

Posons $M = J/J^2$ et $N = B \otimes_A \Omega_k(A)$. Le $B$-module $M$ est de type fini, et le $B$-module $N$ est projectif (n° 5, cor. 3 du th. 2). Pour toute partie multiplicative $S$ de $A$, la $k$-algèbre $S^{-1}A$ est formellement lisse (n° 2, prop. 4, a)). D’après le lemme 4, les conditions (i) et (ii) équivalent donc respectivement à
(i') l’application $\bar{d}_{B_{\mathfrak{p}}} : M_{\mathfrak{p}} \to N_{\mathfrak{p}}$ possède une rétraction $B_{\mathfrak{p}}$-linéaire ;
(ii') il existe $f \in B - \mathfrak{p}$ tel que l’application $\bar{d}_{B_f} : M_f \to N_f$ possède une rétraction $B_f$-linéaire.

La prop. 9 du n° 8 appliquée à l’anneau $B$ et à l’homomorphisme $\bar{d} : M \to N$ implique l’équivalence des conditions (i'), (ii'') et (iii), et entraîne aussi les assertions de b) (en utilisant de nouveau le lemme 4). Par ailleurs (iii) équivaut à :
(iii') l’application $\kappa(q) \otimes_A J \to \kappa(q) \otimes_A \Omega_k(A)$ déduite de $d : J \to \Omega_k(A)$ est injective,
tandis que (iv) peut s’écrire :
(iv') il existe un entier $m \geqslant 0$, des éléments $f_1, \ldots, f_m$ de $J$ dont les images engendrent l’idéal $J_q$ de $A_q$ et des éléments $y_1, \ldots, y_m$ de $\mathrm{Hom}_A(\Omega_k(A), A)$ tels que $\det(<y_j, df_i>) \notin q$.

Puisque le $A$-module $\Omega_k(A)$ est projectif (n° 5, cor. 3 du th. 2), la prop. 9 du n° 8, appliquée à l’anneau $A$ et à l’homomorphisme $d : J \to \Omega_k(A)$, fournit l’équivalence de (iii') et (iv').

Supposons enfin l’anneau $A$ noethérien. Il est clair que (i) implique (v). Sous l’hypothèse (v), le lemme 3 entraîne que l’application

$$
\bar{d}_{\kappa(q)} : \kappa(q) \otimes_{B_p} J_q / J_q^2 \longrightarrow \kappa(q) \otimes_{A_q} \Omega_k(A_q)
$$

est injective, d’où (iii).

Sous les conditions de (iv), on a $m = [\kappa(q) \otimes_A J : \kappa(q)]$ (n° 9, prop. 8). D’après le th. 2 du n° 5, l’idéal $J_q$ est complètement sécant, et la suite $((f_1)_q, \ldots, (f_m)_q)$ est complètement sécante pour $A_q$ ($§ 1$, n° 3, cor. 2 du th. 1). Cela démontre c).

#### Corollaire 1 {#ac-x-s7-thm-3-cor-1 .statement}

*Soient $k_0$ un anneau, $k$ une $k_0$-algèbre noethérienne formellement lisse, et $B$ une $k$-algèbre locale essentiellement de type fini. Si la $k_0$-algèbre $B$ est formellement lisse pour la topologie $\mathfrak{m}_B$-adique, elle est formellement lisse.*

Il existe un entier $n \geqslant 0$, une partie multiplicative $S$ de $k[T_1, \ldots, T_n]$ et un $k$-homomorphisme surjectif $S^{-1} k[T_1, \ldots, T_n] \to B$. L’algèbre $S^{-1} k[T_1, \ldots, T_n]$ est noethérienne et formellement lisse sur $k$ (n° 3, exemple 2 et n° 2, prop. 4, a)), donc sur $k_0$ (n° 2, prop. 3, a)). Le corollaire résulte alors du th. 3, c).

#### Corollaire 2 {#ac-x-s7-thm-3-cor-2 .statement}

*Soient $k_0$ un anneau, $k$ une $k_0$-algèbre noethérienne formellement lisse, et $B$ une $k$-algèbre essentiellement de type fini. L’ensemble $U$ des idéaux premiers $\mathfrak{p}$ de $B$ tels que la $k_0$-algèbre $B_{\mathfrak{p}}$ soit formellement lisse (pour la topologie discrète ou la topologie $\mathfrak{p}B_{\mathfrak{p}}$-adique) est ouvert dans $\operatorname{Spec}(B)$ et les conditions suivantes sont équivalentes :

(i) *on a* $U = \operatorname{Spec}(B)$ ;
(ii) $U$ *contient tous les idéaux maximaux de* $B$ ;
(iii) *la* $k_0$*-algèbre* $B$ *est formellement lisse*.

Cela résulte comme précédemment du th. 3.

#### Remarque 1 {#ac-x-s7-n9-rem-1 .statement}

Les corollaires 1 et 2 s’appliquent notamment lorsque $k_0$ est un corps et que l’on est dans l’un des deux cas suivants :
a) $B$ est une algèbre essentiellement de type fini sur une extension séparable de $k_0$ (th. 1 du n° 3) ;
b) $B$ est une $k_0$ algèbre locale noethérienne complète dont le corps résiduel $\kappa_B$ est une extension séparable de $k_0$ (on prend dans ce cas pour $k$ une algèbre de séries formelles sur $\kappa_B$ dont $B$ est un quotient (n° 3 et IX, § 3, n° 3)).
Dans chacun de ces cas, il résulte du cor. 2, compte tenu de la prop. 8 du n° 7 et de la prop. 6, b) du § 6, n° 4, que la $k_0$-algèbre $B$ est formellement lisse si et seulement si elle est absolument régulière.

**Corollaire 3 (Zariski).** — *Soient $k$ un corps, $A$ une $k$-algèbre locale régulière, et $J$ un idéal de $A$ distinct de $A$. On suppose que la $k$-algèbre $A$ est essentiellement de type fini ou complète. Pour que l’anneau local $A/J$ soit régulier, il faut et il suffit qu’il existe un entier $m \geqslant 0$, des éléments $f_1, \ldots, f_m$ de $J$ engendrant $J$ et des dérivations $D_1, \ldots, D_m$ de $A$ telles que $\det(D_j(f_i)) \notin \mathfrak{m}_A$. Les éléments $(f_1, \ldots, f_m)$ font alors partie d’un système de coordonnées de $A$ et l’idéal $J$ est premier.*

Soit $k_0$ le sous-corps premier de $k$. La $k_0$-algèbre $A$ est absolument régulière ($§ 6$, n° 4, exemple 1), donc formellement lisse (remarque 1 ci-dessus). Pour les mêmes raisons, dire que $A/J$ est régulier équivaut à dire que c’est une $k_0$-algèbre formellement lisse. La première assertion résulte donc du th. 3, qui implique aussi que la suite $(f_1, \ldots, f_m)$ est complètement sécante pour $A$. On applique alors la prop. 2 de VIII, $§ 5$, n° 3.

#### Remarque 2 {#ac-x-s7-n9-rem-2 .statement}

Sous les hypothèses du cor. 3, le $A$-module $\Omega(A)$ est projectif (n° 5, cor. 3 du th. 2), donc libre ; toute dérivation de $A$ dans $\kappa_A$ se relève donc en une dérivation de $A$. La condition de l’énoncé peut donc s’exprimer ainsi : il existe un système générateur $(f_1, \ldots, f_m)$ de $J$ et des dérivations $D_1, \ldots, D_m$ de $A$ dans $\kappa_A$, tels que $\det(D_j(f_i)) \neq 0$.

#### Corollaire 4 (Zariski) {#ac-x-s7-thm-3-cor-4 .statement}

*Soient $k$ un corps et $A$ une $k$-algèbre essentiellement de type fini ou locale noethérienne complète. L’ensemble des idéaux premiers $\mathfrak{p}$ de $A$ tels que l’anneau local $A_{\mathfrak{p}}$ soit régulier est ouvert dans $\mathrm{Spec}(A)$*.

Il suffit d’appliquer la remarque 1 en prenant pour $k_0$ le sous-corps premier de $k$.

### 10. Algèbres lisses

#### Lemme 5 {#ac-x-s7-lem-5 .statement}

*Soit $\rho : A \to B$ un homomorphisme local d’anneaux locaux noethériens. On suppose que $B$ est essentiellement de type fini sur $A$. Pour que la $A$-algèbre $B$ soit formellement lisse, il faut et il suffit que le $A$-module $B$ soit plat et que la $\kappa_A$-algèbre $\kappa_A \otimes_A B$ soit absolument régulière.*

Il existe un entier $n \geqslant 0$, un idéal premier $q$ de $A[T_1, \ldots, T_n]$ et un homomorphisme surjectif $h$ de $A[T_1, \ldots, T_n]_q$ dans $B$. Notons $C$ la $A$-algèbre locale $A[T_1, \ldots, T_n]_q$; elle est formellement lisse (n° 3, exemple 2 et n° 2, prop. 4, a)) et plate sur $A$, et on peut identifier $B$ à la $A$-algèbre $C/J$, où $J = \mathrm{Ker}(h)$.

Posons $\overline{C} = \kappa_A \otimes_A C$ et $\overline{B} = \kappa_A \otimes_A B$. Supposons $B$ formellement lisse sur $A$. La $\kappa_A$-algèbre $\overline{B}$ est alors formellement lisse (n° 2, prop. 4, b)), donc absolument régulière (n° 5, cor. 2 du th. 2). De plus, puisque $\overline{C}/J\overline{C}$ s’identifie à $\overline{B}$ et que la $\kappa_A$-algèbre $\overline{C}$ est formellement lisse, l’idéal $J\overline{C}$ de $\overline{C}$ est complètement sécant (n° 5, th. 2). Il résulte alors du $§ 5$, n° 6, prop. 6 que le $A$-module $B$ est plat.

Supposons inversement que $B$ soit plat sur $A$ et que la $\kappa_A$-algèbre $\overline{B}$ soit absolument régulière. Alors la $\kappa_A$-algèbre locale $\overline{B}$ est formellement lisse (remarque 1 du n° 9 avec $k = k_0 = \kappa_A$). Posons $\overline{J} = \kappa_A \otimes_A J$; puisque $B$ est un $A$-module plat, l’application canonique $\overline{J} \to J\overline{C}$ est bijective et $\overline{B}$ s’identifie à $\overline{C}/\overline{J}$. Il en résulte (remarque 1 du n° 2) que l’application canonique

$$
\overline{J}/\overline{J}^2 \longrightarrow \overline{B} \otimes_{\overline{C}} \Omega_{\kappa_A}(\overline{C})
$$

est injective et admet une rétraction. Or $\overline{J}/\overline{J}^2$ s’identifie à $\kappa_A \otimes_A J/J^2$, donc à $\overline{B} \otimes_B J/J^2$; d’autre part le $\overline{C}$-module $\Omega_{\kappa_A}(\overline{C})$ est canoniquement isomorphe à $\overline{C} \otimes_C \Omega_A(C)$ (A, III, p. 136, prop. 20), donc $\overline{B} \otimes_{\overline{C}} \Omega_{\kappa_A}(\overline{C})$ est canoniquement isomorphe à $\overline{B} \otimes_C \Omega_A(C)$. Passant au quotient par l’idéal maximal de $\overline{B}$, on obtient un homomorphisme injectif

$$
\kappa_B \otimes_B J/J^2 \longrightarrow \kappa_B \otimes_C \Omega_A(C)
$$

qui n’est autre que $d_{\kappa_B}$. Ainsi B est formellement lisse sur A (th. 3).

#### Théorème 4 {#ac-x-s7-thm-4 .statement}

Soient A un anneau noethérien et B une A-algèbre essentiellement de type fini. Les conditions suivantes sont équivalentes :

(i) la A-algèbre B est formellement lisse ;
(ii) pour tout $q \in \mathrm{Spec}(B)$, la A-algèbre $B_q$ est formellement lisse (resp. formellement lisse pour la topologie $qB_q$-adique) ;
(iii) le A-module B est plat et, pour tout $p \in \mathrm{Spec}(A)$, la $\kappa(p)\text{-algèbre} \ \kappa(p) \otimes_A B$ est absolument régulière ;
(iv) le A-module B est plat et, pour toute A-algèbre régulière R, l’anneau $R \otimes_A B$ est régulier ;
(v) le A-module B est plat et le noyau de l’homomorphisme $\mu : B \otimes_A B \to B$ tel que $\mu(x \otimes y) = xy$ est un idéal complètement sécant.

L’équivalence de (i) et (ii) résulte du cor. 2 du th. 3 (n° 9).

(i)⇒(v) : supposons la A-algèbre B formellement lisse. Soient q un idéal premier de B, et p son image réciproque dans A. La $A_p$-algèbre $B_q$ est formellement lisse (prop. 4, a) du n° 2), donc plate (lemme 5) ; par suite le A-module B est plat (II, § 3, n° 4, prop. 15). D’autre part, l’anneau $B \otimes_A B$ est noethérien (§ 6, n° 1, cor. de la prop. 2), donc l’idéal $\mathrm{Ker}\,\mu$ est complètement sécant d’après le cor. 3 du th. 2 (n° 5).

(v)⇒(iii) : supposons la condition (v) satisfaite. Posons $I = \mathrm{Ker}(\mu)$. Soit $p \in \mathrm{Spec}(A)$. L’application

$$
1 \otimes \mu : \kappa(p) \otimes_A (B \otimes_A B) \to \kappa(p) \otimes_A B
$$

s’identifie à l’application

$$
\mu_p : (\kappa(p) \otimes_A B) \otimes_{\kappa(p)} (\kappa(p) \otimes_A B) \to \kappa(p) \otimes_A B
$$

déduite de la multiplication de la $\kappa(p)\text{-algèbre} \ \kappa(p) \otimes_A B$. L’idéal $\mathrm{Ker}(\mu_p)$ s’identifie à $I(\kappa(p) \otimes_A (B \otimes_A B))$. Il est complètement sécant puisque le A-module B est plat (§ 5, n° 6, prop. 6). L’assertion (iii) résulte alors de la prop. 8 du § 6, n° 5.

(iii)⇒(ii) : soient q un idéal premier de B, et p son image réciproque dans A. Sous les hypothèses de (iii), le $A_p$-module $B_q$ est plat, et la $\kappa(p)\text{-algèbre} \ \kappa(p) \otimes_{A_p} B_q$, qui s’identifie à un anneau de fractions de $\kappa(p) \otimes_A B$, est absolument régulière (§ 6, n° 4, prop. 6). Il résulte du lemme 5 que $B_q$ est formellement lisse sur $A_p$, donc sur A (n° 2, prop. 3 et 4).

(iii)⇒(iv) : plaçons-nous sous les hypothèses de (iii). Soit R une A-algèbre régulière. Le R-module $R \otimes_A B$ est plat (I, § 2, n° 7, cor. 2 à la prop. 8). Soient r un idéal premier de R et p son image réciproque dans A ; l’anneau $\kappa(r) \otimes_R (R \otimes_A B)$, qui s’identifie à $\kappa(r) \otimes_{\kappa(p)} (\kappa(p) \otimes_A B)$, est régulier (§ 6, n° 4, cor. 2 de la prop. 7). L’anneau $R \otimes_A B$ est donc régulier (§ 4, n° 5, cor. de la prop. 9).

(iv) ⇒ (iii) : soit $p$ un idéal premier de $A$ et soit $k$ une extension de $\kappa(p)$; sous les hypothèses de (iv), l’anneau $k \otimes_{\kappa(p)} (\kappa(p) \otimes_A B)$, qui s’identifie à $k \otimes_A B$, est régulier, d’où (iii).

#### Définition 2 {#ac-x-s7-def-2 .statement}

Soit $A$ un anneau noethérien. On dit qu’une $A$-algèbre $B$ est lisse si elle est essentiellement de type fini et si elle satisfait aux conditions équivalentes du théorème 4.

#### Proposition 10 {#ac-x-s7-prop-10 .statement}

Soit $A$ un anneau noethérien.

a) Soient $A'$ une $A$-algèbre noethérienne et $B$ une $A$-algèbre lisse. Alors la $A'$-algèbre $A' \otimes_A B$ est lisse.

b) Soient $B$ une $A$-algèbre lisse et $C$ une $B$-algèbre lisse. Alors la $A$-algèbre $C$ est lisse.

c) Soient $B$ et $C$ deux $A$-algèbres lisses. Alors la $A$-algèbre $B \otimes_A C$ est lisse.

Cela résulte de la prop. 4 du n° 2 et des énoncés analogues pour les algèbres essentiellement de type fini (§ 6, n° 1).

#### Exemple 1 {#ac-x-s7-n10-exa-1 .statement}

Les algèbres lisses sur un corps $k$ sont les $k$-algèbres essentiellement de type fini et absolument régulières.

#### Exemple 2 {#ac-x-s7-n10-exa-2 .statement}

Soient $A$ un anneau noethérien, $T = (T_i)_{i \in I}$ une famille finie d’indéterminées. La $A$-algèbre $A[T]$ est lisse. Plus généralement, soient $F_1, \ldots, F_m$ des éléments de $A[T]$, et soit $B$ la $A$-algèbre $A[T]/(F_1, \ldots, F_m)$. Si en tout idéal maximal $n$ de $B$ la classe (mod. $n$) de la matrice $\left( \frac{\partial F_j}{\partial T_i} \right)$ est de rang $m$, la $A$-algèbre $B$ est lisse (th. 3 du n° 9).

## EXERCICES {#ac-x-s7-exercises}

See the [exercises for § 7](exercises/s7/).
