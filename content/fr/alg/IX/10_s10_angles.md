---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 10
section_title: Angles
lang: fr
source: alg-ix-fr
pdf_pages: 0158-0182
extraction: ocr
subsections:
    - "no": 1
      title: Similitudes directes dans un plan.
      page: 0
      pdf_page: 158
    - "no": 2
      title: Trigonométrie plane.
      page: 0
      pdf_page: 162
    - "no": 3
      title: Angles.
      page: 0
      pdf_page: 165
    - "no": 4
      title: Secteurs angulaires.
      page: 0
      pdf_page: 171
statements: 31
exercises: 0
content_sha256: 0b84a77cc13c427d65a3661f23bd3ba63c6c888b0221377a85fb74aed39e12a6
---

## § 10. Angles

Dans tout ce paragraphe, A désigne un corps commutatif de caractéristique $\neq 2$, E un espace vectoriel de dimension 2 sur A, et $\Phi$ une forme bilinéaire symétrique non dégénérée sur E.

### 1. Similitudes directes dans un plan.

Rappelons (§ 6, n° 5) qu’une similitude directe de E est un automorphisme $u$ de l’espace vectoriel E tel que $\Phi(u(x), u(y)) = (\det u)\Phi(x, y)$ quels que soient $x, y$ dans E.

#### Proposition 1 {#alg-ix-s10-prop-1 .statement}

Soit $A(\Phi)$ la sous-algèbre de $\mathcal{L}_A(E)$ engendrée par les similitudes directes de E.

a) Les similitudes directes sont les éléments inversibles de $A(\Phi)$. L’algèbre $A(\Phi)$ est une algèbre commutative de degré 2 sur A. Lorsque E ne contient pas de vecteur isotrope $\neq 0$, $A(\Phi)$ est un corps, extension quadratique de A ; dans le cas contraire c’est la composée directe de deux corps isomorphes à A.

b) Soit $(e_1, e_2)$ une base orthogonale de E ; posons $\alpha_i = \Phi(e_i, e_i)$ $(i = 1, 2)$ et $\delta = -\alpha_2/\alpha_1$. Alors les matrices des éléments de $A(\Phi)$ par rapport à cette base sont les matrices de la forme $\begin{pmatrix} a & \delta b \\ b & a \end{pmatrix}$ où $a \in A, b \in A$.

c) L’espace E est un $A(\Phi)$-module libre monogène, engendré par n’importe quel vecteur non isotrope.

Introduisons en effet une forme bilinéaire alternée auxiliaire $B \neq 0$ sur E ; alors B est non dégénérée. Il existe donc un endon° 1

morphisme $\omega$ de E tel que $\Phi(x, y) = B(\omega(x), y)$ quels que soient $x, y$ dans E. Pour tout endomorphisme inversible $u$ de E, on a
$$
\begin{align*}
\Phi(u(x), u(y)) &= B(\omega u(x), u(y)) = B(uu^{-1}\omega u(x), u(y)) \\
&= (\det u)B(u^{-1}\omega u(x), y);
\end{align*}
$$
pour que $u$ soit une similitude directe, il faut et il suffit donc que l’on ait
$$
(\det u)B(u^{-1}\omega u(x), y) = (\det u)\Phi(x, y) = (\det u)B(\omega(x), y)
$$
quels que soient $x, y$ dans E ; comme $\det u \neq 0$ et que B est non dégénérée, ceci équivaut à $u^{-1}\omega u = \omega$, ou encore à $u\omega = \omega u$. Prenons pour B la forme bilinéaire alternée dont la matrice $S$ par rapport à $(e_1, e_2)$ est $\begin{pmatrix} 0 & 1 \\ -1 & 0 \end{pmatrix}$; en notant $R$ et $W$ les matrices de $\Phi$ et de $\omega$ par rapport à cette base, la relation $\Phi(x, y) = B(\omega(x), y)$ s’écrit, en vertu de la formule (47) du § 1, n° 10, $R = {}^tW.S$; en explicitant ceci montre que l’on a $W = \begin{pmatrix} 0 & \alpha_2 \\ -\alpha_1 & 0 \end{pmatrix}$. Si $\begin{pmatrix} a & c \\ b & d \end{pmatrix}$ désigne la matrice de $u$ par rapport à $(e_1, e_2)$, la relation $u\omega = \omega u$ équivaut donc aux relations $b\alpha_2 = -c\alpha_1, a\alpha_2 = d\alpha_2, a\alpha_1 = d\alpha_1$, c’est-à-dire à $a = d$ et $c = \delta b$; ceci démontre que les matrices des similitudes directes sont les matrices inversibles de la forme $\begin{pmatrix} a & \delta b \\ b & a \end{pmatrix}$ ($a, b$ dans A).

Or les endomorphismes de E dont les matrices sont de la forme $\begin{pmatrix} a & \delta b \\ b & a \end{pmatrix}$ ($a, b$ dans A) forment un sous-espace vectoriel de dimension 2 de $\mathfrak{L}_A(E)$, engendré par 1 et par l’endomorphisme $\omega$; comme $\omega^2$ est l’homothétie de rapport $-\alpha_1\alpha_2$, ce sous-espace est la sous-algèbre $A(\Phi)$ de $\mathfrak{L}_A(E)$ engendrée par les similitudes directes. Les similitudes directes sont les éléments inversibles de $A(\Phi)$, c’est-à-dire ceux dont les matrices vérifient $a^2 - \delta b^2 \neq 0$. Le fait que l’algèbre $A(\Phi)$ est commutative est évident. Appliquons-lui les résultats du chap. II, § 7, n° 7 : si $\delta$ n’est pas un carré dans A, c’est-à-dire si aucun vecteur non nul de E n’est isotrope, $A(\Phi)$ est un corps ; si, au contraire, $\delta$ est un carré dans A, c’est-à-dire si E contient des vecteurs isotropes $\neq 0$, $A(\Phi)$ est composée directe de deux corps isomorphes à A. Ceci démontre a) et b).

Enfin tout vecteur non isotrope de E peut être pris comme premier vecteur $e_1$ d’une base orthogonale $(e_1, e_2)$ (\S 6, n° 1); donc ses transformés $u(e_1)$ par les éléments $u$ de $\Lambda(\Phi)$ sont les vecteurs de la forme $ae_1 + be_2$ ($a, b$ dans $\Lambda$), c’est-à-dire tous les vecteurs de $E$, puisque toutes les matrices $\begin{pmatrix} a & \delta b \\ b & a \end{pmatrix}$ sont des matrices d’éléments de $\Lambda(\Phi)$. Autrement dit $E$ est un $\Lambda(\Phi)$-module monogène, engendré par n’importe quel vecteur non isotrope. On voit de plus que c’est un $\Lambda(\Phi)$-module monogène libre, puisque $u(e_1) = ae_1 + be_2 = 0$ entraîne $a = b = 0$, donc $u = 0$. Ceci démontre c).

#### Remarque 1 {#alg-ix-s10-n1-rem-1 .statement}

Soit $\nu$ la similitude de matrice $\begin{pmatrix} 0 & \delta \\ 1 & 0 \end{pmatrix}$ par rapport à $(e_1, e_2)$; la similitude $\omega$ introduite dans la démonstration de la prop. 1 est égale à $-\alpha_1 \nu$; on a $\nu^2 = \delta$. Le multiplicateur de la similitude directe $u = a + b \nu$ ($a, b$ dans $\Lambda$) est égal au déterminant de sa matrice $\begin{pmatrix} a & \delta b \\ b & a \end{pmatrix}$, c’est-à-dire à $a^2 - \delta b^2 = (a + b \nu)(a - b \nu) = u . \overline{u}$, en désignant par $\overline{u}$ le conjugué de $u$ dans l’algèbre $\Lambda(\Phi)$ (chap. II, § 7, n° 7); autrement dit le multiplicateur de $u$ est la norme $N(u)$ de $u$ dans l’algèbre $\Lambda(\Phi)$ (ibid.). En particulier, pour qu’une similitude directe $u$ soit une rotation, il faut et il suffit que $N(u) = 1$; pour que $u$ soit une homothétie, il faut et il suffit que $u \in \Lambda^*$.

#### Remarque 2 {#alg-ix-s10-n1-rem-2 .statement}

Les similitudes directes $u = a + b \nu$ ($a, b$ dans $\Lambda$, $b \neq 0$) dont le carré est une homothétie sont les homothéties et les multiples scalaires $b \nu$ de $\nu$, puisque $(a + b \nu)^2 = (a^2 + \delta b^2) + 2ab \nu$. Ces derniers ne sont autres que les automorphismes de l’espace vectoriel $E$ qui *transforment tout vecteur en un vecteur orthogonal*; en effet la matrice d’un tel automorphisme est nécessairement de la forme $\begin{pmatrix} 0 & c \\ d & 0 \end{pmatrix}$ ($c, d$ dans $\Lambda$), et la condition de transformer le vecteur $\lambda e_1 + \mu e_2$ en un vecteur orthogonal s’écrit alors $\lambda \mu (d \alpha_2 + c \alpha_1) = 0$.

#### Remarque 3 {#alg-ix-s10-n1-rem-3 .statement}

On vérifie aisément que, pour $x, y$ dans $E$ et $u \in \Lambda(\Phi)$, on a $\Phi(u(x), y) = \Phi(x, \overline{u}(y))$. Ainsi l’endomorphisme *adjoint* d’une similitude directe $u$ est la similitude directe $\overline{u}$ *conjuguée* de $u$ dans $\Lambda(\Phi)$.

#### Remarque 4 {#alg-ix-s10-n1-rem-4 .statement}

Comme toute *similitude inverse* de $E$ est le produit d’une similitude directe et de la symétrie par rapport à $Ae_1$, les matrices n° 1

des similitudes inverses par rapport à $(e_1, e_2)$ sont les matrices de la forme $\begin{pmatrix} a & -\delta b \\ b & -a \end{pmatrix}$.

Nous désignerons désormais par $S$ le groupe des similitudes de $E$, par $S^+$ celui des similitudes directes, par $H$ celui des homothéties $\neq 0$, et par $O^+$ celui des rotations. Rappelons que l’on a $H \subset S^+ (\S 6, n° 5)$.

#### Corollaire 1 {#alg-ix-s10-prop-1-cor-1 .statement}

*Le groupe $S^+$ des similitudes directes est commutatif. Quels que soient les vecteurs non isotropes $x, y$ de $E$, il existe une similitude directe $u$ et une seule telle que $y = u(x)$.*

