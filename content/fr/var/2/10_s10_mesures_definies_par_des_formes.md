---
book: var
book_title: Variétés différentielles et analytiques
chapter: "2"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 10
section_title: Mesures définies par des formes différentielles
lang: fr
source: var-fr
pdf_pages: 0126-0135
extraction: ocr
subsections:
    - "no": 1
      title: Mesure module d’une forme différentielle
      page: 0
      pdf_page: 126
    - "no": 2
      title: Orientations
      page: 0
      pdf_page: 128
    - "no": 3
      title: Formes différentielles M-tordues
      page: 0
      pdf_page: 131
    - "no": 4
      title: Mesure associée à une forme différentielle tordue
      page: 0
      pdf_page: 132
statements: 0
exercises: 0
content_sha256: 0c1bcecfea38bc2fc1272b64c6d5313be25d53ad6f0919550db0761e5da947f0
---

## § 10. Mesures définies par des formes différentielles

Dans ce paragraphe, on suppose que $K$ est localement compact. A partir du no 10.2, on suppose $K=\mathbf{R}$. Dans les nos 10.1 et 10.4, toutes les variétés considérées sont supposées localement de dimension finie; lorsqu’elles sont séparées, elles sont localement compactes.

### 10.1. Mesure module d’une forme différentielle

**Notations.** — On note $\mu$ une mesure de Haar (INT, VII, § 1, no 2) sur le groupe additif de $K$. On note $\mu^{\otimes n}$ la mesure $\mu\otimes\cdots\otimes\mu$ sur $K^n$ et $\mu^{\otimes n}_U$ sa restriction à un ouvert $U$ de $K^n$. Pour $a\in K$, on note $\operatorname{mod}(a)$ le module de $a$ (INT, VII, § 1, no 10 et AC, VI, § 9, no 1). Si $K=\mathbf{R}$, on a $\operatorname{mod}(a)=|a|$; si $K=\mathbf{C}$, on a $\operatorname{mod}(a)=|a|^2$; si $K$ est ultramétrique, on a $\operatorname{mod}(a)=q^{-\nu(a)}$, où $q$ désigne le nombre d’éléments du corps résiduel de $K$ et $\nu$ la valuation nommée de $K$ (AC, VI, § 9, no 1, prop. 1).

### 10.1.1. Soient $U$ et $V$ des ouverts de $K^n$, et soit $f:U\to V$ une application de classe $C^r$, avec $r\in\mathbf{N}$. Soit $x\in U$; on appelle jacobien de $f$ en $x$, et on note $\operatorname{Jac}_x(f)$, le déterminant de l’application linéaire $Df(x)$ dérivée de $f$ en $x$. On note $\operatorname{Jac}(f)$ la fonction $x\mapsto\operatorname{Jac}_x(f)$; la fonction $\operatorname{mod}(\operatorname{Jac}(f))$ est une fonction continue dans $U$ à valeurs réelles positives.

### 10.1.2 (« Changement de variable dans les intégrales »). Les hypothèses étant celles de 10.1.1, supposons que $f$ soit un isomorphisme de classe $C^r$ de la variété $U$ sur la variété $V$. Alors l’image par $f$ de la mesure $\operatorname{mod}(\operatorname{Jac}(f))\mu^{\otimes n}_U$ est $\mu^{\otimes n}_V$; pour toute fonction continue à support compact $\varphi:V\to\mathbf{C}$, on a

$$
\int_V \varphi(y)\mu^{\otimes n}(y)=\int_U \varphi(f(x)).\operatorname{mod}(\operatorname{Jac}_x(f))\mu^{\otimes n}(x).
$$

### 10.1.3. Soit $X$ une variété de classe $C^r$, et soit $A$ une partie de $X$. On dit que $A$ est localement négligeable si, pour toute carte $(U,\varphi,K^n)$ de la variété $X$, l’ensemble $\varphi(A\cap U)$ est $\mu^{\otimes n}$-négligeable (INT, IV, § 2, no 2); cette condition ne dépend pas du choix de $\mu$, et il suffit de la vérifier pour une famille de cartes dont les domaines recouvrent $A$. Tout ensemble contenu dans la réunion d’une famille dénombrable d’ensembles localement négligeables est localement négligeable.

Exemples

a) Toute sous-variété de X qui est de codimension $\geq 1$ en tout point (i.e. d'intérieur vide) est localement négligeable.

b) Soit g une fonction de classe $C^r$ sur X, et soit $A_g$ l'ensemble des points $x \in X$ tels que $g(x) = 0$; supposons que l'intérieur de $A_g$ soit vide, et que $r = \omega$; alors $A_g$ est localement négligeable.

c) Soit $f : Y \to X$ un morphisme de variétés de classe $C^r$, la variété Y étant réunion dénombrable de compacts. On suppose que l'on a $\dim_y Y \leq \dim_{f(y)} X$ pour tout $y \in Y$. L'image par $f$ de toute partie localement négligeable de Y est une partie localement négligeable de X. Il en est de même de l'image par $f$ de l'ensemble des points où $f$ n'est pas étalement (« premier théorème de Sard »); en particulier, si $\dim_y Y < \dim_{f(y)} X$ pour tout $y \in Y, f(Y)$ est une partie localement négligeable de X.

