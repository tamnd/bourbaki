---
book: var
book_title: Variétés différentielles et analytiques
chapter: "1"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 3
section_title: Fonctions analytiques réelles ou complexes
lang: fr
source: var-fr
pdf_pages: 0020-0028
extraction: ocr
subsections:
    - "no": 1
      title: Séries convergentes
      page: 0
      pdf_page: 20
    - "no": 2
      title: Fonctions analytiques
      page: 0
      pdf_page: 24
    - "no": 3
      title: Fonctions holomorphes
      page: 0
      pdf_page: 26
    - "no": 4
      title: Fonctions analytiques réelles
      page: 0
      pdf_page: 28
statements: 0
exercises: 0
content_sha256: cfe146e6a40be8be1b051f760f4e1533856f7696cddc3e4c6f58c02e159289ef
---

## § 3. Fonctions analytiques réelles ou complexes

Dans ce paragraphe, on suppose que $K = \mathbf{R}$ ou $\mathbf{C}$. On désigne par $(E_i),\ 1 \leq i \leq n$, une famille finie d’espaces normés sur $K$, par $E$ l’espace produit des $E_i$, et par $F$ un espace vectoriel topologique localement convexe séparé sur $K$.

### 3.1. Séries convergentes

3.1.1. Soit $f = \sum f_\alpha$ une série formelle appartenant à $\hat{P}(E_1, \ldots, E_n; F)$ (App., n° A.5). Si $\gamma$ est une semi-norme continue sur $F$ et $R = (R_1, \ldots, R_n)$ une suite de $n$ nombres réels strictement positifs, on pose :

$$
\|f\|_{\gamma, R} = \sum_\alpha R^\alpha \|f_\alpha\|_\gamma.
$$

Si $F$ est un espace normé et si $\gamma$ est la norme de $F$, on écrit $\|f\|_R$ au lieu de $\|f\|_{\gamma, R}$.

L’ensemble $\mathcal{H}_R(E_1, \ldots, E_n; F)$ des $f \in \hat{P}(E_1, \ldots, E_n; F)$ telles que $\|f\|_{\gamma, R}$ soit fini pour toute semi-norme continue $\gamma$ sur $F$ est un sous-espace vectoriel de $\hat{P}(E_1, \ldots, E_n; F)$. On a

