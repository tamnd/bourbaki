---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: Valuations
section: 6
section_title: Valeurs absolues
lang: fr
source: ac-v-vii-fr
pdf_pages: 0118-0128, 0181-0182
extraction: ocr
subsections:
    - "no": 1
      title: Préliminaires sur les valeurs absolues
      page: 0
      pdf_page: 118
    - "no": 2
      title: Valeurs absolues ultramétriques
      page: 0
      pdf_page: 120
    - "no": 3
      title: '*Valeurs absolues sur Q*'
      page: 0
      pdf_page: 121
    - "no": 4
      title: Structure des corps munis d’une valeur absolue non ultramétrique
      page: 0
      pdf_page: 123
statements: 13
exercises: 2
content_sha256: 35554ce234a74fedcfcbc63f30d7c781ed0bae0cd26de430a50d4b554e69cbff
---

## § 6. Valeurs absolues.

### 1. Préliminaires sur les valeurs absolues

Soit $K$ un corps (commutatif ou non). Rappelons (Top. gén., chap. IX, § 3, no 2, déf. 2) qu’on appelle valeur absolue sur $K$ toute application $f$ de $K$ dans $\mathbf{R}_+$ vérifiant les axiomes suivants :

(VA_I) *La relation* $f(x) = 0$ *équivaut à* $x = 0$.
(VA_{II}) $f(xy) = f(x)f(y)$ *quels que soient* $x, y$ *dans* $K$.
(VA_{III}) $f(x + y) \leq f(x) + f(y)$ *quels que soient* $x, y$ *dans* $K$.
Il résulte de (VA_I) et (VA_{II}) que l’on a $f(1) = 1, f(-1) = 1$,
et $f(x^{-1}) = \frac{1}{f(x)}$ pour $x \neq 0$.

Pour une application $f$ de $K$ dans $\mathbf{R}_+$, et un nombre réel $A > 0$, nous noterons $(\mathrm{U}_A)$ la relation
$$
f(x + y) \leqslant A \cdot \sup(f(x), f(y)) \text{ quels que soient } x, y \text{ dans } K.
$$
Nous noterons $\mathcal{V}(K)$ l’ensemble des applications $f$ de $K$ dans $\mathbf{R}_+$ vérifiant $(\mathrm{VA}_I)$ et $(\mathrm{VA}_{II})$ et pour lesquelles il existe un $A > 0$ (dépendant de $f$) tel que $(\mathrm{U}_A)$ soit vraie.

On remarquera que si $f \in \mathcal{V}(K)$, on a, en faisant $x = 1, y = 0$ dans $(\mathrm{U}_A)$, $1 = f(1) \leqslant A \cdot \sup(f(1), f(0)) = A$.

#### Proposition 1 {#ac-vi-s6-prop-1 .statement}

Pour qu’une application $f$ de $K$ dans $\mathbf{R}_+$ vérifiant $(\mathrm{VA}_I)$ et $(\mathrm{VA}_{II})$ appartienne à $\mathcal{V}(K)$, il faut et il suffit que $f(1 + x)$ soit borné dans l’ensemble des $x \in K$ tels que $f(x) \leqslant 1$.
En effet, si $f$ vérifie $(\mathrm{U}_A)$, on a $f(1 + x) \leqslant A$ si $f(x) \leqslant 1$.
Inversement, supposons que $f(x + 1) \leqslant A$ pour les $x \in K$ tels que $f(x) \leqslant 1$ (ce qui entraîne $A \geqslant f(1) = 1$); alors, si $x = 0$ ou $y = 0$, la condition $(\mathrm{U}_A)$ est vérifiée; si au contraire $x \neq 0$ et $y \neq 0$, on peut par exemple supposer $f(y) \leqslant f(x)$, donc, d’après $(\mathrm{VA}_{II})$, $f(yx^{-1}) \leqslant 1$, et par suite $f(1 + yx^{-1}) \leqslant A$, ce qui donne, en vertu de $(\mathrm{VA}_{II})$, $f(x + y)f(x)^{-1} \leqslant A$; d’où
$$
f(x + y) \leqslant Af(x) \leqslant A \cdot \sup(f(x), f(y)).
$$
Si $f$ est une valeur absolue sur $K$, on a $f(n.1) \leqslant n$ par récurrence sur l’entier $n > 0$ à partir de $(\mathrm{VA}_{III})$; réciproquement :