d) Supposons K de caractéristique zéro. Soit $f : Y \to X$ un morphisme de variétés de classe $C^r$ ($r \in \mathbf{N}_K, r \geq \infty$), Y étant réunion dénombrable de compacts. Soit C l'ensemble des points de Y où $f$ n'est pas une submersion (« points critiques »). Alors $f(C)$ est une partie localement négligeable de X (« second théorème de Sard »).[^1]

10.1.4. Soit X une variété paracompacte de classe $C^r$. Il existe sur X une classe M de mesures équivalentes (INT, V, § 5, n° 6) et une seule telle que, quelle que soit $\nu \in M$ et quelle que soit la carte $c = (U, \varphi, K^n)$ de X, l'image par $\varphi$ de la restriction de $\nu$ à U soit équivalente à $\mu_{\varphi(U)}^{\otimes n}$. On dit que M est la classe canonique de mesures sur X. Pour qu'un sous-ensemble A de X soit localement négligeable (10.1.3), il faut et il suffit qu'il soit localement négligeable (INT, IV, § 2, n° 2) pour une (resp. toute) mesure $\nu \in M$.

Si $K = \mathbf{R}$ et $r \neq \omega$ (resp. $K = \mathbf{R}$ ou $C$ et $r = \omega$, resp. K est ultramétrique), il existe $\nu \in M$ telle que, pour toute carte $c = (U, \varphi, K^n)$ de X, la densité de $\varphi(\nu_U)$ par rapport à $\mu_{\varphi(U)}^{\otimes n}$ soit partout $> 0$ et de classe $C^{r-1}$ (resp. de classe $C^\infty$, resp. localement constante). Si $\nu$ et $\nu'$ sont deux telles mesures, la densité de $\nu'$ par rapport à $\nu$ est partout $> 0$ et de classe $C^{r-1}$ (resp. de classe $C^\infty$, resp. localement constante).

10.1.5. Soit X une variété de classe $C^r$; soit $T'(X)$ le fibré cotangent de X (8.2.2) et posons $\Omega = \det(T'(X))$ (7.9.9). Le fibré vectoriel $\Omega$ est de rang 1 en chaque point; lorsque X est pure de dimension $n$, il s'identifie au fibré vectoriel $\mathrm{Alt}^n(T(X); K_X)$. Soit $\omega$ une section de $\Omega$ sur X; on dit, par abus de langage, que $\omega$ est une forme différentielle de degré maximum sur X. Soit $c = (U, \varphi, K^n)$ une carte de X; notons $u^1, \ldots, u^n$ les fonctions coordonnées sur $K^n$. Il existe une fonction $f_c$ et une seule sur $\varphi(U)$ telle que $\omega|U = \varphi^*(f_c du^1 \wedge \cdots \wedge du^n)$. On dit que $\omega$ est localement de module intégrable si, pour toute carte $c = (U, \varphi, K^n)$ de X, la fonction réelle $\mathrm{mod}(f_c) : \varphi(U) \to \mathbf{R}$ est localement intégrable pour $\mu_{\varphi(U)}^{\otimes n}$ (INT, IV, § 4, n° 1); il suffit de vérifier cette propriété pour les cartes d'un atlas de X. Si $\omega$ est continue, et en particulier si $\omega$ est de classe $C^s$, avec $s \in \mathbf{N}_K, s \leq r - 1$, alors $\omega$ est localement de module intégrable.

10.1.6 (« Mesure positive définie par une forme différentielle de degré maximum »). Conservons les notations de 10.1.5 et supposons de plus que X soit séparée et que $\omega$ soit localement de module intégrable. Si $c = (U, \varphi, K^n)$ est une carte deX, notons $\nu_c$ la mesure sur $\varphi(U)$ produit de la mesure $\mu_{\varphi(U)}^{\otimes n}$ par la fonction mod$(f_c)$ (INT, V, § 5, n° 2, déf. 2) et soit $\alpha_c$ l’image de $\nu_c$ par $\varphi^{-1}$. Il existe sur X une mesure $\alpha$ et une seule telle que, pour toute carte $c = (U, \varphi, K^n)$ de X, la restriction de $\alpha$ à U soit égale à $\alpha_c$. On dit que la mesure $\alpha$ est le module de $\omega$ et on la note mod$(\omega)_\mu$. C’est une mesure positive. Lorsque $K = \mathbf{R}$ et que $\mu$ est la mesure de Lebesgue, on écrit $|\omega|$ au lieu de mod$(\omega)_\mu$.

Si X est pure de dimension $n$, et si $a$ est un nombre réel $> 0$, on a $\mathrm{mod}(\omega)_{a\mu} = a^n \mathrm{mod}(\omega)_\mu$.

Soit A une partie de X. Pour que A soit localement négligeable (10.1.3), il faut et il suffit que, pour tout ouvert U de X et toute forme différentielle $\omega$ de degré maximum sur U qui est localement de module intégrable, l’ensemble $A \cap U$ soit localement négligeable pour la mesure $\mathrm{mod}(\omega)_\mu$.

