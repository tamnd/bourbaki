---
book: fvr
book_title: Functions of a Real Variable
chapter: III
chapter_title: FONCTIONS ÉLÉMENTAIRES
section: 2
section_title: Développements des fonctions exponentielles et circulaires, et des fonctions qui s'y rattachent
lang: fr
source: fvr-i-vii-fr
book_pages: FVR III.32-FVR III.34
pdf_pages: 0105-0114, 0122-0124
extraction: ocr
subsections:
    - "no": 1
      title: Développement de l’exponentielle réelle
      page: 15
      pdf_page: 105
    - "no": 2
      title: Développements de l’exponentielle complexe, de cos $x$ et sin $x$
      page: 16
      pdf_page: 106
    - "no": 3
      title: Le développement du binôme
      page: 18
      pdf_page: 108
    - "no": 4
      title: Développements de $\log(1 + x)$, de Arc tg $x$ et de Arc sin $x$
      page: 21
      pdf_page: 111
statements: 1
exercises: 9
content_sha256: 7ddef37b1d448391fc3d218cadc826d8f323a7fb34787ecb88c19dc27938bbea
---

## § 2. DÉVELOPPEMENTS DES FONCTIONS EXPONENTIELLES ET CIRCULAIRES, ET DES FONCTIONS QUI S’Y RATTACHENT

### 1. Développement de l’exponentielle réelle

Comme $\mathrm{D}^n(e^x) = e^x$, le développement de Taylor d’ordre $n$ de $e^x$ est

(1)
$$
e^x = 1 + \frac{x}{1!} + \frac{x^2}{2!} + \cdots + \frac{x^n}{n!} + \int_0^x \frac{(x - t)^n}{n!} e^t \, dt.
$$

Le reste de cette formule est $> 0$ pour $x > 0$, du signe de $(-1)^{n+1}$ pour $x < 0$; en outre, l’inégalité de la moyenne montre que

(2)
$$
\frac{x^{n+1}}{(n + 1)!} < \int_0^x \frac{(x - t)^n}{n!} e^t \, dt < \frac{x^{n+1} e^x}{(n + 1)!} \quad \text{pour } x > 0
$$

(3)
$$
\left| \frac{|x|^{n+1} e^x}{(n + 1)!} - \left| \int_0^x \frac{(x - t)^n}{n!} e^t \, dt \right| \right| < \frac{|x|^{n+1}}{(n + 1)!} \quad \text{pour } x < 0.
$$

Or, on sait que la suite $(x^n/n!)$ a pour limite 0 lorsque $n$ croît indéfiniment, pour tout $x \geqslant 0$ (TG, IV, p. 33); donc, en laissant fixe $x$ et faisant croître indéfiniment $n$ dans (1), il vient, d’après (2) et (3)

(4)
$$
e^x = \sum_{n=0}^\infty \frac{x^n}{n!}
$$

et la série du second membre est absolument et uniformément convergente dans tout intervalle compact de $\mathbf{R}$. En particulier, on a la formule

(5)
$$
e = 1 + \frac{1}{1!} + \frac{1}{2!} + \cdots + \frac{1}{n!} + \cdots
$$

Cette formule permet de calculer des valeurs rationnelles aussi approchées que l’on veut du nombre $e$; on obtient ainsi
$$ e = 2,718\ 281\ 828\ldots $$

à 1/10⁹ près par défaut. La formule (5) prouve en outre que $e$ est un nombre *irrationnel*¹ (TG, VI, p. 41).

#### Remarque {#fvr-iii-s2-n1-rem-1 .statement}

Comme le reste de la formule (1) est > 0 pour $x > 0$, on a, pour $x > 0$

$$
e^x > 1 + \frac{x}{1!} + \frac{x^2}{2!} + \ldots + \frac{x^{n+1}}{(n+1)!}
$$

et *a fortiori*

$$
e^x > \frac{x^{n+1}}{(n+1)!}
$$

