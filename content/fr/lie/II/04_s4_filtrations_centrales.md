---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: ALGÈBRES DE LIE LIBRES
section: 4
section_title: Filtrations centrales
lang: fr
source: lie-ii-iii-fr
pdf_pages: 0036-0043, 0077-0082
extraction: ocr
subsections:
    - "no": 1
      title: Filtrations réelles
      page: 0
      pdf_page: 36
    - "no": 2
      title: Fonction d’ordre
      page: 0
      pdf_page: 36
    - "no": 3
      title: Algèbre graduée associée à une algèbre filtrée
      page: 0
      pdf_page: 37
    - "no": 4
      title: Filtrations centrales sur un groupe
      page: 0
      pdf_page: 38
    - "no": 5
      title: Un exemple de filtration centrale
      page: 0
      pdf_page: 40
    - "no": 6
      title: Filtrations centrales entières
      page: 0
      pdf_page: 42
statements: 12
exercises: 5
content_sha256: ed2b5fec59480c910ce66fa175a3dbf26af384b9d04336dddb45498d40fa3157
---

## § 4. Filtrations centrales

### 1. Filtrations réelles

#### Définition 1 {#lie-ii-s4-def-1 .statement}

Soit G un groupe. On appelle filtration réelle sur G une famille $(G_\alpha)_{\alpha \in \mathbf{R}}$ de sous-groupes de G telle que

$$
G_\alpha = \bigcap_{\beta < \alpha} G_\beta \quad \text{pour tout } \alpha \in \mathbf{R}.
$$

La formule (1) entraîne $G_\alpha \subset G_\beta$ pour $\beta < \alpha$, donc la famille $(G_\alpha)$ est décroissante. On dit que la filtration $(G_\alpha)$ est séparée si $\bigcap_\alpha G_\alpha$ est réduit à l’élément neutre et qu’elle est exhaustive si $G = \bigcup_\alpha G_\alpha$.

#### Remarque {#lie-ii-s4-n1-rem-1 .statement}

Soit $(G_n)_{n \in \mathbf{Z}}$ une suite décroissante de sous-groupes de G. C’est une filtration décroissante au sens de AC, III, § 2, no 1, déf. 1. Pour tout entier $n$ et tout $\alpha$ dans l’intervalle $]n-1, n]$ de $\mathbf{R}$, posons $H_\alpha = G_n$, d’où en particulier $H_n = G_n$. Il est immédiat qu’on obtient ainsi une filtration réelle $(H_\alpha)_{\alpha \in \mathbf{R}}$ sur G; on dira qu’une telle filtration est une filtration entière. On peut donc identifier les filtrations décroissantes au sens de AC, III, § 2 aux filtrations entières.

Soit A une algèbre; une filtration réelle $(A_\alpha)$ sur le groupe additif de A est dite compatible avec la structure d’algèbre si l’on a $A_\alpha . A_\beta \subset A_{\alpha + \beta}$ pour $\alpha, \beta$ dans $\mathbf{R}$ et $K . A_\alpha \subset A_\alpha$ pour $\alpha \in \mathbf{R}$. Si la filtration est exhaustive, $(A_\alpha)$ est un système fondamental de voisinages de 0 pour une topologie sur A qui est compatible avec la structure d’algèbre. Soit B une algèbre unifière; une filtration réelle $(B_\alpha)$ sur le groupe additif de B est dite compatible avec la structure d’algèbre unifière si elle est compatible avec la structure d’algèbre et si l’on a $1 \in B_0$.

### 2. Fonction d’ordre

Soit G un groupe d’élément neutre e. Soit $(G_\alpha)$ une filtration réelle sur G. Pour tout $x$ dans G, notons $I_x$ l’ensemble des nombres réels $\alpha$ tels que $x \in G_\alpha$. Si $\alpha \in I_x$ et $\beta < \alpha$, on a $\beta \in I_x$, donc $I_x$ est un intervalle (TG, IV, § 2, no 4, prop. 1). En utilisant la relation (1), on voit que $I_x$ contient son extrémité supérieure lorsque celle-ci est finie. Par conséquent, $I_x$ est de la forme $]-\infty, v(x)] \cap \mathbf{R}$ avec $v(x) \in \overline{\mathbf{R}}$; on a $v(x) = \sup \{ \alpha \mid x \in G_\alpha \}$.