Supposons de plus X paracompacte et soit $\nu$ une mesure sur X appartenant à la classe d’équivalence canonique M (10.1.4). La mesure $\mathrm{mod}(\omega)_\mu$ est de base $\nu$ (INT, V, § 5, n° 2, déf. 2). Pour que $\mathrm{mod}(\omega)_\mu$ appartienne à M, il faut et il suffit que l’ensemble des $x \in X$ tels que $\omega(x) = 0$ soit localement négligeable.

10.1.7. Exemple. — Soit G un groupe de Lie sur K, de dimension finie $n$, et soit $\omega$ une forme différentielle de degré $n$ sur G, invariante par les translations à gauche, et non nulle. La mesure $\mathrm{mod}(\omega)_\mu$ correspondante est alors une mesure de Haar à gauche sur le groupe localement compact G.

Lorsque G est le groupe multiplicatif $K^*$, on peut prendre pour $\omega$ la forme $dx/x$, et l’on a $\mathrm{mod}(\omega)_\mu = (\mathrm{mod})^{-1}.\mu$, cf. INT, VII, § 1, n° 10, prop. 14.

### 10.2. Orientations

Rappelons que, dans ce numéro et les suivants, on suppose $K = \mathbf{R}$.

10.2.1 (« Orientation d’un espace vectoriel réel »). Soit E un espace vectoriel réel de dimension finie $n$. On note Or(E) l’ensemble des orientations de E (A, VI, § 2, n° 7); les éléments de Or(E) sont les deux demi-droites fermées de l’espace vectoriel $\det(E) = \bigwedge^n E$. Si $\xi \in \mathrm{Or}(E)$, l’autre élément de Or(E) est appelé l’orientation opposée à $\xi$, et noté $-\xi$.

Soit $0 \to E' \xrightarrow{\alpha} E \xrightarrow{\beta} E'' \to 0$ une suite exacte d’espaces vectoriels (réels) de dimension finie; posons $p' = \dim E',\ p'' = \dim E''$ et soit $\xi'$ (resp. $\xi''$) une orientation de E' (resp. E''). On note $\xi'\xi''$ (resp. $\xi''\xi'$) l’orientation de E contenant un $(p' + p'')$-vecteur non nul $u' \wedge u''$ (resp. $u'' \wedge u'$), où $u'$ est l’image par $\wedge^\alpha$ d’un $p'$-vecteur de E' appartenant à $\xi'$ et où $u''$ est un $p''$-vecteur de E dont l’image par $\wedge^\beta$ appartient à $\xi''$ (cf. A, VI,§ 2, n° 7). Si $E = E' \times E''$, $\alpha$ et $\beta$ étant les applications canoniques, on dit que $\xi'\xi''$ est la produit de l’orientation $\xi'$ et de l’orientation $\xi''$.

10.2.2 (« Espace des orientations »). Soient B un espace topologique et M un fibré vectoriel réel de base B (au sens topologique — cf. § 6, p. 61, Note (*)), de rang fini

(7.1.6). Soit $\mathrm{Or}_M$ l’ensemble somme des $\mathrm{Or}(M_b)$, pour $b \in B$, et soit $\pi : \mathrm{Or}_M \to B$ l’application telle que $\pi(\mathrm{Or}(M_b)) = \{b\}$. Il existe sur $\mathrm{Or}_M$ une structure d’espace topologique et une seule telle que:

a) $\pi$ soit continue.

b) Si $s$ est une section continue et partout non nulle de $\det(M)$ sur un ouvert $U$ de $B$, et si $\xi(s(b))$ est l’orientation de $M_b$ définie par l’élément $s(b)$ de $\det(M_b)$, l’application $b \mapsto \xi(s(b))$ de $U$ dans $\mathrm{Or}_M$ est continue.

L’espace $\mathrm{Or}_M$ s’appelle l’espace des orientations de $M$. Le groupe $\{\pm 1\}$ opère sur $\mathrm{Or}_M$ par $\xi \mapsto \pm \xi$ (10.2.1). Le quadruplet $(\mathrm{Or}_M, \{\pm 1\}, B, \pi)$ est une fibration principale (6.2.1) de base $B$ et de groupe structural $\{\pm 1\}$; la projection $\pi : \mathrm{Or}_M \to B$ définit un isomorphisme de $\mathrm{Or}_M/\{\pm 1\}$ sur $B$, cf. n° 6.2.

Lorsque $B$ est muni d’une structure de variété, on munit $\mathrm{Or}_M$ de la structure de variété image inverse de celle de $B$ par $\pi$ (5.8.1); la fibration définie ci-dessus est alors une fibration de variétés et le morphisme $\pi$ est étale.

10.2.3. Conservons les hypothèses de 10.2.2. On appelle orientation du fibré vectoriel $M$ une section continue $\xi : B \to \mathrm{Or}_M$ de la projection $\pi : \mathrm{Or}_M \to B$. On dit que $M$ est orientable s’il possède une orientation; il revient au même de dire que le fibré $\mathrm{Or}_M$ est trivialisable, i.e. isomorphe à $B \times \{\pm 1\}$. Si $B$ est connexe non vide, tout fibré vectoriel orientable de base $B$ possède deux orientations, opposées l’une de l’autre.

