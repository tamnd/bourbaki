---
book: int
book_title: Integration
chapter: III
chapter_title: Mesures sur les espaces localement compacts
section: 3
section_title: Intégrales de fonctions vectorielles continues
lang: fr
source: int-i-iv-fr
pdf_pages: 0078-0086, 0106-0107
extraction: ocr
subsections:
    - "no": 1
      title: Définition de l’intégrale d’une fonction vectorielle
      page: 0
      pdf_page: 78
    - "no": 2
      title: Propriétés de l’intégrale vectorielle
      page: 0
      pdf_page: 81
    - "no": 3
      title: Critères pour que l’intégrale appartienne à $E$.
      page: 0
      pdf_page: 83
    - "no": 4
      title: Propriétés de continuité de l’intégrale
      page: 0
      pdf_page: 85
statements: 19
exercises: 4
content_sha256: c85d2ebc1d31dcfec8415642d18d53234a635f52ad050b1d3b81aa50845b850d
---

## § 3. Intégrales de fonctions vectorielles continues

Dans tout ce paragraphe, on note $X$ un espace localement compact, $E$ un espace localement convexe sur $\mathbf{R}$ ou $\mathbf{C}$. On note $E'$ le dual de $E$ (espace des formes linéaires continues sur $E$), ${E'}^*$ le dual algébrique de $E'$ (espace de toutes les formes linéaires sur $E'$); pour $z \in E$, $z' \in E'$, ${z'}^* \in {E'}^*$, on écrit $\langle z, z' \rangle = z'(z)$, $\langle {z'}^*, z' \rangle = {z'}^*(z')$.

On rappelle que si $E$ est séparé, $E$ s’identifie à un sous-espace de ${E'}^*$ en identifiant un élément $z \in E$ à la forme linéaire $z' \mapsto \langle z, z' \rangle$ sur $E'$, et que ${E'}^*$, muni de la topologie faible $\sigma({E'}^*, E')$, s’identifie canoniquement au complété de $E$ muni de la topologie affaiblie $\sigma(E, E')$.

### 1. Définition de l’intégrale d’une fonction vectorielle

Rappelons qu’une application $f$ de $X$ dans $E$ est dite faiblement continue si, pour tout $z' \in E'$, l’application $x \mapsto \langle f(x), z' \rangle$ de $X$ dans $\mathbf{C}$ (autrement dit l’application $z' \circ f$, notée aussi $\langle f, z' \rangle$) est continue. Nous dirons qu’une application $f$ de $X$ dans $E$ est scalairement à support compact si, pour tout $z' \in E'$, l’application $x \mapsto \langle f(x), z' \rangle$ a un support compact. Nous désignerons par $\tilde{\mathcal{K}}(X; E)$ l’espace des applications de $X$ dans $E$ qui sont faiblement continues et scalairement à support compact ; il est clair que l’on a $\tilde{\mathcal{K}}(X; E) \supset \mathcal{K}(X; E)$, mais ces deux espaces ne sont pas nécessairement identiques (voir ci-dessous, Exemple 2); ils le sont toutefois lorsque $E$ est de dimension finie.

On notera que dans la définition d’une fonction faiblement continue (resp. scalairement à support compact), la topologie de $E$ n’intervient que par l’intermédiaire du dual $E'$ de $E$; on ne change donc pas l’ensemble de ces fonctions quand on remplace la topologie de $E$ par toute topologie localement convexe pour laquelle le dual est le même.

Si $E$ et $F$ sont deux espaces vectoriels en dualité, on notera qu’il revient au même de dire qu’une application de $X$ dans $E$ est continue pour $\sigma(E, F)$ ou qu’elle est faiblement continue.

Soit $f$ une application de $X$ dans $E$, faiblement continue et scalairement à support compact, et soit $\mu$ une mesure sur $X$; pour tout $z' \in E'$, on a $z' \circ f \in \mathcal{K}(X)$; posons

$$
\varphi(z') = \int \langle f(x), z' \rangle \, d\mu(x) = \mu(z' \circ f).
$$

Il est clair que $\varphi$ est une forme linéaire sur $E'$, donc un élément de ${E'}^*$.

#### Définition 1 {#int-iii-s3-def-1 .statement}

Pour toute fonction $f \in \tilde{\mathcal{K}}(X; E)$, on appelle intégrale de $f$ par rapport à $\mu$ et on note $\int f \, d\mu$ ou $\int f(x) \, d\mu(x)$, ou $\int f \mu$, ou $\int f(x) \mu(x)$, l’élément de ${E'}^*$ défini par

$$
\left\langle \int f \, d\mu, z' \right\rangle = \int \left\langle f, z' \right\rangle \, d\mu \quad \text{pour tout } z' \in E'.
$$

Lorsque $E$ est séparé, on notera que l’on n’a pas nécessairement $\int f \, d\mu \in E$, même lorsque $f \in \mathcal{K}(X; E)$ (exerc. 1 ; cf. n° 3).

#### Exemple 1 {#int-iii-s3-n1-exa-1 .statement}

Supposons que $E$ soit de dimension finie sur $\mathbf{C}$ et séparé, de sorte que si $(e_i)_{1 \leq i \leq n}$ est une base de $E$, l’application

$$
(\xi_1, \ldots, \xi_n) \mapsto \sum_{i=1}^n \xi_i e_i
$$

est un isomorphisme de $\mathbf{C}^n$ sur $E$. On sait alors que toute forme linéaire sur $E$ est continue, autrement dit $E'$ est identique au dual algébrique $E^*$ de $E$, et ${E'}^*$ s’identifie canoniquement à $E$. Soit $(e'_i)_{1 \leq i \leq n}$ la base duale de $(e_i)$ dans $E'$; pour qu’une application $f$ de $X$ dans $E$ soit faiblement continue et scalairement à support compact, il faut et il suffit que les fonctions $f_i = e'_i \circ f$ soient continues à support compact; on a alors $f(x) = \sum_{i=1}^n f_i(x) e_i$ pour

tout $x \in X$, et
$$
\int f d\mu = \sum_{i=1}^n \mu(f_i) e_i.
$$

#### Exemple 2 {#int-iii-s3-n1-exa-2 .statement}

Prenons pour E l’espace $\mathcal{M}(X; \mathbf{C})$ des mesures sur X, muni de la topologie vague ($§ 1$, n° 9); le dual $E'$ de E s’identifie alors canoniquement à l’espace $\mathcal{K}(X; \mathbf{C})$ (*Esp. vect. top.*, chap. I, 2e éd., $§ 6$, n° 2, prop. 3). L’application $x \mapsto \varepsilon_x$ de X dans E est continue ($§ 1$, n° 9, prop. 13), mais son support n’est pas compact si X n’est pas compact; toutefois elle est *scalairement à support compact*, car pour toute fonction $f \in E'$, la fonction $x \mapsto \langle \varepsilon_x, f \rangle = f(x)$ a par définition un support compact. En outre, on a
$$
\int \langle \varepsilon_x, f \rangle d\mu = \int f(x) d\mu(x) = \langle \mu, f \rangle
$$
pour toute fonction $f \in \mathcal{K}(X; \mathbf{C}) = E'$, ce qui prouve que
$$
\int \varepsilon_x d\mu(x) = \mu
$$
pour toute mesure $\mu$ sur X.

#### Exemple 3 {#int-iii-s3-n1-exa-3 .statement}

Si E est séparé, pour tout point $y \in X$ et toute fonction $f \in \tilde{\mathcal{K}}(X; E)$, on a
$$
\int f d\varepsilon_y = f(y)
$$
car $\int \langle f, z' \rangle d\varepsilon_y = \langle f(y), z' \rangle$ par définition.

#### Remarque 1 {#int-iii-s3-n1-rem-1 .statement}

Si E est un espace localement convexe, N l’adhérence de $\{0\}$ dans E, de sorte que $E_1 = E/N$ est l’espace localement convexe séparé associé à E, on sait que les duals $E'$ et $E'_1$ sont identiques; pour qu’une fonction $f$ appartienne à $\tilde{\mathcal{K}}(X; E)$, il faut et il suffit que $f_1 = \pi \circ f$ (où $\pi : E \to E_1$ est l’homomorphisme canonique) appartienne à $\tilde{\mathcal{K}}(X; E_1)$, et l’on alors $\int f d\mu = \int f_1 d\mu$. On peut donc se limiter à ne considérer que des espaces localement convexes séparés.

#### Remarque 2 {#int-iii-s3-n1-rem-2 .statement}

Soit E un espace localement convexe sur $\mathbf{C}$, et soit $E_0$ l’espace localement convexe sur $\mathbf{R}$ sous-jacent à E; on sait que l’application $z' \mapsto \Re z'$ qui à toute forme linéaire (complexe) continue $z'$ sur E fait correspondre la forme linéaire continue (réelle) $z \mapsto \Re \langle z, z' \rangle$ sur $E_0$, est un $\mathbf{R}$-isomorphisme du dual $E'$ sur le dual $E'_0$ de $E_0$ (*Esp. vect. top.*, chap. II, 2e éd., $§ 8$, n° 1). De même le dual algébrique $E'_0*$ de l’espace vectoriel réel $E'_0$ s’identifie canoniquement à l’espace réel sous-jacent au dual algébrique $E'*$ de $E'$. On en déduit que si $\mu$ est une *mesure réelle* et $f$ une application de $\tilde{\mathcal{K}}(X; E)$, la formule (1) est encore valable lorsque l’on considère $f$ comme prenant ses valeurs dans $E_0$ et que les formes bilinéaires canoniques figurant aux deux membres sont respectivement *relatives* à la dualité entre $E'_0$ et $E'_0*$ au premier membre, à la dualité entre $E_0$ et $E'_0$ au second.

### 2. Propriétés de l’intégrale vectorielle

#### Proposition 1 {#int-iii-s3-prop-1 .statement}

L’application
$$(f, \mu) \mapsto \int f d\mu$$
de $\tilde{\mathcal{K}}(X; E) \times \mathcal{M}(X; \mathbf{C})$ dans ${E'}^*$ est bilinéaire.
La proposition résulte immédiatement de la déf. 1 du n° 1.

Soit $u$ une application linéaire continue de $E$ dans un espace localement convexe $F$; on sait que la transposée $'u$ est une application linéaire du dual $F'$ de $F$ dans le dual $E'$ de $E$; nous désignerons par $"u$ l’application ${E'}^* \to {F'}^*$, transposée de $'u$ (au sens algébrique); lorsque $E$ et $F$ sont séparés, et identifiés canoniquement à des sous-espaces de ${E'}^*$ et ${F'}^*$ respectivement, $"u$ prolonge l’application $u$. Avec ces notations :

#### Proposition 2 {#int-iii-s3-prop-2 .statement}

Soit $u$ une application linéaire continue de $E$ dans un espace localement convexe $F$; pour toute fonction $f \in \tilde{\mathcal{K}}(X; E)$, la fonction $u \circ f$ appartient à $\tilde{\mathcal{K}}(X; F)$, et l’on a
$$
\int u(f(x))\, d\mu(x) = "u \left( \int f(x)\, d\mu(x) \right).
$$
Pour toute forme linéaire continue $z' \in F'$, on a $z' \circ u \circ f = y' \circ f$ en posant $y' = z' \circ u = 'u(z') \in E'$, d’où la première assertion ; en outre, on a, pour tout $z' \in F'$,
$$
\left\langle \int (u \circ f)\, d\mu, z' \right\rangle = \int \left\langle u \circ f, z' \right\rangle\, d\mu =
= \int \left\langle f, 'u(z') \right\rangle\, d\mu = \left\langle \int f\, d\mu, 'u(z') \right\rangle = \left\langle "u \left( \int f\, d\mu \right), z' \right\rangle
$$
d’où la formule (2).

#### Proposition 3 {#int-iii-s3-prop-3 .statement}

Pour toute fonction $g \in \mathcal{C}(X; \mathbf{C})$ et toute fonction $f \in \tilde{\mathcal{K}}(X; E)$, la fonction $gf$ appartient à $\tilde{\mathcal{K}}(X; E)$, et l’on a
$$
\int f\, d(g \cdot \mu) = \int fg\, d\mu.
$$
En effet, pour tout $z' \in E'$, on a $\langle gf, z' \rangle = g \langle f, z' \rangle$, d’où la première assertion ; en outre
$$
\left\langle \int f\, d(g \cdot \mu), z' \right\rangle = \int \left\langle f, z' \right\rangle\, d(g \cdot \mu) = \int g \left\langle f, z' \right\rangle\, d\mu
= \int \left\langle gf, z' \right\rangle\, d\mu = \left\langle \int gf\, d\mu, z' \right\rangle
$$
d’où (3).

#### Proposition 4 {#int-iii-s3-prop-4 .statement}

Soient $\mu$ une mesure positive sur $X$, S son support, $f$ une fonction de $\mathcal{K}(X; E)$. On suppose E séparé, et on munit l’espace ${E'}^*$ de la topologie faible $\sigma({E'}^*, E')$.

(i) L’intégrale $\int f \, d\mu$ appartient à l’adhérence $C$ dans ${E'}^*$ du cône convexe engendré par $f(S)$.

(ii) Si $\mu$ est bornée, l’intégrale $\int f \, d\mu$ appartient à l’ensemble $\| \mu \| . D$, où $D$ est l’enveloppe convexe fermée de $f(S)$ dans ${E'}^*$.

Si E est complexe, munissons E de sa structure d’espace vectoriel réel sous-jacente, ce qui, comme on l’a vu, ne modifie pas la formule (1).

(i) On sait que $C$ est l’intersection des demi-espaces fermés dans ${E'}^*$ contenant $f(S)$, et déterminés par des hyperplans fermés passant par 0 ; il suffit donc de démontrer que, pour $z' \in E'$, la relation $\langle f(x), z' \rangle \geqslant 0$ pour tout $x \in S$ entraîne

$$
\left\langle \int f \, d\mu, z' \right\rangle \geqslant 0;
$$

mais comme

$$
\left\langle \int f \, d\mu, z' \right\rangle = \int \langle f, z' \rangle \, d\mu,
$$

cela résulte du § 2, n° 3, cor. 2 de la prop. 8.

(ii) On sait que $D$ est l’intersection des demi-espaces fermés dans ${E'}^*$ qui contiennent $f(S)$; il suffit donc de démontrer que, pour $z' \in E'$, la relation $\langle f(x), z' \rangle \leqslant a$ pour tout $x \in S$ entraîne

$$
\left\langle \int f \, d\mu, z' \right\rangle \leqslant a \| \mu \|;
$$

mais cela résulte du § 2, n° 3, cor. 3 de la prop. 8.

#### Corollaire {#int-iii-s3-n2-cor-1 .statement}

Soient $\mu$ une mesure positive sur $X$, $f$ une application appartenant à $\mathcal{K}(X; E)$, $D$ l’enveloppe fermée convexe de $f(X)$ dans ${E'}^*$. Il existe un nombre $a > 0$ tel que l’on ait $\int f \, d\mu \in a . D$.

Si $\nu$ est une mesure quelconque sur $X$, il existe des nombres $a_1, a_2, a_3, a_4 > 0$ tels que $\int f \, d\nu \in a_1 D - a_2 D + i a_3 D - i a_4 D$.

Supposons d’abord $\mu$ positive ; par hypothèse, le support K de $f$ est compact ; si $\nu$ est la restriction de $\mu$ à un voisinage ouvert relativement compact de K, $\nu$ est bornée, et l’on a $\int f \, d\mu = \int f \, d\nu \in \| \nu \| . D$ en vertu de la prop. 4, (ii). Le deuxième résultat s’en déduit puisqu’une mesure complexe quelconque s’écrit $\mu_1 - \mu_2 + i \mu_3 - i \mu_4$, où les $\mu_j$ sont positives.

#### Proposition 5 {#int-iii-s3-prop-5 .statement}

Supposons l’espace $X$ compact, et soit $f$ une application continue de $X$ dans un espace localement convexe séparé $E$. L’enveloppe fermée convexe de $f(X)$ dans ${E'}^*$ (pour $\sigma({E'}^*, E')$) est égale à l’ensemble des vecteurs $\int f \, d\mu$ pour toutes les mesures positives $\mu$ de masse 1 sur $X$.

Soit C l’enveloppe fermée convexe de $f(X)$ dans $E'$; comme $f(X)$ est compact et $E'$ *complet*, C est compact. On sait déjà (prop. 4) que l’on a $\int f d\mu \in C$ pour toute mesure $\mu$ appartenant à l’ensemble convexe $H$ des mesures positives sur $X$ de masse totale égale à 1. D’autre part, $H$ est convexe et *compact* pour la topologie vague ($§ 1, n° 9,$ cor. 3 de la prop. 15), et est l’adhérence (pour cette topologie) de l’ensemble convexe $H_0$ des mesures positives de masse 1 et de support *fini* ($§ 2, n° 5,$ cor. 3 du th. 1). Or, l’image de $H_0$ par l’application $\mu \mapsto \int f d\mu$ est l’enveloppe convexe $C_0$ de $f(X)$ dans $E'$. D’autre part, cette application est continue pour la topologie vague sur $\mathcal{M}(X; C)$ et la topologie $\sigma(E', E')$ sur $E'$ puisque $\langle \int f d\mu, z' \rangle = \int \langle f, z' \rangle d\mu$ par définition; donc l’image de $H = \overline{H}_0$ est un ensemble convexe *compact* contenant $C_0$ et contenu dans $C$; comme $C = \overline{C}_0$, cette image est égale à $C$.

#### Proposition 6 {#int-iii-s3-prop-6 .statement}

*Pour toute application continue et à support compact* $f$ *de* $X$ *dans un espace localement convexe séparé* $E$, *toute semi-norme continue* $q$ *sur* $E$ *et toute mesure* $\mu$ *sur* $X$ *telle que* $\int f d\mu \in E$, *on a*
$$
q\left( \int f d\mu \right) \leq \int (q \circ f) d|\mu|.
$$
(4)

Soit $D$ l’ensemble des $z \in E$ tels que $q(z) \leq 1$; $D$ est fermé, convexe et contient 0, donc on a $D = D^{oo}$ (*Esp. vect. top.* chap. IV, $§ 2, n° 3,$ cor. 2 de la prop. 4). Il suffit donc de prouver que pour tout $z' \in D^o$ on a
$$
|\langle \int f d\mu, z' \rangle| \leq \int (q \circ f) d|\mu|;
$$
comme
$$
\langle \int f d\mu, z' \rangle = \int \langle f, z' \rangle d\mu,
$$
et que par définition de $D^o$, on a
$$
|\langle f(x), z' \rangle| \leq q(f(x))
$$
pour tout $x \in X$, cela résulte de l’inégalité (13) du $§ 1, n° 6$.

### 3. Critères pour que l’intégrale appartienne à $E$.

#### Proposition 7 {#int-iii-s3-prop-7 .statement}

*Soient* $E$ *un espace localement convexe séparé* $E$, *et* $f \in \mathcal{H}(X; E)$. *Si* $f(X)$ *est contenu dans une partie convexe complète* $A$ *de* $E$, *on a* $\int f d\mu \in E$.

Soit $K$ le support de $f$, qui est compact par hypothèse. Comme $f$ est nulle dans $X - K$, $f(X)$ est égal à $f(K)$ ou à $f(K) \cup \{0\}$, donc est compact puisque $f$ est continue et $E$ séparé ; l’enveloppe convexe fermée $C$ de $f(X)$ dans $E$ est alors précompacte (pour la structure uniforme induite par celle de $E$) (*Esp. vect. top.*, chap. II, 2\textsuperscript{e} éd., § 4, n\textsuperscript{o} 1, prop. 3). Mais comme $C$ est une partie fermée de l’espace complet $A$, $C$ est complet, donc compact ; *a fortiori*, $C$ est compact pour la topologie affaiblie $\sigma(E, E')$; mais comme celle-ci est induite par $\sigma({E'}^*, E')$, $C$ est l’enveloppe convexe fermée de $f(X)$ dans ${E'}^*$ pour la topologie $\sigma({E'}^*, E')$; on conclut donc par le cor. de la prop. 4 du n\textsuperscript{o} 2.

#### Corollaire 1 {#int-iii-s3-prop-7-cor-1 .statement}

*Soit* $E$ *un espace localement convexe séparé ; pour toute fonction* $f \in \mathscr{K}(X; E)$, $\int f \, d\mu$ *appartient au complété* $\hat{E}$ *de* $E$.

Comme les duals de $E$ et de $\hat{E}$ sont identiques, il suffit d’appliquer la prop. 6 en considérant que $f$ prend ses valeurs dans $\hat{E}$.

#### Corollaire 2 {#int-iii-s3-prop-7-cor-2 .statement}

*Si* $E$ *est un espace localement convexe séparé quasi-complet, on a* $\int f \, d\mu \in E$ *pour toute fonction* $f \in \mathscr{K}(X; E)$.

On a remarqué au début de la démonstration de la prop. 7 que $f(X)$ est compact et que son enveloppe convexe fermée $C$ dans $E$ est précompacte, donc bornée ; mais comme l’ensemble $C$ est fermé et borné, il est complet par hypothèse, et il suffit d’appliquer la prop. 7.

On verra au chap. VI, § 1, n\textsuperscript{o} 2, d’autres critères pour que $\int f \, d\mu$ appartienne à $E$, qui s’appliquent en particulier aux fonctions de $\mathscr{K}(X; E)$, et non plus seulement à celles de $\mathscr{K}(X; E)$.

Le cor. 2 de la prop. 7 s’applique dans les deux cas suivants : 1\textsuperscript{o} $E$ est un *espace de Banach* ; 2\textsuperscript{o} $E$ est le dual d’un espace localement convexe séparé *tonnelé* $G$, et on munit $E$ d’une $\mathcal{S}$-topologie, où $\mathcal{S}$ est un recouvrement de $G$ par des parties bornées (*Esp. vect. top.*, chap. III, § 3, n\textsuperscript{o} 7, cor. 2 du th. 4). Par exemple, on peut appliquer le cor. 2 de la prop. 7 lorsque $E$ est le dual faible d’un espace de Banach, ou un espace de mesures $\mathcal{M}(Y; \mathbf{C})$, muni de la topologie vague.

Si $X = \mathbf{R}$, si $\mu$ est la mesure de Lebesgue sur $\mathbf{R}$, et si $E$ est un *espace de Banach*, l’intégrale $\int f \, d\mu$ d’une fonction de $\mathscr{K}(X; E)$ n’est autre que l’intégrale

$$
\int_{-\infty}^{+\infty} f(x) \, dx
$$

définie dans *Fonct. var. réelle*, chap. II, § 3, n\textsuperscript{o} 1 ; cela résulte de la formule (1) et de *Fonct. var. réelle*, chap. II, § 3, n\textsuperscript{o} 1, formule (10).

### 4. Propriétés de continuité de l’intégrale

#### Proposition 8 {#int-iii-s3-prop-8 .statement}

Supposons E séparé; soit $\mu$ une mesure sur X. L’application $f \mapsto \int f d\mu$ de $\mathcal{K}(X;E)$ dans $\hat{E}$ (n° 3, cor. 1 de la prop. 7) est l’unique application linéaire continue $\Phi$ telle que $\Phi(g.a) = \mu(g).a$ pour tout vecteur $a \in E$ et toute fonction $g \in \mathcal{K}(X;C)$.

Pour prouver la continuité de l’application $f \mapsto \int f d\mu$, il suffit de montrer que sa restriction à $\mathcal{K}(X,K;E)$ est continue pour toute partie compacte K de X (Esp. vect. top., chap. II, 2e éd., §4, n° 4, prop. 5). Notons que si la topologie de E est définie par une famille de semi-normes $(q_\alpha)$, celle de $\mathcal{K}(X,K;E)$ est définie par la famille des semi-normes

$$
p_\alpha(f) = \sup_{x \in K} q_\alpha(f(x)).
$$

Or, soit h une application continue de X dans $[0,1]$, à support compact et telle que $h(x) = 1$ dans K; on a, en vertu du n° 2, prop. 6, pour toute fonction $f \in \mathcal{K}(X,K;E)$,

$$
q_\alpha\left( \int f d\mu \right) = q_\alpha\left( \int h f d\mu \right) \leq \int h(x) q_\alpha(f(x)) d|\mu|(x) \leq |\mu|(h) \cdot p_\alpha(f)
$$

(les $q_\alpha$ étant prolongées par continuité à $\hat{E}$) ce qui démontre la continuité de $f \mapsto \int f d\mu$. D’autre part, avec les notations de l’énoncé,

$$
\int (g(x).a) d\mu(x) = \mu(g).a
$$

en vertu du n° 1, Exemple 1 et de la prop. 2 du n° 2 appliquée à l’injection canonique $C.a \to E$. En outre, le sous-espace de $\mathcal{K}(X;E)$ formé des combinaisons linéaires $\sum_i g_i.a_i$, où $a_i \in E$ et $g_i \in \mathcal{K}(X;C)$, est dense dans $\mathcal{K}(X;E)$ (§ 1, n° 2, prop. 5), ce qui achève la démonstration.

#### Proposition 9 {#int-iii-s3-prop-9 .statement}

Supposons E séparé: soit f une application continue à support compact de X dans E. Lorsqu’on munit l’espace $\mathcal{M}(X;C)$ de la topologie de la convergence strictement compacte (§ 1, n° 10), l’application $\mu \mapsto \int f d\mu$ de $\mathcal{M}(X;C)$ dans $\hat{E}$ est l’unique application linéaire continue $\Psi$ telle que $\Psi(\varepsilon_x) = f(x)$ pour tout $x \in X$.

Pour tout $z' \in E'$, on a

$$
\left\langle \int f d\varepsilon_x, z' \right\rangle = \int (z' \circ f) d\varepsilon_x = z'(f(x)) = \left\langle f(x), z' \right\rangle
$$

d’où $\int f d\varepsilon_x = f(x)$. On sait par ailleurs que l’ensemble des mesures ponctuelles est dense dans $\mathcal{M}(X; \mathbf{C})$ pour la topologie de la convergence strictement compacte ($§ 2$, n° 4, cor. 4 du th. 1). Tout revient donc à prouver la continuité de l’application linéaire $u : \mu \mapsto \int f\, d\mu$. Pour cela, considérons l’application linéaire $v : z' \mapsto \langle f, z' \rangle$ de $E'$ dans $\mathscr{H}(X; \mathbf{C})$, et montrons que l’image par $v$ d’une partie équicontinue $H$ de $E'$ est contenue dans une partie strictement compacte de $\mathscr{H}(X; \mathbf{C})$. En effet, si $K$ est le support de $f$, les fonctions $\langle f, z' \rangle$ pour $z' \in H$ ont leur support contenu dans $K$; d’autre part, ces fonctions forment un ensemble équicontinu, et pour tout $x \in X$, l’ensemble des $z'(f(x))$ est borné ; notre assertion résulte donc du th. d’Ascoli (*Top. gén.*, chap. X, 2e éd., § 2, n° 5, cor. 3 du th. 2). Cela étant, il résulte de la formule (1) du n° 1 que $u$ n’est autre que la restriction à $\mathcal{M}(X; \mathbf{C})$ de la *transposée* $'v$ (au sens algébrique); sa continuité résulte donc de ce qui précède (*Esp. vect. top.*, chap. IV, 2e éd.).

#### Corollaire {#int-iii-s3-n4-cor-1 .statement}

*Les hypothèses et notations étant celles de la prop. 9, la restriction de l’application $\mu \mapsto \int f\, d\mu$ à l’ensemble $\mathcal{M}_+(X)$ des mesures positives, ou à une partie vaguement bornée B de $\mathcal{M}(X; \mathbf{C})$, est vaguement continue.*

En effet, il résulte du § 1, n° 10, prop. 17 et 18, que sur $\mathcal{M}_+(X)$ ou sur B la topologie induite par la topologie de la convergence strictement compacte est la même que la topologie induite par la topologie vague.

Par contre, l’application $\mu \mapsto \int f\, d\mu$ n’est pas nécessairement continue dans $\mathcal{M}(X; \mathbf{C})$ tout entier pour la topologie vague (exerc. 2).

## EXERCICES {#int-iii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