$$
\mathcal{H}_R(E_1, \ldots, E_n; F) \subset \mathcal{H}_{R'}(E_1, \ldots, E_n; F)
$$

toutes les fois que $R_i \geq R'_i$ pour $1 \leq i \leq n$. La réunion des

$$
\mathcal{H}_R(E_1, \ldots, E_n; F)
$$

est un sous-espace vectoriel, noté $\mathcal{H}(E_1, \ldots, E_n; F)$, de $\hat{P}(E_1, \ldots, E_n; F)$, dont les éléments sont appelés séries convergentes sur le produit des $E_i$, à valeurs dans $F$. Il ne dépend que de la topologie des $E_i$ et non de leurs normes. On peut donc parler de l’espace $\mathcal{H}(E_1, \ldots, E_n; F)$ lorsque les $E_i$ sont des espaces normables, sans avoir à choisir une norme sur chaque $E_i$.

3.1.2. L’application $f \mapsto \|f\|_{\gamma, R}$ est une semi-norme sur $\mathcal{H}_R(E_1, \ldots, E_n; F)$. La topologie que définissent ces semi-normes lorsque $\gamma$ décrit l’ensemble des semi-normes continues sur $F$ (ou simplement un ensemble de semi-normes définissant la topologie de $F$) est séparée. Si $F$ est normable (resp. complet), il en est de même de $\mathcal{H}_R(E_1, \ldots, E_n; F)$. Les semi-normes sur $\mathcal{H}(E_1, \ldots, E_n; F)$ dont la restriction à chaque $\mathcal{H}_R$ est continue définissent une topologie séparée sur $\mathcal{H}(E_1, \ldots, E_n; F)$, qui ne dépend que des topologies des $E_i$. L’injection de $\mathcal{H}(E_1, \ldots, E_n; F)$ dans $\hat{P}(E_1, \ldots, E_n; F)$ est continue.

3.1.3. L’isomorphisme canonique de $\hat{P}(E; F)$ sur $\hat{P}(E_1, \ldots, E_n; F)$ donne par restriction un isomorphisme d’espaces vectoriels topologiques de $\mathcal{H}(E; F)$ sur $\mathcal{H}(E_1, \ldots, E_n; F)$.

3.1.4. Soit $f \in \mathcal{H}(E_1, \ldots, E_n; F)$ et soit $J(f)$ l’ensemble des $R \in (\mathbf{R}_+^*)^n$ tels que $f \in \mathcal{H}_R(E_1, \ldots, E_n; F)$. L’intérieur $I(f)$ de $J(f)$ s’appelle l’indicatrice de convergence stricte de $f$. Il se compose de l’ensemble des $R$ pour lesquels il existe un $R' \in J(f)$ avec $0 < R_i < R'_i$ pour $1 \leq i \leq n$. On note $\Omega(f)$ l’ensemble des points $(\log R_1, \ldots, \log R_n)$ de $\mathbf{R}^n$ pour $R \in I(f)$: c’est une partie convexe de $\mathbf{R}^n$.

Lorsque $n = 1$, l’ensemble $I(f)$ est un intervalle $]0, \rho(f)[$ de $\mathbf{R}$ et $\rho(f)$ s’appelle le rayon de convergence strict de $f$. C’est aussi la borne supérieure (finie ou $+\infty$) de l’ensemble des nombres réels $R > 0$ tels que pour toute semi-norme continue $\gamma$ sur $F$, il existe une constante $M$ telle que $\|f_m\|_{\gamma} \leq MR^{-m}$ (avec $f = \sum f_m, f_m \in P_m(E; F)$) pour tout entier $m \geq 0$.

L’ensemble des points $x = (x_i) \in E_1 \times \cdots \times E_n$ tels qu’il existe $R \in I(f)$ avec $\|x_i\| \leq R_i$ pour tout $i$, s’appelle le domaine de convergence strict de $f$ et se note $C(f)$. C’est aussi l’intérieur de l’ensemble des points $x$ pour lesquels il existe $R \in J(f)$ avec $\|x_i\| < R_i$ pour tout $i$.

3.1.5. Pour $f_\alpha \in P_\alpha(E_1, \ldots, E_n; F)$ et pour toute semi-norme continue $\gamma$ sur $F$, posons :
$$
\|f_\alpha\|_{\gamma} = \sup_{\|x_i\| \leq 1} \|f_\alpha(x_1, \ldots, x_n)\|_{\gamma}.
$$
On a alors les inégalités :
$$
\|f_\alpha\|_{\gamma} \leq \|f_\alpha\|_{\gamma'} \leq \frac{\alpha^\alpha}{\alpha!} \|f_\alpha\|_{\gamma}.
$$
Pour $f = \sum f_\alpha \in \hat{P}(E_1, \ldots, E_n; F)$ et $R \in (\mathbf{R}_+^*)^n$, posons :
$$
\|f\|_{\gamma, R} = \sum_\alpha R^\alpha \|f_\alpha\|_{\gamma}
$$
et désignons par $\tilde{\mathcal{H}}_R(E_1, \ldots, E_n; F)$ le sous-espace vectoriel de $\hat{P}(E_1, \ldots, E_n; F)$
formé des $f$ tels que $\|f\|_{\gamma, R}$ soit fini pour tout $\gamma$, muni de la topologie définie par les semi-normes $f \mapsto \|f\|_{\gamma, R}$. On a $\mathcal{H}_R \subset \tilde{\mathcal{H}}_R$ et l’injection de $\mathcal{H}_R$ dans $\tilde{\mathcal{H}}_R$ est continue. L’espace $\mathcal{H}(E_1, \ldots, E_n; F)$ est la réunion des $\tilde{\mathcal{H}}_R(E_1, \ldots, E_n; F)$ et sa topologie est la topologie localement convexe la plus fine qui rende continues les injections des $\mathcal{H}_R$ dans $\mathcal{H}$.

Si $f \in \mathcal{H}(E_1, \ldots, E_n; F)$, on appelle indicatrice de convergence l’intérieur $\tilde{I}(f)$ de l’ensemble $\tilde{J}(f)$ des $R \in (\mathbf{R}_+^*)$ tels que $f \in \tilde{\mathcal{H}}_R$. On a :
$$
e^{-1}\tilde{I}(f) \subset I(f) \subset \tilde{I}(f)
$$
(où $e$ est la base des logarithmes népériens). A partir de $\tilde{I}(f)$, on définit comme en 3.1.4. le domaine de convergence $\tilde{C}(f)$ et, lorsque $n = 1$, le rayon de convergence $\tilde{\rho}(f)$. On a en particulier :
$$
e^{-1}\tilde{\rho}(f) \leq \rho(f) \leq \tilde{\rho}(f).
$$

3.1.6. Pour $R \in (\mathbf{R}_+^*)^n$, on appelle polyboule (fermée) de centre 0 et de rayon $R$ de $E$ l’ensemble $B(R)$ des $x \in E$ tels que $\|x_i\| \leq R_i$ pour tout $i$. Si $\dim E_i = 1$, on dit aussi polydisque. Si $f \in \mathcal{H}(E_1, \ldots, E_n; F)$, le domaine de convergence (resp. strict) de $f$ est la réunion des polyboules $B(R)$ pour $R \in \tilde{I}(f)$ (resp. $R \in I(f)$).

3.1.7. Soit $f \in \mathcal{H}(E_1, \ldots, E_n; F)$. Supposons $F$ quasi-complet. Pour tout $x \in \tilde{C}(f)$, la famille des $f_a(x)$ est sommable dans $F$. Sa somme, notée $\hat{f}(x)$ ou simplement $f(x)$, est une fonction continue sur $\tilde{C}(f)$. Plus précisément, pour tout $R$ tel que $f \in \tilde{\mathcal{H}}_R$, la famille des $f_a(x)$ est uniformément sommable pour $x \in B(R)$. L’application $f \mapsto \hat{f}$ est une application linéaire continue injective de $\tilde{\mathcal{H}}_R$ dans l’espace des fonctions continues bornées sur $B(R)$, muni de la topologie de la convergence uniforme.

3.1.8. Soient $F_1, \ldots, F_m$ des espaces polynormés séparés et soit $u$ une application $m$-linéaire continue de $F_1 \times \cdots \times F_m$ dans $F$. Soient $f_i \in \mathcal{H}(E_1, \ldots, E_n; F_i)$ pour $1 \leq i \leq m$. La série formelle $u(f_1, \ldots, f_m)$ appartient à $\mathcal{H}(E_1, \ldots, E_n; F)$. On a:

$$
C(u(f_1, \ldots, f_m)) \supset \bigcap_i C(f_i)
$$
$$
\tilde{C}(u(f_1, \ldots, f_m)) \supset \bigcap_i \tilde{C}(f_i)
$$

et si $x \in \bigcap_i \tilde{C}(f_i)$, $F$ et les $F_i$ étant quasi-complets, on a:
$$
u(f_1, \ldots, f_m)(x) = u(f_1(x), \ldots, f_m(x)).
$$

3.1.9. Soient $F_1, \ldots, F_m$ des espaces normés complets et supposons $F$ quasi-complet. Soient $f = (f_i)_{1 \leq i \leq m}$ avec $f_i \in \mathcal{H}(E_1, \ldots, E_n; F_i)$ et $g \in \mathcal{H}(F_1, \ldots, F_m; F)$, tels que $(f_i(0))_{1 \leq i \leq m}$ appartienne au domaine de convergence strict de $g$. Alors, pour tout $\alpha \in \mathbf{N}^m$, la série formelle $g_\alpha \circ f$ appartient à $\mathcal{H}(E_1, \ldots, E_n; F)$ et la famille des $g_\alpha \circ f$ est sommable dans $\mathcal{H}(E_1, \ldots, E_n; F)$ et $a fortiori$ dans $\hat{P}(E_1, \ldots, E_n; F)$. Sa somme sera notée $g \circ f$.

De manière plus précise, il existe $R \in \bigcap_i I(f_i)$ et $R' \in I(g)$ tels que $\|f_i\|_R < R'_i$ pour $1 \leq i \leq m$. Sous ces conditions, la série formelle $g_\alpha \circ f$ appartient à $\mathcal{H}_R(E_1, \ldots, E_n; F)$, et la famille des $g_\alpha \circ f$ est sommable dans $\mathcal{H}_R(E_1, \ldots, E_n; F)$. Enfin, si $x \in B(R)$, alors $f(x) = (f_i(x))$ appartient à $B(R') \subset F_1 \times \cdots \times F_m$ et on a:
$$
g(f(x)) = (g \circ f)(x).
$$

3.1.10. Supposons que $E_i = K$ pour $1 \leq i \leq n$. L’espace $\hat{P}(K^n; F)$ s’identifie alors à l’espace des séries formelles à $n$ indéterminées $X_1, \ldots, X_n$ à coefficients dans $F$ et un élément de $\hat{P}(K^n; F)$ s’écrit :

$$
f = \sum_{\alpha} X^\alpha c_\alpha \quad \text{avec } c_\alpha \in F.
$$

Si $R \in (\mathbf{R}_+^*)^n$ et si $\gamma$ est une semi-norme continue sur $F$, on a :

$$
\| f \|_{\gamma, R} = \| f \|_{\gamma, R} = \sum_{\alpha} R^\alpha \| c_\alpha \|_\gamma
$$

On a $I(f) = \tilde{I}(f)$, $C(f) = \tilde{C}(f)$ et, lorsque $n = 1$, $\rho(f) = \tilde{\rho}(f)$.

L’espace $\mathcal{H}(K^n; K)$ des séries convergentes à coefficients dans $K$ se note aussi $K\{(X_1, \ldots, X_n)\}$; c’est une sous-algèbre de $K[[X_1, \ldots, X_n]]$. L’espace $\mathcal{H}(K^n; F)$ est un module sur $K\{(X_1, \ldots, X_n)\}$ et si $F$ est de dimension finie, ce module s’identifie à $K\{(X_1, \ldots, X_n)\} \otimes_K F$.

3.1.11. Soit $f \in \mathcal{H}(K^n; K^m)$, représenté par un système de $m$ séries convergentes $f_j(X_1, \ldots, X_n)$, à coefficients dans $K$. Soit de même $g \in \mathcal{H}(K^m; K^p)$, représenté par un système de $p$ séries convergentes $g_k(Y_1, \ldots, Y_m) = \sum g_{k,\beta} Y^\beta$. L’élément $h = g \circ f$ de $\mathcal{H}(K^n; K^p)$ (cf. 3.1.9) est représenté par $p$ séries formelles $h_k(X_1, \ldots, X_n)$, déterminées comme suit : pour $\alpha \in \mathbf{N}^n$ et $\beta \in \mathbf{N}^m$, soit $c_{\alpha,\beta}$ le coefficient de $X^\alpha$ dans la série formelle $f^\beta = \prod f_j^{\beta_j}$; alors la famille $(g_{k,\beta} c_{\alpha,\beta})_{\beta \in \mathbf{N}^m}$ est sommable dans $K$ et a pour somme le coefficient de $X^\alpha$ dans $h_k$.

3.1.12. Supposons $F$ quasi-complet et soit $\hat{E}_i$ le complété de $E_i$. Tout polynôme-continu sur $E_1 \times \cdots \times E_n$ à valeurs dans $F$ se prolonge par continuité en un polynôme-continu sur $\hat{E}_1 \times \cdots \times \hat{E}_n$, à valeurs dans $F$. On en déduit une bijection $j$ de $\hat{P}(E_1, \ldots, E_n; F)$ sur $\hat{P}(\hat{E}_1, \ldots, \hat{E}_n; F)$. Si $f \in \mathcal{H}(E_1, \ldots, E_n; F)$, alors $j(f) \in \mathcal{H}(\hat{E}_1, \ldots, \hat{E}_n; F)$ et réciproquement. Les indicatrices de convergence strictes de $f$ et de $j(f)$ sont les mêmes.

3.1.13. On suppose que $K = \mathbf{R}$, mais que $F$ est muni d’une structure d’espace vectoriel complexe compatible avec sa structure d’espace vectoriel réel. Soit $E_i^C = E_i \otimes_\mathbf{R} \mathbf{C}$. Si $y \in E_i^C$, posons

$$
y = \inf \sum_k |a_k| \cdot \| x_k \|,
$$

la borne inférieure étant étendue à toutes les familles finies de couples $(x_k, a_k) \in E_i \times \mathbf{C}$ telles que $y = \sum_k x_k \otimes a_k$. On obtient ainsi une norme sur l’espace vectoriel complexe $E_i^C$; cette norme prolonge la norme donnée sur $E_i$ si l’on convient d’identifier $x \in E_i$ à $x \otimes 1$. Soit $h$ un $\mathbf{R}$-polynôme-continu sur $E_1 \times \cdots \times E_n$, à valeurs dans $F$, et homogène de multidegré $\alpha$; il existe alors un $\mathbf{C}$-polynôme-continu $\tilde{h}$ sur $E_1^C \times \cdots \times E_n^C$, et un seul, à valeurs dans $F$, prolongeant $h$, et homogène de multidegré $\alpha$. On a

$$
\| \tilde{h} \|_\gamma = \| h \|_\gamma
$$

pour toute semi-norme continue $\gamma$ sur l’espace vectoriel complexe $F$.

Si $f = \sum_{\alpha} f_{\alpha} \in \mathcal{H}(E_1, \ldots, E_n; F)$, alors $\tilde{f} = \sum_{\alpha} \tilde{f}_{\alpha} \in \mathcal{H}(E_1^c, \ldots, E_n^c; F)$. Les séries $f$ et $\tilde{f}$ ont même indicatrice de convergence stricte (et même rayon de convergence strict lorsque $n = 1$).

Inversement, supposons $K = C$. Soient $E_i^0$ et $F^0$ les espaces sur $\mathbf{R}$ obtenus par restriction des scalaires. Si $f_{\alpha} \in P_{\alpha}(E_1, \ldots, E_n; F)$, alors $f_{\alpha} \in P_{\alpha}(E_1^0, \ldots, E_n^0; F^0)$. Si $f = \sum_{\alpha} f_{\alpha} \in \mathcal{H}(E_1, \ldots, E_n; F)$, alors la série formelle $f^0 = \sum_{\alpha} f_{\alpha} \in \hat{P}(E_1^0, \ldots, E_n^0; F^0)$ est une série convergente. Les indicatrices de convergence (resp. les indicatrices de convergence strictes) de $f$ et $f^0$ sont identiques et on a $f(x) = f^0(x)$ pour tout $x \in \bar{C}(f) = \bar{C}(f^0)$.

### 3.2. Fonctions analytiques

3.2.1. Soient $U$ un ouvert de $E$ et $f$ une application de $U$ dans $F$. On dit que $f$ est *de classe* $C^{\omega}$, ou *K-analytique* (ou simplement *analytique*) dans $U$ si, pour tout point $a$ de $U$, il existe une série convergente $f_{\alpha} \in \mathcal{H}(E; F)$ telle que $f(a + x) = f_{\alpha}(x)$ pour tout $x$ dans $E$ assez voisin de zéro. Si $K = \mathbf{R}$ (resp. $\mathbf{C}$), on dit encore que $f$ est *analytique réelle* (resp. *analytique complexe* ou *holomorphe*). Les applications analytiques de $U$ dans $F$ forment un sous-espace vectoriel, noté $\mathcal{C}^{\omega}(U; F)$, de l’espace de toutes les applications de $U$ dans $F$.

Pour $a \in U$, la série formelle $f_{\alpha}$ est unique : on l’appelle le *développement en série entière* de $f$ au point $a$. Si $f_{\alpha} = \sum_{\alpha} (f_{\alpha})_{\alpha}$ (avec $(f_{\alpha})_{\alpha} \in P_{\alpha}(E_1, \ldots, E_n; F)$), on pose :

$$
\Delta^{\alpha} f(a) = (f_{\alpha})_{\alpha}.
$$

3.2.2. Si $f \in \mathcal{C}^{\omega}(U; F)$, l’application $\Delta^{\alpha} f : a \mapsto \Delta^{\alpha} f(a)$ de $U$ dans

$$
P_{\alpha}(E_1, \ldots, E_n; F)
$$

est analytique. L’application $\Delta^{\alpha} : f \mapsto \Delta^{\alpha} f$ est une application $K$-linéaire de $\mathcal{C}^{\omega}(U; F)$ dans $\mathcal{C}^{\omega}(U; P_{\alpha}(E_1, \ldots, E_n; F))$. Pour $a \in U$, on a donc, pour $\alpha, \beta \in \mathbf{N}^n$, $\Delta^{\beta}(\Delta^{\alpha} f)(a) \in P_{\beta}(E_1, \ldots, E_n; P_{\alpha}(E_1, \ldots, E_n; F))$. Si $x = (x_i) \in E$, on a donc $(\Delta^{\beta}(\Delta^{\alpha} f)(a))(x) \in P_{\alpha}(E_1, \ldots, E_n; F)$ et $((\Delta^{\beta}(\Delta^{\alpha} f)(a))(x))(x) \in F$. Cet élément de $F$ est égal à $((\alpha, \beta))(\Delta^{\alpha+\beta} f(a))(x)$. On exprime ceci en écrivant :

$$
\Delta^{\beta} \circ \Delta^{\alpha} = ((\alpha, \beta)) \Delta^{\alpha+\beta}.
$$

3.2.3. Les indicatrices de convergence strictes (et les rayons de convergence stricts lorsque $n = 1$) des développements en série entière de $f$ et de $\Delta^{\alpha} f$ en un même point $a$ de $U$, sont identiques.

3.2.4. Soit $f \in \mathcal{C}^\omega(U; F)$. Alors $f$ est strictement dérivable et indéfiniment dérivable dans $U$ (si $K = \mathbf{R}$, $f$ est de classe $C^\infty$ dans $U$). Les dérivées itérées de $f$ sont analytiques, et leurs valeurs en un point $a$ sont des applications multilinéaires symétriques. On peut alors introduire la notation $D^\alpha f$ pour les dérivées partielles itérées comme au n° 2.4.2. On a :

$$
\alpha! \Delta^\alpha f(a)(h) = D^\alpha f(a) . (h, \ldots, h)
$$

quels que soient $a \in U$ et $h \in E$, ce qu’on écrit :

$$
\alpha! \Delta^\alpha f = D^\alpha f .
$$

3.2.5. Soient $U$ un ouvert de $E$ et $f, g$ deux applications analytiques de $U$ dans $F$. Soit $a \in U$. Pour que $f$ et $g$ aient un contact d’ordre $\geq k$ en $a$, il faut et il suffit que $\Delta^\alpha f(a) = \Delta^\alpha g(a)$ pour tout $\alpha$ avec $|\alpha| \leq k$. Si $f$ et $g$ ont un contact d’ordre infini en $a$, elles sont égales dans un voisinage de $a$. L’ensemble des points de $U$ où $f$ et $g$ ont un contact d’ordre infini est ouvert et fermé.

En particulier, si $U$ est connexe et s’il existe une partie ouverte non vide de $U$ sur laquelle $f$ et $g$ sont égales, on a $f = g$ (« principe du prolongement analytique »).

3.2.6. Soient $U$ un ouvert de $E$ et $f$ une application analytique de $U$ dans $F$. Si la dérivée $Df$ de $f$ est nulle, $f$ est localement constante.

3.2.7. Supposons $F$ quasi-complet et soit $G$ un espace normé complet. Soit $g$ une application analytique d’un ouvert $U$ de $E$ dans $G$ et soit $f$ une application analytique d’un ouvert $V$ de $G$, contenant $g(U)$, dans $F$. L’application composée $f \circ g$ est analytique dans $U$. Supposons en outre que $0 \in U$ et que $g(0) = 0$. Le développement de $f \circ g$ en série entière en $0$ s’obtient alors en substituant, dans le développement de $f$ en $0$, le développement en série entière de $g$ en $0$ (3.1.9).

3.2.8. Soient $F_1, \ldots, F_m$ des espaces polynormés séparés et $u$ une application multilinéaire continue de $F_1 \times \cdots \times F_m$ dans $F$. Soient $U$ un ouvert de $E$ et $f_i \in \mathcal{C}^\omega(U; F_i)$. La fonction $u(f_1, \ldots, f_m)$ est analytique, et son développement en série entière en un point $a \in U$ est la série $u((f_1)_a, \ldots, (f_m)_a)$ (3.1.8).

3.2.9. On suppose $F$ quasi-complet. Soit $f \in \mathcal{H}(E_1, \ldots, E_n; F)$; la fonction $x \mapsto f(x)$ (3.1.7) est analytique dans l’ouvert $C(f)$, domaine de convergence strict de $f$. Si $n = 1$ et si $\|a\| < \rho(f)$, le rayon de convergence strict du développement de $f$ en série entière en $a$ est au moins égal à $\rho(f) - \|a\|$. Si $\rho(f) = + \infty$, on dit que $f$ est une fonction entière.

3.2.10. Gardons les hypothèses de 3.2.9. Si $K = \mathbf{C}$, les résultats de 3.2.9 restent exacts si l’on remplace $C(f)$ par $\tilde{C}(f)$ et $\rho(f)$ par $\tilde{\rho}(f)$ (pour $n = 1$). Si $K = \mathbf{R}$, la fonction $x \mapsto f(x)$ est analytique dans $\tilde{C}(f)$.

3.2.11. Supposons que $E_i = K$ pour $1 \leq i \leq n$. Soient $U$ un ouvert de $K^n$ et $f \in \mathcal{C}^\omega(K^n; F)$. Si $0 \in U$ et si $f_0 = \sum_\alpha X^\alpha c_\alpha$ est le développement en série entière de $f$ en $0$, le développement en série entière de $\Delta^\alpha f$ en $0$ s’écrit (après identification de $P_\alpha(K^n; F)$ avec $F$):

$$
(\Delta^\alpha f)_0 = \sum_\beta ((\alpha, \beta)) X^\beta c_{\alpha + \beta}.
$$

On a en particulier pour $1 \leq i \leq n$ et pour $x \in C(f_0)$:

$$
\partial_i f(x) = \sum_\alpha (\alpha_i + 1) x^\alpha c_{\alpha + e_i}.
$$

### 3.3 Fonctions holomorphes

Dans ce n°, on suppose que $K = \mathbf{C}$.

3.3.1. On suppose $F$ quasi-complet. Soient $U$ un ouvert de $E$ et $f$ une application de $U$ dans $F$. Les conditions suivantes sont équivalentes:
(i) $f$ est holomorphe;
(ii) $f$ est dérivable;
(iii) $f$ est localement bornée et quels que soient $a \in U$ et $h \in E$, la fonction $t \mapsto f(a + th)$, définie dans un voisinage ouvert de $0$ dans $C$, est holomorphe;
(iv) $f$ est localement bornée et pour toute forme linéaire continue $u$ sur $F$, la fonction $u \circ f$ à valeurs dans $\mathbf{C}$ est holomorphe;
(v) $f$ est continue et localement bornée et il existe un ensemble total $H$ du dual de $F$ tel que $u \circ f$ soit holomorphe pour tout $u \in H$.

Lorsque $E$ est de dimension finie (resp. lorsque $F$ est un espace de Banach), ces conditions sont encore équivalentes aux conditions (iii'), (iv') ou (v') (resp. (iv') ou (v')) obtenues à partir de (iii), (iv) ou (v) (resp. (iv) ou (v)) en enlevant l’hypothèse « $f$ est localement bornée ».

3.3.2. Supposons $F$ quasi-complet. Soient $U$ un ouvert de $E$ et $(f_n)$ une suite d’applications holomorphes de $U$ dans $F$, possédant la propriété suivante:
(W) Tout point de $U$ possède un voisinage dans lequel la suite $(f_n)$ converge uniformément.
Alors la limite $f$ de la suite $(f_n)$ est holomorphe, la suite des dérivées $(Df_n)$ (à valeurs dans l’espace quasi-complet $\mathcal{L}(E; F)$) possède la propriété (W) et $Df$ est la limite de $(Df_n)$.

3.3.3. Soient U un ouvert de E et f une application holomorphe de U dans F, supposé quasi-complet. Soit $R = (R_i) \in (\mathbf{R}_+^*)^n$ et supposons que la polyboule B(R) est contenue dans U et que f est bornée sur B(R). On a alors, pour tout $α \in \mathbf{N}^n$ et tout $x = (x_i) \in B(R)$:

$$
Δ^αf(0)(x) = \int_0^1 \cdots \int_0^1 f(e(\theta_1)x_1, \ldots, e(\theta_n)x_n)e(-α_1θ_1 - \cdots - α_nθ_n)\ dθ_1 \ldots dθ_n
$$

(avec $e(θ) = \exp 2πi θ$).

Soit de plus $γ$ une semi-norme continue sur F et soit M la borne supérieure de $\|f(x)\|_γ$ pour $\|x_i\| = R_i$. On a $\|Δ^αf(0)(x)\|_γ \leq M$ pour tout $x \in B(R)$ et $\|Δ^αf(0)\|_γ \leq MR^{-α}$. Enfin, le domaine de convergence du développement en série de f en 0 contient l'intérieur de la polyboule B(R).

3.3.4. Gardons les hypothèses de 3.3.3 et supposons de plus que $E_i = \mathbf{C}$. Soit $\sum_{α} X^αc_α$ le développement en série de f en 0. On a:

$$
c_α = R^{-α}\int_0^1 \cdots \int_0^1 f(e(\theta_1)R_1, \ldots, e(\theta_n)R_n)e(-α_1θ_1 - \cdots - α_nθ_n)\ dθ_1 \ldots dθ_n
$$

et:

$$
\|c_α\|_γ \leq R^{-α} \sup_{x \in B(R)} \|f(x)\|_γ
$$

(« inégalités de Cauchy »). Le domaine de convergence strict de la série $\sum_{α} X^αc_α$ contient l'intérieur de B(R).

3.3.5. Supposons E de dimension finie et F quasi-complet. Soit f une application holomorphe de E dans F. Il existe alors dans $\mathscr{H}(E; F)$ une série $f_0$ et une seule, de rayon de convergence infini (pour toute norme sur E), telle que $f(x) = f_0(x)$ pour tout $x \in E$.

3.3.6. Si f est une application holomorphe de E dans F telle que $f(E)$ soit borné, alors la fonction f est constante (« théorème de Liouville »).

3.3.7. On suppose que $E \neq 0$. Soit f une application holomorphe d'un ouvert U de E dans F. Soient a un point de U et $γ$ une semi-norme continue sur F. Pour tout voisinage V de a, contenu dans U, il existe $x \in V, x \neq a$, tel que:

$$
\|f(a)\|_γ \leq \|f(x)\|_γ.
$$

Si de plus $F = \mathbf{C}$ et si f n'est pas constante au voisinage de a, on a $|f(a)| < \sup_{x \in V, x \neq a} |f(x)|$ et l'application f est ouverte au voisinage de a.

Enfin, soit B un ouvert borné d'adhérence contenue dans U et soit B' sa frontière. On a:

$$
\sup_{x \in \overline{B}} |f(x)| = \sup_{x \in B'} |f(x)|
$$

(« principe du maximum »).

3.3.8. Supposons E de dimension finie. Soient U un ouvert de E, S un sous-espace vectoriel de codimension $\geq 2$ de E et $f$ une application holomorphe de $U \cap (E - S)$ dans F. Alors $f$ se prolonge par continuité en une application holomorphe de U dans F.

3.3.9. Supposons que $E = \mathbf{C}$ et soit $0 \leq \lambda < \mu \leq +\infty$. Soit $f$ une application holomorphe de l’ouvert $U = \{ z \in \mathbf{C} | \lambda < |z| < \mu \}$ dans F. Il existe une famille $(a_n(f))_{n \in \mathbf{Z}}$ et une seule d’éléments de F telle que, pour tout compact H de U, la famille $(a_n(f)z^n)_{n \in \mathbf{Z}}$ soit uniformément sommable de somme $f(z)$ pour $z$ décrivant H (« développement de Laurent »).

Supposons de plus $\lambda = 0$. On appelle ordre de $f$ au point $x = 0$ la borne inférieure (finie ou infinie) de l’ensemble des entiers $n$ tels que $a_n(f) \neq 0$. S’il existe un voisinage V de 0 tel que $f$ soit bornée dans $V - \{0\}$, alors $f$ est d’ordre 0 au point $x = 0$ et se prolonge par continuité en une fonction holomorphe sur l’ouvert $|z| < \mu$. Soit $p$ un entier $> 0$; si $f$ est d’ordre $-p$ au point $x = 0$, on dit que 0 est un pôle d’ordre $p$ de $f$.

3.3.10. Supposons que $E = \mathbf{C}$ et que F soit normé. Soit $f$ une application holomorphe du disque unité ouvert U de E dans F, telle que $f(0) = 0$ et soit $M = \sup_{z \in U} \|f(z)\|$. On a alors $\|f(z)\| \leq M \cdot |z|$ pour tout $z \in U$ (« lemme de Schwarz »).

### 3.4. Fonctions analytiques réelles

Supposons que $K = \mathbf{R}$.

3.4.1. Soient U un ouvert de E et $f$ une application de U dans F, supposé quasi-complet.

Les conditions suivantes sont équivalentes:
(i) $f$ est analytique.
(ii) $f$ est de classe $C^\infty$ et, pour tout $a \in U$, il existe un voisinage $V_a$ de $a$ et un nombre réel $M$ tels que, pour toute semi-norme $\gamma$ continue sur F, il existe une constante $A_\gamma$ telle que l’on ait
$$
\|\Delta^\alpha f(x)\|_\gamma \leq A_\gamma M^{|\alpha|} \quad \text{pour tout } x \in V_a \text{ et tout } \alpha \in \mathbf{N}^n.
$$

3.4.2. Soient U un ouvert de E et $f$ une application de U dans F. Si F est quasi-complet, et si son dual fort $F'$ est un espace de Baire, alors $f$ est analytique si et seulement si $u \circ f$ est analytique pour tout $u \in F'$.