Lorsque $M$ est réduit à 0, le fibré $\det(M)$ est le fibré trivial $R_B$ et $\mathrm{Or}_M$ s’identifie à $\mathrm{Or}(R) \times B$; le fibré $M$ possède une orientation canonique, correspondant à la demi-droite positive de $R$.

10.2.4 (« Orientation d’une variété »). Soit $X$ une variété localement de dimension finie sur $R$ de classe $C^r$, et soit $T(X)$ son fibré tangent. On note $\tilde{X}$ la variété $\mathrm{Or}_{T(X)}$; le groupe $\{\pm 1\}$ opère proprement et librement sur $\tilde{X}$ et $\tilde{X}/\{\pm 1\}$ s’identifie à $X$; les fibres de la projection $\pi : \tilde{X} \to X$ sont les ensembles $\mathrm{Or}(T_x(X))$, pour $x \in X$. On appelle orientation de $X$ une orientation du fibré $T(X)$, autrement dit une section continue du fibré $\tilde{X}$; une telle section est de classe $C^r$. On dit que $X$ est orientable si elle possède une orientation. Toute variété de dimension zéro est orientable et possède une orientation canonique (10.2.3).

Soit $\xi \in \tilde{X}$ et soit $x = \pi(\xi)$ son image dans $X$; l’application $T_\xi(\pi) : T_\xi(\tilde{X}) \to T_x(X)$ est un isomorphisme; elle permet d’identifier $\xi$ à un élément $\tilde{\xi}$ de $\mathrm{Or}(T_\xi(\tilde{X}))$. L’application $\xi \mapsto \tilde{\xi}$ est une orientation de $\tilde{X}$, dite canonique; en particulier, $\tilde{X}$ est orientable.

10.2.5 (« Orientation d’un morphisme »). Soient $X$ et $Y$ deux variétés localement de dimension finie et soit $f : X \to Y$ un morphisme de variétés. On appelle orientation de $f$ un morphisme $\tilde{f} : \tilde{X} \to \tilde{Y}$ rendant commutatif le diagramme

$$
\begin{array}{ccc}
\tilde{X} & \xrightarrow{\tilde{f}} & \tilde{Y} \\
| & & | \\
X & \xrightarrow{f} & Y
\end{array}
$$

et compatible avec l’action du groupe $\{\pm 1\}$.

Si $\tilde{f}$ est une orientation de $f$ et si $\eta$ est une orientation de $Y$, il existe une orientation $\xi$ et une seule de $X$ telle que le diagramme

$$
\begin{array}{ccc}
\tilde{X} & \xrightarrow{\tilde{f}} & \tilde{Y} \\
\xi \downarrow & & \eta \downarrow \\
X & \xrightarrow{f} & Y
\end{array}
$$

soit commutatif. On dit que $\xi$ est associée à $\eta$ par $\tilde{f}$.

**Exemples**

a) Si $Y$ est réduite à un point, une orientation de $f$ équivaut à une orientation de $X$.

b) Supposons $f$ étale. Pour tout $x \in X$, l’application $T_x(f)$ est un isomorphisme de $T_x(X)$ sur $T_{f(x)}(Y)$, et définit (par transport de structure) une bijection

$$
\tilde{f}_x : \mathrm{Or}(T_x(X)) \to \mathrm{Or}(T_{f(x)}(Y)).
$$

La famille des $\tilde{f}_x$ définit une orientation $\tilde{f} : \tilde{X} \to \tilde{Y}$ de $f$, dite canonique.

c) Plus généralement, supposons que $f$ soit une submersion, et soit $\alpha$ une orientation du fibré $T(X/Y)$ (8.1.3). Soient $x \in X$ et $\xi$ une orientation de $T_x(X)$. Posons $y = f(x)$; on a une suite exacte (8.1.3)

$$
0 \to T_x(X/Y) \to T_x(X) \xrightarrow{T_x(f)} T_y(Y) \to 0
$$

et il existe donc une orientation $\tilde{f}_\alpha(\xi)$ de $T_y(Y)$ et une seule telle que $\xi = \tilde{f}_\alpha(\xi)\alpha(x)$ (10.2.1). L’application $\tilde{f}_\alpha : \tilde{X} \to \tilde{Y}$ est une orientation de $f$, dite associée à $\alpha$. L’application $\alpha \mapsto \tilde{f}_\alpha$ est une bijection de l’ensemble des orientations de $T(X/Y)$ sur l’ensemble des orientations de $f$.

d) Si $f : X \to Y$ est une immersion, les orientations de $f$ correspondent aux orientations du fibré normal à $f$.

10.2.6 (« Orientation d’un produit »). Soient $X_1$ (resp. $X_2$) une variété localement de dimension finie et $\xi_1$ (resp. $\xi_2$) une orientation de $X_1$ (resp. $X_2$). Soit $X = X_1 \times X_2$. L’application $(x_1, x_2) \mapsto \xi_1(x_1)\xi_2(x_2)$ (10.2.1) est une orientation de $X_1 \times X_2$, appelée *produit* des orientations $\xi_1$ et $\xi_2$, et notée $\xi_1 \xi_2$, ou $\xi_1 \otimes \xi_2$.

