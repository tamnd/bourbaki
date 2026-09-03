---
book: int
book_title: Integration
chapter: VII
chapter_title: Mesure de Haar
section: 1
section_title: Construction d'une mesure de Haar
lang: fr
source: int-vii-viii-fr
pdf_pages: 0006-0037, 0099-0110
extraction: ocr
subsections:
    - "no": 1
      title: Définitions et notations.
      page: 0
      pdf_page: 6
    - "no": 2
      title: Le théorème d’existence et d’unicité.
      page: 0
      pdf_page: 12
    - "no": 3
      title: Module.
      page: 0
      pdf_page: 17
    - "no": 4
      title: Module d'un automorphisme.
      page: 0
      pdf_page: 20
    - "no": 5
      title: Mesure de Haar d'un produit.
      page: 0
      pdf_page: 21
    - "no": 6
      title: Mesure de Haar d’une limite projective.
      page: 0
      pdf_page: 22
    - "no": 7
      title: Définition locale d’une mesure de Haar.
      page: 0
      pdf_page: 27
    - "no": 8
      title: Mesures relativement invariantes.
      page: 0
      pdf_page: 28
    - "no": 9
      title: '*Mesures quasi-invariantes.*'
      page: 0
      pdf_page: 29
    - "no": 10
      title: Corps localement compacts.
      page: 0
      pdf_page: 31
    - "no": 11
      title: Algèbres de dimension finie sur un corps localement compact.
      page: 0
      pdf_page: 36
statements: 50
exercises: 30
content_sha256: f072591059dd7b101cc550f66919f7fb096329c53ac2e20f8fd1ce7da768b66e
---

## § 1. Construction d'une mesure de Haar.

### 1. Définitions et notations.

Soit G un groupe topologique opérant continûment à gauche (Top. gén., chap. III, 3e éd., § 2, n° 4) dans un espace localement compact X ; pour s ∈ G et x ∈ X, soit sx le transformé de x par s. On notera γ_X(s), ou γ(s), l’homéomorphisme de X sur X défini par

(1) $\gamma(s)x = sx.$

On a

(2) $\gamma(st) = \gamma(s)\gamma(t).$

Si f est une fonction définie sur X, $\gamma(s)f$ sera définie par transport de structure, c’est-à-dire par la formule $(\gamma(s)f)(\gamma(s)x) = f(x)$; autrement dit :

(3) $(\gamma(s)f)(x) = f(s^{-1}x).$

Si μ est une mesure définie sur X, $\gamma(s)\mu$ sera aussi définie par transport de structure, ce qui conduit à

(4) $\langle f, \gamma(s)\mu \rangle = \langle \gamma(s^{-1})f, \mu \rangle$ pour $f \in \mathcal{K}(X)$.

Autrement dit

(5) $\int_X f(x)d(\gamma(s)\mu)(x) = \int_X f(sx)d\mu(x).$

Si A est un ensemble $(\gamma(s)\mu)$-intégrable, $s^{-1}A$ est $\mu$-intégrable, et

(6) $(\gamma(s)\mu)(A) = \mu(s^{-1}A).$

La mesure $\gamma(s)\mu$ peut aussi être définie comme l’image de $\mu$ par $\gamma(s)$.

Au lieu d’écrire $d(\gamma(s)\mu)(x)$, il est parfois commode d’écrire $d\mu(s^{-1}x)$; alors, (5) prend la forme suivante :

$$ \int_X f(x)d\mu(s^{-1}x) = \int_X f(sx)d\mu(x); $$

le membre de droite se déduit de celui de gauche « en changeant x en sx ».

#### Définition 1 {#int-vii-s1-def-1 .statement}

Soit $\mu$ une mesure sur X.
a) On dit que $\mu$ est invariante par G si $\gamma(s)\mu = \mu$ pour tout $s \in G$.

b) On dit que $\mu$ est relativement invariante par $G$ si $\gamma(s)\mu$ est proportionnelle à $\mu$ pour tout $s \in G$.

c) On dit que $\mu$ est quasi-invariante par $G$ si $\gamma(s)\mu$ est équivalente à $\mu$ pour tout $s \in G$.

#### Remarque 1 {#int-vii-s1-n1-rem-1 .statement}

Supposons $\mu$ invariante. Alors $|\mu|$, $\Re \mu$, $\mathcal{I}\mu$ sont invariantes. Si $\mu$ est réelle, $\mu^+$ et $\mu^-$ sont invariantes.

#### Remarque 2 {#int-vii-s1-n1-rem-2 .statement}

Supposons $\mu$ relativement invariante et non nulle. Il existe, pour tout $s \in G$, un nombre complexe $\chi(s)$ unique tel que

$$
\gamma(s)\mu = \chi(s)^{-1}\mu
$$

et la fonction $\chi$ sur $G$ est une représentation de $G$ dans $\mathbf{C}^*$ appelée multiplicateur de $\mu$. La formule (5) donne alors

$$
\int_X f(sx)d\mu(x) = \chi(s)^{-1}\int_X f(x)d\mu(x)
$$

et la formule (6) donne

$$
\mu(sA) = \chi(s)\mu(A).
$$

Avec les conventions faites plus haut, (7) peut aussi s'écrire

$$
d\mu(sx) = \chi(s)d\mu(x).
$$

#### Remarque 3 {#int-vii-s1-n1-rem-3 .statement}

Comme $|\gamma(s)\mu| = \gamma(s)(|\mu|)$, dire que $\mu$ est quasi-invariante revient à dire que $|\mu|$ est quasi-invariante.

Si $\mu$ est quasi-invariante et si $\mu'$ est une autre mesure sur $X$ équivalente à $\mu$, $\gamma(s)\mu'$ est équivalente à $\gamma(s)\mu$, donc à $\mu$, donc à $\mu'$, de sorte que $\mu'$ est quasi-invariante. Dire que $\mu$ est quasi-invariante par $G$ signifie donc que la classe de $\mu$ est invariante par $G$.

Pour que $\mu$ soit quasi-invariante, il faut et il suffit que l'ensemble des parties localement $\mu$-négligeables de $X$ soit invariant par $G$ (chap. V, § 5, n° 5, th. 2), ou encore que, pour toute partie compacte $\mu$-négligeable $K$ de $X$ et tout $s \in G$, $sK$ soit $\mu$-négligeable (*loc. cit.*, Remarque).

Si $\mu$ est quasi-invariante, le support de $\mu$ est invariant par G. En particulier, si G est transitif dans X, ce support est ou bien vide (si $\mu = 0$) ou bien égal à X (si $\mu \neq 0$).

#### Lemme 1 {#int-vii-s1-lem-1 .statement}

Soient X, Y, Z trois espaces topologiques, Y étant localement compact. Soit $(x, y) \to xy$ une application continue de $X \times Y$ dans Z, qui définit une application $x \to u_x$ de X dans $\mathcal{F}(Y; Z)$ par la relation $u_x(y) = xy$. Soient $f$ une fonction continue dans Z, à valeurs dans $\overline{\mathbf{R}}$ ou dans un espace de Banach, S le support de $f$, et $µ$ une mesure sur Y. On suppose que, pour tout $x_0 \in X$, il existe un voisinage V de $x_0$ dans X tel que $\bigcup_{x \in V} u_x^{-1}(S)$ soit relativement compact dans Y. Alors :

a) pour tout $x \in X$, $f \circ u_x$ est continue dans Y et à support compact ;

b) l’application $x \to \int_Y f(xy)d\mu(y)$, qui est définie d’après a), est continue dans X.

L’assertion a) est évidente. Prouvons b). Comme la continuité est une propriété locale, on se ramène au cas où $\bigcup_{x \in X} u_x^{-1}(S)$ est contenu dans une partie compacte $Y'$ de Y. Comme la fonction $(x, y) \to f(xy)$ est continue dans $X \times Y$, $f \circ u_x$ tend uniformément dans $Y'$ vers $f \circ u_{x_0}$ quand $x$ tend vers $x_0$ (Top. Gén., chap. X, 2e éd., § 3, no 4, th. 3), donc $\mu(f \circ u_x)$ tend vers $\mu(f \circ u_{x_0})$. D’où le lemme.

Revenons maintenant aux notations antérieures.

#### Proposition 1 {#int-vii-s1-prop-1 .statement}

Supposons G localement compact. Soit $µ$ une mesure relativement invariante non nulle sur X. Alors son multiplicateur $χ$ est une fonction continue dans G.

En effet, soient $f \in \mathcal{H}(X)$, S le support de $f$, $s_0$ un point de G, et V un voisinage compact de $s_0$ dans G ; alors

$$
\bigcup_{s \in V} γ(s)^{-1}(S) = V^{-1}S
$$

est compact dans X ; d’après le lemme 1 et la formule (8), $\chi(s)^{-1}\langle \mu, f \rangle$ dépend continûment de s ; si on a choisi $f$ telle que $\langle \mu, f \rangle \neq 0$, on voit que $\chi$ est continu.

Soit maintenant G un groupe topologique opérant continûment à droite dans un espace localement compact X ; pour $s \in G$ et $x \in X$, soit $xs$ le transformé de $x$ par $s$. On notera $\delta_X(s)$, ou $\delta(s)$, l’homéomorphisme de X défini par