pour tout entier $n$; on en déduit que $e^x / x^n$ *tend vers* $+ \infty$ avec $x$, pour tout entier $n$; nous retrouverons ce résultat au chap. V par une autre méthode (V, p. 21).

### 2. Développements de l’exponentielle complexe, de cos $x$ et sin $x$

Soit $z$ un nombre complexe quelconque, et considérons la fonction $\varphi(t) = e^{zt}$ de la variable réelle $t$; on a $D^n \varphi(t) = z^n e^{zt}$ et $e^z = \varphi(1)$; l’expression de $\varphi(1)$ par la formule de Taylor d’ordre $n$ relative au point $t = 0$ (II, p. 12), donne donc

$$
e^z = 1 + \frac{1}{1!} + \frac{z^2}{2!} + \cdots + \frac{z^n}{n!} + z^{n+1} \int_0^1 \frac{(1-t)^n}{n!} e^{zt} \, dt
$$

formule qui, lorsque $z$ est réel, est équivalente à (1). Le reste

$$
r_n(z) = z^{n+1} \int_0^1 \frac{(1-t)^n}{n!} e^{zt} \, dt
$$

de cette formule se majore encore, en valeur absolue, à l’aide de l’inégalité de la moyenne; si $z = x + iy$, on a $|e^{zt}| = e^{xt}$, donc $|e^{zt}| \leqslant 1$ si $x \leqslant 0$, $|e^{zt}| \leqslant e^x$ si $x > 0$; il vient donc

$$
|r_n(z)| \leqslant \frac{|z|^{n+1}}{(n+1)!} \quad \text{si } x \leqslant 0
$$
$$
|r_n(z)| \leqslant \frac{|z|^{n+1} e^x}{(n+1)!} \quad \text{si } x > 0.
$$

Comme ci-dessus, on en conclut que

$$
e^z = \sum_{n=0}^\infty \frac{z^n}{n!}
$$

la série étant *absolument et uniformément convergente* dans toute partie compacte de $\mathbf{C}$.

De (6) on tire en particulier, pour $x$ réel

$$
e^{ix} = 1 + \frac{ix}{1!} + \frac{i^2 x^2}{2!} + \cdots + \frac{i^n x^n}{n!} + i^{n+1} \int_0^x \frac{(x-t)^n}{n!} e^{it} \, dt
$$

¹ Ch. Hermite a démontré en 1873 que $e$ est un nombre *transcendant* sur le corps $\mathbf{Q}$ des nombres rationnels (autrement dit, n’est racine d’aucun polynôme à coefficients rationnels) (*Œuvres*, t. III, p. 150, Paris (Gauthier-Villars), 1912).

d’où on déduit les développements de Taylor de cos $x$ et de sin $x$: en prenant la partie réelle de (10) pour l’ordre $2n + 1$, on a

$$
\cos x = 1 - \frac{x^2}{2!} + \frac{x^4}{4!} + \cdots + (-1)^n \frac{x^{2n}}{(2n)!}
$$
$$
+ (-1)^{n+1} \int_0^x \frac{(x-t)^{2n+1}}{(2n+1)!} \cos t \, dt
$$

avec la limitation du reste

$$
\left| \int_0^x \frac{(x-t)^{2n+1}}{(2n+1)!} \cos t \, dt \right| \leq \frac{|x|^{2n+2}}{(2n+2)!}.
$$

De même, en prenant la partie imaginaire de (10) pour l’ordre $2n$, il vient

$$
\sin x = x - \frac{x^3}{3!} + \frac{x^5}{5!} + \cdots + (-1)^{n-1} \frac{x^{2n-1}}{(2n-1)!}
$$
$$
+ (-1)^n \int_0^x \frac{(x-t)^{2n}}{(2n)!} \cos t \, dt
$$

avec la limitation du reste