L’application $v$ de $G$ dans $\mathbf{R}$ s’appelle la fonction d’ordre associée à la filtration réelle $(G_\alpha)$ et $v(x)$ s’appelle l’ordre de $x$. Cette application possède les propriétés suivantes:

a) Pour $x \in G$ et $\alpha \in \mathbf{R}$, les relations $x \in G_\alpha$ et $v(x) \geq \alpha$ sont équivalentes.

b) Pour $x, y$ dans $G$, on a
$$
v(x^{-1}) = v(x), \quad v(e) = +\infty,
$$
$$
v(xy) \geq \inf(v(x), v(y)).
$$
De plus, il y a égalité dans (3) si $v(x) > v(y)$.

c) Pour tout $\alpha \in \mathbf{R}$, notons $G_\alpha^+$ l’ensemble des $x \in G$ tels que $v(x) > \alpha$. On a $G_\alpha^+ = \bigcup_{\beta > \alpha} G_\beta$ et en particulier $G_\alpha^+$ est un sous-groupe de $G$.

Réciproquement, soit $v$ une application de $G$ dans $\overline{\mathbf{R}}$ satisfaisant aux relations (2) et (3). Pour tout $\alpha \in \mathbf{R}$, soit $G_\alpha$ l’ensemble des $x \in G$ tels que $v(x) \geq \alpha$. Alors $(G_\alpha)_{\alpha \in \mathbf{R}}$ est une filtration réelle de $G$, et $v$ est la fonction d’ordre associée à cette filtration. Pour que la filtration $(G_\alpha)$ soit entière, il faut et il suffit que $v$ applique $G$ dans $\mathbf{Z} \cup \{+\infty, -\infty\}$. Pour qu’elle soit exhaustive (resp. séparée), il faut et il suffit que $v^{-1}(-\infty) = \emptyset$ (resp. $v^{-1}(+\infty) = \{e\}$).

Soit $A$ une K-algèbre (resp. K-algèbre unifère). D’après ce qui précède, la relation
$$
\langle x \in A_\alpha \Leftrightarrow v(x) \geq \alpha \text{ pour } x \in A \text{ et } \alpha \in \mathbf{R} \rangle
$$
définit une bijection de l’ensemble des filtrations réelles exhaustives $(A_\alpha)_{\alpha \in \mathbf{R}}$ compatibles avec la structure d’algèbre (resp. d’algèbre unifère) de $A$, sur l’ensemble des applications $v : A \to \overline{\mathbf{R}}$ ne prenant pas la valeur $-\infty$ et satisfaisant aux axiomes (4) à (7) (resp. (4) à (8)) suivants:
$$
\begin{align*}
(4) \quad & v(x+y) \geq \inf(v(x), v(y)) \quad (x, y \text{ dans } A) \\
(5) \quad & v(-x) = v(x) \quad (x \in A) \\
(6) \quad & v(\lambda x) \geq v(x) \quad (\lambda \in \mathbf{K}, x \in A) \\
(7) \quad & v(xy) \geq v(x) + v(y) \quad (x, y \text{ dans } A) \\
(8) \quad & v(1) \geq 0.
\end{align*}
$$

#### Remarque {#lie-ii-s4-n2-rem-1 .statement}

Si $v(x)$ n’est pas toujours égal à $+\infty$, les conditions (7) et (8) entraînent $v(1) = 0$.

### 3. Algèbre graduée associée à une algèbre filtrée

Soit $G$ un groupe commutatif muni d’une filtration réelle $(G_\alpha)_{\alpha \in \mathbf{R}}$. Posons comme précédemment
$$
G_\alpha^+ = \bigcup_{\beta > \alpha} G_\beta;
$$

il est clair que $G_\alpha^+$ est un sous-groupe de $G_\alpha$. Nous poserons $\mathrm{gr}_\alpha(G) = G_\alpha / G_\alpha^+$ et $\mathrm{gr}(G) = \bigoplus_{\alpha \in \mathbf{R}} \mathrm{gr}_\alpha(G)$. On appelle groupe gradué associé au groupe filtré $G$ le groupe $\mathrm{gr}(G)$ muni de sa graduation naturelle de type $\mathbf{R}$.