(1')
$$
\delta(s)x = xs^{-1}.
$$
On a
(2')
$$
\delta(st) = \delta(s)\delta(t).
$$

Par transport de structure, on définit l’action de $\delta(s)$ sur les fonctions et les mesures sur X :

(3')
$$
(\delta(s)f)(x) = f(xs)
$$
(4')
$$
\langle f, \delta(s)\mu \rangle = \langle \delta(s^{-1})f, \mu \rangle
$$
(5')
$$
\int_X f(x)d(\delta(s)\mu)(x) = \int_X f(xs^{-1})d\mu(x)
$$
(6')
$$
(\delta(s)\mu)(A) = \mu(As).
$$

On convient d’écrire $d\mu(xs)$ au lieu de $d(\delta(s)\mu)(x)$, et (5') prend la forme
$$
\int_X f(x)d\mu(xs) = \int_X f(xs^{-1})d\mu(x).
$$

On définit de manière analogue les mesures invariantes, relativement invariantes et quasi-invariantes par G sur X. Si $\mu$ est relativement invariante, on définit son multiplicateur $\chi$ par les formules

(7')
$$
\delta(s)\mu = \chi(s)\mu
$$
(8')
$$
\int_X f(xs)d\mu(x) = \chi(s)^{-1}\int_X f(x)d\mu(x)
$$

(9') $\mu(As) = \chi(s)\mu(A).$

(10') $d\mu(xs) = \chi(s)d\mu(x).$

Si on considère le groupe opposé $G^o$ à $G$ comme opérant dans $X$ par $(x, s) \to xs$, $\mu$ est relativement invariante par $G^o$ de même multiplicateur $\chi$.

Soit enfin $G$ un groupe localement compact. Il opère sur lui-même par translations à gauche et à droite, suivant les formules $\gamma(s)x = sx$, $\delta(s)x = xs^{-1}$. On a

(11) $\gamma(s)\delta(t) = \delta(t)\gamma(s).$

Tout ce qui précède est applicable, et on a donc, sur $G$, les notions de mesures invariantes à gauche, invariantes à droite, relativement invariantes à gauche, relativement invariantes à droite, quasi-invariantes à gauche, quasi-invariantes à droite (cf., toutefois, les nos 8 et 9).

L’application $x \to x^{-1}$ est un homéomorphisme de $G$ sur $G$. Pour toute fonction $f$ sur $G$, on définira la fonction $\tilde{f}$ sur $G$ par

(12) $\tilde{f}(x) = f(x^{-1}).$

Pour toute mesure $\mu$ sur $G$, on définira la mesure $\tilde{\mu}$ par

(13) $\tilde{\mu}(f) = \mu(\tilde{f}) \quad \text{pour } f \in \mathcal{K}(G).$

Autrement dit

(14) $\int_G f(x)d\tilde{\mu}(x) = \int_G f(x^{-1})d\mu(x).$

Si $A$ est un ensemble $\tilde{\mu}$-intégrable, $A^{-1}$ est $\mu$-intégrable, et

(15) $\tilde{\mu}(A) = \mu(A^{-1}).$

On convient d’écrire $d\mu(x^{-1})$ au lieu de $d\tilde{\mu}(x)$, et (14) prend la forme

$\int_G f(x)d\mu(x^{-1}) = \int_G f(x^{-1})d\mu(x).$

### 2. Le théorème d’existence et d’unicité.

#### Définition 2 {#int-vii-s1-def-2 .statement}

Soit G un groupe localement compact. On appelle mesure de Haar à gauche (resp. à droite) sur G une mesure positive non nulle sur G, invariante à gauche (resp. à droite).

#### Théorème 1 {#int-vii-s1-thm-1 .statement}

Sur tout groupe localement compact, il existe une mesure de Haar à gauche (resp. à droite), et, à un facteur constant près, il n’en existe qu’une.

A) Existence. — Posons $\mathcal{K}(G) = \mathcal{K}$, $\mathcal{K}_+(G) = \mathcal{K}_+$,

$$
\mathcal{K}_+^* = \mathcal{K}_+ - \{0\}.
$$

Si C est une partie compacte de G, on notera $\mathcal{K}_+^*(C)$ l’ensemble des $f \in \mathcal{K}_+^*$ à support dans C. Pour $f \in \mathcal{K}$ et $g \in \mathcal{K}_+^*$, il existe des nombres $c_1, \ldots, c_n \geq 0$ et des éléments $s_1, \ldots, s_n$ de G tels que $f \leq \sum_{i=1}^n c_i \gamma(s_i)g$ : en effet, il existe une partie ouverte non vide U de G telle que $\inf_{s \in U} g(s) > 0$, et le support de $f$ peut être recouvert par un nombre fini de translatés à gauche de U. Soit alors $(f : g)$ la borne inférieure des nombres $\sum_{i=1}^n c_i$ pour tous les systèmes $(c_1, \ldots, c_n, s_1, \ldots, s_n)$ de nombres $\geq 0$ et d’éléments de G tels que $f \leq \sum_{i=1}^n c_i \gamma(s_i)g$. On a :

(i) $(\gamma(s)f : g) = (f : g)$ pour $f \in \mathcal{K}$, $g \in \mathcal{K}_+^*$, $s \in G$;
(ii) $(\lambda f : g) = \lambda(f : g)$ pour $f \in \mathcal{K}$, $g \in \mathcal{K}_+^*$, $\lambda \geq 0$;
(iii) $((f + f') : g) \leq (f : g) + (f' : g)$ pour $f \in \mathcal{K}$, $f' \in \mathcal{K}$, $g \in \mathcal{K}_+^*$;
(iv) $(f : g) \geq (\sup f)/(\sup g)$ pour $f \in \mathcal{K}$, $g \in \mathcal{K}_+^*$;
(v) $(f : h) \leq (f : g)(g : h)$ pour $f \in \mathcal{K}$, $g \in \mathcal{K}_+^*$, $h \in \mathcal{K}_+^*$;
(vi) $0 < \frac{1}{(f_0 : f)} \leq \frac{(f : g)}{(f_0 : g)} \leq (f : f_0)$ pour $f, f_0, g$ dans $\mathcal{K}_+^*$;
(vii) soient $f, f', h$ dans $\mathcal{K}_+$ avec $h(s) \geq 1$ dans le support de $f + f'$, et soit $\varepsilon > 0$; il existe un voisinage compact V de e tel que, pour toute $g \in \mathcal{K}_+^*(V)$, on ait

$$
(f : g) + (f' : g) \leq ((f + f') : g) + \varepsilon(h : g).
$$

Les propriétés (i), (ii), (iii) sont évidentes. Soient $f \in \mathcal{K}$, $g \in \mathcal{K}_+^*$; si $f \leq \sum_{i=1}^n c_i \gamma(s_i)g$ avec des $c_i \geq 0$, on a
$$
\sup f \leq \sum_{i=1}^n c_i g(s_i^{-1}s)
$$
pour un $s \in G$, donc $\sup f \leq \left( \sum_{i=1}^n c_i \right) \sup g$, d'où (iv). Prouvons (v) ; soient $f \in \mathcal{K}$, $g, h$ dans $\mathcal{K}_+^*$; si $f \leq \sum_{i=1}^n c_i \gamma(s_i)g$ et $g \leq \sum_{j=1}^p d_j \gamma(t_j)h$ ($c_i \geq 0, \ d_j \geq 0, \ s_i, \ t_j$ dans $G$), on a
$$
f \leq \sum_{i,j} c_i d_j \gamma(s_i t_j)h,
$$
donc $(f : h) \leq \sum_{i,j} c_i d_j = \left( \sum_i c_i \right) \left( \sum_j d_j \right)$;
donc $(f : h) \leq (f : g)(g : h)$. Si on applique (v) à $f_0, f, g$ d'une part et à $f, f_0, g$ d'autre part, on obtient (vi). Enfin, soient $f, f', h$ dans $\mathcal{K}_+$ avec $h(s) \geq 1$ dans le support de $f + f'$, et soit $\varepsilon > 0$. Posons $F = f + f' + \frac{1}{2} \varepsilon h$; les fonctions $\varphi, \varphi'$, qui coïncident respectivement avec $f/F$ et $f'/F$ dans le support de $f + f'$ et qui sont nulles en dehors de celui-ci, appartiennent à $\mathcal{K}_+$; pour tout $\eta > 0$, il existe un voisinage compact $V$ de $e$ tel que $|\varphi(s) - \varphi(t)| \leq \eta$ et $|\varphi'(s) - \varphi'(t)| \leq \eta$ pour $s^{-1}t \in V$. Soit alors $g \in \mathcal{K}_+^*(V)$; pour tous $s \in G$, on a $\varphi \cdot \gamma(s)g \leq (\varphi(s) + \eta) \cdot \gamma(s)g$: en effet, c'est évident aux points où $\gamma(s)g$ s'annule, donc hors de $sV$; et, dans $sV$, on a $\varphi \leq \varphi(s) + \eta$; de même,
$$
\varphi' \cdot \gamma(s)g \leq (\varphi'(s) + \eta) \cdot \gamma(s)g.
$$
Ceci posé, soient $c_1, \ldots, c_n$ des nombres $\geq 0$ et $s_1, \ldots, s_n$ des éléments de $G$ tels que $F \leq \sum_{i=1}^n c_i \gamma(s_i)g$; on a
$$
f = \varphi F \leq \sum_{i=1}^n c_i \varphi \cdot \gamma(s_i)g \leq \sum_{i=1}^n c_i (\varphi(s_i) + \eta) \cdot \gamma(s_i)g
$$
et de même pour $f'$; par suite
$$
(f : g) + (f' : g) \leq \sum_{i=1}^n c_i (\varphi(s_i) + \varphi'(s_i) + 2\eta) \leq (1 + 2\eta) \sum_{i=1}^n c_i
$$

puisque $\varphi + \varphi' \leq 1$. En appliquant la définition de F, puis (ii), (iii), et (v), on en conclut

$$
(f : g) + (f' : g) \leq (1 + 2\eta)(F : g) \leq
$$
$$
(1 + 2\eta)[((f + f') : g) + \frac{1}{2} \varepsilon(h : g)] \leq ((f + f') : g) + \frac{1}{2} \varepsilon(h : g)
$$
$$
+ 2\eta((f + f') : h)(h : g) + \varepsilon\eta(h : g)
$$

et, si l’on a choisi $\eta$ tel que $\eta[2((f + f') : h) + \varepsilon] \leq \frac{1}{2} \varepsilon$, on obtient (vii).

Quand V parcourt l’ensemble des voisinages compacts de e, les $\mathcal{K}_+^*(V)$ forment une base d’un filtre $\mathfrak{B}$ sur $\mathcal{K}_+^*$. Soit $\mathfrak{F}$ un ultrafiltre sur $\mathcal{K}_+^*$ plus fin que $\mathfrak{B}$. D’autre part, fixons $f_0 \in \mathcal{K}_+^*$ et posons, pour $f \in \mathcal{K}_+^*$ et $g \in \mathcal{K}_+^*$

$$
I_g(f) = \frac{(f : g)}{(f_0 : g)}.
$$

D’après (vi), $\lim_{g, \mathfrak{F}} I_g(f) = I(f)$ existe dans l’espace compact $\{1/(f_0 : f), (f : f_0)\}$. D’après (iii), on a $I(f + f') \leq I(f) + I(f')$. D’après (vii), on a $I(f) + I(f') \leq I(f + f') + \varepsilon I(h)$ quel que soit $\varepsilon > 0$ si $h$ est $\geq 1$ dans le support de $f + f'$; il s’ensuit que $I(f + f') = I(f) + I(f')$. D’après le chap. II, § 2, no 1, prop. 2, I se prolonge en une forme linéaire sur $\mathcal{K}$; cette forme linéaire est une mesure positive non nulle sur G, invariant à gauche d’après (i) ; c’est la mesure de Haar à gauche cherchée. Passant au groupe opposé, on en déduit l’existence d’une mesure de Haar à droite.

B) Unicité. — Soient $\mu$ une mesure de Haar à gauche, $\nu$ une mesure de Haar à droite. Alors $\check{\nu}$ est une mesure de Haar à gauche. On va montrer que $\mu$ et $\check{\nu}$ sont proportionnelles. Ceci prouvera bien que deux mesures de Haar à gauche sont proportionnelles.

Soit $f \in \mathcal{K}$ telle que $\mu(f) \neq 0$. D’après le lemme 1, la fonction $D_f$, définie sur G par

$$
(16) \quad D_f(s) = \mu(f)^{-1} \int f(t^{-1}s) d\nu(t)
$$

est continue dans G. Soit $g \in \mathcal{K}$. La fonction $(s, t) \to f(s)g(ts)$ est continue à support compact dans $G \times G$. D’après le chap. III, § 5, n° 1, th. 2, on a

$$
\mu(f)\nu(g) = \left( \int f(s)d\mu(s) \right) \left( \int g(t)d\nu(t) \right)
$$
$$
= \int d\mu(s) \int f(s)g(ts)d\nu(t) = \int d\nu(t) \int f(s)g(ts)d\mu(s)
$$
$$
= \int d\nu(t) \int f(t^{-1}s)g(s)d\mu(s)
$$
$$
= \int g(s) \left[ \int f(t^{-1}s)d\nu(t) \right] d\mu(s) = \mu(g \cdot \mu(f)D_f)
$$

d’où

$$
\nu(g) = \mu(D_f \cdot g).
$$

Ceci prouve d’abord que $D_f$ ne dépend pas de $f$. Car, si $f' \in \mathcal{K}$ est telle que $\mu(f') \neq 0$, on a $D_{f'} \mu = D_f \cdot \mu$, donc $D_f = D_{f'}$ localement presque partout pour $\mu$, donc partout puisque $D_f$ et $D_{f'}$ sont continues et que le support de $\mu$ est $G$. Posons donc $D_f = D$. La formule (16) donne

$$
\mu(f)D(e) = \tilde{\nu}(f).
$$

La formule (19) s’étend par linéarité aux fonctions $f \in \mathcal{K}$ telles que $\mu(f) = 0$. On a $D(e) \neq 0$ puisque $\tilde{\nu} \neq 0$. Ceci établit bien la proportionnalité de $\mu$ et $\tilde{\nu}$.

#### Corollaire {#int-vii-s1-n2-cor-1 .statement}

*Toute mesure invariante à gauche (resp. à droite) sur G est proportionnelle à une mesure de Haar à gauche (resp. à droite).*

#### Exemple 1 {#int-vii-s1-n2-exa-1 .statement}

Sur le groupe additif $\mathbf{R}$, la mesure de Lebesgue $dx$ est une mesure de Haar (Chap. III, § 2, n° 2, *Exemple*).

#### Exemple 2 {#int-vii-s1-n2-exa-2 .statement}

Pour toute fonction $f \in \mathcal{K}(\mathbf{R}_+^*)$, on a (*Fonct. var. réelle*, chap. II, § 1, formule (13))

$$
\int_0^{+\infty} \frac{f(x)}{x} dx = \int_0^{+\infty} \frac{f(tx)}{tx} t dx = \int_0^{+\infty} \frac{f(tx)}{x} dx
$$
quel que soit $t > 0$; la mesure $x^{-1} dx$ est donc une mesure de Haar sur le groupe multiplicatif $\mathbf{R}_+^*$.

#### Exemple 3 {#int-vii-s1-n2-exa-3 .statement}

Prenons pour $G$ le tore $\mathbf{T} = \mathbf{R}/\mathbf{Z}$. Soit $\varphi$ l’application canonique de $\mathbf{R}$ sur $\mathbf{T}$. Pour $f \in \mathcal{H}(\mathbf{T})$, la fonction $f \circ \varphi$ est continue et périodique de période 1 sur $\mathbf{R}$, et l’intégrale
$$
I(f) = \int_a^{a+1} f(\varphi(x)) dx
$$
est indépendante du choix de $a \in \mathbf{R}$; il est immédiat qu’elle est invariante par translation ; elle définit donc une mesure de Haar sur $\mathbf{T}$. Par transport de structure, on en déduit que
$$
I(f) = \int_a^{a+1} f(e^{2\pi i t}) dt
$$
est une mesure de Haar sur le groupe multiplicatif $\mathbf{U}$ des nombres complexes de valeur absolue 1 (*Top. gén.*, chap. VIII, § 2, no 1).

#### Proposition 2 {#int-vii-s1-prop-2 .statement}

*Soient G un groupe localement compact, $\mu$ une mesure de Haar à gauche ou à droite sur G. Pour que G soit discret, il faut et il suffit que $\mu(\{e\}) > 0$. Pour que G soit compact, il faut et il suffit que $\mu^*(G) < +\infty$.*

Les conditions sont évidemment nécessaires. Montrons leur suffisance. Soit V un voisinage compact de e. Si $\mu(\{e\}) > 0$, V est un ensemble fini puisque $\mu(V) < +\infty$; comme G est séparé, il est donc discret. Supposons $\mu^*(G) < +\infty$, et $\mu$ invariante à gauche par exemple. Considérons l’ensemble $\mathscr{E}$ des parties finies $\{s_1, \ldots, s_n\}$ de G telles que $s_i V \cap s_j V = \varnothing$ pour $i \neq j$; on a
$$
n \mu(V) = \mu(s_1 V \cup \ldots \cup s_n V) \leq \mu^*(G),
$$
donc $n \leq \mu^*(G)/\mu(V)$. On peut donc choisir dans $\mathscr{E}$ un élément $\{s_1, \ldots, s_n\}$ maximal. Alors, pour tout $s \in G$, il y a un $i$ tel que $s V \cap s_i V \neq \varnothing$, donc tel que $s \in s_i V V^{-1}$. Donc G est réunion des ensembles compacts $s_i V V^{-1}$ et est par suite compact.

### 3. Module.

Soit $\mu$ une mesure de Haar à gauche sur $G$. Pour tout $s \in G$, $\delta(s)\mu$ est encore invariante à gauche (n° 1, formule (11)), donc (th. 1) il existe un nombre unique $\Delta_G(s) > 0$ tel que $\delta(s)\mu = \Delta_G(s)\mu$. En vertu du th. 1, le nombre $\Delta_G(s)$ est indépendant du choix de $\mu$.

#### Définition 3 {#int-vii-s1-def-3 .statement}

La fonction $\Delta_G$ sur $G$ s'appelle le module de $G$. Si $\Delta_G = 1$, le groupe $G$ est dit unimodulaire.

On peut dire aussi que $\mu$ est relativement invariante à droite de multiplicateur $\Delta_G$. Donc $\Delta_G$ est une représentation continue de $G$ dans $\mathbf{R}_+^*$ (n° 1, prop. 1).

#### Remarque {#int-vii-s1-n3-rem-1 .statement}

Si $\varphi$ est un isomorphisme de $G$ sur un groupe localement compact $G'$, on a $\Delta_{G'} \circ \varphi = \Delta_G$. En particulier :
1) Comme $x \to x^{-1}$ est un isomorphisme de $G$ sur le groupe opposé $G^o$, on a $\Delta_{G^o} = \Delta_G^{-1}$.
2) Si $\varphi$ est un automorphisme de $G$, on a $\Delta_G \circ \varphi = \Delta_G$.

Soit $s \in G$. On a :

$$
\delta(s)(\Delta_G^{-1}.\mu) = (\delta(s)\Delta_G^{-1}) . (\delta(s)\mu) = (\Delta_G(s)^{-1}\Delta_G^{-1}) . (\Delta_G(s)\mu) = \Delta_G^{-1}.\mu
$$

donc $\Delta_G^{-1}.\mu = \mu'$ est une mesure de Haar à droite. On en déduit que $\gamma(s)\mu' = (\gamma(s)\Delta_G^{-1}) . \mu = \Delta_G(s)(\Delta_G^{-1}.\mu) = \Delta_G(s)\mu'$, donc, pour toute mesure de Haar à droite $\nu$, on a $\gamma(s)\nu = \Delta_G(s)\nu$. Puisque $\tilde{\nu}$ est une mesure de Haar à droite, on a $\tilde{\nu} = a\Delta_G^{-1}.\mu$ avec une constante $a > 0$; on en déduit

$$
\mu = a(\Delta_G^{-1}.\mu)^\vee = a\Delta_G . \tilde{\nu} = a^2\mu,
$$

donc $a = 1$ et finalement $\tilde{\nu} = \Delta_G^{-1}.\mu$. On voit de même que $\nu = \Delta_G . \nu$. On a donc les résultats suivants :

Formulaire. — Soient $G$ un groupe localement compact, $\Delta$ son module, $\mu$ une mesure de Haar à gauche, $\nu$ une mesure de Haar à droite.

1) On a

(20) $\gamma(s)\mu = \mu \quad \delta(s)\mu = \Delta(s)\mu \quad \tilde{\mu} = \Delta^{-1}\cdot\mu.$

Si $f$ est $\mu$-intégrable sur $G$, les translatées à gauche et à droite de $f$ sont $\mu$-intégrables, et on a

$$
\int f(sx)d\mu(x) = \int f(x)d\mu(x)
$$
(21)
$$
\int f(xs)d\mu(x) = \Delta(s)^{-1} \int f(x)d\mu(x).
$$

En outre, $\tilde{f}$ est intégrable pour $\Delta^{-1}\cdot\mu$ et
$$
\int f(x^{-1})\Delta(x)^{-1}d\mu(x) = \int f(x)d\mu(x).
$$
(22)

Si $A$ est une partie $\mu$-intégrable de $G$, $sA$ et $As$ sont $\mu$-intégrables et
$$
\mu(sA) = \mu(A) \qquad \mu(As) = \Delta(s)\mu(A).
$$
(23)

2) On a

(24) $\delta(s)\nu = \nu \quad \gamma(s)\nu = \Delta(s)\nu \quad \tilde{\nu} = \Delta.\nu.$

Si $f$ est $\nu$-intégrable sur $G$, les translatées à gauche et à droite de $f$ sont $\nu$-intégrables, et on a

$$
\int f(xs)d\nu(x) = \int f(x)d\nu(x)
$$
(25)
$$
\int f(xs)d\nu(x) = \Delta(s) \int f(x)d\nu(x).
$$

En outre, $\tilde{f}$ est intégrable pour $\Delta.\nu$ et
$$
\int f(x^{-1})\Delta(x)d\nu(x) = \int f(x)d\nu(x).
$$
(26)

Si $A$ est une partie $\nu$-intégrable de $G$, $sA$ et $As$ sont $\nu$-intégrables et
$$
\nu(As) = \nu(A) \qquad \nu(sA) = \Delta(s)^{-1}\nu(A).
$$
(27)

3) $v$ est proportionnelle à $\Delta^{-1}.\mu$, $\mu$ est proportionnelle à $\Delta . v$.

4) Supposons G unimodulaire. Soit $\mu$ une mesure de Haar sur G. On a

$$
\gamma(s)\mu = \delta(s)\mu = \tilde{\mu} = \mu.
$$

Si $f$ est $\mu$-intégrable sur G, les translatées à gauche et à droite de $f$ sont $\mu$-intégrables ainsi que $\tilde{f}$, et l’on a

$$
\int f(sx)d\mu(x) = \int f(xs)d\mu(x) = \int f(x^{-1})d\mu(x) = \int f(x)d\mu(x).
$$

Si A est une partie $\mu$-intégrable de G, sA, As et $A^{-1}$ sont $\mu$-intégrables, et

$$
\mu(sA) = \mu(As) = \mu(A^{-1}) = \mu(A).
$$

On a des propriétés analogues pour l’intégrale essentielle.

#### Proposition 3 {#int-vii-s1-prop-3 .statement}

S’il existe dans G un voisinage compact V de e invariant par les automorphismes intérieurs, alors G est unimodulaire.

En effet, soit $\mu$ une mesure de Haar à gauche sur G. On a, pour tout $s \in G$, $\mu(V) = \mu(s^{-1}Vs) = \Delta_G(s)\mu(V)$, d’où

$$
\Delta_G(s) = 1
$$

puisque $0 < \mu(V) < +\infty$.

On en déduit aussitôt :

#### Corollaire {#int-vii-s1-n3-cor-1 .statement}

Si G est discret, ou compact, ou commutatif, G est unimodulaire.

Ceci est d’ailleurs trivial lorsque G est commutatif. Notons aussi que, si G est discret, la mesure sur G pour laquelle chaque point est de masse 1 est évidemment une mesure de Haar à gauche et à droite sur G, qu’on appelle mesure de Haar normalisée sur G. Si G est compact, il existe une mesure de Haar $\mu$ et une seule sur G telle que $\mu(G) = 1$; on l’appelle la mesure de Haar normalisée de G. Les deux conventions précédentes ne concordent pas lorsque G est à la fois discret et compact, c'est-à-dire fini ; quand on sera dans ce cas, on précisera toujours explicitement ce qu'on entend par mesure de Haar normalisée.

Un sous-groupe, un groupe quotient d'un groupe unimodulaire ne sont pas toujours unimodulaires (§ 2, exerc. 5). Cf., toutefois, le § 2, no 7, prop. 10.

*Nous verrons plus tard que les groupes de Lie connexes semi-simples ou nilpotents sont unimodulaires.*

### 4. Module d'un automorphisme.

Soient G un groupe localement compact, φ un automorphisme de G, μ une mesure de Haar à gauche sur G. Il est clair que $\varphi^{-1}(\mu)$ est encore une mesure de Haar à gauche sur G. Il existe donc (no 2, th. 1) un nombre $a > 0$ et un seul tel que $\varphi^{-1}(\mu) = a\mu$. D'après le no 2, th. 1, ce nombre est indépendant du choix de $\mu$. Remarquons que, si l'on partait d'une mesure de Haar à droite, par exemple $\Delta_G^{-1} \cdot \mu$ (no 3), on aboutirait au même scalaire $a$ : car, comme $\varphi^{-1}$ laisse $\Delta_G$ invariant (no 3, Remarque), on a $\varphi^{-1}(\Delta_G^{-1} \cdot \mu) = \Delta_G^{-1} \cdot \varphi^{-1}(\mu) = a \Delta_G^{-1} \cdot \mu$.

#### Définition 4 {#int-vii-s1-def-4 .statement}

Le nombre $a > 0$ tel que $\varphi^{-1}(\mu) = a\mu$ s'appelle le module de l'automorphisme $\varphi$ et se note $\mathrm{mod}_G \varphi$ ou simplement $\mathrm{mod} \varphi$.

Si $f$ est une fonction $\mu$-intégrable sur G, on a

(31)
$$
\int f(\varphi^{-1}(x)) d\mu(x) = (\mathrm{mod}\ \varphi) \int f(x) d\mu(x).
$$

Si A est une partie $\mu$-intégrable de G, on a

(32)
$$
\mu(\varphi(A)) = (\mathrm{mod}\ \varphi) \mu(A).
$$

En particulier, pour $s \in G$, soit $i_s$ l'automorphisme intérieur $x \to s^{-1} xs$. On a $i_s^{-1} = \delta(s) \gamma(s)$, donc
$$
i_s^{-1}(\mu) = \delta(s) \mu = \Delta_G(s) \mu,
$$

et par suite

(33) $$ \operatorname{mod} i_s = \Delta_G(s). $$

Si G est soit discret, soit compact, sa mesure de Haar normalisée est transformée en elle-même par tout automorphisme $\varphi$ de G, comme on le voit tout de suite par transport de structure. Donc un automorphisme d'un groupe discret ou compact est de module 1.

#### Proposition 4 {#int-vii-s1-prop-4 .statement}

Soient G un groupe localement compact, $\Gamma$ un groupe topologique, et $\gamma \to u_\gamma$ un homomorphisme de $\Gamma$ dans le groupe $\mathcal{G}$ des automorphismes de G, tel que $(\gamma, x) \to u_\gamma(x)$ soit une application continue de $\Gamma \times G$ dans G. Alors l'application $\gamma \to \operatorname{mod}(u_\gamma)$ est une représentation continue de $\Gamma$ dans $\mathbf{R}_+^*$.

Cette application est évidemment une représentation (algébrique) de $\Gamma$ dans $\mathbf{R}_+^*$; il suffit de prouver sa continuité. Soient $f \in \mathcal{K}(G)$ et S son support. Soient $\gamma_0 \in \Gamma$ et U un voisinage relativement compact de $u_{\gamma_0}^{-1}(S)$. L'application $\gamma \to u_\gamma$ est une application continue de $\Gamma$ dans $\mathcal{G}$ muni de la topologie de la convergence compacte (Top. Gén., chap. X, 2e éd., § 3, no 4, th. 3); donc $u_{\gamma_0}^{-1}(S) \subset U$ pour $\gamma$ assez voisin de $\gamma_0$. Le lemme 1 du no 1 prouve alors que $\int f(u_\gamma(x)) d\mu(x)$ (où $\mu$ désigne une mesure de Haar à gauche de G) dépend continûment de $\gamma$; d'où la proposition.

### 5. Mesure de Haar d'un produit.

#### Proposition 5 {#int-vii-s1-prop-5 .statement}

Soit $(G_i)_{i \in I}$ une famille de groupes localement compacts. Pour tout $i \in I$, soit $\mu_i$ une mesure de Haar à gauche (resp. à droite) sur $G_i$. On suppose qu'il existe une partie finie J de I telle que, pour tout $i \in I - J$, $G_i$ soit compact et $\mu(G_i) = 1$. Alors la mesure produit $\bigotimes_{i \in I} \mu_i$ est une mesure de Haar à gauche (resp. à droite) sur $G = \prod_{i \in I} G_i$. Si $x = (x_i) \in G$, on a

$$ \Delta_G(x) = \prod_{i \in I} \Delta_{G_i}(x_i). $$

Pour toute partie finie J de I, $\bigotimes_{i \in J} \mu_i$ est une mesure de Haar à gauche (resp. à droite) sur $\prod_{i \in J} G_i$, comme il résulte aussitôt des définitions. Donc $\bigotimes_{i \in I} \mu_i$ est une mesure de Haar à gauche (resp. à droite) sur G (chap. III, § 5, no 5, prop. 6). D'autre part, si les $\mu_i$ sont des mesures de Haar à gauche, on a

$$
\delta(x)(\bigotimes_{i \in I} \mu_i) = \bigotimes_{i \in I} \delta(x_i) \mu_i = \bigotimes_{i \in I} (\Delta_{G_i}(x_i) \mu_i) = (\prod_{i \in I} \Delta_{G_i}(x_i)) \bigotimes_{i \in I} \mu_i,
$$

d'où $\Delta_G(x) = \prod_{i \in I} \Delta_{G_i}(x_i)$.

#### Exemple 1 {#int-vii-s1-n5-exa-1 .statement}

La mesure de Lebesgue sur $\mathbf{R}^n$ est une mesure de Haar du groupe additif $\mathbf{R}^n$.

#### Exemple 2 {#int-vii-s1-n5-exa-2 .statement}

L’application $(r, u) \to ru$ est un isomorphisme de $\mathbf{R}_+^* \times \mathbf{U}$ sur $\mathbf{C}^*$ (*Top. gén.*, chap. VIII, § 1, no 3). Si on identifie $\mathbf{C}^*$ à $\mathbf{R}_+^* \times \mathbf{U}$ par cet isomorphisme, et si on note $du$ une mesure de Haar de $\mathbf{U}$, $r^{-1} dr du$ est une mesure de Haar de $\mathbf{C}^*$ d’après l’exemple 2 du no 2. D’autre part, la bijection $\theta \to e^{2i\pi\theta}$ de $[0, 1[$ sur $\mathbf{U}$ transforme la mesure de Lebesgue $d\theta$ de $[0, 1[$ en une mesure de Haar sur $\mathbf{U}$ d’après l’exemple 3 du no 2. Il en résulte que, si $f \in \mathcal{H}(\mathbf{C}^*)$, l’intégrale

$$
\int_0^{+\infty} \int_0^1 f(re^{2i\pi\theta}) r^{-1} dr d\theta
$$

définit une mesure de Haar sur $\mathbf{C}^*$.

### 6. Mesure de Haar d’une limite projective.

Soit G un groupe localement compact (donc complet). Soit $(K_\alpha)_{\alpha \in A}$ une famille filtrante décroissante de sous-groupes distingués compacts de G, d’intersection $\{e\}$ (de sorte que la base de filtre formée des $K_\alpha$ converge vers $e$). Posons $G_\alpha = G/K_\alpha$; soient $\varphi_\alpha : G \to G_\alpha$ et $\varphi_{\beta \alpha} : G_\alpha \to G_\beta$ ($\alpha \geq \beta$) les homomorphismes canoniques. Alors la limite projective du système projectif $(G_\alpha, \varphi_{\beta \alpha})$ s’identifie à G et l’application canonique de cette limite projective dans $G_\alpha$ s'identifie à $\varphi_\alpha$ (*Top. Gén.*, chap. III, 3e éd., § 7, n° 3, prop. 2). Les applications $\varphi_\alpha$ et $\varphi_{\beta\alpha}$ sont propres (*loc. cit.*, § 4, n° 1, cor. 2 de la prop. 1). Ces données resteront fixées dans tout ce n°.

#### Lemme 2 {#int-vii-s1-lem-2 .statement}

a) *Soient* $f \in \mathcal{K}_+(G)$, *S une partie compacte de* $G$ *contenant* $\mathrm{Supp}\ f$, *U un voisinage ouvert de* $S$ *dans* $G$, *et* $\varepsilon > 0$. *Il existe un* $\alpha \in A$ *et une fonction* $g \in \mathcal{K}_+(G)$, *nulle hors de* $U$, *constante sur les classes suivant* $K_\alpha$, *telle que* $|f - g| \leq \varepsilon$.

b) *Soient* $\mu$ *et* $\mu'$ *deux mesures sur* $G$ *telles que* $\varphi_\alpha(\mu) = \varphi_\alpha(\mu')$ *pour tout* $\alpha \in A$. *Alors* $\mu = \mu'$.

Il existe un $\alpha_1 \in A$ tel que $K_{\alpha_1} S \cap K_{\alpha_1}(G - U) = \varnothing$ (*Top. Gén.*, chap. II, 3e éd., § 4, n° 3, prop. 4). En augmentant $S$ et en diminuant $U$, on peut donc supposer que $S$ et $U$ sont des réunions de classes suivant $K_{\alpha_1}$. Considérons les fonctions numériques continues $h$ sur $S$ qui possèdent la propriété suivante : il existe $\alpha \geq \alpha_1$ tel que $h$ soit constante sur les classes suivant $K_\alpha$. Ces fonctions forment une sous-algèbre de $\mathcal{K}(S)$ (parce que la famille $(K_\alpha)$ est filtrante décroissante) qui contient les constantes et qui sépare les points de $S$ : en effet, soient $x, y$ deux points distincts de $S$; comme l’intersection des $K_\alpha$ est $\{e\}$, il existe $\alpha \geq \alpha_1$ tel que $\varphi_\alpha(x) \neq \varphi_\alpha(y)$, puis une fonction numérique $u$ continue dans $\varphi_\alpha(S)$, telle que $u(\varphi_\alpha(x)) \neq u(\varphi_\alpha(y))$. D’après le th. de Weierstrass-Stone, il existe un $\alpha \geq \alpha_1$ et une fonction $h \geq 0$ continue dans $S$, constante sur les classes suivant $K_\alpha$, et telle que $|f - h| \leq \frac{\varepsilon}{2}$ dans $S$. Pour tout $t \in \mathbf{R}$, posons $\delta(t) = \left( t - \frac{\varepsilon}{2} \right)^+$, et posons $h' = \delta \circ h$. Alors $h'$ est une fonction $\geq 0$, continue dans $S$, constante sur les classes suivant $K_\alpha$, et l’on a $|h - h'| \leq \frac{\varepsilon}{2}$ dans $S$, donc $|f - h'| \leq \varepsilon$ dans $S$. D’autre part, on a $h'(x) = 0$ si $x$ appartient à la frontière de $S$ dans $G$, car alors $h(x) \leq \frac{\varepsilon}{2}$. Si on prolonge $h'$ par 0 dans le complémentaire de $S$, on obtient une fonction $g$ qui répond à la question, ce qui prouve a).

Soient maintenant $\mu, \mu'$ deux mesures sur $G$ telles que $\varphi_\alpha(\mu) = \varphi_\alpha(\mu')$ pour tout $\alpha \in A$. Soit $v \in \mathcal{K}(G)$ une fonction constante sur les classes suivant $K_\alpha$ pour un $\alpha \in A$, de sorte qu’on peut écrire $v = w \circ \varphi_\alpha$ avec $w \in \mathcal{K}(G_\alpha)$; on a alors $\mu(v) = (\varphi_\alpha(\mu))(w) = (\varphi_\alpha(\mu'))(w) = \mu'(v)$; on en conclut que $\mu = \mu'$ en vertu de a).

#### Proposition 6 {#int-vii-s1-prop-6 .statement}

*Pour tout $\alpha \in A$, soit $\mu_\alpha$ une mesure positive sur $G_\alpha$. On suppose que $\varphi_{\beta\alpha}(\mu_\alpha) = \mu_\beta$ pour $\alpha \geq \beta$. Il existe alors une mesure positive $\mu$ sur $G$ et une seule telle que $\varphi_\alpha(\mu) = \mu_\alpha$ pour tout $\alpha \in A$.*

L’unicité résulte aussitôt du lemme 2 b). Prouvons l’existence de $\mu$. Soit V l’espace vectoriel des fonctions appartenant à $\mathcal{K}(G)$ et constantes sur les classes suivant un $K_\alpha$. D’après le lemme 2 a), V est un sous-espace vectoriel positivement riche (chap. III, § 2, no 5) de $\mathcal{K}(G)$. Soit $f \in V$. Il existe un $\alpha \in A$ tel que $f$ soit constante sur les classes suivant $K_\alpha$. Par passage au quotient, $f$ définit une fonction $f_\alpha \in \mathcal{K}(G_\alpha)$. Le nombre $\mu(f) = \mu_\alpha(f_\alpha)$ ne dépend pas du choix de $\alpha$; car soit $\beta$ un indice tel que $f$ soit constante sur les classes suivant $K_\beta$; soit $\gamma \in A$ tel que $\gamma \geq \alpha, \gamma \geq \beta$; alors $f$ définit des fonctions $f_\beta \in \mathcal{K}(G_\beta), f_\gamma \in \mathcal{K}(G_\gamma)$ telles que $f = f_\beta \circ \varphi_\beta = f_\gamma \circ \varphi_\gamma$; on a $f_\alpha \circ \varphi_{\alpha\gamma} = f_\gamma$, donc $\mu_\gamma(f_\gamma) = (\varphi_{\alpha\gamma}(\mu_\gamma))(f_\alpha) = \mu_\alpha(f_\alpha)$, et de même $\mu_\gamma(f_\gamma) = \mu_\beta(f_\beta)$, d’où notre assertion. Ceci posé, il est clair que $\mu$ est une forme linéaire sur V et que $\mu(f) \geq 0$ pour $f \geq 0$. D’après la prop. 2 du chap. III, § 2, no 5, $\mu$ se prolonge en une mesure positive, que nous noterons encore $\mu$, sur $G$. On a $\varphi_\alpha(\mu) = \mu_\alpha$ pour tout $\alpha \in A$ par construction même de $\mu$.

#### Définition 5 {#int-vii-s1-def-5 .statement}

*On dit que $\mu$ est la limite projective des $\mu_\alpha$*.

#### Proposition 7 {#int-vii-s1-prop-7 .statement}

*On conserve les notations de la prop. 6. Si chaque $\mu_\alpha$ est une mesure de Haar à gauche (resp. à droite) sur $G_\alpha$, alors $\mu$ est une mesure de Haar à gauche (resp. à droite) sur $G$*.

Supposons par exemple que les $\mu_\alpha$ soient des mesures de Haar à gauche. Soit $s \in G$. On a, pour tout $x \in G$,

$$(\varphi_\alpha \circ \gamma(s))(x) = \varphi_\alpha(sx) = \varphi_\alpha(s)\varphi_\alpha(x) = (\gamma(\varphi_\alpha(s)) \circ \varphi_\alpha)(x);$$
donc $\varphi_\alpha(\gamma(s)\mu) = \gamma(\varphi_\alpha(s))\mu_\alpha = \mu_\alpha$. Donc $\gamma(s)\mu = \mu$ d'après le lemme 2 b), de sorte que $\mu$ est une mesure de Haar à gauche.

On suppose désormais les $K_\alpha$, non seulement compacts, mais *ouverts* dans G. Alors les $G_\alpha$ sont discrets, et $K_\alpha/K_\beta$ est, pour $\beta \geq \alpha$, un groupe compact et discret, donc fini. Le groupe G est unimodulaire (prop. 3).

#### Proposition 8 {#int-vii-s1-prop-8 .statement}

a) *Soient $\mu$ et $\mu'$ deux mesures positives sur G telles que, pour tout $\alpha$ et toute classe C suivant $K_\alpha$, on ait $\mu(C) = \mu'(C)$. Alors $\mu = \mu'$.*

b) *Fixons un $\alpha_0 \in A$. Pour tout $\alpha \geq \alpha_0$, soit $n_\alpha$ le nombre d'éléments du groupe fini $K_{\alpha_0}/K_\alpha$. Il existe sur G une mesure positive $\mu$ et une seule telle que, pour tout $\alpha \in A$, chaque classe suivant $K_\alpha$ soit de mesure $n_\alpha^{-1}$. En outre, $\mu$ est une mesure de Haar sur G, telle que $\mu(K_{\alpha_0}) = 1$.*

Soient $\mu$ et $\mu'$ deux mesures positives sur G vérifiant la condition de a). Alors les points du groupe discret $G_\alpha$ ont même mesure pour $\varphi_\alpha(\mu)$ et $\varphi_\alpha(\mu')$, d'où $\varphi_\alpha(\mu) = \varphi_\alpha(\mu')$ et ceci quel que soit $\alpha$. Donc $\mu = \mu'$ (lemme 2 b)).

Prouvons b). Pour tout $\alpha \geq \alpha_0$, soit $\mu_\alpha$ la mesure de Haar du groupe discret $G_\alpha$ telle que chaque point soit de mesure $n_\alpha^{-1}$. Soient $\alpha, \beta$ tels que $\alpha \geq \beta \geq \alpha_0$. Alors $K_\beta/K_\alpha$ a $n_\alpha/n_\beta$ éléments. Donc $\varphi_{\beta\alpha}(\mu_\alpha)$ est la mesure sur $G_\beta$ telle que chaque point ait pour mesure $n_\alpha^{-1} \frac{n_\alpha}{n_\beta} = n_\beta^{-1}$; autrement dit,
$$
\varphi_{\beta\alpha}(\mu_\alpha) = \mu_\beta.
$$
Il suffit alors d'appliquer les prop. 6 et 7.

#### Exemple {#int-vii-s1-n6-exa-1 .statement}

Soit $\mathbf{Q}_p$ le corps $p$-adique, complété de $\mathbf{Q}$ pour la valeur absolue $p$-adique $|x|_p = p^{-v_p(x)}$ (*Top. Gén.*, chap. IX, 2e éd., § 3, n° 2). Les éléments de $\mathbf{Q}_p$ s'appellent *nombres $p$*-*adiques*. Nous noterons encore $|x|_p$ le prolongement continu à $\mathbf{Q}_p$ de la valeur absolue $p$-adique. On a
$$
|x + y|_p \leq \sup(|x|_p, |y|_p)
$$

pour $x, y$ dans $\mathbf{Q}$ (*loc. cit.*), donc pour $x, y$ dans $\mathbf{Q}_p$; en outre, si $|y|_p < |x|_p$, on a $|x + y|_p = |x|_p$, car
$$
|x|_p = |(x + y) - y|_p \leq \sup(|x + y|_p, |y|_p).
$$
Si $(x_n)$ est une suite de points de $\mathbf{Q}_p$ tendant vers $x \in \mathbf{Q}_p^*$, on a $|x - x_n|_p < |x|_p$ et $|x - x_n|_p < |x_n|_p$ pour $n$ assez grand, donc $|x|_p = |x_n|_p$. Ceci prouve que, pour tout $x \in \mathbf{Q}_p^*$, $|x|_p$ est une puissance de $p$.

Soit $\mathbf{Z}_p$ l’adhérence de $\mathbf{Z}$ dans $\mathbf{Q}_p$; c’est un sous-anneau de $\mathbf{Q}_p$; ses éléments s’appellent *entiers p-adiques*. On a $|x|_p \leq 1$ pour tout $x \in \mathbf{Z}_p$. Réciproquement, soit $x$ un élément de $\mathbf{Q}_p$ tel que $|x|_p \leq 1$, et montrons que $x \in \mathbf{Z}_p$; il existe une suite $(x_n)$ d’éléments de $\mathbf{Q}$ tendant vers $x$, et $|x_n|_p \leq 1$ pour $n$ assez grand d’après ce qu’on a vu plus haut ; il suffit de montrer que $x_n$ appartient à $\mathbf{Z}_p$ pour $n$ assez grand ; autrement dit, nous sommes ramenés au cas où $x \in \mathbf{Q}$; alors $x = a/b$ avec $b$ étranger à $p$; pour tout entier $n > 0$, il existe $b'_n \in \mathbf{Z}$ et $h_n \in \mathbf{Z}$ tels que $bb'_n + h_n p^n = 1$, d’où
$$
x = \frac{abb'_n + ah_n p^n}{b} = ab'_n + \frac{ah_n p^n}{b}
$$
et $|x - ab'_n|_p \leq p^{-n}$, donc $ab'_n$ tend vers $x$.

Il résulte de là que la boule fermée de centre 0 et de rayon $p^{-n}$, identique à la boule ouverte de centre 0 et de rayon $p^{-n+1}$, est $p^n \mathbf{Z}_p$. L’espace topologique $\mathbf{Q}_p$ est donc éparpillé et par suite totalement discontinu (*Top. Gén.*, Chap. IX, 2e éd., § 6, no 4).

Montrons que les entiers $0, 1, \ldots, p^n - 1$ constituent un système de représentants de $\mathbf{Z}_p$ modulo $p^n \mathbf{Z}_p$. D’abord, on a $|k - k'|_p > p^{-n}$ pour deux tels entiers $k$ et $k'$, donc les classes modulo $p^n \mathbf{Z}_p$ de ces entiers sont distinctes. D’autre part, soit $x \in \mathbf{Z}_p$; il existe un $k \in \mathbf{Z}$ tel que $|x - k|_p \leq p^{-n}$; en ajoutant à $k$ un multiple de $p^n$, on peut supposer que $k \in \{0, p^n - 1\}$, et $x$ est congru à $k$ modulo $p^n \mathbf{Z}_p$. D’où notre assertion. Ceci montre que $\mathbf{Z}_p / p^n \mathbf{Z}_p$ est canoniquement isomorphe à $\mathbf{Z}/p^n \mathbf{Z}$. On voit en outre que $\mathbf{Z}_p$ est précompact, donc *compact* puisqu’il est complet. Comme $\mathbf{Z}_p$ est un sous-groupe ouvert de $\mathbf{Q}_p$, $\mathbf{Q}_p$ est *localement compact*. La topologie de $\mathbf{Q}_p$ est à base dénombrable (*Top. Gén.*, Chap. IX, 2e éd., § 2, n° 9, cor. de la prop. 16). Le groupe additif $\mathbf{Q}_p$ s’identifie à la limite projective des groupes discrets $\mathbf{Q}_p / p^n \mathbf{Z}_p$.

Il existe sur le groupe additif $\mathbf{Q}_p$ une mesure de Haar $\alpha$ et une seule telle que $\alpha(\mathbf{Z}_p) = 1$; celle-ci est dite la *mesure de Haar normalisée* sur $\mathbf{Q}_p$. Comme $\mathbf{Z}_p$ est réunion de $p^n$ classes disjointes suivant $p^n \mathbf{Z}_p$ ($n$ entier $\geqslant 0$), on a $\alpha(p^n \mathbf{Z}_p) = p^{-n}$; de même, $\alpha(p^{-n} \mathbf{Z}_p) = p^n$, de sorte que finalement $\alpha(p^n \mathbf{Z}_p) = p^{-n}$ pour tout $n \in \mathbf{Z}$. D’après la prop. 8 b), $\alpha$ *est la seule mesure positive sur* $\mathbf{Q}_p$ *telle que toute classe suivant* $p^n \mathbf{Z}_p$ ($n$ entier $\geqslant 0$) *soit de mesure* $p^{-n}$.

La restriction de $\alpha$ à $\mathbf{Z}_p$ est évidemment une mesure de Haar sur $\mathbf{Z}_p$.

### 7. Définition locale d’une mesure de Haar.

#### Proposition 9 {#int-vii-s1-prop-9 .statement}

Soient $G$ un groupe localement compact, $V$ une partie ouverte de $G$, $\mu$ une mesure positive non nulle sur $V$, ayant la propriété suivante : si $U$ est une partie ouverte de $V$ et si $s \in G$ est tel que $sU \subset V$, l’image de la mesure $\mu_U$, induite par $\mu$ sur $U$, par l’homéomorphisme $x \to sx$ de $U$ sur $sU$, est $\mu_{sU}$. Alors il existe sur $G$ une mesure de Haar à gauche $\alpha$ et une seule induisant $\mu$ sur $V$.

Pour tout $s \in G$, soit $\mu_s$ l’image de $\mu$ par l’homéomorphisme $x \to sx$ de $V$ sur $sV$. La restriction de $\mu_s$ à $V \cap sV$ est l’image de $\mu_{s^{-1}V \cap V}$ par la restriction de $x \to sx$ à $s^{-1}V \cap V$; par hypothèse, cette image est $\mu_{V \cap sV}$. Par translation, on en conclut que $\mu_s$ et $\mu_t$ ont même restriction à $sV \cap tV$ quels que soient $s, t$. D’après la prop. 1 du chap. III, § 3, n° 1, il existe donc une mesure $\alpha$ sur $G$ induisant $\mu_s$ sur $sV$ quel que soit $s$. Il est clair que $\alpha$ est l’unique mesure de Haar à gauche sur $G$ induisant $\mu$ sur $V$.

#### Corollaire {#int-vii-s1-n7-cor-1 .statement}

Soient $G, G'$ deux groupes localement compacts, $V$ (resp. $V'$) un voisinage ouvert de l’élément neutre de $G$ (resp. $G'$), $\varphi$ un isomorphisme local de $G'$ à $G$ (*Top. Gén.*, chap. III, § 1, n° 3, déf. 2) défini dans $V'$, *tel que* $\varphi(V') = V$.

Soient $\alpha'$ une mesure de Haar à gauche sur $G'$, et $\alpha'_{V'}$ sa restriction à $V'$. Alors $\varphi(\alpha'_{V'})$ est la restriction à $V$ d'une mesure de Haar à gauche unique $\alpha$ sur $G$.

Soit $V_1$ un voisinage ouvert de $e$ dans $G$ tel que $V_1 V_1^{-1} \subset V$. Soit $\mu$ la restriction de $\varphi(\alpha'_{V'})$ à $V_1$. Soient $U$ une partie ouverte de $V_1$ et $s \in G$ tels que $sU \subset V_1$. On a $s \in V_1 V_1^{-1} \subset V$, donc $s = \varphi(s')$ avec un $s' \in V'$. Soit $x \in U$. On a $x = \varphi(x')$ avec un $x' \in V'$, donc $sx = \varphi(s')\varphi(x') = \varphi(s'x')$ puisque $sx \in sU \subset V$. Comme les translations à gauche dans $G'$ conservent $\alpha'$, on voit que $V_1$ et $\mu$ satisfont aux conditions de la prop. 9. Soit $\alpha$ la mesure de Haar à gauche sur $G$ induisant $\mu$ sur $V_1$. Pour tout $t \in V$, il existe un voisinage ouvert $W$ de $e$ dans $V_1$ tel que $tW \subset V$. Alors la restriction de $\varphi(\alpha'_{V'})$ à $tW$ se déduit par translation de la restriction de $\mu$ à $W$, donc est la restriction de $\alpha$ à $tW$. Donc $\varphi(\alpha'_{V'})$ est la restriction de $\alpha$ à $V$.