#### Proposition 2 {#ac-vi-s6-prop-2 .statement}

Soit $f$ une application de $K$ dans $\mathbf{R}_+$ appartenant à $\mathcal{V}(K)$; s’il existe $C > 0$ tel que $f(n.1) \leqslant C.n$ pour tout entier $n > 0$, $f$ est une valeur absolue sur $K$.
Par récurrence sur $r > 0$, on déduit de $(\mathrm{U}_A)$ la relation
$$
f(x_1 + x_2 + \cdots + x_{2^r}) \leqslant A^r \sup_{1 \leqslant i \leqslant 2^r} f(x_i)
$$
pour toute famille $(x_i)$ de $2^r$ éléments de $K$. Posons $n = 2^r - 1$; pour tout $x \in K$, on déduit de (1)
$$
(f(1 + x))^n = f((1 + x)^n) = f \left( \sum_{i=0}^n \binom{n}{i} x^i \right) \leqslant A^r \sup \left( f \left( \binom{n}{i} \right) (f(x))^i \right)
$$
$$
\leqslant CA^r \sum_{i=0}^n \binom{n}{i} (f(x))^i = CA^r (1 + f(x))^n
$$
car $f \left( \binom{n}{i} \right) \leqslant C \binom{n}{i}$; on a donc
$$
f(1 + x) \leqslant C^{1/n} A^{r/n} (1 + f(x)).
$$

Faisant tendre $r$ vers $+\infty$, il vient $f(1 + x) \leq 1 + f(x)$ pour tout $x \in K$; appliquant cette inégalité en remplaçant $x$ par $xy^{-1}$ (pour $y \neq 0$) et tenant compte de (VA$_{\text{II}}$), on obtient la relation (VA$_{\text{III}}$), ce qui prouve la proposition.

#### Corollaire 1 {#ac-vi-s6-prop-2-cor-1 .statement}

Pour qu’une application $f$ de $K$ dans $\mathbf{R}_+$ soit une valeur absolue, il faut et il suffit qu’elle vérifie les conditions (VA$_{\text{I}}$), (VA$_{\text{II}}$) et (U$_2$).

C’est nécessaire, car (VA$_{\text{III}}$) entraîne
$$
f(x + y) \leq f(x) + f(y) \leq 2 \sup(f(x), f(y)).
$$
Inversement, supposons que $f$ vérifie (VA$_{\text{I}}$), (VA$_{\text{II}}$) et (U$_2$); pour tout entier $n > 0$, soit $r$ le plus petit entier tel que $2^r \geq n$; si dans (1) on remplace $A$ par 2, les $x_i$ d’indice $i \leq n$ par 1 et les $x_i$ d’indice $i > n$ par 0, on obtient $f(n.1) \leq 2^r < 2n$; on peut alors appliquer la prop. 2 avec $C = 2$, donc $f$ est une valeur absolue.

#### Corollaire 2 {#ac-vi-s6-prop-2-cor-2 .statement}

Pour qu’une application $f$ de $K$ dans $\mathbf{R}_+$ appartienne à $\mathcal{V}(K)$, il faut et il suffit qu’elle soit de la forme $g^t$, où $t > 0$ et $g$ est une valeur absolue sur $K$.

En effet, dire que $f$ vérifie (U$_A$) équivaut à dire que $f^s$ vérifie (U$_{A^s}$); comme il existe $s > 0$ tel que $A^s \leq 2$, le cor. 1 montre que pour une telle valeur de $s$, $f^s$ est une valeur absolue.

### 2. Valeurs absolues ultramétriques

On dit qu’une application $f$ de $K$ dans $\mathbf{R}_+$ est une valeur absolue ultramétrique si elle vérifie les conditions (VA$_{\text{I}}$), (VA$_{\text{II}}$) et (U$_1$) (ce qui entraîne évidemment que $f$ est une valeur absolue).

#### Proposition 3 {#ac-vi-s6-prop-3 .statement}

Soit $f$ une application de $K$ dans $\mathbf{R}_+$. Les propriétés suivantes sont équivalentes:

