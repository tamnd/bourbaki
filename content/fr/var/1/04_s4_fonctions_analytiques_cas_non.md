---
book: var
book_title: Variétés différentielles et analytiques
chapter: "1"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 4
section_title: Fonctions analytiques (cas non archimédien)
lang: fr
source: var-fr
pdf_pages: 0029-0032
extraction: ocr
subsections:
    - "no": 1
      title: Séries convergentes
      page: 0
      pdf_page: 29
    - "no": 2
      title: Fonctions analytiques
      page: 0
      pdf_page: 31
    - "no": 3
      title: Quelques inégalités
      page: 0
      pdf_page: 32
statements: 0
exercises: 0
content_sha256: 6c33d48ae550ea870abdc7669dc0ffa3b18d55302bafba43eeb9d2a04fcc67f0
---

## § 4. Fonctions analytiques (cas ultramétrique)

Dans ce paragraphe, on suppose que la valeur absolue de K est ultramétrique. On désigne par $(E_i)_{1 \leq i \leq n}$ une famille finie d’espaces normés sur K, et par E l’espace produit des $E_i$, muni de la norme:

$$
\|x\| = \sup \|x_i\| \quad \text{si } x = (x_i).
$$

On désigne par F un espace polynormé séparé sur K.

### 4.1. Séries convergentes

4.1.1. Soit $f = \sum_a f_a$ une série formelle appartenant à $\hat{P}(E_1, \ldots, E_n; F)$, (cf. Appendice). Si $\gamma$ est une semi-norme continue sur F, et $R = (R_i)$ est un système de $n$ nombres réels $> 0$, on pose

$$
\|f\|_{\gamma, R} = \sup_a \|f_a\|_\gamma R^\alpha.
$$

Les définitions et les résultats du n° 3.1.1 (deuxième alinéa) et du n° 3.1.2 s’appliquent sans changement ; on définit en particulier les espaces

$$
\mathcal{H}_R(E_1, \ldots, E_n; F) \quad \text{et} \quad \mathcal{H}(E_1, \ldots, E_n; F).
$$

4.1.2. L’isomorphisme canonique $j$ de $\hat{P}(E; F)$ sur $\hat{P}(E_1, \ldots, E_n; F)$ donne, par restriction, un isomorphisme d’espaces vectoriels topologiques de $\mathcal{H}_R(E; F)$ sur $\mathcal{H}_{(R, \ldots, R)}(E_1, \ldots, E_n; F)$ pour tout $R \in \mathbf{R}_+^*$; il donne également un isomorphisme de $\mathcal{H}(E; F)$ sur $\mathcal{H}(E_1, \ldots, E_n; F)$. Plus précisément, si $f = \sum_m f_m \in \hat{P}(E; F)$ et si $j(f) = \sum_a f_a$, on a, pour toute semi-norme continue $\gamma$ sur F :

$$
\|f_m\|_\gamma = \sup_{|\alpha|=m} \|f_\alpha\|_\gamma
$$
$$
\|f\|_{\gamma, R} = \|j(f)\|_{\gamma, (R, \ldots, R)}.
$$

4.1.3. Soit $f = \sum_a f_a$ un élément de $\mathcal{H}(E_1, \ldots, E_n; F)$; soit $I(f)$ l’ensemble des $R \in (\mathbf{R}_+^*)^n$ tels que, pour toute semi-norme continue $\gamma$ sur F, le produit $\|f_\alpha\|_\gamma R^\alpha$ tende vers zéro quand $|\alpha|$ tend vers l’infini. L’ensemble $I(f)$ est non vide ; on l’appelle l’indicatrice de convergence stricte de $f$. L’ensemble $\Omega(f)$ des points

$$(\log R_1, \ldots, \log R_n) \quad \text{pour } R \in I(f)$$

est une partie convexe de $\mathbf{R}^n$.

Lorsque $n = 1$, l’ensemble $I(f)$ est un intervalle de $\mathbf{R}$, ouvert à gauche et ouvert ou fermé à droite ; sa borne supérieure (finie ou $+\infty$) se note $\rho(f)$ et s’appelle le *rayon de convergence strict* de $f$.

Avec les notations de 4.1.2, on a $R \in I(f)$ si et seulement si
$$
(R, \ldots, R) \in I(j(f)).
$$
L’ensemble des points $x = (x_i)$ tels qu’il existe $R = (R_i) \in I(f)$ avec $\|x_i\| \leq R_i$ pour $1 \leq i \leq n$ s’appelle le *domaine de convergence strict* de $f$ et se note $C(f)$. C’est un ouvert de $E$, réunion des polyboules
$$
B(R) = \{ x \in E \mid \|x_i\| \leq R_i \text{ pour } 1 \leq i \leq n \},
$$
pour $R \in I(f)$.