On dit que $\alpha$ se déduit de $\alpha'$ par l'isomorphisme local $\varphi$.

#### Exemple {#int-vii-s1-n7-exa-1 .statement}

La mesure de Haar sur $\mathbf{T}$ obtenue au no 2, Exemple 3, peut se déduire de la mesure de Lebesgue de $\mathbf{R}$ par un isomorphisme local de $\mathbf{R}$ à $\mathbf{T}$.

### 8. Mesures relativement invariantes.

#### Proposition 10 {#int-vii-s1-prop-10 .statement}

Soient $G$ un groupe localement compact, $\mu$ une mesure relativement invariante à gauche de multiplicateur $\chi$ sur $G$. Si $\chi_1$ est une représentation continue de $G$ dans $\mathbf{C}^*$, la mesure $\chi_1.\mu$ est relativement invariante à gauche de multiplicateur $\chi_1 \chi$.

En effet,

$$
\gamma(s)(\chi_1 \cdot \mu) = (\gamma(s)\chi_1) \cdot (\gamma(s)\mu) = (\chi_1(s^{-1})\chi_1) \cdot (\chi(s)^{-1}\mu)
= (\chi_1 \chi)(s)^{-1}(\chi_1 \cdot \mu).
$$

#### Corollaire 1 {#int-vii-s1-prop-10-cor-1 .statement}

