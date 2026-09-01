---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: ÉTUDE LOCALE DES FONCTIONS
section: 4
section_title: Application aux séries à termes positifs
lang: fr
source: fvr-i-vii-fr
book_pages: FVR V.27-FVR V.35, FVR V.50-FVR V.51
pdf_pages: 0232-0240, 0255-0256
extraction: ocr
subsections:
    - "no": 1
      title: Critères de convergence des séries à termes positifs
      page: 27
      pdf_page: 232
    - "no": 2
      title: Développement asymptotique des sommes partielles d’une série
      page: 28
      pdf_page: 233
    - "no": 3
      title: Développement asymptotique des produits partiels d’un produit infini
      page: 32
      pdf_page: 237
    - "no": 4
      title: 'Application : critères de convergence de seconde espèce pour les séries à termes positifs'
      page: 34
      pdf_page: 239
statements: 9
exercises: 11
content_sha256: f31eec3f4ce12257376ba4df2f6ca957d7555f0b68f1004931fe0002156487b5
---

## § 4. APPLICATION AUX SÉRIES À TERMES POSITIFS

### 1. Critères de convergence des séries à termes positifs

Dans tout ce paragraphe, nous entendons (par abus de langage) par série à termes positifs une série $(u_n)$ à termes réels tels que $u_n \geqslant 0$ à partir d’une certaine valeur de $n$. Tout ce qui sera dit sur ces séries s’étend aussitôt par changement de signe aux séries dont tous les termes sont $\leqslant 0$ à partir d’une certaine valeur de $n$.