La première assertion résulte du fait que l’algèbre $A(\Phi)$ est commutative. Comme $E$ est un $A(\Phi)$-module libre monogène engendré par $x$ (resp. $y$), il existe un élément $u$ (resp. $u'$) de $A(\Phi)$ et un seul tel que $y = u(x)$ (resp. $x = u'(y)$) ; d’où $x = u(u'(x))$, et $uu'$ est l’identité ; ceci montre que $u$ est inversible, et est donc une similitude directe.

#### Corollaire 2 {#alg-ix-s10-prop-1-cor-2 .statement}

*Le groupe $O^+$ des rotations est commutatif. Quels que soient les vecteurs $x, y$ de $E$ tels que $\Phi(x, x) = \Phi(y, y) \neq 0$, il existe une rotation $u$ et une seule telle que $y = u(x)$.*

La première assertion résulte du cor. 1. Celui-ci montre aussi qu’il existe une similitude directe $u$ et une seule telle que $y = u(x)$ ; comme $\Phi(u(x), u(x)) = \Phi(x, x)$, le multiplicateur de $u$ est égal à 1, et $u$ est donc une rotation.

#### Corollaire 3 {#alg-ix-s10-prop-1-cor-3 .statement}

*Le groupe $S^+/H$ est commutatif. Il opère sur l’ensemble des droites non isotropes de $E$. Quelles que soient les droites non isotropes $D, D'$ de $E$, il existe un élément $\varphi$ et un seul de $S^+/H$ tel que $D' = \varphi(D)$.*

Ceci résulte du cor. 1 et du fait que $H$ laisse globalement invariante toute droite de $E$.

#### Proposition 2 {#alg-ix-s10-prop-2 .statement}

*Le noyau de l’homomorphisme canonique de $O^+$ dans $S^+/H$ est $\{1, -1\}$.*

En effet 1 et $-1$ sont les seuls éléments de $H \cap O^+$.

#### Proposition 3 {#alg-ix-s10-prop-3 .statement}

L’homomorphisme $u \to u/\overline{u} = u^2 / N(u)$ de $S^+$ dans lui-même admet $H$ pour noyau, et définit, par passage au quotient, un isomorphisme de $S^+/H$ sur $O^+$.

En effet la relation $u/\overline{u} = 1$ équivaut à $u = \overline{u}$, c’est-à-dire à $u \in A^* = H$; donc $H$ est le noyau de $u \to u/\overline{u}$. Comme $N(u/\overline{u}) = 1$, $u/\overline{u}$ est une rotation (Remarque 1). Il reste à montrer que tout élément $\varphi$ de $O^+$ est de la forme $u/\overline{u}$ ($u \in S^+$). Si $1 + \varphi$ est inversible, on peut prendre $u = 1 + \varphi$, car la relation $N(\varphi) = \varphi \overline{\varphi} = 1$ implique $1 + \varphi = \varphi(1 + \overline{\varphi})$. Sinon, l’on a $N(1 + \varphi) = (1 + \varphi)(1 + \overline{\varphi}) = 0$, c’est-à-dire, en posant $\varphi = a + b\omega$ ($a \in A,\ b \in A,\ \omega^2 = \delta \in A$), $2(1 + a) = 0$, d’où $a = -1$; or les relations $a = -1$ et $N(\varphi) = a^2 - \delta b^2 = 1$ entraînent $b = 0$, d’où $\varphi = -1$; comme $\overline{\omega} = -\omega$, il suffit, dans ce cas, de prendre $u = \omega$.

Lorsque $A(\Phi)$ est un corps, la prop. 3 est un cas particulier du théorème de Hilbert (chap. V, § 11, n° 5, th. 3).

#### Corollaire {#alg-ix-s10-n1-cor-1 .statement}

Notons $i : O^+ \to S^+/H$ et $d : S^+/H \to O^+$ les homomorphismes définis dans les prop. 2 et 3, et écrivons additive-
ment les groupes abéliens $O^+$ et $S^+/H$; on a $d(i(\theta)) = 2\theta$ pour $\theta \in O^+$
et $i(d(\varphi)) = 2\varphi$ pour $\varphi \in S^+/H$.

En effet, si $\overline{\varphi}$ est une rotation, on a $\overline{\varphi} = \varphi^{-1}$, d’où $d(i(\varphi)) = \varphi/\overline{\varphi} = \varphi^2$. D’autre part, si $\varphi \in S^+/H$, $\varphi$ est la classe mod. $H$ d’une similitude directe $u$, et $d(\varphi) = u/\overline{u} = u^2 / N(u)$ est congru à $u^2$ mod. $H$; d’où la seconde formule.

### 2. Trigonométrie plane.

Nous ferons choix, dans ce n°, d’un générateur $\omega$ de l’algèbre $A(\Phi)$ tel que $\omega^2 \in A$. Un tel générateur est déterminé à une homothétie près (n° 1, Remarque 2), donc l’élément $\omega^2$ de $A$, que nous noterons $\delta$, est déterminé modulo le sous-groupe multiplicatif $(A^*)^2$ des carrés d’éléments non nuls de $A$.

#### Remarque {#alg-ix-s10-n2-rem-1 .statement}

Lorsque –1 appartient à la classe mod. $(A^*)^2$ en question, on choisit en général $\omega$ de telle sorte que $\omega^2 = -1$, ce qui le détermine au signe près. Lorsque cette classe contient 1 mais non –1, on choisit en général $\omega$ de telle sorte que $\omega^2 = 1$, ce qui le détermine encore au signe près.

n° 2

ANGLES

Ceci étant, tout élément $\varphi$ de $S^+$ s’écrit, d’une façon et d’une seule, sous la forme

(1)
$$
\varphi = c_w(\varphi) + s_w(\varphi)\omega
$$
où $c_w(\varphi), s_w(\varphi)$ appartiennent à $A$; l’élément $s_w(\varphi)/c_w(\varphi)$ du corps projectif $\tilde{A}$ (chap. II, 2e éd., App. III, n° 5) est noté $t_w(\varphi)$; il ne dépend que de la classe de $\varphi$ mod. $H$; ainsi $t_w$ définit, par passage au quotient, une application de $S^+/H$ dans le corps projectif $\tilde{A}$, que nous noterons encore $t_w$ par abus de langage. Nous écrirons souvent $c, s$ et $t$ au lieu de $c_w, s_w$ et $t_w$. On a $c_{-w} = c_w, s_{-w} = -s_w$ et $t_{-w} = -t_w$.

#### Proposition 4 {#alg-ix-s10-prop-4 .statement}

a) Lorsque $\omega^2 = \delta$ n’est pas un carré dans $A$ (c’est-à-dire lorsque $E$ ne contient pas de droite isotrope), l’application $t$ de $S^+/H$ dans $\tilde{A}$ est une bijection.

b) Lorsque $\delta$ est le carré d’un élément $\gamma$ de $A$, l’application $t$ est une bijection de $S^+/H$ sur $\tilde{A}$ privé des éléments $1/\gamma$ et $-1/\gamma$.

c) En notant $S^+/H$ additivement, on a, pour $\varphi, \varphi'$ dans $S^+/H$

