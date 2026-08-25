---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: GROUPES DE LIE
section: 9
section_title: Commutateurs, centralisateurs, normalisateurs dans un groupe de Lie
lang: fr
source: lie-ii-iii-fr
pdf_pages: 0228-0244, 0274-0282
extraction: ocr
subsections:
    - "no": 1
      title: Commutateurs dans un groupe topologique
      page: 0
      pdf_page: 228
    - "no": 2
      title: Commutateurs dans un groupe de Lie
      page: 0
      pdf_page: 229
    - "no": 3
      title: Centralisateurs
      page: 0
      pdf_page: 231
    - "no": 4
      title: Normalisateurs
      page: 0
      pdf_page: 232
    - "no": 5
      title: Groupes de Lie nilpotents
      page: 0
      pdf_page: 233
    - "no": 6
      title: Groupes de Lie résolubles
      page: 0
      pdf_page: 238
    - "no": 7
      title: Radical d’un groupe de Lie
      page: 0
      pdf_page: 239
    - "no": 8
      title: Groupes de Lie semi-simples
      page: 0
      pdf_page: 240
statements: 54
exercises: 16
content_sha256: 109986749383b217d0c46ad2877b500a3a378fd480c3bba88251c24d0f838385
---

## § 9. Commutateurs, centralisateurs, normalisateurs dans un groupe de Lie

Dans ce paragraphe, on suppose que K est de caractéristique zéro.

### 1. Commutateurs dans un groupe topologique

Soit G un groupe topologique. On définit les groupes $\overline{D^0}G, \overline{D^1}G, \overline{D^2}G, \ldots$ et $\overline{C^1}G, \overline{C^2}G, \overline{C^3}G, \ldots$ par les formules

$$
\overline{D^0}G = G, \quad \overline{D^{i+1}}G = (\overline{D^i}G, \overline{D^i}G)
$$
$$
\overline{C^1}G = G, \quad \overline{C^{i+1}}G = (G, \overline{C^i}G).
$$

#### Proposition 1 {#lie-iii-s9-prop-1 .statement}

Soient G un groupe topologique, A et B des sous-groupes de G. On a $(\overline{A}, \overline{B}) = (\overline{A}, \overline{B}), \overline{D^i}A = \overline{D^i}A, \overline{C^i}A = \overline{C^i}A$.

Soit $\varphi$ l’application continue $(x, y) \mapsto x^{-1}y^{-1}xy$ de $G \times G$ dans G. On a $\varphi(A \times B) \subset (A, B)$, donc $\varphi(\overline{A} \times \overline{B}) \subset (\overline{A}, \overline{B})$, donc $(\overline{A}, \overline{B}) \subset (\overline{A}, \overline{B})$; l’inclusion opposée est évidente, donc $(\overline{A}, \overline{B}) = (\overline{A}, \overline{B})$. Il est clair que $\overline{D^0}A = \overline{D^0}A$; admettant l’égalité $\overline{D^i}A = \overline{D^i}A$, on en déduit

$$
\overline{D^{i+1}}A = (\overline{D^i}A, \overline{D^i}A) = (\overline{D^i}A, \overline{D^i}A) = (\overline{D^i}A, \overline{D^i}A) = \overline{D^{i+1}}A
$$

donc $\overline{D^i}A = \overline{D^i}A$ pour tout $i$. La démonstration de la formule $\overline{C^i}A = \overline{C^i}A$ est analogue.

#### Corollaire 1 {#lie-iii-s9-prop-1-cor-1 .statement}

Si G est séparé, les conditions suivantes sont équivalentes:

(i) G est résoluble (resp. nilpotent);
(ii) on a $\overline{D^i}G = \{e\}$ (resp. $\overline{C^i}G = \{e\}$) pour i assez grand.

On a $D^iG \subset \overline{D^i}G, C^iG \subset \overline{C^i}G$, donc (ii) $\Rightarrow$ (i). On a $\{e\} = \overline{\{e\}}$, donc (i) $\Rightarrow$ (ii) d’après la prop. 1.

#### Corollaire 2 {#lie-iii-s9-prop-1-cor-2 .statement}

Soient G un groupe topologique séparé, A un sous-groupe de G. Pour que A soit résoluble (resp. nilpotent, commutatif), il faut et il suffit que $\overline{A}$ le soit.

Cela résulte aussitôt de la prop. 1.

#### Proposition 2 {#lie-iii-s9-prop-2 .statement}

Soient G un groupe topologique, A et B des sous-groupes de G. Si A est connexe, (A, B) est connexe.

Pour y fixé dans B, l’ensemble M_y des (x, y) pour x ∈ A est connexe (car l’application x ↦ (x, y) de A dans G est continue). On a e ∈ M_y, donc la réunion R des M_y pour y ∈ B est connexe. Or (A, B) est le sous-groupe de G engendré par R, d’où la proposition.

### 2. Commutateurs dans un groupe de Lie

#### Proposition 3 {#lie-iii-s9-prop-3 .statement}

Soient G un groupe de Lie de dimension finie, H_1 et H_2 des sous-groupes de G. Soient h_1, h_2 et h la sous-algèbre de Lie tangente en e à H_1, H_2 et (H_1, H_2) respectivement. Alors [h_1, h_2] ⊂ h.

Soient a ∈ h_1, b ∈ h_2. Il existe un voisinage ouvert I de 0 dans K, et des applications analytiques f_1, f_2 de I dans G telles que
$$
f_1(0) = f_2(0) = e, f_1(I) \subset H_1, f_2(I) \subset H_2, (T_0 f_1)1 = a, (T_0 f_2)1 = b.
$$
Posons
$$
f(\lambda, \mu) = (f_1(\lambda), f_2(\mu)) \in (H_1, H_2) \quad \text{pour } \lambda, \mu \text{ dans } I.
$$
Identifions un voisinage ouvert de e dans G à une partie ouverte de K' à l’aide d’une carte qui transforme e en 0. Alors L(G) s’identifie à K'. D’après le § 5, n° 2, prop. 1, le développement en série entière à l’origine de f(λ, μ) est
$$
f(\lambda, \mu) = \lambda \mu [a, b] + \sum_{i \geq 1, j \geq 1, i+j \geq 3} \lambda^i \mu^j a_{ij}
$$
où a_{ij} ∈ K' (les termes en λ^i ou en μ^j dans le développement de f(λ, μ) sont nuls parce que f(λ, 0) = f(0, μ) = 0). Fixons μ dans I. En faisant tendre λ vers 0, on voit que
$$
\mu [a, b] + \sum_{j \geq 2} \mu^j a_{1j} \in h.
$$
Cela étant vrai pour tout μ ∈ I, on en conclut que [a, b] ∈ h.

#### Remarque {#lie-iii-s9-n2-rem-1 .statement}

Même si H_1 et H_2 sont des sous-groupes de Lie connexes de G, la sous-algèbre de Lie de L(G) engendrée par [h_1, h_2] est distincte de h en général.

#### Proposition 4 {#lie-iii-s9-prop-4 .statement}

Soit G un groupe de Lie réel ou complexe de dimension finie. Soient A, B, C des sous-groupes intégraux de G tels que [L(A), L(C)] ⊂ L(C), [L(B), L(C)] ⊂ L(C). Si [L(A), L(B)] ⊂ L(C), on a (A, B) ⊂ C. Si [L(A), L(B)] = L(C), on a (A, B) = C.

Supposons [L(A), L(B)] ⊂ L(C). La somme L(A) + L(B) + L(C) est une sous-algèbre de Lie de L(G). En considérant le sous-groupe intégral de G d’algèbre de Lie L(A) + L(B) + L(C), on est ramené au cas où
$$
L(A) + L(B) + L(C) = L(G)
$$

$$
[L(\varphi)(L(A)), L(\varphi)(L(B))] = \{0\},
$$

donc, φ(A) et φ(B) commutent d’après la formule de Hausdorff; par suite, (A, B) ⊂ C. Dans le cas général, soient G′ le revêtement universel de G, et A′, B′, C′ les sous-groupes intégraux de G′ tels que L(A′) = L(A), L(B′) = L(B), L(C′) = L(C). On a (A′, B′) ⊂ C′, et A, B, C sont les images canoniques de A′, B′, C′ dans G, d’où (A, B) ⊂ C. D’autre part, (A, B) est l’ensemble sous-jacent d’un sous-groupe intégral de G (§ 6, n° 2, cor. de la prop. 4), et son algèbre de Lie contient [L(A), L(B)] (prop. 3). Si [L(A), L(B)] = L(C), on a donc (A, B) ⊃ C, d’où (A, B) = C.