a) $f$ est une valeur absolue ultramétrique.

b) Il existe une valuation $v$ de $K$, à valeurs dans $\mathbf{R}$, et un nombre réel $a$ tels que $0 < a < 1$ et $f = a^v$.

c) $f$ appartient à $\mathcal{V}(K)$ et l’on a $f(n.1) \leq 1$ pour tout entier $n > 0$.

d) Pour tout $s > 0$, $f^s$ est une valeur absolue.
Pour tout nombre réel $c$ tel que $0 < c < 1$, l’application $t \to c^t$ est un isomorphisme du groupe ordonné $\mathbf{R}$ (muni de l’ordre opposé à l’ordre usuel) sur le groupe ordonné $\mathbf{R}_+^*$; cela montre l’équivalence de a) et b). Il est clair que a) implique $c);$ c) entraîne d), car on déduit de c) que $(f(n.1))^s \leqslant 1 \leqslant n$ pour tout entier $n > 0$ et la prop. 2 du no 1 montre que $f^s$ est une valeur absolue. Enfin d) entraîne a): en effet, si $f^s$ est une valeur absolue, elle vérifie $(\mathrm{U}_2)$, donc $f$ vérifie $\mathrm{U}_{2^{1/s}}$ pour tout $s > 0$, et par suite aussi $(\mathrm{U}_1)$ en faisant tendre $s$ vers $+ \infty$.

#### Corollaire {#ac-vi-s6-n2-cor-1 .statement}

*Si K est un corps (non nécessairement commutatif) de caractéristique $p > 0$, toute fonction de $\mathcal{V}(K)$ est une valeur absolue ultramétrique.*

En effet, tout élément $z = n.1$ (*n* entier $> 0$) non nul appartient au sous-corps premier $\mathbf{F}_p$ de $K$, donc vérifie la relation $z^{p-1} = 1$, ce qui entraîne $f(z) = 1$ et l’on peut appliquer la prop. 3, c).

Étant donné un nombre réel $c$ tel que $0 < c < 1$, les formules
$$
f(x) = c^{\nu(x)}, \quad \nu(x) = \log_c f(x)
$$
établissent donc une correspondance biunivoque entre valeurs absolues ultramétriques sur $K$ et valuations de $K$ à valeurs réelles. À la valeur absolue impropre (*Top. gén.*, chap. IX, § 3, no 2) correspond la valuation impropre. Soient $\nu_1, \nu_2$ deux valuations de $K$ à valeurs réelles, et $f_1, f_2$ les valeurs absolues correspondantes; pour que $\nu_1$ et $\nu_2$ soient équivalentes, il faut et il suffit que $f_1$ et $f_2$ le soient : en effet, dire que $\nu_1$ et $\nu_2$ sont équivalentes revient à dire que les relations $\nu_1(x) \geqslant 0$ et $\nu_2(x) \geqslant 0$ sont équivalentes, ou encore que les relations $f_1(x) \leqslant 1$ et $f_2(x) \leqslant 1$ sont équivalentes; il suffit donc d’appliquer la prop. 5 de *Top. gén.*, chap. IX, § 3, no 2. En outre (*loc. cit.*) pour que les topologies définies sur $K$ par $f_1$ et $f_2$ soient identiques, il faut et il suffit que $f_1$ et $f_2$ soient équivalentes.

### 3. *Valeurs absolues sur Q*

#### Proposition 4 {#ac-vi-s6-prop-4 .statement}

*Soit $f$ une application de $\mathbf{Q}$ dans $\mathbf{R}_+$ appartenant à $\mathcal{V}(\mathbf{Q})$. Alors*:

(i) *Ou bien $f$ est la valeur absolue impropre sur $\mathbf{Q}$*.

(ii) *Ou bien il existe un nombre réel $a$ et un nombre premier $p$ tels que $0 < a < 1$ et $f = a^{\nu_p}$, où $\nu_p$ est la valuation $p$-adique*.

(iii) *Ou bien il existe $s > 0$ tel que $f(x) = |x|^s$ pour tout $x \in \mathbf{Q}$.*

Dans le cas (iii), pour que $f$ soit une valeur absolue sur $\mathbf{Q}$, il faut et il suffit que $0 < s \leq 1$.