(2)
$$
t(\varphi + \varphi') = (t(\varphi) + t(\varphi'))/(1 + \delta t(\varphi)t(\varphi'))
$$
lorsque $t(\varphi)$ et $t(\varphi')$ sont finis et que $1 + t(\varphi)t(\varphi')$ est $\neq 0$.

En effet, comme $S^+/H$ est un ensemble de droites (privées de 0) de $A(\Phi)$ considéré comme plan vectoriel sur $A$, $t$ est injective. D’autre part, pour qu’un élément $a + b\omega$ ($a \in A, b \in A$) de $A(\Phi)$ soit une similitude directe, il faut et il suffit qu’il soit inversible, c’est-à-dire que l’on ait $N(a + b\omega) = a^2 - \delta b^2 \neq 0$, ou encore $(b/a)^2 \neq 1/\delta$; ceci démontre les assertions de surjectivité dans a) et b). Enfin le produit des similitudes $1 + t(\varphi)\omega$ et $1 + t(\varphi')\omega$ est la similitude $1 + \delta t(\varphi)t(\varphi') + (t(\varphi) + t(\varphi'))\omega$, ce qui démontre c).

#### Proposition 5 {#alg-ix-s10-prop-5 .statement}

Notons $O^+$ additivement. Pour tout couple d’éléments $\theta, \theta'$ de $O^+$ on a

(3)
$$
c(\theta)^2 - \delta s(\theta)^2 = 1
$$
(4)
$$
c(\theta + \theta') = c(\theta)c(\theta') + \delta s(\theta)s(\theta')
$$
(5)
$$
s(\theta + \theta') = s(\theta)c(\theta') + c(\theta)s(\theta').
$$

La relation (3) exprime en effet que $N(c(\theta) + s(\theta)\omega) = 1$. Pour (4) et (5) il suffit de calculer, dans $A(\Phi)$, le produit des rotations $c(\theta) + s(\theta)\omega$ et $c(\theta') + s(\theta')\omega$.

#### Proposition 6 {#alg-ix-s10-prop-6 .statement}

*Soit d l’isomorphisme de $S^+/H$ sur $O^+$ défini dans la prop. 3. Pour tout élément $\varphi$ de $S^+/H$ tel que $t = t(\varphi)$ soit fini, on a*

(6)
$$
s(d(\varphi)) = 2t/(1 - \delta t^2), \qquad c(d(\varphi)) = (1 + \delta t^2)/(1 - \delta t^2).
$$

En effet $\varphi$ est la classe mod. $H$ de la similitude $1 + t\omega$, et la rotation $d(\varphi)$ est donc $(1 + t\omega)^2/N(1 + t\omega) = (1 + \delta t^2 + 2t\omega)/(1 - \delta t^2)$ (prop. 3), ce qui démontre (6).

#### Corollaire {#alg-ix-s10-n2-cor-1 .statement}

*Pour tout élément $\theta$ de $O^+$ tel que $t(\theta)$ soit fini, on a*

(7)
$$
s(2\theta) = 2t(\theta)/(1 - \delta t(\theta)^2), \qquad c(2\theta) = (1 + \delta t(\theta)^2)/(1 - \delta t(\theta)^2).
$$
*Pour tout élément $\varphi$ de $S^+/H$ tel que $t(\varphi)$ soit fini et $1 + \delta t(\varphi)^2 \neq 0$, on a*
(8)
$$
t(2\varphi) = 2t(\varphi)/(1 + \delta t(\varphi)^2).
$$

En effet ceci résulte aussitôt de la prop. 6 et du cor. de la prop. 3.

#### Remarque {#alg-ix-s10-n2-rem-2 .statement}

Les formules (6) restent vraies pour $t = \infty$ à condition de remplacer les fonctions rationnelles qui figurent au second membre par leurs prolongements canoniques au corps projectif $\tilde{A}$ (chap. II, 2e éd., App. III, n° 5); en effet, si $t = \infty$, $\varphi$ est la classe de $\omega$, et on a $d(\varphi) = -1, s(d(\varphi)) = 0$ et $c(d(\varphi)) = -1$; ce sont bien là les valeurs prises par les prolongements canoniques des seconds membres pour $t = \infty$. Il en est de même pour (7) lorsque $t(\theta) = \infty$, et pour (8) lorsque $t(\varphi) = \infty$ ou que $1 + \delta t(\varphi)^2 = 0$. De même la formule (2) reste vraie lorsqu’un seul des éléments $t(\varphi), t(\varphi'), t(\varphi)$ par exemple, est infini, à condition de considérer son second membre comme une fonction rationnelle de $t(\varphi)$ seulement : en effet le produit des similitudes $1 + t(\varphi')\omega$ et $\omega$ est $\delta t(\varphi') + \omega$, tandis que la valeur prise par le prolongement canonique du second membre de (2) est $1/\delta t(\varphi')$. Enfin, lorsque $t(\varphi)$ et $t(\varphi')$ sont finis et que l’on a $1 + \delta t(\varphi)t(\varphi') = 0$, on a $t(\varphi) + t(\varphi') = 0$ (sinon $t(\varphi)^2$ serait égal à $1/\delta$, ce qui est impossible (prop. 4)); on peut donc convenir que la valeur du second membre de (2) est $\infty$, et cette valeur est bien celle du premier membre. Lorsque $t(\varphi)$ et $t(\varphi')$ sont tous deux infinis, le second membre de (2) n’est pas défini.

### 3. Angles.

Nous supposerons, dans ce n° et le suivant, que A est un corps ordonné, donc de caractéristique nulle. Rappelons (Rectifications au chap. VI) que, si F est un espace vectoriel sur A, la relation « il existe $\lambda > 0$ tel que $y = \lambda x$ » est une relation d’équivalence entre éléments $x, y$ de $F - \{ 0 \}$, que toute classe d’équivalence pour cette relation s’appelle une demi-droite ouverte d’origine 0, et que la réunion d’une demi-droite ouverte et de $\{ 0 \}$ s’appelle une demi-droite fermée (ou simplement demi-droite) d’origine 0 ; si D est une droite et $\Delta$ une demi-droite fermée contenue dans D, D est réunion de $\Delta$ et de $-\Delta$, et ne contient pas d’autre demi-droite fermée. Nous dirons qu’une demi-droite est isotrope si la droite qui la contient est isotrope.

Rappelons aussi (ibid.) que, étant donné un espace vectoriel de dimension finie $n$ sur A, une orientation sur F est la donnée d’une des deux demi-droites de l’espace $\wedge^n F$; les $n$-vecteurs appartenant à cette demi-droite sont dits positifs. Un espace vectoriel de dimension finie muni d’une orientation est dit orienté.

Les homothéties de E dont le rapport est $> 0$ forment évidemment un sous-groupe d’indice 2 de H ; nous le noterons $H^+$. L’homomorphisme canonique $i : O^+ \to S^+/H$ (cf. prop. 2) est le composé des homomorphismes canoniques de $S^+/H^+$ sur $S^+/H$ et de $O^+$ dans $S^+/H^+$; comme $O^+ \cap H^+ = \{ 1 \}$, ce dernier homomorphisme est injectif.

#### Proposition 7 {#alg-ix-s10-prop-7 .statement}

Supposons que A soit un corps ordonné maximal et que $\Phi$ soit une forme positive (\S 7). Alors les homomorphismes canoniques de $O^+$ dans $S^+/H^+$ et de $O^+/\{ 1, -1 \}$ dans $S^+/H$ sont bijectifs, et $S^+$ est isomorphe à $O^+ \times H^+$.

Nous avons déjà vu que les homomorphismes en question sont injectifs, et il suffit de montrer que le premier est surjectif. Soit $(e_1, e_2)$ une base orthonormale de E, et soit $\omega$ la similitude directe telle que $\omega(e_1) = e_2$ (cor. 1 de la prop. 1, n° 1) ; on a alors $\omega^2 = -1$ (prop. 1, b)). Étant donnée une similitude directe quelconque u = a + bw (a \in A,\ b \in A),\ \text{on a}\ N(u) = a^2 + b^2 > 0,\ \text{et il existe une rotation et une seule contenue dans la même demi-droite de } A(\Phi) \text{ que } u, \text{ à savoir } (a^2 + b^2)^{1/2}\ u.\ \text{CQFD.}

#### Corollaire {#alg-ix-s10-n3-cor-1 .statement}

*Etant données deux demi-droites* D, D' *d’origine* 0, *il existe une rotation* v *et une seule telle que* v(D) = D'.

Les hypothèses impliquent en effet que E ne contient point de droites isotropes. Notre assertion résulte alors du cor. 1 de la prop. 1 (n° 1).

Nous supposerons désormais que A est un *corps ordonné maximal*, et que la forme $\Phi$ est *positive*. Dans l’ensemble des couples $(D_1, D_2)$ de droites (resp. demi-droites d’origine 0) de E, la relation « il existe une similitude directe (resp. une rotation) u telle que $u(D_1) = D'_1$ et $u(D_2) = D'_2$ » est une relation d’équivalence entre les couples $(D_1, D_2)$ et $(D'_1, D'_2)$. La classe d’équivalence du couple $(D_1, D_2)$ s’appelle, par définition *l’angle des droites* (resp. *demi-droites*) $D_1, D_2$ (prises dans cet ordre); on le note $(\widehat{D_1, D_2})$.

#### Proposition 8 {#alg-ix-s10-prop-8 .statement}

*On suppose que* A *est un corps ordonné maximal*, et que la *forme* $\Phi$ *est positive*. *Soient* $D_1, D_2, D'_1, D'_2$ *quatre droites* (resp. *demi-droites*) *d’origine* 0 *de* E. *Pour que les angles* $(\widehat{D_1, D_2})$ *et* $(\widehat{D'_1, D'_2})$ *soient égaux, il faut et il suffit que les angles* $(\widehat{D_1, D'_1})$ *et* $(\widehat{D_2, D'_2})$ *soient égaux*.

Démontrons la nécessité de la condition énoncée. Soit u une similitude directe (resp. une rotation) telle que $u(D_1) = D'_1$ et $u(D_2) = D'_2$. Il existe, d’après le cor. 3 de la prop. 1, une similitude directe (resp. d’après le cor. de la prop. 7, une rotation) v telle que $v(D_1) = D_2$. Comme le groupe $S^+$ (resp. $O^+$) est *commutatif*, on a $D'_2 = u(v(D_1)) = v(u(D_1)) = v(D'_1)$, et ceci montre que $(\widehat{D_1, D'_1}) = (\widehat{D_2, D'_2})$. La suffisance se déduit de la nécessité en échangeant $D_2$ et $D'_1$.

Il résulte de la prop. 8 que, à tout angle $(\widehat{D_1, D_2})$ de droites (resp. demi-droites) d’origine 0 de E, est canoniquement associé un élément bien déterminé de $S^+/H$ (resp. $O^+$), à savoir la classe mod. H des similitudes directes $\varphi$ (resp. la rotation $\varphi$) telles que $u(D_1) = D_2$ pour n’importe quel représentant $(D_1, D_2)$ de l’angle $(\widehat{D_1, D_2})$. On a ainsi défini une bijection canonique $h$ (resp. $h'$) de l’ensemble $\mathfrak{A}_0$ des angles de droites (resp. $\mathfrak{A}$ des angles de demi-droites) sur $S^+/H$ (resp. $O^+$) ; en particulier, pour tout $\varphi \in \mathfrak{A}$, on dit que $h(\varphi)$ est la rotation d’angle $\varphi$. Nous transporterons à $\mathfrak{A}_0$ et $\mathfrak{A}$, au moyen de $h^{-1}$ et de $h'^{-1}$, les structures de groupes commutatifs de $S^+/H$ et de $O^+$, et nous noterons additivement les groupes $\mathfrak{A}_0$ et $\mathfrak{A}$ ainsi obtenus. Si l’on désigne par $D, D', D''$ des droites (resp. demi-droites) d’origine 0 de E, on a par définition

$$
(9) \quad (\widehat{D, D''}) = (\widehat{D, D'}) + (\widehat{D', D''}) \tag{relation de Chasles};
$$

on en déduit

$$
(10) \quad (\widehat{D, D}) = 0, \qquad (\widehat{D, D'}) = - (\widehat{D', D}).
$$

#### Remarque 1 {#alg-ix-s10-n3-rem-1 .statement}

L’ensemble L des droites (resp. demi-droites) d’origine 0 de E est un espace homogène du groupe abélien $S^+/H$ (resp. $O^+$) tel que l’élément neutre soit le seul opérateur laissant invariants tous les éléments de L. On peut donc appliquer à L les formules du chap. II, 2e éd., App. II, no 1 ; la prop. 8 est ainsi un cas particulier de la « règle du parallélogramme », et les formules (9) et (10) des cas particuliers des formules (2) (ibid.).

#### Remarque 2 {#alg-ix-s10-n3-rem-2 .statement}

Dans la définition du groupe des angles de droites, on peut, au lieu du groupe $S^+/H$, utiliser le groupe $O^+/ \{ -1, 1 \}$ qui lui est canoniquement isomorphe (prop. 7). L’homomorphisme canonique de $O^+$ sur $O^+/ \{ -1, 1 \}$ correspond ainsi à un homomorphisme de $\mathfrak{A}$ sur $\mathfrak{A}_0$, à savoir celui qui, à l’angle des deux demi-droites $\Delta, \Delta'$, fait correspondre l’angle des droites $D, D'$ contenant respectivement $\Delta, \Delta'$. *Dans le cas où le corps A est le corps des nombres réels, le groupe $\mathfrak{A}$ est ainsi un revêtement d’ordre 2 du groupe $\mathfrak{A}_0$*

D’après la prop. 8, tous les angles de droites (resp. demi-droites) de la forme $(\widehat{D', D''})$ où $D'$ et $D''$ sont orthogonales (resp.

de la forme ($\widehat{D, - D}$) sont égaux : ceci résulte en effet de la Remarque 2 du no 1 (resp. est évident). Cet angle de droites (resp. de demi-droites) s’appelle l’angle droit (resp. l’angle plat) ; c’est un élément d’ordre 2 de $\mathfrak{A}_0$ (resp. de $\mathfrak{A}$).

#### Proposition 9 {#alg-ix-s10-prop-9 .statement}

On suppose que le corps $\mathbf{A}$ est ordonné maximal, et que $\Phi$ est une forme positive. Pour tout entier $n > 1$, le nombre des éléments $\theta$ du groupe $\mathfrak{A}_0$ des angles de droites (resp. $\mathfrak{A}$ des angles de demi-droites) tels que $n\theta = 0$ est égal à $n$.

Comme $\mathfrak{A}_0, S^+/H, \mathfrak{A}$ et $O^+$ sont isomorphes (prop. 3), il suffit de faire la démonstration pour $O^+$, c’est-à-dire montrer qu’il y a exactement $n$ rotations $\varphi$ telles que $\varphi^n = 1$. Or, comme $\mathbf{A}$ est un corps ordonné maximal et que $\mathbf{A}(\Phi)$ est un surcorps de degré 2 de $\mathbf{A}$ (prop. 1 a)), $\mathbf{A}(\Phi)$ est un corps algébriquement clos (chap. VI, § 2, no 6, th. 3). Donc les racines $n$-ièmes de l’unité dans $\mathbf{A}(\Phi)$ forment un groupe cyclique d’ordre $n$ (chap. V, § 11, no 1, th. 1). Comme on a $N(u) = u \overline{u} \geqslant 0$ pour tout $u \in \mathbf{A}(\Phi)$, la relation $u^n = 1$ entraîne que l’on a $N(u) = 1$, donc que $u$ est une rotation (no 1, Remarque 1). Ceci démontre notre assertion.

#### Corollaire {#alg-ix-s10-n3-cor-2 .statement}

L’angle droit (resp. plat) est le seul élément d’ordre 2 du groupe $\mathfrak{A}_0$ (resp. $\mathfrak{A}$).

Nous supposerons enfin que le plan $E$ est orienté.

#### Lemme 1 {#alg-ix-s10-lem-1 .statement}

Soit $u$ une similitude directe de $E$; tous les bivecteurs de la forme $x \wedge u(x)$ appartiennent à la même demi-droite fermée de $\overset{2}{\wedge} E$.

Le cas où $u$ est une homothétie est trivial. Dans le cas contraire on a $x \wedge u(x) \neq 0$ pour tout $x \neq 0$; soient $x, y$ deux vecteurs de $E$ ($x \neq 0, y \neq 0$); il existe $\varphi \in S^+$ tel que $y = \varphi(x)$, d’où $y \wedge u(y) = \varphi(x) \wedge u \varphi(x) = \varphi(x) \wedge \varphi(u(x)) = (\det \varphi)(x \wedge u(x))$; en prenant une base orthonormale de $E$, on voit que $\det \varphi$ est positif (prop. 1 b)); d’où notre assertion.

Ceci étant, parmi les deux générateurs $\omega$ de $\mathbf{A}(\Phi)$ tels que $\omega^2 = -1$, il en existe un et un seul tel que le bivecteur $x \wedge \omega(x)$ soit positif pour tout $x \in E$. C’est ce générateur que nous choisirons pour définir les fonctions $c_w, s_w$ et $t_w$ (no 2). Soient $h$ et $h'$ les bijections canoniques ci-dessus définies du groupe $\mathfrak{A}_0$ des angles de droites sur $S^+/H$ et du groupe $\mathfrak{A}$ des angles de demi-droites sur $O^+$. Les applications composées $t_w \circ h$ de $\mathfrak{A}_0$ dans le corps projectif $\tilde{\mathfrak{A}}$, $c_w \circ h'$ et $s_w \circ h'$ de $\mathfrak{A}$ dans le corps $A$ se notent respectivement $\operatorname{tg}$, $\cos$ et $\sin$, et s’appellent les *fonctions tangente*, *cosinus* et *sinus*. L’application $\varphi \to 1/\operatorname{tg} \varphi$ de $\mathfrak{A}_0$ dans $\tilde{\mathfrak{A}}$ se note $\operatorname{cotg}$ et s’appelle la *fonction cotangente*. On dit que les fonctions sinus, tangente et cotangente sont les *fonctions trigonométriques*. Les applications composées $\operatorname{tg} \circ p$ et $\operatorname{cotg} \circ p$, où $p$ désigne l’homomorphisme canonique de $\mathfrak{A}$ sur $\mathfrak{A}_0$ (Remarque 2 ci-dessus) se notent encore $\operatorname{tg}$ et $\operatorname{cotg}$ par abus de langage.

Les formules (2), (8), (3), (4), (5) et (7) du no 2 donnent, puisqu’on a ici $\delta = -1$

$$
\begin{align*}
(11) \quad & \operatorname{tg} (\varphi + \varphi') = (\operatorname{tg} \varphi + \operatorname{tg} \varphi')/(1 - \operatorname{tg} \varphi \operatorname{tg} \varphi') \\
(12) \quad & \operatorname{tg} (2\varphi) = 2 \operatorname{tg} \varphi/(1 - \operatorname{tg}^2 \varphi)
\end{align*}
$$

pour $\varphi, \varphi'$ dans $\mathfrak{A}_0$;

$$
\begin{align*}
(13) \quad & \cos^2 \theta + \sin^2 \theta = 1 \\
(14) \quad & \cos (\theta + \theta') = \cos \theta \cos \theta' - \sin \theta \sin \theta' \\
(15) \quad & \sin (\theta + \theta') = \sin \theta \cos \theta' + \cos \theta \sin \theta' \\
(16) \quad & \left\{ \begin{array}{l}
\sin (2\theta) = 2 \operatorname{tg} \theta/(1 + \operatorname{tg}^2 \theta), \\
\cos (2\theta) = (1 - \operatorname{tg}^2 \theta)/(1 + \operatorname{tg}^2 \theta)
\end{array} \right.
\end{align*}
$$

pour $\theta, \theta'$ dans $\mathfrak{A}$. D’autre part on a, par définition ou comme conséquence facile des formules précédentes :

$$
\begin{align*}
(17) \quad & \operatorname{tg} \theta = \sin \theta/\cos \theta, \qquad \operatorname{cotg} \theta = \cos \theta/\sin \theta \\
(18) \quad & 1 + \operatorname{tg}^2 \theta = 1/\cos^2 \theta, \qquad 1 + \operatorname{cotg}^2 \theta = 1/\sin^2 \theta
\end{align*}
$$

pour $\theta \in \mathfrak{A}$.

Étant donnés deux vecteurs non nuls $x, y$ de $E$, on appelle *angle* de ces deux vecteurs (pris dans cet ordre), et on note $\widehat{(x, y)}$, l’angle des demi-droites auxquelles ils appartiennent. Pour tout vecteur $x$ de $E$ on appelle *longueur* de $x$, et on note $|x|$, l’élément $\Phi(x, x)^{1/2}$ de $A$.

#### Proposition 10 {#alg-ix-s10-prop-10 .statement}

On suppose que le corps $\mathbf{A}$ est ordonné maximal, que le plan $\mathbf{E}$ est orienté, et que la forme $\Phi$ est positive. Pour tout couple de vecteurs non nuls $x, y$ de $\mathbf{E}$ on a

$$
\cos (\widehat{x, y}) = \Phi(x, y)/|x|.|y|
$$
$$
\sin (\widehat{x, y}).e = (x \wedge y)/|x|.|y|,
$$

où $e$ désigne le bivecteur positif tel que $\Phi_{(2)}(e, e) = 1$.

En effet, comme les vecteurs $x' = x/|x|$ et $y' = y/|y|$ sont tous deux de longueur 1, il existe une rotation $\varphi$ et une seule telle que $\varphi(x') = y'$ (n° 1, cor. 2 de la prop. 1). Si l’on pose $\varphi = a + b \omega$ ($a, b$ dans $\mathbf{A}$), on a par définition $a = \cos (\widehat{x, y})$ et $b = \sin (\widehat{x, y})$. La relation $y' = \varphi(x') = ax' + b \omega(x')$ donne $\Phi(x', y') = a \Phi(x', x') = a$ puisque $x'$ et $\omega(x')$ sont orthogonaux (Remarque 2 du n° 1); ceci démontre (19). D’autre part cette relation donne aussi $x' \wedge y' = bx' \wedge \omega(x') = b.e$ d’après la définition de l’extension $\Phi_{(2)}$ de $\Phi$ à $\bigwedge^2 \mathbf{E}$ ($\S 1,$ n° 9, formule (37)) et le choix de $\omega$; ceci démontre (20).

#### Remarque 3 {#alg-ix-s10-n3-rem-3 .statement}

Étant données deux droites (resp. demi-droites) $D, D'$ d’un *plan affine* $L$ attaché à $E$, on appelle angle de $D$ et $D'$, et on note $(\widehat{D, D'})$, l’angle que font leurs directions dans $E$ (resp. les demi-droites d’origine 0 de $E$ correspondant à $D$ et $D'$) (chap. II, 2e éd., App. II, n° 1 et n° 3).

#### Remarque 4 {#alg-ix-s10-n3-rem-4 .statement}

Soient $F$ un espace vectoriel *de dimension quelconque* sur le corps ordonné maximal $\mathbf{A}$, et $\Psi$ une forme bilinéaire symétrique positive non dégénérée sur $F$. Étant donnés deux vecteurs $x, y$ linéairement indépendants de $F$, soit $F'$ le plan vectoriel qu’ils engendrent ; on appelle *angle* de $x$ et $y$ l’angle de $x$ et $y$ considérés comme éléments du plan $F'$; on le note $(\widehat{x, y})$. Le cosinus de cet angle est, en vertu de (19), donné par

$$
\cos (\widehat{x, y}) = \Psi(x, y)/|x|.|y|
$$

(où $|x| = \Psi(x, x)^{1/2}$ est encore appelé la *longueur* du vecteur $x$), et est donc *indépendant de l’orientation choisie* sur $F'$; le sinus et la tangente de $(\widehat{x, y})$ changent de signe si l’on change l’orientation de $F'$. Étant donnés deux vecteurs non nuls et proportionnels $x, y$ de $F$, on pose $(\widehat{x, y}) = 0$ par convention.

### 4. Secteurs angulaires.

Nous supposerons d’abord, sans autre hypothèse, que E est un plan orienté sur le corps ordonné A. On dira que trois demi-droites D₀, D₁, D₂ (d’origine 0) de E forment une suite directe si, pour xᵢ ∈ Dᵢ, xᵢ ≠ 0 (i = 0, 1, 2), deux au moins des bivecteurs x₀ ∧ x₁, x₁ ∧ x₂, x₂ ∧ x₀ sont > 0 ; dans ce cas les suites D₁, D₂, D₀ et D₂, D₀, D₁ sont aussi directes. Il est clair que trois demi-droites formant une suite directe sont distinctes. Étant données deux demi-droites D₁, D₂ de E, on appelle secteur angulaire ouvert (resp. fermé) d’origine D₁ et d’extrémité D₂, l’ensemble (ou, par abus de langage, la réunion) des demi-droites D telles que la suite D₁, D, D₂ soit directe (resp. telles que D = D₁ ou D = D₂ ou que la suite D₁, D, D₂ soit directe).

#### Proposition 11 {#alg-ix-s10-prop-11 .statement}

Soient E un plan orienté sur un corps ordonné A, D₀ une demi-droite de E, et G l’ensemble des demi-droites de E distinctes de D₀. La relation

« D₁ = D₂, ou la suite D₀, D₁, D₂ est directe »

entre éléments D₁, D₂ de G est une relation d’ordre total dans G.

En effet les axiomes des relations d’ordre total se vérifient trivialement, à l’exception de la transitivité. Soient D₁, D₂, D₃ trois demi-droites telles que les suites, D₀, D₁, D₂ et D₀, D₂, D₃ soient directes ; nous allons montrer que la suite D₀, D₁, D₃ est directe. Pour cela prenons un vecteur xᵢ ≠ 0 dans Dᵢ (i = 0, 1, 2, 3), choisissons un bivecteur e > 0 et posons xᵢ ∧ xⱼ = aᵢⱼe (aᵢⱼ ∈ A). En écrivant e = x₀ ∧ y (y ∈ E), et en prenant (x₀, y) pour base de E, on vérifie aisément la relation

$$
a_{01}a_{23} + a_{02}a_{31} + a_{03}a_{12} = 0.
$$

Ceci étant, si a₀₁ ≤ 0, on a a₁₂ > 0 et a₂₀ > 0 (puisque la première suite est directe), puis a₂₃ > 0 et a₃₀ > 0 (puisque a₀₂ < 0 et que la seconde suite est directe), d’où a₁₃ > 0 (en vertu de (22)) ; donc la suite (D₀, D₁, D₃) est directe dans ce cas. Supposons désormais a₀₁ > 0. Si a₃₀ ≤ 0, on a a₀₂ > 0 et a₂₃ > 0 (puisque la seconde suite est directe), puis a₁₂ > 0 (puisque a₂₀ < 0 et que la première suite est directe), d’où $a_{13} > 0$ (d’après (22)), et la suite $(D_0, D_1, D_3)$ est directe. Enfin il en est évidemment de même si $a_{01} > 0$ et $a_{30} > 0$. CQFD.

#### Corollaire {#alg-ix-s10-n4-cor-1 .statement}

*Soient $D_1$ et $D_2$ deux demi-droites distinctes de E. Pour toute demi-droite $D_0$ de E telle que la suite $D_0, D_1, D_2$ soit directe, l’ensemble des demi-droites $D$ de E telles que $D_1 < D < D_2$ (pour la relation d’ordre total définie par $D_0$) est égal au secteur angulaire ouvert d’origine $D_1$ et d’extrémité $D_2$.

En effet, étant donnée une demi-droite $D_3$, il s’agit de montrer que les relations « la suite $D_1, D_3, D_2$ est directe » et « les suites $D_0, D_1, D_3$ et $D_0, D_3, D_2$ sont directes » sont équivalentes. Pour abréger notons $(ijk)$ la relation « la suite $(D_i, D_j, D_k)$ est directe ». D’après la prop. 11, la conjonction de (132) et (120) entraîne (130) ; de même la conjonction de (201) et de (213) entraîne (203) ; d’où la moitié de notre assertion. Réciproquement supposons (012), (013) et (032) ; comme la conjonction de (312) et (320) entraîne (310) (prop. 11), et que (310) et (013) sont incompatibles, (312) est fausse ; ceci démontre (132) et achève la démonstration.

En vertu du corollaire qui précède, le secteur angulaire ouvert (resp. fermé) d’origine $D_1$ et d’extrémité $D_2$ est noté $\{D_1, D_2\}$ (resp. $[D_1, D_2]$), étant entendu qu’il s’agit d’intervalles pour la structure d’ordre définie par n’importe quelle demi-droite $D_0$ telle que la suite $D_0, D_1, D_2$ soit directe.

#### Proposition 12 {#alg-ix-s10-prop-12 .statement}

*Soient A un corps ordonné maximal, E un plan orienté sur A, $D_0$ une demi-droite de E et G l’ensemble des demi-droites de E distinctes de $D_0$. Les ensembles totalement ordonnés A et G (prop. 11) sont isomorphes.

Soit, en effet, $(x, y)$ une base de E telle que $x \in - D_0$ et le bivecteur $x \wedge y$ soit $> 0$. À tout élément $t$ de A faisons correspondre la demi-droite $f(t)$ à laquelle appartient le vecteur $(1 - t^2)x + 2ty$. Il est clair que $f(A) \subset G$. Montrons que $f$ est strictement croissante. En effet, pour que la suite $D_0, f(t), f(t')$ ($t, t'$ dans A) soit directe, il faut et il suffit, par définition, que deux au moins des éléments

$$
-2t, \quad (1-t^2)2t' - (1-t'^2)2t, \quad 2t'
$$

soient $> 0$. Or le second est égal à $2(t' - t)(1 + tt')$. Donc, si $t < t'$, on a, soit $tt' \geqslant 0$, donc $t' > 0$ ou $-t > 0$, soit $tt' < 0$, donc $-t > 0$ et $t' > 0$; en tous cas $D_0, f(t), f(t')$ est directe. Comme $A$ est totalement ordonné, $f$ est un isomorphisme de $A$ sur l’ensemble ordonné $f(A)$ (*Ens*, chap. III, § 1, no 14, prop. 13).

Il reste à montrer que $f$ est *surjective*. Pour cela considérons la forme positive $\Phi$ sur $E$ telle que $(x, y)$ soit une base orthonormale pour $\Phi$. Pour toute demi-droite $D \in G$, il existe un angle $\varphi$ et un seul tel que $2\varphi = (\widehat{-D_0, D})$ (no 1, prop. 3) ; comme $(\widehat{-D_0, D})$ n’est pas l’angle plat, $\varphi$ n’est pas l’angle droit, et $\operatorname{tg} \varphi$ est donc fini. Alors, en vertu des formules (16) (no 3), on a $D = f(\operatorname{tg} \varphi)$. Ceci termine la démonstration.

*Exercices.* — 1) Avec les notations du no 1, on pose $Q(x) = \Phi(x, x)$; l’espace vectoriel $E$ s’identifie canoniquement à $C^-(Q)$ (§ 9, no 1). Pour tout $z \in C^+(Q)$, et tout $x \in E$, on a $zx \in E$; montrer que $x \to zx$ est un élément de $A(\Phi)$, et que $z \to s_z$ est un isomorphisme de $C^+(Q)$ sur l’algèbre $A(\Phi)$.

2) Les hypothèses et notations sont celles du no 1 et de l’exerc. 1.

a) Soit $C$ l’ensemble des $x \in E$ tels que $\Phi(x, x) = 1$ (*cercle unité*), et soit $\mathcal{D}$ l’ensemble des droites $D$ dont l’intersection avec $C$ n’est pas vide (et par suite formée de deux éléments opposés de $E$). On appelle *droite pointée* tout couple $\Delta = (D, z)$ formé d’une droite $D \in \mathcal{D}$ et d’un des points $z \in D \cap C$. Montrer que si $\Delta_1 = (D_1, z_1)$, $\Delta_2 = (D_2, z_2)$ sont deux droites pointées, il existe une rotation $u$ et une seule telle que $u(z_1) = z_2$ (et par suite $u(D_1) = D_2$), ce qu’on exprime en écrivant $u(\Delta_1) = \Delta_2$. Dans l’ensemble des couples $(\Delta_1, \Delta_2)$ de droites pointées, la relation « il existe une rotation $u$ telle que $u(\Delta_1) = \Delta_1'$ et $u(\Delta_2) = \Delta_2'$ » est une relation d’équivalence. L’ensemble $\mathfrak{U}_1$ des classes d’équivalence de droites pointées suivant cette relation est appelé l’ensemble des *angles de droites pointées*, et la classe d’équivalence à laquelle appartient un couple $(\Delta_1, \Delta_2)$ de droites pointées est appelée l’*angle* de ce couple et notée $(\widehat{\Delta_1, \Delta_2})$; la relation $(\widehat{\Delta_1, \Delta_2}) = (\widehat{\Delta_1', \Delta_2'})$ est équivalente à $(\widehat{\Delta_1, \Delta_1'}) = (\widehat{\Delta_2, \Delta_2'})$ et la rotation qui transforme $\Delta_1$ en $\Delta_2$ est dite *rotation d’angle* $0 = (\widehat{\Delta_1, \Delta_2})$ et notée $h_1(\theta)$; $h_1$ est une bijection de $\mathfrak{U}_1$ sur $O^+$ et on transporte à $\mathfrak{U}_1$ au moyen de $h_1^{-1}$ la structure de groupe commutatif de $O^+$, en notant additivement le groupe $\mathfrak{U}_1$ ainsi défini ; on appelle encore angle *plat* dans $\mathfrak{U}_1$ l’angle du couple formé d’une droite pointée $(D, z)$ et de la droite pointée « opposée » $(D, -z)$, qui correspond à la rotation $x \to -x$.

b) Dans l’ensemble $\mathcal{D}_0 \supset \mathcal{D}$ des droites non isotropes, on définit comme au no 3 la notion d’*angle de droites*, le groupe $\mathfrak{U}_0$ (en utilisant le cor. 3 de la prop. 1 du no 1), l’angle *droit* dans $\mathfrak{U}_0$, et la bijection canonique $h$ de $\mathfrak{U}_0$ sur $S^+/H$. Avec les notations du cor. de la prop. 3, on pose $\bar{d} = h_1^{-1} \circ d \circ h$ et $\bar{i} = h^{-1} \circ i \circ h_1$, de sorte que $\bar{i}$ est un homomorphisme de $\mathfrak{U}_1$ dans $\mathfrak{U}_0$ et $\bar{d}$ un homomorphisme de $\mathfrak{U}_0$ dans $\mathfrak{U}_1$; $\bar{d}$ est bijectif, et le noyau de $\bar{i}$ est formé de '0 et de l’angle plat; en outre on a $\bar{d}(\bar{i}(\theta)) = 2\theta$ pour $\theta \in \mathfrak{U}_1$ et $\bar{i}(\bar{d}(\varphi)) = 2\varphi$ pour $\varphi \in \mathfrak{U}_0$. Pour que $\bar{i}$ soit surjectif (autrement dit, pour que $\mathcal{D}$ soit l’ensemble de toutes les droites non isotropes), il faut et il suffit que le corps A soit *pythagoricien* (chap. VI, § 2, exerc. 8 d)) et qu’il existe une base orthonormale pour $\Phi$; il revient au même de dire que $\Phi(x, x)$ est un *carré* pour tout $x \in E$.

