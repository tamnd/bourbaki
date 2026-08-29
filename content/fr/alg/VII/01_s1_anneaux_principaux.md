---
book: alg
book_title: Algebra
chapter: VII
chapter_title: Modules sur les anneaux principaux
section: 1
section_title: ANNEAUX PRINCIPAUX
lang: fr
source: alg-iv-vii-fr
pdf_pages: 0334-0339, 0381-0386
extraction: ocr
subsections:
    - "no": 1
      title: Définition d’un anneau principal
      page: 0
      pdf_page: 334
    - "no": 2
      title: Divisibilité dans les anneaux principaux
      page: 0
      pdf_page: 334
    - "no": 3
      title: Décomposition en facteurs extrémaux dans les anneaux principaux
      page: 3
      pdf_page: 336
    - "no": 4
      title: Divisibilité des entiers rationnels
      page: 4
      pdf_page: 337
    - "no": 5
      title: Divisibilité des polynômes à une indéterminée sur un corps
      page: 5
      pdf_page: 338
statements: 15
exercises: 10
content_sha256: 9dc599f9b4c10081b93a10c9bf65a28d23367b7369c57f86f2d79b8655b439f0
---

## § 1. ANNEAUX PRINCIPAUX

### 1. Définition d’un anneau principal

Rappelons (I, p. 99) qu’un idéal d’un anneau commutatif $A$ est dit *principal* s’il est de la forme $(a) = Aa$, avec $a \in A$.

#### Définition 1 {#alg-vii-s1-def-1 .statement}

*Un anneau principal est un anneau commutatif, intègre* (I, p. 110) *dont tout idéal est principal*.

#### Exemple {#alg-vii-s1-n1-exa-1 .statement}

L’anneau $\mathbf{Z}$ des entiers rationnels est principal (I, p. 47). Si $K$ est un corps commutatif, l’anneau $K[X]$ des polynômes à une indéterminée sur $K$ est un anneau principal (IV, p. 11, prop. 11); il en est de même de l’anneau de séries formelles $K[[X]]$, car tout idéal de cet anneau est de la forme $(X^n)$ (IV, p. 36, prop. 12). *L’anneau des entiers d’un corps $p$-adique est principal.* \*

Si $Q(i)$ désigne le corps obtenu à partir du corps $Q$ des nombres rationnels par adjonction d’une racine $i$ du polynôme irréductible $X^2 + 1$, les éléments $a + bi$ de $Q(i)$, où $a$ et $b$ sont des entiers rationnels, forment un sous-anneau $A$ de $Q(i)$, appelé « anneau des *entiers de Gauss* », qui est principal (VII, p. 49, exerc. 7). Par contre, dans le corps $Q(\rho)$, où $\rho$ est une racine de $X^2 + 5$, le sous-anneau $B$ composé des éléments $a + b\rho$ ($a$ et $b$ entiers rationnels) n’est pas un anneau principal (VII, p. 51, exerc. 12).

L’anneau $K[X, Y]$ des polynômes à deux indéterminées sur un corps $K$ n’est pas principal : en effet seules les constantes non nulles divisent à la fois $X$ et $Y$, et aucune n’engendre l’idéal engendré par $X$ et $Y$.

### 2. Divisibilité dans les anneaux principaux

Soient $A$ un anneau principal, et $K$ son corps des fractions (I, p. 110); nous allons voir que le groupe ordonné $\mathcal{P}^*$ des idéaux principaux fractionnaires (VI, p. 6) de $K$ est réticulé ; de façon plus précise :

#### Proposition 1 {#alg-vii-s1-prop-1 .statement}

*Soient $K$ le corps des fractions d’un anneau principal $A$, et $(x_i)_{i \in I}$ une famille d’éléments de $K$ admettant un dénominateur commun $b \in K^*$ (c’est-à-dire que $bx_i \in A$ pour tout $i$). Alors :*

a) *La famille $(x_i)$ admet un pgcd dans $K$.*

b) Tout pgcd de $(x_i)$ se met sous la forme $d = \sum a_i x_i$ où les $a_i$ sont des éléments de $A$, nuls à l’exception d’un nombre fini d’entre eux.