#### Remarque {#lie-ii-s4-n3-rem-1 .statement}

Lorsque la filtration $(G_\alpha)$ est entière, on a $\mathrm{gr}_\alpha(G) = \{0\}$ pour $\alpha$ non entier et $\mathrm{gr}_n(G) = G_n / G_{n-1}$ pour tout entier $n$. La définition du groupe gradué associé coïncide donc essentiellement avec celle de AC, III, § 2, no 3.

Soient $A$ une algèbre (resp. une algèbre unifère) et $(A_\alpha)_{\alpha \in \mathbf{R}}$ une filtration réelle compatible avec la structure d’algèbre (resp. d’algèbre unifère) (no 1). On a
$$
A_\alpha \cdot A_\beta \subset A_{\alpha + \beta}, \qquad A_\alpha^+ \cdot A_\beta + A_\alpha \cdot A_\beta^+ \subset A_{\alpha + \beta}^+,
$$
et l’application bilinéaire de $A_\alpha \times A_\beta$ dans $A_{\alpha + \beta}$ restriction de la multiplication de $A$ définit par passage au quotient une application bilinéaire
$$
\mathrm{gr}_\alpha(A) \times \mathrm{gr}_\beta(A) \to \mathrm{gr}_{\alpha + \beta}(A).
$$
On en déduit une application bilinéaire de $\mathrm{gr}(A) \times \mathrm{gr}(A)$ dans $\mathrm{gr}(A)$ qui en fait une algèbre graduée (resp. une algèbre graduée unifère) de type $\mathbf{R}$. Si $A$ est une algèbre associative (resp. commutative, resp. de Lie), il en est de même de $\mathrm{gr}(A)$.

### 4. Filtrations centrales sur un groupe

#### Définition 2 {#lie-ii-s4-def-2 .statement}

Soit $G$ un groupe. On dit qu’une filtration réelle $(G_\alpha)$ sur $G$ est centrale si l’on a $G = \bigcup_{\alpha > 0} G_\alpha$ et si le commutateur $(x, y) = x^{-1} y^{-1} xy$ d’un élément $x$ de $G_\alpha$ et d’un élément $y$ de $G_\beta$ appartient à $G_{\alpha + \beta}$.

En termes de la fonction d’ordre $v$, la définition précédente se traduit par les relations
$$
v(x) > 0, \qquad v((x, y)) \geq v(x) + v(y) \qquad \text{quels que soient } x, y \text{ dans } G.
$$
On en déduit que $v((x, y)) > v(x)$ si $v(x) \neq +\infty$; si l’on pose $x^y = y^{-1} xy$ (cf. A, I, p. 66), on a $x^y = x . (x, y)$ d’où
$$
v(x^y) = v(x).
$$
Cette relation traduit le fait que chacun des sous-groupes $G_\alpha$ de $G$ est distingué. Les $G_\alpha$ forment un système fondamental de voisinages de $e$ pour une topologie compatible avec la structure de groupe de $G$ (TG, III, § 1, no 2, Exemple), dite définie par la filtration $(G_\alpha)$.

Dans la suite de ce no, on note $G$ un groupe muni d’une filtration centrale $(G_\alpha)$. Pour tout $\alpha \in \mathbf{R}$, on définit le sous-groupe $G_\alpha^+$ de $G$ par
$$
G_\alpha^+ = \bigcup_{\beta > \alpha} G_\beta.
$$

On a en particulier $G_\alpha^+ = G_\alpha = G$ pour $\alpha \leq 0$. Rappelons que si $A$ et $B$ sont deux sous-groupes de $G$, on note $(A, B)$ le sous-groupe de $G$ engendré par les commutateurs $(a, b)$ avec $a \in A$ et $b \in B$. Avec cette notation, on a les formules