Soit $\mu$ une mesure de Haar à gauche sur $G$. Pour qu'une mesure non nulle $\nu$ sur $G$ soit relativement invariante à gauche, il faut et il suffit qu'elle soit de la forme $a \chi \cdot \mu$, où $a \in \mathbf{C}^*$ et où $\chi$ est une représentation continue de $G$ dans $\mathbf{C}^*$; son multiplicateur est alors $\chi$.

La condition est suffisante (prop. 10). D'autre part, si $\nu$ est une mesure non nulle relativement invariante à gauche de multiplicateur $\chi$, $\chi^{-1}.\nu$ est invariante à gauche (prop. 10), donc de la forme $a\mu$ avec $a \in \mathbf{C}^*$ (n° 2, cor. du th. 1).

#### Corollaire 2 {#int-vii-s1-prop-10-cor-2 .statement}

*Toute mesure relativement invariante à gauche est relativement invariante à droite.*

En effet, avec les notations du cor. 1, on a

$$
\delta(s)(\chi \cdot \mu) = (\delta(s)\chi) \cdot (\delta(s)\mu) = (\chi(s)\chi) \cdot (\Delta_G(s)\mu)
= (\chi \Delta_G)(s)(\chi \cdot \mu).
$$

En raison du cor. 2, on parlera désormais de *mesures relativement invariantes sur* $G$, sans préciser. Les mesures relativement invariantes admettent comme cas particuliers les mesures de Haar à gauche et les mesures de Haar à droite. Etant donnée une mesure relativement invariante $\nu$ sur $G$, il convient de distinguer son *multiplicateur à gauche* $\chi$ et son *multiplicateur à droite* $\chi'$ définis par $\gamma(s)\nu = \chi(s)^{-1}\nu, \delta(s)\nu = \chi'(s)\nu$. D'après (34), on a entre ces multiplicateurs la relation