En effet l’idéal $\sum Abx_i$ de $A$ est principal, donc de la forme $Ad'$. Posons $d' = bd$ ($d \in K$). De la relation $d' = \sum a_i b x_i$, on tire $d = \sum a_i x_i$, où $a_i \in A$, donc tout diviseur commun des $x_i$ divise $d$. D’autre part, comme $bd$ est un diviseur commun des $bx_i$ par construction, $d$ est un diviseur commun des $x_i$.

#### Remarque {#alg-vii-s1-n2-rem-1 .statement}

La prop. 1 s’applique sans restriction à une famille quelconque $(x_i)$ d’éléments de $A$ (il suffit de prendre $b = 1$), et aussi à une famille *finie* $(x_i)$ d’éléments de $K$ (en effet, si $x_i = c_i b_i^{-1}$, avec $c_i \in A$ et $b_i \in A$, il suffit de prendre pour $b$ le produit des $b_i$).

#### Corollaire {#alg-vii-s1-n2-cor-1 .statement}

Soit $(x_i)$ une famille quelconque d’éléments d’un sous-anneau principal $A$ d’un anneau intègre $B$, et soit $d$ un pgcd de la famille $(x_i)$ dans $A$. Alors la famille $(x_i)$ admet des pgcd dans $B$, et $d$ est l’un de ces pgcd.

En effet $d$ est un diviseur commun des $x_i$ dans $B$. D’autre part la relation $d = \sum a_i x_i$ ($a_i \in A$) montre que tout diviseur commun des $x_i$ dans $B$ divise $d$.

Un cas important d’application de ce corollaire est celui où $A = K[X]$, $B = E[X]$, $K$ étant un corps et $E$ une extension de $K$ (IV, p. 12, cor. 1).

La première assertion de la prop. 1 montre que le groupe ordonné $\mathcal{P}^*$ est réticulé (VI, p. 10). En particulier toute famille finie d’éléments de $K$ admet un ppcm. Nous pouvons donc appliquer à un anneau principal les résultats notés (DIV) de VI, p. 10 à 17.

Comme conséquence de la seconde assertion de la prop. 1, on a le résultat suivant :

#### Théorème 1 (« identité de Bezout ») {#alg-vii-s1-thm-1 .statement}

Pour que les éléments $x_i$ ($i \in I$) d’un anneau principal $A$ soient étrangers dans leur ensemble, il faut et il suffit qu’il existe des éléments $a_i$ ($i \in I$) de $A$, nuls sauf un nombre fini d’entre eux, et tels que $\sum a_i x_i = 1$.

C’est nécessaire d’après la prop. 1. Réciproquement, si $\sum a_i x_i = 1$, tout diviseur commun des $x_i$ dans $K$ divise 1, donc 1 est un pgcd des $x_i$.

#### Proposition 2 {#alg-vii-s1-prop-2 .statement}

Soient $a, b, d, m$ et $p$ des éléments du corps des fractions $K$ d’un anneau principal $A$.
a) « $d$ est un pgcd de $a$ et $b$ » équivaut à « $(d) = (a) + (b)$ ».
b) « $m$ est un ppcm de $a$ et $b$ » équivaut à « $(m) = (a) \cap (b)$ ».
c) « $p$ est élément extrémal de $A$ » équivaut à « $(p)$ est un idéal maximal non nul de $A$ » et à « $(p)$ est un idéal premier non nul de $A$ ».

Nous avons déjà démontré $a$ (prop. 1). Comme les multiples communs de $a$ et $b$ sont les éléments de $(a) \cap (b)$, et que $(a) \cap (b)$ est, par hypothèse, un idéal principal $(m)$, $m$ est un ppcm de $a$ et $b$, ce qui démontre $b$. Enfin dire que $p \neq 0$ est élément extrémal de $A$ veut dire, par définition (VI, p. 16), que $(p)$ est un élément maximal de la famille ordonnée par inclusion des idéaux principaux $\neq A$ de $A$; comme $A$ n’a d’autres idéaux que les idéaux principaux, ceci veut dire que $(p)$ est idéal maximal de $\mathbf{A}$, d’où $c$), compte tenu de la remarque de VI, p. 17.