$$
\left| \int_0^x \frac{(x-t)^{2n}}{(2n)!} \cos t \, dt \right| \leq \frac{|x|^{2n+1}}{(2n+1)!}.
$$

En outre, en comparant les restes de (11) pour l’ordre $2n + 1$ et l’ordre $2n + 3$, on a

$$
\int_0^x \frac{(x-t)^{2n+3}}{(2n+3)!} \cos t \, dt = \frac{x^{2n+2}}{(2n+2)!} - \int_0^x \frac{(x-t)^{2n+1}}{(2n+1)!} \cos t \, dt
$$

et, en tenant compte de (12), on voit que le reste de (11) est du signe de $(-1)^{n+1}$ quel que soit $x$; de même manière, on montre que le reste de (13) est du signe de $(-1)^n x$. En particulier, pour $n = 0$ et $n = 1$ dans (11), pour $n = 1$ et $n = 2$ dans (13), on obtient les inégalités

$$
1 - \frac{x^2}{2} \leq \cos x \leq 1 \quad \text{pour tout } x
$$
$$
x - \frac{x^3}{6} \leq \sin x \leq x \quad \text{pour tout } x \geq 0.
$$

Enfin, en faisant $z = ix$ dans (9), on a

$$
\cos x = \sum_{n=0}^\infty (-1)^n \frac{x^{2n}}{(2n)!}
$$
$$
\sin x = \sum_{n=0}^\infty (-1)^n \frac{x^{2n+1}}{(2n+1)!}
$$

ces séries étant absolument et uniformément convergentes dans tout intervalle compact.

Il est clair d’ailleurs que les formules (17) et (18) sont encore valables pour tout $x$ complexe, les séries des seconds membres étant absolument et uniformément convergentes dans toute partie compacte de $\mathbf{C}$. En particulier, on a pour tout $x$ (réel ou complexe)

$$
\operatorname{ch} x = \sum_{n=0}^{\infty} \frac{x^{2n}}{(2n)!}
$$
$$
\operatorname{sh} x = \sum_{n=0}^{\infty} \frac{x^{2n+1}}{(2n+1)!}
$$

### 3. Le développement du binôme

Soit $m$ un nombre réel quelconque. Pour $x > 0$, on a
$$
D^n(x^m) = m(m-1)\ldots(m-n+1)x^{m-n};
$$
en appliquant à la fonction $(1+x)^m$ la formule de Taylor d’ordre $n$ relative au point $x = 0$, on obtient, pour tout $x > -1$, la formule
$$
(19) \quad (1+x)^m = 1 + \binom{m}{1}x + \binom{m}{2}x^2 + \cdots + \binom{m}{n}x^n + r_n(x)
$$
avec
$$
r_n(x) = \frac{m(m-1)\ldots(m-n)}{n!} \int_0^x \left( \frac{x-t}{1+t} \right)^n (1+t)^{m-1} dt
$$
où on a posé $\binom{m}{n} = \frac{m(m-1)\ldots(m-n+1)}{n!}$. La formule (19) se réduit à la formule du binôme (A, I, p. 94) lorsque $m$ est entier $> 0$ et $n \geq m$; par extension, on la nomme encore *formule du binôme*, et les coefficients $\binom{m}{n}$ sont dits *coefficients binomiaux*, lorsque $m$ est un nombre réel quelconque et $n$ un entier quelconque $> 0$.

Le reste de (19) a le signe de $\binom{m}{n+1}$ si $x > 0$, le signe de $(-1)^{n+1} \binom{m}{n+1}$ si $-1 < x < 0$. Comme $\left| \frac{x-t}{1+t} \right| \leq |x|$ pour tout $t > -1$ appartenant à l’intervalle d’extrémités 0 et $x$, on a la limitation suivante du reste, pour $m$ et $n$ quelconques et $x > -1$
$$
(20) \quad \left| \frac{m(m-1)\ldots(m-n)}{n!} \int_0^x \left( \frac{x-t}{1+t} \right)^n (1+t)^{m-1} dt \right|
$$
$$
\leq \left| \binom{m-1}{n} x^n ((1+x)^m - 1) \right|.
$$

