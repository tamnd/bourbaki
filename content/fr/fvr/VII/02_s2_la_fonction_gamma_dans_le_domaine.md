---
book: fvr
book_title: Functions of a Real Variable
chapter: VII
chapter_title: LA FONCTION GAMMA
section: 2
section_title: La fonction gamma dans le domaine complexe
lang: fr
source: fvr-i-vii-fr
book_pages: FVR VII.21-FVR VII.22
pdf_pages: 0301-0310, 0312-0313
extraction: ocr
subsections:
    - "no": 1
      title: Prolongement à $\mathbf{C}$ de la fonction gamma
      page: 10
      pdf_page: 301
    - "no": 2
      title: La relation des compléments et la formule de multiplication de Legendre-Gauss
      page: 12
      pdf_page: 303
    - "no": 3
      title: Le développement de Stirling
      page: 15
      pdf_page: 306
statements: 7
exercises: 6
content_sha256: cd4a974777c72198bdedb8ec97eb2bed5ff208ea9b408fe4cca6e704ca4f5a7e
---

## § 2. LA FONCTION GAMMA DANS LE DOMAINE COMPLEXE

### 1. Prolongement à $\mathbf{C}$ de la fonction gamma

Reprenons la formule de Weierstrass qui donne l’expression de $1/\Gamma(x)$ pour tout $x$ réel
$$
\frac{1}{\Gamma(x)} = x e^{x \gamma} \prod_{n=1}^\infty \left( 1 + \frac{x}{n} \right) e^{-x/n}
$$
et considérons le produit infini de terme général $\left( 1 + \frac{z}{n} \right) e^{-z/n}$, pour $z$ complexe quelconque. On peut écrire $e^{-z/n} = 1 - \frac{z}{n} + h(z)$, avec $|h(z)| \leq \frac{|z|^2}{2n^2} e^{|z/n|}$ (III, p. 16, formule (8)), d’où

$$
\left(1 + \frac{z}{n}\right) e^{-z/n} = 1 + v_n(z)
$$

avec $|v_n(z)| \leq \frac{|z|^2}{n^2} (1 + \frac{e^{|z|}}{2} (1 + |z|))$; le produit infini considéré est donc absolument et uniformément convergent dans toute partie compacte de $\mathbf{C}$; en outre, sa valeur n’est nulle que pour les points $z = -n$ (TG, IX, p. 80, corollaire). En raison de la formule (1) de VII, p. 10, on pose, pour tout $z$ complexe

$$
\frac{1}{\Gamma(z)} = z e^{z/2} \prod_{n=1}^{\infty} \left(1 + \frac{z}{n}\right) e^{-z/n}.
$$

La fonction $\Gamma(z)$ est ainsi définie pour tout point $z \in \mathbf{C}$ distinct des points $-n$ ($n \in \mathbf{N}$); elle est continue dans cet ensemble, et au voisinage de $-n$, on a $(z + n)\Gamma(z) \sim \frac{(-1)^n}{n!}$. La formule (2) montre que l’on a $\Gamma(z) = \overline{\Gamma(\overline{z})}$ pour tout $z$ distinct d’un entier négatif.

Le raisonnement qui permet de passer de la formule de Gauss (VII, p. 3, formule (8)) à la formule de Weierstrass, repris en sens inverse, s’applique aussi pour $z$ complexe, et montre que, pour tout $z \neq -n$ ($n \in \mathbf{N}$), on a

$$
\Gamma(z) = \lim_{n \to \infty} \frac{n^z \cdot n!}{z(z+1)\ldots(z+n)}
$$

en convenant de poser $n^z = e^{z \log n}$. Comme on a

$$
\frac{n^{z+1} \cdot n!}{(z+1)(z+2)\ldots(z+n+1)} = z \cdot \frac{n}{n+1+z} \cdot \frac{n^z \cdot n!}{z(z+1)\ldots(z+n)}
$$

on a encore, en passant à la limite, l’équation fonctionnelle fondamentale

$$
\Gamma(z+1) = z \Gamma(z)
$$