Dans un anneau principal $\mathbf{A}$, on dit encore que la somme (resp. l’intersection) d’un nombre fini d’idéaux de $\mathbf{A}$ est le pgcd (resp. ppcm) de ces idéaux.

#### Proposition 3 {#alg-vii-s1-prop-3 .statement}

*Soient $a, b, c$ des éléments du corps des fractions d’un anneau principal $\mathbf{A}$, et soit $d$ un pgcd de $a$ et $c$; pour que la congruence $ax \equiv b$ (mod. $c$) admette une solution $x_0 \in \mathbf{A}$, il faut et il suffit que $d$ divise $b$; dans ce cas les éléments $x \in \mathbf{A}$ solutions de $ax \equiv b$ (mod. $c$) sont les mêmes que ceux qui satisfont à $x \equiv x_0$ (mod. $cd^{-1}$).

Si $ax \equiv b$ (mod. $c$) avec $x \in \mathbf{A}$, il existe $y \in \mathbf{A}$ tel que $b = ax + cy$, donc $d$ divise $b$. Réciproquement, si $d$ divise $b$, on a $b = ax_0 + cy_0$, où $x_0$ et $y_0$ appartiennent à $\mathbf{A}$ (prop. 1), donc $ax_0 \equiv b$ (mod. $c$); en outre, la relation $ax \equiv b$ (mod. $c$) est alors équivalente à $a(x - x_0) \equiv 0$ (mod. $c$); en posant $a = da'$ et $c = dc'$, ceci s’écrit $a'(x - x_0) \equiv 0$ (mod. $c'$). Mais cette dernière relation équivaut (pour $x \in \mathbf{A}$) à $x - x_0 \equiv 0$ (mod. $c'$), puisque $a'$ et $c'$ sont des éléments étrangers (VI, p. 14, prop. 10 (DIV) et VI, p. 15, cor. 2 de la prop. 11 (DIV)).

#### Proposition 4 {#alg-vii-s1-prop-4 .statement}

*Soit $(a_i)_{1 \leq i \leq n}$ une famille finie d’éléments deux à deux étrangers d’un anneau principal $\mathbf{A}$. Alors l’homomorphisme canonique (I, p. 104) de $\mathbf{A}/(\prod_{i=1}^n a_i)$ dans le produit $\prod_{i=1}^n \mathbf{A}/(a_i)$ est un isomorphisme de $\mathbf{A}$-algèbres.

Cela résulte de I, p. 104, prop. 9 et de la prop. 2, *a*).

La conclusion de la prop. 4 n’est plus valable si on ne suppose pas que les $a_i$ sont deux à deux étrangers (*cf.* VII, p. 24, prop. 9).

### 3. Décomposition en facteurs extrémaux dans les anneaux principaux

Nous allons maintenant appliquer aux anneaux principaux les résultats de VI, p. 17, relatifs à la décomposition en éléments extrémaux. D’après la prop. 2, pour qu’un élément $p \neq 0$ d’un anneau principal $\mathbf{A}$ soit extrémal, il faut et il suffit que l’anneau $\mathbf{A}/(p)$ soit un corps (I, p. 109, cor. 1), c’est-à-dire que la congruence $ax \equiv b$ (mod. $p$) admette une solution dans $\mathbf{A}$ quels que soient $b \in \mathbf{A}$ et $a \in \mathbf{A}$ non multiple de $p$.

#### Définition 2 {#alg-vii-s1-def-2 .statement}

*Soit $\mathbf{A}$ un anneau intègre. On appelle système représentatif d’éléments extrémaux de $\mathbf{A}$ une famille $(p_\alpha)$ d’éléments extrémaux de $\mathbf{A}$ telle que tout élément extrémal de $\mathbf{A}$ soit associé à un $p_\alpha$ et à un seul.*

#### Théorème 2 {#alg-vii-s1-thm-2 .statement}

*Soient $\mathbf{A}$ un anneau principal et $(p_\alpha)$ un système représentatif d’éléments extrémaux de $\mathbf{A}$. Alors tout élément non nul $x$ du corps des fractions de $\mathbf{A}$ s’écrit, et d’une seule manière, sous la forme*

$$
x = u \prod_\alpha p_\alpha^{n_\alpha},
$$

