---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: Sous-algèbres de Cartan. Éléments réguliers
section: 2
section_title: Sous-algèbres de Cartan et éléments réguliers d’une algèbre de Lie
lang: fr
source: lie-vii-viii-fr
pdf_pages: 0012-0020, 0052-0053
extraction: ocr
subsections:
    - "no": 1
      title: Sous-algèbres de Cartan
      page: 0
      pdf_page: 12
    - "no": 2
      title: Eléments réguliers d'une algèbre de Lie
      page: 0
      pdf_page: 15
    - "no": 3
      title: Sous-algèbres de Cartan et éléments réguliers
      page: 0
      pdf_page: 17
    - "no": 4
      title: Sous-algèbres de Cartan des algèbres de Lie semi-simples
      page: 0
      pdf_page: 19
statements: 40
exercises: 16
content_sha256: 376c38db366a6ff349b58d48f96a6a454428002a828f1a1940ce66799ee1c9d7
---

## § 2. Sous-algèbres de Cartan et éléments réguliers d’une algèbre de Lie

A partir du no 2, le corps $k$ est supposé infini.

### 1. Sous-algèbres de Cartan

#### Définition 1 {#lie-vii-s2-def-1 .statement tag=00TJ}

Soit $g$ une algèbre de Lie. On appelle sous-algèbre de Cartan de $g$ une sous-algèbre nilpotente de $g$ égale à son normalisateur.

Nous obtiendrons plus loin les résultats suivants:
1) si $k$ est infini, $g$ possède des sous-algèbres de Cartan (no 3, cor. 1 du th. 1);
2) si $k$ est de caractéristique 0, toutes les sous-algèbres de Cartan de $g$ ont même dimension ($§ 3$, no 3, th. 2);
3) si $k$ est algébriquement clos de caractéristique 0, toutes les sous-algèbres de Cartan de $g$ sont conjuguées par le groupe des automorphismes élémentaires de $g$ ($§ 3$, no 2, th. 1).

#### Exemple 1 {#lie-vii-s2-n1-exa-1 .statement tag=00TK}

Si $g$ est nilpotente, la seule sous-algèbre de Cartan de $g$ est $g$ elle-même (I, $§ 4$, no 1, prop. 3).

#### Exemple 2 {#lie-vii-s2-n1-exa-2 .statement tag=00TL}

Soient $g = gl(n, k)$, et $h$ l’ensemble des matrices diagonales appartenant à $g$. Montrons que $h$ est une sous-algèbre de Cartan de $g$. D’abord $h$ est commutative, donc nilpotente. Soit $(E_{ij})$ la base canonique de $gl(n, k)$, et soit $x = \sum \mu_{ij} E_{ij}$ un élément du normalisateur de $h$ dans $g$. Si $i \neq j$, les formules (5) de I, $§ 1$, no 2 montrent que le coefficient de $E_{ij}$ dans $[E_{ii}, x]$ est $\mu_{ij}$. Puisque $E_{ii} \in h$, on a $[E_{ii}, x] \in h$, et le coefficient en question est nul. On a donc $\mu_{ij} = 0$ pour $i \neq j$, d’où $x \in h$, ce qui montre bien que $h$ est une sous-algèbre de Cartan de $g$.

#### Exemple 3 {#lie-vii-s2-n1-exa-3 .statement tag=00TM}

Soit $\mathfrak{h}$ une sous-algèbre de Cartan de $\mathfrak{g}$ et soit $\mathfrak{g}_1$ une sous-algèbre de $\mathfrak{g}$ contenant $\mathfrak{h}$. Alors $\mathfrak{h}$ est une sous-algèbre de Cartan de $\mathfrak{g}_1$; cela résulte aussitôt de la déf. 1.

#### Proposition 1 {#lie-vii-s2-prop-1 .statement tag=00TN}

*Soit $\mathfrak{g}$ une algèbre de Lie et soit $\mathfrak{h}$ une sous-algèbre de Cartan de $\mathfrak{g}$. Alors $\mathfrak{h}$ est une sous-algèbre nilpotente maximale de $\mathfrak{g}$.

Soit $\mathfrak{h}'$ une sous-algèbre nilpotente de $\mathfrak{g}$ contenant $\mathfrak{h}$. Alors $\mathfrak{h}$ est sous-algèbre de Cartan de $\mathfrak{h}'$ (exemple 3), donc $\mathfrak{h} = \mathfrak{h}'$ (exemple 1).

Il existe des sous-algèbres nilpotentes maximales qui ne sont pas des sous-algèbres de Cartan (exerc. 2).