Si l’on suppose $x \geq 0$, et $n \geq m - 1$, on a $(1 + t)^{n-m+1} \geq 1$ dans l’intervalle d’intégration, donc

$$
0 \leq \int_0^x \frac{(x-t)^n}{(1+t)^{n-m+1}} dt \leq \int_0^x (x-t)^n dt = \frac{x^{n+1}}{n+1}
$$

ce qui donne la majoration du reste

$$(21)$$
$$
|r_n(x)| \leq \left| \binom{m}{n+1} \right| x^{n+1} \quad (x \geq 0, n \geq m-1).
$$

D’autre part, supposons $-1 \leq m < 0$; si dans l’intégrale de (19) on fait le changement de variables $u = \frac{x-t}{x(1+t)}$, on obtient

$$(22)$$
$$
r_n(x) = \frac{m(m-1)\ldots(m-n)}{n!} (1+x)^mx^{n+1} \int_0^1 \frac{u^n du}{(1+ux)^{m+1}}.
$$

Pour majorer l’intégrale pour $x > -1$, on remarque que, puisque $m+1 < 1$, l’intégrale $\int_0^1 \frac{u^n du}{(1-u)^{m+1}}$ est convergente et majore l’intégrale du second membre de (22) puisque $1+ux > 1-u$. Or, pour $-1 < x < 0$, l’hypothèse sur $m$ entraîne que tous les termes $\binom{m}{1}x, \binom{m}{2}x^2, \ldots, \binom{m}{n}x^n$ figurant au second membre de (19) sont $\geq 0$, et par suite $r_n(x) \leq (1+x)^m$, d’où en divisant par $(1+x)^m$,

$$
\frac{m(m-1)\ldots(m-n)}{n!} x^{n+1} \int_0^1 \frac{u^n du}{(1+ux)^{m+1}} \leq 1.
$$

D’ailleurs pour $-1 < x < 0$, le facteur devant l’intégrale est $\geq 0$, d’où en faisant tendre $x$ vers $-1$,

$$
\left| \frac{m(m-1)\ldots(m-n)}{n!} \int_0^1 \frac{u^n du}{(1-u)^{m+1}} \right| \leq 1
$$

et par suite, pour $-1 \leq m < 0$ et $x > -1$

$$(23)$$
$$
|r_n(x)| \leq (1+x)^m |x|^{n+1}.
$$

De ces inégalités, nous allons déduire d’abord que, pour $|x| < 1$, on a

$$(24)$$
$$
(1+x)^m = \sum_{n=0}^\infty \binom{m}{n} x^n
$$

