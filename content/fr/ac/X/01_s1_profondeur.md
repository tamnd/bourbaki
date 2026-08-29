---
book: ac
book_title: Commutative Algebra
chapter: X
chapter_title: Profondeur, régularité, dualité
section: 1
section_title: Profondeur
lang: fr
source: ac-x-fr
book_pages: AC X.3-AC X.22
pdf_pages: 0002-0021, 0150-0153
extraction: ocr
subsections:
    - "no": 2
      title: Profondeur et acyclicité
      page: 4
      pdf_page: 3
    - "no": 3
      title: Profondeur et complexe de Koszul
      page: 5
      pdf_page: 4
    - "no": 4
      title: Profondeur et suites régulières
      page: 8
      pdf_page: 7
    - "no": 5
      title: Profondeur le long d’une partie fermée
      page: 0
      pdf_page: 9
    - "no": 6
      title: Profondeur des algèbres
      page: 11
      pdf_page: 10
    - "no": 7
      title: Majorations de la profondeur
      page: 13
      pdf_page: 12
    - "no": 8
      title: Anneaux noethériens localement intègres ; anneaux noethériens normaux
      page: 15
      pdf_page: 14
    - "no": 9
      title: Profondeur et connexité
      page: 0
      pdf_page: 15
    - "no": 10
      title: Profondeur et normalité
      page: 19
      pdf_page: 18
statements: 60
exercises: 18
content_sha256: 225c9460593c8de13dabe30c37d11a994b8dc41f2db1aa24ece65402eb5a3910
---

## § 1. PROFONDEUR

#### Proposition 1 {#ac-x-s1-prop-1 .statement}

Soient $A$ un anneau, $J$ un idéal de $A$ et $0 \to M' \to M \to M'' \to 0$ une suite exacte de $A$-modules. Posons

$$
p' = \operatorname{prof}(J; M') \quad , \quad p = \operatorname{prof}(J; M) \quad , \quad p'' = \operatorname{prof}(J; M'') .
$$

On est alors dans l’un des trois cas suivants, qui s’excluent mutuellement :

$$
p' = p \leqslant p'' \quad , \quad p = p'' < p' \quad , \quad p'' = p' - 1 < p .
$$

Considérons la suite exacte des modules d’extensions associée à $A/J$ et à la suite exacte ci-dessus (A, X, p. 92, th. 2). Excluons le cas $p = p' = p'' = +\infty$; il existe alors dans cette suite un premier module non nul, et le module suivant est également non nul. Cela donne les trois possibilités suivantes :

a) Le premier module non nul est $\operatorname{Ext}_A^{p'}(A/J, M')$. On a alors $p' = p \leqslant p''$.

b) Le premier module non nul est $\operatorname{Ext}_A^p(A/J, M)$. On a alors $p = p'' < p'$.

c) Le premier module non nul est $\operatorname{Ext}_A^{p''}(A/J, M'')$. On a alors $p'' + 1 = p' \leqslant p$.

#### Remarque 5 {#ac-x-s1-rem-5 .statement}

Supposons que l’on ait $p = p'$ et que l’injection $u : M' \to M$ qui intervient dans la suite exacte de la prop. 1 appartienne à $J \operatorname{Hom}_A(M', M)$. *On a alors* $p'' = p - 1$. En effet, l’hypothèse entraîne que l’application $\operatorname{Ext}_A^i(1_{A/J}, u)$ est nulle pour tout entier $i$; cela exclut le cas a) considéré ci-dessus.

#### Proposition 2 {#ac-x-s1-prop-2 .statement}

Soient $A$ un anneau, $J$ un idéal de $A$, $M$ un $A$-module et $N$ un $A$-module annulé par une puissance de $J$. *On a* $\operatorname{Ext}_A^i(N, M) = 0$ *pour tout entier* $i < \operatorname{prof}_A(J; M)$.

Supposons d’abord $JN = 0$ et raisonnons par récurrence sur l’entier $i < \operatorname{prof}_A(J; M)$. L’assertion est évidente pour $i < 0$. Considérons $N$ comme un $(A/J)$-module et choisissons une suite exacte de $(A/J)$-modules

$$
0 \to K \longrightarrow (A/J)^{(I)} \longrightarrow N \to 0 .
$$

On en déduit une suite exacte de modules d’extensions

$$
\operatorname{Ext}_A^{i-1}(K, M) \longrightarrow \operatorname{Ext}_A^i(N, M) \longrightarrow \operatorname{Ext}_A^i((A/J)^{(I)}, M) .
$$

Le $A$-module $\operatorname{Ext}_A^{i-1}(K, M)$ est nul d’après l’hypothèse de récurrence, et le $A$-module $\operatorname{Ext}_A^i((A/J)^{(I)}, M)$ est isomorphe à $\operatorname{Ext}_A^i(A/J, M)^I$ (A, X, p. 89, prop. 7), qui est nul par définition de la profondeur. Par suite on a $\operatorname{Ext}_A^i(N, M) = 0$.

Passons au cas général, et raisonnons par récurrence sur le plus petit entier $m > 0$ tel que $J^m N = 0$. Nous venons de traiter le cas $m = 1$. Supposons $m > 1$ et soit $i < \operatorname{prof}_A(J; M)$ un entier. Considérons la suite exacte

$$
\operatorname{Ext}_A^i(N/JN, M) \longrightarrow \operatorname{Ext}_A^i(N, M) \longrightarrow \operatorname{Ext}_A^i(JN, M)
$$

déduite de la suite exacte $0 \to JN \to N \to N/JN \to 0$. Les deux modules extrêmes sont nuls d’après l’hypothèse de récurrence, puisque $N/JN$ et $JN$ sont annulés par $J^{m-1}$. On a donc $\operatorname{Ext}_A^i(N, M) = 0$, ce qu’on voulait démontrer.

#### Corollaire 1 {#ac-x-s1-prop-2-cor-1 .statement}

Soit m un entier > 0 et soit J' un idéal de A qui contient J^m. On a prof_A(J ; M) \leq prof_A(J' ; M).

En effet J^m annule le A-module A/J', donc Ext^i_A(A/J', M) est nul pour tout entier i < prof_A(J ; M) (prop. 2).

#### Corollaire 2 {#ac-x-s1-prop-2-cor-2 .statement}

Supposons l’idéal J de type fini, et soit J' un idéal de A tel que V(J) \supset V(J').