#### Proposition 2 {#lie-vii-s2-prop-2 .statement tag=00TO}

*Soient $(\mathfrak{g}_i)_{i \in I}$ une famille finie d’algèbres de Lie et $\mathfrak{g} = \prod_{i \in I} \mathfrak{g}_i$. Les sous-algèbres de Cartan de $\mathfrak{g}$ sont les sous-algèbres de la forme $\prod_{i \in I} \mathfrak{h}_i$ où $\mathfrak{h}_i$ est une sous-algèbre de Cartan de $\mathfrak{g}_i$.

Si $\mathfrak{h}_i$ est une sous-algèbre de $\mathfrak{g}_i$ de normalisateur $\mathfrak{n}_i$, alors $\prod_{i \in I} \mathfrak{h}_i$ est une sous-algèbre de $\mathfrak{g}$ de normalisateur $\prod_{i \in I} \mathfrak{n}_i$; si les $\mathfrak{h}_i$ sont nilpotentes, $\prod_{i \in I} \mathfrak{h}_i$ est nilpotente; donc si, pour tout $i$, $\mathfrak{h}_i$ est une sous-algèbre de Cartan de $\mathfrak{g}_i$, $\prod_{i \in I} \mathfrak{h}_i$ est une sous-algèbre de Cartan de $\mathfrak{g}$. Réciproquement, soit $\mathfrak{h}$ une sous-algèbre de Cartan de $\mathfrak{g}$; la projection $\mathfrak{h}_i$ de $\mathfrak{h}$ sur $\mathfrak{g}_i$ est une sous-algèbre nilpotente de $\mathfrak{g}_i$, et $\prod_{i \in I} \mathfrak{h}_i$ est une sous-algèbre nilpotente de $\mathfrak{g}$ contenant $\mathfrak{h}$; on a donc $\mathfrak{h} = \prod_{i \in I} \mathfrak{h}_i$ (prop. 1); pour tout $i$, $\mathfrak{h}_i$ est alors son propre normalisateur dans $\mathfrak{g}_i$, donc est une sous-algèbre de Cartan de $\mathfrak{g}_i$.

#### Exemple 4 {#lie-vii-s2-n1-exa-4 .statement tag=00TP}

Si $k$ est de caractéristique 0, $\mathrm{gl}(n, k)$ est produit des idéaux $\mathfrak{sl}(n, k)$ et $k.1$. Il résulte de l’exemple 2 et de la prop. 2 que l’ensemble des matrices diagonales de trace 0 dans $\mathfrak{sl}(n, k)$ est une sous-algèbre de Cartan de $\mathfrak{sl}(n, k)$.

#### Proposition 3 {#lie-vii-s2-prop-3 .statement tag=00TQ}

*Soient $\mathfrak{g}$ une algèbre de Lie, $\mathfrak{h}$ une sous-algèbre de $\mathfrak{g}$, $k'$ une extension de $k$. Alors $\mathfrak{h}$ est une sous-algèbre de Cartan de $\mathfrak{g}$ si et seulement si $\mathfrak{h} \otimes_k k'$ est une sous-algèbre de Cartan de $\mathfrak{g} \otimes_k k'$.

En effet, $\mathfrak{h}$ est nilpotente si et seulement si $\mathfrak{h} \otimes_k k'$ l’est (I, § 4, n° 5). D’autre part, si $\mathfrak{n}$ est le normalisateur de $\mathfrak{h}$ dans $\mathfrak{g}$, le normalisateur de $\mathfrak{h} \otimes_k k'$ dans $\mathfrak{g} \otimes_k k'$ est $\mathfrak{n} \otimes_k k'$ (I, § 3, n° 8).

#### Proposition 4 {#lie-vii-s2-prop-4 .statement tag=00TR}

*Soient $\mathfrak{g}$ une algèbre de Lie, $\mathfrak{h}$ une sous-algèbre nilpotente de $\mathfrak{g}$. Pour que $\mathfrak{h}$ soit sous-algèbre de Cartan de $\mathfrak{g}$, il faut et il suffit que $\mathfrak{g}^0(\mathfrak{h}) = \mathfrak{h}$.