où u est un élément inversible de A, et où les $n_\alpha$ sont des entiers rationnels nuls sauf un nombre fini d’entre eux. Pour que x appartienne à A, il faut et il suffit que tous les $n_\alpha$ soient positifs.

Nous allons utiliser le théorème de décomposition en somme d’éléments extrémaux (VI, p. 17, th. 2), dont l’énoncé ci-dessus n’est qu’une traduction. Comme $\mathcal{P}^*$ est un groupe réticulé, il nous suffira, pour constater que nous sommes bien dans les conditions d’application de ce théorème, de montrer que tout ensemble non vide d’idéaux principaux de A contient un élément maximal ; or c’est ce qui résulte du lemme suivant :

#### Lemme 1 {#alg-vii-s1-lem-1 .statement}

Soit A un anneau tel que tout idéal à gauche de A soit de type fini. Alors tout ensemble non vide $\Phi$ d’idéaux à gauche de A, ordonné par inclusion, possède un élément maximal.

En vertu du th. de Zorn (E, III, p. 20, th. 2), il nous suffit de prouver que $\Phi$ est inductif. Or, si $(\alpha_\lambda)$ est une famille totalement ordonnée d’éléments de $\Phi$, la réunion $\alpha$ des idéaux $\alpha_\lambda$ est un idéal à gauche de A, et admet donc un système fini de générateurs $(a_i)_{1 \leq i \leq n}$. Comme chacun des $a_i$ appartient à un idéal $\alpha_{\lambda_i}$, et que la famille $(\alpha_\lambda)$ est totalement ordonnée, les $a_i$ ($1 \leq i \leq n$) appartiennent tous au plus grand des idéaux $\alpha_{\lambda_i}$, soit $\alpha_\mu$. Alors $\alpha = \alpha_\mu$ appartient à $\Phi$, qui est donc bien un ensemble inductif.

Nous étudierons plus tard, sous le nom d’anneaux noethériens, les anneaux B tels que tout ensemble non vide d’idéaux à gauche de B possède un élément maximal.

#### Remarque {#alg-vii-s1-n3-rem-1 .statement}

La famille $(u, (n_\alpha))$ est appelée la décomposition de x en facteurs extrémaux ; par abus de langage, on dit aussi que la formule (1) est la décomposition de x en facteurs extrémaux. Si $x = u \prod_\alpha p_\alpha^{n_\alpha}$ et $y = v \prod_\alpha p_\alpha^{m_\alpha}$ sont les décompositions de x et y en facteurs extrémaux, une condition nécessaire et suffisante pour que x divise y est que l’on ait $n_\alpha \leq m_\alpha$ pour tout $\alpha$ ; de ceci on déduit les formules

(2)
$$
\operatorname{pgcd}(x, y) = \prod_\alpha p_\alpha^{\inf(n_\alpha, m_\alpha)}
$$

(3)
$$
\operatorname{ppcm}(x, y) = \prod_\alpha p_\alpha^{\sup(n_\alpha, m_\alpha)}.
$$

La propriété exprimée par le th. 2 est vraie pour des anneaux plus généraux que les anneaux principaux ; nous les étudierons plus tard sous le nom d’anneaux factoriels ; et nous verrons que les anneaux de polynômes et de séries formelles à un nombre quelconque d’indéterminées sur un corps sont des anneaux factoriels (AC, VII, § 3).

### 4. Divisibilité des entiers rationnels

Comme il a été dit au n° 1, l’anneau $\mathbf{Z}$ des entiers rationnels est un anneau principal ; son corps des fractions est $\mathbf{Q}$. Le groupe multiplicatif U des éléments inversibles de $\mathbf{Z}$ a deux éléments 1 et $-1$. Le groupe $\mathbf{Q}_+^*$ des nombres rationnels $> 0$ contient un élément et un seul de chaque classe d’éléments associés de $\mathbf{Q}$ ; il est donc isomorphe au groupe multiplicatif $\mathcal{P}^* = \mathbf{Q}_+^*/U$ des idéaux principaux fractionnaires de $\mathbf{Q}$, auquel on l’identifiera le plus souvent. En particulier, chaque fois qu’il sera question de pgcd ou de ppcm dans le corps $\mathbf{Q}$ (relativement à l’anneau $\mathbf{Z}$), il sera sous-entendu que ce sont des éléments $\geqslant 0$; grâce à cette convention on pourra parler sans ambiguïté *du* pgcd et *du* ppcm d’une famille de nombres rationnels.