a) On a prof_A(J ; M) \leq prof_A(J' ; M).

b) Si l’idéal J' est de type fini et si V(J) = V(J'), on a prof_A(J ; M) = prof_A(J' ; M).

D’après II, § 4, n° 3, cor. 2 de la prop. 11 et § 2, n° 6, prop. 15, il existe un entier m > 0 tel que J^m \subset J'. L’assertion a) résulte donc du cor. 1 et l’assertion b) s’en déduit.

Le cor. 2 peut être en défaut lorsque l’idéal J n’est pas de type fini (exercice 2).

### 2. Profondeur et acyclicité

#### Proposition 3 {#ac-x-s1-prop-3 .statement}

Soient A un anneau, C un complexe borné à gauche de A-modules et p un entier. On suppose que pour tout couple d’entiers (m, n) avec m \geq n \geq p, la profondeur du A-module C_m relativement à l’annulateur de H_n(C) est > m - n. On a alors H_n(C) = 0 pour n \geq p.

Puisque C est borné à gauche, H_n(C) est nul pour n assez grand. Si la conclusion était fausse, il existerait un entier q \geq p tel que H_n(C) = 0 pour n > q et H_q(C) \neq 0. Désignons par J l’annulateur de H_q(C) ; on a alors prof_A(J ; H_q(C)) = 0. Par ailleurs, puisque Z_q(C) est un sous-module de C_q, et qu’on a par hypothèse prof_A(J ; C_q) > q - q = 0, on a prof_A(J ; Z_q(C)) > 0. On déduit alors de la suite exacte

$$
0 \to B_q(C) \to Z_q(C) \to H_q(C) \to 0
$$

l’égalité prof_A(J ; B_q(C)) = 1 (n° 1, prop. 1). D’après la définition de q, B_n(C) est égal à Z_n(C) pour tout entier n > q. Des suites exactes canoniques

$$
0 \to B_n(C) \to C_n \to B_{n-1}(C) \to 0 \quad (n > q)
$$

et de l’hypothèse prof_A(J ; C_n) > n - q, on tire par récurrence l’égalité prof_A(J ; B_n(C)) = n - q + 1 pour tout n \geq q (loc. cit.). Mais cela est absurde puisque B_n(C) est nul pour n assez grand.

#### Corollaire 1 {#ac-x-s1-prop-3-cor-1 .statement}

Soient A un anneau, J un idéal de A, C un complexe borné à gauche de A-modules et p un entier. On suppose qu’on a JH_m(C) = 0 et prof_A(J ; C_m) > m - p pour m \geq p. On a alors H_n(C) = 0 pour n \geq p.

En effet pour n \geq p l’annulateur J_n de H_n(C) contient J, donc on a prof_A(J_n ; C_m) \geq prof_A(J ; C_m) (n° 1, cor. 1 de la prop. 2), de sorte que l’hypothèse de la proposition est satisfaite.

#### Corollaire 2 {#ac-x-s1-prop-3-cor-2 .statement}

Soient $A$ un anneau local, $C$ un complexe borné à gauche de $A$-modules, $p$ un entier. On suppose que pour $m \geq p$, $H_m(C)$ est de longueur finie et $C_m$ de profondeur $> m - p$. On a alors $H_n(C) = 0$ pour $n \geq p$.

Le $A$-module $\bigoplus_{m \geq p} H_m(C)$ est de longueur finie. Notons $J$ son annulateur ; d’après A, VIII, § 1, n° 3, corollaire, l’anneau $A/J$ est artinien, donc $J$ contient une puissance de l’idéal maximal de $A$ (A, VIII, § 10, n° 1, th. 1). On a par suite $\operatorname{prof}_A(J; C_m) \geq \operatorname{prof}(C_m) > m - p$ pour $m \geq p$ (n° 1, cor. 1 de la prop. 2), de sorte qu’on peut appliquer le cor. 1.

### 3. Profondeur et complexe de Koszul

Soient $A$ un anneau, $M$ un $A$-module, $x = (x_i)_{i \in I}$ une famille d’éléments de $A$. Notons $u : A^{(I)} \to A$ la forme linéaire telle que $u(e_i) = x_i$ pour tout $i \in I$, et $K^\bullet(x, M)$ le complexe $K_A^\bullet(u, M)$ associé à $u$ (A, X, p. 147). On a $K^p(x, M) = 0$ pour $p < 0$; pour $p \geq 0$ le $A$-module $K^p(x, M) = \operatorname{Hom}_A(\Lambda^p(A^{(I)}), M)$ s’identifie canoniquement au $A$-module $C_I^p(M)$ formé des applications alternées de $I^p$ dans $M$ (A, X, p. 153), la différentielle $\partial^p : K^p(x, M) \to K^{p+1}(x, M)$ étant donnée par la formule

$$
(\partial^p m)(\alpha_1, \ldots, \alpha_{p+1}) = \sum_{j=1}^{p+1} (-1)^{j+1} x_{\alpha_j} m(\alpha_1, \ldots, \alpha_{j-1}, \alpha_{j+1}, \ldots, \alpha_{p+1})
$$

pour $m \in K^p(x, M)$ et $(\alpha_1, \ldots, \alpha_{p+1}) \in I^{p+1}$ (A, X, p. 154, formule (12)). Il en résulte en particulier que le complexe $K^\bullet(x, M)$ ne dépend que de la structure de $\mathbf{Z}$-module de $M$ et des endomorphismes $(x_i)_M$.

On note $H^\bullet(x, M)$ l’homologie du complexe $K^\bullet(x, M)$. Le $A$-module $H^0(x, M)$ s’identifie à $\operatorname{Hom}_A(A/J, M)$, où $J$ est l’idéal de $A$ engendré par les $x_i$ (A, X, p. 147, lemme 1).

Soient $(M_\alpha)_{\alpha \in K}$ une famille de $A$-modules, et $M$ son produit ; le complexe $K^\bullet(x, M)$ est canoniquement isomorphe au complexe produit des $K^\bullet(x, M_\alpha)$, de sorte que pour chaque entier $s$ le $A$-module $H^s(x, M)$ s’identifie au produit des $H^s(x, M_\alpha)$ (A, X, p. 28, prop. 1).

#### Théorème 1 {#ac-x-s1-thm-1 .statement}

Soient $A$ un anneau, $J$ un idéal de $A$, $x = (x_i)_{i \in I}$ une famille génératrice de $J$, $M$ un $A$-module. La profondeur de $M$ relativement à $J$ est la borne inférieure (dans $\mathbf{N} \cup \{+\infty\}$) des entiers $n$ tels que $H^n(x, M) \neq 0$.

Posons $p = \operatorname{prof}_A(J; M)$. Considérons le complexe $K^\bullet(x, M)$. Son homologie est annulée par $J$ (A, X, p. 148, cor. 2), et la profondeur relativement à $J$ de chacun des modules $K^i(x, M)$ est égale à $p$ ou à $+\infty$ (n° 1, remarque 4). Il résulte alors du cor. 1 du n° 2 que l’on a $H^i(x, M) = 0$ pour $i < p$. Il reste à prouver que $H^p(x, M)$ n’est pas nul lorsque $p < +\infty$.

Le cas $p = 0$ étant évident, supposons $0 < p < +\infty$ et $H^p(x, M) = 0$. Soit $L$ une résolution libre du $A$-module $A/J$; notons $C$ le complexe $\operatorname{Homgr}_A(L, M)$. Le $A$-module $H^i(C)$ est isomorphe à $\operatorname{Ext}_A^i(A/J, M)$ (A, X, p. 100, th. 1); il est donc nul pour $i < p$. On a alors pour $i < p$ des suites exactes canoniques

$$
0 \to B^i(C) \to C^i \to B^{i+1}(C) \to 0 .
$$

Le A-module $C^i$ est produit de A-modules isomorphes à M ; on a donc $H^s(x, C^i) = 0$ pour $s \leq p$. On déduit des suites exactes précédentes et de A, X, p. 150 que l’homomorphisme de liaison $\partial^s : H^s(x, B^{i+1}(C)) \longrightarrow H^{s+1}(x, B^i(C))$ est injectif pour $s \leq p$ et $i < p$; comme $B^0(C) = 0$, il en résulte que $H^{p-i}(x, B^{i+1}(C))$ est nul pour $i < p$. On a en particulier $H^1(x, B^p(C)) = 0$, de sorte que la suite exacte

$$
0 \to B^p(C) \to Z^p(C) \to H^p(C) \to 0
$$

fournit une surjection $H^0(x, Z^p(C)) \longrightarrow H^0(x, H^p(C))$. Comme $H^p(C)$ est isomorphe à $\operatorname{Ext}_A^p(A/J, M)$, qui est non nul et annulé par J, on a $H^0(x, H^p(C)) \neq 0$, d’où $H^0(x, Z^p(C)) \neq 0$ et par suite $H^0(x, C^p) \neq 0$. Mais cela implique $H^0(x, M) \neq 0$, contrairement à l’hypothèse. On a donc $H^p(x, M) \neq 0$, ce qui achève la démonstration.

#### Corollaire 1 {#ac-x-s1-thm-1-cor-1 .statement}

*Supposons l’idéal J de type fini et JM $\neq$ M. Alors* $\operatorname{prof}_A(J; M)$ *est finie et $\leq$ Card(I)* ; *pour qu’elle soit égale à Card(I), il faut et il suffit que la famille x soit complètement sécante pour M* (A, X, p. 157, déf. 2).

Supposons d’abord I fini, et notons r son cardinal. Le A-module $H^r(x, M)$ est canoniquement isomorphe à $H_0(x, M)$, lui-même isomorphe à $M/JM$ (A, X, p. 155) ; l’inégalité $\operatorname{prof}_A(J; M) \leq r$ résulte donc du th. 1. Pour qu’on ait égalité, il faut et il suffit que le A-module $H^i(x, M)$ soit nul pour $i < r$, ce qui signifie que la famille x est complètement sécante pour M (A, X, p. 157).

D’après ce qui précède, $\operatorname{prof}_A(J; M)$ est finie ; il reste à démontrer que si la famille x est complètement sécante pour M, l’ensemble I est fini. Or la condition $H_1(x, M) = 0$ (A, X, p. 157, déf. 2) implique qu’on a une suite exacte

$$
\Lambda^2(A^{(I)}) \otimes_A M \xrightarrow{\partial_2} M^{(I)} \xrightarrow{\partial_1} JM \to 0 ,
$$

où l’image de $\partial_2$ est contenue dans $JM^{(I)}$. Par produit tensoriel avec $A/J$, on en déduit un isomorphisme A-linéaire de $(M/JM)^{(I)}$ sur $JM/J^2M$. Or ce dernier module est de type fini, puisque J et M le sont ; comme $M/JM$ n’est pas nul, il en résulte que l’ensemble I est fini.

#### Corollaire 2 {#ac-x-s1-thm-1-cor-2 .statement}

*Soient A un anneau local, J un idéal de type fini de A distinct de A, M un A-module non nul de type fini. Posons* $r = [J/m_AJ : \kappa_A]$. *On a* $\operatorname{prof}_A(J; M) \leq r$ ; *il y a égalité si et seulement si J est engendré par une famille complètement sécante pour M. Dans ce cas, pour qu’une famille génératrice de J soit complètement sécante, il faut et il suffit qu’elle ait r éléments*.

D’après le lemme de Nakayama, on a $JM \neq M$, et r est le nombre minimal de générateurs de J ; le cor. 2 résulte donc du cor. 1.

#### Proposition 4 {#ac-x-s1-prop-4 .statement}

Soient $\rho : A \to B$ un homomorphisme d’anneaux, $J$ un idéal de $A$ et $N$ un $B$-module. On a l’égalité $\operatorname{prof}_A(J; N) = \operatorname{prof}_B(JB; N)$.

Soit $x = (x_i)_{i \in I}$ une famille génératrice de $J$; la famille $\rho(x) = (\rho(x_i))_{i \in I}$ engendre $JB$. Par construction le complexe $K^\bullet(\rho(x), N)$ est égal à $K^\bullet(x, N)$. La proposition résulte donc du th. 1.

#### Corollaire {#ac-x-s1-n3-cor-1 .statement}

Soient $A$ un anneau local, $a$ un idéal de $A$ distinct de $A$ et $M$ un $A$-module annulé par $a$. On a $\operatorname{prof}_A(M) = \operatorname{prof}_{A/a}(M)$.

Soient $\rho : A \to B$ un homomorphisme d’anneaux, $x = (x_i)_{i \in I}$ une famille finie d’éléments de $A$ et $M$ un $A$-module. Pour tout entier $p$, notons $u^p : B \otimes_A C_I^p(M) \to C_I^p(B \otimes_A M)$ l’homomorphisme $B$-linéaire qui associe à $b \otimes m$ l’application alternée $(\alpha_1, \ldots, \alpha_p) \mapsto b \otimes m(\alpha_1, \ldots, \alpha_p)$. La famille $(u^p)$ définit un isomorphisme de complexes

$$
u : B \otimes_A K^\bullet(x, M) \to K^\bullet(x, B \otimes_A M)
$$

Considérons l’homomorphisme canonique

$$
\gamma^p(B, K^\bullet(x, M)) : B \otimes_A H^p(x, M) \to H^p(B \otimes_A K^\bullet(x, M))
$$

(A, X, p. 62); par composition avec $H^p(u)$, on en déduit un homomorphisme

$$
v^p : B \otimes_A H^p(x, M) \to H^p(x, B \otimes_A M)
$$

#### Lemme 1 {#ac-x-s1-lem-1 .statement}

Si le $A$-module $B$ est plat, l’homomorphisme $v^p$ est bijectif pour tout entier $p$.

Cela résulte de A, X, p. 66, cor. 2.

#### Proposition 5 {#ac-x-s1-prop-5 .statement}

Soient $A$ un anneau, $J$ un idéal de type fini de $A$ et $M$ un $A$-module. Notons $\Omega$ l’ensemble des idéaux maximaux de $A$ appartenant à $\operatorname{Supp}(M)$ et contenant $J$. On a

$$
\operatorname{prof}_A(J; M) = \inf_{p \in \operatorname{Spec}(A)} \operatorname{prof}_{A_p}(J_p; M_p) = \inf_{m \in \Omega} \operatorname{prof}_{A_m}(J_m; M_m)
$$

Soit $x = (x_i)_{i \in I}$ une famille génératrice finie de $J$. Soit $p$ un idéal premier de $A$; l’idéal $J_p$ est engendré par l’image $x_p$ de la famille $(x_i)$ dans $A_p$. Pour tout $p \geq 0$, le $A_p$-module $(H^p(x, M))_p$ est isomorphe à $H^p(x_p, M_p)$ (lemme 1); d’après le th. 1, on a donc $\operatorname{prof}_A(J; M) \leq \inf_{p \in \operatorname{Spec}(A)} \operatorname{prof}_{A_p}(J_p; M_p) \leq \inf_{m \in \Omega} \operatorname{prof}_{A_m}(J_m; M_m)$.

Soit $p$ un entier strictement inférieur à $\operatorname{prof}_{A_m}(JA_m; M_m)$ pour tout $m \in \Omega$. On a alors $H^p(x_m, M_m) = 0$ pour tout idéal maximal $m$ de $A$: cela résulte du th. 1 si $m \in \Omega$, du fait que $M_m = 0$ si $m \not\in \operatorname{Supp}(M)$, et du fait que l’idéal $JA_m$, qui annule $H^p(x_m, M_m)$ (A, X, p. 148, cor. 2), est égal à $A_m$ si $m \not\in V(J)$. On a donc $(H^p(x, M))_m = 0$ pour tout idéal maximal $m$ de $A$, ce qui entraîne $H^p(x, M) = 0$ (II, § 3, n° 3, cor. 2 du th. 1). La proposition résulte alors du th. 1.

#### Proposition 6 {#ac-x-s1-prop-6 .statement}

Soient $A$ un anneau, $J$ un idéal de type fini de $A$ et $M$ un $A$-module. Soient $B$ un anneau et $\rho : A \to B$ un homomorphisme d’anneaux faisant de $B$ un $A$-module plat.

a) On a $\operatorname{prof}_A(J; M) \leq \operatorname{prof}_B(JB; B \otimes_A M)$.