Supposons d’abord que l’on ait $f(n) \leq 1$ pour tout entier $n > 0$. En vertu de la prop. 3 du no 2, il existe un nombre réel $b$ et une valuation $\nu$ de $\mathbf{Q}$ tels que $0 < b < 1$ et $f = b^\nu$. Or, on sait ($\S 3$, no 4, Exemple 4) que les seules valuations sur $\mathbf{Q}$ sont (à équivalence près) la valuation impropre et les valuations $p$-adiques $\nu_p$; on est donc dans l’un des cas (i) ou (ii).

Supposons désormais qu’il existe un entier $h > 0$ tel que $f(h) > 1$; en vertu du no 1, cor. 2 de la prop. 2, il existe un nombre $\rho > 0$ tel que $f^\rho$ soit une valeur absolue; posons

$$
g(x) = \rho \log (f(x))/\log |x|
$$

pour tout nombre rationnel $x \neq 0$. Soient $a, b$ deux entiers $\geq 2$; pour tout entier $n \geq 2$, notons $q(n)$ la partie entière de $n.\log a/\log b$, autrement dit le plus petit entier $m$ tel que $a^n < b^{m+1}$; le développement de $a^n$ de base $b$ est donc

$$
a^n = c_0 + c_1 b + \cdots + c_{q(n)} b^{q(n)}
$$

avec $0 \leq c_i < b$ pour $0 \leq i \leq q(n)$. Comme $f^\rho$ est une valeur absolue, on a $f^\rho(c_i) \leq c_i \leq b$, et l’on déduit donc de (2) que

$$
\begin{align*}
(f(a))^{n\rho} &= (f(a^n))^\rho \leq b(1 + (f(b))^\rho + \cdots + (f(b))^{pq(n)}) \\
&\leq b(q(n) + 1) (\sup (1, (f(b))^\rho))^{q(n)}.
\end{align*}
$$

Prenant les logarithmes des deux membres de cette inégalité et divisant par $n.\log a$, on obtient

$$
g(a) \leq \frac{\log b}{n.\log a} + \frac{\log (q(n) + 1)}{q(n)} \cdot \frac{q(n)}{n \log a} + \frac{\sup (0, \rho \log f(b))}{\log a} \cdot \frac{q(n)}{n}.
$$

Notons maintenant que lorsque $n$ tend vers $+\infty$, $q(n)/n$ tend vers $\log a/\log b$; par suite $q(n)$ tend vers $+\infty$ et

$$
\log (q(n) + 1)/q(n)
$$

tend vers 0 (Fonct. var. réelle, chap. III, § 2, no 1). Passant à la limite dans (3), il vient

$$
g(a) \leq \frac{\sup (0, \rho \log f(b))}{\log b} = \sup (0, g(b)).
$$

Mais l’on a $f(h) > 1$, d’où $g(h) > 0$; si l’on remplace $a$ par $h$ dans (4), on obtient $\sup (0, g(b)) > 0$, donc

$$
\sup (0, g(b)) = g(b).
$$

C.Q.F.D.

### 4. Structure des corps munis d’une valeur absolue non ultramétrique

#### Théorème 1 (Gelfand-Mazur) {#ac-vi-s6-thm-1 .statement}

Soit $K$ une algèbre sur le corps $\mathbf{R}$ ayant les deux propriétés suivantes:

1° $K$ est un corps (non nécessairement commutatif).

2° Il existe sur $K$ une norme $x \to ||x||$ compatible avec la structure d’algèbre de $K$ (*Top. gén.*, chap. IX, § 3, no 7, déf. 9).
Alors l’algèbre $K$ est isomorphe à l’une des algèbres $\mathbf{R}, \mathbf{C}$ ou $\mathbf{H}$.

Rappelons (loc. cit.) que l’on peut toujours supposer que l’on a $||xy|| \leq ||x||.||y||$ quels que soient $x, y$ dans $K$. Nous munirons $K$ de la topologie (compatible avec la structure d’algèbre) définie par la norme.