3) Les hypothèses et notations sont celles de l’exerc. 2.
   a) Soit s une symétrie par rapport à une droite non isotrope D ($§ 6$, n° 4). Pour toute droite pointée $\Delta_1 = (D_1, z_1)$, soit
   $$
   \Delta_2 = s(\Delta_1) = (s(D_1), s(z_1)),
   $$
   et soit $\varphi = (\widehat{D_1}, \widehat{D})$; montrer que l’on a $(\widehat{\Delta_1}, \widehat{\Delta_2}) = \bar{d}(\varphi)$.
   b) Montrer que toute transformation orthogonale de déterminant -1 est une symétrie s par rapport à une droite non isotrope (cf. § 6, exerc. 15 e)); pour toute rotation u, on a $sus^{-1} = u^{-1}$.
   c) Si $x, y$ sont deux points quelconques de E tels que $\Phi(x, x) = \Phi(y, y) \neq 0$, il existe une symétrie et une seule par rapport à une droite non isotrope, qui transforme $x$ en $y$.
   d) Soient s, s' les symétries par rapport à deux droites non isotropes D, D', et soit $\varphi = (\widehat{D}, \widehat{D'})$; pour que s’s soit une rotation d’angle $\theta$, il faut et il suffit que $\bar{d}(\varphi) = \theta$.
   e) Montrer que le groupe des commutateurs du groupe orthogonal O(Q) est l’image de $\mathfrak{U}_1$ par l’homomorphisme $\theta \to h_1(2\theta)$ ($§ 6$, exerc. 17 a)); pour que cette image soit égale à $O^+$, il faut et il suffit que l’homomorphisme $\bar{i}$ soit surjectif (exerc. 2 b)).