Supposons que $X_i$ ($i = 1, 2$) soit pure de dimension $n_i$. L’isomorphisme canonique $X_1 \times X_2 \to X_2 \times X_1$ transforme $\xi_1 \otimes \xi_2$ en $\xi_2 \otimes \xi_1$ (resp. en $-\xi_2 \otimes \xi_1$) si l’un des $n_i$ est pair (resp. si $n_1$ et $n_2$ sont impairs).

10.2.7 (« Cas complexe »). Soit $F$ un espace vectoriel complexe de dimension finie et soit $F_\mathbf{R}$ l’espace vectoriel réel sous-jacent. Soit $\{e_1, \ldots, e_m\}$ une base de $F$; alors $\{e_1, ie_1, e_2, ie_2, \ldots, e_m, ie_m\}$ est une base de $F_\mathbf{R}$ et l’orientation de $F_\mathbf{R}$ définie par le $2m$-vecteur

$$
e_1 \wedge ie_1 \wedge e_2 \wedge ie_2 \wedge \cdots \wedge e_m \wedge ie_m
$$

est indépendante du choix de la base $\{e_1, \ldots, e_m\}$ de $F$; on dit que c’est *l’orientation de $F_\mathbf{R}$* définie *par la structure complexe donnée*. Si $F$ est somme directe de deux sous-espaces $G$ et $H$, l’orientation de $F_\mathbf{R} = G_\mathbf{R} \oplus H_\mathbf{R}$ est le produit des orientations de $G_\mathbf{R}$ et $H_\mathbf{R}$.

Soit X une variété réelle localement de dimension finie, munie d'une structure presque complexe (8.8.3). Pour tout $x \in X$, soit $\xi(x)$ l'orientation de $T_x(X)$ définie par sa structure complexe. L'application $x \mapsto \xi(x)$ est une orientation de X, dite définie par la structure presque complexe. En particulier, nous munirons la variété analytique réelle X sous-jacente à une variété analytique complexe $X^c$, localement de dimension finie, de l'orientation définie par la structure presque complexe associée (8.8.6). Si l'on remplace la structure de variété analytique complexe donnée sur X par sa conjuguée (5.4.12.b)), cette orientation est multipliée par la fonction $x \mapsto (-1)^{\dim_{\mathbf{R}} X^c}$.

10.2.8. Exemples

a) Soit E un espace vectoriel réel de dimension finie. La variété analytique réelle définie par E (5.2.2) est orientable. Plus précisément, l'application $\xi \mapsto \xi(0)$ est une bijection de l'ensemble des orientations de cette variété sur Or(E).

En particulier, la variété $\mathbf{R}^n$ a une orientation canonique $\xi^n$ définie par la demi-droite $\mathbf{R}_+ e_1 \wedge \cdots \wedge e_n$ de Or($\mathbf{R}^n$).

b) Soit X une *sphère* de centre 0 et de rayon $> 0$ dans $\mathbf{R}^n$; c'est une sous-variété de $\mathbf{R}^n$. Pour tout $x \in X$, l'espace $T_x(\mathbf{R}^n) = \mathbf{R}^n$ est somme directe de la droite Rx et de l'hyperplan $T_x(X)$. Soit $\eta_x$ l'orientation $\mathbf{R}_+ x$ de Rx (« normale extérieure ») et soit $\xi_x$ l'unique orientation de $T_x(X)$ telle que le produit de $\eta_x$ et $\xi_x$ soit l'orientation $\xi^n$ de $\mathbf{R}^n$. L'application $x \mapsto \xi_x$ est une orientation de X, dite canonique.

c) Soit X une variété connexe, et soit G un groupe discret opérant proprement et librement sur X. Pour que X/G soit orientable, il faut et il suffit que X soit orientable et que l'action de G sur l'ensemble des orientations de X soit triviale.

d) *L'espace projectif réel* $P_{n-1}(\mathbf{R})$ s'identifie au quotient de la sphère $S_{n-1}$ par le groupe $\{ \pm 1 \}$ opérant par $x \mapsto \pm x$; il est orientable si $n$ est pair, et non orientable si $n$ est impair.

e) Tout quotient d'un groupe de Lie par un sous-groupe de Lie *connexe* est orientable.

### 10.3. Formes différentielles M-tordues

10.3.1. Soit X une variété réelle de classe $C^r$, et soit M un fibré vectoriel de base X, de rang fini et de classe $C^k$, avec $0 \leq k \leq r$. Soit $\lambda_M = (\mathrm{Or}_M, \{ \pm 1 \}, X, \pi)$ la fibration principale associée à la variété des orientations de M (10.2.2). Faisons opérer le groupe structural $\{ \pm 1 \}$ sur $\mathbf{R}$ par multiplication. On note $\tilde{R}_M$ l'espace fibré associé à $\lambda_M$ de fibre type $\mathbf{R}$ (muni de la loi d'opération définie ci-dessus) (6.5.1); il est muni (7.10.2) d'une structure de fibré vectoriel de base X, de rang 1 et de classe $C^k$; on l'appelle *fibré des scalaires M-tordus*.