$$
\chi' = \chi \Delta_G.
$$

Notant toujours $\mu$ une mesure de Haar à gauche, on a

$$
\tilde{\nu} = (\chi \cdot \mu)\tilde{\nu} = \tilde{\chi} \cdot \tilde{\mu} = (\chi^{-1}\Delta_G^{-1}) \cdot \mu,
$$

donc $\tilde{\nu}$ est relativement invariante de multiplicateur à gauche $\chi^{-1}\Delta_G^{-1}$, de multiplicateur à droite $\chi^{-1}$.

Les notions de fonctions négligeables, localement négligeables, mesurables, localement intégrables sont les mêmes vis-à-vis de toute mesure relativement invariante.

### 9. *Mesures quasi-invariantes.*

#### Proposition 11 {#int-vii-s1-prop-11 .statement}

*Soient* $G$ *un groupe localement compact*, $\mu$ *une mesure de Haar à gauche sur* $G$. *Pour qu'une mesure* ν ≠ 0 sur G soit quasi-invariante à gauche, il faut et il suffit que ν soit équivalente à μ.

La suffisance est évidente. Soit ν ≠ 0 une mesure quasi-invariante à gauche, et montrons que ν est équivalente à μ. On peut se borner au cas où ν > 0. Soit A une partie compacte de G. On va montrer, ce qui établira la proposition, que les conditions μ(A) = 0, ν(A) = 0 sont équivalentes (chap. V, § 5, no 5, Remarque).