pour tout $z \neq -n$ ($n \in \mathbf{N}$).

Soit $p$ un entier $> 0$ quelconque, et $K_p$ le disque ouvert $|z| < p$; pour tout $z \in K_p$ et tout entier $n > p$, $1 + \frac{z}{n}$ n’est pas un nombre réel négatif, donc $\log \left(1 + \frac{z}{n}\right)$ est défini, et il résulte de ce qui précède que la série de terme général $\log \left(1 + \frac{z}{n}\right) - \frac{z}{n}$ ($n > p$) est normalement convergente dans $K_p$; il en est de même des séries obtenues en dérivant un nombre quelconque de fois le terme général, puisqu’on a

$$
\left| \frac{1}{n} - \frac{1}{z+n} \right| \leq \frac{p}{n(n-p)} \quad \text{et} \quad \left| \frac{1}{(z+n)^k} \right| \leq \frac{1}{(n-p)^k} \quad (k > 1)
$$

pour $z \in K_p$ et $n > p$. On voit donc (cf. II, p. 68, Remarque 3) que $\Gamma(z)$ est *indéfiniment dérivable* en tous les points $z \in \mathbf{C}$ distincts des points $-n$, et on a en ces points

$$
\frac{\Gamma'(z)}{\Gamma(z)} = -\gamma - \frac{1}{z} + \sum_{n=1}^{\infty} \left( \frac{1}{n} - \frac{1}{z+n} \right)
$$

$$
D^{k-1}\left( \frac{\Gamma'(z)}{\Gamma(z)} \right) = \sum_{n=0}^{\infty} \frac{(-1)^k(k-1)!}{(z+n)^k} \quad \text{pour } k \geq 2,
$$

les séries des seconds membres de (5) et (6) étant *normalement convergentes* dans tout ensemble compact contenu dans $\mathbf{C}$ et ne contenant aucun entier $\leq 0$. On peut écrire en outre

$$
\log \Gamma(z) \equiv -\gamma z - \log z + \sum_{n=1}^{\infty} \left( \frac{z}{n} - \log \left( 1 + \frac{z}{n} \right) \right) \pmod{2\pi i}
$$

en convenant que lorsqu’un logarithme, dans cette formule, porte sur un nombre réel négatif, il a l’une ou l’autre des deux valeurs limites (différant de $2\pi i$) de $\log z$ en ce point; la série du second membre de (7) est alors normalement convergente dans tout ensemble compact contenu dans $\mathbf{C}$ et ne contenant aucun entier $\leq 0$.

### 2. La relation des compléments et la formule de multiplication de Legendre-Gauss

On tire aussitôt de la formule (2) de VII, p. 11, que, pour tout $z \in \mathbf{C}$

$$
\frac{1}{\Gamma(z)\Gamma(-z)} = -z^2 \prod_{n=1}^{\infty} \left( 1 - \frac{z^2}{n^2} \right).
$$

Or, le développement eulérien de $\sin z$ (VI, p. 18, th. 2) montre que

$$
z \prod_{n=1}^{\infty} \left( 1 - \frac{z^2}{n^2} \right) = \frac{1}{\pi} \sin \pi z;
$$

tenant compte de l’équation fonctionnelle (4) de VII, p. 11, on voit donc que:

#### Proposition 1 {#fvr-vii-s2-prop-1 .statement}

*Pour tout z complexe, on a*

$$
\frac{1}{\Gamma(z)\Gamma(1-z)} = \frac{1}{\pi} \sin \pi z
$$

*(relation des compléments)*.

#### Corollaire {#fvr-vii-s2-n2-cor-1 .statement}

*Pour tout t réel, on a*

$$
|\Gamma(it)| = \sqrt{\frac{\pi}{t \sinh \pi t}} \quad (t \neq 0)
$$

(10) $$|\Gamma(\frac{1}{2} + it)| = \sqrt{\frac{\pi}{\operatorname{ch}\pi t}}.$$

En effet on déduit de (8) que $\Gamma(it)\Gamma(-it) = \frac{i\pi}{t \sin \pi it} = \frac{\pi}{t \operatorname{sh} \pi t}$ et on a $\Gamma(-it) = \overline{\Gamma(it)}$; de même, (8) donne

$$ \Gamma(\frac{1}{2} + it)\Gamma(\frac{1}{2} - it) = \frac{\pi}{\sin\left(\frac{\pi}{2} + \pi it\right)} = \frac{\pi}{\cos \pi it} = \frac{\pi}{\operatorname{ch} \pi t}, $$

et on a

$$ \Gamma(\frac{1}{2} - it) = \overline{\Gamma(\frac{1}{2} + it)}. $$

Soit maintenant $p$ un entier $> 0$ quelconque, et considérons le produit

$$ f(z) = \Gamma\left(\frac{z+1}{p}\right)\Gamma\left(\frac{z+2}{p}\right) \ldots \Gamma\left(\frac{z+p}{p}\right). $$

D’après (3) (VII, p. 11), pour tout $z \neq -n \ (n \in \mathbf{N})$, $f(z)$ est limite du produit

$$ \frac{n^{(z+1)p} n!}{\left(\frac{z+1}{p}\right)\left(\frac{z+1}{p} + 1\right) \ldots \left(\frac{z+1}{p} + n\right)} \cdot \frac{n^{(z+2)p} n!}{\left(\frac{z+2}{p}\right)\left(\frac{z+2}{p} + 1\right) \ldots \left(\frac{z+2}{p} + n\right)} \cdots $$
$$ \frac{n^{(z+p)p} n!}{\left(\frac{z+p}{p}\right)\left(\frac{z+p}{p} + 1\right) \ldots \left(\frac{z+p}{p} + n\right)} = \frac{n^{z+(p+1)/2} p^{(n+1)p} (n!)^p}{(z+1)(z+2) \ldots (z+(n+1)p)} $$

et en particulier $f(0)$ est limite du produit

$$ \frac{n^{(p+1)/2} p^{(n+1)p} (n!)^p}{((n+1)p)!} $$

d’où résulte que $f(z)/f(0)$ est limite de

$$ \frac{n^z ((n+1)p)!}{(z+1)(z+2) \ldots (z+(n+1)p)} $$
$$ = z p^{-z} \left( \frac{n}{n+1} \right)^z \frac{((n+1)p)^z ((n+1)p)!}{z(z+1)(z+2) \ldots (z+(n+1)p)} $$

ce qui, d’après (3) (VII, p. 11), donne

(11) $$ f(z) = f(0) z p^{-z} \Gamma(z). $$

Mais on peut écrire

$$ f(0) = \prod_{k=1}^{p-1} \Gamma\left(\frac{k}{p}\right) = \prod_{k=1}^{p-1} \Gamma\left(1 - \frac{k}{p}\right) = \sqrt{\prod_{k=1}^{p-1} \Gamma\left(\frac{k}{p}\right) \Gamma\left(1 - \frac{k}{p}\right)} $$

puisque $f(0) > 0$; la relation des compléments donne par suite
$$
f(0) = \sqrt{\pi^{p-1} \prod_{k=1}^{p-1} \sin \frac{k\pi}{p}}
$$
et comme le produit du second membre est égal à $p/2^{p-1}$ (VI, p. 15, cor. 1), on voit finalement que:

#### Proposition 2 {#fvr-vii-s2-prop-2 .statement}

*Pour tout nombre complexe z distinct d’un entier $\leq 0$ et pour tout entier $p > 0$, on a*
$$
\Gamma\left(\frac{z}{p}\right) \Gamma\left(\frac{z+1}{p}\right) \ldots \Gamma\left(\frac{z+p-1}{p}\right) = (2\pi)^{(p-1)/2} p^{1-z} \Gamma(z)
$$
(formule de multiplication de Legendre–Gauss).

#### Proposition 3 {#fvr-vii-s2-prop-3 .statement}

*Pour tout nombre réel $x > 0$, on a*
$$
\int_x^{x+1} \log \Gamma(t) \, dt = x(\log x - 1) + \frac{1}{2} \log 2\pi
$$
(intégrale de Raabe).

Démontrons d’abord la formule (13) pour $x = 0$. Comme $\log \Gamma(x) \sim \log \frac{1}{x}$ lorsque $x$ tend vers 0, l’intégrale $\int_0^1 \log \Gamma(x) \, dx$ est convergente. En outre, dans ]0, 1[, la fonction $\log \Gamma(x)$ est décroissante (VII, p. 6); pour tout $\alpha > 0$, on a donc
$$
\frac{1}{n} \sum_{k=1}^q \log \Gamma\left(\frac{k}{n}\right) \leq \int_0^\infty \log \Gamma(x) \, dx,
$$
$q$ étant le plus grand entier tel que $q/n \leq \alpha$. Comme $\int_0^\infty \log \Gamma(x) \, dx$ tend vers 0 avec $\alpha$ et que $\frac{1}{n} \sum_{k=q+1}^n \log \Gamma\left(\frac{k}{n}\right)$ tend vers $\int_\alpha^1 \log \Gamma(x) \, dx$ lorsque $n$ tend vers $+\infty$ (II, p. 7, prop. 5), on a
$$
\int_0^1 \log \Gamma(x) \, dx = \lim_{n \to \infty} \frac{1}{n} \sum_{k=1}^n \log \Gamma\left(\frac{k}{n}\right).
$$
Mais, d’après (12), le second membre de cette formule est limite de
$$
\frac{n-1}{2n} \log 2\pi - \frac{1}{2} \frac{\log n}{n},
$$
d’où
$$
\int_0^1 \log \Gamma(x) \, dx = \frac{1}{2} \log 2\pi.
$$
Remarquons maintenant que, de l’identité
$$
\log \Gamma(x+1) = \log \Gamma(x) + \log x
$$

on déduit, en intégrant, pour $x > 0$

$$
\int_0^x \log \Gamma(t + 1) \, dt = \int_0^x \log \Gamma(t) \, dt + \int_0^x \log t \, dt.
$$

Mais l’intégrale du premier membre est aussi égale à $\int_1^{x+1} \log \Gamma(t) \, dt$. On a donc, d’après (14),

$$
\int_x^{x+1} \log \Gamma(t) \, dt = \int_0^x \log t \, dt + \frac{1}{2} \log 2\pi = x(\log x - 1) + \frac{1}{2} \log 2\pi.
$$

### 3. Le développement de Stirling

Soient $x$ et $y$ deux nombres complexes non situés sur le demi-axe réel négatif; d’après la formule (3) de VII, p. 11, et avec les conventions de VII, p. 12 concernant les logarithmes, $\log \Gamma(x) - \log \Gamma(y)$ est congru modulo $2\pi i$ à la limite de l’expression

(15)
$$
(x - y) \log n + \sum_{k=0}^n (\log (y + k) - \log (x + k)).
$$

Posons $f(t) = \log (y + t) - \log (x + t)$; nous allons appliquer à la fonction $f$ la formule sommatoire d’Euler–Maclaurin (VI, p. 20)

$$
f(0) + f(1) + \cdots + f(n) = \int_0^{n+1} f(t) \, dt - \frac{1}{2}(f(n + 1) - f(0))
$$
$$
+ \sum_{k=1}^p \frac{b_{2k}}{(2k)!} (f^{(2k-1)}(n + 1) - f^{(2k-1)}(0)) + T_p(n)
$$

avec

(16)
$$
|T_p(n)| \leq \frac{4 e^{2\pi}}{(2\pi)^{2p+1}} \int_0^{n+1} |f^{(2p+1)}(u)| \, du.
$$

Comme

$$
f^{(m)}(t) = (-1)^{m-1}(m-1)! \left( \frac{1}{(y + t)^m} - \frac{1}{(x + t)^m} \right),
$$

$f^{(2k-1)}(n + 1)$ tend vers 0 lorsque $n$ tend vers $+\infty$, pour tout $k \geq 1$; il en est d’ailleurs de même de

$$
f(n + 1) = \log \left( 1 + \frac{y}{n + 1} \right) - \log \left( 1 + \frac{x}{n + 1} \right).
$$

D’autre part, on a

$$
\int_0^{n+1} \log (x + t) \, dt = (x + n + 1)(\log (x + n + 1) - 1) - x(\log x - 1);
$$

lorsque $n$ tend vers $+\infty$, on a le développement asymptotique

$$
(x + n)(\log (x + n) - 1) = n \log n - n + x \log n + O \left( \frac{1}{n} \right).
$$

Portant dans l’expression (15) on voit finalement que, lorsque $n$ tend vers $+\infty$, $T_p(n)$ a une limite $R_p(x, y)$ et que l’on peut écrire

$$
\log \Gamma(x) - g(x) \equiv \log \Gamma(y) - g(y) + R_p(x, y) \pmod{2\pi i}
$$

en posant

$$
g(x) = x \log x - x - \frac{1}{2} \log x + \sum_{k=1}^p \frac{b_{2k}}{2k(2k-1)} \frac{1}{x^{2k-1}}.
$$

![Figure 2](https://i.imgur.com/3Q5z5QG.png)

Fig. 2

Nous allons maintenant évaluer une borne supérieure de $R_p(x, y)$ à l’aide de l’inégalité (16), en supposant que $x$ et $y$ soient tous deux dans la partie $H_A$ de $\mathbf{C}$ définie par la relation « $\Re(z) \geqslant A$ ou $|\mathcal{F}(z)| \geqslant A$ », où $A$ est un nombre $> 0$ arbitraire (fig. 2). Remarquons pour cela que si $x = s + it$ avec $s > A$, on a $|x + u| \geqslant A + u$ pour tout $u > 0$ et par suite

$$
\int_0^{n+1} \frac{du}{|x + u|^{2p+1}} \leqslant \int_0^\infty \frac{du}{(A + u)^{2p+1}} = \frac{1}{2pA^{2p}}.
$$

De même, si $|t| \geq A$, on a $|x + u| = |s + u + it| \geq \sqrt{A^2 + (s + u)^2}$ pour tout $u$ réel, d’où
$$
\int_0^{n+1} \frac{du}{|x + u|^{2p+1}} \leq \int_{-\infty}^{+\infty} \frac{du}{(A^2 + u^2)^{p+\frac{1}{2}}} = \frac{2}{A^{2p}} \int_0^{\infty} \frac{dv}{(1 + v^2)^{p+\frac{1}{2}}}.
$$
On voit donc que, lorsque $x$ et $y$ sont dans $H_A$, on a
$$
|R_p(x, y)| \leq \frac{C_p}{A^{2p}}
$$
où $C_p$ ne dépend que de $p$. Soit alors $\mathfrak{F}$ le filtre ayant pour base les ensembles $H_A$; le critère de Cauchy montre que, suivant le filtre $\mathfrak{F}$, la fonction $\log \Gamma(z) - g(z)$ a une limite finie $\delta$ (modulo $2\pi i$) et que, si on pose $\omega(z) = \max (\Re(z), |\Im(z)|)$, on a
$$
\log \Gamma(z) - g(z) - \delta \equiv O \left( \frac{1}{(\omega(z))^{2p}} \right) \quad \text{(mod. } 2\pi i \text{)}.
$$
Pour $x$ réel et $> 0$, on a $\Gamma(x) > 0$, et $g(x)$ est réel, donc on peut supposer $\delta$ réel, et on a
$$
\log \Gamma(x) = g(x) + \delta + O \left( \frac{1}{x^{2p}} \right).
$$
Nous allons en déduire la valeur de la constante $\delta$; d’après la prop. 2 de VII, p. 14, appliquée pour $p = 2$, on a, pour $x$ réel tendant vers $+\infty$
$$
\frac{x-1}{2} \log \frac{x}{2} - \frac{x}{2} + \frac{x}{2} \log \frac{x+1}{2} - \frac{x+1}{2} + 2\delta \\
= x \log x - x - \frac{1}{2} \log x + (\frac{1}{2} - x) \log 2 + \frac{1}{2} \log 2\pi + \delta + o(1)
$$
d’où on tire aisément $\delta = \frac{1}{2} \log 2\pi$. On a donc finalement le résultat suivant:

#### Proposition 4 {#fvr-vii-s2-prop-4 .statement}

*Suivant le filtre $\mathfrak{F}$, on a (pour tout entier $p \geq 1$) le développement asymptotique*
$$
\log \Gamma(z) \equiv z \log z - z - \frac{1}{2} \log z + \frac{1}{2} \log 2\pi \\
+ \sum_{k=1}^p \frac{b_{2k}}{2k(2k-1)} \frac{1}{z^{2k-1}} + O \left( \frac{1}{(\omega(z))^{2p}} \right) \quad \text{(mod. } 2\pi i \text{)}
$$
*(développement de Stirling)*.

#### Corollaire {#fvr-vii-s2-n3-cor-1 .statement}

*Suivant le filtre $\mathfrak{F}$, on a*
$$
\Gamma(z) \sim \sqrt{2\pi} \exp \left( z \log z - z - \frac{1}{2} \log z \right).
$$
En particulier, pour $x$ réel et tendant vers $+\infty$, la formule (20) s’écrit
$$
\Gamma(x) \sim \sqrt{2\pi x^{x-\frac{1}{2}} e^{-x}},
$$

d’où pour $n$ entier tendant vers $+\infty$

$$
n! \sim \sqrt{2\pi}\ n^{n+\frac{1}{2}}\ e^{-n}
$$

(cf. V, p. 34).

On déduit de là de nombreuses formules. Par exemple, pour tout nombre complexe $\alpha$ et tout entier $n$, on a, lorsque $n$ tend vers $+\infty$

$$
\frac{\Gamma(n+\alpha)}{\Gamma(n)} \sim n^{\alpha} \ (= e^{\alpha \log n}).
$$

(22)

De même, pour tout nombre complexe $a$ distinct d’un entier $\leqslant 0$, on a

$$
a(a+1)(a+2)\ldots(a+n) = \frac{\Gamma(n+a+1)}{\Gamma(a)} \sim \frac{\sqrt{2\pi}}{\Gamma(a)}\ n^{n+a+\frac{1}{2}}\ e^{-n}
$$

et pour nombre complexe $a$, distinct d’un entier $\geqslant 0$

$$
\binom{a}{n} = \frac{(-1)^n}{\Gamma(-a)} \frac{\Gamma(n-a)}{\Gamma(n+1)} \sim \frac{(-1)^n}{\Gamma(-a)}\ n^{-a-1}.
$$

(24)

Enfin, pour toute constante réelle $k > 1$, on a

$$
\binom{kn}{n} = \frac{\Gamma(kn+1)}{\Gamma(n+1)\Gamma((k-1)n+1)} \sim \sqrt{\frac{k}{2\pi(k-1)n}} \left( \frac{k^n}{((k-1)^{k-1})^n} \right),
$$

(25)

Le même raisonnement conduit à la proposition analogue suivante:

#### Proposition 5 {#fvr-vii-s2-prop-5 .statement}

*Suivant le filtre $\mathfrak{F}$, on a (pour tout entier $p \geqslant 1$), le développement asymptotique*

$$
\frac{\Gamma'(z)}{\Gamma(z)} = \log z - \frac{1}{2z} - \sum_{k=1}^p \frac{b_{2k}}{2k} \frac{1}{z^{2k}} + O \left( \frac{1}{(\omega(z))^{2p+1}} \right).
$$

(26)

Au lieu de la prop. 2 de VII, p. 14, on utilise pour la détermination de la constante la formule

$$
\int_x^{x+1} \frac{\Gamma'(t)}{\Gamma(t)}\ dt = \log \Gamma(x+1) - \log \Gamma(x) = \log x.
$$

Exercices

## EXERCICES {#fvr-vii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