Les entiers extrémaux $> 0$ de $\mathbf{Z}$ ne sont autres que ceux que nous avons appelés *nombres premiers* (I, p. 48) (on les appelle parfois *nombres premiers rationnels*) ; tout élément extrémal de $\mathbf{Z}$ est donc de la forme $p$ ou $-p$, où $p$ est un nombre premier, et l’ensemble $P$ des nombres premiers est un système représentatif d’éléments extrémaux de $\mathbf{Z}$.

#### Proposition 5 {#alg-vii-s1-prop-5 .statement}

*L’ensemble des nombres premiers est infini.*

En effet, étant donnée une famille finie quelconque $(p_i)$ ($1 \leqslant i \leqslant n$) de nombres premiers distincts, un diviseur premier $q$ du nombre $\left( \prod_{i=1}^n p_i \right) + 1$ (qui est $> 1$) est distinct de tous les $p_i$, sinon il diviserait 1.

### 5. Divisibilité des polynômes à une indéterminée sur un corps

L’anneau $K[X]$ des polynômes à une indéterminée sur un corps commutatif $K$ est un anneau principal (IV, p. 11, prop. 11). Son corps des fractions est le corps $K(X)$ des fractions rationnelles en $X$ à coefficients dans $K$. L’anneau $K[X]$ contient le sous-anneau des polynômes de degré 0, c’est-à-dire le corps des constantes, qu’on identifie à $K$ ; les éléments de $K^*$ sont inversibles dans $K$, donc dans $K[X]$ ; et réciproquement la formule $\deg(uv) = \deg(u) + \deg(v)$ montre que tout polynôme inversible de $K[X]$ est de degré 0 ; le groupe $U$ des éléments inversibles de $K[X]$ est donc identique à $K^*$. Ainsi deux polynômes associés ne diffèrent que par un facteur constant non nul ; en particulier toute classe de polynômes associés contient un polynôme *unitaire* et un seul. Le sous-groupe du groupe multiplicatif $K(X)^*$ engendré par les polynômes unitaires contient donc un élément et un seul de chaque classe de fractions rationnelles associées, et est par conséquent isomorphe au groupe

$$
\mathcal{P}^* = K(X)^*/U
$$

des idéaux principaux fractionnaires de $K(X)$. En particulier, chaque fois qu’il sera question de pgcd ou de ppcm dans le corps $K(X)$ (relativement à l’anneau $K[X]$), il sera le plus souvent sous-entendu que ce sont des quotients de polynômes unitaires (ou 0) ; grâce à cette convention on pourra parler *du* pgcd et *du* ppcm d’une famille de fractions rationnelles.

Les éléments extrémaux de $K[X]$ ne sont autres que les *polynômes irréductibles* (IV, p. 13, déf. 2), et l’ensemble des polynômes unitaires irréductibles est un système représentatif d’éléments extrémaux de $K[X]$.

Un polynôme du premier degré est toujours irréductible. Si $K$ est un corps *algébriquement clos* la réciproque est vraie (V, p. 19, prop. 1) ; donc, dans ce cas, tout polynôme p(X) de degré n de K[X] s’écrit, d’une façon et d’une seule (à l’ordre près des facteurs)

$$
p(X) = c(X - a_1)(X - a_2) \ldots (X - a_n)
$$

où c et les $a_i$ sont des éléments de K.

#### Proposition 6 {#alg-vii-s1-prop-6 .statement}

*Pour tout corps K, l’ensemble des polynômes unitaires irréductibles de K[X] est infini.*

En effet, étant donnée une famille finie non vide quelconque $(p_i)$ ($1 \leq i \leq n$) de polynômes unitaires irréductibles distincts, le polynôme $\left( \prod_{i=1}^n p_i \right) + 1$ n’est pas inversible, et un facteur unitaire irréductible $q$ de ce polynôme est nécessairement distinct de tous les $p_i$, sinon il diviserait 1.

## EXERCICES {#alg-vii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