b) Supposons de plus que tout idéal maximal de $\operatorname{Supp}(M)$ contenant $J$ appartienne à l’image de l’application canonique $\operatorname{Spec}(B) \to \operatorname{Spec}(A)$. On a alors $\operatorname{prof}_A(J; M) = \operatorname{prof}_B(JB; B \otimes_A M)$. C’est le cas par exemple si le $A$-module $B$ est fidèlement plat.

L’assertion a) résulte du th. 1 et du lemme 1.

Soit $p$ un entier strictement inférieur à $\operatorname{prof}_B(JB; B \otimes_A M)$, et soit $m$ un idéal maximal de $A$ appartenant à $\operatorname{Supp}(M) \cap V(J)$. Soit $x$ une famille génératrice finie de l’idéal $J$. Sous l’hypothèse de b), il existe un idéal premier $n$ de $B$ au-dessus de $m$, et l’on a un isomorphisme canonique

$$
B_n \otimes_{A_m} (A_m \otimes_A H^p(x, M)) \longrightarrow B_n \otimes_B (B \otimes_A H^p(x, M))
$$

Or $B \otimes_A H^p(x, M)$ est isomorphe à $H^p(\rho(x), B \otimes_A M)$ (lemme 1), donc est nul ; de plus $B_n$ est fidèlement plat sur $A_m$ (I, § 3, n° 5, prop. 9 et II, § 3, n° 4, prop. 14 et remarque). On a donc $A_m \otimes_A H^p(x, M) = 0$ et par suite $p < \operatorname{prof}_{A_m}(J_m; M_m)$ (lemme 1 et th. 1). La première assertion de b) résulte alors de la prop. 5 ; la seconde résulte de I, § 3, n° 5, prop. 9).

#### Corollaire {#ac-x-s1-n3-cor-2 .statement}

Soient $A$ un anneau noethérien, $J$ un idéal de $A$, $M$ un $A$-module de type fini, $\widehat{A}$ et $\widehat{M}$ les séparés complétés de $A$ et $M$ pour la topologie $J$-adique. On a alors $\operatorname{prof}_A(J; M) = \operatorname{prof}_{\widehat{A}}(J\widehat{A}; \widehat{M})$.

En effet, le $A$-module $\widehat{A}$ est plat et le $\widehat{A}$-module $\widehat{M}$ est isomorphe à $\widehat{A} \otimes_A M$ (III, § 3, n° 4, th. 3) ; par ailleurs, tout idéal maximal de $A$ contenant $J$ appartient à l’image de l’application $\operatorname{Spec}(\widehat{A}) \to \operatorname{Spec}(A)$ (*loc. cit.*, prop. 8).

### 4. Profondeur et suites régulières

Soient $A$ un anneau, $M$ un $A$-module. Rappelons (A, X, p. 158) qu’une suite finie $(x_1, \ldots, x_r)$ d’éléments de $A$ est dite *régulière pour $M$* ou *$M$*-régulière si, pour $i = 1, \ldots, r$, l’homothétie de rapport $x_i$ dans le $A$-module $M/(x_1 M + \ldots + x_{i-1} M)$ est injective. Soit $(x_1, \ldots, x_r)$ une suite $M$-régulière ; pour tout $A$-module plat $N$, la suite $(x_1, \ldots, x_r)$ est $M \otimes_A N$ régulière. Si $\rho : A \to B$ est un homomorphisme d’anneaux faisant de $B$ un $A$-module plat, la suite $(\rho(x_1), \ldots, \rho(x_r))$ est régulière pour le $B$-module $B \otimes_A M$. En particulier, pour tout idéal premier $p$ de $A$, l’image dans $A_p$ de la suite $(x_1, \ldots, x_r)$ est $M_p$-régulière.

Dans la suite nous considérerons surtout la notion de suite $M$-régulière dans le cas où l’anneau $A$ est local noethérien, le module $M$ est de type fini et les éléments de la suite appartiennent à $m_A$ ; la notion de suite $M$-régulière coïncide alors avec celle de suite complètement sécante pour $M$ (A, X, p. 160, cor. 1).

#### Proposition 7 {#ac-x-s1-prop-7 .statement}

Soient $A$ un anneau, $J$ un idéal de $A$, $M$ un $A$-module, et $(x_1, \ldots, x_r)$ une suite $M$-régulière d’éléments de $J$. On a
$$
\operatorname{prof}_A(J; M) = r + \operatorname{prof}_A(J; M/(x_1M + \ldots + x_rM))
$$
et en particulier $\operatorname{prof}_A(J; M) \geqslant r$.

Le cas $r = 1$ résulte de la remarque 5 du n° 1, appliquée à la suite exacte
$$
0 \to M \xrightarrow{(x_1)_M} M \longrightarrow M/x_1M \to 0 .
$$
Le cas général s’en déduit par récurrence sur $r$.

#### Théorème 2 {#ac-x-s1-thm-2 .statement}

Soient $A$ un anneau noethérien, $J$ un idéal de $A$ et $M$ un $A$-module de type fini.

a) Supposons que $\operatorname{prof}_A(J; M)$ soit finie. Alors toute suite $M$-régulière d’éléments de $J$ peut être complétée en une suite $M$-régulière de longueur $\operatorname{prof}_A(J; M)$ d’éléments de $J$.

b) La profondeur de $M$ relativement à $J$ est la borne supérieure des longueurs des suites $M$-régulières formées d’éléments de $J$.

c) Pour que $\operatorname{prof}_A(J; M)$ soit finie, il faut et il suffit que le support de $M$ rencontre $V(J)$, ou encore que l’on ait $JM \neq M$.

Soit $(x_1, \ldots, x_r)$ une suite $M$-régulière d’éléments de $J$. On a $r \leqslant \operatorname{prof}_A(J; M)$ (prop. 7) ; supposons que l’inégalité soit stricte. Notons $N$ le $A$-module $M/(x_1M + \ldots + x_rM)$. On a $\operatorname{prof}_A(J; N) > 0$ (*loc. cit.*), de sorte qu’il existe un élément $x$ de $J$ tel que l’homothétie $x_N$ soit injective (n° 1, remarque 2), c’est-à-dire que la suite $(x_1, \ldots, x_r, x)$ soit $M$-régulière. Il en résulte par récurrence que pour tout entier $s$ tel que $r \leqslant s \leqslant \operatorname{prof}_A(J; M)$ la suite $(x_1, \ldots, x_r)$ peut être complétée en une suite $M$-régulière de longueur $s$, ce qui entraîne les assertions a) et b). L’assertion c) résulte de la remarque 1 du n° 1 et du cor. 1 du th. 1 du n° 3.

#### Corollaire 1 {#ac-x-s1-thm-2-cor-1 .statement}

Pour toute suite $M$-régulière $(x_1, \ldots, x_r)$ d’éléments de $J$, les propriétés suivantes sont équivalentes :

(i) on a $r = \operatorname{prof}_A(J; M)$ ;
(ii) la suite $(x_1, \ldots, x_r)$ est maximale parmi les suites $M$-régulières formées d’éléments de $J$ ;
(iii) le $A$-module $M/(x_1M + \ldots + x_rM)$ possède un élément non nul annulé par $J$ ;
(iv) on a $\operatorname{Ass}(M/(x_1M + \ldots + x_rM)) \cap V(J) \neq \varnothing$.

L’équivalence de (i) et (ii) résulte du th. 2 ; l’équivalence de (ii), (iii) et (iv) résulte de la remarque 2 du n° 1 appliquée au $A$-module $M/(x_1M + \ldots + x_rM)$.

#### Corollaire 2 {#ac-x-s1-thm-2-cor-2 .statement}

Soient $A$ un anneau local noethérien, $M$ un $A$-module non nul de type fini. On a
$$
\operatorname{prof}_A(M) \leqslant \dim_A(M) < +\infty .
$$

### 5. Profondeur le long d’une partie fermée

Soient A un anneau noethérien, F une partie fermée de $\mathrm{Spec}(A)$ et M un A-module. D’après le cor. 2 de la prop. 2 du n° 1, l’élément $\mathrm{prof}_A(J;M)$ de $\mathbf{N} \cup \{+\infty\}$ ne dépend pas de l’idéal J de A tel que $F = V(J)$ ; on l’appelle *profondeur de M le long de F* et on le note $\mathrm{prof}_F(M)$.

#### Remarque 1 {#ac-x-s1-n5-rem-1 .statement}

Soit r un entier. D’après la prop. 2 du n° 1 et II, § 4, n° 4, cor. 2 de la prop. 17, l’inégalité $\mathrm{prof}_F(M) \geqslant r$ équivaut à la propriété suivante : pour tout A-module N de type fini et de support contenu dans F, on a $\mathrm{Ext}_A^i(N,M) = 0$ pour $i < r$.

#### Remarque 2 {#ac-x-s1-n5-rem-2 .statement}

Supposons que le A-module M soit de type fini. D’après la remarque 2 du n° 1 et le th. 2 du n° 4, on a les équivalences suivantes

$$
\mathrm{prof}_F(M) = 0 \iff \mathrm{Ass}(M) \cap F \neq \varnothing \\
\mathrm{prof}_F(M) < +\infty \iff \mathrm{Supp}(M) \cap F \neq \varnothing .
$$

#### Proposition 8 {#ac-x-s1-prop-8 .statement}