10.3.2. On a un diagramme commutatif:

$$
\begin{array}{ccc}
\mathrm{Or}_M \times \mathbf{R} & \xrightarrow{\rho} & \tilde{R}_M \\
\downarrow \mathrm{pr}_1 & & \downarrow p \\
\mathrm{Or}_M & \xrightarrow{\varphi} & X
\end{array}
$$

où $p$ désigne la projection canonique de $\tilde{\mathbf{R}}_M$ sur $X$, $\rho$ l’application repère (6.5.1) de $\tilde{\mathbf{R}}_M$ et où $\varphi(\xi) = \rho(\xi, 1)$ pour $\xi \in \mathrm{Or}_M$. En particulier, l’image réciproque du fibré $\tilde{\mathbf{R}}_M$ par $\pi$ s’identifie au fibré trivial $\mathrm{Or}_M \times \mathbf{R}$. On identifie également un élément $\xi$ de $\mathrm{Or}_M$ à son image dans $\tilde{\mathbf{R}}_M$ par $\varphi$; avec cette convention, on a $\rho(\xi, a) = a\xi$ pour tout $(\xi, a) \in \mathrm{Or}_M \times \mathbf{R}$; on a $a\xi = b\eta$ si et seulement s’il existe $e \in \{ \pm 1 \}$ tel que $b = ea$ et $\eta = e\xi$. Une orientation $\xi$ de $M$ définit ainsi une section $x \mapsto \xi(x)$ de $\tilde{\mathbf{R}}_M$.

Il existe un isomorphisme $j$ et un seul de $\tilde{\mathbf{R}}_M \otimes \tilde{\mathbf{R}}_M$ sur le fibré trivial $R_X = X \times \mathbf{R}$ tel que $j(\xi \otimes \xi) = (\pi(\xi), 1)$ pour tout $\xi \in \mathrm{Or}_M$; cela permet d’identifier le fibré vectoriel $\tilde{\mathbf{R}}_M$ à son dual.

10.3.3. Soit de plus $F$ un fibré vectoriel de base $X$ et de classe $C^{r-1}$. Une forme différentielle sur $X$ à valeurs dans $\tilde{\mathbf{R}}_M \otimes F$ est appelée une forme différentielle $M$-tordue à valeurs dans $F$. Une telle forme de degré $p$ est une section du fibré $\mathrm{Alt}^p(T(X); \tilde{\mathbf{R}}_M \otimes F)$, qu’on identifie de façon évidente à $\tilde{\mathbf{R}}_M \otimes \mathrm{Alt}^p(T(X); F)$. Lorsque $F$ est le fibré trivial défini par un espace de Banach $E$, on parle simplement de forme $M$-tordue à valeurs dans $E$; lorsque $E = \mathbf{C}$ (resp. $\mathbf{R}$), on dit forme $M$-tordue complexe (resp. forme $M$-tordue réelle, ou forme $M$-tordue).

Soit $\omega$ une forme $M$-tordue de degré $p$ à valeurs dans $F$. Le fait que $\pi : \mathrm{Or}_M \to X$ soit étale et que $\pi^*(\tilde{\mathbf{R}}_M) = \mathrm{Or}_M \times \mathbf{R}$ permet d’identifier $\pi^*(\mathbf{R}_M \otimes \mathrm{Alt}^p(T(X); F))$ à $\mathrm{Alt}^p(T(\mathrm{Or}_M); \pi^*(F))$ et $\omega$ définit une section $\tilde{\omega}$ de $\mathrm{Alt}^p(T(\mathrm{Or}_M); \pi^*(F))$ (7.4.3), autrement dit, une forme différentielle de degré $p$ sur $\mathrm{Or}_M$ à valeurs dans $\pi^*(F)$. On obtient ainsi une bijection de l’espace des formes $M$-tordues de degré $p$ sur $X$ à valeurs dans $F$, sur l’espace des formes $\tilde{\omega}$ de degré $p$ sur $\mathrm{Or}_M$ à valeurs dans $\pi^*(F)$ telles que
$$
\tilde{\omega}(-\xi) = -\tilde{\omega}(\xi) \quad \text{pour tout } \xi \in \mathrm{Or}_M.
$$
Lorsque $M$ est muni d’une orientation $\xi$, l’application $\omega \mapsto \xi \otimes \omega$ permet d’identifier les sections de $\mathrm{Alt}^p(T(X); F)$ (autrement dit les formes différentielles de degré $p$ usuelles) aux formes $M$-tordues de degré $p$ à valeurs dans $F$.

10.3.4. Soit $\omega$ une forme différentielle $M$-tordue de degré $p$ sur $X$, à valeurs dans un espace de Banach $E$, et de classe $C^s$ ($1 \leq s \leq \inf(k, r-1)$). Il existe une forme différentielle $M$-tordue $d\omega$, de degré $p+1$ sur $X$, à valeurs dans $E$, et une seule telle que, quels que soient l’ouvert $U$ de $X$, l’orientation $\xi$ de $M|U$ et la forme différentielle $\alpha$ sur $U$ tels que $\omega|U = \xi \otimes \alpha$, on ait $d\omega|U = \xi \otimes d\alpha$. La forme $d\omega$ est de classe $C^{s-1}$; on l’appelle la différentielle extérieure de $\omega$.