A) Premier cas: $K$ est commutatif et il existe $j \in K$ tel que $j^2 = -1$. Il existe alors un isomorphisme $\sigma$ du corps $\mathbf{C}$ sur un sous-corps de $K$ tel que $\sigma(\xi + i\eta) = \xi . 1 + \eta . j$ pour $\xi, \eta$ dans $\mathbf{R}$. Nous allons prouver par l’absurde que l’on a $K = \sigma(\mathbf{C})$. Supposons donc qu’il existe $x \in K - \sigma(\mathbf{C})$; pour tout $z \in \mathbf{C}$, $x - \sigma(z)$ est donc inversible dans $K$; posons $F(z) = (x - \sigma(z))^{-1}$; comme $\sigma$ est continue et que l’inverse est continu dans $K$ (*Top. gén.*, chap. IX, § 3, no 7, prop. 13 appliquée à l’algèbre complétée de $K$), $F$ est une application continue de $\mathbf{C}$ dans $K$. On peut d’ailleurs écrire, pour $z \neq 0$,

$$
F(z) = (\sigma(z))^{-1}(x(\sigma(z))^{-1} - 1)^{-1}.
$$

Mais comme $(\sigma(z))^{-1} = \sigma(z^{-1})$ tend vers 0 lorsque $z$ tend vers l’infini dans $\mathbf{C}$, on voit que $F(z)$ tend alors vers 0; autrement dit, $z \to ||F(z)||$ est une fonction numérique continue

Soit $z \in P$; posons $y = x - \sigma(z)$ et soit $t$ un nombre complexe $\neq 0$ tel que $||\sigma(t)|| < \alpha^{-1}$, d’où $||\sigma(t).y^{-1}|| < 1$ par définition de $\alpha$. La suite des $(\sigma(t)y^{-1})^n$ et celle des $n(\sigma(t)y^{-1})^n$ tendent donc vers $0$ dans $K$ lorsque $n$ tend vers $+ \infty$, car il en est ainsi des suites des normes correspondantes dans $\mathbf{R}$.

Notons d’autre part que pour tout polynôme $H(T) = \prod_{k=1}^p (T - \sigma(c_k))$ où les $c_k$ sont des nombres complexes deux à deux distincts, on a, dans le corps $K(T)$ des fractions rationnelles

$$
\frac{H'(T)}{H(T)} = \sum_{k=1}^p \frac{1}{T - \sigma(c_k)}.
$$

Appliquons cette formule au polynôme

$$
H(T) = T^n - (\sigma(t))^n = \prod_{k=0}^{n-1} (T - \sigma(\omega_n^k t)),
$$

où $\omega_n = \exp(2\pi i / n)$, et substituons à $T$ l’élément $y \in K$, qui est distinct de tous les $\sigma(\omega_n^k t)$. Il vient (dans le corps commutatif $K$)

$$
\frac{ny^{n-1}}{y^n - (\sigma(t))^n} = \frac{1}{y - \sigma(t)} + \sum_{k=1}^{n-1} \frac{1}{y - \sigma(\omega_n^k t)}.
$$

Compte tenu des définitions de $F$ et de $y$, on obtient

$$
\begin{align}
F(z + t) + \sum_{k=1}^{n-1} F(z + \omega_n^k t) - nF(z) \\
= \frac{ny^{n-1}}{y^n - (\sigma(t))^n} - \frac{n}{y} = \frac{1}{y} \cdot \frac{n(\sigma(t)y^{-1})^n}{1 - (\sigma(t)y^{-1})^n}.
\end{align}
$$

Mais en vertu du choix de $t$ et des remarques faites plus haut, le dernier membre de (7) tend vers $0$ lorsque $n$ tend vers $+ \infty$; donc

$$
||F(z + t)|| = \lim_{n \to +\infty} \left| nF(z) - \sum_{k=1}^{n-1} F(z + \omega_n^k t) \right|.
$$

Or on a $||\mathbf{F}(z)|| = \alpha$ et $||\mathbf{F}(z + \omega_n^{k t})|| \leq \alpha$ par définition de $\alpha$, d’où

$$
\left| n \mathbf{F}(z) - \sum_{k=1}^{n-1} \mathbf{F}(z + \omega_n^{k t}) \right|
$$
$$
\geq n ||\mathbf{F}(z)|| - \sum_{k=1}^{n-1} ||\mathbf{F}(z + \omega_n^{k t})|| \geq n \alpha - (n-1)\alpha = \alpha.
$$

En vertu de (8), on a par suite, en faisant tendre $n$ vers $+\infty$, $||\mathbf{F}(z + t)|| \geq \alpha$, et par définition de $\alpha$ cela entraîne

$$
||\mathbf{F}(z + t)|| = \alpha,
$$

autrement dit $z + t \in \mathbf{P}$. Cela prouve que l’ensemble $\mathbf{P}$ est ouvert dans $\mathbf{C}$; comme il est aussi fermé et non vide et que $\mathbf{C}$ est connexe, on a $\mathbf{P} = \mathbf{C}$ et $||\mathbf{F}||$ est donc constante dans $\mathbf{C}$; comme cette fonction tend vers 0 au point à l’infini, on a $||\mathbf{F}(z)|| = 0$ dans $\mathbf{C}$, et en particulier $||\mathbf{F}(0)|| = ||x^{-1}|| = 0$, ce qui est absurde.

B) Deuxième cas : K est commutatif, et $-1$ n’est pas le carré d’un élément de K.