a) Pour toute f ∈ $\mathcal{K}_+(G)$, la fonction $(x, y) \to f(x)\varphi_A(xy)$ sur $G \times G$ est $(\nu \otimes \mu)$-intégrable, car elle est semi-continue supérieurement, bornée, et son support est contenu dans l’ensemble compact $K \times K^{-1}A$ si l’on pose $K = \mathrm{Supp}\, f$. On a donc, par le théorème de Lebesgue-Fubini

$$
\int d\nu(y) \int \varphi_A(xy)f(x)d\mu(x) = \int f(x)d\mu(x) \int \varphi_A(xy)d\nu(y).
$$

b) Supposons ν(A) = 0. Par hypothèse, ν(xA) = 0 pour tout $x \in G$, donc le second membre de (36) est nul. Il existe donc un ensemble ν-négligeable N, tel que, pour $y \notin N_f$, on ait

$$
0 = \int \varphi_A(xy)f(x)d\mu(x) = \Delta_G(y)^{-1} \int \varphi_A(x)f(xy^{-1})d\mu(x).
$$

Soit B une partie compacte de G telle que ν(B) ≠ 0, et prenons pour f une fonction de $\mathcal{K}_+(G)$ égale à 1 sur AB⁻¹. Il existe alors un $y \in B$ tel que (37) soit vérifié. Mais comme

