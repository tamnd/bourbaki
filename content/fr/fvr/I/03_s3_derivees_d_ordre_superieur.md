---
book: fvr
book_title: Functions of a Real Variable
chapter: I
chapter_title: DÉRIVÉES
section: 3
section_title: Dérivées d'ordre supérieur
lang: fr
source: fvr-i-vii-fr
book_pages: FVR I.28-FVR I.31, FVR I.46-FVR I.51
pdf_pages: 0026-0029, 0044-0049
extraction: ocr
subsections:
    - "no": 1
      title: Dérivées d’ordre $n$
      page: 28
      pdf_page: 26
    - "no": 2
      title: Formule de Taylor
      page: 29
      pdf_page: 27
statements: 7
exercises: 18
content_sha256: 06cc441886cea46c47dd5f5659be99ff22d01a6d0f65be5bebb20aab2a0bd8ab
---

## § 3. DÉRIVÉES D’ORDRE SUPÉRIEUR

### 1. Dérivées d’ordre $n$

Soit $\mathbf{f}$ une fonction vectorielle d’une variable réelle, définie, continue et dérivable dans un intervalle $I$. Si la dérivée $\mathbf{f}'$ existe dans un voisinage (par rapport à $I$) d’un point $x_0 \in I$, et est dérivable au point $x_0$, sa dérivée est appelée la dérivée seconde de $\mathbf{f}$ au point $x_0$, et se note $\mathbf{f}''(x_0)$ ou $D^2\mathbf{f}(x_0)$. Si cette dérivée seconde existe en tout point de $I$ (ce qui implique que $\mathbf{f}'$ existe et est continue dans $I$), $x \mapsto \mathbf{f}''(x)$ est une fonction vectorielle qu’on désigne par la notation $\mathbf{f}''$ ou $D^2\mathbf{f}$.

Par récurrence, on définit de même la dérivée $n$-ème (ou dérivée d’ordre $n$) de $\mathbf{f}$, qu’on note $\mathbf{f}^{(n)}$ ou $D^n\mathbf{f}$; par définition, elle a pour valeur au point $x_0 \in I$ la dérivée de la fonction $\mathbf{f}^{(n-1)}$ au point $x_0$: cette définition suppose donc l’existence de toutes les dérivées $\mathbf{f}^{(k)}$ d’ordre $k \leq n - 1$ dans un voisinage de $x_0$ par rapport à $I$, et la dérivabilité de $\mathbf{f}^{(n-1)}$ au point $x_0$.

On dira que $\mathbf{f}$ est $n$ fois dérivable au point $x_0$ (resp. dans un intervalle) si elle admet une dérivée $n$-ème en ce point (resp. dans cet intervalle). On dit que $\mathbf{f}$ est indéfiniment dérivable dans $I$ si, pour tout entier $n > 0$, elle admet une dérivée d’ordre $n$ dans $I$.

Par récurrence sur $m$, on voit que

$$
D^m(D^n\mathbf{f}) = D^{m+n}\mathbf{f}.
$$

De façon précise, lorsque l’un des deux membres de (1) est défini, l’autre est défini et lui est égal.

#### Proposition 1 {#fvr-i-s3-prop-1 .statement}

L’ensemble des fonctions vectorielles définies dans un intervalle $I \subset \mathbf{R}$, prenant leurs valeurs dans un même espace vectoriel topologique $E$, et admettant une dérivée $n$-ème dans $I$, est un espace vectoriel sur $\mathbf{R}$, et $\mathbf{f} \mapsto D^n\mathbf{f}$ est une application linéaire de cet espace dans l’espace vectoriel des applications de $I$ dans $E$.

On démontre en effet par récurrence sur $n$ les formules

$$
D^n(\mathbf{f} + \mathbf{g}) = D^n\mathbf{f} + D^n\mathbf{g}
$$
$$
D^n(a\mathbf{f}) = D^n\mathbf{f} \cdot a
$$

lorsque $\mathbf{f}$ et $\mathbf{g}$ ont une dérivée $n$-ème dans $I$ ($a$ constante).

**Proposition 2** (« formule de Leibniz »). — Soient $E, F, G$ trois espaces vectoriels topologiques sur $\mathbf{R}$, $(\mathbf{x}, \mathbf{y}) \mapsto [\mathbf{x}, \mathbf{y}]$ une application bilinéaire continue de $E \times F$ dans $G$. Si $\mathbf{f}$ (resp. $\mathbf{g}$) est définie dans un intervalle $I \subset \mathbf{R}$, prend ses valeurs dans $E$ (resp. $F$) et admet une dérivée n-ème dans I, [f.g] admet dans I une dérivée n-ème donnée par la formule