Si $\mathfrak{g}^0(\mathfrak{h}) = \mathfrak{h}$, $\mathfrak{h}$ est son propre normalisateur ($\S$ 1, prop. 10 (i)), donc $\mathfrak{h}$ est une sous-algèbre de Cartan de $\mathfrak{g}$. Supposons $\mathfrak{g}^0(\mathfrak{h}) \neq \mathfrak{h}$. Considérons la représentation de $\mathfrak{h}$ dans $\mathfrak{g}^0(\mathfrak{h})/\mathfrak{h}$ déduite par passage au quotient de la représentation adjointe. En lui appliquant le théorème d’Engel (I, § 4, n° 2, th. 1), on voit qu’il existe x \in g^0(\mathfrak{h}) \text{ tel que } x \notin \mathfrak{h} \text{ et } [\mathfrak{h}, x] \subset \mathfrak{h}; \text{ alors } x \text{ appartient au normalisateur de } \mathfrak{h} \text{ dans } g, \text{ de sorte que } \mathfrak{h} \text{ n'est pas une sous-algèbre de Cartan de } g.

#### Corollaire 1 {#lie-vii-s2-prop-4-cor-1 .statement tag=00TS}

*Soient g une algèbre de Lie, h une sous-algèbre de Cartan de g. Si k est infini, il existe x \in h tel que h = g^0(x).*
En effet, on a $h = g^0(h)$, et on applique la prop. 9 (ii) du § 1.

#### Corollaire 2 {#lie-vii-s2-prop-4-cor-2 .statement tag=00TT}

*Soit f : g \to g' un homomorphisme surjectif d’algèbres de Lie. Si h est une sous-algèbre de Cartan de g, f(h) est une sous-algèbre de Cartan de g'.*
En effet, $f(h)$ est une sous-algèbre nilpotente de $g'$. D’autre part, considérons la représentation $x \mapsto \mathrm{ad}\,f(x)$ de $h$ dans $g'$. D’après la prop. 9 (iv) du § 1, n° 3, on a $f(g^0(h)) = {g'}^0(f(h))$. Or $g^0(h) = h$, et d’autre part, il est clair que ${g'}^0(f(h)) = {g'}^0(f(h))$. Donc $f(h) = {g'}^0(f(h))$ et il suffit d’appliquer la prop. 4.

#### Corollaire 3 {#lie-vii-s2-prop-4-cor-3 .statement tag=00TU}

*Soit h une sous-algèbre de Cartan d’une algèbre de Lie g, et soit C^n_g (n \geq 1) un terme de la série centrale descendante de g (I, § 1, n° 5, 2ème édition). On a g = h + C^n_g.*
En effet, le corollaire 2 montre que l’image de $h$ dans $g/C^n_g$ est une sous-algèbre de Cartan de $g/C^n_g$, donc est égale à $g/C^n_g$ puisque $g/C^n_g$ est nilpotente (exemple 1).

#### Corollaire 4 {#lie-vii-s2-prop-4-cor-4 .statement tag=00TV}

*Soient g une algèbre de Lie, h une sous-algèbre de Cartan de g, a une sous-algèbre de g contenant h.*
(i) *a est égale à son normalisateur dans g.*
(ii) *Supposons k = \mathbf{R} ou \mathbf{C} ; soient G un groupe de Lie d’algèbre de Lie g, A le sous-groupe intégral de G d’algèbre de Lie a. Alors A est un sous-groupe de Lie de G, et c’est la composante neutre du normalisateur de A dans G.*
Soit n le normalisateur de a dans g. Comme h est une sous-algèbre de Cartan de n (exemple 3), \{0\} est une sous-algèbre de Cartan de n/a (cor. 2), donc est égal à son normalisateur dans n/a; autrement dit, n = a. L’assertion (ii) résulte de (i) et de III, § 9, n°4, cor. de la prop. 11.

#### Corollaire 5 {#lie-vii-s2-prop-4-cor-5 .statement tag=00TW}

*Soient g une algèbre de Lie, E une partie de g. Faisons opérer E dans g par la représentation adjointe. Pour que E soit une sous-algèbre de Cartan de g, il faut et il suffit que E = g^0(E).*
La condition est nécessaire (prop. 4). Supposons maintenant que $E = g^0(E)$. D’après la prop. 2 (ii) du § 1, n° 1, E est alors une sous-algèbre de g. Si $x \in E$, $\mathrm{ad}_E x$ est nilpotent puisque $E \subset g^0(E)$; donc l’algèbre E est nilpotente. Alors E est une sous-algèbre de Cartan d’après la prop. 4.

#### Corollaire 6 {#lie-vii-s2-prop-4-cor-6 .statement tag=00TX}

*Soient g une algèbre de Lie, k_0 un sous-corps de k tel que [k:k_0] < + \infty, g_0 l’algèbre de Lie déduite de g par restriction à k_0 du corps des scalaires. Soit h une partie de g. Pour que $\mathfrak{h}$ soit une sous-algèbre de Cartan de $\mathfrak{g}$, il faut et il suffit que $\mathfrak{h}$ soit une sous-algèbre de Cartan de $\mathfrak{g}_0$.

Cela résulte du cor. 5, car la condition $\mathfrak{h} = \mathfrak{g}^0(\mathfrak{h})$ ne fait pas intervenir le corps de base.

#### Proposition 5 {#lie-vii-s2-prop-5 .statement tag=00TY}

Soient $\mathfrak{g}$ une algèbre de Lie, $c$ son centre, $\mathfrak{h}$ un sous-espace vectoriel de $\mathfrak{g}$. Pour que $\mathfrak{h}$ soit une sous-algèbre de Cartan de $\mathfrak{g}$, il faut et il suffit que $\mathfrak{h}$ contienne $c$ et que $\mathfrak{h}/c$ soit une sous-algèbre de Cartan de $\mathfrak{g}/c$.

Supposons que $\mathfrak{h}$ soit une sous-algèbre de Cartan de $\mathfrak{g}$. Puisque $[c, \mathfrak{g}] \subset \mathfrak{h}$, on a $c \subset \mathfrak{h}$. D'autre part, $\mathfrak{h}/c$ est une sous-algèbre de Cartan de $\mathfrak{g}/c$ d'après le cor. 2 de la prop. 4.

Supposons que $\mathfrak{h} \supset c$ et que $\mathfrak{h}/c$ soit une sous-algèbre de Cartan de $\mathfrak{g}/c$. Soit $f$ le morphisme canonique de $\mathfrak{g}$ sur $\mathfrak{g}/c$. L'algèbre $\mathfrak{h}$, qui est extension centrale de $\mathfrak{h}/c$, est nilpotente. Soit $n$ le normalisateur de $\mathfrak{h}$ dans $\mathfrak{g}$. Si $x \in n$, on a $[f(x), \mathfrak{h}/c] \subset \mathfrak{h}/c$, donc $f(x) \in \mathfrak{h}/c$, donc $x \in \mathfrak{h}$. Cela prouve que $\mathfrak{h}$ est une sous-algèbre de Cartan de $\mathfrak{g}$.

#### Corollaire {#lie-vii-s2-n1-cor-1 .statement tag=00TZ}

Soit $\mathcal{C}_{\infty} \mathfrak{g}$ la réunion de la série centrale ascendante de l'algèbre de Lie $g$ (I, § 1, no 6). Les sous-algèbres de Cartan de $\mathfrak{g}$ sont les images réciproques des sous-algèbres de Cartan de $\mathfrak{g}/\mathcal{C}_{\infty} \mathfrak{g}$.

En effet, le centre de $\mathfrak{g}/\mathcal{C}_i \mathfrak{g}$ est $\mathcal{C}_{i+1} \mathfrak{g}/\mathcal{C}_i \mathfrak{g}$, et le corollaire se déduit de la prop. 5 par une récurrence immédiate.

#### Remarque {#lie-vii-s2-n1-rem-1 .statement tag=00U0}

$\mathcal{C}_{\infty} \mathfrak{g}$ est le plus petit idéal $n$ de $\mathfrak{g}$ tel que le centre de $\mathfrak{g}/n$ soit nul; c'est un idéal caractéristique et nilpotent de $\mathfrak{g}$.

### 2. Eléments réguliers d'une algèbre de Lie

[Rappelons que désormais $k$ est supposé infini.]

Soit $\mathfrak{g}$ une algèbre de Lie de dimension $n$. Si $x \in \mathfrak{g}$, écrivons le polynôme caractéristique de $\mathrm{ad}\, x$ sous la forme

$$
\det(T - \mathrm{ad}\, x) = \sum_{i=0}^{n} a_i(x) T^i, \quad \text{avec} \quad a_i(x) \in k.
$$

On a $a_i(x) = (-1)^{n-i} \operatorname{Tr} \left( \wedge^{n-i} \mathrm{ad}\, x \right)$, cf. A, III, p. 107. Ceci montre que $x \mapsto a_i(x)$ est une application polynomiale homogène de degré $n - i$ de $\mathfrak{g}$ dans $k$ (A, IV, § 5, no 9).

#### Remarque 1 {#lie-vii-s2-n2-rem-1 .statement tag=00U1}

Si $\mathfrak{g} \neq \{0\}$, on a $a_0 = 0$ car $(\mathrm{ad}\, x)(x) = 0$ pour tout $x \in \mathfrak{g}$.

#### Remarque 2 {#lie-vii-s2-n2-rem-2 .statement tag=00U2}

Soit $k'$ une extension de $k$. Ecrivons $\det(T - \mathrm{ad}\, x') = \sum_{i=0}^{n} a'_i(x') T^i$ pour $x' \in \mathfrak{g} \otimes_k k'$. Alors $a'_i|_{\mathfrak{g}} = a_i$ pour tout $i$.