4) Les hypothèses et notations sont celles de l’exerc. 2. Soient $a, b$ deux points du cercle C, $\Delta_a, \Delta_b$ les droites pointées passant par $a$ et $b$ (et par 0) respectivement, et soit $\theta = (\widehat{\Delta_a}, \widehat{\Delta_b})$. Pour tout $x \in E$, distinct de $a$ et $b$, soit $D_{xa}$ (resp. $D_{xb}$) la droite affine passant par $a$ et $x$ (resp. $b$ et $x$), et soit $D'_{xa}$ (resp. $D'_{xb}$) la direction de $D_{xa}$ (resp. $D_{xb}$); montrer que pour que $x \in C$ ($x$ distinct de $a$ et $b$), il faut et il suffit que l’angle $\varphi = (\widehat{D'_{xa}}, \widehat{D'_{xb}})$ soit tel que $\bar{d}(\varphi) = \theta$ (utiliser l’exerc. 3). Comment se modifie ce résultat lorsque $x = a$ ou $x = b$ (cf. § 6, exerc. 25 a))?

5) Avec les notations des n°s 1 et 2 et de l’exerc. 2, on suppose que $\Phi$ est d’indice 1, autrement dit que $\delta$ est un carré $\gamma^2$ dans A; on désigne par $D_1, D_2$ les droites isotropes de E, contenant respectivement les vecteurs $e_1 - \frac{1}{\gamma} e_2$ et $e_1 + \frac{1}{\gamma} e_2$.
   a) Montrer que le groupe des rotations $O^+$ est isomorphe au groupe multiplicatif $A^*$ du corps A.
   b) Pour tout angle $\theta \in \mathfrak{U}_1$, on pose $e_w(\theta) = c_w(h_1(\theta)) + \gamma s_w(h_1(0))$. Montrer que $\theta \to e_w(\theta)$ est un isomorphisme de $\mathfrak{U}_1$ sur le groupe $A^*$.