*Soient A un anneau noethérien, F une partie fermée de $\mathrm{Spec}(A)$, et M un A-module de type fini. On a*

$$
\mathrm{prof}_F(M) = \inf_{p \in F} \mathrm{prof}_{A_p}(M_p) = \inf_{p \in \mathrm{Supp}(M) \cap F} \mathrm{prof}_{A_p}(M_p) .
$$

Cela est clair si $\mathrm{prof}_F(M) = +\infty$ (remarque 2). Si $\mathrm{prof}_F(M) = 0$, il existe un idéal premier $p \in \mathrm{Ass}(M) \cap F$ (remarque 2) ; on a $pA_p \in \mathrm{Ass}(M_p)$ (IV, § 1, n° 2, prop. 5), donc $\mathrm{prof}_{A_p}(M_p) = 0$ (remarque 2 du n° 1), d’où la proposition en ce cas.

Supposons $0 < \mathrm{prof}_F(M) < +\infty$ ; soit J un idéal de A tel que $V(J) = F$, et soit x un élément de J tel que l’homothétie $x_M$ soit injective (*loc. cit.*). Pour chaque idéal premier p, l’homothétique $x_{M_p}$ est injective. D’après la prop. 7 du n° 4, on a donc

$$
\mathrm{prof}_F(M/xM) = \mathrm{prof}_F(M) - 1 \\
\mathrm{prof}_{A_p}((M/xM)_p) = \mathrm{prof}_{A_p}(M_p) - 1 .
$$

On conclut alors par récurrence sur l’entier $\mathrm{prof}_F(M)$.

#### Remarque 3 {#ac-x-s1-n5-rem-3 .statement}

Si q est un point de $\mathrm{Supp}(M)$, on a donc $\mathrm{prof}_A(q;M) = \inf_{p \supseteq q} \mathrm{prof}_{A_p}(M_p)$. On a en particulier l’inégalité $\mathrm{prof}_A(q;M) \leqslant \mathrm{prof}_{A_q}(M_q)$ ; il y a égalité lorsque q est maximal. Dans le cas général, on peut avoir $\mathrm{prof}_A(q;M) < \mathrm{prof}_{A_q}(M_q)$ ; on peut également avoir $\mathrm{prof}_A(q;M) < \inf \mathrm{prof}_{A_m}(M_m)$ où m parcourt l’ensemble des idéaux maximaux de A contenant q. Soit par exemple p un idéal premier non maximal de A, contenant q et distinct de q ; posons $M = A/p$. On a $\mathrm{prof}_A(q;M) = 0$, $\mathrm{prof}_{A_q}(M_q) = +\infty$ et $\mathrm{prof}_{A_m}(M_m) > 0$ pour tout idéal maximal m de A.

#### Proposition 9 {#ac-x-s1-prop-9 .statement}

Soient $A$ un anneau noethérien, $M$ et $N$ deux $A$-modules de type fini et $F$ le support de $N$. Alors $\mathrm{prof}_F(M)$ est la borne inférieure (dans $N \cup \{+\infty\}$) de l’ensemble des entiers $n$ tels que $\mathrm{Ext}_A^n(N, M) \neq 0$.

D’après la remarque 1, on a $\mathrm{Ext}_A^i(N, M) = 0$ pour tout $i < \mathrm{prof}_F(M)$. Il reste à prouver que si $\mathrm{prof}_F(M) = n < +\infty$, on a $\mathrm{Ext}_A^n(N, M) \neq 0$. Soit $J$ l’annulateur de $N$; on a $F = V(J)$, donc $\mathrm{prof}_F(M) = \mathrm{prof}_A(J; M)$. D’après le cor. 1 du th. 2 (n° 4), il existe une suite $M$-régulière $(x_1, \ldots, x_n)$ de longueur $n$ formée d’éléments de $J$, et la profondeur relativement à $J$ du $A$-module $\overline{M} = M/(x_1 M + \ldots + x_n M)$ est nulle. D’après A, X, p. 166, prop. 9, il suffit de prouver que $\mathrm{Hom}_A(N, \overline{M})$ est non nul. Or, d’après la prop. 8, il existe $p \in \mathrm{Supp}(M) \cap \mathrm{Supp}(N)$ tel que $\mathrm{prof}_{A_p}(\overline{M}_p) = 0$, c’est-à-dire $\mathrm{Hom}_{A_p}(\kappa(p), \overline{M}_p) \neq 0$. Puisque $N_p$ est non nul, le $\kappa(p)$-espace vectoriel $N_p \otimes_{A_p} \kappa(p)$ est non nul (lemme de Nakayama), ainsi que son dual ; il existe donc une application $A_p$-linéaire surjective de $N_p$ dans $\kappa(p)$. Il en résulte qu’on a $\mathrm{Hom}_{A_p}(N_p, \overline{M}_p) \neq 0$, donc $\mathrm{Hom}_A(N, \overline{M}) \neq 0$ (II, § 2, n° 7, prop. 19), ce qu’on voulait démontrer.

#### Remarque 4 {#ac-x-s1-n5-rem-4 .statement}

Soient $A$ un anneau noethérien, $N$ un $A$-module de type fini. On appelle parfois grade de $N$, et on note grade$(N)$, la borne inférieure dans $N \cup \{+\infty\}$ de l’ensemble des entiers $n$ tels que $\mathrm{Ext}_A^n(N, A)$ soit non nul. D’après la prop. 9, c’est aussi la profondeur de $A$ le long du support de $N$, ou encore (n° 4, th. 2) la borne supérieure de l’ensemble des longueurs de suites $A$-régulières d’éléments de l’annulateur de $N$. Comme pour tout idéal premier $p$ de $A$ l’annulateur de $N_p$ est égal à $\mathrm{Ann}(N)_p$ (II, § 2, n° 4, formule (9)), on déduit de la prop. 5 du n° 3 l’égalité

$$
\mathrm{grade}(N) = \inf_{p \in \mathrm{Spec}(A)} \mathrm{grade}(N_p) = \inf_{m \in \Omega} \mathrm{grade}(N_m),
$$

où $\Omega$ désigne l’ensemble des idéaux maximaux de $A$.

### 6. Profondeur des algèbres

#### Lemme 2 {#ac-x-s1-lem-2 .statement}

Soient $\rho : A \to B$ un homomorphisme local d’anneaux locaux noethériens, $N$ un $B$-module de type fini et $y$ un élément de $m_B$. Les deux conditions suivantes sont équivalentes :

(i) le $A$-module $N/yN$ est plat et l’homothétie $y_N$ est injective ;
(ii) le $A$-module $N$ est plat et l’homothétie $y_{\kappa_A \otimes N}$ est injective.

Lorsqu’elles sont satisfaites, l’homothétie $y_{M \otimes_A N}$ est injective pour tout $A$-module $M$.

Supposons les hypothèses de (i) satisfaites, et prouvons (ii) ainsi que la dernière assertion. Soit $M$ un $A$-module. Puisque le $A$-module $N/yN$ est plat, on déduit de la suite exacte $0 \to N \xrightarrow{y_N} N \to N/yN \to 0$ des suites exactes

$$
0 \to M \otimes_A N \xrightarrow{u} M \otimes_A N \to M \otimes_A (N/yN) \to 0
$$
$$
0 \to \mathrm{Tor}_1^A(M, N) \xrightarrow{v} \mathrm{Tor}_1^A(M, N) \to 0
$$

où $u = 1_M \otimes y_N$ et $v = \mathrm{Tor}_1^A(1_M, y_N)$; il en résulte que l’homothétie de rapport $y$ est injective dans $M \otimes_A N$, et bijective dans $\mathrm{Tor}_1^A(M, N)$. Supposons de plus le A-module $M$ de type fini ; alors le B-module $\mathrm{Tor}_1^A(M, N)$ est de type fini (A, X, p. 107, prop. 6), donc est nul puisque $y$ appartient à $m_B$ (lemme de Nakayama), ce qui entraîne que le A-module $N$ est plat (A, X, p. 74, th. 2).

(ii) $\Rightarrow$ (i) : supposons les hypothèses de (ii) satisfaites. Considérons les deux suites exactes de B-modules

(1)
$$
0 \to \mathrm{Ker}(y_N) \longrightarrow N \xrightarrow{p} \mathrm{Im}(y_N) \to 0
$$

(2)
$$
0 \to \mathrm{Im}(y_N) \xrightarrow{i} N \longrightarrow N/yN \to 0,
$$

où $p$ et $i$ sont les homomorphismes canoniques. On en déduit que l’homomorphisme $1 \otimes p : \kappa_A \otimes_A N \longrightarrow \kappa_A \otimes_A \mathrm{Im}(y_N)$ est surjectif, et (puisque $N$ est plat) que le noyau de l’homomorphisme $1 \otimes i : \kappa_A \otimes_A \mathrm{Im}(y_N) \longrightarrow \kappa_A \otimes_A N$ est isomorphe à $\mathrm{Tor}_1^A(\kappa_A, N/yN)$. Mais l’application $(1 \otimes i) \circ (1 \otimes p)$, égale à $y_{\kappa_A \otimes_A N}$, est injective par hypothèse ; on en déduit que $1 \otimes p$ est bijective et $1 \otimes i$ injective, et par suite qu’on a $\mathrm{Tor}_1^A(\kappa_A, N/yN) = 0$. Il en résulte que le A-module $N/yN$ est plat (III, § 5, n° 2, th. 1 et n° 4, prop. 2).

Puisque $N$ et $N/yN$ sont plats sur $A$, il en est de même de $\mathrm{Im}(y_N)$ (suite exacte (2)). On déduit alors de la suite exacte (1) que $\kappa_A \otimes_A \mathrm{Ker}(y_N)$ est isomorphe au noyau de $1 \otimes p$, donc est nul ; ainsi l’homothétie $y_N$ est injective par le lemme de Nakayama.

#### Proposition 10 {#ac-x-s1-prop-10 .statement}

*Soient $\rho : \Lambda \to B$ un homomorphisme local d’anneaux locaux noethériens, $N$ un B-module de type fini et $y = (y_1, \ldots, y_s)$ une suite d’éléments de $m_B$. Notons $\mathfrak{y}$ l’idéal de $B$ engendré par cette suite. Les conditions suivantes sont équivalentes :

(i) le A-module $N/\mathfrak{y}N$ est plat et la suite $y$ est N-régulière ;
(ii) le A-module $N$ est plat et la suite $y$ est $(\kappa_A \otimes_A N)$-régulière.*

Lorsqu’elles sont satisfaites, pour tout A-module $M$, la suite $y$ est $M \otimes_A N$-régulière.