#### Définition 2 {#lie-vii-s2-def-2 .statement tag=00U3}

On appelle rang de $g$ et on note $\mathrm{rg}(g)$ le plus petit entier $l$ tel que $a_l \neq 0$. Un élément $x$ de $g$ est dit régulier si $a_l(x) \neq 0$.

Pour tout $x \in g$, on a donc $\mathrm{rg}(g) \leqslant \dim g^0(x)$, et l'égalité a lieu si et seulement si $x$ est régulier.

L'ensemble des éléments réguliers est ouvert et dense dans $g$ pour la topologie de Zariski (App. I).

#### Exemple 1 {#lie-vii-s2-n2-exa-1 .statement tag=00U4}

Si $g$ est nilpotente, on a $\mathrm{rg}(g) = \dim g$ et tous les éléments de $g$ sont réguliers.

#### Exemple 2 {#lie-vii-s2-n2-exa-2 .statement tag=00U5}

Soit $g = \mathfrak{sl}(2, k)$. Si $x = \begin{pmatrix} \gamma & \alpha \\ \beta & -\gamma \end{pmatrix} \in g$, un calcul facile donne
$$
\det(T - \operatorname{ad} x) = T^3 - 4(\alpha \beta + \gamma^2)T.
$$
Si la caractéristique de $k$ est $\neq 2$, alors $\mathrm{rg}(g) = 1$ et les éléments réguliers sont les $x$ tels que $\alpha \beta + \gamma^2 \neq 0$.