#### Corollaire {#lie-iii-s9-n2-cor-1 .statement}

Soit G un groupe de Lie réel ou complexe, connexe, de dimension finie, d’algèbre de Lie g. Les sous-groupes D^iG (resp. C^iG) sont des sous-groupes intégraux d’algèbres de Lie D^ig (resp. C^ig). Si G est simplement connexe, ce sont des sous-groupes de Lie.

La première assertion résulte de la prop. 4 par récurrence sur i. La deuxième résulte de la première et du § 6, n° 6, prop. 14.

#### Proposition 5 {#lie-iii-s9-prop-5 .statement}

Soient G un groupe de Lie réel ou complexe de dimension finie, A un sous-groupe intégral de G. On a D\overline{A} = DA. En particulier, A est un sous-groupe distingué de \overline{A}, et \overline{A}/A est commutatif.

Posons a = L(A). Soit G_1 l’ensemble des g ∈ G tels que

$$(\mathrm{Ad}\ g)x \equiv x \pmod{\mathcal{D}a} \quad \text{pour tout } x \in a.$$

Alors G_1 est un sous-groupe fermé de G. Si y ∈ a, on a exp y ∈ G_1, d’après le § 6, n° 4, cor. 3 (ii) de la prop. 10. Donc G_1 contient A et par suite \overline{A}. Ainsi, pour g ∈ \overline{A}, L(Int g) laisse stable a, et par suite Int g laisse stable A; plus précisément, L(Int g) définit l’automorphisme identique de a/\mathcal{D}a, donc Int g définit l’automorphisme identique de A/DA. Cela prouve que (\overline{A}, A) ⊂ DA. Pour la structure de groupe de Lie réel de G, \overline{A} est un sous-groupe de Lie (§ 8, n° 2, th. 2); soit b son algèbre de Lie. Soit G_2 l’ensemble des g ∈ G tels que

$$(\mathrm{Ad}\ g)x \equiv x \pmod{\mathcal{D}a} \quad \text{pour tout } x \in b.$$

D’après ce qui précède, on a G_2 ⊃ A, donc G_2 ⊃ \overline{A}. Par suite, pour g ∈ \overline{A}, Int g laisse stable DA et définit l’automorphisme identique de \overline{A}/DA. Donc DA ⊃ D\overline{A}.

#### Proposition 6 {#lie-iii-s9-prop-6 .statement}

Supposons K ultramétrique. Soit G un groupe de Lie de dimension finie. Soient A, B, C des sous-groupes de Lie de G tels que [L(A), L(C)] ⊂ L(C), [L(B), L(C)] ⊂ L(C). Si [L(A), L(B)] ⊂ L(C), il existe des sous-groupes ouverts A′, B′ de A, B tels que (A′, B′) ⊂ C. Si [L(A), L(B)] = L(C), il existe des sous-groupes ouverts A′, B′, C′ de A, B, C tels que (A′, B′) = C.

Supposons $[\mathrm{L}(A), \mathrm{L}(B)] \subset \mathrm{L}(C)$. Comme dans la démonstration de la prop. 4, on se ramène au cas où $\mathrm{L}(C)$ est un idéal de $\mathrm{L}(G)$. Puis, en remplaçant $G$ par un sous-groupe ouvert, on se ramène au cas où $C$ est distingué dans $G$ (\S 7, no 1, prop. 2). Soit $\varphi$ le morphisme canonique de $G$ sur $G/C$. Alors
$$
[\mathrm{L}(\varphi)(\mathrm{L}(A)), \mathrm{L}(\varphi)(\mathrm{L}(B))] = \{0\}.
$$
D’après la formule de Hausdorff, il existe des sous-groupes ouverts $A', B'$ de $A, B$ tels que $\varphi(A')$ et $\varphi(B')$ commutent, d’où $(A', B') \subset C$. Supposons de plus
$$
[\mathrm{L}(A), \mathrm{L}(B)] = \mathrm{L}(C).
$$
D’après la prop. 3, la sous-algèbre de Lie tangente en $e$ à $(A', B')$ contient $\mathrm{L}(C)$. Donc $(A', B')$ contient un sous-groupuscule de Lie de $G$ d’algèbre de Lie $\mathrm{L}(C)$. Par suite, $(A', B')$ est un sous-groupe ouvert de $C$.

#### Corollaire {#lie-iii-s9-n2-cor-2 .statement}

*Supposons K ultramétrique. Soit G un groupe de Lie de dimension finie, d’algèbre de Lie g. Il existe un sous-groupe ouvert $G_0$ de G tel que, pour tout i, $D^i G_0$ (resp. $C^i G_0$) soit un sous-groupe de Lie de G d’algèbre de Lie $\mathcal{D}^i g$ (resp. $\mathcal{C}^i g$).*

a) D’après la prop. 3 appliquée par récurrence, pour tout sous-groupe ouvert $G_1$ de $G$ et pour tout $i$, $D^i G_1$ contient un sous-groupuscule de Lie de $G$ d’algèbre de Lie $\mathcal{D}^i g$.

b) Soit $G'$ un sous-groupe ouvert de $G$ tel que, pour $i \leq n$, $D^i G'$ soit un sous-groupe de Lie de $G$ d’algèbre de Lie $\mathcal{D}^i g$. D’après la prop. 6, il existe des sous-groupes ouverts $H_1, H_2$ de $D^n G'$ tels que $(H_1, H_2)$ soit un sous-groupe de Lie d’algèbre de Lie $\mathcal{D}^{n+1} g$. Soit $G''$ un sous-groupe ouvert de $G'$ assez petit pour que $D^n G'' \subset H_1 \cap H_2$. Alors $D^{n+1} G'' \subset (H_1, H_2)$. Les relations
$$
D^0 G'' \subset D^0 G', \quad D^1 G'' \subset D^1 G', \ldots, D^n G'' \subset D^n G', \quad D^{n+1} G'' \subset (H_1, H_2)
$$
prouvent, compte tenu de $a)$, que $D^i G''$ est, pour $i \leq n + 1$, un sous-groupe de Lie de $G$ d’algèbre de Lie $\mathcal{D}^i g$.

c) Il existe un entier $p$ tel que $\mathcal{D}^p g = \mathcal{D}^{p+1} g = \ldots$. D’après ce qui précède, il existe un sous-groupe ouvert $G_0$ de $G$ tel que $D^i G_0$ soit, pour $i \leq p$, un sous-groupe de Lie de $G$ d’algèbre de Lie $\mathcal{D}^i g$. Mais, compte tenu de $a)$, la même assertion reste vraie pour $i > p$ puisque $D^p G_0 \supset D^i G_0$ pour $i > p$.

d) On raisonne de même pour les $C^i$.

### 3. Centralisateurs

Rappelons que deux éléments $x, y$ d’un groupe sont dits permutables si $(x, y) = e$, ou $(\mathrm{Int}\, x)y = y$, ou $(\mathrm{Int}\, y)x = x$; et que deux éléments $a, b$ d’une algèbre de Lie sont dits permutables si $[a, b] = 0$, ou $(\mathrm{ad}\, a).b = 0$, ou $(\mathrm{ad}\, b).a = 0$. Soient $G$ un groupe de Lie, $x \in G, a \in \mathrm{L}(G)$; on dira que $x$ et $a$ sont permutables si $(\mathrm{Ad}\, x).a = a$, c’est-à-dire si $xa = ax$ dans $\mathrm{T}(G)$.

Soient G un groupe de Lie, g son algèbre de Lie, A une partie de G, a une partie de g. On note $Z_G(A)$ (resp. $Z_G(a)$) l’ensemble des éléments de G permutables à tous les éléments de A (resp. a). C’est un sous-groupe fermé de G. On note $\delta_g(A)$ (resp. $\delta_g(a)$) l’ensemble des éléments de g permutables à tous les éléments de A (resp. a). C’est une sous-algèbre de Lie fermée de g.

#### Proposition 7 {#lie-iii-s9-prop-7 .statement}