$$
(13) \qquad (G_\alpha, G_\beta) \subset G_{\alpha + \beta}
$$
$$
(13') \qquad (G_\alpha^+, G_\beta) \subset G_{\alpha + \beta}^+
$$
$$
(14) \qquad (G, G_\alpha) \subset G_\alpha^+.
$$

D’après (14), $G_\alpha^+$ est un sous-groupe distingué de $G_\alpha$ pour tout $\alpha \in \mathbf{R}$ et le groupe quotient $\mathrm{gr}_\alpha(G) = G_\alpha / G_\alpha^+$ est commutatif. On pose $\mathrm{gr}(G) = \bigoplus_{\alpha \in \mathbf{R}} \mathrm{gr}_\alpha(G)$, et l’on munit ce groupe de la graduation de type $\mathbf{R}$ dans laquelle $\mathrm{gr}_\alpha(G)$ se compose des éléments de degré $\alpha$. On a $\mathrm{gr}_\alpha(G) = \{0\}$ pour $\alpha \leq 0$.

#### Proposition 1 {#lie-ii-s4-prop-1 .statement}

(i) *Soient $\alpha, \beta$ dans $\mathbf{R}$. Il existe une application biadditive*
$$
\varphi_{\alpha \beta} : \mathrm{gr}_\alpha(G) \times \mathrm{gr}_\beta(G) \to \mathrm{gr}_{\alpha + \beta}(G)
$$
*qui applique* $(x G_\alpha^+, y G_\beta^+)$ *sur* $(x, y) G_{\alpha + \beta}^+$.
(ii) *Soit $\varphi$ l’application biadditive de $\mathrm{gr}(G) \times \mathrm{gr}(G)$ dans $\mathrm{gr}(G)$ dont la restriction à $\mathrm{gr}_\alpha(G) \times \mathrm{gr}_\beta(G)$ est $\varphi_{\alpha \beta}$ *pour tout couple* $(\alpha, \beta)$. *L’application $\varphi$ munit $\mathrm{gr}(G)$ d’une structure de $\mathbf{Z}$-algèbre de Lie*.

(i) Rappelons l’identité
$$
(xx', y) = (x, y)^{x'}(x', y)
$$
pour $x, x', y$ dans $G$ (A, I, p. 66, formule (4 bis)).

Pour $x \in G_\alpha$ et $y \in G_\beta$, la classe modulo $G_{\alpha + \beta}^+$ de l’élément $(x, y)$ de $G_{\alpha + \beta}$ sera notée $f(x, y)$. Pour $a$ dans $G_{\alpha + \beta}$ et $x'$ dans $G$, on a $a^{-1} . a^{x'} = (a, x') \in G_{\alpha + \beta}^+$; en particulier $f(x, y)$ est égale à la classe modulo $G_{\alpha + \beta}^+$ de $(x, y)^{x'}$. La formule (15) entraîne donc
$$
f(xx', y) = f(x, y)f(x', y).
$$
On a $(y, x) = (x, y)^{-1}$, d’où
$$
f(y, x) = f(x, y)^{-1}.
$$
De (16) et (17), on déduit
$$
f(x, yy') = f(x, y)f(x, y').
$$

Nous avons à prouver que l’application $f : G_\alpha \times G_\beta \to \mathrm{gr}_{\alpha + \beta}(G)$ définit par passage au quotient une application $\varphi_{\alpha \beta} : \mathrm{gr}_\alpha(G) \times \mathrm{gr}_\beta(G) \to \mathrm{gr}_{\alpha + \beta}(G)$. D’après (16) et (18), il suffit de prouver que l’on a $f(x, y) = 0$ si $x \in G_\alpha^+$ *ou* si $y \in G_\beta^+$, ce qui résulte de (13').

(ii) Comme on a $(x, x) = e$, il résulte de (17) que $\varphi$ est une application

Z-bilinéaire alternée. Il reste donc à prouver que pour $u \in \mathrm{gr}_\alpha(G)$, $v \in \mathrm{gr}_\beta(G)$ et $w \in \mathrm{gr}_\gamma(G)$, on a

$$
\varphi(u, \varphi(v, w)) + \varphi(v, \varphi(w, u)) + \varphi(w, \varphi(u, v)) = 0.
$$

Soient $x \in G_\alpha$, $y \in G_\beta$ et $z \in G_\gamma$ des éléments représentant respectivement $u$, $v$ et $w$. On sait que $x^y$ et $x$ sont deux éléments de $G_\alpha$ congrus modulo $G_\alpha^+$, donc $x^y$ est un représentant de $u$ dans $G_\alpha$; comme $(y, z)$ est un représentant de $\varphi(v, w)$ dans $G_{\beta+\gamma}$, on voit que $(x^y, (y, z))$ est un représentant de $\varphi(u, \varphi(v, w))$ dans $G_{\alpha+\beta+\gamma}$. Par permutation circulaire, on voit que $(y^z, (z, x))$ et $(z^x, (x, y))$ représentent respectivement $\varphi(v, \varphi(w, u))$ et $\varphi(w, \varphi(u, v))$ dans $G_{\alpha+\beta+\gamma}$. La relation (19) est alors conséquence de l’identité suivante (A, I, p. 66, formule (15)):

$$
(x^y, (y, z)).(y^z, (z, x)).(z^x, (x, y)) = e.
$$

C.Q.F.D.

L’algèbre de Lie $\mathrm{gr}(G)$ sur $\mathbf{Z}$ définie dans la proposition 1 s’appelle l’algèbre de Lie graduée associée au groupe filtré $G$.

### 5. Un exemple de filtration centrale

Soit $A$ une algèbre associative unifière munie d’une filtration d’algèbre unifière $(A_\alpha)$ telle que $A_0 = A$; alors $A_\alpha$ est un idéal bilatère de $A$ pour tout $\alpha \in \mathbf{R}$. On note $A^*$ le groupe multiplicatif des éléments inversibles de $A$. Pour tout $\alpha > 0$, on note $\Gamma_\alpha$ l’ensemble des $x \in A^*$ tels que $x - 1 \in A_\alpha$; on pose $\Gamma = \bigcup_{\alpha > 0} \Gamma_\alpha$ et $\Gamma_\beta = \Gamma$ pour $\beta \leqslant 0$.

#### Proposition 2 {#lie-ii-s4-prop-2 .statement}

L’ensemble $\Gamma$ est un sous-groupe de $A^*$ et $(\Gamma_\alpha)$ est une filtration centrale sur $\Gamma$.

On a $\Gamma = \bigcup_{\alpha > 0} \Gamma_\alpha$ par construction, et la relation $\Gamma_\alpha = \bigcap_{\beta < \alpha} \Gamma_\beta$ résulte de $A_\alpha = \bigcap_{\beta < \alpha} A_\beta$.

Montrons que $\Gamma_\alpha$ est un sous-groupe de $A^*$. On a $1 \in \Gamma_\alpha$; soient $x, y$ dans $\Gamma_\alpha$, d’où $x - 1 \in A_\alpha, y - 1 \in A_\alpha$. Comme $A_\alpha$ est un idéal bilatère de $A$, les formules

$$
xy - 1 = (x - 1)(y - 1) + (x - 1) + (y - 1)
$$
$$
x^{-1} - 1 = -x^{-1}(x - 1),
$$

entraînent $xy - 1 \in A_\alpha$ et $x^{-1} - 1 \in A_\alpha$, d’où $xy \in \Gamma_\alpha$ et $x^{-1} \in \Gamma_\alpha$.

Comme $\Gamma = \bigcup_{\alpha > 0} \Gamma_\alpha$, c’est un sous-groupe de $A^*$.

Soient enfin $\alpha > 0, \beta > 0, x \in \Gamma_\alpha$ et $y \in \Gamma_\beta$. Posons $x - 1 = \xi$ et $y - 1 = \eta$.

On a

$$(x, y) - 1 = x^{-1}y^{-1}(\xi \eta - \eta \xi);$$

par hypothèse, on a $\xi \in A_\alpha$ et $\eta \in A_\beta$, d’où $\xi \eta - \eta \xi \in A_{\alpha + \beta}$. Comme $A_{\alpha + \beta}$ est un idéal bilatère de $A$, on a $(x, y) - 1 \in A_{\alpha + \beta}$ d’où $(x, y) \in \Gamma_{\alpha + \beta}$.

C.Q.F.D.

#### Remarque {#lie-ii-s4-n5-rem-1 .statement}

Soient $\alpha \geqslant 0, \beta \geqslant 0$ et $x \in \Gamma_\alpha, y \in \Gamma_\beta$. D’après les formules (21), (22) et (23), on a

$$(24)$$
$$x^{-1} - 1 \equiv -(x - 1) \quad \text{mod. } A_{2\alpha}$$

$$(25)$$
$$xy - 1 \equiv (x - 1) + (y - 1) \quad \text{mod. } A_{\alpha + \beta}$$

$$(26)$$
$$(x, y) - 1 \equiv [(x - 1), (y - 1)] \quad \text{mod. } A_{\alpha + \beta + \inf(\alpha, \beta)}.$$

Démontrons par exemple (26). Si $x - 1 = \xi$ et $y - 1 = \eta$, (23) donne:

$$(x, y) - 1 - [\xi, \eta] = ((x^{-1} - 1) + (y^{-1} - 1) + (x^{-1} - 1)(y^{-1} - 1))[\xi, \eta].$$

Or $[\xi, \eta] \in A_{\alpha + \beta}$, $(x^{-1} - 1) \in A_\alpha$, $(y^{-1} - 1) \in A_\beta$, d’où (26).

Soient $G$ un groupe et $\rho : G \to \Gamma$ un homomorphisme. Pour tout $\alpha$ réel, on pose $G_\alpha = \rho^{-1}(\Gamma_\alpha)$. Comme $(\Gamma_\alpha)$ est une filtration centrale sur $\Gamma$, il est immédiat que $(G_\alpha)$ est une filtration centrale sur $G$.

#### Proposition 3 {#lie-ii-s4-prop-3 .statement}

(i) *Pour tout $\alpha \in \mathbf{R}$, il existe un unique homomorphisme de groupes $g_\alpha : \mathrm{gr}_\alpha(G) \to \mathrm{gr}_\alpha(A)$ qui applique la classe modulo $G_\alpha^+$ d’un élément $a \in G_\alpha$ sur la classe modulo $A_\alpha^+$ de $\rho(a) - 1$.*

(ii) *Soit $g$ l’homomorphisme de groupes de $\mathrm{gr}(G)$ dans $\mathrm{gr}(A)$ dont la restriction à $\mathrm{gr}_\alpha(G)$ est $g_\alpha$ pour tout $\alpha$. L’application $g$ est un homomorphisme injectif de $\mathbf{Z}$-algèbres de Lie.*

(i) Soit $\alpha > 0$. Par hypothèse, pour tout $a$ dans $G_\alpha$, on a $\rho(a) - 1 \in A_\alpha$; on note $p_\alpha(a)$ la classe de $\rho(a) - 1$ modulo $A_\alpha^+$. Comme on a $A_{2\alpha} \subset A_\alpha^+$, la relation (25) entraîne $p_\alpha(ab) = p_\alpha(a) + p_\alpha(b)$. On a $a \in G_\alpha^+$ si et seulement si $\rho(a) - 1 \in A_\alpha^+$; par suite, $G_\alpha^+$ est le noyau de l’homomorphisme $p_\alpha$ de $G_\alpha$ dans $\mathrm{gr}_\alpha(A)$. Par passage au quotient, $p_\alpha$ définit donc un homomorphisme injectif $g_\alpha$ de $\mathrm{gr}_\alpha(G)$ dans $\mathrm{gr}_\alpha(A)$.

Pour $\alpha \leqslant 0$, on a $\mathrm{gr}_\alpha(G) = \{0\}$, et l’on n’a pas d’autre choix que $g_\alpha = 0$.

(ii) Comme $g_\alpha$ est injectif pour tout $\alpha$ réel, $g$ est injectif. Montrons que $g$ est un homomorphisme d’algèbres de Lie. Comme on a $\mathrm{gr}_\alpha(G) = \{0\}$ pour $\alpha \leqslant 0$, il suffit d’établir la formule

$$(27)$$
$$p_{\alpha + \beta}((a, b)) = [p_\alpha(a), p_\beta(b)]$$

pour $\alpha > 0, \beta > 0, a \in G_\alpha$ et $b \in G_\beta$, ce qui résulte de (26).

### 6. Filtrations centrales entières

Rappelons (n° 1, Remarque) qu’une filtration $(G_\alpha)$ sur le groupe $G$ est dite entière si l’on a $G_\alpha = G_n$ pour tout entier $n$ et tout $\alpha \in ]n - 1, n]$. La donnée d’une filtration centrale entière sur un groupe $G$ équivaut à la donnée d’une suite $(G_n)_{n \geq 1}$ de sous-groupes de $G$ satisfaisant aux conditions

