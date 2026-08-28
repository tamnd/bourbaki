---
book: int
book_title: Integration
chapter: IV
chapter_title: Prolongement d'une mesure. Espaces $L^p$
section: 2
section_title: Fonctions et ensembles négligeables
lang: fr
source: int-i-iv-fr
pdf_pages: 0120-0127
extraction: ocr
subsections:
    - "no": 1
      title: Fonctions positives négligeables
      page: 0
      pdf_page: 120
    - "no": 2
      title: Ensembles négligeables
      page: 0
      pdf_page: 121
    - "no": 3
      title: Propriétés vraies presque partout
      page: 0
      pdf_page: 122
    - "no": 4
      title: Classes de fonctions équivalentes
      page: 0
      pdf_page: 123
    - "no": 5
      title: Fonctions définies presque partout
      page: 0
      pdf_page: 125
    - "no": 6
      title: Classes d’équivalence de fonctions à valeurs dans $\bar{\mathbf{R}}$
      page: 0
      pdf_page: 126
statements: 15
exercises: 0
content_sha256: a972bec1a97a6ae98c38d6651435818b6e27108e993a851d20ed336bf9d34e48
---

## § 2. Fonctions et ensembles négligeables

### 1. Fonctions positives négligeables

#### Définition 1 {#int-iv-s2-def-1 .statement}

*Etant donnée une mesure $\mu$ sur un espace localement compact X, on dit qu’une fonction numérique $f \geq 0$ (finie ou non) définie dans X est négligeable pour la mesure $\mu$ si l’on a $|\mu|^*(f) = 0$.*

On dit aussi alors que $f$ est $\mu$-négligeable, ou simplement négligeable si aucune confusion n’en résulte.

#### Proposition 1 {#int-iv-s2-prop-1 .statement}

*Si $f$ est une fonction négligeable $\geqslant 0$, toute fonction numérique $g$ telle que $0 \leqslant g \leqslant \alpha f$ ($\alpha$ scalaire $> 0$) est négligeable.*
En effet, on a $0 \leqslant |\mu|^*(g) \leqslant \alpha|\mu|^*(f) = 0$.

#### Proposition 2 {#int-iv-s2-prop-2 .statement}

*La somme et l’enveloppe supérieure d’une suite $(f_n)$ de fonctions négligeables $\geqslant 0$ sont négligeables.*
En effet, on a $|\mu|^*\left( \sum_n f_n \right) \leqslant \sum_n |\mu|^*(f_n) = 0$ ($§ 1$, no 3, prop. 13) et $\sup_n f_n \leqslant \sum_n f_n$.

#### Proposition 3 {#int-iv-s2-prop-3 .statement}

*Pour qu’une fonction $f \geqslant 0$, semi-continue inférieurement dans $X$, soit négligeable, il faut et il suffit que $f$ soit nulle dans le support de $\mu$.*
En effet, si $|\mu|^*(f) = 0$, on a $|\mu|(g) = 0$ pour toute fonction $g \in \mathcal{K}_+$ telle que $g \leqslant f$; il en résulte (chap. III, $§ 2$, no 3, prop. 9) que $g$ est nulle dans le support $S$ de $\mu$; comme $f$ est l’enveloppe supérieure des fonctions $g \in \mathcal{K}_+$ telles que $g \leqslant f$ ($§ 1$, no 1, lemme 1), on a $f(x) = 0$ dans $S$. Réciproquement, si $f(x) = 0$ dans $S$, on a $g(x) = 0$ dans $S$ pour toute fonction $g \in \mathcal{K}_+$ telle que $g \leqslant f$, et par suite (chap. III, $§ 3$, no 3, prop. 8) $|\mu|(g) = 0$, ce qui, par définition, entraîne $|\mu|^*(f) = 0$.

### 2. Ensembles négligeables

#### Définition 2 {#int-iv-s2-def-2 .statement}

*Etant donnée une mesure $\mu$ sur un espace localement compact $X$, on dit qu’une partie $A$ de $X$ est négligeable pour la mesure $\mu$ si $|\mu|^*(A) = 0$.*
On dit encore que $A$ est $\mu$-négligeable, ou simplement négligeable si aucune confusion n’en résulte. Il revient au même de dire que la fonction caractéristique $\varphi_A$ est négligeable.

#### Proposition 4 {#int-iv-s2-prop-4 .statement}