*Soient G un groupe de Lie de dimension finie, g son algèbre de Lie, a une partie de g. Alors $Z_G(a)$ est un sous-groupe de Lie de G d’algèbre de Lie $\delta_g(a)$.*
Cela résulte du § 3, prop. 44 et cor. 2 de la prop. 39.

#### Proposition 8 {#lie-iii-s9-prop-8 .statement}

*Soient G un groupe de Lie réel ou complexe de dimension finie, g son algèbre de Lie, A une partie de G. Alors $Z_G(A)$ est un sous-groupe de Lie de G d’algèbre de Lie $\delta_g(A)$.*
Supposons A réduit à un point a. Alors $Z_G(A)$ est l’ensemble des points fixes de Int a; donc $Z_G(A)$ est un sous-groupe de Lie de G, et $L(Z_G(A))$ est l’ensemble des points fixes de Ad a, c’est-à-dire $\delta_g(A)$ ($\S 3, n° 8,$ cor. 1 de la prop. 29). Le cas général se déduit de là grâce au $\S 6, n° 2,$ cor. 3 de la prop. 1.

#### Proposition 9 {#lie-iii-s9-prop-9 .statement}

*Soient G un groupe de Lie réel ou complexe de dimension finie, g son algèbre de Lie, A un sous-groupe intégral de G, a = L(A). Alors $Z_G(A) = Z_G(a)$, $\delta_g(A) = \delta_g(a)$, et $Z_G(A)$ est un sous-groupe de Lie de G d’algèbre de Lie $\delta_g(a)$.*
Soit $x \in G$. On a
$$
x \in Z_G(A) \iff A \subset Z_G(\{x\}) \\
\iff a \subset L(Z_G(\{x\})) \quad (\S 6, \text{cor. 2 de la prop. 3}) \\
\iff a \subset \delta_g(\{x\}) \quad (\text{prop. 8}) \\
\iff x \in Z_G(a),
$$
donc $Z_G(A) = Z_G(a)$. Soit $u \in g$. On a
$$
u \in \delta_g(A) \iff A \subset Z_G(\{u\}) \\
\iff a \subset L(Z_G(\{u\})) \quad (\S 6, \text{cor. 2 de la prop. 3}) \\
\iff a \subset \delta_g^1(\{u\}) \quad (\text{prop. 7}) \\
\iff u \in \delta_g(a),
$$
donc $\delta_g(A) = \delta_g(a)$. La dernière assertion résulte alors de la prop. 7 ou de la prop. 8.

### 4. Normalisateurs

Soient G un groupe de Lie, g son algèbre de Lie, A une partie de G, a une partie de g. Dans cette section, on note $N_G(A)$ l’ensemble des $g \in G$ tels que $gAg^{-1} = A$. C’est

#### Proposition 10 {#lie-iii-s9-prop-10 .statement}

*Soient G un groupe de Lie de dimension finie, g son algèbre de Lie, a un sous-espace vectoriel de g. Alors $N_G(a)$ est un sous-groupe de Lie de G d’algèbre de Lie $n_g(a)$.*

Cela résulte du § 3, prop. 44 et cor. 1 de la prop. 39.

#### Proposition 11 {#lie-iii-s9-prop-11 .statement}

*Soient G un groupe de Lie réel ou complexe de dimension finie, g son algèbre de Lie, A un sous-groupe intégral de G, et $a = L(A)$. Alors $N_G(A) = N_G(a)$, et $N_G(A)$ est un sous-groupe de Lie de G, contenant $\overline{A}$, d’algèbre de Lie $n_g(a)$.*

L’égalité $N_G(A) = N_G(a)$ résulte du § 6, no 2, cor. 2 de la prop. 3. D’après la prop. 10, $N_G(A)$ est alors un sous-groupe de Lie de G d’algèbre de Lie $n_g(a)$. Donc $N_G(A)$ est fermé. Comme $N_G(A) \supset A$, on a $N_G(A) \supset \overline{A}$.

#### Corollaire {#lie-iii-s9-n4-cor-1 .statement}

*Si $a = n_g(a)$, A est un sous-groupe de Lie de G, et est la composante neutre de $N_G(A)$.*

En effet, cette composante neutre est un sous-groupe de Lie d’algèbre de Lie $n_g(a)$ (prop. 11), donc est égal à A d’après le § 6, no 2, th. 2 (i).

### 5. Groupes de Lie nilpotents

#### Proposition 12 {#lie-iii-s9-prop-12 .statement}

*Soit G un groupe de Lie de dimension finie. Pour que $L(G)$ soit nilpotente, il faut et il suffit que G possède un sous-groupe ouvert nilpotent.*

Supposons que G possède un sous-groupe ouvert nilpotent $G_0$. D’après les cor. des prop. 4 et 6, no 2, on a $C^i L(G_0) = \{0\}$ pour $i$ assez grand. Donc $L(G_0) = L(G)$ est nilpotente.

Supposons $L(G)$ nilpotente. Si $K = \mathbf{R}$ ou $\mathbf{C}$, la composante neutre $G_0$ de G est nilpotente d’après le cor. de la prop. 4, no 2, et $G_0$ est ouvert dans G. Si K est ultramétrique, le cor. de la prop. 6, no 2, prouve qu’il existe un sous-groupe ouvert $G_1$ de G, un entier $i > 0$, et un voisinage V de $e$ dans G tels que $C^i G_1 \cap V = \{e\}$. Alors, si $G_0$ est un sous-groupe assez petit de $G_1$, on a $C^i G_0 \subset V$, donc $C^i G_0 = \{e\}$, et $G_0$ est nilpotent. C.Q.F.D.

Soit $g$ une algèbre de Lie nilpotente. La série de Hausdorff $H(X, Y)$ correspondant à $g$ n’a qu’un nombre fini de termes non nuls, et l’on sait (chap. II, § 6, no 5, Remarque 3) que la loi de composition $(x, y) \mapsto H(x, y)$ définit sur $g$ une structure de groupe. Supposons de plus $g$ normable complète. Il est clair que la loi $H$ est un polynôme-continu (VAR, R, Appendice). Donc $g$, muni de la loi $H$, est un groupe de Lie G, dit associé à $g$. D’après le § 4, no 2, lemmes 2 et 3, on a

L(G) = g. L’application identique φ de g dans G est une application exponentielle de G, telle que $\varphi(\lambda x)\varphi(\lambda'x) = \varphi((\lambda + \lambda')x)$ quels que soient $x \in g, \lambda \in K, \lambda' \in K$. Toute sous-algèbre de Lie $\mathfrak{h}$ de g admettant un supplémentaire topologique est un sous-groupe de Lie H de G, et $L(H) = \mathfrak{h}$.

#### Proposition 13 {#lie-iii-s9-prop-13 .statement}

*Soit G un groupe de Lie nilpotent simplement connexe de dimension finie sur $\mathbf{R}$ ou $\mathbf{C}$.*

(i) $\exp_G$ est un isomorphisme du groupe de Lie associé à $L(G)$ sur G.
(ii) *Tout sous-groupe intégral de G est un sous-groupe de Lie simplement connexe de G.*

Soit $g = L(G)$, qui est nilpotente (prop. 12). Comme deux groupes de Lie simplement connexes sur $\mathbf{R}$ ou $\mathbf{C}$ qui ont même algèbre de Lie sont isomorphes ($\S 6$, n° 3, th. 3 (ii)), il suffit de prouver la proposition quand G est le groupe associé à g. Alors (i) et (ii) résultent de ce qu’on a dit avant la proposition.

#### Proposition 14 {#lie-iii-s9-prop-14 .statement}

*Soit G un groupe de Lie connexe de dimension finie sur $\mathbf{R}$ ou $\mathbf{C}$.*

(i) *Si G est nilpotent, $\exp_G$ est étale et surjective.*
(ii) *Si $K = \mathbf{C}$ et si $\exp_G$ est étale, alors G est nilpotent.*