4.1.4. Les résultats de 3.1.7 et 3.1.8 restent exacts, en y remplaçant partout $\tilde{C}(f)$ par $C(f)$ et $\tilde{\mathcal{H}}_R$ par $\mathcal{H}_R$.

4.1.5. Soient $F_1, \ldots, F_m$ des espaces normés complets et supposons $F$ quasi-complet. Soit $f = (f_i)_{1 \leq i \leq m}$, avec $f_i \in \mathcal{H}(E_1, \ldots, E_n; F_i)$ et soit $g \in \mathcal{H}(F_1, \ldots, F_m; F)$, tels que le point $(f_i(0))_{1 \leq i \leq m}$ de $E$ appartienne au domaine de convergence strict de $g$. Alors, pour tout $\alpha \in \mathbf{N}^m$, la série formelle $g_\alpha \circ f$ appartient à $\mathcal{H}(E_1, \ldots, E_n; F)$ et la famille des $g_\alpha \circ f$ est sommable dans $\mathcal{H}(E_1, \ldots, E_n; F)$ (donc *a fortiori* dans $\hat{P}(E_1, \ldots, E_n; F)$). Sa somme sera notée $g \circ f$.

De manière plus précise, il existe $R \in \bigcap_i I(f_i)$ et $R' \in I(g)$ tels que
$$
\sup_{|\alpha| > 0} \|f_{i,\alpha}\| R^\alpha < R'_i \quad (\text{pour } 1 \leq i \leq m).
$$
Sous ces conditions la série formelle $g_\alpha \circ f$ appartient à $\mathcal{H}_R(E_1, \ldots, E_n; F)$ et la famille des $g_\alpha \circ f$ est sommable dans $\mathcal{H}_R(E_1, \ldots, E_n; F)$. Enfin, si $x \in B(R)$, alors $f(x) = (f_i(x))$ appartient à $C(g)$ et on a :
$$
g(f(x)) = (g \circ f)(x).
$$

Supposons de plus que, pour chaque $i$, il existe une famille $(e_j^i)$ d’éléments de $E_i$ tel que tout élément $x$ de $E_i$ soit somme d’une famille sommable $(\lambda_j e_j^i)$ (avec $\lambda_j \in K$) telle que $\|x\| = \sup_j |\lambda_j|$. On peut alors dans l’alinéa précédent, remplacer la condition $\sup_{|\alpha| > 0} \|f_{i,\alpha}\| R^\alpha < R'_i$ par la condition $\|f_i\|_R \leq R'_i$.

4.1.6. Supposons que $E_i = K$ pour $1 \leq i \leq n$. L’espace $\hat{P}(K^n; F)$ s’identifie alors à l’espace des séries formelles à $n$ indéterminées $X_1, \ldots, X_n$ à coefficients dans $F$ et un élément $f$ de $\hat{P}(K^n; F)$ s’écrit :
$$
f = \sum_a X^a c_a \quad \text{avec } c_a \in F.
$$
Si $R \in (\mathbf{R}_+^*)^n$ et si $\gamma$ est une semi-norme continue sur $F$, on a :
$$
\|f\|_{\gamma, R} = \sup \|c_a\|_\gamma \cdot R^\alpha.
$$

Le dernier alinéa de 3.1.10 reste valable, ainsi que 3.1.11.

4.1.7. Supposons que K soit un sous-corps fermé d’un corps valué complet (nécessairement ultramétrique) L. Pour $y \in E_i \otimes_K L$, posons:

$$
\|y\| = \inf_k (\sup |a_k| \cdot \|x_k\|)
$$

la borne inférieure étant étendue à toutes les familles finies de couples $(x_k, a_k) \in E_i \times L$ telles que $y = \sum_k x_k \otimes a_k$. On obtient ainsi une norme sur le L-espace vectoriel $E_i \otimes_K L$, qui induit sur $E_i$ la norme donnée. On désigne par $E_i^L$ le complété de $E_i \otimes_K L$ pour cette norme.

Soit maintenant F un L-espace vectoriel polynormé séparé complet. Pour tout K-polynome-continu $f_\alpha$, homogène de multidegré $\alpha$, sur $E_1 \times \cdots \times E_n$, à valeurs dans le K-espace vectoriel polynormé $F_K$ sous-jacent à F, il existe un L-polynome-continu $\tilde{f}_\alpha$ et un seul, homogène de même multidegré, sur $E_1^L \times \cdots \times E_n^L$, à valeurs dans F qui prolonge $f_\alpha$. Pour toute semi-norme continue sur le L-espace vectoriel F, on a