(4) $D^n[f.g] = [f^{(n)}.g] + \binom{n}{1} [f^{(n-1)}.g'] + \ldots$
$$
+ \binom{n}{p} [f^{(n-p)}.g^{(p)}] + \ldots + [f.g^{(n)}].
$$

La formule (4) se démontre encore par récurrence sur n (compte tenu de la relation $\binom{n}{p} = \binom{n-1}{p} + \binom{n-1}{p-1}$ entre coefficients binomiaux).

On vérifie de même la formule suivante (où les hypothèses sont les mêmes que dans la prop. 2):

(5) $[f^{(n)}.g] + (-1)^{n-1}[f.g^{(n)}]$
$$
= D([f^{(n-1)}.g] - [f^{(n-2)}.g']) + \ldots + (-1)^{n-1} [f.g^{(n-1)}].
$$

Les propositions précédentes ont été énoncées pour des fonctions n fois dérivables dans un intervalle; nous laissons au lecteur le soin d’énoncer les propositions analogues pour les fonctions n fois dérivables en un point.

### 2. Formule de Taylor

Soit f une fonction vectorielle définie dans un intervalle I ⊂ ℝ, à valeurs dans un espace normé E sur ℝ; dire que f a une dérivée en un point a ∈ I signifie que l’on a

(6) $\lim_{x \to a,\ x \in I,\ x \neq a} \frac{f(x) - f(a) - f'(a)(x-a)}{x-a} = 0$

autrement dit, que f est « approximativement égale » à la fonction linéaire $f(a) + f'(a)(x-a)$ au voisinage de a (cf. chap. V, où cette notion est développée de façon générale). Nous allons voir que l’existence de la dérivée d’ordre n de f au point a entraîne de la même manière que f est « approximativement égale » à un polynôme en x, de degré n, à coefficients dans E (TG, X, p. 39) au voisinage de a. De façon précise:

#### Théorème 1 {#fvr-i-s3-thm-1 .statement}

Si la fonction f admet une dérivée n-ème au point a, on a

(7) $\lim_{x \to a,\ x \in I,\ x \neq a} \frac{f(x) - f(a) - f'(a)\frac{(x-a)}{1!} - \ldots - f^{(n)}(a)\frac{(x-a)^n}{n!}}{(x-a)^n} = 0.$

Procédons par récurrence sur n. Le théorème est vrai pour $n = 1$. Pour $n$

quelconque, on peut, d’après l’hypothèse de récurrence, l’appliquer à la dérivée $f'$ de $f$: pour tout $\varepsilon > 0$, il existe donc $h > 0$ tel que, si on pose
$$
g(x) = f(x) - f(a) - f'(a) \frac{(x-a)}{1!} - f''(a) \frac{(x-a)^2}{2!} - \ldots - f^{(n)}(a) \frac{(x-a)^n}{n!}
$$
on ait, pour $|y-a| \leq h$ et $y \in I$
$$
\|g'(y)\| = \left\| f'(y) - f'(a) - f''(a) \frac{(y-a)}{1!} - \ldots \right. \\
\left. - f^{(n)}(a) \frac{(y-a)^{n-1}}{(n-1)!} \right\| \leq \varepsilon |y-a|^{n-1}.
$$

Appliquons le th. des accroissements finis (I, p. 22, th. 2) dans l’intervalle d’extrémités $a, x$ (avec $|x-a| \leq h$) à la fonction vectorielle $g$ et à la fonction numérique croissante égale à $\varepsilon |y-a|^n/n$ si $x > a$, à $-\varepsilon |y-a|^n/n$ si $x < a$; il vient $\|g(x)\| \leq \varepsilon |x-a|^n/n$, ce qui démontre le théorème.

On peut donc écrire
$$
f(x) = f(a) + f'(a) \frac{(x-a)}{1!} + f''(a) \frac{(x-a)^2}{2!} + \ldots \\
+ f^{(n)}(a) \frac{(x-a)^n}{n!} + u(x) \frac{(x-a)^n}{n!}
$$
où $u(x)$ tend vers 0 lorsque $x$ tend vers $a$ en restant dans $I$; cette formule est dite *formule de Taylor d’ordre n*, relative au point $a$, et le second membre de (8) est appelé le *développement de Taylor d’ordre n* de la fonction $f$ au point $a$. Le dernier terme $r_n(z) = u(x)(x-a)^n/n!$ est appelé le *reste* de la formule de Taylor d’ordre $n$.

Lorsque $f$ admet une *dérivée d’ordre n + 1* dans $I$, on peut avoir en fonction de cette dérivée $(n+1)$-ème une majoration de $\|r_n(x)\|$ valable dans $I$ tout entier, et non seulement dans un voisinage non précisé de $a$:

#### Proposition 3 {#fvr-i-s3-prop-3 .statement}

*Si $\|f^{(n+1)}(x)\| \leq M$ dans $I$, on a*
$$
\|r_n(x)\| \leq M \frac{|x-a|^{n+1}}{(n+1)!}
$$
*dans I*.

En effet, la formule est vraie pour $n = 0$, d’après I, p. 23, th. 2. Démontrons-la par récurrence sur $n$; d’après l’hypothèse de récurrence appliquée à $f'$, on a
$$
\|r'_n(y)\| \leq M \frac{|y-a|^n}{n!}
$$
d’où la formule (9) par application du th. des accroissements finis (I, p. 23, th. 2).

#### Corollaire {#fvr-i-s3-n2-cor-1 .statement}

Si f est une fonction numérique finie admettant une dérivée (n + 1)-ème dans I, et si m $\leq f^{(n+1)}(x) \leq M$ dans I, on a, pour tout $x \geq a$ dans I

$$
m \frac{(x-a)^{n+1}}{(n+1)!} \leq r_n(x) \leq M \frac{(x-a)^{n+1}}{(n+1)!}
$$

le second membre ne pouvant être égal au premier (resp. au troisième) que si $f^{(n+1)}$ est constante et égale à m (resp. M) dans l’intervalle $[a, x]$.

La démonstration se fait de la même manière, mais en appliquant le th. 1 de I, p. 17.

#### Remarque 1 {#fvr-i-s3-n2-rem-1 .statement}

On a déjà noté, au cours de la démonstration du th. 1, que si $\mathbf{f}$ admet une dérivée n-ème dans I, et si

$$
\mathbf{f}(x) = a_0 + a_1(x-a) + a_2(x-a)^2 + \ldots + a_n(x-a)^n + r_n(x)
$$

est son développement de Taylor d’ordre n au point a, le développement de Taylor d’ordre $n-1$ de $\mathbf{f}'$ au point a est

$$
\mathbf{f}'(x) = a_1 + 2a_2(x-a) + \ldots + na_n(x-a)^{n-1} + r'_n(x).
$$

On dit qu’il s’obtient en *dérivant terme à terme* le développement (11) de $\mathbf{f}$.

#### Remarque 2 {#fvr-i-s3-n2-rem-2 .statement}

Dans les mêmes hypothèses, les coefficients $a_i$ de (11) sont déterminés par récurrence par les relations

$$
a_0 = \mathbf{f}(a)
$$
$$
a_1 = \lim_{x \to a} \frac{\mathbf{f}(x) - \mathbf{f}(a)}{x-a}
$$
$$
a_2 = \lim_{x \to a} \frac{\mathbf{f}(x) - \mathbf{f}(a) - a_1(x-a)}{(x-a)^2}
$$
$$
\ldots
$$
$$
a_n = \lim_{x \to a} \frac{\mathbf{f}(x) - \mathbf{f}(a) - a_1(x-a) - \ldots - a_{n-1}(x-a)^{n-1}}{(x-a)^n}.
$$

Dans le cas où $a = 0$, on conclut de là en particulier que, si $\mathbf{f}(x^p)$ ($p$ entier > 0) admet une dérivée d’ordre $pn$ dans un voisinage de 0, le développement de Taylor d’ordre $pn$ de cette fonction n’est autre que

$$
\mathbf{f}(x^p) = a_0 + a_1 x^p + a_2 x^{2p} + \ldots + a_n x^{np} + r_n(x^p)
$$

$r_n(x^p)$ étant le reste du développement (cf. V, p. 11).

#### Remarque 3 {#fvr-i-s3-n2-rem-3 .statement}

La définition de la dérivée d’ordre n et les résultats qui précèdent se généralisent de façon immédiate aux fonctions d’une variable complexe; nous n’insistons pas davantage ici sur cette question, qui sera reprise en détail dans un Livre ultérieur de cet ouvrage.

## EXERCICES {#fvr-i-s3-exercises}

See the [exercises for § 3](exercises/s3/).