*Toute partie d’un ensemble négligeable est négligeable ; toute réunion dénombrable d’ensembles négligeables est négligeables.*
C’est une conséquence immédiate des prop. 1 et 2.

#### Exemple {#int-iv-s2-n2-exa-1 .statement}

Soit $\mu$ la mesure de Lebesgue sur $\mathbf{R}$. Tout ensemble $\{ x_0 \}$ réduit à un point est négligeable (cf. $§ 1$, no 3, Remarque 1). Il en résulte que toute partie dénombrable de $\mathbf{R}$ est négligeable pour la mesure de Lebesgue. La réciproque de cette proposition est inexacte ($§ 4$, exerc. 4 b)).

#### Proposition 5 {#int-iv-s2-prop-5 .statement}

Le complémentaire du support S de $\mu$ est le plus grand ensemble ouvert négligeable dans X.

En effet, d’après la prop. 3, pour qu’un ensemble ouvert G soit négligeable, il faut et il suffit que $G \cap S = \varnothing$, c’est-à-dire $G \subset \complement S$.

### 3. Propriétés vraies presque partout

Soient X un espace localement compact, $\mu$ une mesure sur X. Si $P\{x\}$ est une propriété, la propriété « $P\{x\}$ presque partout (par rapport à $\mu$) » est par définition équivalente à la propriété « l’ensemble des x tels que $(x \in X \text{ et non } P\{x\})$ est $\mu$-négligeable ».

#### Théorème 1 {#int-iv-s2-thm-1 .statement}

Pour qu’une fonction numérique (finie ou non) $f \geqslant 0$ définie dans X soit négligeable, il faut et il suffit que $f(x) = 0$ presque partout.

La condition est nécessaire. En effet, supposons que $f$ soit négligeable, et soit N l’ensemble des $x \in X$ tels que $f(x) \neq 0$; on a $\varphi_N \leqslant \sup_n (n f)$, donc $\varphi_N$ est négligeable (n° 1, prop. 1 et 2).

La condition est suffisante. Supposons en effet que l’ensemble N des points où $f(x) \neq 0$ soit négligeable ; on a alors $f \leqslant \sup_n n \varphi_N$, donc $f$ est négligeable (n° 1, prop. 1 et 2).

#### Proposition 6 {#int-iv-s2-prop-6 .statement}

Si $f$ et $g$ sont deux fonctions $\geqslant 0$ (finies ou non) définies dans X et telles que $f(x) = g(x)$ presque partout, on a $|\mu|^*(f) = |\mu|^*(g)$.

En effet, soit N l’ensemble négligeable des points $x \in X$ tels que $f(x) \neq g(x)$. Les fonctions $\inf(f, g)$ et $\sup(f, g)$ étant égales sauf aux points de N, il suffit de démontrer la proposition lorsque $f \leqslant g$. Soit $h$ la fonction égale à $+ \infty$ aux points de N, à 0 dans $\complement N$; on a $f \leqslant g \leqslant f + h$, d’où

$$
|\mu|^*(f) \leqslant |\mu|^*(g) \leqslant |\mu|^*(f + h) \leqslant |\mu|^*(f) + |\mu|^*(h) = |\mu|^*(f)
$$

(puisque $h$ est négligeable), d’où la proposition.

#### Proposition 7 {#int-iv-s2-prop-7 .statement}

Si $f$ est une fonction $\geqslant 0$ définie dans X et telle que $|\mu|^*(f) < +\infty$, $f(x)$ est fini presque partout.

En effet, soit N l’ensemble des points $x \in X$ tels que f(x) = +\infty ; pour tout entier n, on a n\varphi_N \leq f, d’où
n|\mu|^*(\varphi_N) \leq |\mu|^*(f);
comme n est arbitrairement grand, on a |\mu|^*(\mathbf{N}) = 0.

Par contre, même lorsque X est compact, une fonction f \geq 0 définie dans X et partout finie peut avoir une intégrale supérieure infinie, comme le montre l’exemple où X = \{0, 1\}, f(x) = 1/x pour x > 0 et f(0) = 0, \mu étant la mesure de Lebesgue sur X.

### 4. Classes de fonctions équivalentes