la série du second membre (dite série du binôme) étant absolument et uniformément convergente dans tout intervalle compact contenu dans $]-1, +1[$. En effet on peut écrire

$$(25)$$
$$
\binom{m}{n} = (-1)^n \left( 1 - \frac{m+1}{1} \right) \left( 1 - \frac{m+1}{2} \right) \ldots \left( 1 - \frac{m+1}{n} \right)
$$

d’où
$$
\left| \binom{m}{n} \right| \leq \left( 1 + \frac{|m+1|}{1} \right) \left( 1 + \frac{|m+1|}{2} \right) \cdots \left( 1 + \frac{|m+1|}{n} \right).
$$

Si $|x| \leq r < 1$, il existe $n_0$ tel que $1 + \frac{|m|}{n_0} < 1/r'$, où $r < r' < 1$, d’où, en posant
$$
k = \left( 1 + \frac{|m|}{1} \right) \left( 1 + \frac{|m|}{2} \right) \cdots \left( 1 + \frac{|m|}{n_0} \right) \quad \left| \frac{(m-1)}{n} x^n \right| \leq k|x|^{n_0} \left( \frac{r}{r'} \right)^{n-n_0}
$$
ce qui démontre la proposition. Au contraire, pour $x > 1$, la valeur absolue du terme général de la série (24) croit indéfiniment avec $n$, si $m$ n’est pas un entier $\geq 0$; en effet, d’après (25), on a, pour $n > n_1 \geq |m+1|$
$$
\left| \binom{m}{n} \right| \geq \left| \left( 1 - \frac{m+1}{1} \right) \left( 1 - \frac{m+1}{2} \right) \cdots \left( 1 - \frac{m+1}{n_1} \right) \right|
$$
$$
\left( 1 - \frac{|m+1|}{n_1+1} \right) \cdots \left( 1 - \frac{|m+1|}{n} \right).
$$
Soit $n_0 \geq n_1$ tel que, pour $n \geq n_0$, on ait $1 - \frac{|m+1|}{n} > 1/x'$, où $1 < x' < x$. Si on pose
$$
k' = \left| \left( 1 - \frac{m+1}{1} \right) \cdots \left( 1 - \frac{m+1}{n_1} \right) \right| \left( 1 - \frac{|m+1|}{n_1+1} \right) \cdots \left( 1 - \frac{|m+1|}{n_0} \right)
$$
on aura, pour $n > n_0$,
$$
\left| \binom{m}{n} x^n \right| \geq k'|x|^{n_0} \left( \frac{x}{x'} \right)^{n-n_0}
$$
d’où la proposition.

On notera que, pour $m = -1$, l’identité algébrique
$$
\frac{1}{1+x} = 1 - x + x^2 - \cdots + (-1)^{n-1} x^{n-1} + (-1)^n \frac{x^n}{1+x}
$$
donne l’expression du reste de la formule générale (19) sans intégration; la formule (23) se réduit dans ce cas à l’expression de la somme de la série (ou progression) géométrique (TG, IV, p. 32).

En second lieu, étudions la convergence de la série du binôme pour $x = 1$ ou $x = -1$ (le cas trivial $m = 0$ étant exclu):

a) $m \leq -1$. Le produit de terme général $1 - \frac{m+1}{n}$ converge vers $+\infty$ si $m < -1$, vers 1 si $m = -1$, donc il résulte de (25) que pour $x = \pm 1$, le terme général de la série du binôme ne tend pas vers 0.

b) $-1 < m < 0$. Cette fois, le produit de terme général $1 - \frac{m+1}{n}$ converge vers 0, donc l’inégalité (21) montre que $r_n(1)$ tend vers 0. La série du binôme est donc convergente pour $x = 1$ et a pour somme $2^m$; en outre, la série du binôme est uniformément convergente dans tout intervalle $]x_0, 1]$ avec $-1 < x_0 \leq 1$, en vertu de ce qui a été vu plus haut et de (21). Par contre, pour $x = -1$ tous les termes du second membre de (24) sont $\geq 0$; si cette série était convergente, on en déduirait que la série du binôme serait normalement convergente dans $(-1, 1)$ et aurait par suite pour somme une fonction continue dans cet intervalle, ce qui est absurde puisque $(1 + x)^m$ n’est pas bornée dans $]-1, 1]$ pour $m < 0$. On en conclut aussi que pour $x = 1$, la série du binôme n’est pas absolument convergente.

c) $m > 0$. La définition de $r_n(x)$ montre alors que lorsque $x$ tend vers $-1$, $r_n(x)$ tend vers une limite $r_n(-1)$; en passant à la limite dans (20), on en conclut que $|r_n(-1)| \leq \left| \binom{m-1}{n} \right|$, et comme $m - 1 > -1$, on voit que, pour $x = -1$, la série du binôme est convergente. D’ailleurs, pour $n > m + 1$, tous les termes de cette série sont de même signe; donc la série du binôme est *normalement convergente* dans l’intervalle $(-1, 1)$ et a pour somme $(1 + x)^m$ dans cet intervalle.