Si l’on note $\tilde{\omega}$ (resp. $\tilde{d\omega}$) la forme différentielle sur $\mathrm{Or}_M$ correspondant à $\omega$ (resp. à $d\omega$) comme en 10.3.3, on a $d(\tilde{\omega}) = \tilde{d\omega}$.

Si $\zeta$ est un champ de vecteurs de classe $C^s$ sur $X$, on définit de manière analogue la forme $M$-tordue $\theta_\zeta.\omega$. On a
$$
\theta_\zeta.\omega = d(i(\zeta)\omega) + i(\zeta)d\omega
$$
et $\theta_\zeta.\omega$ est de classe $C^{s-1}$.

### 10.4. Mesure associée à une forme différentielle tordue

Rappelons que, dans ce numéro, on suppose $K = \mathbf{R}$ et que toutes les variétés considérées sont localement de dimension finie.

10.4.1. Soit X une variété de classe C'. On peut appliquer les définitions et résultats de 10.3 en prenant pour fibré vectoriel M le fibré tangent T(X). On a alors Or_M = $\tilde{X}$ (10.2.4); on note $\tilde{R}_X$ et on appelle simplement fibré des scalaires tordus le fibré $\tilde{R}_{T(X)}$ (10.3.1)[^2]; une forme différentielle T(X)-tordue à valeurs dans un fibré vectoriel F est appelée simplement une forme différentielle tordue (ou impaire) à valeurs dans F. Lorsque X est muni d'une orientation, l'application $\omega \mapsto \xi \otimes \omega$ permet d'identifier les formes différentielles usuelles (parfois appelées «paires») aux formes tordues.

10.4.2. Soit $f : X \to Y$ un morphisme de variétés de classe C' et soit $\tilde{f} : \tilde{X} \to \tilde{Y}$ une orientation de $f$ (10.2.5). Il existe un isomorphisme $j$ et un seul de $f^*(\tilde{R}_Y)$ sur $\tilde{R}_X$ tel que $\tilde{x} = j(\pi(\tilde{x}), \tilde{f}(\tilde{x}))$ pour tout $\tilde{x} \in \tilde{X}$. On identifie ces deux fibrés grâce à $j$. Si $\omega$ est une forme tordue de degré $p$ sur Y à valeurs dans un fibré vectoriel F, l'image réciproque $f^*(\omega)$ s'identifie à une forme différentielle tordue de degré $p$ sur X à valeurs dans $f^*(F)$. Si l'on note $\tilde{\omega}$ (resp. $\tilde{f}^*(\omega)$) la forme différentielle sur $\tilde{Y}$ (resp. $\tilde{X}$) correspondant à $\omega$ (resp. $f^*(\omega)$) comme en 10.3.3, on a $\tilde{f}^*(\tilde{\omega}) = \tilde{f}^*(\omega)$.

Lorsque F est le fibré trivial défini par un espace de Banach, l'opération $f^*$ commute à la différentiation extérieure (10.3.4).

10.4.3. Soit X une variété pure de dimension n, et soit $\omega$ une forme différentielle tordue de degré n sur X, à valeurs dans un espace de Banach E. Soit $c = (U, \varphi, \mathbf{R}^n)$ une carte de X et soit $\xi^n$ l'orientation canonique de $\mathbf{R}^n$; notons $u^1, \ldots, u^n$ les fonctions coordonnées sur $\mathbf{R}^n$. Il existe une fonction $f_c$ et une seule sur $\varphi(U)$, à valeurs dans E, telle que

$$
\omega|U = \varphi^*(\xi^n \otimes f_c . du^1 \wedge \cdots \wedge du^n).
$$

On dit que $\omega$ est localement intégrable si, pour toute carte $c = (U, \varphi, \mathbf{R}^n)$ de X, la fonction $f_c$ correspondante est localement intégrable par rapport à $\lambda_{\varphi(U)}^{\otimes n}$ (où $\lambda$ désigne la mesure de Lebesgue sur $\mathbf{R}$). Supposons que ce soit le cas et que X soit séparée. Il existe sur X une mesure vectorielle $\alpha(\omega)$ à valeurs dans E et une seule possédant la propriété suivante: pour toute carte $c = (U, \varphi, \mathbf{R}^n)$ de X, l'image par $\varphi$ de la restriction à U de la mesure $\alpha(\omega)$ est la mesure $f_c . \lambda_{\varphi(U)}^{\otimes n}$ (INT, VI, § 2, n° 4). On dit que $\alpha(\omega)$ est la mesure définie par $\omega$ et on la note le plus souvent simplement $\omega$. Le support de $\alpha(\omega)$ est contenu dans le support Supp $\omega$ de $\omega$ (en appelant support d'une forme différentielle $\omega$ l'adhérence de l'ensemble des $x \in X$ tels que $\omega(x) \neq 0$).

Si $f$ est une fonction réelle sur X, localement intégrable pour la mesure $\alpha(\omega)$, alors la forme différentielle $f \omega$ est localement intégrable et l'on a $\alpha(f \omega) = f . \alpha(\omega)$.