c) Soient D, D' deux droites quelconques, et soit $\varphi = (\widehat{D}, \widehat{D'})$. Montrer que le birapport $\begin{bmatrix} D_1 & D_2 \\ D' & D \end{bmatrix}$ (chap. II, 2e éd., App. III, exerc. 5) est égal à $e_w(\bar{d}(\varphi))$ ("formule de Laguerre"). (Remarquer que $D_1$ et $D_2$ sont invariantes par toute similitude directe, et en utilisant l’exerc. 4 c) du chap. II, 2e éd., App. III, se ramener au cas où $D = Ae_1$.)

6) On suppose que A est un corps ordonné.
a) Soient $D_1, D_2$ deux demi-droites non isotropes d’origine 0. Montrer qu’il existe une similitude directe $u$ telle que $u(D_1) = D_2$; toute autre similitude directe ayant cette propriété est de la forme $v = su$, où s est une homothétie de rapport $> 0$.

b) Dans l’ensemble des couples $(D_1, D_2)$ de demi-droites non isotropes, la relation « il existe une similitude directe $u$ telle que $u(D_1) = D'_1$ et $u(D_2) = D'_2$ » est une relation d’équivalence. L’ensemble $\mathfrak{A}$ des classes d’équivalence de demi-droites non isotropes, suivant cette relation, est appelé l’ensemble des angles de demi-droites (non isotropes) et la classe d’équivalence d’un couple $(D_1, D_2)$ de telles demi-droites est appelée l’angle de ce couple et notée $(\widehat{D_1}, \widehat{D_2})$; si $\theta = (\widehat{D_1}, \widehat{D_2})$, on dit que $\theta$ est l’angle de toute similitude directe transformant $D_1$ en $D_2$; soit $h_2(\theta)$ la classe mod. $H^+$ de ces similitudes, de sorte que $h_2$ est une bijection de l’ensemble $\mathfrak{A}$ sur le groupe $S^+/H^+$; on transporte à $\mathfrak{A}$ au moyen de $h_2^{-1}$ la structure de groupe commutatif de $S^+/H^+$, en notant additivement le groupe $\mathfrak{A}$ ainsi défini. Définir une injection canonique $\bar{j}$ du groupe $\mathfrak{A}_1$, des angles de droites pointées (exerc. 2) dans le groupe $\mathfrak{A}$, telle que $h_2 \circ \bar{j} \circ h_2^{-1}$ soit l’injection canonique $j$ de $O^+$ dans $S^+/H^+$. Pour que $\bar{j}$ soit surjective, il faut et il suffit que l’homomorphisme $\bar{i}$ de $\mathfrak{A}_1$ dans $\mathfrak{A}_0$ (exerc. 2 b)) soit surjectif.

c) Montrer que dans $\mathfrak{A}$ l’équation $2\theta = 0$ a 2 solutions si $\delta < 0$ et 4 solutions si $\delta > 0$. Dans le premier cas, la solution $\varpi \neq 0$ de cette équation est encore appelée l’angle plat.

¶ 7) Les hypothèses et notations étant celles de l’exerc. 6, on suppose l’homomorphisme $\bar{j}$ bijectif ; on définit alors cos $\theta$ et sin $\theta$ pour tout $\theta \in \mathfrak{A}$ comme au no 3. Soit T l’ensemble des $\theta \in \mathbf{A}$ tels que $\sin \theta \geqslant 0$.

a) Montrer que pour tout $\theta \in T$, il existe un angle $\theta' \in T$ et un seul tel que $2\theta' = \theta$; on pose $\theta' = \theta/2$.

b) Soit L le $\mathbf{Z}$-module des combinaisons linéaires formelles des éléments de T à coefficients dans $\mathbf{Z}$ (chap. II, § 1, no 8); on désigne par $\xi + \eta$ et $-\xi$ la somme et l’opposé dans L. Soit N le sous-module de L engendré par les éléments de L de la forme $\xi + \eta - (\xi + \eta)$ pour tous les couples $(\xi, \eta)$ d’éléments de T tels que $\xi + \eta \in T$ (somme prise dans le groupe $\mathfrak{A}$). Soient $\dot{f}$ l’homomorphisme de L dans $\mathfrak{A}$ qui prolonge l’injection canonique de T dans $\mathfrak{A}$, et $\dot{g}$ l’endomorphisme de L qui prolonge l’application $\theta \to \theta/2$ de T dans lui-même. On a $\dot{f}(N) = \{0\}$ et $\dot{g}(N) \subset N$; par passage aux quotients, on déduit de $\dot{f}$ un homomorphisme $f$ de $M = L/N$ dans $\mathfrak{A}$, et de $\dot{g}$ un endomorphisme $g$ de $M$; on pose $g(\mu) = \mu/2$ et si $g^m$ est le m-ème itéré de g, $g^m(\mu) = 2^{-m}\mu$; on a $2^m(2^{-m}\mu) = \mu$ pour tout $\mu \in M$.

c) Montrer que la restriction à T de l’application canonique $\psi$ de L sur $M = L/N$ est injective, ce qui permet d’identifier T à une partie de M au moyen de $\psi$. Montrer que, si $\lambda_1, \ldots, \lambda_m$ sont des éléments $\neq 0$ de T, la somme $\lambda_1 + \lambda_2 + \cdots + \lambda_m$ ne peut être 0 dans M (considérer l’élément $2^{-m}(\lambda_1 + \cdots + \lambda_m)$ et raisonner par récurrence sur m, en remarquant que ces éléments appartiennent à T).

d) Soit $M_+$ l’ensemble des sommes finies (dans M) d’éléments de T ; montrer que $M_+ \cap (-M_+) = \{0\}$ et $M = M_+ \cup (-M_+)$, et par suite que $M_+$ est l’ensemble des éléments $\geqslant 0$ pour une structure de groupe totalement ordonné sur M (on notera que pour tout $\mu \in M_+$, il existe un entier m tel que $2^{-m}\mu \in T$) ; on dit que ce groupe totalement ordonné est le groupe des mesures des angles de demi-droites. Montrer que l’homomorphisme $f$ de M dans $\mathfrak{A}$ est surjectif, et que son noyau est l’ensemble des multiples entiers de $2\pi$, où $\pi$ est l’angle plat (exerc. 6 c)). Prouver que T s’identifie à l’intervalle $[0, \pi]$ dans M (établir par récurrence sur m que si $\mu, \lambda_1, \ldots, \lambda_m$ appartiennent à T et si on a $\lambda_1 + \cdots + \lambda_m \leqslant \mu$, alors $\lambda_1 + \cdots + \lambda_m \in T$). Montrer que dans T (ainsi identifié à un intervalle de M), la fonction $\theta \to \cos \theta$ est strictement décroissante.

e) Pour que le groupe totalement ordonné M soit archimédien (chap. VI, § 1, exerc. 31), il faut et il suffit que le groupe additif du corps A soit archimédien. (Pour voir que la condition est nécessaire, remarquer que si sin $\theta$ est infiniment petit par rapport au sous-corps $\mathbf{Q}$ de A (chap. VI, § 2, exerc. 1), il en est de même de sin $n\theta$ pour tout entier n. Pour voir que la condition est suffisante, remarquer que si $0 \leqslant \theta \leqslant \pi/4$, on a sin $2\theta \geqslant \sqrt{2} \sin \theta$).

8) Soit E un plan orienté sur un corps ordonné A. Soient D', D'' deux demi-droites distinctes ; soit $x'$ (resp. $x''$) un vecteur $\neq 0$ dans D' (resp. D'') ; on dit que le secteur angulaire (ouvert ou fermé) d’origine D' et d’extrémité D'' est saillant (resp. rentrant, plat) si $x' \wedge x'' > 0$ (resp. $x' \wedge x'' < 0, x' \wedge x'' = 0$).

a) Pour qu’il existe un automorphisme de l’espace vectoriel E transformant un secteur angulaire ouvert (resp. fermé) $\Sigma_1$ en un secteur angulaire ouvert (resp. fermé) $\Sigma_2$, il faut et il suffit que $\Sigma_1$ et $\Sigma_2$ soient tous deux saillants, ou tous deux rentrants, ou tous deux plats.

b) Montrer que l’ensemble ordonné $\{D', D''\}$ est isomorphe à l’intervalle $[0, 1]$ de A (considérer d’abord le cas d’un secteur saillant et remarquer que, dans A, deux intervalles fermés bornés quelconques sont des ensembles ordonnés isomorphes).

c) Avec les notations et hypothèses de l’exerc. 7, définir une application bijective canonique de l’ensemble T sur un secteur angulaire plat, et montrer que cette application est un isomorphisme pour les structures d’ordre.

9) Soient A un corps ordonné pythagoricien, E un espace vectoriel sur A de dimension finie, Q une forme quadratique positive non dégénérée sur E, pour laquelle E admet une base orthonormale (autrement dit, Q(x) est un carré dans A pour tout x ∈ E). Montrer que le groupe des commutateurs Ω(Q) du groupe orthogonal O(Q) est le groupe des rotations O⁺(Q) = SO(Q) (utiliser l’exerc. 3 e) du § 10 et l’exerc. 17 a) du § 6).

10) Soient A un corps ordonné maximal, E un espace vectoriel de dimension finie sur A, Q une forme quadratique positive non dégénérée sur E. Pour toute transformation orthogonale u ∈ O(Q), montrer qu’il existe une décomposition de E en somme directe de sous-espaces deux à deux orthogonaux P, N, R_i (1 ≤ i ≤ r) ayant les propriétés suivantes : 1° u(x) = x dans P, u(x) = −x dans N ; 2° chacun des R_i est de dimension 2, on a u(R_i) = R_i et la restriction de u à R_i est une rotation d’angle θ_i, distinct de 0 et de l’angle plat. En outre, pour deux décompositions de cette nature, les sous-espaces P et N sont les mêmes, ainsi que la suite des éléments cos θ_i, à l’ordre près (cf. § 7, no 3, cor. 2 du th. 2). En déduire que toute rotation u ∈ O⁺(Q) est un commutateur tst⁻¹s⁻¹, où s et t sont dans O(Q) et s² = 1 (cf. exerc. 3 d)).