#### Exemple 3 {#lie-vii-s2-n2-exa-3 .statement tag=00U6}

Soient $V$ un espace vectoriel de dimension finie $n$, et $g = \mathfrak{gl}(V)$. Soit $\bar{k}$ une clôture algébrique de $k$. Soient $x \in g$, et $\lambda_1, \ldots, \lambda_n$ les racines dans $\bar{k}$ du polynôme caractéristique de $x$ (chaque racine étant écrite un nombre de fois égal à sa multiplicité). L'isomorphisme canonique de $V^* \otimes V$ sur $g$ est compatible avec les structures de $g$-module de ces deux espaces, autrement dit transforme $1 \otimes x - {}^t x \otimes 1$ en $\operatorname{ad} x$ (I, § 3, no 3, prop. 4). Compte tenu du § 1, prop. 4 (i), on en déduit que les racines du polynôme caractéristique de $\operatorname{ad} x$ sont les $\lambda_i - \lambda_j$ pour $1 \leq i \leq n, 1 \leq j \leq n$ (chaque racine étant écrite un nombre de fois égal à sa multiplicité). Le rang de $g$ est donc $n$ et, pour que $x$ soit régulier, il faut et il suffit que chaque $\lambda_i$ soit racine simple du polynôme caractéristique de $x$.

#### Proposition 6 {#lie-vii-s2-prop-6 .statement tag=00U7}