Soit L le corps commutatif obtenu par adjonction à K d’une racine $j$ de $T^2 + 1$; L est un espace vectoriel sur K admettant $(1, j)$ pour base, et L est évidemment une algèbre sur $\mathbf{R}$. Il est clair que la fonction $x + yj \to ||x|| + ||y||$ est une norme sur L compatible avec sa structure d’espace vectoriel sur $\mathbf{R}$; d’autre part, pour $z = x + yj,\ z' = x' + y'j$ dans L, on a

$$
||zz'|| = ||xx' - yy'|| + ||xy' + x'y|| \leq ||xx'|| + ||yy'|| + ||xy'|| + ||x'y||
$$
$$
\leq ||x||.||x'|| + ||y||.||y'|| + ||x||.||y'|| + ||x'||.||y||
$$
$$
= (||x|| + ||y||)(||x'|| + ||y'||) = ||z||.||z'||.
$$

La norme ainsi définie est par suite compatible avec la structure de R-algèbre de L. En vertu du cas A), L est une R-algèbre isomorphe à $\mathbf{C}$; or la seule sous-R-algèbre de $\mathbf{C}$ distincte de $\mathbf{C}$ est $\mathbf{R}$, donc K est isomorphe à $\mathbf{R}$.

C) Troisième cas : K est non commutatif.

Soient Z le centre de K, $x$ un élément de K non dans Z; le sous-corps $Z(x)$ de K est commutatif et la norme induite par celle de K est compatible avec la structure de R-algèbre de $Z(x)$; comme $Z \neq Z(x)$ et que Z et $Z(x)$ sont des R-algèbres isomorphes à $\mathbf{R}$ ou à $\mathbf{C}$ en vertu de A) et B), Z est nécessairement isomorphe à $\mathbf{R}$ et $Z(x)$ à $\mathbf{C}$. Pour tout $x \in K$, $Z(x)$ est donc de rang $\leq 2$ sur Z. Or on a le lemme suivant :

#### Lemme 1 {#ac-vi-s6-lem-1 .statement}

Soit D un corps de centre L, tel que pour tout $x \in D$, $L(x)$ soit une extension de L de degré $\leq m$. Alors le rang de D sur L est $\leq m^2$.

On peut évidemment se borner au cas où $D \neq L$. Il existe alors dans D une extension commutative algébrique séparable E de L, de degré fini $> 1$ (Alg., chap. VIII, § 10, no 3, lemme 1); comme $E = L(x)$ pour un $x$ convenable dans E (Alg., chap. V, § 7, no 7, prop. 12 et chap. VII, § 5, no 7), on a par hypothèse $[E : L] \leq m$. Supposons l’extension séparable E prise telle que $[E : L]$ soit fini et le plus grand possible, et considérons le commutant $E' \supset E$ de E dans D, qui est un corps de centre E, tel que