Soit \mu une mesure sur un espace localement compact X. Etant donné un ensemble F, on dit que deux applications f, g de X dans F sont équivalentes par rapport à \mu (ou \mu-équivalentes, ou simplement équivalentes si aucune confusion n’en résulte) si l’on a f(x) = g(x) presque partout dans X. Comme la réunion de deux ensembles négligeables est négligeable, on définit bien ainsi une relation d’équivalence dans l’ensemble F^X de toutes les applications de X dans F; quand nous parlerons de classe d’équivalence d’une telle fonction f (sans préciser davantage), il sera sous-entendu qu’il s’agit de la classe des fonctions égales presque partout à f ; dans ce chapitre et les suivants, nous désignerons cette classe par la notation \tilde{f}.

#### Proposition 8 {#int-iv-s2-prop-8 .statement}

Soit (F_n) une famille dénombrable (finie ou infinie) d’ensembles. Pour tout indice n, soient f_n, g_n deux applications équivalentes de X dans F_n; alors il existe un ensemble négligeable H tel que, pour tout x \notin H, on ait f_n(x) = g_n(x) pour tout n.

En effet, l’ensemble H_n des x \in X tels que f_n(x) \neq g_n(x) est négligeable, donc il en est de même de leur réunion H (n° 2, prop. 4) et cet ensemble répond à la question.

#### Corollaire {#int-iv-s2-n4-cor-1 .statement}

Si \varphi est une application de \prod_n F_n dans un ensemble G, les applications \varphi((f_n)) et \varphi((g_n)) de X dans G sont équivalentes.

On désignera par \varphi((\tilde{f}_n)) la classe d’équivalence de toute fonction \varphi((f_n)), lorsque f_n est une fonction arbitraire de la classe \tilde{f}_n.

En particulier, si F est un espace vectoriel sur \mathbf{R}, on définit \tilde{f} + \tilde{g} et \alpha \tilde{f} comme classes d’équivalence de f + g et \alpha f respectivement (f et g applications de X dans F, α scalaire); on obtient ainsi, sur l’ensemble des classes d’équivalence des applications de X dans F, une structure d’espace vectoriel: c’est d’ailleurs la structure d’espace quotient de celle de $F^X$ par le sous-espace des applications f telles que $\tilde{f} = \tilde{0}$ (fonctions nulles presque partout) qu’on appelle encore fonctions négligeables (à valeurs dans F). On définit de même le produit $\tilde{g}\tilde{f}$, où $\tilde{f}$ est une classe d’équivalence d’applications de X dans F, et $\tilde{g}$ une classe d’équivalence de fonctions numériques (finies) définies dans X: l’ensemble des classes d’équivalence d’applications de X dans F est ainsi muni d’une structure de module sur l’ensemble des classes d’équivalence des fonctions numériques finies définies dans X (lui-même muni d’une structure d’anneau). Si F est une algèbre sur $\mathbf{R}$, on définit de même une structure d’algèbre sur l’ensemble des classes d’équivalence d’applications de X dans F.

Soit F un espace topologique métrisable, et considérons sur F une structure uniforme compatible avec sa topologie, et définie par une famille dénombrable d’écarts $\rho_n$ (Top. gén., chap. IX, §§ 1 et 2); pour que deux applications $f, g$ de X dans F soient équivalentes, il faut et il suffit que les fonctions numériques $\rho_n(f, g)$ soient négligeables; cela équivaut en effet à dire qu’il existe dans X un ensemble négligeable H tel que, pour tout $x \notin H$, on ait $\rho_n(f(x), g(x)) = 0$ pour tout $n$, c’est-à-dire $f(x) = g(x)$. En particulier, si F est un espace localement convexe métrisable, $(q_n)$ une famille dénombrable de semi-normes définissant la topologie de F (Esp. vect. top., chap. II, 2e éd., § 4, n° 1), pour que deux applications $f, g$ de X dans F soient équivalentes, il faut et il suffit que les fonctions numériques $q_n(f(x) - g(x))$ soient toutes négligeables.

#### Proposition 9 {#int-iv-s2-prop-9 .statement}

*Soient f et g deux applications continues de X dans un espace topologique séparé F; pour que f et g soient équivalentes, il faut et il suffit que $f(x) = g(x)$ en tout point du support de $\mu$.*

En effet, l’ensemble des $x \in X$ tels que $f(x) \neq g(x)$ est un ensemble ouvert (Top. gén., chap. I, 3e éd., § 8, n° 1); pour qu’il soit négligeable, il faut et il suffit qu’il ne rencontre pas le support de $\mu$ (n° 2, prop. 5).

#### Proposition 10 {#int-iv-s2-prop-10 .statement}