Prouvons l’équivalence de (i) et (ii) par récurrence sur $s$. Le cas $s = 0$ étant évident, supposons $s \geqslant 1$ ; notons $y'$ la suite $(y_1, \ldots, y_{s-1})$ et $\mathfrak{y}'$ l’idéal de $B$ qu’elle engendre. D’après le lemme 2 appliqué au B-module $N/\mathfrak{y}'N$ et à l’élément $y_s$ de $B$, la condition (i) équivaut à

(i') le A-module $N/\mathfrak{y}'N$ est plat, la suite $y'$ est N-régulière et l’homothétie de rapport $y_s$ dans $\kappa_A \otimes_A (N/\mathfrak{y}'N) = (\kappa_A \otimes_A N)/\mathfrak{y}'(\kappa_A \otimes_A N)$ est injective.

Cette condition équivaut à (ii) d’après l’hypothèse de récurrence.

La dernière assertion résulte de même par récurrence sur $s$ de la dernière assertion du lemme 2.

#### Proposition 11 {#ac-x-s1-prop-11 .statement}

*Soient $\rho : \Lambda \to B$ un homomorphisme local d’anneaux locaux noethériens, $M$ un A-module de type fini et $N$ un B-module de type fini ; on suppose que le A-module $N$ est plat.*

a) Soient $(x_1, \ldots, x_r)$ une suite d’éléments de $m_A$ régulière pour le A-module $M$, et $(y_1, \ldots, y_s)$ une suite d’éléments de $m_B$ régulière pour le B-module $\kappa_A \otimes_A N$; alors la suite $(y_1, \ldots, y_s, \rho(x_1), \ldots, \rho(x_r))$ d’éléments de $m_B$ est régulière pour le B-module $M \otimes_A N$.

b) On a l’égalité

$$
\operatorname{prof}_B(M \otimes_A N) = \operatorname{prof}_A(M) + \operatorname{prof}_B(\kappa_A \otimes_A N)
$$

Notons $x$ l’idéal de A engendré par la suite $x$ et $y$ l’idéal de B engendré par $y$. D’après la prop. 10, la suite $y$ est $M \otimes_A N$-régulière et $N/yN$ est plat sur A, de sorte que la suite $\rho(x) = (\rho(x_1), \ldots, \rho(x_r))$ est régulière pour $M \otimes_A (N/yN) = (M \otimes_A N)/y(M \otimes_A N)$. Cela prouve a).

Pour démontrer b), on peut supposer M et N non nuls. D’après le lemme de Nakayama, $\kappa_A \otimes_A N$ est également non nul, de sorte que $\operatorname{prof}_A(M)$ et $\operatorname{prof}_B(\kappa_A \otimes_A N)$ sont finis (n° 4, cor. 2 du th. 2). Prenons les suites régulières $x$ et $y$ maximales ; on a alors $r = \operatorname{prof}_A(M)$, $s = \operatorname{prof}_B(\kappa_A \otimes_A N)$, et il existe une application A-linéaire injective $u : \kappa_A \to M/xM$ et une application B-linéaire injective $v : \kappa_B \to \kappa_A \otimes_A (N/yN)$ (n° 4, cor. 1 du th. 2). Puisque $N/yN$ est plat sur A, l’application B-linéaire $(u \otimes 1_{N/yN}) \circ v$ de $\kappa_B$ dans $(M/xM) \otimes_A (N/yN) = (M \otimes_A N)/(\rho(x) + y)(M \otimes_A N)$ est injective. Cela implique l’égalité $\operatorname{prof}_B(M \otimes_A N) = r + s$ (*loc. cit.*).

#### Remarque {#ac-x-s1-n6-rem-1 .statement}

Rappelons qu’on a, sous les hypothèses précédentes,

$$
\dim_B(M \otimes_A N) = \dim_A(M) + \dim_B(\kappa_A \otimes_A N)
$$
(VIII, § 3, n° 4, prop. 7).

#### Corollaire {#ac-x-s1-n6-cor-1 .statement}

Soit $\rho : A \to B$ un homomorphisme local d’anneaux locaux noethériens faisant de B un A-module plat. On a

$$
\operatorname{prof}(B) = \operatorname{prof}(A) + \operatorname{prof}(\kappa_A \otimes_A B),
$$
$$
\dim(B) = \dim(A) + \dim(\kappa_A \otimes_A B).
$$

En effet la profondeur (resp. la dimension) du B-module $\kappa_A \otimes_A B$ est égale à la profondeur (resp. la dimension) de l’anneau $\kappa_A \otimes_A B$ d’après le cor. de la prop. 4 (resp. d’après VIII, § 1, n° 4).

### 7. Majorations de la profondeur

#### Proposition 12 {#ac-x-s1-prop-12 .statement}

Soient A un anneau local noethérien, M un A-module non nul de type fini et J un idéal de A distinct de A. On a la suite d’inégalités

$$
\operatorname{prof}_A(J; M) \leq \operatorname{codim}(\operatorname{Supp}(M) \cap V(J), \operatorname{Supp}(M)) \leq \dim(M) - \dim(M/JM)
$$
$$
\leq [J/m_A J : \kappa_A].
$$

Pour tout élément $p$ de $\operatorname{Supp}(M) \cap V(J)$, $\operatorname{prof}_A(J; M)$ est inférieur à $\dim_{A_p}(M_p)$ (n° 5, prop. 8 et n° 4, cor. 2 du th. 2), c’est-à-dire (VIII, § 1, n° 4, prop. 9)

#### Remarque 1 {#ac-x-s1-n7-rem-1 .statement}

Considérons la chaîne d’inégalités de la prop. 12.

a) Pour qu’on ait prof_A(J ; M) = [J/m_AJ : κ_A], il faut et il suffit que J puisse être engendré par une suite M-régulière (n° 3, cor. 2 du th. 1 et A, X, p. 160, cor. 1).

b) L’égalité dim(M) − dim(M/JM) = [J/m_AJ : κ_A] signifie que J peut être engendré par une suite sécante pour M (VIII, § 3, n° 2).

c) *Si M est macaulayen, on a prof_A(J ; M) = dim(M) − dim(M/JM) (§ 2, n° 2, cor. de la prop. 2).*

#### Lemme 3 {#ac-x-s1-lem-3 .statement}

Soient A un anneau noethérien, p ⊂ p_1 ⊂ ... ⊂ p_{r−1} ⊂ q une chaîne saturée de longueur r d’idéaux premiers de A, M un Λ-module de type fini et n un entier. Si le A-module Ext^n_{A_p}(κ(p), M_p) est non nul, il en est de même de Ext^{n+r}_{A_q}(κ(q), M_q).

Il suffit évidemment de traiter le cas r = 1 ; remplaçant alors A, M, p et q par A_q, M_q, pA_q et qA_q respectivement, on est ramené à traiter le cas où A est local et où q = m_A. Soit x un élément de m_A − p. Le A_p-module Ext^n_A(A/p, M) ⊗_A A_p est isomorphe à Ext^n_{A_p}(κ(p), M_p) (A, X, p. 111, prop. 10 b)), donc n’est pas nul par hypothèse ; a fortiori Ext^n_A(A/p, M) n’est pas nul. La suite exacte

$$
0 \to A/p \xrightarrow{x_{A/p}} A/p \to A/(p + xA) \to 0
$$

fournit une suite exacte de modules d’extensions

$$
\text{Ext}^n_A(A/p, M) \xrightarrow{u} \text{Ext}^n_A(A/p, M) \to \text{Ext}^{n+1}_A(A/(p + xA), M),
$$

où u est l’homothétie de rapport x. D’après le lemme de Nakayama, celle-ci n’est pas surjective, donc le A-module Ext^{n+1}_A(A/(p + xA), M) n’est pas nul. Mais le seul idéal premier de A contenant p + xA est m_A, donc le A-module A/(p + xA) est de longueur finie (VIII, § 3, n° 2, lemme 2). Si Ext^{n+1}_A(κ_A, M) était nul, on en déduirait, par récurrence sur la longueur de N, la nullité de Ext^{n+1}_A(N, M) pour tout A-module N de longueur finie. Cette contradiction achève la démonstration.

#### Proposition 13 {#ac-x-s1-prop-13 .statement}

Soient A un anneau noethérien, M un A-module de type fini, p et q deux idéaux premiers de Supp(M) avec p ⊂ q. On a

$$
\text{prof}_{A_q}(M_q) \leq \text{prof}_{A_p}(M_p) + \dim(A_q/pA_q).
$$

Plus précisément, pour toute chaîne saturée d’idéaux premiers p ⊂ p_1 ⊂ ... ⊂ p_{r−1} ⊂ q, on a \text{prof}_{A_q}(M_q) \leq \text{prof}_{A_p}(M_p) + r.

Posons p = \text{prof}_{A_p}(M_p), et prouvons la seconde inégalité. Elle est évidente si p = +∞ ; dans le cas contraire on a \text{Ext}^p_{A_p}(κ(p), M_p) ≠ 0, d’où

$Ext_{A_q}^{p+r}(\kappa(q), M_q) \neq 0$ d'après le lemme 3, ce qui entraîne $prof_{A_q}(M_q) \leq p + r$. Comme $\dim(A_q/pA_q)$ est la borne supérieure des longueurs des chaînes saturées d'idéaux premiers d'extrémités $p$ et $q$, la première assertion est une conséquence de la seconde.

#### Corollaire 1 {#ac-x-s1-prop-13-cor-1 .statement}

*On a l'inégalité*

$$
\dim(M_q) - prof_{A_q}(M_q) \geq \dim(M_p) - prof_{A_p}(M_p) \geq 0 .
$$

Cela résulte de la prop. 13 et de l'inégalité $\dim(M_q) \geq \dim(M_p) + \dim(A_q/pA_q)$ (VIII, § 1, n° 4, prop. 9, a) et n° 3, prop. 7, b)).

#### Corollaire 2 {#ac-x-s1-prop-13-cor-2 .statement}

*Soient A un anneau local noethérien et M un A-module de type fini. On a l'inégalité*

$$
prof_A(M) \leq \inf_{p \in \operatorname{Ass}(M)} \dim(A/p) .
$$

Soit $p$ un idéal premier associé à $M$; on a $prof_{A_p}(M_p) = 0$ (n° 1, remarque 2). La prop. 13 appliquée aux idéaux $p \subset m_A$ fournit l'inégalité $prof_A(M) \leq \dim(A/p)$, d'où le corollaire.

#### Remarque 2 {#ac-x-s1-n7-rem-2 .statement}

On a $\sup_{p \in \operatorname{Ass}(M)} \dim(A/p) = \dim(M)$ (VIII, § 1, n° 4, remarque 2) et on retrouve l'inégalité $prof(M) \leq \dim(M)$ pour $M \neq 0$ (n° 4, cor. 2 du th. 2).