(i) $$G_1 = G$$
(ii) $$G_n \supset G_{n+1}$$ pour tout $n \geq 1$
(iii) $$(G_m, G_n) \subset G_{m+n}$$ pour $m \geq 1$ et $n \geq 1$.

Pour tout entier $n \geq 1$, $G_n$ est un sous-groupe distingué de $G$ et le groupe quotient $\mathrm{gr}_n(G) = G_n/G_{n+1}$ est commutatif. Par passage au quotient, l’application $(x, y) \mapsto (x, y) = x^{-1}y^{-1}xy$ de $G_m \times G_n$ dans $G_{m+n}$ permet de définir sur $\mathrm{gr}(G) = \bigoplus_{n \geq 1} \mathrm{gr}_n(G)$ une structure d’algèbre de Lie graduée de type $\mathbf{N}$ sur l’anneau $\mathbf{Z}$.

On rappelle (A, I, p. 68, déf. 5) que la suite centrale descendante du groupe $G$ est définie par
$$(28)\quad C^1G = G,\quad C^{n+1}G = (G, C^nG)$$ pour $n \geq 1$.

La filtration correspondante s’appelle la filtration centrale descendante de $G$.

#### Proposition 4 {#lie-ii-s4-prop-4 .statement}

(i) *La suite centrale descendante de $G$ est une filtration centrale entière sur $G$*.