### 4. Développements de $\log(1 + x)$, de Arc tg $x$ et de Arc sin $x$

Intégrons les deux membres de (26) entre 0 et $x$; on obtient le développement de Taylor d’ordre $n$ de $\log (1 + x)$, valable pour $x > -1$

$$
\log (1 + x) = \frac{x}{1} - \frac{x^2}{2} + \frac{x^3}{3} + \cdots + (-1)^{n-1} \frac{x^n}{n} + (-1)^n \int_0^\infty \frac{t^n \, dt}{1 + t}.
$$

Le reste est du signe de $(-1)^n$ si $x > 0$, et est $< 0$ si $-1 < x < 0$; en outre, pour $x > 0$, on a $1 + t \geq 1$ pour $0 \leq t \leq x$, et, pour $-1 < x < 0$, $1 + t \geq 1 - |x|$ pour $x \leq 0$; d’où les limitations du reste

$$
\left| \int_0^\infty \frac{t^n \, dt}{1 + t} \right| \leq \frac{|x|^{n+1}}{n + 1} \quad \text{pour } x \geq 0
$$
$$
\left| \int_0^\infty \frac{t^n \, dt}{1 + t} \right| \leq \frac{|x|^{n+1}}{(n + 1)(1 - |x|)} \quad \text{pour } -1 < x \leq 0.
$$

De ces deux dernières formules, on déduit aussitôt que, pour $-1 < x \leq 1$, on a

$$
\log (1 + x) = \sum_{n=1}^\infty (-1)^{n-1} \frac{x^n}{n}
$$

la série étant *uniformément convergente* dans tout intervalle compact contenu dans $]-1, +1]$, *absolument convergente* pour $|x| < 1$.

Au contraire, pour $|x| > 1$, le terme général de la série du second membre de (30) croît indéfiniment en valeur absolue avec $n$ (III, p. 16). Pour $x = -1$, la série se réduit à la série harmonique, qui a pour somme $+\infty$ (TG, IV, p. 33).

De même, remplaçons dans (26) $x$ par $x^2$ et intégrons les deux membres entre 0 et $x$; on obtient le développement de Taylor d’ordre $2n - 1$ de Arc tg $x$, valable pour tout $x$ réel

(31) $$
\text{Arc tg } x = \frac{x}{1} - \frac{x^3}{3} + \frac{x^5}{5} + \cdots + (-1)^{n-1} \frac{x^{2n-1}}{2n-1} + (-1)^n \int_0^x \frac{t^{2n}\,dt}{1 + t^2}.
$$

Le reste est du signe de $(-1)^n x$, et comme $1 + t^2 \geqslant 1$ pour tout $t$, on a la limitation

(32) $$
\left| \int_0^x \frac{t^{2n}\,dt}{1 + t^2} \right| \leqslant \frac{|x|^{2n+1}}{2n+1}
$$

d’où on tire que, pour $|x| \leqslant 1$,

(33) $$
\text{Arc tg } x = \sum_{n=1}^\infty (-1)^{n-1} \frac{x^{2n-1}}{2n-1}
$$

la série étant uniformément convergente dans $[-1, +1]$, et absolument convergente pour $|x| < 1$.

En particulier, pour $x = 1$, on obtient la formule

(34) $$
\frac{\pi}{4} = 1 - \frac{1}{3} + \frac{1}{5} + \cdots + (-1)^n \frac{1}{2n+1} + \ldots
$$

Pour $|x| > 1$, le terme général de la série du second membre de (33) croît indéfiniment en valeur absolue avec $n$.

Enfin, pour le développement de Taylor de Arc sin $x$, partons du développement de sa dérivée $(1 - x^2)^{-\frac{1}{2}}$; ce dernier s’obtient en remplaçant $x$ par $-x^2$ dans le développement de $(1 + x)^{-\frac{1}{2}}$ suivant la formule du binôme, ce qui donne pour $|x| < 1$,