### 8. Anneaux noethériens localement intègres ; anneaux noethériens normaux

Soit $A$ un anneau noethérien. On note $(Y_i)_{i \in I}$ la famille finie (II, § 4, n° 2, prop. 10 et n° 3, cor. 7 de la prop. 11) des composantes connexes de $\operatorname{Spec}(A)$. D'après II, § 4, n° 3, prop. 15, il existe pour chaque $i$ un unique élément idempotent $e_i$ de $A$ tel que $Y_i = V(e_i)$, et l'application canonique de $A$ dans le produit des anneaux $A/Ae_i$ est bijective. On dit que les anneaux quotients $A/Ae_i$ de $A$ sont les *composants canoniques* de $A$. Posons $f_i = 1 - e_i$. On a $\sum_{i \in I} f_i = 1$ et $(f_i)_{i \in I}$ est une famille orthogonale d'idempotents non nuls de $A$ (*loc. cit.*). Il en résulte que l'image de $f_i$ dans $A/Ae_j$ est égale à 1 si $j = i$ et à 0 si $j \neq i$; on déduit donc de l'homomorphisme d'anneaux $A \to \prod_j A/Ae_j$ un isomorphisme canonique $A_{f_i} \to A/Ae_i$.

D'après *loc. cit.*, cor. 2 de la prop. 14, les conditions suivantes sont équivalentes :
(i) les composantes connexes de $\operatorname{Spec}(A)$ sont irréductibles ;
(ii) tout idéal premier (resp. maximal) de $A$ n'appartient qu'à une seule composante irréductible de $\operatorname{Spec}(A)$ ;
(iii) tout idéal premier (resp. maximal) de $A$ ne contient qu'un seul idéal premier minimal ;
(iv) pour tout idéal premier (resp. maximal) $p$ de $A$, l'espace topologique $\operatorname{Spec}(A_p)$ est irréductible ;
(v) pour tout composant canonique $C$ de $A$, l'espace topologique $\operatorname{Spec}(C)$ est irréductible.

(i) $A$ est réduit et les composantes connexes de $\mathrm{Spec}(A)$ sont irréductibles ;
(ii) pour tout idéal premier (resp. maximal) $p$ de $A$, l’anneau $A_p$ est intègre ;
(iii) les composants canoniques de $A$ sont intègres.

On dit qu’un anneau noethérien est *localement intègre* s’il satisfait aux conditions équivalentes (i) à (iii) ci-dessus.

Supposons l’anneau $A$ localement intègre ; soit $u$ un isomorphisme de $A$ sur un produit (fini) $\prod_{j \in J} A_j$ d’anneaux intègres. Il existe une bijection $\sigma : J \to I$ telle que l’application de $\mathrm{Spec}(\prod_{j \in J} A_j)$ dans $\mathrm{Spec}(A)$ associée à $u$ définisse un homéomorphisme de $\mathrm{Spec}(A_j)$ sur la composante connexe $Y_{\sigma(j)}$ de $\mathrm{Spec}(A)$ ; on déduit alors de $u$ un isomorphisme du composant canonique $A/Ae_{\sigma(j)}$ sur $A_j$.

#### Proposition 14 {#ac-x-s1-prop-14 .statement}

*Soit $A$ un anneau noethérien. Les conditions suivantes sont équivalentes :*

(i) $A$ est réduit et intégralement fermé dans son anneau total des fractions ;
(ii) $A$ est isomorphe au produit d’une famille finie d’anneaux intégralement clos ;
(iii) *les composants canoniques de $A$ sont intégralement clos* ;
(iv) *pour tout idéal premier (resp. maximal) $p$ de $A$, l’anneau $A_p$ est intégralement clos*.

L’équivalence de (i) et (ii) résulte de V, § 1, n° 2, cor. 2 de la prop. 9, et celle de (ii) et (iii) des remarques précédant la proposition. Soit $p$ un idéal premier de $A$ ; il existe un unique composant canonique $A'$ de $A$ tel que $p$ appartienne à la partie fermée $\mathrm{Spec}(A')$ de $\mathrm{Spec}(A)$ et on a un isomorphisme canonique $A_p \to A'_pA'$. L’équivalence de (iii) et (iv) résulte donc de *loc. cit.*, n° 5, cor. 1 et cor. 3 de la prop. 16.

Un anneau $A$ est dit *normal* s’il est noethérien et qu’il satisfait aux conditions équivalentes (i) à (iv) de la proposition 14. Un anneau noethérien est intégralement clos si et seulement s’il est intègre et normal. Un anneau local normal est intégralement clos.

### 9. Profondeur et connexité

#### Lemme 4 {#ac-x-s1-lem-4 .statement}

*Soient $A$ un anneau noethérien, $F$ une partie fermée de $\mathrm{Spec}(A)$, $U$ l’ouvert complémentaire, et $u : M \to N$ un homomorphisme de $A$-modules de type fini.*

a) *Supposons que $u_p : M_p \to N_p$ soit injectif pour tout $p \in U$ et qu’on ait $\mathrm{prof}_F(M) \geqslant 1$. Alors $u$ est injectif.*

b) Supposons que $u_p : M_p \to N_p$ soit bijectif pour tout $p \in U$ et qu’on ait $\mathrm{prof}_F(M) \geqslant 2$ et $\mathrm{prof}_F(N) \geqslant 1$. Alors $u$ est bijectif.

a) Les hypothèses impliquent $\mathrm{Supp}(\mathrm{Ker}\,u) \subset F$, puis $\mathrm{Hom}_\Lambda(\mathrm{Ker}\,u, M) = 0$ (n° 5, remarque 1) ; on a donc $\mathrm{Ker}\,u = 0$.

b) On sait déjà que $u$ est injectif, et on a $\mathrm{Supp}(\mathrm{Coker}\,u) \subset F$. D’après loc. cit., on a $\mathrm{Hom}_A(\mathrm{Coker}\,u, N) = 0$ et $\mathrm{Ext}_A^1(\mathrm{Coker}\,u, M) = 0$. De la suite exacte des modules d’extensions

$$
\mathrm{Hom}_A(\mathrm{Coker}\,u, N) \to \mathrm{Hom}_A(\mathrm{Coker}\,u, \mathrm{Coker}\,u) \to \mathrm{Ext}_A^1(\mathrm{Coker}\,u, M)
$$

on tire $\mathrm{Hom}_A(\mathrm{Coker}\,u, \mathrm{Coker}\,u) = 0$, ce qui implique $\mathrm{Coker}\,u = 0$.

#### Remarque 1 {#ac-x-s1-n9-rem-1 .statement}

Soient $A$ un anneau noethérien, $F$ une partie fermée de $\mathrm{Spec}(A)$, $U$ l’ouvert complémentaire. Pour qu’on ait $\mathrm{prof}_F(A) \geqslant 1$, il faut et il suffit qu’on ait $\mathrm{Ass}(A) \subset U$ (remarque 2, n° 5). Lorsque cette condition est satisfaite, chaque composante irréductible de $\mathrm{Spec}(A)$ rencontre $U$, de sorte que $U$ est dense dans $\mathrm{Spec}(A)$.

#### Théorème 3 (Hartshorne) {#ac-x-s1-thm-3 .statement}

Soient $A$ un anneau noethérien, $F$ une partie fermée de $\mathrm{Spec}(A)$ et $U$ l’ouvert complémentaire. On suppose qu’on a $\mathrm{prof}_F(A) \geqslant 2$. Alors, pour toute composante connexe $Y$ de $\mathrm{Spec}(A)$, l’ensemble $Y \cap \overline{U}$ est connexe et dense dans $Y$.

Supposons d’abord que $\mathrm{Spec}(A)$ soit connexe. D’après la remarque 1, $U$ est dense dans $\mathrm{Spec}(A)$ et il s’agit de prouver qu’il est connexe. Raisonnons par l’absurde et supposons donnés deux ouverts disjoints $U_0$ et $U_1$ de $\mathrm{Spec}(A)$, non vides et de réunion $U$. Comme l’ensemble $\mathrm{Ass}(\Lambda)$ est contenu dans $U$ d’après la remarque 1, il est réunion disjointe de $\mathrm{Ass}(A) \cap U_0$ et $\mathrm{Ass}(A) \cap U_1$. D’après IV, § 1, n° 1, prop. 4, il existe des idéaux $J_0$ et $J_1$ de $A$ tels que $\mathrm{Ass}(J_i) = \mathrm{Ass}(A) \cap U_i$, $\mathrm{Ass}(A/J_i) = \mathrm{Ass}(A) \cap U_{1-i} \quad (i = 0, 1)$. Le complémentaire de $U_i$ dans $\mathrm{Spec}(A)$ contient $\mathrm{Ass}(A/J_i)$ et $\mathrm{Ass}(J_{1-i})$; comme il est fermé, il contient $\mathrm{Supp}(A/J_i)$ et $\mathrm{Supp}(J_{1-i})$. Pour $p \in U_i$, on a ainsi $(J_i)_p = A_p$ et $(J_{1-i})_p = 0$; cela implique notamment que $J_0$ et $J_1$ sont distincts de $A$. Soit $B$ le $A$-module $A/J_0 \times A/J_1$ et soit $u : A \to B$ l’homomorphisme canonique. D’après ce qui précède, l’homomorphisme $u_p$ est bijectif pour tout $p \in U$; par ailleurs, on a $\mathrm{Ass}(B) \subset U_0 \cup U_1 = U$, donc $\mathrm{prof}_F(B) \geqslant 1$ d’après la remarque 1. Le lemme 4 implique alors que $u$ est bijectif, ce qui contredit la connexité de $\mathrm{Spec}(A)$.

Traitons le cas général. Soit $J$ un idéal de $A$ tel que $F = V(J)$ et soit $Y$ une composante connexe de $\mathrm{Spec}(A)$. D’après II, § 4, n° 3, prop. 15, il existe un élément idempotent $f$ de $\Lambda$ tel que $Y$ s’identifie à la partie $\mathrm{Spec}(A_f)$ de $\mathrm{Spec}(A)$. Alors $Y \cap F$ s’identifie à $V(J_f)$; on a $\mathrm{prof}_{\Lambda_f}(J_f, A_f) \geqslant \mathrm{prof}_A(J; A) \geqslant 2$ d’après la prop. 6, a) du n° 3. Il résulte de la première partie de la démonstration que $Y \cap U = Y - (Y \cap F)$ est connexe et dense dans $Y$.

#### Corollaire 1 {#ac-x-s1-thm-3-cor-1 .statement}