$$
\varphi_A(x)f(xy^{-1}) = \varphi_A(x)
$$

pour $y \in B$, cela prouve que $\mu(A) = 0$.

c) Supposons $\mu(A) = 0$. Alors, pour toute $f \in \mathcal{K}_+(G)$, le premier membre de (36) est nul, donc aussi le second. Par suite, il existe un ensemble M localement $\mu$-négligeable tel que

$$
\int \varphi_A(xy)d\nu(y) = 0,
$$

pour $x \notin M$. Comme $\mu \neq 0$, on en conclut que ν(xA) = 0 pour certains $x \in G$, d’où ν(A) = 0.

Appliquant la prop. 11 à G°, on voit que les mesures quasi-invariantes à droite sont identiques aux mesures quasi-invariantes à gauche. On les appelle simplement mesures quasi-invariantes sur G.

### 10. Corps localement compacts.

#### Définition 6 {#int-vii-s1-def-6 .statement}

Soit K un corps localement compact. Pour $a \in K^*$, on appelle module de a, et on note $\mathrm{mod}_K(a)$ ou simplement $\mathrm{mod}(a)$, le module de l’automorphisme $x \to ax$ du groupe additif $K^+$ sous-jacent à K ; on pose $\mathrm{mod}(0) = 0$.

#### Exemple 1 {#int-vii-s1-n10-exa-1 .statement}

Soit $K = \mathbf{R}$. Si $s > 0$, on a $s \cdot (0,1) = (0,s)$; si $s < 0$, on a $s \cdot (0,1) = (s,0)$. Donc $\mathrm{mod}_\mathbf{R} t = |t|$ pour tout $t \in \mathbf{R}$.

#### Exemple 2 {#int-vii-s1-n10-exa-2 .statement}

Soit $K = \mathbf{Q}_p$. Si $s \in \mathbf{Q}_p^*$ est tel que $|s|_p = p^{-n}$, alors $s \mathbf{Z}_p$ est l’ensemble des $x \in \mathbf{Q}_p$ tels que $|x|_p \leq p^{-n}$; donc, si on désigne par $\mu$ la mesure de Haar normalisée sur $\mathbf{Q}_p$, on a
$$
\mu(s \mathbf{Z}_p) = p^{-n}.
$$
Donc $\mathrm{mod}_{\mathbf{Q}_p} t = |t|_p$ pour tout $t \in \mathbf{Q}_p$.

#### Proposition 12 {#int-vii-s1-prop-12 .statement}

La fonction mod est continue dans K, et on a $\mathrm{mod}(ab) = \mathrm{mod}(a)\mathrm{mod}(b)$ quels que soient $a, b$ dans K.

La dernière relation est évidente. La prop. 4 du n° 4 montre que la fonction mod est continue en tout point de $K^*$. Il ne reste qu’à démontrer sa continuité en 0. Celle-ci est évidente pour K discret ; nous supposerons donc K non discret. Soient $\alpha$ une mesure de Haar sur $K^+$ et C une partie compacte de K telle que $\alpha(C) > 0$; pour $a \in K^*$, on a $\alpha(aC) = \mathrm{mod}(a)\alpha(C)$. Comme K n’est pas discret, on a $\alpha(\{0\}) = 0$ (n° 2, prop. 2); pour tout $\varepsilon > 0$, il existe donc un voisinage ouvert U de 0 tel que $\alpha(U) \leq \varepsilon$. Comme le produit dans K est continu, on a $aC \subset U$ pour $a$ assez voisin de 0, et alors $\mathrm{mod}(a) \leq \varepsilon / \alpha(C)$.

#### Proposition 13 {#int-vii-s1-prop-13 .statement}

Pour tout $M > 0$, soit $V_M$ l’ensemble des $x \in K$ tels que $\mathrm{mod}(x) \leq M$. Si K est non discret, les $V_M$ forment un système fondamental de voisinages compacts de 0 dans K.

Les $V_M$ sont des voisinages fermés de 0 d’après la prop. 12. Montrons qu’ils sont compacts. Soit U un voisinage compact de 0. Il existe un $r \neq 0$ dans K tel que $\mathrm{mod}(r) < 1$ et $r^n \in U$ pour tout $n > 0$: en effet, soit W un voisinage de 0 tel que $WU \subset U$; d’après la prop. 12, il existe un $r \neq 0$ dans K tel que $\mathrm{mod}(r) < 1$ et $r \in U \cap W$; on a $r^2 \in WU \subset U$, et $r^n \in U$ pour tout $n > 0$, par récurrence sur $n$. Nous allons montrer que $V_M$ est contenu dans une réunion finie d’ensemble $r^{-q}U$ ($q$ entier $\geqslant 0$), ce qui prouvera bien que les $V_M$ sont compacts. Si $x$ est une valeur d’adhérence de la suite $(r^n)$, $\mathrm{mod}(x)$ est valeur d’adhérence de la suite $(\mathrm{mod}(r)^n)$, donc $\mathrm{mod}(x) = 0,\ x = 0$; comme U est compact, on en conclut (*Top. Gén.*, chap. I, 3e éd., § 9, no 1, cor. du th. 7) que $\lim_{n \to \infty} r^n = 0$. Soit alors $a \in V_M$.

Comme la suite $(r^n a)_{n \geqslant 0}$ tend vers 0, il existe un plus petit entier $n \geqslant 0$ tel que $r^n a \in U$. Si $n > 0$, on a $r^{n-1} a \notin U$, donc $r^n a \in U \cap C(rU)$; l’adhérence X de $U \cap C(rU)$ est compacte puisque U est compact, et ne contient pas 0 puisque $rU$ est un voisinage de 0 ; donc, dans X, $\mathrm{mod}\, x$ est minoré par un nombre $m > 0$. Donc, si $n > 0$, on a $m \leqslant \mathrm{mod}(r^n a)$, d’où $\mathrm{mod}(r^{-1})^n \leqslant M/m$. Comme $\mathrm{mod}(r^{-1}) > 1$, l’entier $n$ n’est susceptible que d’un nombre fini de valeurs ne dépendant pas de $a$, ce qui achève de prouver notre assertion.

Ceci étant, comme l’intersection des $V_M$ est réduite à {0}, les $V_M$ forment un système fondamental de voisinages de 0 (*Top. Gén.*, Chap. I, 3e éd., § 9, no 2, prop. 1).

#### Corollaire {#int-vii-s1-n10-cor-1 .statement}

*La topologie d’un corps localement compact non discret admet une base dénombrable*.

En effet, K est réunion des ensembles compacts $V_1, V_2, \ldots$. D’autre part, K est métrisable d’après la prop. 1 de *Top. Gén.*, Chap. IX, 2e éd., § 3, no 1. Donc la topologie de K admet une base dénombrable (*loc. cit.*, § 2, cor. de la prop. 16).

#### Proposition 14 {#int-vii-s1-prop-14 .statement}

*Soit $\alpha$ une mesure de Haar sur $K^+$. Alors la mesure $\beta = (\mathrm{mod}_K)^{-1} \cdot \alpha$ sur $K^*$ est une mesure de Haar à gauche sur le groupe multiplicatif $K^*$.*

En effet, si $b \in K^*$, l’application $a \to b^{-1}a$ de $K$ dans $K$ transforme $\alpha$ en $(\mathrm{mod}_K\ b)\alpha$, donc $(\mathrm{mod}_K)^{-1}\alpha$ en elle-même, d’où la proposition.

#### Corollaire {#int-vii-s1-n10-cor-2 .statement}

*Soit $f$ une fonction définie dans $K^*$, à valeurs dans $\overline{\mathbf{R}}$ ou dans un espace de Banach. Pour que $f$ soit $\beta$-intégrable, il faut et il suffit que $(\mathrm{mod}_K)^{-1}f$ soit $\alpha$-intégrable, et on a*

$$
\int_{K^*} f(x)d\beta(x) = \int_{K^+} (\mathrm{mod}_K(x))^{-1}f(x)d\alpha(x).
$$

Ceci résulte de la prop. 14, du cor. de la prop. 13, et du chap. V, § 5, no 3, th. 1.

#### Proposition 15 {#int-vii-s1-prop-15 .statement}

*Supposons $K$ commutatif. Soit $u$ un automorphisme de l’espace vectoriel $E = K^n$. Alors*

$$
\mathrm{mod}_E u = \mathrm{mod}_K (\det u).
$$

Il suffit de vérifier la formule lorsque $u$ parcourt un système de générateurs de $\mathbf{GL}(E)$. Or $\mathbf{GL}(E)$ est engendré par les éléments suivants (*Alg.*, chap. II, 3e éd., § 10, no 13, cor. 2 de la prop. 14) :
(a) les éléments $u_1$ de la forme

$$
(x_1, \ldots, x_n) \to (x_{\sigma(1)}, \ldots, x_{\sigma(n)}),
$$
où $\sigma \in \mathfrak{S}_n$;
(b) les éléments $u_2$ de la forme

$$
(x_1, \ldots, x_n) \to (ax_1, x_2, \ldots, x_n)
$$
avec $a \in K^*$;
(c) les éléments $u_3$ de la forme

$$
(x_1, \ldots, x_n) \to (x_1 + \sum_{i=2}^n c_i x_i, x_2, \ldots, x_n).
$$

Si $f \in \mathcal{K}(E)$, on a, en notant $\alpha$ une mesure de Haar sur $K^+$,

$$
\int \cdots \int_{K^n} f(x_1 + \sum_{i=2}^n c_i x_i, x_2, \ldots, x_n) d\alpha(x_1) d\alpha(x_2) \cdots d\alpha(x_n)
$$
$$
= \int \cdots \int_{K^{n-1}} d\alpha(x_2) \cdots d\alpha(x_n) \int_K f(x_1 + \sum_{i=2}^n c_i x_i, x_2, \ldots, x_n) d\alpha(x_1)
$$
$$
= \int \cdots \int_{K^{n-1}} d\alpha(x_2) \cdots d\alpha(x_n) \int_K f(x_1, x_2, \ldots, x_n) d\alpha(x_1)
$$
$$
= \int \cdots \int_{K^n} f(x_1, \ldots, x_n) d\alpha(x_1) \cdots d\alpha(x_n);
$$