(ii) *Si $(G_n)_{n \in \mathbf{N}^*}$ est une filtration centrale entière sur $G$, on a $C^nG \subset G_n$ pour tout $n \in \mathbf{N}^*$*.

L’assertion (i) a été prouvée en A, I, p. 68, formule (7).

On démontre (ii) par récurrence sur $n$; on a $C^1G = G = G_1$; pour $n > 1$, on a $C^nG = (G, C^{n-1}G) \subset (G, G_{n-1}) \subset G_n$.

#### Proposition 5 {#lie-ii-s4-prop-5 .statement}

*Soit $G$ un groupe et soit $\mathrm{gr}(G)$ la $\mathbf{Z}$-algèbre de Lie graduée associée à la filtration centrale descendante de $G$. Alors $\mathrm{gr}(G)$ est engendrée par $\mathrm{gr}_1(G) = G/(G, G)$*.

Soit $L$ la sous-algèbre de Lie de $\mathrm{gr}(G)$ engendrée par $\mathrm{gr}_1(G)$; montrons que $L \supset \mathrm{gr}_n(G)$ par récurrence sur $n$, l’assertion étant triviale pour $n = 1$. Supposons $n > 1$ et $L \supset \mathrm{gr}_{n-1}(G)$. Comme $C^nG = (G, C^{n-1}G)$, la construction de la loi d’algèbre de Lie sur $\mathrm{gr}(G)$ montre aussitôt que $\mathrm{gr}_n(G) = [\mathrm{gr}_1(G), \mathrm{gr}_{n-1}(G)] \subset L$.