Si g est une fonction réelle sur X essentiellement intégrable pour $\alpha(\omega)$, son intégrale se note généralement $\int_X g \omega$, ou $\int g \omega$, ou $\int g(x) \omega(x)$; on évite de la noter $\int g \, d\omega$, à cause des risques de confusion avec la différentielle extérieure $d\omega$ de $\omega$, qui est définie (et d'ailleurs égale à 0) si $\omega$ est de classe $C^1$. Si A est une partie de X dont la fonction caractéristique $\varphi_A$ est essentiellement intégrable pour $\alpha(\omega)$, l'intégrale de $\varphi_A$ se note

∫_A ω. Si la constante 1 est essentiellement intégrable pour α(ω), on dit que ω est intégrable.

Soit maintenant p un entier, avec 0 ≤ p ≤ n, et soit ω une forme différentielle tordue de degré p sur X, à valeurs dans un espace de Banach E. Soit de plus Y une sous-variété pure de dimension p de X ; supposons que l’injection canonique i : Y → X soit munie d’une orientation. L’image réciproque i*(ω) (10.4.2) se note alors parfois ω|Y. Si ω|Y est intégrable, on pose

$$
\int_Y \omega = \int_Y \omega|Y.
$$

10.4.4. Soit X une variété pure de dimension n, munie d’une orientation ξ. L’identification ω ↦ ξ ⊗ ω entre formes différentielles usuelles et formes différentielles tordues permet d’appliquer ce qui précède aux formes de degré n sur X ; ainsi, à toute forme localement intégrable ω, de degré n, est associée une mesure sur X, notée encore ω. Si E = R, une telle forme ω est localement de module intégrable (10.1.5) et la mesure mod(ω)_μ correspondante (10.1.6) n’est autre que la valeur absolue |ω| de la mesure ω (INT, III, § 1, n° 6).

10.4.5. Exemple. — Soit X une variété réelle pure de dimension 1, orientée, séparée, et soit z : X → C une application différentiable de X dans C. La forme différentielle complexe dz définit sur X une mesure complexe également notée dz. Ceci s’applique notamment lorsque X est une sous-variété différentielle pure de dimension 1 de C, z étant l’injection de X dans C.

Plus particulièrement, prenons pour X un cercle de centre 0 et de rayon ρ > 0 ; orientons X comme indiqué dans 10.2.8, b), compte tenu de l’identification usuelle de C avec R² ; si x ∈ X, l’espace tangent T_x(X) s’identifie à la droite Rix de T_x(C) = C et l’orientation choisie est la demi-droite R_+ ix. Si f est une fonction continue sur X, à valeurs dans un espace de Banach complexe, l’intégrale de f pour la mesure dz est donnée par la formule

$$
\int_X f(z)\,dz = i\rho \int_0^{2\pi} f(\rho e^{i\alpha})\,e^{i\alpha}\,d\alpha.
$$

Par exemple, si n est un entier, on a

$$
\int_X z^n\,dz = i\rho^{n+1} \int_0^{2\pi} e^{(n+1)i\alpha}\,d\alpha = \begin{cases} 0 & \text{si } n \neq -1 \\ 2i\pi & \text{si } n = -1. \end{cases}
$$

10.4.6 (« Cas complexe »). Soit X^c une variété analytique complexe séparée, pure de dimension m, et soit ω une forme différentielle holomorphe de degré m sur X^c. Soit X la variété analytique réelle sous-jacente à X^c ; la forme ω s’identifie à une forme de type (m, 0) sur X (8.8.9) ; soit $\overline{\omega}$ sa conjuguée (8.8.2). La forme $i^{m^2} \omega \wedge \overline{\omega}$ est une forme différentielle réelle de degré 2m sur X ; compte tenu de l’orientation canonique de X (10.2.7), cette forme s’identifie à une mesure sur X, qui n’est autre que la mesure positive mod(ω)_μ définie en 10.1.6, où μ est la mesure définie par la forme différentielle $i\,dz\wedge d\bar z$, autrement dit le double de la mesure de Lebesgue $\lambda^{\otimes 2}$ sur $\mathbf{C}$ (identifié à $\mathbf{R}^2$ de la manière usuelle).

Soit H l’espace des formes holomorphes $\omega$ de degré $m$ sur $X^c$ telles que la mesure $\omega\wedge\bar\omega$ soit bornée. Pour $\alpha,\beta$ dans H, la mesure complexe $\alpha\wedge\bar\beta$ est bornée; en posant

$$
(\alpha|\beta)=i^{m^2}\int_X \alpha\wedge\bar\beta,
$$

on obtient une forme hermitienne sur H, qui fait de H un espace de Hilbert.

[^1]: Lorsque $K = \mathbf{R}$, il suffit de supposer que $r > \sup_{y \in Y} (\dim_{f(y)} X - \dim_y Y)$; cf. par exemple A. SARD, Bull. Am. Math. Soc., XLVIII (1943), p. 883–890.
[^2]: On prendra garde que cette notation est contradictoire avec la notation $\tilde{R}_M$ lorsque l'on considère X comme munie de sa structure de fibré vectoriel de rang 0 sur elle-même.
