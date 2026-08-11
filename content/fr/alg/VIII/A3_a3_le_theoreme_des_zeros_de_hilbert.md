---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 3
section_title: Le théorème des zéros de Hilbert
appendix: true
lang: fr
source: alg-viii-fr
book_pages: A VIII.451-A VIII.452
pdf_pages: 0452-0453
extraction: native
statements: 3
exercises: 0
content_sha256: e1e47e8f56708fded9c13b338ea2c9b4a1db3a4f4b74ce13cacbbe020c7db8d6
---

### APPENDICE 3 LE THÉORÈME DES ZÉROS DE HILBERT

#### Théorème 1 {#alg-viii-a3-thm-1 .statement tag=00QM}

Soient A un anneau intègre, K son corps des fractions et L une K-algèbre commutative. Supposons que la A-algèbre L soit engendrée par un nombre fini d’éléments et que L soit un corps.

a) Le degré de L sur K est fini ;

b) Il existe un élément non nul $a$ de A tel que K soit égal à $A[a^{-1}]$.

Soit S une partie génératrice de la A-algèbre L. Raisonnons par récurrence sur le cardinal de S.

Supposons d’abord que les éléments de S soient tous algébriques sur K. Le degré de L sur K est alors fini (V, p. 17, th. 2). Soit $(e_i)_{i\in I}$ une base de L sur K. Il existe un élément non nul $a$ de A tel que les coordonnées par rapport à cette base des éléments de S, de l’élément 1 et des éléments $e_ie_j$ pour $i,j$ dans I appartiennent à $A[a^{-1}]$. L’ensemble des combinaisons linéaires $\sum_{i\in I}a_ie_i$, avec $a_i\in A[a^{-1}]$ pour tout $i$, est alors un sous-anneau de L. Il contient A et S par construction, donc est égal à L. Il contient en particulier $Ke_1$, donc K est égal à $A[a^{-1}]$.

Supposons maintenant qu’un élément $s$ de S soit transcendant sur K. Notons E le corps des fractions de l’anneau $A[s]$. La $A[s$]-algèbre L est engendrée par S$-\{s\}$. D’après l’hypothèse de récurrence, il existe un polynôme non nul $P\in A[X]$ tel que E soit égal à $A[s][P(s)^{-1}]$. Soit K une clôture algébrique de K (V, p. 22, th. 2). Comme le corps K est infini (V, p. 20, prop. 3), il existe un élément $x$ de K tel que $P(x)\not= 0$. Soit $\varphi : E\rightarrow K$ l’unique homomorphisme de la K-algèbre $E = A[s][P(s)^{-1}]$ dans la K-algèbre K qui applique $s$ sur $x$. Mais cela est absurde puisque E est une extension transcendante de K et K une extension algébrique de K. Cela termine la démonstration du théorème.

#### Corollaire 1 {#alg-viii-a3-thm-1-cor-1 .statement tag=00RV}

Soient K un corps commutatif, A une K-algèbre commutative engendrée par un nombre fini d’éléments et $\mathfrak{m}$ un idéal maximal de A.

a) Le degré de $A/\mathfrak{m}$ sur K est fini.

b) Soit Ω un extension algébriquement close de K. Il existe un homomorphisme de K-algèbres de A dans Ω dont le noyau est $\mathfrak{m}$.

La K-algèbre $A/\mathfrak{m}$ est engendrée par un nombre fini d’éléments et $A/\mathfrak{m}$ est un corps. D’après le théorème 1, le degré de $A/\mathfrak{m}$ est fini d’où a). Toute extension de degré fini de K est isomorphe à une sous-extension de Ω (V, p. 20, th. 1), d’où b).

#### Corollaire 2 {#alg-viii-a3-thm-1-cor-2 .statement tag=00QN}

Soient K un corps commutatif, $n$ un entier naturel, $(P_i)_{i\in I}$ une famille d’éléments de $K[X_1, . . . ,X_n]$et Ω une extension algébriquement close de K. Les conditions suivantes sont équivalentes :

(i) Les polynômes $P_i$ n’ont pas de zéro commun dans $\Omega^n$;

(ii) Il existe une famille $(Q_i)_{i\in I}$ à support fini d’éléments de $K[X_1, . . . ,X_n]$telle que $\sum_{i\in I}P_iQ_i= 1$.

Notons A l’anneau $K[X_1, . . . ,X_n]$ et $\mathfrak{a}$ l’idéal engendré par les polynômes $P_i$. La condition (i) signifie qu’il n’existe aucun homomorphisme de K-algèbres de $A/\mathfrak{a}$ dans Ω. Si elle est satisfaite, l’anneau $A/\mathfrak{a}$ ne possède d’après le cor. 1 aucun idéal maximal, donc est nul et 1 appartient à $\mathfrak{a}$. Cela prouve que (i) implique (ii). L’implication (ii) $\Rightarrow$ (i) est claire.