et d'autre part $\mathrm{mod}_K (\det u_3) = \mathrm{mod}_K(1) = 1$, d'où le résultat pour $u_3$. On l'établit de manière analogue pour $u_1$ et $u_2$.

Soient K un corps localement compact commutatif, E un espace vectoriel de dimension finie n sur K. Si $\varphi$ est un isomorphisme de l'espace vectoriel $K^n$ sur l'espace vectoriel E, $\varphi$ transforme la topologie de $K^n$ en une topologie sur E qui fait de E un espace vectoriel localement compact. Cette topologie (dite canonique) est indépendante de $\varphi$ puisque tout automorphisme de l'espace vectoriel $K^n$ est bicontinu. Sauf mention du contraire, quand on parlera de E comme d'un espace vectoriel topologique, il s'agira toujours de la topologie qu'on vient de définir. Tout automorphisme $u$ de l'espace vectoriel E est bicontinu, donc $\mathrm{mod}_E u$ est défini. Par ailleurs, si $u$ est un endomorphisme non inversible de E, on pose $\mathrm{mod}_E u = 0$. Alors :

#### Corollaire 1 {#int-vii-s1-prop-15-cor-1 .statement}

*Soient K un corps localement compact commutatif, E un espace vectoriel de dimension finie sur K, et u un endomorphisme de l'espace vectoriel E. On a*
$$
\mathrm{mod}_E(u) = \mathrm{mod}_K(\det u).
$$
Si $u$ est inversible, cela résulte de la prop. 15. Si $u$ n'est pas inversible, on a $\det u = 0$, donc $\mathrm{mod}_K(\det u) = 0 = \mathrm{mod}_E u$.

#### Corollaire 2 {#int-vii-s1-prop-15-cor-2 .statement}

*Soient E un espace vectoriel réel de dimension finie n, $(e_1, e_2, \ldots, e_n)$ une base de E, P l'ensemble des $x = \sum_{i=1}^n \xi_i e_i \in E$ tels que $0 \leq \xi_i \leq 1$ pour tout i, $\mu$ l'unique mesure de Haar sur le groupe additif E telle que $\mu(P) = 1$. Soient $x_1, \ldots, x_n$ des points de E, S l’enveloppe convexe fermée dans E de l’ensemble $\{0, x_1, \ldots, x_n\}$. Si on pose $x_i = \sum_{j=1}^n \alpha_{ij} e_j$, on a

$$
\mu(S) = \mu(\dot{S}) = \frac{1}{n!} |\det(\alpha_{ij})|.
$$

Nous identifierons E à $\mathbf{R}^n$ par l’isomorphisme qui transforme $(e_i)$ en la base canonique de $\mathbf{R}^n$. Alors $\mu$ s’identifie à la mesure de Lebesgue $\mu_n$ sur $\mathbf{R}^n$.

Supposons d’abord que $x_i = e_i$ pour tout i. Alors S est l’ensemble $S_n$ des $x = (\xi_i) \in \mathbf{R}^n$ tels que

$$
\xi_i \geqslant 0 \text{ pour tout } i \text{ et } \xi_1 + \ldots + \xi_n \leqslant 1.
$$

Posons $\mu_n(S_n) = a_n$. Soit $\lambda \in \mathbf{R}$. Identifiant $\mathbf{R}^n$ à $\mathbf{R}^{n-1} \times \mathbf{R}$, on peut considérer la coupe $C_\lambda$ de $S_n$ suivant $\lambda$. Cette coupe est vide si $\lambda < 0$ ou $\lambda > 1$; si $0 \leqslant \lambda \leqslant 1$, $C_\lambda$ est l’ensemble des $(\xi_1, \ldots, \xi_{n-1}) \in \mathbf{R}^{n-1}$ tels que

$$
\xi_1 \geqslant 0, \ldots, \xi_{n-1} \geqslant 0, \quad \xi_1 + \ldots + \xi_{n-1} \leqslant 1 - \lambda,
$$

donc se déduit de $S_{n-1}$ par une homothétie de rapport $1 - \lambda$, de sorte que $\mu_{n-1}(C_\lambda) = (1 - \lambda)^{n-1} a_{n-1}$. D’après le théorème de Lebesgue-Fubini,

$$
a_n = \int_0^1 (1 - \lambda)^{n-1} a_{n-1} d\lambda = \frac{1}{n} a_{n-1}.
$$

Comme $a_1 = 1$, on voit que $a_n = \frac{1}{n!}$.

Revenons au cas général du corollaire. Soit u l’endomorphisme de $\mathbf{R}^n$ tel que $u(e_i) = x_i$ pour tout i. On a $u(S_n) = S$. Si u est inversible, la prop. 15 prouve que

$$
\mu_n(S) = \frac{1}{n!} |\det u| = \frac{1}{n!} |\det(\alpha_{ij})|.
$$

Comme $S - \dot{S}$ est contenu dans un nombre fini d’hyperplans, on a $\mu(\dot{S}) = \mu(S)$. Enfin, si u est non inversible, S est contenu dans un hyperplan, de sorte que $\mu(S) = 0 = \det(\alpha_{ij})$.

### 11. Algèbres de dimension finie sur un corps localement compact.

Soient K un corps commutatif, A une K-algèbre de rang fini à élément unité. Pour tout $a \in A$, soient $L_a, R_a$ les endomorphismes $x \to ax, x \to xa$ de l’espace vectoriel A, et soient $N_{A/K}(a) \in K, N_{A^o/K}(a) \in K$ les normes de $a$ dans les représentations régulières de A et de l’algèbre opposée $A^o$; rappelons que $N_{A/K}(a) = \det(L_a), N_{A^o/K}(a) = \det(R_a)$. Les conditions suivantes sont équivalentes : $a$ inversible, $L_a$ inversible dans $\mathrm{Hom}_K(A,A)$, $R_a$ inversible dans $\mathrm{Hom}_K(A,A)$, $N_{A/K}(a) \neq 0$, $N_{A^o/K}(a) \neq 0$. Notons $A^*$ l’ensemble des éléments inversibles de A.

Supposons maintenant le corps K localement compact, donc l’algèbre A localement compacte. Alors $N_{A/K}$ et $N_{A^o/K}$ sont des applications continues de A dans K, donc $A^*$ est ouvert dans A. D’après le cor. 1 de la prop. 15 du no 10, on a

$$
\mathrm{mod}_A L_a = \mathrm{mod}_K N_{A/K}(a), \quad \mathrm{mod}_A R_a = \mathrm{mod}_K N_{A^o/K}(a).
$$

#### Proposition 16 {#int-vii-s1-prop-16 .statement}

Soit $\alpha$ une mesure de Haar du groupe additif de A. Les mesures

$$
(\mathrm{mod}_K N_{A/K}(a))^{-1} d\alpha(a), \quad (\mathrm{mod}_K N_{A^o/K}(a))^{-1} d\alpha(a)
$$

sur $A^*$ sont des mesures de Haar respectivement à gauche et à droite du groupe multiplicatif $A^*$.

En effet, soit $\alpha'$ la restriction de $\alpha$ à l’ensemble ouvert $A^*$. Pour $a \in A^*$, on a $L_a(\alpha') = (\mathrm{mod}_K N_{A/K}(a))^{-1} \alpha'$, donc

$$
(\mathrm{mod}_K N_{A/K}(a))^{-1} d\alpha'(a)
$$

est une mesure de Haar à gauche sur $A^*$ (no 8, cor. 1 de la prop. 10). Passant à l’algèbre opposée, on voit que

$$
(\mathrm{mod}_K N_{A^o/K}(a))^{-1} d\alpha'(a)
$$

est une mesure de Haar à droite sur $A^*$.

#### Proposition 17 {#int-vii-s1-prop-17 .statement}

Supposons que $A$ soit un corps (localement compact). Pour tout $a \in A$, on $a \mod_A(a) = \mathrm{mod}_K N_{A/K}(a)$.

C'est une traduction de la première formule (38).

#### Exemple 1 {#int-vii-s1-n11-exa-1 .statement}

Prenons $K = \mathbf{R}$, $A = \mathbf{C}$. Compte tenu d'Alg., chap. VIII, § 12, n° 2, prop. 4, on obtient $\mathrm{mod}_C(z) = |z|^2$ pour tout $z \in \mathbf{C}$.

#### Exemple 2 {#int-vii-s1-n11-exa-2 .statement}

Prenons $K = \mathbf{R}$, et pour $A$ le corps des quaternions $\mathbf{H}$ (Top. Gén., chap. VIII, 3e éd., § 1, n° 4). Considérons les éléments suivants de $\mathbf{M}_2(\mathbf{C})$:

$$
X_1 = \begin{pmatrix} 0 & i \\ i & 0 \end{pmatrix} \quad X_2 = \begin{pmatrix} 0 & -1 \\ 1 & 0 \end{pmatrix} \quad X_3 = \begin{pmatrix} i & 0 \\ 0 & -i \end{pmatrix}
$$

qui, avec $I_2$, forment une base de $\mathbf{M}_2(\mathbf{C})$ sur $\mathbf{C}$. On vérifie aisément que

$$
X_1^2 = X_2^2 = X_3^2 = -I_2, \quad X_1 X_2 = -X_2 X_1 = X_3,
$$
$$
X_2 X_3 = -X_3 X_2 = X_1, \quad X_3 X_1 = -X_1 X_3 = X_2.
$$

Donc l'application $a + b i + c j + d k \to a I_2 + b X_1 + c X_2 + d X_3$ se prolonge en un $\mathbf{C}$-isomorphisme de l'algèbre $\mathbf{C} \otimes_\mathbf{R} \mathbf{H}$ sur l'algèbre $\mathbf{M}_2(\mathbf{C})$. Comme $[\mathbf{H} : \mathbf{R}] = 4$, $\mathbf{C}$ est un corps neutralisant de $\mathbf{H}$, et la norme réduite de $q = a + b i + c j + d k \in \mathbf{H}$ est

$$
\mathrm{Nrd}(q) = \det(a I_2 + b X_1 + c X_2 + d X_3)
$$
$$
= \det \begin{pmatrix} a + id & -c + ib \\ c + ib & a - id \end{pmatrix} = a^2 + b^2 + c^2 + d^2 = \|q\|^2.
$$

D'après Alg., chap. VIII, § 12, n° 3, prop. 8, on a

$$
N_{\mathbf{H}/\mathbf{R}}(q) = (\mathrm{Nrd}_{\mathbf{H}/\mathbf{R}}(q))^2 = \|q\|^4.
$$

Ceci posé, la prop. 17 montre que

$$
\mathrm{mod}_\mathbf{H}(q) = \|q\|^4.
$$

Une étude plus approfondie de la structure des corps localement compacts sera faite en Alg. comm., chap. VI, § 9.

## EXERCICES {#int-vii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