On a vu (II, p. 14, Exemple 3) qu’à toute suite $(u_n)_{n \geqslant 1}$ de points d’un espace normé E, on associe une fonction en escalier $u$ définie dans $[1, +\infty[$ par les conditions $u(x) = u_n$ pour $n \leqslant x < n + 1$: alors, pour que la série $(u_n)$ soit convergente, il faut et il suffit que l’intégrale $\int_1^{+\infty} u(t)\,dt$ soit convergente.

Soient $(u_n)$ et $(v_n)$ deux séries à termes positifs, $u$ et $v$ les fonctions en escalier associées: la relation $u_n \leqslant v_n$ pour $n \geqslant n_0$ équivaut à $u(x) \leqslant v(x)$ pour $x \geqslant n_0$. Par suite, chacune des relations $u_n \ll v_n$, $u_n \ll v_n$, $u_n \sim v_n$ est respectivement équivalente à $u(x) \ll v(x)$, $u(x) \ll v(x)$, $u(x) \sim v(x)$; cette remarque permet de traduire comme suit les propositions 1 (V, p. 18) et 6 (V, p. 20):

#### Proposition 1 {#fvr-v-s4-prop-1 .statement}

Soient $(u_n)$ et $(v_n)$ deux séries à termes positifs. Si $u_n \ll v_n$, et si la série $(v_n)$ est convergente, la série $(u_n)$ est convergente; si $u_n \gg v_n$ et si $\sum_{n=1}^\infty v_n = +\infty$, on a $\sum_{n=1}^\infty u_n = +\infty$.

#### Proposition 2 {#fvr-v-s4-prop-2 .statement}

Soient $(u_n)$ et $(v_n)$ deux séries à termes positifs:
1° Si la série $(v_n)$ est convergente, la relation $u_n \ll v_n$ (resp. $u_n \sim v_n$) entraîne $\sum_{p=n}^\infty u_p \ll \sum_{p=n}^\infty v_p$ (resp. $\sum_{p=n}^\infty u_p \sim \sum_{p=n}^\infty v_p$).
2° Si $\sum_{n=1}^\infty v_n = +\infty$, la relation $u_n \ll v_n$ (resp. $u_n \sim v_n$) entraîne $\sum_{p=1}^n u_p \ll \sum_{p=1}^n v_p$ (resp. $\sum_{p=1}^n u_p \sim \sum_{p=1}^n v_p$).

On obtient des critères commodes de convergence en prenant pour série de comparaison $(v_n)$ dans la prop. 1 une série dont les termes sont de la forme $v_n = f(n)$, où $f$ est une fonction $\geqslant 0$, définie pour tout nombre réel $x > x_0$ et décroissante dans l’intervalle $[x_0, +\infty[$; en effet:

**Proposition 3** (critère de Cauchy-Maclaurin). — Si $f$ est une fonction $\geqslant 0$ et décroissante dans $[x_0, +\infty[$, pour que la série de terme général $v_n = f(n)$ soit convergente, il faut et il suffit que l’intégrale $\int_{x_0}^{+\infty} f(t)\,dt$ soit convergente.

Il suffit pour le voir de remarquer que si $v$ est la fonction en escalier associée à la série $(v_n)$, on a $v(x+1) \leq f(x) \leq v(x)$ pour tout $x \geq x_0$, puisque $f$ est décroissante; la proposition résulte donc du principe de comparaison (II, p. 17, prop. 3).

Comme les fonctions qui figurent dans les critères logarithmiques de convergence des intégrales (V, p. 19–20, prop. 2, 3 et 4) sont décroissantes dans un intervalle $[x_0, +\infty[$, l’application des prop. 1 et 3 de V, p. 27, donne les critères suivants:

**Proposition 4** (*critère logarithmique d’ordre 0*). — Soit $(u_n)$ une série à termes positifs; si $u_n \leq n^\mu$ pour un $\mu < -1$, la série $(u_n)$ est convergente; si $u_n \geq n^\mu$ pour un $\mu \geq -1$, la série $(u_n)$ a une somme infinie.

**Proposition 5** (*critère logarithmique d’ordre $p$*). — Soit $(u_n)$ une série à termes positifs. Si $u_n \leq \frac{1}{n.l_1(n).l_2(n)\ldots l_{p-1}(n)\,(l_p(n))^\mu}$ pour un $\mu > 1$, la série $(u_n)$ est convergente; si $u_n \geq \frac{1}{n.l_1(n)\ldots l_{p-1}(n)\,(l_p(n))^\mu}$ pour un $\mu \leq 1$, la série $(u_n)$ a une somme infinie.

Si $0 \leq q < 1$, on a $q^n \leq n^{-\mu}$ quel que soit $\mu > 0$; l’application du critère logarithmique d’ordre 0 prouve à nouveau la convergence de la série géométrique $\sum_{n=0}^\infty q^n$ pour $|q| < 1$ (TG, IV, p. 32). Si on applique la prop. 1 en prenant $v_n = q^n$ on obtient un critère qui peut se mettre sous la forme suivante (*critère de Cauchy*): Soit $(u_n)$ une série à termes positifs; si $\limsup (u_n)^{1/n} < 1$, la série $(u_n)$ est convergente; si $\limsup (u_n)^{1/n} > 1$, la série $(u_n)$ a une somme infinie. En effet, si $\limsup (u_n)^{1/n} = a < 1$, pour tout nombre $q$ tel que $a < q < 1$, on a $u_n \leq q^n$. Si au contraire $\limsup (u_n)^{1/n} = a > 1$, pour tout $q$ tel que $1 < q < a$, on a $u_n \geq q^n > 1$ pour une infinité de valeurs de $n$; $u_n$ ne tendant pas vers 0, on a $\sum_{n=1}^\infty u_n = +\infty$.

Ce critère est fort utile dans la théorie des séries entières, que nous étudierons plus tard; mais il ne permet déjà plus de décider de la convergence des séries $(1/n^\alpha)$, autrement dit son champ d’application est beaucoup plus restreint que celui des critères logarithmiques.

### 2. Développement asymptotique des sommes partielles d’une série

Pour $x$ réel tendant vers $+\infty$, soit $\mathscr{E}$ une échelle de comparaison formée de fonctions dont chacune est définie dans tout un intervalle $[x_0, +\infty[$ (dépendant de la fonction) et est $\geq 0$ dans cet intervalle. Soit $(\mathbf{u}_n)$ une série dont les termes appartiennent à un espace normé complet $E$, telle que $\mathbf{u}_n$ admette un développement asymptotique à la précision $g_\alpha$ par rapport à l’échelle $\mathscr{E}^\alpha$ des restrictions à $\mathbf{N}$ des fonctions de $\mathscr{E}$:

$$
\mathbf{u}_n = \sum_{\lambda \leq \alpha} a_\lambda g_\lambda(n) + r_\alpha(n).
$$

Supposons que toute somme partielle $\sum_{m=1}^{n} g(m)$ où $g \in \mathcal{E}$, admette un développement asymptotique par rapport à $\mathcal{E}'$. On peut alors obtenir un développement asymptotique de $s_n = \sum_{m=1}^{n} u_m$ par rapport à $\mathcal{E}'$; nous distinguerons encore deux cas:

$1^\circ \sum_{n=1}^{\infty} g_{\alpha}(n) = +\infty$. Alors (V, p. 27, prop. 2), on a $\sum_{m=1}^{n} r_{\alpha}(m) \ll \sum_{m=1}^{n} g_{\alpha}(m)$; par hypothèse, on peut obtenir un développement asymptotique de

$$
\sum_{\lambda < \alpha} a_{\lambda} \left( \sum_{m=1}^{n} g(m) \right)
$$

(V, p. 13) à une certaine précision $g_p$; si $c g_{\sigma}(n)$ est la partie principale de $\sum_{m=1}^{n} g_{\alpha}(m)$, on aura un développement asymptotique de $s_n$ à la précision $g_{\min(\rho,\sigma)}$.

$2^\circ \sum_{n=1}^{\infty} g_{\alpha}(n)$ est convergente; soit alors $\beta$ le plus petit des indices $\lambda \leq \alpha$ tels que $a_{\lambda} \neq 0$ et que $\sum_{n=1}^{\infty} g_{\lambda}(n)$ soit convergente; la série

$$
C = \sum_{n=1}^{\infty} \left( u_n - \sum_{\lambda < \beta} a_{\lambda} g_{\lambda}(n) \right)
$$

est alors absolument convergente, et on peut écrire

$$
s_n = \sum_{\lambda < \beta} a_{\lambda} \left( \sum_{m=1}^{n} g_{\lambda}(m) \right) + C - \sum_{\beta \leq \lambda \leq \alpha} a_{\lambda} \left( \sum_{m=n+1}^{\infty} g_{\lambda}(m) \right) - \sum_{m=n+1}^{\infty} r_{\alpha}(m).
$$

On a en outre $\sum_{m=n+1}^{\infty} r_{\alpha}(m) \ll \sum_{m=n+1}^{\infty} g_{\alpha}(m)$; si $c g_{\sigma}(n)$ est la partie principale de $\sum_{m=n+1}^{\infty} g_{\alpha}(m)$, et si on a un développement asymptotique de

$$
\sum_{\lambda < \beta} a_{\lambda} \left( \sum_{m=1}^{n} g_{\lambda}(m) \right) + C - \sum_{\beta \leq \lambda \leq \alpha} a_{\lambda} \left( \sum_{m=n+1}^{\infty} g_{\lambda}(m) \right)
$$

à la précision $g_p$, on obtiendra ainsi un développement asymptotique de $s_n$ à la précision $g_{\min(\rho,\sigma)}$.

On est ainsi ramené au cas particulier des séries $(g(n))$ où $g \in \mathcal{E}$. Nous allons voir comment, moyennant certaines conditions, on peut tout d’abord obtenir une partie principale de $s_n = \sum_{m=1}^{n} g(m)$ (lorsque $\sum_{n=1}^{\infty} g(n) = +\infty$) ou de $r_n = \sum_{m=n+1}^{\infty} g(m)$ (lorsque $\sum_{n=1}^{\infty} g(n) < +\infty$).

#### Proposition 6 {#fvr-v-s4-prop-6 .statement}

*Soit g une fonction numérique > 0 et monotone définie dans un intervalle $[x_0, +\infty[$ (où $x_0 \leq 1$), et telle que log g et x soient comparables d’ordre 1.*

1° Si g est d'ordre infini par rapport à $e^x$, on a

(1) $$
s_n = \sum_{m=1}^n g(m) \sim g(n) \quad \text{si } \sum_{n=1}^\infty g(n) = +\infty;
$$

(2) $$
r_n = \sum_{m=n+1}^\infty g(m) \sim g(n+1) \quad \text{si } \sum_{n=1}^\infty g(n) < +\infty.
$$

2° Si g est d'ordre fini $\mu$ par rapport à $e^x$, on a

(3) $$
s_n = \sum_{m=1}^n g(m) \sim \frac{\mu}{1 - e^{-\mu}} \int_{x_0}^n g(t)\, dt \quad \text{si } \sum_{n=1}^\infty g(n) = +\infty;
$$

(4) $$
r_n = \sum_{m=n+1}^\infty g(m) \sim \frac{\mu}{1 - e^{-\mu}} \int_n^\infty g(t)\, dt \quad \text{si } \sum_{n=1}^\infty g(n) < +\infty
$$

(le nombre $\frac{\mu}{1 - e^{-\mu}}$ devant être remplacé par 1 dans (3) et (4) lorsque $\mu = 0$).

1° Si g est d'ordre $+\infty$ par rapport à $e^x$, on a $\log g \gg x$, d'où $g'/g \gg 1$ ou $g' \gg g$ d'après l'hypothèse; g est donc croissante et tend vers $+\infty$ avec $x$, d'où $\sum_{n=1}^\infty g(n) = +\infty$. Si u est la fonction en escalier associée à la série $(g(n))$ (V, p. 27), on a $u(x) \leqslant g(x)$ à partir d'une certaine valeur de $x$, donc $u \ll g$ et par suite

$$
s_{n-1} = \int_1^n u(t)\, dt \ll \int_1^n g(t)\, dt \ll \int_1^n g'(t)\, dt \sim g(n);
$$

comme $s_n = s_{n-1} + g(n)$, on a bien $s_n \sim g(n)$. Démonstration analogue lorsque g est d'ordre $-\infty$ par rapport à $e^x$; on a alors la formule (2).

2° Si g est d'ordre $\mu$ par rapport à $e^x$, on peut écrire $g(x) = e^{\mu x} h(x)$, où h est d'ordre 0 par rapport à $e^x$; en outre, par hypothèse, $\log g \sim \mu x$ pour $\mu \neq 0$ ($\log g \ll x$ pour $\mu = 0$) entraîne $h' \ll h$. Supposons d'abord que $\sum_{n=1}^\infty g(n) = +\infty$ (ce qui implique $\mu \geqslant 0$, et est réciproquement toujours vérifié si $\mu > 0$, puisqu'alors $g(x)$ tend vers $+\infty$ avec $x$); évaluons une partie principale de $\int_{n-1}^n g(t)\, dt$. On peut écrire

$$
\int_{n-1}^n g(t)\, dt = \int_{n-1}^n e^{\mu t} h(t)\, dt = h(n) \int_{n-1}^n e^{\mu t}\, dt + \int_{n-1}^n e^{\mu t}(h(t) - h(n))\, dt
$$
$$
= \frac{1 - e^{-\mu}}{\mu} g(n) + \int_{n-1}^n e^{\mu t}(h(t) - h(n))\, dt.
$$

Or, la relation $h' \ll h$ signifie que, pour tout $\varepsilon > 0$, il existe $n_0$ tel que la relation $x \geqslant n_0$ entraîne $|h'(x)/h(x)| \leqslant \varepsilon$; on en déduit, pour $n-1 \leqslant t \leqslant n$, que $-\varepsilon \leq \log |h(t)/h(n)| \leq \varepsilon$ d’après le th. des accroissements finis, si $n \geq n_0$, d’où
$$
|h(t) - h(n)| \leq (e^\varepsilon - 1)h(n)
$$
et par suite
$$
\left| \int_{n-1}^n e^{ut}(h(t) - h(n))\,dt \right| \leq (e^\varepsilon - 1)e^{un}h(n) = (e^\varepsilon - 1)g(n)
$$
puisque $e^{ut}$ est croissante. Comme $e^\varepsilon - 1$ est arbitrairement petit avec $\varepsilon$, on voit qu’on peut écrire
$$
\int_{n-1}^n g(t)\,dt = \frac{1 - e^{-\mu}}{\mu} g(n) + o(g(n))
$$
$(\frac{1 - e^{-\mu}}{\mu}$ étant remplacé par 1 lorsque $\mu = 0$). La proposition est alors une conséquence de la prop. 2 de V, p. 27. On raisonne de même lorsque $\sum_{n=1}^\infty g(n)$ est finie.

Par application répétée de la prop. 6 de V, p. 29, on peut parfois obtenir un développement asymptotique de $s_n = \sum_{m=1}^n g(m)$. Supposons d’abord que $g$ soit d’ordre $+\infty$ par rapport à $e^x$; pour toute valeur fixe de $p$, on peut écrire, d’après la prop. 6,
$$
s_n = g(n) + g(n-1) + \cdots + g(n-p) + o(g(n-p))
$$
et il suffira de développer (relativement à $e^x$) chacune des fonctions $g(n-k)$ ($0 \leq k \leq p$) en limitant la précision de ces développements à la partie principale de $g(n-p)$, pour avoir un développement de $s_n$.

#### Exemple {#fvr-v-s4-n2-exa-1 .statement}

Soit $g(x) = x^x = \exp(x \log x)$, d’ordre $+\infty$ par rapport à $e^x$. En prenant $p = 2$, on a
$$
(n-1) \log (n-1) = (n-1) \log n - 1 + \frac{1}{2n} + o\left(\frac{1}{n}\right)
$$
d’où (V, p. 16)
$$
(n-1)^{n-1} = \frac{1}{e} n^{n-1} + \frac{1}{2e} n^{n-2} + o_1(n^{n-2})
$$
et de même
$$
(n-2)^{n-2} = \frac{1}{e^2} n^{n-2} + o_2(n^{n-2});
$$
par suite
$$
s_n = n^n + \frac{1}{e} n^{n-1} + \left(\frac{1}{2e} + \frac{1}{e^2}\right) n^{n-2} + o_3(n^{n-2}).
$$

On procède de même (pour $r_n$) lorsque $g$ est d’ordre $-\infty$ par rapport à $e^x$.

Si maintenant $g$ est d’ordre fini $\mu$ par rapport à $e^x$, et si par exemple $\sum_{n=1}^\infty g(n) = +\infty$, on peut écrire

$$
s_n = \frac{\mu}{1 - e^{-\mu}} \int_1^n g(t) \, dt + \sum_{m=1}^n f_1(m)
$$
où $f_1(n) = g(n) - \frac{\mu}{1 - e^{-\mu}} \int_{n-1}^n g(t) \, dt \ll g(n)$ d’après la prop. 6 de V, p. 29. Si on a une partie principale $c g_1(n)$ de $f_1(n)$ par rapport à $\mathscr{E}'$, et si on peut appliquer de nouveau la prop. 6 à la fonction $g_1$, on obtiendra une primitive équivalente à $\sum_{m=1}^n f_1(m)$ si $\sum_{n=1}^\infty g_1(n) = +\infty$, équivalente à $\sum_{m=n+1}^\infty f_1(m)$ dans le cas contraire (dans ce dernier cas, on écrit $\sum_{m=1}^n f_1(m) = C - \sum_{m=n+1}^\infty f_1(m)$, avec $C = \sum_{n=1}^\infty f_1(n)$).

De proche en proche, on peut obtenir ainsi éventuellement une expression de $s_n$ sous forme de la somme d’un certain nombre de primitives, dont chacune est négligeable devant la précédente, d’un terme restant négligeable devant la dernière primitive écrite, et éventuellement d’une constante (cas où le terme restant tend vers 0). Il reste ensuite à développer chacune des primitives obtenues relativement à $\mathscr{E}'$ (cf. V, p. 25).

#### Exemple {#fvr-v-s4-n2-exa-2 .statement}

Soit $g(n) = \frac{1}{n}$; on a
$$
s_n = \sum_{m=1}^n \frac{1}{m} \sim \int_1^n \frac{dt}{t} = \log n
$$
puis
$$
\frac{1}{n} - (\log n - \log (n-1)) \sim - \frac{1}{2n^2}
$$
d’où
$$
s_n = \log n + \gamma + \frac{1}{2n} + o\left(\frac{1}{n}\right).
$$
La constante $\gamma$ qui s’introduit dans cette formule joue un rôle important en Analyse (cf. chap. VI et VII); elle est connue sous le nom de *constante d’Euler*; on a
$$
\gamma = 0,577\ 215\ 664...
$$
à $1/10^8$ près par défaut.

Nous verrons dans VI, p. 20, comment la *formule sommatoire d’Euler-Maclaurin* donne, dans les cas les plus importants, un développement asymptotique d’ordre *quelconque* de $s_n$ (ou de $r_n$).

### 3. Développement asymptotique des produits partiels d’un produit infini

On sait (TG, V, p. 14) que, pour que le produit infini de facteur général $1 + u_n$ ($u_n > -1$) soit convergent (resp. commutativement convergent), il faut et il suffit que la série de terme général $\log (1 + u_n)$ soit convergente (resp. commutativement convergente), et que l’on a alors la relation
$$
\log \prod_{n=1}^\infty (1 + u_n) = \sum_{n=1}^\infty \log (1 + u_n).
$$

Lorsque le produit infini est convergent, on sait que $u_n$ tend vers 0; on a donc $\log(1 + u_n) \sim u_n$; or, on sait que, pour qu’une série de nombres réels soit commutativement convergente, il faut et il suffit qu’elle soit absolument convergente (TG, IV, p. 39, prop. 5); en vertu de la prop. 1, on retrouve ainsi que, pour que le produit de facteur général $1 + u_n$ soit commutativement convergent, il faut et il suffit que la série de terme général $u_n$ soit absolument convergente (TG, IV, p. 35, th. 4).

Un raisonnement analogue s’applique à un produit infini de facteur général complexe $1 + u_n$ ($u_n \neq -1$). En effet, pour qu’un tel produit soit commutativement convergent, il faut et il suffit (TG, VIII, p. 16, prop. 2) que le produit infini de facteur général $|1 + u_n|$ le soit, et en outre, si $\theta_n$ est l’amplitude de $1 + u_n$ (comprise entre $-\pi$ et $+\pi$), que la série des $\theta_n$ soit commutativement convergente. Comme $u_n$ tend alors vers 0, $\log(1 + u_n)$ est défini à partir d’une certaine valeur de $n$ (III, p. 10) et on a
$$
\log(1 + u_n) = \log |1 + u_n| + i \theta_n;
$$
donc, pour que le produit de facteur général $1 + u_n$ soit commutativement convergent il faut et il suffit que la série de terme général $|\log(1 + u_n)|$ soit absolument convergente (TG, VII, p. 16, th. 1); or $\log(1 + u_n) \sim u_n$ (I, p. 26, prop. 5), donc on retrouve la condition que la série de terme général $u_n$ soit absolument convergente (TG, VIII, p. 16, th. 1).

La relation entre produits infinis et séries de nombres réels permet parfois d’obtenir un développement asymptotique du produit partiel $p_n = \prod_{k=1}^n (1 + u_k)$; il suffit d’avoir un développement asymptotique de la somme partielle $s_n = \sum_{k=1}^n \log (1 + u_k)$, puis de développer $p_n = \exp(s_n)$; on est donc ramené à deux problèmes examinés antérieurement (V, p. 28, et p. 16).

Exemple : formule de Stirling. — Cherchons un développement asymptotique de $n!$; on est ramené à développer $s_n = \sum_{p=1}^n \log p$, puis $\exp(s_n)$. La méthode du no 2 donne successivement
$$
s_n = \sum_{p=1}^n \log p \sim \int_1^n \log t \, dt = n \log n - n + 1
$$
puis
$$
\log n - \int_{n-1}^n \log t \, dt = \log n - (n \log n - (n-1) \log (n-1) - 1) \sim \frac{1}{2n}
$$
d’où
$$
s_n = n \log n - n + \frac{1}{2} \log n + o(\log n).
$$
On a ensuite
$$
\log n - \int_{n-1}^n \log t \, dt - \frac{1}{2} (\log n - \log (n-1)) \sim - \frac{1}{12n^2}
$$
d’où
$$
s_n = n \log n - n + \frac{1}{2} \log n + k + \frac{1}{12n} + o_1\left(\frac{1}{n}\right) \quad (k \text{ constante})
$$

et on tire finalement (V, p. 16)

$$
n! = e^{k n + 1/2} e^{-n} \left(1 + \frac{1}{12n} + o_2 \left(\frac{1}{n}\right)\right).
$$

Nous démontrerons dans VII, p. 17, qu’on a $e^x = \sqrt{2\pi}$. La formule (5) (avec cette valeur de $k$) est dite *formule de Stirling*. De la même manière, pour tout nombre réel $a$ distinct d’un entier $> 0$, on démontre que

$$(a+1)(a+2)\ldots(a+n) \sim K(a)n^{n+a+\frac{1}{2}}e^{-n}.$$

Nous déterminerons également la fonction $K(a)$ (VII, p. 18). Des formules (5) et (6) on tire en particulier

$$\binom{a}{n} \sim (-1)^n \varphi(a)n^{-a-1}$$

pour tout nombre réel $a$ distinct d’un entier $> 0$, $\varphi(a)$ étant une fonction de $a$ qui sera précisée dans VII, p. 18.

### 4. Application : critères de convergence de seconde espèce pour les séries à termes positifs

On rencontre assez souvent des séries $(u_n)$, pour lesquelles $u_n > 0$ à partir d’un certain rang, et $u_{n+1}/u_n$ a un développement asymptotique facile à déterminer. Il est commode, pour de telles séries, d’avoir des critères (dits *critères de seconde espèce*) permettant de déterminer si la série est convergente d’après le seul aspect de $u_{n+1}/u_n$. Un tel critère est le suivant:

**Proposition 7** (*critère de Raabe*). — *Soit* $(u_n)$ *une série à termes* $> 0$ *à partir d’un certain rang. Si, à partir d’un certain rang,*
$$ u_{n+1}/u_n \leq 1 - \frac{\alpha}{n} \text{ pour un } \alpha > 1,$$
*la série* $(u_n)$ *est convergente ; si à partir d’un certain rang,*
$$ u_{n+1}/u_n \geq 1 - \frac{1}{n},$$
*la série* $(u_n)$ *a une somme infinie.*

En effet, si $u_{n+1}/u_n \leq 1 - \frac{\alpha}{n}$ avec $\alpha > 1$, pour tout $n \geq n_0$, on a $u_n \leq p_n = \prod_{k=n_0}^n \left(1 - \frac{\alpha}{k}\right)$. Or, on a $\log \left(1 - \frac{\alpha}{n}\right) = -\frac{\alpha}{n} - \frac{n^2}{2n^2} + o\left(\frac{1}{n^2}\right)$, d’où $\log p_n = -\alpha \log n + k + o(1/n)$ ($k$ constante), et $p_n \sim e^k \frac{1}{n^\alpha}$; comme $\alpha > 1$, le critère logarithmique d’ordre 0 permet de conclure.

Si au contraire $u_{n+1}/u_n \geq 1 - \frac{1}{n}$ à partir d’un certain rang, le même calcul prouve que $u_n \geq \frac{1}{n}$ d’où la proposition.

On démontrerait de la même manière, en utilisant les critères logarithmiques d’ordre $> 0$, le critère de seconde espèce suivant:

#### Proposition 8 {#fvr-v-s4-prop-8 .statement}

Soit $(u_n)$ une série à termes $> 0$ à partir d’un certain rang. Si, à partir d’un certain rang, on a
$$
\frac{u_{n+1}}{u_n} \leq 1 - \frac{1}{n} - \frac{1}{n.l_1(n)} - \ldots
$$
$$
- \frac{1}{n.l_1(n).l_2(n) \ldots l_{p-1}(n)} - \frac{\alpha}{n.l_1(n).l_2(n) \ldots l_p(n)}
$$
pour un $\alpha > 1$, la série $(u_n)$ est convergente ; si, à partir d’un certain rang, on a
$$
\frac{u_{n+1}}{u_n} \geq 1 - \frac{1}{n} - \frac{1}{n.l_1(n)} - \ldots - \frac{1}{n.l_1(n).l_2(n) \ldots l_p(n)}
$$
la série $(u_n)$ a une somme infinie.

#### Exemple {#fvr-v-s4-n4-exa-1 .statement}

Considérons la série hypergéométrique, de terme général
$$
u_n = \frac{\alpha(\alpha + 1) \ldots (\alpha + n - 1) \beta(\beta + 1) \ldots (\beta + n - 1)}{1.2 \ldots n. \gamma(\gamma + 1) \ldots (\gamma + n - 1)}
$$
où $\alpha, \beta, \gamma$ sont des nombres réels quelconques, différents des entiers $\leq 0$ ; il est clair que $u_n$ est $> 0$ à partir d’un certain rang, ou $< 0$ à partir d’un certain rang. On a
$$
\frac{u_{n+1}}{u_n} = \frac{(\alpha + n)(\beta + n)}{(n + 1)(\gamma + n)} = \left(1 + \frac{\alpha + \beta}{n} + \frac{\alpha \beta}{n^2}\right) \left(1 + \frac{\gamma + 1}{n} + \frac{\gamma}{n^2}\right)^{-1}
$$
$$
= 1 + \frac{\alpha + \beta - \gamma - 1}{n} + \frac{\alpha \beta - (\alpha + \beta)(\gamma + 1) + \gamma^2 + \gamma + 1}{n^2} + o\left(\frac{1}{n^2}\right).
$$

Le critère de Raabe montre donc que la série est convergente pour $\alpha + \beta < \gamma$, et a une somme infinie pour $\alpha + \beta > \gamma$ ; lorsque $\alpha + \beta = \gamma$, la série a encore une somme infinie, comme le montre la prop. 8.

#### Remarque 1 {#fvr-v-s4-n4-rem-1 .statement}

Comme cas particulier du critère de Raabe, on voit que si $\limsup_{n \to \infty} u_{n+1}/u_n < 1$, la série $(u_n)$ est convergente ; si au contraire $\liminf_{n \to \infty} u_{n+1}/u_n > 1$, la série a une somme infinie (critère de d’Alembert).

#### Remarque 2 {#fvr-v-s4-n4-rem-2 .statement}

Les critères de seconde espèce ne peuvent s’appliquer qu’à des séries dont le terme général se comporte de façon très régulière lorsque $n$ tend vers $+\infty$ ; autrement dit, leur champ d’application est bien plus restreint que celui des critères logarithmiques, et ce serait une maladresse que de vouloir les utiliser en dehors des cas spéciaux auxquels ils sont particulièrement adaptés. Par exemple, pour la série $(u_n)$ définie par $u_{2m} = 2^{-m}$, $u_{2m+1} = 3^{-m}$, on a $u_{2m+1}/u_{2m} = (\frac{3}{2})^m$, $u_{2m+2}/u_{2m+1} = \frac{1}{2}(\frac{3}{2})^m$ ; le premier de ces rapports tend vers 0 et le second vers $+\infty$ lorsque $m$ croît indéfiniment, donc aucun critère de seconde espèce n’est applicable ; cependant, comme $u_n \leq 2^{-n/2}$, il est immédiat que la série est convergente.

Même lorsque $u_{n+1}/u_n$ a une expression simple, une évaluation directe d’une partie principale de $u_n$ conduit souvent au résultat aussi vite que les critères de seconde espèce. Par exemple, pour la série hypergéométrique, la formule de Stirling montre aussitôt que $u_n \sim a n^{\alpha + \beta - \gamma - 1}$, où $a$ est une constante $\neq 0$, et le critère logarithmique d’ordre 0 est par suite applicable.

## EXERCICES {#fvr-v-s4-exercises}

See the [exercises for § 4](exercises/s4/).