$$
[D : E'] = [E : L] \leq m
$$

(Alg., chap. VIII, § 10, no 2, th. 2). Si l’on avait $E \neq E'$, il existerait dans $E'$ une extension algébrique séparable F de E, de degré fini $> 1$ (Alg., chap. VIII, § 10, no 3, lemme 1); F serait donc une extension algébrique séparable de L (Alg., chap. V, § 7, no 4, prop. 7) de degré fini $> [E : L]$, contrairement à la définition de E; on a donc $E' = E$, d’où $[D : L] = [D : E][E : L] \leq m^2$.

Appliquant ce lemme à K avec $m = 2$, on voit que K est un surcorps non commutatif de rang fini de $\mathbf{R}$, donc nécessairement isomorphe au corps de quaternions $\mathbf{H}$ (Alg., chap. VIII, § 11, no 2, th. 2).

C.Q.F.D.

Remarque 1). — Indiquons le principe d’une démonstration plus courte du th. de Gelfand-Mazur, valable lorsque, au lieu de $2^o$, on suppose seulement qu’il existe sur K une topologie localement convexe séparée compatible avec sa structure de corps : on se ramène (comme dans les cas B) et C)) au cas où K est une algèbre commutative sur $\mathbf{C}$; si $x \in K - \mathbf{C}.1$, on considère comme plus haut l’application $z \to (x - z.1)^{-1}$ de $\mathbf{C}$ dans K, qui est continue et dérivable dans $\mathbf{C}$. Pour tout élément $x'$ du dual $K'$ de l’espace localement convexe K, $z \to \langle (x - z.1)^{-1}, x' \rangle$ est donc une fonction entière et bornée dans $\mathbf{C}$, donc constante en vertu du th. de Liouville, et l’on conclut, comme dans la partie A) de la démonstration du th. 1, que cela implique nécessairement $\langle (x - z.1)^{-1}, x' \rangle = 0$ pour tout $z \in \mathbf{C}$ et tout $x' \in K'$; le th. de Hahn-Banach montre que cette conclusion est absurde, puisque $(x - z.1)^{-1} \neq 0$. On notera que le raisonnement de la partie A) de la démonstration du th. 1 ne diffère du précédent qu’en apparence, car ce raisonnement n’est en fait qu’un cas particulier de celui qui sert à prouver le principe du maximum pour les fonctions analytiques, la sommation sur les racines de l’unité et le passage à la limite équivalant au calcul de l’intégrale $\int_{\gamma} \frac{F(z + t)}{t} dt$ le long d’un cercle de centre 0,
et l’utilisation de la formule de Cauchy étant ici évitée grâce à la forme particulière de la fonction F.

#### Théorème 2 (Ostrowski) {#ac-vi-s6-thm-2 .statement}

Soient K un corps (non nécessairement commutatif), f un élément de $\mathcal{V}(K)$ qui n’est pas une valeur absolue ultramétrique. Il existe alors un nombre réel $s > 0$ et un seul et un isomorphisme j de K sur un sous-corps partout dense de l’un des corps $\mathbf{R}, \mathbf{C}$ ou $\mathbf{H}$, tels que $f(x) = |j(x)|^s$ pour tout $x \in K (*)$. Pour que f soit une valeur absolue sur K, il faut et il suffit que $s \leq 1$.

En vertu du no 2, cor. de la prop. 3, K est de caractéristique 0, donc une algèbre sur $\mathbf{Q}$; pour tout $x \in \mathbf{Q}$, posons $h(x) = f(x.1)$; il est clair que $h \in \mathcal{V}(\mathbf{Q})$, et l’on peut donc appliquer la prop. 4 du no 3; on ne peut être dans le cas (i) ou (ii) de l’énoncé de cette proposition, car cela entraînerait $f(n.1) \leq 1$ pour tout entier $n > 0$, et f serait une valeur absolue ultramétrique en vertu du no 2, prop. 3. Il existe donc un nombre réel $s > 0$ tel que $h(x) = |x|^s$ pour tout $x \in \mathbf{Q}$, c’est-à-dire $f(x.1) = |x|^s$; posons $g = f^{1/s}$. Alors on a $g \in \mathcal{V}(K)$ et $g(n.1) = n$ pour tout entier $n > 0$; la prop. 2 du no 1 montre par suite que g est une valeur absolue sur K.