11) Soient A un corps ordonné maximal, L le corps des quaternions sur A (relatif au couple (−1, −1)), E le sous-espace (de dimension 3) de L formé des quaternions purs (§ 9, exerc. 15 a)) ; tout quaternion s’écrit donc d’une seule manière s = α . 1 + v, où α ∈ A et v ∈ E ; on a α² − v² = ρ . 1, où ρ ∈ A et ρ ≥ 0 ; on pose \|v\| = \sqrt{\rho}.

a) Soit φ(s) la rotation x → sx s⁻¹ dans E, pour la forme quadratique positive non dégénérée x → \|x\|^2 sur E (§ 9, no 5, th. 4 et exerc. 15). Montrer que si v ≠ 0, les vecteurs de la droite D ⊂ E contenant v sont invariants par φ(s) ; la restriction de φ(s) au plan orthogonal P = D⁰ est une rotation d’angle θ telle que (pour une orientation convenable de P) on ait tg \frac{\theta}{2} = \|v\|/α. (Si (1, i, j, k) est la base canonique de L sur A, se ramener au cas où v = βi, β ∈ A, et calculer alors sjs⁻¹).

b) Montrer que tout quaternion de norme 1 peut s’écrire tst⁻¹s⁻¹, où s ∈ L, t ∈ E (cf. exerc. 10), et que, si a, b sont deux quaternions purs de norme 1, il existe un quaternion s tel que b = sas⁻¹.

c) Pour que deux quaternions s = α + v, t = β + w, où α, β sont dans A, v, w dans E, soient permutables, il faut et il suffit que v = λw, λ ∈ A ; pour que st = −ts, il faut et il suffit que α = β = 0 et que les vecteurs v et w dans E soient orthogonaux (cf. § 3, exerc. 10).

12) Soient A un corps ordonné maximal, L un espace euclidien de dimension n sur A, dont la forme métrique Φ est positive non dégénérée ; on désigne par d(x, y) la distance \sqrt{\Phi(x - y, x - y)} de deux points de L (§ 7, no 1, Remarque). Pour tout point c ∈ L et tout élément ρ > 0 de A, on appelle sphère de centre c et de rayon ρ l’ensemble des x ∈ L tels que d(x, c) = ρ ; les sphères sont donc des quadriques affines non dégénérées dans L, admettant un centre (§ 6, exerc. 25).

a) Montrer qu’en tout point x d’une sphère S de centre c, l’hyperplan tangent à S en x (§ 6, exerc. 25) est perpendiculaire (§ 6, exerc. 22) à la droite passant par c et x.

b) Soient S une sphère de centre c et de rayon ρ, a un point de L, D une droite passant par a et rencontrant S en deux points distincts x₁, x₂ (resp. tangente à S en un point x). Montrer que l’on a

$$
\Phi(x_1 - a, x_2 - a) = (d(a, c))^2 - \rho^2 \quad (\text{resp. } (d(x, a))^2 = (d(a, c))^2 - \rho^2).
$$

L’élément $(d(a, c))^2 - \rho^2$ de A est appelé la puissance de a par rapport à S.

c) Soient S₁, S₂ deux sphères n’ayant pas même centre ; montrer que l’ensemble des points de L dont les puissances par rapport à S₁ et S₂ sont égales, est un hyperplan perpendiculaire à la droite passant par les centres des deux sphères, et contenant l’intersection S₁ ∩ S₂ ; on dit que cet hyperplan est l’hyperplan radical de S₁ et S₂.

d) Soient S₁, S₂ deux sphères de centres respectifs c₁, c₂, de rayons respectifs ρ₁, ρ₂. Montrer que les propriétés suivantes sont équivalentes :

α) L’intersection S₁ ∩ S₂ n’est pas vide et, pour tout point de cette intersection, les hyperplans tangents à S₁ et S₂ en ce point sont perpendiculaires.

$\beta_1$ La puissance de c₁ par rapport à S₂ est $\rho_1^2$.

$\beta_2$ La puissance de c₂ par rapport à S₁ est $\rho_2^2$.

$\gamma_1$ L’hyperplan radical de S₁ et S₂ est l’hyperplan polaire (§ 6, exerc. 25) de c₁ par rapport à S₂.

$\gamma_2$ L’hyperplan radical de S₁ et S₂ est l’hyperplan polaire de c₂ par rapport à S₁.

Lorsque ces propriétés sont vérifiées, on dit que les sphères S₁, S₂ sont orthogonales.

e) Soient S₁, S₂ deux sphères orthogonales, c₁, c₂ leurs centres. Montrer que si $\varpi_1, \varpi_2$ sont les puissances d’un point x par rapport à S₁, S₂ respectivement, on a $\varpi_1 + \varpi_2 = 2\Phi(x - c_1, x - c_2)$. Réciproque.

13) Les hypothèses et notations sont les mêmes que dans l’exerc. 12. Étant donnés un point c ∈ L et un élément $\alpha \neq 0$ de A, on appelle inversion de pôle c et de puissance $\alpha$ la permutation involutive u de l’ensemble $L - \{ c \}$ qui est telle que, pour tout $x \in L - \{ c \}$, $u(x)$ appartienne à la droite passant par c et x et vérifie la relation $\Phi(x - c, u(x) - c) = \alpha$. Par abus de langage, on dit que u est une inversion dans L.

a) Si u, v sont deux inversions de même pôle c et de puissances $\alpha, \beta$, $uv^{-1}$ est la restriction à $L - \{ c \}$ de l’homothétie (chap. II, 2e éd., App. II, exerc. 6) de centre c et de rapport $\alpha \beta^{-1}$.

b) Soit S une sphère (exerc. 12) contenant c. Montrer que l’image de $S - \{ c \}$ par une inversion de pôle c est un hyperplan perpendiculaire à la droite joignant c au centre de S (on dit par abus de langage que cet hyperplan est l’image de S par l’inversion considérée). Réciproque.

c) Soit S une sphère ne contenant pas c. Montrer que, si $\varpi$ est la puissance de c par rapport à S (exerc. 12 b)), l’image de S par une inversion de pôle c et de puissance $\alpha$ est l’image de S par une homothétie de centre c et de rapport $\alpha / \varpi$. Si $n = 2$ et si, pour tout $x \in S$, on désigne par T (resp. T’) la tangente à S (resp. $u(S)$) au point x (resp. $u(x)$), par D la droite passant par c, x et $u(x)$, montrer que l’on a $(\widehat{D, T}) = (\widehat{T', D})$.

d) Soient $S_1, S_2$ deux sphères orthogonales (exerc. 12 d)), $S'_1, S'_2$ leurs images par une inversion de pôle $c$. Si $c$ n’appartient pas à $S_1$ ni à $S_2$, montrer que $S'_1$ et $S'_2$ sont des sphères orthogonales. Si $c \in S_1$ et $c \notin S_2$, $S'_1$ est un hyperplan contenant le centre de $S'_2$. Si $c \in S_1 \cap S_2$, $S'_1$ et $S'_2$ sont des hyperplans perpendiculaires (\$ 6, exerc. 22). Réciproques.

e) Soient $u$ une inversion de pôle $c$ et de puissance $\alpha = \rho^2 > 0$ et $C$ la sphère de centre $c$ et de rayon $\rho$. Si $x_1, x_2$ sont deux points distincts situés sur une droite passant par $c$, et distincts de $c$, les propriétés suivantes sont équivalentes : $\alpha )$ $x_1$ et $x_2$ sont transformés l’un de l’autre par $u ; \beta )$ $x_1$ et $x_2$ sont conjugués par rapport à $C$ (\$ 6, exerc. 25); $\gamma )$ toute sphère contenant $x_1$ et $x_2$ est orthogonale à $C$. On dit encore que $u$ est l’inversion de sphère $C$.

¶ 14) Les hypothèses et notations étant les mêmes que dans l’exerc. 12, on prend une origine 0 dans L. Soit $E_1$ l’espace vectoriel somme directe de L et d’un espace $Af_1$ de dimension 1; on désigne par $Q_1$ la forme quadratique sur $E_1$ telle que pour $x \in L$ et $\eta \in A$, on ait

$$
Q_1(x + \eta f_1) = Q(x) + \eta^2,
$$

forme qui est positive et non dégénérée; on désigne par $C$ la sphère de centre 0 et de rayon 1 dans $E_1$ (pour $Q_1$).

Dans l’espace euclidien $E_1$, soit $s$ l’inversion de pôle $-f_1$ et de puissance 2 (exerc. 13); sa restriction $s_0$ à L transforme L en $C - \{ -f_1 \}$; $s_0$ (resp. $s_0^{-1}$) est appelée, par abus de langage, la projection stéréographique de L sur C (resp. de C sur L) de point de vue $-f_1$. Pour toute inversion $u$ dans L, de pôle $c$, $s_0 us_0^{-1}$ est une permutation involutive du complémentaire dans C de l’ensemble $\{ s_0(c), -f_1 \}$; on la prolonge en une permutation involutive $u'$ de c en posant $u'(s_0(c)) = -f_1,\ u'(-f_1) = s_0(c)$, et on dit que $u'$ est une inversion dans C. De même, pour toute symétrie $\nu$ dans L par rapport à un hyperplan, $s_0 \nu s_0^{-1}$ est une permutation involutive du complémentaire dans C de l’ensemble $\{ -f_1 \}$; on la prolonge en une permutation involutive $\nu'$ de C en posant $\nu'(-f_1) = -f_1$ et on dit que $\nu'$ est une symétrie dans C. Le groupe des permutations de C engendré par les inversions et symétries est appelé le groupe conforme de C (ou de L par abus de langage).

a) Montrer que le groupe conforme de C est engendré par les symétries $\nu'$ et les inversions $u'$ correspondant aux inversions $u$ dans L, de puissance $> 0$. (Utiliser l’exerc. 13 a) et remarquer que dans L toute translation, ainsi que l’homothétie $x \to -x$, sont des produits de symétries par rapport à des hyperplans).

b) Soit $u$ une inversion dans L de puissance $> 0$; montrer que l’inversion correspondante $u'$ dans C est la restriction à C d’une transformation bien déterminée $u'_1$ qui est, soit une inversion de puissance $> 0$ dans $E_1$, dont la sphère (exerc. 13 e)) est orthogonale à C, soit une symétrie par rapport à un hyperplan de $E_1$ passant par 0 (considérer dans $E_1$ l’inversion $u_1$ de même pôle et de même puissance que $u$). Formuler la proposition correspondante pour la symétrie $\nu'$ dans C correspondant à une symétrie $\nu$ dans L par rapport à un hyperplan.