Soit G′ le revêtement universel de G. Soit $\varphi$ le morphisme canonique de G′ sur G. On a $\exp_G = \varphi \circ \exp_{G'}$ ($\S 6$, n° 4, prop. 10), donc (i) résulte de la prop. 13 (i).

Si $K = \mathbf{C}$ et si exp est étale, alors, pour tout $x \in L(G)$, ad $x$ n’a aucune valeur propre appartenant à $2i\pi(\mathbf{Z} - \{0\})$ ($\S 6$, n° 4, cor. de la prop. 12). Appliquant cela à $\lambda x$, où $\lambda$ varie dans $\mathbf{C}$, on en conclut que toutes les valeurs propres de ad $x$ sont nulles, donc que ad $x$ est nilpotent. Par suite, $L(G)$ est nilpotente (chap. I, $\S 4$, cor. 1 du th. 1), donc G est nilpotent (prop. 12).

#### Proposition 15 {#lie-iii-s9-prop-15 .statement}

*Soient G un groupe de Lie nilpotent connexe de dimension finie sur $\mathbf{R}$ ou $\mathbf{C}$, A un sous-groupe intégral de G. Alors $Z_G(A)$ est le sous-groupe de Lie connexe de G d’algèbre de Lie $\delta_G(L(A))$.*

Compte tenu de la prop. 9 du n° 3 il suffit de prouver que $Z_G(A)$ est connexe. Soit $g \in Z_G(A)$. Il existe un $x \in L(G)$ tel que $g = \exp x$ (prop. 14). On a $\mathrm{Ad}\ g|L(A) = 1$ (n° 3, prop. 9), donc $\mathrm{Ad}\ g^n|L(A) = 1$ pour tout $n \in \mathbf{Z}$, donc $\exp (\mathrm{ad}\ nx)|L(A) = 1$ pour tout $n \in \mathbf{Z}$. Comme l’application $\lambda \mapsto \exp (\mathrm{ad}\ \lambda x)|L(A)$ de K dans $\mathcal{L}(L(A), L(G))$ est polynomiale, on a $\exp(\mathrm{ad}\ \lambda x)|L(A) = 1$ pour tout $\lambda \in K$, c’est-à-dire $\exp(\lambda x) \in Z_G(A)$ pour tout $\lambda \in K$.

#### Proposition 16 {#lie-iii-s9-prop-16 .statement}

*Soient G un groupe de Lie nilpotent de dimension finie sur $\mathbf{R}$ ou $\mathbf{C}$, A un sous-groupe intégral de G distinct de G. Alors $N_G(A)$ est un sous-groupe de Lie connexe de G distinct de A.*

On a $N_G(A) \neq A$ (A, I, $\S 6$, cor. 1 de la prop. 8). Compte tenu de la prop. 11 du n° 4, tout revient à prouver que $N_G(A)$ est connexe. Soit $g \in N_G(A)$. Il existe un $x \in L(G)$ tel que $g = \exp x$ (prop. 14). Soit E le sous-espace vectoriel de

L(\mathcal{L}(L(G))) formé des $u \in \mathcal{L}(L(G))$ tels que $u(L(A)) \subset L(A)$. On a Ad $g^n \in E$, donc $\exp(\mathrm{ad}\ nx) \in E$, pour tout $n \in \mathbf{Z}$. Donc $\exp(\mathrm{ad}\ \lambda x) \in E$ pour tout $\lambda \in K$, c’est-à-dire $\exp(\lambda x) \in N_G(A)$ pour tout $\lambda \in K$.

#### Proposition 17 {#lie-iii-s9-prop-17 .statement}

*Soient $g$ une algèbre de Lie nilpotente de dimension finie sur $K$, $(g_0, g_1, \ldots, g_n)$ une suite décroissante d’idéaux de $g$ tels que $g_0 = g, g_n = \{0\}, [g, g_1] \subset g_{i+1}$ pour $0 \leq i < n$. Soient $a_1, a_2, \ldots, a_p$ des sous-espaces vectoriels de $g$ tels que chaque $g_i$ soit somme directe de ses intersections avec les $a_j$. Munissons $g$ de la loi de composition de Hausdorff $\mathsf{H}$. Soit $\varphi$ l’application*

$$
(x_1, x_2, \ldots, x_p) \mapsto x_1 \mathsf{H} x_2 \mathsf{H} \ldots \mathsf{H} x_p
$$

*de $a_1 \times a_2 \times \cdots \times a_p$ dans $g$.
(i) $\varphi$ est une bijection de $a_1 \times a_2 \times \cdots \times a_p$ sur $g$;
(ii) $\varphi$ et $\varphi^{-1}$ sont des applications polynomiales;
(iii) l’application $(x, y) \mapsto \varphi^{-1}(\varphi(x) \cdot \varphi(y)^{-1})$ de $(a_1 \times a_2 \times \cdots \times a_p)^2$ dans $a_1 \times a_2 \times \cdots \times a_p$ est *polynomiale*.

La proposition est évidente pour $\dim g = 0$. Supposons $\dim g > 0$ et la proposition établie pour les dimensions $< \dim g$. On peut supposer $g_{n-1} \neq \{0\}$, et $g_{n-1}$ est alors un idéal central non nul de $g$. Il existe un indice $j$ tel que $\mathfrak{h} = g_{n-1} \cap a_j \neq \{0\}$. Soient $g' = g/\mathfrak{h}$, $\theta$ le morphisme canonique de $g$ sur $g'$, $g'_i = \theta(g_i), a'_i = \theta(a_i)$. Alors $(g'_0, g'_1, \ldots, g'_n)$ est une suite décroissante d’idéaux de $g'$ tels que $g'_0 = g', g'_n = \{0\}, [g', g'_i] \subset g'_{i+1}$ pour $0 \leq i < n$, et chaque $g'_i$ est somme directe de ses intersections avec les $a'_j$. Soit $\varphi'$ l’application

$$
(x'_1, x'_2, \ldots, x'_p) \mapsto x'_1 \mathsf{H} x'_2 \mathsf{H} \ldots \mathsf{H} x'_p
$$

*de $a'_1 \times a'_2 \times \cdots \times a'_p$ dans $g'$. D’après l’hypothèse de récurrence, $\varphi'$ est bijective et $\varphi', \varphi'^{-1}$ sont des applications polynomiales.

Soit $x \in g$. Posons

(1)
$$
\varphi'^{-1}(\theta(x)) = (x'_1(x), x'_2(x), \ldots, x'_p(x)).
$$
On a donc
(2)
$$
\theta(x) = x'_1(x) \mathsf{H} x'_2(x) \mathsf{H} \ldots \mathsf{H} x'_p(x).
$$
Soit $\mathfrak{h}_1$ un sous-espace vectoriel supplémentaire de $\mathfrak{h}$ dans $g$, somme des $a_k$ pour $k \neq j$ et d’un supplémentaire de $\mathfrak{h}$ dans $a_j$. Il existe une bijection $\eta$ de $g'$ sur $\mathfrak{h}_1$ telle que $\theta \circ \eta = \mathrm{Id}_{g'}$. Posons, pour $x \in g$,
(3)
$$
\zeta(x) = \eta(x'_1(x)) \mathsf{H} \eta(x'_2(x)) \mathsf{H} \ldots \mathsf{H} \eta(x'_p(x)) \in g.
$$
(4)
$$
y(x) = \zeta(x)^{-1} \mathsf{H} x = (-\zeta(x)) \cdot x.
$$
D’après (2) et (3), on a $\theta(\zeta(x)) = \theta(x)$, donc $y(x) \in \mathfrak{h}$. Posons enfin
(5)
$$
\psi(x) = (\eta(x'_1(x)), \ldots, \eta(x'_j(x)) + y(x), \ldots, \eta(x'_p(x))) \in a_1 \times \cdots \times a_p.
$$

Comme $y(x)$ est central dans $g$, on a
$$
\varphi(\psi(x)) = \eta(x_1'(x)) \circ \ldots \circ \eta(x_j'(x)) \circ \ldots \circ \eta(x_p'(x)) \circ y(x)
$$
$$
= \zeta(x) \circ y(x) \tag{d'après (3)}
$$
$$
= x \tag{d'après (4)}.
$$
Donc $\varphi \circ \psi = \mathrm{Id}_g$. Soit maintenant $(x_1, x_2, \ldots, x_p) \in a_1 \times a_2 \times \cdots \times a_p$, et posons $x = \varphi(x_1, x_2, \ldots, x_p) = x_1 \circ x_2 \circ \ldots \circ x_p$. On a $\theta(x) = \theta(x_1) \circ \theta(x_2) \circ \ldots \circ \theta(x_p)$, donc $x_i'(x) = \theta(x_i)$ pour $1 \leq i \leq p$, et par suite
$$
\zeta(x) = x_1 \circ x_2 \circ \ldots \circ (\eta \theta(x_j)) \circ \ldots \circ x_p
$$
$$
y(x) = x_j - \eta \theta(x_j).
$$
Alors, d’après (5),
$$
\psi(x) = (x_1, \ldots, \eta \theta(x_j) + x_j - \eta \theta(x_j), \ldots, x_p) = (x_1, x_2, \ldots, x_p).
$$
Donc $\psi \circ \varphi = \mathrm{Id}_{a_1 \times \ldots \times a_p}$. Cela prouve (i). Comme la loi de Hausdorff est polynomiale, $\varphi$ est polynomiale. D’après l’hypothèse de récurrence, $\varphi'^{-1}$ est polynomiale; d’après la formule (1), les fonctions $x_j'$ sont polynomiales, donc $\zeta$ est polynomiale (formule (3)), $y$ est polynomiale (formule (4)), $\psi$ est polynomiale (formule (5)). Cela prouve (ii). L’assertion (iii) résulte de (i) et (ii) et du fait que la loi de Hausdorff est polynomiale. C.Q.F.D.

Exemple de groupe de Lie nilpotent. — Soit G le sous-groupe trigonal strict inférieur de $\mathbf{GL}(n, K)$. C’est un sous-groupe de Lie de $\mathbf{GL}(n, K)$, et $L(G) \subset \mathfrak{gl}(n, K)$ est l’algèbre de Lie des matrices triangulaires inférieures de diagonale nulle (\S 3, n° 10, prop. 36). D’après le chap. II, § 4, n° 6, Remarque, G est nilpotent. Supposons désormais que $K = \mathbf{R}$ ou $\mathbf{C}$. Comme G est homéomorphe à $K^{n(n-1)/2}$, G est simplement connexe. L’application exponentielle de $L(G)$ dans G n’est autre que l’application
$$
u \mapsto \exp u = \sum_{k \geq 0} \frac{u^k}{k!} = \sum_{k=0}^{n-1} \frac{u^k}{k!}
$$
(\S 6, n° 4, Exemple). D’après la prop. 13, l’exponentielle est un isomorphisme de la variété $L(G)$ sur la variété G. La prop. 17 du \S 6, n° 9, fournit la bijection réciproque log. Munissons $K^n$ d’une norme. D’après TS, I, § 4, n° 9, on a pour $g \in G$ et $\|g - 1\| < 1$,
$$
\log g = \sum_{k \geq 1} \frac{(-1)^{k-1}}{k} (g - 1)^k
$$
c’est-à-dire
$$
\log g = \sum_{k=1}^{n-1} \frac{(-1)^{k-1}}{k} (g - 1)^k. \tag{6}
$$
Mais les deux membres de (6) sont des fonctions analytiques de $g$ pour $g \in G$, et sont donc égaux pour tout $g \in G$.

#### Proposition 18 {#lie-iii-s9-prop-18 .statement}

Soient k un corps commutatif, V un espace vectoriel de dimension finie > 0 sur k, G un sous-groupe de $\mathbf{GL}(V)$ dont les éléments sont unipotents.

(i) Il existe un élément non nul v de V tel que gv = v pour tout g ∈ G.

(ii) Il existe une base B de V telle que, pour tout g ∈ G, la matrice de g par rapport à B soit triangulaire inférieure et ait tous ses éléments diagonaux égaux à 1.

(iii) Le groupe G est nilpotent.

(a) Supposons d’abord que k soit algébriquement clos et que la représentation identique de G soit simple. Soient a, b dans G. Alors

$$
\operatorname{Tr}(a(b - 1)) = \operatorname{Tr}(ab - 1) - \operatorname{Tr}(a - 1) = 0 - 0 = 0
$$

car $ab - 1$ et $a - 1$ sont nilpotents. Comme le sous-espace vectoriel de $\mathcal{L}(V)$ engendré par G est $\mathcal{L}(V)$ (A, VIII, § 4, cor. 1 de la prop. 2), on a $\operatorname{Tr}(u(b - 1)) = 0$ pour tout $u \in \mathcal{L}(V)$, donc $b = 1$. Ainsi, $G = \{1\}$.

b) Passons au cas général. Soient $\overline{k}$ une clôture algébrique de k, $\overline{V} = V \otimes_k \overline{k}$, et $\overline{G} \subset \mathbf{GL}(\overline{V})$ l’ensemble des $a \otimes 1$ pour $a \in G$. Soit W (resp. W’) l’ensemble des éléments de V (resp. $\overline{V}$) invariants par G (resp. $\overline{G}$). On a $W' = W \otimes_k \overline{k}$ car $W = \bigcap_{g \in G} \operatorname{Ker}(g - 1)$ et $W' = \bigcap_{g \in G} \operatorname{Ker}(g - 1) \otimes 1$. Si $V_1$ désigne un élément minimal dans l’ensemble des sous-espaces vectoriels non nuls de $\overline{V}$ stables par $\overline{G}$, on a $V_1 \subset W'$ d’après la partie a) de la démonstration; donc $W \neq \{0\}$, ce qui prouve (i).

c) Par récurrence sur dim V, on déduit de (i) qu’il existe une suite croissante $(V_1, V_2, \ldots, V_n)$ de sous-espaces vectoriels de V stables par G tels que $V_n = V$ et que le groupe d’automorphismes de $V_i / V_{i-1}$ canoniquement déduit de G se réduit à $\{1\}$ pour tout i (on convient que $V_r = \{0\}$ pour $r \leq 0$). Cela entraîne d’abord (ii) et par conséquent (iii) (chap. II, § 4, n° 6, Remarque).

#### Corollaire 1 {#lie-iii-s9-prop-18-cor-1 .statement}

Soit G un groupe de Lie réel ou complexe connexe de dimension finie. Pour que G soit nilpotent, il faut et il suffit que tout élément de Ad G soit unipotent.

Si tout élément de Ad G est unipotent, Ad G est nilpotent (prop. 18), donc G, qui est extension centrale de Ad G, est nilpotent. Si G est nilpotent, L(G) est nilpotente, donc ad x est nilpotent pour tout $x \in L(G)$, donc $\operatorname{Ad}(\exp x) = \exp \operatorname{ad} x$ est unipotent; or tout élément de G est de la forme $\exp x$ pour un $x \in L(G)$ (prop. 14).

#### Corollaire 2 {#lie-iii-s9-prop-18-cor-2 .statement}

Tout sous-groupe analytique de $\mathbf{GL}(n, K)$ formé d’éléments unipotents est un sous-groupe de Lie simplement connexe.

Cela résulte des prop. 13 (ii), 18 (ii), et du fait que le groupe trigonal strict inférieur est simplement connexe.

### 6. Groupes de Lie résolubles

#### Proposition 19 {#lie-iii-s9-prop-19 .statement}

Soit G un groupe de Lie de dimension finie. Pour que L(G) soit résoluble, il faut et il suffit que G possède un sous-groupe ouvert résoluble.
La démonstration est analogue à celle de la prop. 12 du n° 5.

#### Proposition 20 {#lie-iii-s9-prop-20 .statement}

Soient G un groupe de Lie résoluble de dimension finie n sur R ou C, simplement connexe, et g = L(G). Soit (g_n, g_{n-1}, \ldots, g_0) une suite de sous-algèbres de g de dimensions n, n - 1, \ldots, 0, telle que g_{i-1} soit un idéal de g_i pour i = n, n - 1, \ldots, 1^1. Soit G_i le sous-groupe intégral de G correspondant à g_i. Soit x_i un vecteur de g_i n’appartenant pas à g_{i-1}. Soit \varphi_i l’application
$$(\lambda_1, \lambda_2, \ldots, \lambda_i) \mapsto (\exp \lambda_1 x_1)(\exp \lambda_2 x_2)\ldots(\exp \lambda_i x_i)$$
de K^i dans G. Alors \varphi_n est un isomorphisme de variétés analytiques, et \varphi_i(K^i) = G_i pour tout i.

Pour n = 0, la proposition est évidente. Raisonnons par récurrence sur n. Soit H le sous-groupe intégral de G tel que L(H) = Kx_n. D’après le § 6, n° 6, cor. 1 de la prop. 14, H et G_{n-1} sont des sous-groupes de Lie simplement connexes de G, et, en tant que groupe de Lie, G est produit semi-direct de H par G_{n-1}. Donc \lambda \mapsto \exp (\lambda x_n) est un isomorphisme de K sur H, et, d’après l’hypothèse de récurrence, l’application
$$(\lambda_1, \lambda_2, \ldots, \lambda_{n-1}) \mapsto (\exp \lambda_1 x_1)(\exp \lambda_2 x_2)\ldots(\exp \lambda_{n-1} x_{n-1})$$
est un isomorphisme de la variété analytique K^{n-1} sur la variété analytique G_{n-1} qui transforme K^i \times \{0\} en G_i pour i = 1, 2, \ldots, n - 1. D’où la proposition.

#### Proposition 21 {#lie-iii-s9-prop-21 .statement}

Soient G un groupe de Lie résoluble de dimension finie sur R ou C, simplement connexe, et M un sous-groupe intégral de G. Alors M est un sous-groupe de Lie de G, et est simplement connexe.

Reprenons les notations n, g, g_i, x_i, \varphi de la prop. 20, mais imposons aux x_i la condition supplémentaire suivante: soient i_p > i_{p-1} > \cdots > i_1 les entiers i tels que L(M) \cap g_i \neq L(M) \cap g_{i-1}; alors on prend x_{i_k} \in L(M) \cap g_{i_k} pour k = 1, 2, \ldots, p. Par récurrence sur n, on voit aisément que (x_{i_p}, x_{i_{p-1}}, \ldots, x_{i_1}) est une base de L(M). Soit N un groupe de Lie simplement connexe, tel qu’il existe un isomorphisme h de L(N) sur L(M). Soient y_p = h^{-1}(x_{i_p}), \ldots, y_1 = h^{-1}(x_{i_1}). D’après la prop. 20, l’application
$$(\lambda_1, \lambda_2, \ldots, \lambda_p) \mapsto (\exp \lambda_1 y_1)(\exp \lambda_2 y_2)\ldots(\exp \lambda_p y_p)$$
est un isomorphisme de la variété K^p sur la variété N. Il existe un morphisme \tau de

1 Une telle suite existe d’après le chap. I, § 5, prop. 2.

groupes de Lie de N dans G tel que $h = L(\tau)$, et on a $\tau(N) = M$ (\S 6, n° 2, cor. 1 de la prop. 1). Donc M est l’ensemble des éléments de G de la forme
$$
\tau((\exp \lambda_1 y_1) \ldots (\exp \lambda_p y_p)) = \exp(\lambda_1 L(\tau)y_1) \ldots \exp(\lambda_p L(\tau)y_p)
= \exp(\lambda_1 x_{i_1}) \ldots \exp(\lambda_p x_{i_p}).
$$
Ainsi, $M = \varphi(T)$ où T est un sous-espace vectoriel de $K^n$.

#### Proposition 22 {#lie-iii-s9-prop-22 .statement}

*On suppose $K = \mathbf{R}$ ou $\mathbf{C}$. Soient V un espace vectoriel de dimension finie, G un sous-groupe résoluble connexe de $\mathbf{GL}(V)$. On suppose que la représentation identique de G est simple.*
(i) *Si $K = \mathbf{R}$, on a $\dim V \leq 2$ et G est commutatif.*
(ii) *Si $K = \mathbf{C}$, on a $\dim V = 1$.*
(i) Supposons $K = \mathbf{R}$. Alors l’adhérence H de G dans $\mathbf{GL}(V)$ est un sous-groupe de Lie de $\mathbf{GL}(V)$, connexe, et résoluble (n° 1, cor. 2 de la prop. 1). Donc $L(H)$ est résoluble (prop. 19). La représentation identique de $L(G)$ est simple (\S 6, n° 5, cor. 2 de la prop. 13). Donc $\dim V \leq 2$ et $L(G)$ est commutative (chap. I, \S 5, cor. 1 et 4 du th. 1). Donc G est commutatif.
(ii) Supposons $K = \mathbf{C}$. Soit W un élément minimal parmi les sous-espaces vectoriels réels non nuls de V stables par G. Le sous-espace vectoriel complexe de V engendré par W est égal à V puisque la représentation identique de G est simple. D’après (i), $G|W$ est commutatif. Donc G est commutatif. Par suite, tout élément de G est une homothétie (A, VIII, \S 4, cor. 1 de la prop. 2), de sorte que $\dim V = 1$.

#### Corollaire {#lie-iii-s9-n6-cor-1 .statement}

*Soient V un espace vectoriel complexe de dimension finie > 0, G un sous-groupe résoluble connexe de $\mathbf{GL}(V)$.*
(i) *Il existe un élément non nul v de V tel que gv $\in \mathbf{C}v$ pour tout $g \in G$.*
(ii) *Il existe une base B de V tel que, pour tout $g \in G$, la matrice de g par rapport à B soit triangulaire inférieure.*
Soit $V_1$ un élément minimal parmi les sous-espaces vectoriels non nuls de V stables par G. D’après la prop. 22 (ii), on a $\dim V_1 = 1$. Cela prouve (i). Par récurrence sur $\dim V$, on déduit de là l’existence d’une suite croissante $(V_1, V_2, \ldots, V_n)$ de sous-espaces vectoriels de V stables par G tels que $\dim V_{i+1}/V_i = 1$ pour $i < n$, et $V_n = V$; d’où (ii).

### 7. Radical d’un groupe de Lie

#### Proposition 23 {#lie-iii-s9-prop-23 .statement}

*Soient G un groupe de Lie réel ou complexe de dimension finie, r le radical de $L(G)$ (chap. I, \S 5, déf. 2), n le plus grand idéal nilpotent de $L(G)$ (chap. I, \S 4, n° 4). Soit R (resp. N) le sous-groupe intégral de G d’algèbre de Lie r (resp. n). Alors R (resp. N) est un sous-groupe de Lie de G, résoluble (resp. nilpotent), invariant par tout automorphisme continu de G. Tout sous-groupe distingué connexe résoluble (resp. nilpotent) de G est contenu dans R (resp. N).

Le groupe R est résoluble (n° 6, prop. 19). Supposons K = R. Soit G' un sous-groupe distingué résoluble connexe de G. Alors $\overline{G}'$ est un sous-groupe de Lie de G ($\S 8, n° 2, th. 2$), distingué résoluble (n° 1, cor. 2 de la prop. 1), connexe. Donc L($\overline{G}'$) est un idéal résoluble de L(G), d’où L($\overline{G}'$) $\subset r$ et $\overline{G}' \subset R$. En particulier, $\overline{R} \subset R$, donc R est fermé et par suite est un sous-groupe de Lie de G. Supposons K = C. Soit H le groupe de Lie réel sous-jacent à G. Si r' est le radical de L(H), ir' est un idéal résoluble de L(H), d’où $r' = i r'$; on a donc $r \subset r' \subset r$, et, d’après ce qui précède, R est fermé dans H et par suite dans G; ainsi, R est un sous-groupe de Lie de G. Tout sous-groupe distingué résoluble connexe de G est un sous-groupe distingué résoluble connexe de H donc est contenu dans R. On a donc prouvé, pour K = C comme pour K = R, que R est le plus grand sous-groupe distingué résoluble connexe de G; par suite R est invariant par tout automorphisme continu de G. La démonstration dans le cas de N est entièrement analogue.

#### Définition 1 {#lie-iii-s9-def-1 .statement}

Soit G un groupe de Lie réel ou complexe de dimension finie. On appelle radical de G le plus grand sous-groupe distingué résoluble connexe de G.

#### Remarque {#lie-iii-s9-n7-rem-1 .statement}

Même si G est connexe, il peut exister des sous-groupes distingués résolubles de G non contenus dans le radical de G.

#### Proposition 24 {#lie-iii-s9-prop-24 .statement}

On suppose K = R ou C. Soient G_1, G_2 deux groupes de Lie connexes de dimension finie, R_1 et R_2 leurs radicaux, φ un morphisme surjectif de G_1 dans G_2. Alors $\varphi(R_1) = R_2$.

D’après le § 3, n° 8, prop. 28, L(φ) est surjectif. Donc L(φ)(L(R_1)) = L(R_2) (chap. I, § 6, cor. 3 de la prop. 2). Soit i l’injection canonique de R_1 dans G_1. Alors l’image de φ ∘ i est R_2 (§ 6, n° 2, cor. 1 de la prop. 1).

#### Proposition 25 {#lie-iii-s9-prop-25 .statement}

On suppose K = R ou C. Soient G_1, G_2 des groupes de Lie connexes de dimension finie, R_1 et R_2 leurs radicaux. Le radical de $G_1 \times G_2$ est $R_1 \times R_2$.

Cela résulte du chap. I, § 5, prop. 4.

### 8. Groupes de Lie semi-simples

#### Proposition 26 {#lie-iii-s9-prop-26 .statement}

Soit G un groupe de Lie réel ou complexe connexe de dimension finie. Les conditions suivantes sont équivalentes:
(i) L(G) est semi-simple;
(ii) le radical de G est {e};
(iii) tout sous-groupe intégral commutatif distingué de G est égal à {e}.
La condition (ii) signifie que le radical de L(G) est {0}, donc (i) ⇔ (ii) (chap. I, § 6, th. 1). L’équivalence de (i) et (iii) résulte du § 6, n° 6, prop. 14.

#### Définition 2 {#lie-iii-s9-def-2 .statement}

Un groupe de Lie réel ou complexe connexe est dit semi-simple s’il est de dimension finie et s’il vérifie les conditions de la prop. 26.

#### Remarque 1 {#lie-iii-s9-n8-rem-1 .statement}

Soit G un groupe de Lie réel ou complexe connexe de dimension finie. Si G n’est pas semi-simple, G possède un sous-groupe de Lie connexe G’ commutatif et invariant par tout automorphisme continu, tel que G’ ≠ {e}. En effet, soit n le plus grand idéal nilpotent de L(G) ; on a n ≠ {0}, et le sous-groupe analytique correspondant N est un sous-groupe de Lie invariant par tout automorphisme continu de G (no 7, prop. 23) ; le centre G’ de N possède les propriétés voulues.

#### Proposition 27 {#lie-iii-s9-prop-27 .statement}

Soit G un groupe de Lie réel ou complexe connexe de dimension finie. Les conditions suivantes sont équivalentes :
(i) L(G) est simple ;
(ii) les seuls sous-groupes intégraux distingués de G sont {e} et G, et en outre G n’est pas commutatif.
Cela résulte du § 6, no 6, prop. 14.

#### Définition 3 {#lie-iii-s9-def-3 .statement}

Un groupe de Lie réel ou complexe connexe est dit presque simple s’il est de dimension finie et s’il vérifie les conditions de la prop. 27.

#### Proposition 28 {#lie-iii-s9-prop-28 .statement}

Soit G un groupe de Lie réel ou complexe simplement connexe. Les conditions suivantes sont équivalentes :
(i) G est semi-simple ;
(ii) G est isomorphe au produit d’un nombre fini de groupes presque simples.
Si G est produit fini de groupes de Lie presque simples, L(G) est produit fini d’algèbres de Lie simples, donc est semi-simple. Si G est semi-simple, L(G) est isomorphe à un produit d’algèbres de Lie simples L₁, ..., Lₙ. Soit Gᵢ un groupe de Lie simplement connexe d’algèbre de Lie Lᵢ, donc presque simple. Alors G et G₁ × ... × Gₙ sont simplement connexes et ont des algèbres de Lie isomorphes, donc sont isomorphes.

#### Lemme 1 {#lie-iii-s9-lem-1 .statement}

Soient G un groupe topologique connexe, Z son centre, Z’ un sous-groupe discret de Z. Alors le centre de G/Z’ est Z/Z’.
Soit y un élément de G dont la classe modulo Z’ est un élément central de G/Z’. Soit φ l’application g ↦ gyg⁻¹y⁻¹ de G dans G. Alors φ(G) est connexe et contenu dans Z’, donc φ(G) = φ({e}) = {e}. Par suite, y ∈ Z.

#### Proposition 29 {#lie-iii-s9-prop-29 .statement}

Soit G un groupe de Lie réel ou complexe connexe semi-simple.
(i) G = (G, G).
(ii) Le centre Z de G est discret.
(iii) Le centre de G/Z est {e}.

L’assertion (i) résulte du cor. de la prop. 4, n° 2, et du chap. I, § 6, th. 1.
L’assertion (ii) résulte du § 6, n° 4, cor. 4 de la prop. 10, et du chap. I, § 6, n° 1, Remarque 2.
L’assertion (iii) résulte de (ii) et du lemme 1.

#### Proposition 30 {#lie-iii-s9-prop-30 .statement}

(i) Soit $g$ une algèbre de Lie réelle ou complexe semi-simple. Alors Int $g$ est la composante neutre de Aut $g$.
(ii) Soit $G$ un groupe de Lie réel ou complexe connexe semi-simple. Le groupe adjoint de $G$ est la composante neutre de Aut $L(G)$. Son centre est réduit à l’élément neutre.
Toute dérivation de $g$ est intérieure (chap. I, § 6, cor. 3 de la prop. 1), donc $L(\mathrm{Int}\,g) = L(\mathrm{Aut}\,g)$, ce qui prouve (i). La première assertion de (ii) résulte de (i). La seconde résulte de la prop. 29 (iii) et du § 6, n° 4, cor. 4 (ii) de la prop 10.

#### Remarque 2 {#lie-iii-s9-n8-rem-2 .statement}

Soient $g$ une algèbre de Lie semi-simple complexe, $g_0$ l’algèbre de Lie réelle sous-jacente. Alors Aut$(g)$ est ouvert dans Aut$(g_0)$. En effet, Int $(g_0) \subset \mathrm{Aut}\,(g)$.

#### Proposition 31 {#lie-iii-s9-prop-31 .statement}

Soient $G$ un groupe de Lie réel ou complexe de dimension finie simplement connexe, $R$ son radical. Il existe un sous-groupe de Lie simplement connexe semi-simple $S$ de $G$ tel que $G$ soit, en tant que groupe de Lie, produit semi-direct de $S$ par $R$. Si $S'$ est un sous-groupe intégral semi-simple de $G$, il existe un $x$ dans le radical nilpotent de $L(G)$ tel que $(\mathrm{Ad}\,\exp\,x)(S') \subset S$.
Cela résulte du § 6, n° 6, cor. 1 de la prop. 14, et du chap. I, § 6, th. 5 et cor. 1.

#### Lemme 2 {#lie-iii-s9-lem-2 .statement}

Soient $G$ un groupe (resp. un groupe topologique), $G'$ un sous-groupe distingué de $G$, $V$ un espace vectoriel de dimension finie sur un corps commutatif $k$ (resp. sur $K$), $\rho$ une représentation linéaire (resp. une représentation linéaire continue) de $G$ dans $V$, et $\rho' = \rho|G'$.
(i) Si $\rho$ est semi-simple, $\rho'$ est semi-simple.
(ii) Si $\rho'$ est semi-simple, et si toute $k$-représentation linéaire (resp. toute $K$-représentation linéaire continue) de dimension finie de $G/G'$ (resp. $G/\overline{G}'$) est semi-simple, alors $\rho$ est semi-simple.
Supposons $\rho$ semi-simple, et prouvons que $\rho'$ est semi-simple. Il suffit d’envisager le cas où $\rho$ est simple. Soit $V'$ un sous-$G'$-module non nul minimal de $V$. Pour tout $g \in G$, on a $\rho(G')\rho(g)V' = \rho(g)\rho(G')V' = \rho(g)V'$, autrement dit $\rho(g)V'$ est stable par $\rho(G')$; si $V''$ est un sous-$G'$-module de $\rho(g)V'$, alors $\rho(g)^{-1}V''$ est un sous-$G'$-module de $V'$, donc $V''$ est égal à $\{0\}$ ou à $\rho(g)V'$. Ainsi, pour tout $g \in G$, $\rho(g)V'$ est un $G'$-module simple. Or $\sum_{g \in G} \rho(g)V'$ est un sous-$G$-module non nul de $V$, d’où $V = \sum_{g \in G} \rho(g)V'$. Donc $\rho'$ est semi-simple.
Supposons $\rho'$ semi-simple. Soit $W$ un sous-$G$-module non nul de $V$. Comme $\rho'$ est semi-simple, il existe un projecteur $f_0$ de $V$ sur $W$ commutant à $\rho(G')$. Soit

E l’ensemble des $f \in \mathcal{L}(V, V)$ qui commutent à $\rho(G')$, qui appliquent V dans W, et dont la restriction à W est une homothétie; pour $f \in E$, notons $\alpha(f)$ le rapport de l’homothétie $f|W$. On a $f_0 \in E$ et $\alpha(f_0) = 1$. Il est clair que $\alpha$ est une forme linéaire sur E. Soit F = Ker $\alpha$, qui est un hyperplan de E. Pour $f \in E$ et $g \in G$, posons $\sigma(g)f = \rho(g) \circ f \circ \rho(g)^{-1}$; alors $\sigma(g)f$ applique V dans W et sa restriction à W cst l’homothétie de rapport $\alpha(f)$; si $g' \in G'$, on a

$$
\begin{align*}
\sigma(g)f \circ \rho(g') &= \rho(g) \circ f \circ \rho(g)^{-1} \circ \rho(g') \\
&= \rho(g) \circ f \circ \rho(g^{-1}g'g) \circ \rho(g^{-1}) \\
&= \rho(g) \circ \rho(g^{-1}g'g) \circ f \circ \rho(g^{-1}) \\
&= \rho(g') \circ \rho(g) \circ f \circ \rho(g^{-1}) \\
&= \rho(g') \circ \sigma(g)f.
\end{align*}
$$

Donc $\sigma(g)f \in E$. Par suite $\sigma$ est une k-représentation linéaire (resp. une K-représentation linéaire continue) de G dans E laissant stable F. On a $\sigma(g) = \mathrm{Id}_E$ pour $g \in G'$, donc pour $g \in \overline{G}'$ dans le cas topologique. Supposons que toute représentation $k$-linéaire (resp. toute représentation K-linéaire continue) de dimension finie de $G/G'$ (resp. $G/\overline{G}'$) soit semi-simple. Alors il existe dans E un supplémentaire de F stable pour G. Autrement dit, il existe un $f \in E$ tel que $\alpha(f) = 1$, invariant par G. Alors $f$ est un projecteur de V sur W, et, pour $g \in G$, on a $\rho(g) \circ f \circ \rho(g^{-1}) = f$, c’est-à-dire que $f$ commute à $\rho(G)$. Ainsi, $\rho$ est semi-simple.

#### Théorème 1 {#lie-iii-s9-thm-1 .statement}

Soient G un groupe de Lie réel ou complexe de dimension finie, $G_0$ sa composante neutre, R son radical, r le radical de $L(G)$; on suppose que $G/G_0$ est fini. Soit $\rho$ une représentation linéaire analytique de G de dimension finie. Les conditions suivantes sont équivalentes:
(i) $\rho$ est semi-simple;
(ii) $\rho|G_0$ est semi-simple;
(iii) $\rho|R$ est semi-simple;
(iv) $L(\rho)$ est semi-simple;
(v) $L(\rho)|r$ est semi-simple.
On a (i) $\Leftrightarrow$ (ii) d’après le lemme 2 et INT, VII, § 3, prop. 1. On a (ii) $\Leftrightarrow$ (iv) et (iii) $\Leftrightarrow$ (v) d’après le § 6, n° 5, cor. 2 de la prop. 13. On a (iv) $\Leftrightarrow$ (v) d’après le chap. I, § 6, th. 4.

#### Corollaire 1 {#lie-iii-s9-thm-1-cor-1 .statement}

Soient $\rho, \rho_1, \rho_2$ des représentations linéaires analytiques semi-simples de dimension finie de G et n un entier $\geq 0$. Alors $\rho_1 \otimes \rho_2, T^n \rho, S^n \rho, \wedge^n \rho$ (Appendice) sont semi-simples.
La semi-simplicité de $\rho_1 \otimes \rho_2$ résulte du th. 1, et du chap. I, § 6, cor. 1 du th. 4. La semi-simplicité de $T^n \rho, S^n \rho, \wedge^n \rho$ résulte de la semi-simplicité de $\rho_1 \otimes \rho_2$.

Nous verrons plus tard que si $k$ est un corps commutatif de caractéristique 0, $\Gamma$ un groupe, $\rho_1$ et $\rho_2$ des $k$-représentations linéaires semi-simples de dimension finie de $\Gamma$, alors $\rho_1 \otimes \rho_2$ est semi-simple.

#### Corollaire 2 {#lie-iii-s9-thm-1-cor-2 .statement}

*Soient $\rho$ une représentation linéaire analytique semi-simple de dimension finie de $G$ dans un espace vectoriel $V$, $S$ l’algèbre symétrique de $V$, et $S^G$ la sous-algèbre de $S$ formée des éléments invariants par $(S\rho)(G)$. Alors $S^G$ est une algèbre de type fini.*
    Cela résulte du th. 1, du chap. I, § 6, th. 6 a), et de AC, V, § 1, th. 2.

#### Corollaire 3 {#lie-iii-s9-thm-1-cor-3 .statement}

*Soient $G$ un groupe de Lie réel ou complexe, $G_0$ sa composante neutre. On suppose que $G_0$ est semi-simple et que $G/G_0$ est fini. Alors toute représentation linéaire analytique de dimension finie de $G$ est semi-simple.*

#### Proposition 32 {#lie-iii-s9-prop-32 .statement}

*Soit $G$ un groupe de Lie réel connexe de dimension finie. On suppose $L(G)$ réductive. Les conditions suivantes sont équivalentes*:
    (i) $G/\overline{D^1}G$ est compact;
    (ii) (resp. (ii')) toute représentation linéaire analytique de dimension finie de $G$ dans un espace vectoriel complexe (resp. réel) est semi-simple.

(i) $\Rightarrow$ (ii') : Supposons $G/\overline{D^1}G$ compact. Alors toute représentation linéaire continue de $G/\overline{D^1}G$ dans un espace vectoriel réel de dimension finie est semi-simple (INT, VII, § 3, prop. 1). Soit $\rho$ une représentation linéaire analytique de dimension finie de $G$ dans un espace vectoriel réel. Alors $\rho|D^1G$ est analytique, $D^1G$ est semi-simple (chap. I, § 6, prop. 5), donc $\rho|D^1G$ est semi-simple (cor. 3 du th. 1). Donc $\rho$ est semi-simple (lemme 2).

On voit de même que (ii) $\Rightarrow$ (i).

(ii') $\Rightarrow$ (i) : supposons que $G/\overline{D^1}G$ soit non compact, donc isomorphe à un groupe de la forme $\mathbf{R}^p \times \mathbf{T}^q$ avec $p > 0$ ($\S 6$, n° 4, prop. 11 (ii)). Il existe alors un morphisme surjectif de $G/\overline{D^1}G$ dans $\mathbf{R}$, donc un morphisme surjectif $\rho$ de $G$ dans $\mathbf{R}$. L’application
$$
g \mapsto \sigma(g) = \begin{pmatrix} 1 & 0 \\ \rho(g) & 1 \end{pmatrix}
$$
est une représentation linéaire analytique de $G$ dans $\mathbf{R}^2$ qui n’est pas semi-simple, car le seul sous-espace vectoriel de dimension 1 de $\mathbf{R}^2$ stable par $\sigma(G)$ est $\mathbf{R}(0, 1)$.

On voit de même que (ii) $\Rightarrow$ (i).

#### Proposition 33 {#lie-iii-s9-prop-33 .statement}

*Soient $G$ un groupe de Lie complexe de dimension finie et dont le nombre de composantes connexes est fini, $\rho$ une représentation linéaire analytique de $G$ de dimension finie, $G'$ un sous-groupe intégral du groupe de Lie réel $G$ tel que $L(G')$ engendre $L(G)$ sur $\mathbf{C}$. Alors, pour que $\rho$ soit semi-simple, il faut et il suffit que $\rho|G'$ soit semi-simple.*
    Soit $\rho' = \rho|G'$. Pour que $\rho$ (resp. $\rho'$) soit semi-simple, il faut et il suffit que $L(\rho)$ (resp. $L(\rho')$) soit semi-simple (th. 1). Soit $V$ l’espace de $\rho$. Pour qu’un sous-espace vectoriel de $V$ soit stable pour $L(\rho)(L(G))$, il faut et il suffit qu’il soit stable pour $L(\rho')(L(G'))$. D’où la proposition.

## EXERCICES {#lie-iii-s9-exercises}

See the [exercises for § 9](exercises/s9/).