L’application qui associe à chaque composante connexe de $U$ son adhérence dans $\mathrm{Spec}(A)$ est une bijection de l’ensemble des composantes connexes de $U$ sur l’ensemble des composantes connexes de $\mathrm{Spec}(A)$.

#### Corollaire 2 {#ac-x-s1-thm-3-cor-2 .statement}

Pour tout anneau local noethérien B de profondeur $\geq 2$, l’espace topologique $\operatorname{Spec}(B) - \{ m_B \}$ est connexe.

#### Corollaire 3 {#ac-x-s1-thm-3-cor-3 .statement}

Sous les hypothèses du théorème 3, supposons que $\operatorname{Spec}(A_p)$ soit irréductible (resp. que $A_p$ soit intègre) pour tout $p \in U$; alors $\operatorname{Spec}(A_p)$ est irréductible (resp. $A_p$ est intègre) pour tout $p \in \operatorname{Spec}(A)$.

Soit $(Y_i)_{i \in I}$ la famille (finie) des composantes irréductibles de $\operatorname{Spec}(A)$. Soit $p \in U$; comme $\operatorname{Spec}(\Lambda_p)$ est irréductible, $p$ contient un seul idéal premier minimal de $\Lambda$, donc n’appartient qu’à une seule des $Y_i$ (II, § 4, n° 3, cor. 2 de la prop. 14). Les sous-ensembles $Y_i \cap U$ sont des parties fermées de $U$, disjointes, non vides puisque $U$ est dense dans $\operatorname{Spec}(A)$, et irréductibles d’après II, § 4, n° 1, prop. 7; ce sont donc les composantes connexes de $U$. Leurs adhérences $Y_i$ sont les composantes connexes de $\operatorname{Spec}(\Lambda)$ (cor. 1). Cela prouve que les composantes connexes de $\operatorname{Spec}(A)$ sont irréductibles, donc que $\operatorname{Spec}(A_p)$ est irréductible pour tout $p$ (n° 8).

Supposons que $A_q$ soit intègre pour tout $q \in U$. Soit $p \in \operatorname{Spec}(A)$. Puisque $\operatorname{Spec}(A_p)$ est irréductible, le nilradical de $A_p$ est l’unique idéal premier minimal de $A_p$; il appartient donc à $\operatorname{Ass}(A_p)$ (IV, § 1, n° 3, cor. 1 de la prop. 7), et par suite est égal à $qA_p$, où $q$ est un idéal premier associé à $A$ (IV, § 1, n° 2, cor. de la prop. 5). On a $q \in U$ (remarque 1) et $qA_q \in \operatorname{Ass}(A_q)$ (loc. cit.); puisque $A_q$ est intègre, $q$ est nul, donc $A_p$ est intègre.

#### Corollaire 4 {#ac-x-s1-thm-3-cor-4 .statement}

Soit $\Lambda$ un anneau noethérien dont le spectre est connexe. Supposons qu’il existe un entier $d \geq 1$ tel qu’on ait $\operatorname{prof}(\Lambda_p) \geq 2$ pour tout idéal premier $p$ de $A$ de hauteur $> d$.

a) Pour toute partie fermée $Z$ de $\operatorname{Spec}(A)$ de codimension $> d$, l’espace $\operatorname{Spec}(A) - Z$ est connexe.

b) Soient $Y$ et $Y'$ des composantes irréductibles de $\operatorname{Spec}(A)$. Il existe une suite $X_1, X_2, \ldots, X_n$ de composantes irréductibles de $\operatorname{Spec}(A)$ telle que l’on ait $X_1 = Y$, $X_n = Y'$ et, pour $i = 1, \ldots, n-1$

$$
\operatorname{codim}(X_i \cap X_{i+1}, \operatorname{Spec}(A)) \leq d .
$$

Soit $Z \subset \operatorname{Spec}(A)$ une partie fermée de codimension $> d$. Pour tout $p \in Z$, on a $\dim(A_p) > d$, donc $\operatorname{prof}(A_p) \geq 2$, ce qui implique que $\operatorname{prof}_Z(A)$ est $\geq 2$ (n° 5, prop. 8) et donc que $\operatorname{Spec}(A) - Z$ est connexe (th. 3).

Prouvons b). Désignons par $Z$ la réunion des ensembles $X' \cap X''$ où $(X', X'')$ parcourt l’ensemble (fini) des couples de composantes irréductibles de $\operatorname{Spec}(A)$ tels que $\operatorname{codim}(X' \cap X'', \operatorname{Spec}(A)) > d$. D’après a), l’ensemble $\operatorname{Spec}(A) - Z$ est connexe. Toutes les composantes irréductibles de $\operatorname{Spec}(A)$ rencontrent $\operatorname{Spec}(A) - Z$; leurs traces sur $\operatorname{Spec}(A) - Z$ sont les composantes irréductibles de $\operatorname{Spec}(A) - Z$ (II, § 4, n° 1, prop. 7). Puisque $\operatorname{Spec}(A) - Z$ est connexe, il existe une suite $X_1, \ldots, X_n$ de composantes irréductibles de $\operatorname{Spec}(A)$ telles que l’on ait $X_1 - Z = Y - Z$, $X_n - Z = Y' - Z$ et $(X_i - Z) \cap (X_{i+1} - Z) \neq \varnothing$ pour $1 \leq i \leq n-1$; autrement dit on a $X_1 = Y$, $X_n = Z$ et $\operatorname{codim}(X_i \cap X_{i+1}) \leq d$.

#### Remarque 2 {#ac-x-s1-n9-rem-2 .statement}

*Lorsque A est un anneau de Macaulay, on peut appliquer le corollaire avec $d = 1$ (§ 2, n° 5).*

#### Exemple (Intersection complète formée par quatre plans de coordonnées d’un espace affine de dimension 4) {#ac-x-s1-n9-exa-1 .statement}

Soit $k$ un corps. Notons S l’anneau de polynômes $k[T_1, T_2, T_3, T_4]$. Rappelons (VIII, § 2, n° 4, th. 3) que toute chaîne maximale d’idéaux premiers de S est de longueur 4. Notons m l’idéal de S engendré par les $T_i$, a l’idéal engendré par $T_1T_2$ et $T_3T_4$, et $p_{ij}$, pour $1 \leq i < j \leq 4$, l’idéal engendré par $T_i$ et $T_j$. Les idéaux $p_{ij}$ sont premiers de hauteur 2, leur somme est l’idéal maximal m et l’on a $a = p_{13} \cap p_{14} \cap p_{23} \cap p_{24}$.

a) L’anneau $A = S/a$ est réduit ; les composantes irréductibles de Spec(A) sont les ensembles $X_{ij} = V(p_{ij}/a)$ pour $i = 1,2,\ j = 3,4$, qui sont de dimension 2 et contiennent tous le point $m/a$. En particulier, Spec(A) est connexe et de dimension 2. L’intersection de deux composantes distinctes $X_{ij}$ et $X_{kl}$ est réduite à $\{m/a\}$ si $\{i,j\} \cap \{k,l\} = \varnothing$, de dimension 1 sinon. Il en résulte que la conclusion du cor. 4 est satisfaite avec $d = 1$ (nous verrons plus loin que A est un anneau de Macaulay, de sorte que l’hypothèse du corollaire 4 est elle-même satisfaite pour $d = 1$).

b) Notons b l’idéal de S engendré par $T_1T_2$, $T_1T_3$, $T_2T_4$, $T_3T_4$, et B l’anneau $S/b$. On a $b = p_{14}p_{23} = p_{14} \cap p_{23}$. L’anneau B est réduit. Son spectre s’identifie à la partie fermée $X_{14} \cup X_{23}$ de Spec(A) ; il a deux composantes irréductibles (de dimension 2) dont l’intersection est réduite à un point. La profondeur de B le long de ce point est strictement positive car B est réduit, et inférieure à 1 d’après le th. 3, donc égale à 1.* Ainsi B n’est pas un anneau de Macaulay. \*

### 10. Profondeur et normalité

Soient A un anneau noethérien et $p$ un idéal premier de A. On a $\mathrm{prof}(A_p) \leq \mathrm{ht}(p)$ (n° 4, cor. 2 du th. 2). Si de plus A est réduit, l’anneau local $A_p$ est réduit (II, § 2, n° 6, prop. 17), ce qui entraîne :

a) si $\mathrm{ht}(p) = 0$, $A_p$ est un corps ;
b) si $\mathrm{ht}(p) \geq 1$, on a $\mathrm{prof}(A_p) \geq 1$ (n° 1, remarque 3).

Inversement :

#### Proposition 15 {#ac-x-s1-prop-15 .statement}

Soit A un anneau noethérien satisfaisant aux deux conditions suivantes :
(i) pour tout idéal premier minimal $p$ de $\Lambda$, l’anneau $\Lambda_p$ est réduit ;
(ii) pour tout idéal premier $p$ de A de hauteur $\geq 1$, on a $\mathrm{prof}(A_p) \geq 1$.
Alors A est réduit.

Notons $n$ le nilradical de A. Pour tout idéal premier minimal $p$ de A, on a d’après (i) $n_p = 0$, c’est-à-dire $p \not\in \mathrm{Supp}(n)$ et $a fortiori$ $p \not\in \mathrm{Ass}_A(n)$. Pour tout $p \in \mathrm{Spec}(A)$ de hauteur $\geq 1$, on a d’après (ii) $pA_p \not\in \mathrm{Ass}_{A_p}(A_p)$ et $a fortiori$ $pA_p \not\in \mathrm{Ass}_{A_p}(n_p)$, d’où $p \not\in \mathrm{Ass}_A(n)$ (IV, § 1, n° 2, prop. 5). Ainsi l’ensemble $\mathrm{Ass}_A(n)$ est vide, ce qui implique que $n$ est nul.

#### Proposition 16 {#ac-x-s1-prop-16 .statement}

Soient $A$ un anneau noethérien intégralement clos, $J$ un idéal de $A$ de hauteur $\geqslant 2$, et $M$ un $A$-module réflexif de type fini. On a $\operatorname{prof}_A(J; M) \geqslant 2$.

Choisissons un espace vectoriel $V$ de dimension finie sur le corps des fractions de $A$ et un réseau $N$ de $V$ isomorphe à $M$ (VII, § 4, n° 2, remarque 1). Les idéaux premiers associés à $V/N$, étant de hauteur 1 (*loc. cit.*, th. 2), ne contiennent pas $J$; d’après la remarque 2 du n° 1, cela entraîne $\operatorname{prof}_A(J; V/N) \geqslant 1$. D’autre part, le $A$-module $V$ est divisible et sans torsion, donc injectif (A, X, p. 17, cor. 2 de la prop. 10), ce qui implique $\operatorname{prof}_A(J; V) = +\infty$. L’inégalité $\operatorname{prof}_A(J; N) \geqslant 2$ résulte alors de la prop. 1 du n° 1.