c) Dans l’espace vectoriel $E_2 = A \times E_1$, on considère la forme quadratique $Q_2$ telle que, pour $\zeta \in A, y \in E_1$, on ait
$$
Q_2((\zeta, y)) = \zeta^2 - Q_1(y),
$$
forme qui est non dégénérée et de signature $(1, n + 1)$. On identifie $E_1$ à son image canonique dans l’espace projectif $\mathbf{P}(E_2)$ (chap. II, 2e éd., App. III, n° 4). Montrer (avec les notations de $b$) que $u'$ est aussi la restriction à $C$ d’une application linéaire projective $\bar{u}''$ provenant par passage aux quotients d’une transformation $u''$ du groupe orthogonal $O(Q_2)$, qui est une symétrie par rapport à un hyperplan non isotrope dans $E_2$. Formuler la proposition correspondante pour $\varphi'$. En déduire que le groupe conforme de $L$ est isomorphe au quotient du groupe $O(Q_2)$ par son centre (utiliser la prop. 5 et l’exerc. 17 c) du § 6). Conclure de là que toute transformation du groupe conforme est produit d’au plus $n + 2$ transformations qui sont des inversions ou des symétries dans $L$ (cf. § 6, exerc. 15 e)).

$d$ ) Soit $\Sigma$ l’ensemble dont les éléments sont les sphères et les hyperplans dans l’espace affine $L$. Déduire de $b$ qu’il existe une bijection de $\Sigma$ sur le complémentaire, dans $\mathbf{P}(E_2)$ de l’ensemble des $x \in E_1$ tels que $Q_1(x) \leqslant 1$, de sorte qu’à deux sphères orthogonales correspondent deux points conjugués par rapport à $C$.

15) Généraliser les définitions et résultats des exerc. 12 à 14 au cas où $A$ est un corps pythagoricien et où il existe une base orthonormale pour $\Phi$.

16) Soient $A$ un corps commutatif, $V$ un espace vectoriel sur $A$ de dimension impaire $2r + 1$, $F$ l’espace produit $A \times V$, $\Psi'$ une forme alternée non dégénérée sur $F$; dans l’espace projectif $\mathbf{P}(F)$, de dimension $2r + 1$, on dit que l’ensemble $C_0$ des droites qui sont les images canoniques des plans totalement isotropes de $F$ (pour $\Psi'$) est le complexe linéaire (projectif) associé à $\Psi'$.

On suppose dans ce qui suit que $A$ est ordonné maximal ; soit $\Phi$ une forme symétrique positive non dégénérée sur $V$. Soit $D$ la droite orthogonale à $V$ (pour $\Psi'$) dans $F$, qui est contenue dans $V$, et soit $H$ l’hyperplan orthogonal à $D$ (pour $\Phi$) dans $V$; dans $F$, $H$ est un sous-espace non isotrope pour $\Psi'$, dont l’orthogonal pour $\Psi'$ est donc un plan $P$ supplémentaire de $H$ et contenant $D$. Dans l’espace affine $E = \{1\} \times V \subset F$, on dit encore que l’ensemble $C$ des intersections avec $E$ des plans totalement isotropes de $F$ (pour $\Psi'$) non contenues dans $V$, est le complexe linéaire (affine) associé à $\Psi'$; la droite $\Delta = P \cap E$ est appelée l’axe du complexe linéaire $C$ (pour la structure d’espace euclidien définie sur $E$ par la forme métrique $\Phi$).

a) Montrer que, dans $E$, toute translation égale à un vecteur directeur de $\Delta$ (chap. II, 2e éd., App. II, n° 3) laisse $C$ invariant (cf. § 4, exerc. 6).

b) Soit $(e_i)_{0 \leq i \leq 2r}$ une base orthonormale de $V$ pour $\Phi$, telle que $e_0 \in D$ et que l’on ait $\Psi'(e_{2i-1}, e_{2i}) = \rho_i > 0$ pour $1 \leq i \leq r$, $\Psi'(e_j, e_k) = 0$ pour les couples d’indices qui ne sont pas de la forme $(e_{2i-1}, e_{2i})$ ou $(e_{2i}, e_{2i-1})$ (§ 7, n° 3, prop. 6). On prend dans l’espace affine E une origine $a \in \Delta$, et on pose $\Psi(a, e_0) = \rho_0$. Soit $x$ un vecteur appartenant au plan engendré par $e_{2i-1}$ et $e_{2i}$, et soit $y$ le vecteur de ce même plan tel que $\Phi(x, y) = 0$, $\Phi(y, y) = 1$ et que $x \wedge y = \lambda e_{2i-1} \wedge e_{2i}$ avec $\lambda > 0$. Soit $E_i$ la variété linéaire affine de dimension 3 engendrée par les points $a, a + e_0, a + e_{2i-1}, a + e_{2i}$ dans E, et soit $R_x$ l’intersection de $E_i$ et de l’hyperplan affine (dans E) engendré par les droites de C contenant le point $a + x$. Montrer que la direction des droites orthogonales (pour $\Phi$) au plan $R_x$ dans $E_i$ est une droite $L_x$ du plan $Ae_0 + Ay$, telle que si $\theta = (\widehat{D}, \widehat{L_x})$, on ait

$$
\operatorname{tg} \theta = \frac{\rho_i}{\rho_0} \sqrt{\Phi(x, x)}
$$

lorsque le plan $Ae_0 + Ay$ est orienté de sorte que $e_0 \wedge y$ soit positif.

¶ 17) a) Soient A un corps commutatif, $J : \xi \to \overline{\xi}$ un automorphisme involutif de A, E un espace vectoriel de dimension 2 sur A, $\Phi$ une forme sesquilinéaire hermitienne (non alternée) non dégénérée sur E, $(e_1, e_2)$ une base orthogonale de E pour $\Phi$ (§ 6, n° 1, th. 1), telle que

$$
\Phi(\xi_1 e_1 + \xi_2 e_2, \eta_1 e_1 + \eta_2 e_2) = \alpha \xi_1 \overline{\eta_1} + \beta \xi_2 \overline{\eta_2}
$$

$(\alpha$ et $\beta$ appartenant au corps K des invariants de J); on pose $\gamma = \beta / \alpha$. On identifie le point $\xi_1 e_1 + \xi_2 e_2 \in E$ à l’élément $\xi_1 + \xi_2 \rho$ de l’anneau B défini par les conditions $\rho^2 = -\gamma$, $\rho \xi = \overline{\xi} \rho$ pour $\xi \in A$ (§ 3, exerc. 4 a)). Pour tout $x = \xi_1 + \xi_2 \rho \in B$, on pose $\tilde{x} = \overline{\xi_1} - \xi_2 \rho$ et $N(x) = x \tilde{x} = \tilde{x} x$, de sorte que $x \to \tilde{x}$ est un antiautomorphisme involutif de l’algèbre B (sur K) et que l’on a $\Phi(x, x) = \alpha N(x)$. Montrer que toute similitude pour $\Phi$ dont le déterminant est égal au multiplicateur (appelée encore similitude directe) s’écrit d’une seule manière $x \to xy$, où $y$ est un vecteur non isotrope de E, et que son multiplicateur est $N(y)$.

b) On suppose d’abord que J est l’identité, donc $K = A$. Si A est de caractéristique $\neq 2$, retrouver ainsi les résultats du n° 1. Développer la théorie correspondante lorsque A est de caractéristique 2 (cf. § 4, exerc. 14 ; on distinguera deux cas, suivant que $\gamma$ est ou non un carré dans A).

c) On suppose $J \neq 1$, de sorte que A est une extension quadratique séparable de K. Alors $\Phi$ vérifie nécessairement la condition (T) (§ 4, n° 2 et exerc. 1) ; si $\Phi$ est d’indice 0, B est un corps réflexif de centre K (chap. VIII, § 11, exerc. 4), et si $\Phi$ est d’indice 1, B est isomorphe à $\mathbf{M}_2(K)$.

d) On suppose $J \neq 1$ et A de caractéristique $\neq 2$ ; on a alors $A = K(\theta)$ avec $\theta^2 = -\delta \in K$. Si S est le groupe des similitudes directes pour $\Phi$, H le groupe des homothéties dans E, de rapport $\neq 0$ et appartenant à K (groupe isomorphe à $K^*$), montrer que le groupe S/H est isomorphe au groupe des rotations $O^+(Q)$, où Q est une forme quadratique non dégénérée sur un espace vectoriel F de dimension 3 sur K, telle qu’il existe une base orthogonale $(f_1, f_2, f_3)$ de F pour laquelle on ait

$$
Q(\zeta_1 f_1 + \zeta_2 f_2 + \zeta_3 f_3) = \gamma \zeta_1^2 + \delta \zeta_2^2 + \gamma \delta \zeta_3^2
$$

(cf. § 9, exerc. 15).

¶ 18) a) Soient $A$ un corps commutatif, $\xi \to \bar{\xi}$ un automorphisme involutif de $A$, $E$ un espace vectoriel de dimension paire $2m$ sur $A$, $\Phi$ une forme hermitienne non dégénérée et d’indice 0 sur $E$, satisfaisant à la condition (T), $\Delta$ le discriminant de $\Phi$ par rapport à une base de $E$. Soit $M(\Phi)$ le groupe des multiplicateurs des similitudes pour $\Phi$ ($\S 4$, exerc. 8). Montrer que $M(\Phi)$ est un sous-groupe du groupe multiplicatif des éléments de $A$ de la forme $\alpha \bar{\alpha} - (-1)^m \beta \bar{\beta} \Delta$. (Raisonner par récurrence sur $m$, en utilisant l’exerc. 17, ainsi que les deux remarques suivantes : 1° si $u$ est une similitude de multiplicateur $\mu$, $x$ un vecteur de $E$, $y = u(x)$ et $z = u(y)$, il existe une transformation unitaire $v$ telle que $v(y) = y$ et $v(z) = \mu x$; 2° si $\alpha, \beta, \lambda$ sont trois éléments $\neq 0$ de $A$ tels qu’ils existe $a, b, c, d$ dans $A$ vérifiant les conditions $\lambda = a \bar{a} + \alpha c \bar{c}$, $\lambda = b \bar{b} + \beta d \bar{d}$, alors il existe $s, t$ dans $A$ vérifiant la condition $\lambda = s \bar{s} - \alpha \beta t \bar{t}$.

b) Soient $K$ un corps ordonné maximal, $K_1 = K((t_1))$ le corps des séries formelles par rapport à une indéterminée $t_1$, à coefficients dans $K$ (chap. IV, $\S 5$, no 7), $A = K_1((t_2))$ le corps des séries formelles par rapport à une seconde indéterminée $t_2$, à coefficients dans $K_1$. Soient $E$ un espace vectoriel de dimension 6 sur $A$, $Q$ une forme quadratique non dégénérée sur $E$, telle qu’il existe une base orthogonale $(e_i)$ pour laquelle on ait

$$
Q\left( \sum_{i=1}^{6} \xi_i e_i \right) = \xi_1^2 + \xi_2^2 + \xi_3^2 + \xi_4^2 + t_1 \xi_5^2 + t_2 \xi_6^2.
$$

Montrer qu’il n’existe aucune similitude pour $Q$, de multiplicateur $t_1 t_2$.