Pour $x \in \mathbf{Q}$ et $y \in K$, on a $g(xy) = |x|g(y)$, donc g est une norme sur K compatible avec sa structure de $\mathbf{Q}$-algèbre (pour la valeur absolue usuelle sur $\mathbf{Q}$). Le complété $\hat{K}$ de K est par suite une algèbre normée sur $\hat{\mathbf{Q}} = \mathbf{R}$ (Top. gén., chap. IX, § 3, no 7); soit $\hat{g}$ la norme sur $\hat{K}$, prolongement continu de g. Comme g est une valeur absolue sur K, $\hat{K}$ est un corps et $\hat{g}$ une valeur absolue sur $\hat{K}$ (Top. gén., chap. IX, § 3, no 3, prop. 6). En vertu du th. 1, il existe un isomorphisme $\hat{j}$ de $\mathbf{R}$-algèbres de $\hat{K}$ sur l’un des corps $\mathbf{R}, \mathbf{C}$ ou $\mathbf{H}$, et $g'(x) = |\hat{j}(x)|$ est par suite une valeur absolue sur $\hat{K}$; comme $\hat{K}$ est de dimension finie sur $\mathbf{R}$, et que $g'$ et $\hat{g}$ coïncident dans le sous-corps $\mathbf{R}.1$ de $\hat{K}$, on a $g' = \hat{g}$ en vertu du lemme suivant:

(*) Sur $\mathbf{H}$, on pose $|z|^2 = z.\overline{z} = \overline{z}.z$, $\overline{z}$ étant le quaternion conjugué de z.

#### Lemme 2 {#ac-vi-s6-lem-2 .statement}

Soient $L$ un corps (non nécessairement commutatif), $K$ un sous-corps de $L$ tel que $L$ soit un espace vectoriel à gauche de dimension finie sur $K$. Soient $g$ une valeur absolue sur $L$, $f$ sa restriction à $K$. Si $K$ est complet et non discret pour $f$, $L$ est complet pour $g$; si en outre $g'$ est une seconde valeur absolue sur $L$ ayant la même restriction $f$ à $K$, on a $g' = g$.

Comme la topologie définie par $g$ est séparée et compatible avec la structure de $K$-espace vectoriel à gauche de $L$, la première assertion résulte de *Esp. vect. top.*, chap. I, § 2, no 3, th. 2. En outre les topologies sur $L$ définies par $g$ et $g'$ sont identiques (*loc. cit.*); il existe par suite un nombre réel $s > 0$ tel que $g' = g^s$ (*Top. gén.*, chap. IX, § 3, no 2, prop. 5). Soit $x$ un élément de $K$ tel que $f(x) \neq 1$; l’égalité $g'(x) = g(x)$ prouve que $s = 1$.

Revenant à la démonstration du th. 2, on voit que si l’on note $j$ la restriction de $\hat{j}$ à $K$, $j$ est un isomorphisme de $K$ sur un sous-corps partout dense de $\mathbf{R}, \mathbf{C}$ ou $\mathbf{H}$ et l’on a $g(x) = |j(x)|$ pour $x \in K$, d’où $f(x) = |j(x)|^s$.

Notons enfin que si $f$ est une valeur absolue sur $K$, $h$ est une valeur absolue sur $\mathbf{Q}$ et l’on a $s \leq 1$ en vertu du no 3, prop. 4; réciproquement, si $s \leq 1$, $f = g^s$ est une valeur absolue sur $K$ puisqu’il en est ainsi de $g$ (*Top. gén.*, chap. IX, § 3, no 2); cela prouve la dernière assertion de l’énoncé. C.Q.F.D.

#### Remarque 2 {#ac-vi-s6-n4-rem-2 .statement}

Si $K$ est un corps et une algèbre normée sur $\mathbf{R}$, la norme n’est pas nécessairement une valeur absolue sur $K$; par exemple, $\xi + i\eta \to |\xi| + |\eta|$ est une norme sur $\mathbf{C}$ compatible avec sa structure d’algèbre sur $\mathbf{R}$.

#### Remarque 3 {#ac-vi-s6-n4-rem-3 .statement}

Pour une démonstration du cas C) du th. 1 qui n’utilise pas les résultats généraux d'*Alg.*, chap. VIII, voir exerc. 2.

## EXERCICES {#ac-vi-s6-exercises}

See the [exercises for § 6](exercises/s6/).