La démonstration précédente montre que la suite centrale descendante de l’algèbre de Lie $\mathrm{gr}(G)$ (\S 2, n° 7) est donnée par
$$(29)\quad \mathcal{C}^n(\mathrm{gr}(G)) = \sum_{m \geq n} \mathrm{gr}_m(G).$$

#### Remarque {#lie-ii-s4-n6-rem-1 .statement}

Soient $k$ un anneau, $n$ un entier $> 0$, $A$ l’ensemble des matrices à $n$ lignes et $n$ colonnes, à éléments dans $k$, triangulaires inférieures. Pour $p \geq 0$, soit $A_p$ l’ensemble des $(x_{ij}) \in A$ telles que $x_{ij} = 0$ pour $i - j < p$. Alors $A_0 = A$ et

A_p A_q \subset A_{p+q}. Soit $\Gamma_p = 1 + A_p$. Alors $\Gamma_1$ est un sous-groupe de $\mathbf{GL}(n, k)$ appelé groupe trigonal strict inférieur d’ordre $n$ sur $k$. D’après la prop. 2 du n° 5, ($\Gamma_p$) est une filtration centrale entière sur $\Gamma_1$. Comme $\Gamma_n = \{1\}$, on voit que le groupe $\Gamma_1$ est nilpotent (A, I, p. 69, déf. 6).

## EXERCICES {#lie-ii-s4-exercises}

Dans les exercices ci-après, la lettre G désigne un groupe.

See the [exercises for § 4](exercises/s4/).