*Soit F un espace localement convexe séparé sur $\mathbf{R}$ tel qu’il existe dans le dual $F'$ de F une suite $(\mathbf{a}'_n)$ partout dense pour la topologie faible $\sigma(F', F)$ (Esp. vect. top., chap. II, 2e éd., § 6, n° 2). Pour que deux applications f, g de X dans F soient équivalentes, il faut et il suffit que, pour tout n, les fonctions numériques $\langle f(x), a'_n \rangle$ et $\langle g(x), a'_n \rangle$ soient équivalentes.

La condition est évidemment nécessaire. Inversement, si elle est remplie, il existe un ensemble négligeable H tel que, pour tout $x \notin H$, on ait $\langle f(x), a'_n \rangle = \langle g(x), a'_n \rangle$ pour tout n ; cela signifie que les formes linéaires faiblement continues sur F', $z' \mapsto \langle f(x), z' \rangle$ et $z' \mapsto \langle g(x), z' \rangle$ sont égales en chacun des points $a'_n$, donc sont identiques en vertu de l’hypothèse, ce qui prouve que $f(x) = g(x)$ pour tout $x \notin H$.

On notera que l’hypothèse de la prop. 10 s’applique en particulier lorsque F est un espace localement convexe métrisable et de type dénombrable (Esp. vect. top., chap. IV, § 2, n° 2, cor. de la prop. 3).

### 5. Fonctions définies presque partout

Conformément à la définition du n° 3, une application f d’une partie A de X dans un ensemble F est dite définie presque partout si le complémentaire de l’ensemble A où elle est définie est un ensemble négligeable. On appelle encore classe d’équivalence de f, et on note $\tilde{f}$, la classe d’équivalence de toute fonction définie dans X tout entier et égale à $f(x)$ aux points $x \in X$ où $f$ est définie ; il est clair que cette classe ne dépend que de $f$. On dit encore que deux fonctions $f, g$, définies presque partout, sont équivalentes, si $\tilde{f} = \tilde{g}$ : cela signifie donc que l’ensemble des points où $f(x)$ et $g(x)$ sont tous deux définis et égaux a un complémentaire négligeable.

On en déduit aussitôt que la prop. 8 du n° 4 et son corollaire se généralisent au cas où, dans leur énoncé, on suppose seulement que chacune des fonctions $f_n, g_n$ est définie presque partout ; les fonctions $\varphi((f_n))$ et $\varphi((g_n))$ sont alors, elles aussi, définies presque partout ; la classe d’équivalence de $\varphi((f_n))$ est encore $\varphi((\tilde{f}_n))$.

Une fonction définie presque partout, à valeurs dans un espace vectoriel F, est encore dite négligeable si elle est équivalente à 0. Si $f$ est une fonction négligeable à valeurs dans F, et $u$ une application linéaire de F dans un espace vectoriel G, la fonction composée $u \circ f$ (définie presque partout), est négligeable ; de même, pour toute fonction numérique (finie) $g$, définie presque partout, la fonction $gf$ (définie presque partout) est négligeable.

On aura soin d’observer que, dans l’ensemble des fonctions à valeurs dans F et définies presque partout, la loi de composition interne $(f, g) \mapsto f + g$ n’est pas une loi de groupe, car la fonction 0 est bien élément neutre pour cette loi, mais si $f$ n’est pas partout définie, il n’existe pas de fonction $g$ telle que $f + g = 0$. C’est ce qui motive l’introduction des classes d’équivalence $\tilde{f}$ qui, elles, forment un espace vectoriel.

Soit $(f_n)$ une suite d’applications dans un espace topologique F, chacune d’elles étant définie presque partout dans X. On dit que la suite $(f_n)$ converge (simplement) presque partout vers $f$ dans X si l’ensemble des points $x \in X$ où tous les $f_n(x)$ sont définis et où la suite $(f_n(x))$ a une limite égale à $f(x)$, a un complémentaire négligeable. Il est clair que si, pour chaque $n$, la fonction $g_n$ (définie presque partout) est équivalente à $f_n$, la suite $(g_n)$ converge presque partout vers $f$.

Si F est un espace vectoriel topologique, on définit de même une série presque partout convergente dont le terme général est une fonction $f_n$ définie presque partout dans X et à valeurs dans F ; la somme de cette série est une fonction définie aux points où les sommes partielles $\sum_{k=1}^n f_k(x)$ sont définies et ont une limite, et sa classe ne dépend que des classes $\tilde{f}_n$.

### 6. Classes d’équivalence de fonctions à valeurs dans $\bar{\mathbf{R}}$

Conformément à la définition du n° 3, on dit qu’une fonction $f$, définie presque partout dans X, et à valeurs dans $\bar{\mathbf{R}}$, est finie presque partout si l’ensemble des $x \in X$ pour lesquels $f(x)$ est défini et fini a un complémentaire négligeable. Une fonction finie presque partout est équivalente à une fonction partout finie ; on peut donc identifier sa classe $\tilde{f}$ à une classe de fonctions numériques finies définies dans X (ou presque partout dans X). En particulier, la somme et le produit de deux classes de fonctions finies presque partout sont définis, et l’ensemble de ces classes est une algèbre sur $\mathbf{R}$. Si $(f_n)$ est une suite de fonctions à valeurs dans $\bar{\mathbf{R}}$, définies et finies presque partout, les sommes partielles $\sum_{k=1}^n f_k(x)$ sont définies presque partout ; si, pour presque tout $x \in X$, elles ont une limite $f(x)$ dans $\bar{\mathbf{R}}$, on dit encore que la série de terme général $f_n$ converge presque partout et que $f$ est la somme de cette série (on notera que $f$ n’est pas nécessairement finie presque partout).

Si $f$ et $g$ sont deux fonctions numériques définies et finies presque partout dans X, $\tilde{f} + \tilde{g}$ (resp. $\tilde{f}\tilde{g}$) est la classe de toute fonction égale à $f(x) + g(x)$ (resp. $f(x)g(x)$) aux points $x \in X$ où cette expression a un sens. On notera que $f$ et $g$ peuvent être *partout définies* toutes deux sans que $f(x) + g(x)$ (resp. $f(x)g(x)$) soit défini pour tout $x$ (*Top. gén.*, chap. IV, § 4, n° 3); par définition $f + g$ (resp. $fg$) est alors la fonction égale à $f(x) + g(x)$ (resp. $f(x)g(x)$) aux points où cette expression est définie; elle est donc seulement définie presque partout.

Soient $f$ et $g$ deux fonctions numériques (finies ou non) définies presque partout dans $X$ et telles que $f(x) \leq g(x)$ presque partout; si $f_1$ est équivalente à $f$ et $g_1$ équivalente à $g$, il est clair que l’on a aussi $f_1(x) \leq g_1(x)$ presque partout. La relation considérée ne dépend donc que des classes de $f$ et de $g$; on l’écrit $\tilde{f} \leq \tilde{g}$, et on vérifie aussitôt que cette relation est une *relation d’ordre* dans l’ensemble des classes d’équivalence des fonctions à valeurs dans $\bar{\mathbf{R}}$. Si $(\tilde{f}_n)$ est une famille dénombrable (finie ou infinie) de ces classes, et si, pour tout $n$, $f_n$ et $g_n$ sont deux fonctions définies presque partout, appartenant à la classe $\tilde{f}_n$, il résulte de la prop. 8 du n° 4 que les fonctions $\sup_{n} f_n$ et $\sup_{n} g_n$, définies presque partout, sont équivalentes; leur classe ne dépend donc que des classes $\tilde{f}_n$, et l’on vérifie aussitôt que c’est la *borne supérieure* $\sup_{n} \tilde{f}_n$ de ces classes dans l’ensemble des classes de fonctions à valeurs dans $\bar{\mathbf{R}}$, ordonné comme il vient d’être dit (ensemble qui en particulier est donc *réticulé*). On montre de même l’existence de la borne inférieure $\inf_{n} \tilde{f}_n$, et l’on a $\inf_{n} \tilde{f}_n = -\sup_{n} (-\tilde{f}_n)$. Il en résulte que $\limsup_{n \to \infty} f_n$ et $\limsup_{n \to \infty} g_n$ sont aussi équivalentes, et leur classe, qu’on note $\limsup_{n \to \infty} \tilde{f}_n$, est égale à $\inf_{n} (\sup_{p \geq 0} \tilde{f}_{n+p})$; on définit de même $\liminf_{n \to \infty} \tilde{f}_n$.

Une fonction numérique finie ou non $f$ est dite *négligeable* si elle est équivalente à 0; cette définition équivaut à la définition 1 pour les fonctions positives et partout définies, en vertu du th. 1. Pour que $f$ soit négligeable, il faut et il suffit que $|f|$ le soit (ou que $f^+$ et $f^-$ soient toutes deux négligeables).