$$(1 - x^2)^{-\frac{1}{2}} = 1 + \frac{1}{2} x^2 + \frac{1.3}{2.4} x^4 + \cdots + \frac{1.3.5\ldots(2n-1)}{2.4.6\ldots2n} x^{2n} + r_n(x)$$

avec la limitation déduite de (23)

$$0 \leqslant r_n(x) \leqslant \frac{x^{2n+2}}{\sqrt{1 - x^2}}.$$

En prenant la primitive du développement précédent, il vient

(35) $$
\text{Arc sin } x = x + \frac{1}{2} \frac{x^3}{3} + \frac{1.3}{2.4} \frac{x^5}{5} + \cdots
$$
$$
+ \frac{1.3.5\ldots(2n-1)}{2.4.6\ldots2n} \frac{x^{2n+1}}{2n+1} + R_n(x)
$$

où $R_n(x)$ est du signe de $x$ et satisfait à l’inégalité
$$
|R_n(x)| \leq \int_0^x \frac{t^{2n+2}\,dt}{\sqrt{1-t^2}}.
$$
D’ailleurs, la relation (35) montre que $R_n(x)$ tend vers une limite lorsque $x$ tend vers 1 ou $-1$, et on a donc
$$
|R_n(1)| \leq \int_0^1 \frac{t^{2n+2}\,dt}{\sqrt{1-t^2}}.
$$
Mais l’intégrale du second membre de (37) tend vers 0 lorsque $n$ tend vers $+\infty$: en effet, l’intégrale $\int_0^1 dt/\sqrt{1-t^2}$ étant convergente, pour tout $\varepsilon > 0$, il existe $a$ tel que $0 < a < 1$ et $\int_a^1 dt/\sqrt{1-t^2} \leq \varepsilon$; d’autre part, on a
$$
\int_0^a \frac{t^{2n+2}\,dt}{\sqrt{1-t^2}} \leq \frac{1}{\sqrt{1-a^2}} \int_0^a t^{2n+2}\,dt = \frac{a^{2n+3}}{(2n+3)\sqrt{1-a^2}},
$$
et il existe donc $n_0$ tel que pour $n \geq n_0$ on ait $\frac{a^{2n+3}}{(2n+3)\sqrt{1-a^2}} \leq \varepsilon$, d’où finalement $|R_n(x)| \leq 2\varepsilon$ pour $|x| \leq 1$ et $n \geq n_0$. On a donc
$$
\text{Arc sin } x = \sum_{n=0}^\infty \frac{1.3.5\ldots(2n-1)}{2.4.6\ldots2n} \frac{x^{2n+1}}{2n+1}
$$
la série du second membre étant normalement convergente dans l’intervalle compact $(-1, 1)$.

Au contraire, on montre, comme pour la formule du binôme, que le terme général de la série du second membre de (38) croît indéfiniment en valeur absolue pour $|x| > 1$.
En faisant par exemple $x = \frac{1}{2}$ dans (38), on obtient une nouvelle expression du nombre $\pi$:
$$
\frac{\pi}{6} = \sum_{n=0}^\infty \frac{1.3.5\ldots(2n-1)}{1.4.6\ldots2n} \frac{1}{(2n+1)2^{2n+1}}
$$
qui se prête beaucoup mieux que la formule (34) au calcul de valeurs approchées de $\pi$ (voir Calcul numérique); on peut ainsi obtenir
$$
\pi = 3,141\ 592\ 653\ldots
$$
à $1/10^9$ près par défaut.\footnote{Le nombre $\pi$ est, non seulement irrationnel (cf. III, p. 35 exerc. 5), mais même transcendant sur le corps $\mathbf{Q}$ des nombres rationnels, comme il a été démontré pour la première fois en 1882 par Lindemann (v. par exemple D. Hilbert, Gesammelte Abhandlungen, t. I, p. I, Berlin (Springer), 1932).}

Exercices

## EXERCICES {#fvr-iii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