Soient $g$ une algèbre de Lie, $k'$ une extension de $k$, et $g' = g \otimes_k k'$.
(i) Pour qu'un élément $x$ de $g$ soit régulier dans $g$, il faut et il suffit que $x \otimes 1$ soit régulier dans $g'$.
(ii) On a $\mathrm{rg}(g) = \mathrm{rg}(g')$.
Cela résulte de la remarque 2.

#### Proposition 7 {#lie-vii-s2-prop-7 .statement tag=01IY}

Soient $(g_i)_{i \in I}$ une famille finie d'algèbres de Lie, et $g = \prod_{i \in I} g_i$.
(i) Pour qu'un élément $(x_i)_{i \in I}$ de $g$ soit régulier dans $g$, il faut et il suffit que, pour tout $i \in I$, $x_i$ soit régulier dans $g_i$.
(ii) On a $\mathrm{rg}(g) = \sum_{i \in I} \mathrm{rg}(g_i)$.
En effet, pour tout $x = (x_i)_{i \in I} \in g$, le polynôme caractéristique de $\operatorname{ad}_g x$ est le produit des polynômes caractéristiques des $\operatorname{ad}_{g_i} x_i$.

#### Proposition 8 {#lie-vii-s2-prop-8 .statement tag=00U8}

Soit $f : g \to g'$ un homomorphisme surjectif d'algèbres de Lie.
(i) Si $x$ est un élément régulier de $g$, $f(x)$ est régulier dans $g'$. La réciproque est vraie si $\mathrm{Ker}\, f$ est contenu dans le centre de $g$.

(ii) *On a* $\mathrm{rg}(g) \geqslant \mathrm{rg}(g')$.

Posons $\mathrm{rg}(g) = r, \mathrm{rg}(g') = r'$. Soit $x \in g$. Les polynômes caractéristiques de $\mathrm{ad}\,x, \mathrm{ad}\,f(x)$ et $\mathrm{ad}\,x|\mathrm{Ker}\,f$ sont de la forme
$$
\begin{align*}
P(T) &= T^n + a_{n-1}(x)T^{n-1} + \cdots + a_r(x)T^r, \\
Q(T) &= T^{n'} + b_{n'-1}(x)T^{n'-1} + \cdots + b_{r'}(x)T^{r'}, \\
R(T) &= T^{n''} + c_{n''-1}(x)T^{n''-1} + \cdots + c_{r''}(x)T^{r''},
\end{align*}
$$
où les $a_i, b_i, c_i$ sont des fonctions polynomiales sur $g$, avec $a_r \neq 0, b_{r'} \neq 0, c_{r''} \neq 0$. On a $P = QR$, donc $r = r' + r''$ et $a_r(x) = b_{r'}(x)c_{r''}(x)$, ce qui prouve (ii) et la première assertion de (i). Si $\mathrm{Ker}\,f$ est contenu dans le centre de $g$, on a $R(T) = T^{n''}$, donc $a_r(x) = b_{r'}(x)$, d'où la deuxième assertion de (i).

#### Corollaire {#lie-vii-s2-n2-cor-1 .statement tag=00U9}

*Soit* $\mathcal{C}_n g$ (*n \geqslant 0*) *un terme de la série centrale ascendante de* $g$ *(I, § 1, n° 6)*. *Les éléments réguliers de* $g$ *sont ceux dont l’image dans* $g/\mathcal{C}_n g$ *est régulière*.

#### Proposition 9 {#lie-vii-s2-prop-9 .statement tag=00UA}

*Soient* $g$ *une algèbre de Lie,* $g'$ *une sous-algèbre de* $g$. *Tout élément de* $g'$ *régulier dans* $g$ *est régulier dans* $g'$.

Pour $x \in g'$, $\mathrm{ad}_g x$ admet $\mathrm{ad}_{g'} x$ pour restriction à $g'$, et définit par passage au quotient un endomorphisme $u(x)$ de l’espace vectoriel $g/g'$. Soit $d_0(x)$ (resp. $d_1(x)$) la dimension du nilspace de $\mathrm{ad}_{g'} x$ (resp. de $u(x)$), et soit $c_0$ (resp. $c_1$) le minimum de $d_0(x)$ (resp. $d_1(x)$) quand $x$ parcourt $g'$. Il existe des applications polynomiales non nulles $p_0, p_1$ de $g'$ dans $k$ telles que
$$
d_0(x) = c_0 \Leftrightarrow p_0(x) \neq 0, \qquad d_1(x) = c_1 \Leftrightarrow p_1(x) \neq 0.
$$
Comme $k$ est infini, l’ensemble $S$ des $x \in g'$ tels que $d_0(x) = c_0$ et $d_1(x) = c_1$ est non vide. Tout élément de $S$ est régulier dans $g'$. D’autre part, $S$ est l’ensemble des éléments de $g'$ tels que le nilspace de $\mathrm{ad}_g x$ soit de dimension minimum, et contient donc tout élément de $g'$ qui est régulier dans $g$.

#### Remarque 3 {#lie-vii-s2-n2-rem-3 .statement tag=00UB}

Il n’existe pas nécessairement d’élément de $g'$ régulier dans $g$. S’il en existe au moins un, l’ensemble de ces éléments n’est autre que l’ensemble noté $S$ dans la démonstration ci-dessus.

### 3. Sous-algèbres de Cartan et éléments réguliers

#### Théorème 1 {#lie-vii-s2-thm-1 .statement tag=00UC}

*Soit* $g$ *une algèbre de Lie*.
(i) *Si* $x$ *est un élément régulier de* $g$, $g^0(x)$ *est une sous-algèbre de Cartan de* $g$.
(ii) *Si* $\mathfrak{h}$ *est une sous-algèbre nilpotente maximale de* $g$, *et si* $x \in \mathfrak{h}$ *est régulier dans* $g$, *alors* $\mathfrak{h} = g^0(x)$.
(iii) *Si* $\mathfrak{h}$ *est une sous-algèbre de Cartan de* $g$, *on a* $\dim(\mathfrak{h}) \geqslant \mathrm{rg}(g)$.
(iv) *Les sous-algèbres de Cartan de* $g$ *de dimension* $\mathrm{rg}(g)$ *sont les* $g^0(x)$ *où* $x$ *est un élément régulier*.

Soit $x$ un élément régulier de $g$ et soit $h = g^0(x)$. On a évidemment $h^0(x) = h$. Comme $x$ est régulier dans $h$ (prop. 9), on a $\mathrm{rg}(h) = \dim(h)$, de sorte que $h$ est nilpotente. D’autre part, $h = g^0(x) \supset g^0(h) \supset h$, donc $h = g^0(h)$ est une sous-algèbre de Cartan de $g$ (prop. 4). Cela prouve (i).

Si $h$ est une sous-algèbre nilpotente maximale de $g$, et si $x \in h$ est régulier dans $g$, on a $h \subset g^0(x)$, et $g^0(x)$ est nilpotente d’après (i), donc $h = g^0(x)$, ce qui établit (ii).

Si $h$ est une sous-algèbre de Cartan de $g$, il existe $x \in h$ tel que $h = g^0(x)$ (cor. 1 de la prop. 4), d’où $\dim(h) \geq \mathrm{rg}(g)$, ce qui prouve (iii). Si en outre $\dim(h) = \mathrm{rg}(g)$, $x$ est régulier. Enfin, si $x'$ est régulier dans $g$, $g^0(x')$ est une sous-algèbre de Cartan d’après (i), évidemment de dimension $\mathrm{rg}(g)$. Cela prouve (iv).

Nous verrons au § 3, th. 2, que, lorsque $k$ est de caractéristique zéro, toutes les sous-algèbres de Cartan de $g$ ont pour dimension $\mathrm{rg}(g)$.

#### Corollaire 1 {#lie-vii-s2-thm-1-cor-1 .statement tag=00UD}

Toute algèbre de Lie $g$ possède des sous-algèbres de Cartan, et le rang de $g$ est la dimension minimum des sous-algèbres de Cartan.

#### Corollaire 2 {#lie-vii-s2-thm-1-cor-2 .statement tag=00UE}

Soit $f : g \to g'$ un homomorphisme surjectif d’algèbres de Lie. Si $h'$ est une sous-algèbre de Cartan de $g'$, il existe une sous-algèbre de Cartan $h$ de $g$ telle que $h' = f(h)$.

Soit $a = f^{-1}(h')$. D’après le cor. 1, $a$ possède une sous-algèbre de Cartan $h$. D’après le cor. 2 de la prop. 4, on a $f(h) = h'$. Montrons que $h$ est une sous-algèbre de Cartan de $g$. Soit $n$ le normalisateur de $h$ dans $g$. Il s’agit de prouver que $h = n$. Si $x \in n, f(x)$ appartient au normalisateur de $h'$ dans $g'$, donc $f(x) \in h'$ et $x \in a$; mais $h$ est son propre normalisateur dans $a$, donc $x \in h$.

#### Corollaire 3 {#lie-vii-s2-thm-1-cor-3 .statement tag=00UF}

Toute algèbre de Lie $g$ est somme de ses sous-algèbres de Cartan.

La somme $s$ des sous-algèbres de Cartan de $g$ contient l’ensemble des éléments réguliers de $g$ (th. 1 (i)). Comme cet ensemble est dense dans $g$ pour la topologie de Zariski, on a $s = g$.

#### Proposition 10 {#lie-vii-s2-prop-10 .statement tag=00UG}

Soient $g$ une algèbre de Lie, $a$ une sous-algèbre commutative de $g$ et $c$ le commutant de $a$ dans $g$. On suppose que $\mathrm{ad}_g x$ est semi-simple pour tout $x \in a$. Alors les sous-algèbres de Cartan de $c$ sont les sous-algèbres de Cartan de $g$ contenant $a$.

Soit $h$ une sous-algèbre de Cartan de $c$. Comme $a$ est contenue dans le centre $\delta$ de $c$, on a $a \subset \delta \subset h$ (prop. 5). Soit $n$ le normalisateur de $h$ dans $g$. On a

$$
[a, n] \subset [h, n] \subset h.
$$

Comme les $\mathrm{ad}_g x, x \in a$, sont semi-simples et commutent entre eux, il résulte de A, VIII, § 5, n° 1, qu’il existe un sous-espace vectoriel $\delta$ de $n$ stable par $\mathrm{ad}_g a$ et tel que $n = h \oplus \delta$. On a $[a, \delta] \subset h \cap \delta = 0$, donc $\delta \subset c$. Ainsi, $n$ est le normalisateur de $\mathfrak{h}$ dans $c$, et par suite $n = h$, de sorte que $h$ est une sous-algèbre de Cartan de $g$ contenant $a$.

Inversement, soit $h$ une sous-algèbre de Cartan de $g$ contenant $a$. On a $h = g^0(h) \subset g^0(a)$, et par hypothèse $g_0(a) = g^0(a) = c$. D’où $a \subset h \subset c$ et $h$ est une sous-algèbre de Cartan de $c$ (car égale à son normalisateur dans $g$, donc $a$ fortiori dans $c$).

#### Proposition 11 {#lie-vii-s2-prop-11 .statement tag=00UH}

Soit $n$ une sous-algèbre nilpotente d’une algèbre de Lie $g$. Il existe une sous-algèbre de Cartan de $g$ contenue dans $g^0(n)$.

Posons $a = g^0(n)$. On a $n \subset a$ puisque $n$ est nilpotente. Si $x \in a$, soit $P(x)$ le déterminant de l’endomorphisme de $g/a$ défini par ad $x$. Notons $a'$ l’ensemble des $x \in a$ tels que $P(x) \neq 0$, c’est un ouvert de $a$ pour la topologie de Zariski ; les relations $x \in a'$ et $g^0(x) \subset a$ sont équivalentes. D’après la prop. 7 (ii) du § 1, n° 2, il existe $y \in n$ tel que $g^0(y) = a$, et l’on a $y \in a'$, ce qui montre que $a'$ est non vide. Comme $a'$ est ouvert, son intersection avec l’ensemble des éléments réguliers de $a$ est non vide. Soit $x$ un élément de cette intersection. On a $g^0(x) \subset a$ et $g^0(x)$ est une sous-algèbre de Cartan de $a$, donc est nilpotente. D’autre part, la prop. 10 (i) du § 1, n° 3, montre que $g^0(x)$ est son propre normalisateur dans $g$; c’est donc une sous-algèbre de Cartan de $g$, ce qui achève la démonstration.

### 4. Sous-algèbres de Cartan des algèbres de Lie semi-simples

#### Théorème 2 {#lie-vii-s2-thm-2 .statement tag=00UI}

Supposons $k$ de caractéristique 0. Soient $g$ une algèbre de Lie semi-simple, $h$ une sous-algèbre de Cartan de $g$. Alors $h$ est commutative, et tous ses éléments sont semi-simples dans $g$ (I, § 6, n° 3, déf. 3).

Comme $h = g^0(h)$, $h$ est réductive ($\S$ 1, prop. 11), donc commutative puisque nilpotente. D’autre part, la restriction à $h$ de la représentation adjointe de $g$ est semi-simple (*loc. cit.*), donc les éléments de $h$ sont semi-simples dans $g$ (A, VIII, $\S$ 5, n° 1).

#### Corollaire 1 {#lie-vii-s2-thm-2-cor-1 .statement tag=00UJ}

Si $x \in h$ et $y \in g^\lambda(h)$, on a $[x, y] = \lambda(x)y$.

En effet, puisque ad $x$ est semi-simple, on a $g^{\lambda(x)}(x) = g_{\lambda(x)}(x)$.

#### Corollaire 2 {#lie-vii-s2-thm-2-cor-2 .statement tag=00UK}

Tout élément régulier de $g$ est semi-simple.

En effet, un tel élément appartient à une sous-algèbre de Cartan (n° 3, th. 1 (i)).

#### Corollaire 3 {#lie-vii-s2-thm-2-cor-3 .statement tag=00UL}

Soit $h$ une sous-algèbre de Cartan d’une algèbre de Lie réductive $g$.
a) $h$ est commutative.
b) Si $\rho$ est une représentation semi-simple de dimension finie de $g$, les éléments de $\rho(h)$ sont semi-simples.

Soient c le centre de g, et s son algèbre dérivée. On a $g = c \times s$, d'où $h = c \times h'$, où $h'$ est une sous-algèbre de Cartan de s (prop. 2). Vu le th. 2, $h'$ est commutative, et il en est de même de $h$. De plus, $\rho(h')$ est formée d’éléments semi-simples et il en est de même de $\rho(c)$ (I, § 6, n° 5, th. 4); l’assertion (b) en résulte.

## EXERCICES {#lie-vii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