$$
\|\tilde{f}_\alpha\|_i = \|f_\alpha\|_i.
$$

Si $f = \sum f_\alpha \in \mathcal{H}(E_1, \ldots, E_n; F_K)$, alors $\tilde{f} = \sum \tilde{f}_\alpha \in \mathcal{H}(E_1^L, \ldots, E_n^L; F)$.

Les séries $f$ et $\tilde{f}$ ont même indicatrice de convergence stricte (et même rayon de convergence strict lorsque $n = 1$).

Inversement, soit L un sous-corps fermé non discret de K et soient $E_i^0$ et $F^0$ les espaces sur L obtenus par restriction des scalaires à partir des $E_i$ et de F. Si $f = \sum f_\alpha \in \mathcal{H}(E_1, \ldots, E_n; F)$, alors $f_\alpha \in P_\alpha(E_1^0, \ldots, E_n^0; F^0)$; si l’on pose $f^0 = \sum \tilde{f}_\alpha \in \hat{P}(E_1^0, \ldots, E_n^0; F^0)$, alors $f^0 \in \mathcal{H}(E_1^0, \ldots, E_n^0; F^0)$.

On a $C(f) \subset C(f^0)$ et $f(x) = f^0(x)$ pour tout $x \in C(f)$.

### 4.2. Fonctions analytiques

4.2.1. Les définitions et résultats de 3.2.1 et 3.2.2 restent valables sans changements.

4.2.2. Avec les notations de 3.2.2, l’indicatrice de convergence stricte du développement en série entière de $\Delta^a f$ en un point $a$ de U contient celle du développement en série entière de $f$ en $a$.

4.2.3. Les résultats de 3.2.4, 3.2.5, 3.2.7, 3.2.8 et 3.2.11 restent exacts. Celui de 3.2.6 aussi, à condition de supposer en plus que K est de caractéristique zéro.

4.2.4. Supposons F quasi-complet et soit $f \in \mathcal{H}(E_1, \ldots, E_n; F)$. La fonction $x \mapsto f(x)$ est analytique dans $C(f)$. Pour tout $a \in C(f)$, l’indicatrice de convergence du développement en série entière de $f$ en $a$ est égale à celle de $f$.

### 4.3. Quelques inégalités

4.3.1. On suppose que K satisfait à l’une au moins des conditions suivantes :
(a) le corps résiduel de K est infini ;
(b) l’image de K par l’application $a \mapsto |a|$ est dense dans $\mathbf{R}_+$. (Autrement dit, on suppose que K n’est pas localement compact).
Soit $f = \sum_\alpha f_\alpha \in \mathcal{H}(E_1, \ldots, E_n; F)$ et soit $R \in I(f)$. On a :
$$
\sup_{x \in B(R)} \|f(x)\|_y = \sup_\alpha \sup_{x \in B(R)} \|f_\alpha(x)\|_y
$$
pour toute semi-norme continue $\gamma$ sur F (« inégalités de Cauchy »).

4.3.2. Il existe une constante $a > 0$ telle que pour tout polynôme homogène continu $f_\alpha \in P_\alpha(E_1, \ldots, E_n; F)$ et tout $R \in (\mathbf{R}_+^*)^n$, l’on ait :
$$
a^{|\alpha|} R^{\alpha} |\alpha|! \|f_\alpha\|_y \leq \sup_{x \in B(R)} \|f_\alpha(x)\|_y \leq \|f_\alpha\|_y R^\alpha
$$
pour toute semi-norme continue $\gamma$ sur F. Si K satisfait à la condition (b) de 4.3.1 ou si l’image de $E_i$ par l’application $x \mapsto \|x\|$ est contenue dans l’image de K par l’application $a \mapsto |a|$ et contient $R_i$ (pour $1 \leq i \leq n$), on peut prendre $a = 1$.

4.3.3. Si K est de caractéristique zéro, la série formelle $f = \sum_\alpha f_\alpha$ appartient à $\mathcal{H}(E_1, \ldots, E_n; F)$ si et seulement si il existe $R \in (\mathbf{R}_+^*)^n$ tel que
$$
\sup_\alpha \sup_{x \in B(R)} \|f_\alpha(x)\|_y < +\infty
$$
pour toute semi-norme continue $\gamma$ sur F.