#### Corollaire {#ac-x-s1-n10-cor-1 .statement}

*Un anneau local noethérien intégralement clos de dimension $\geqslant 2$ est de profondeur $\geqslant 2$*.

Soient $A$ un anneau normal (n° 8) et $\mathfrak{p}$ un idéal premier de $A$. Alors :
a) si $\operatorname{ht}(\mathfrak{p}) = 0$, $A_{\mathfrak{p}}$ est un corps ;
b) si $\operatorname{ht}(\mathfrak{p}) = 1$, $A_{\mathfrak{p}}$ est un anneau de valuation discrète (VII, § 1, n° 7, prop. 11) ;
c) si $\operatorname{ht}(\mathfrak{p}) \geqslant 2$, on a $\operatorname{prof}(A_{\mathfrak{p}}) \geqslant 2$ (cor. de la prop. 16).

Inversement :

#### Théorème 4 (Serre) {#ac-x-s1-thm-4 .statement}

*Soit $A$ un anneau noethérien satisfaisant aux conditions suivantes*:
(i) *pour tout idéal premier minimal $\mathfrak{p}$ de $A$, l’anneau $A_{\mathfrak{p}}$ est réduit* ;
(ii) *pour tout idéal premier $\mathfrak{p}$ de $A$ de hauteur 1, l’anneau $A_{\mathfrak{p}}$ est intégralement clos* ;
(iii) *pour tout idéal premier $\mathfrak{p}$ de $A$ de hauteur $\geqslant 2$, on a $\operatorname{prof}(A_{\mathfrak{p}}) \geqslant 2$*.

*Alors $A$ est normal*.

Il s’agit de prouver que l’anneau $A_{\mathfrak{p}}$ est intégralement clos pour tout $\mathfrak{p} \in \operatorname{Spec}(A)$, ce que nous allons faire par récurrence sur $\operatorname{ht}(\mathfrak{p})$. Pour $\operatorname{ht}(\mathfrak{p}) \leqslant 1$ cela résulte des hypothèses (i) et (ii). Supposons donc qu’on ait $\operatorname{ht}(\mathfrak{p}) \geqslant 2$ et que $A_q$ soit intégralement clos pour tout idéal premier $q$ de $A$ de hauteur $< \operatorname{ht}(\mathfrak{p})$. D’après l’hypothèse (iii), on a $\operatorname{prof}(A_{\mathfrak{p}}) \geqslant 2$. D’après l’hypothèse de récurrence et le cor. 3 du th. 3 du n° 9, appliqué à l’anneau $A_{\mathfrak{p}}$ et à la partie fermée $\{\mathfrak{p}A_{\mathfrak{p}}\}$ de $\operatorname{Spec}(A_{\mathfrak{p}})$, l’anneau $A_{\mathfrak{p}}$ est intègre. Soit $K$ son corps des fractions et soit $B$ un sous-anneau de $K$, contenant $A_{\mathfrak{p}}$ et fini sur $A_{\mathfrak{p}}$. Il s’agit de prouver que $B$ est égal à $A_{\mathfrak{p}}$. Notons $i$ l’injection canonique de $A_{\mathfrak{p}}$ dans $B$. Comme $B$ est contenu dans $K$, c’est un $A_{\mathfrak{p}}$-module sans torsion, donc de profondeur $\geqslant 1$. Par ailleurs, pour tout idéal premier $q$ de $A_{\mathfrak{p}}$ distinct de $\mathfrak{p}A_{\mathfrak{p}}$, l’homomorphisme $i_q : (A_{\mathfrak{p}})_q \to B_q$ est bijectif puisque $A_q$ est intégralement clos. D’après le lemme 4 du n° 9, appliqué à la partie fermée $F = \{\mathfrak{p}A_{\mathfrak{p}}\}$ de $\operatorname{Spec}(A_{\mathfrak{p}})$, l’homomorphisme $i$ est bijectif, ce qui achève la démonstration du théorème.

#### Remarque 1 {#ac-x-s1-n10-rem-1 .statement}

Une forme commode du th. 4 est la suivante : soit $A$ un anneau noethérien, tel que pour tout idéal premier $p$ de $A$ l’anneau $A_p$ soit intégralement clos ou de profondeur $\geqslant 2$; alors $A$ est normal. Vérifions en effet les hypothèses du th. 4. Soit $p \in \mathrm{Spec}(A)$. Si $\mathrm{ht}(p) \leqslant 1$, alors on a $\mathrm{prof}(A_p) \leqslant 1$, donc $A_p$ est intégralement clos. Si $\mathrm{ht}(p) \geqslant 2$, l’anneau $A_p$ est soit de profondeur $\geqslant 2$, soit intégralement clos, ce qui implique encore $\mathrm{prof}(A_p) \geqslant 2$ (n° 1, cor. 2 de la prop. 1), d’où la conclusion cherchée. On vérifie de même l’énoncé suivant : soit $A$ un anneau noethérien tel que pour tout idéal premier $p$ de $A$, l’anneau $A_p$ soit réduit ou de profondeur $\geqslant 1$; alors $A$ est réduit.

#### Corollaire 1 {#ac-x-s1-thm-4-cor-1 .statement}

*Soient $\Lambda$ un anneau noethérien, $F$ une partie fermée de $\mathrm{Spec}(A)$, $U$ l’ouvert complémentaire. On suppose que $\mathrm{prof}_F(A)$ est $\geqslant 2$ (resp. $\geqslant 1$) et que, pour tout $p \in U$, l’anneau $A_p$ est intégralement clos (resp. réduit). Alors $A$ est normal* (resp. réduit).

Pour tout $p \in F$, on a $\mathrm{prof}(A_p) \geqslant \mathrm{prof}_F(A)$ (n° 5, prop. 8); il suffit donc d’appliquer la remarque précédente.

#### Corollaire 2 {#ac-x-s1-thm-4-cor-2 .statement}

*Soit $\rho : A \to B$ un homomorphisme d’anneaux noethériens faisant de $B$ un $A$-module plat.

a) *Si $B$ est normal et fidèlement plat sur $A$, $A$ est normal.*

b) *Supposons que $A$ soit normal et que l’anneau $\kappa(p) \otimes_A B$ soit normal lorsque $p$ est un idéal premier minimal de $A$, et réduit lorsque $p$ est un idéal premier de hauteur 1. Alors l’anneau $B$ est normal.*

a) Supposons $B$ normal et fidèlement plat sur $A$. Alors $\rho$ est injectif (I, § 3, n° 5, prop. 9) et $B$ est réduit, donc $A$ est réduit. Soit $S$ l’ensemble des éléments de $A$ non diviseurs de zéro. Puisque $B$ est plat sur $A$, $\rho(S)$ est formé d’éléments non diviseurs de zéro dans $B$, de sorte que $B$ est intégralement fermé dans $\rho(S)^{-1}B$. Soit $x$ un élément de $S^{-1}A$ entier sur $A$; alors l’élément $x \otimes 1_B$ de l’anneau $S^{-1}A \otimes_A B$ (qui s’identifie à $\rho(S)^{-1}B$) est entier sur $B$, donc appartient à $B$. Puisque $B$ est fidèlement plat sur $A$, on a $x \in A$ (I, § 3, n° 5, prop. 10, (ii)), et $A$ est normal.

b) Sous les hypothèses de b), il suffit d’après la remarque 1 de prouver que pour tout idéal premier $q$ de $B$, l’anneau local $B_q$ est normal ou de profondeur $\geqslant 2$. Notons $p$ l’idéal premier $\rho^{-1}(q)$ de $A$; l’homomorphisme local $A_p \to B_q$ déduit de $\rho$ fait de $B_q$ un $A_p$-module fidèlement plat (I, § 3, n° 5, prop. 9). Distinguons quatre cas :

1) $\mathrm{ht}(p) = 0$. Alors $A_p$ est un corps, égal à $\kappa(p)$; l’anneau $A_p \otimes_A B$ est normal par hypothèse. Il en est de même de $B_q$, qui en est un anneau de fractions.

#### Remarque 2 {#ac-x-s1-n10-rem-2 .statement}

$\mathrm{ht}(p) = 1$ et $\mathrm{ht}(q) \leqslant 1$. Alors $A_p$ est un anneau de valuation discrète; soit $\pi$ une uniformisante de $A_p$. Puisque $B_q$ est fidèlement plat sur $A_p$, l’élément $\pi 1_{B_q}$ de $B_q$ n’est pas diviseur de zéro, de sorte que l’anneau local $B_q/\pi B_q$ est de dimension 0 (VIII, § 3, n° 1, cor. 2 de la prop. 1). Il est réduit, puisque c’est un anneau de fractions de l’anneau réduit $\kappa(p) \otimes_A B$, et par suite c’est un corps. Par conséquent $B_q$ est un anneau de valuation discrète (VI, § 1, n° 4, prop. 2), donc intégralement clos.

#### Remarque 3 {#ac-x-s1-n10-rem-3 .statement}

$\mathrm{ht}(p) = 1$ et $\mathrm{ht}(q) \geq 2$. Alors, d’après la relation
$$
\dim(B_q) = \dim(A_p) + \dim(\kappa(p) \otimes_A B_q)
$$
(VIII, § 3, n° 4, cor. 1 de la prop. 7), l’anneau $\kappa(p) \otimes_A B_q$ est de dimension $\geq 1$. Il est réduit par hypothèse, donc de profondeur $\geq 1$ (n° 1, remarque 3). On a alors (n° 6, cor. de la prop. 11)
$$
\mathrm{prof}(B_q) = \mathrm{prof}(A_p) + \mathrm{prof}(\kappa(p) \otimes_A B_q) \geq 1 + 1 = 2 .
$$

#### Remarque 4 {#ac-x-s1-n10-rem-4 .statement}

$\mathrm{ht}(p) \geq 2$. Puisque $A_p$ est de profondeur $\geq 2$ (cor. de la prop. 16), il en est de même de $B_q$ d’après *loc. cit*.

#### Corollaire 3 {#ac-x-s1-thm-4-cor-3 .statement}

*Soit $\rho : A \to B$ un homomorphisme d’anneaux noethériens. On suppose que $B$ est un $A$-module plat, que $A$ est normal et que $\kappa(p) \otimes_A B$ est normal pour tout $p \in \mathrm{Spec}(A)$. Alors $B$ est normal.*

## EXERCICES {#ac-x-s1-exercises}

See the [exercises for § 1](exercises/s1/).
