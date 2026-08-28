---
book: top
book_title: General Topology
chapter: IV
chapter_title: NOMBRES RÉELS
section: 5
section_title: Fonctions numériques
lang: fr
source: top-i-iv-fr
book_pages: TG IV.17-TG IV.27, TG IV.53-TG IV.55
pdf_pages: 0288-0298, 0324-0326
extraction: ocr
subsections:
    - "no": 1
      title: Fonctions numériques
      page: 17
      pdf_page: 288
    - "no": 2
      title: Fonctions numériques définies dans un ensemble filtré
      page: 18
      pdf_page: 289
    - "no": 3
      title: Limites à droite et à gauche d’une fonction d’une variable réelle
      page: 19
      pdf_page: 290
    - "no": 4
      title: Bornes d’une fonction numérique
      page: 19
      pdf_page: 290
    - "no": 5
      title: Enveloppes d’une famille de fonctions numériques
      page: 21
      pdf_page: 292
    - "no": 6
      title: Limite supérieure et limite inférieure d’une fonction numérique suivant un filtre
      page: 22
      pdf_page: 293
    - "no": 7
      title: Opérations algébriques sur les fonctions numériques
      page: 25
      pdf_page: 296
statements: 29
exercises: 18
content_sha256: 8ec7cc47403277d79bf66884ad4d3671e9b0ad48466a3154d7d41196f4a8fda9
---

## § 5. FONCTIONS NUMÉRIQUES

### 1. Fonctions numériques

#### Définition 1 {#top-iv-s5-def-1 .statement}

Les applications d’un ensemble $E$ dans la droite numérique sont appelées fonctions numériques (ou fonctions réelles) définies dans $E$.

Par un abus de langage analogue à celui signalé dans IV, p. 14, nous appellerons fonctions numériques définies dans $E$, dans ce paragraphe et dans le suivant, les applications de $E$ dans $\overline{\mathbf{R}}$; les applications de $E$ dans $\mathbf{R}$ seront appelées fonctions numériques finies.

Si $f$ et $g$ sont deux fonctions numériques définies dans $E$, la relation $f \leq g$ est par définition équivalente à « quel que soit $x \in E, f(x) \leq g(x)$ »; cette relation est une relation d’ordre dans l’ensemble $\overline{\mathbf{R}}^E$ des fonctions numériques définies dans $E$. En outre, $\overline{\mathbf{R}}^E$, ordonné par cette relation, est un ensemble réticulé ; en effet, si $f$ et $g$ sont deux fonctions numériques, la fonction numérique $h$ telle que, pour tout $x \in E, h(x) = \sup(f(x), g(x))$, est la plus petite des fonctions numériques qui sont à la fois $\geq f$ et $\geq g$; conformément aux notations générales, on désignera cette fonction (qui est la borne supérieure de $f$ et $g$ dans $\overline{\mathbf{R}}^E$) par la notation $\sup(f, g)$; de même, la fonction numérique égale à $\inf(f(x), g(x))$ pour tout $x \in E$, sera notée $\inf(f, g)$.

On remarquera que $\sup(f, g)$ est l’application composée de l’application $(u, v) \mapsto \sup(u, v)$ de $\overline{\mathbf{R}} \times \overline{\mathbf{R}}$ dans $\overline{\mathbf{R}}$, et de l’application $x \mapsto (f(x), g(x))$ de $E$ dans $\overline{\mathbf{R}} \times \overline{\mathbf{R}}$. On a une propriété analogue pour $\inf(f, g)$.

Une fonction numérique $f$ définie dans un ensemble $E$ est dite majorée (resp. minorée) dans $E$, si $f(E)$ est une partie majorée de $A'' = (-\infty, +\infty[$ (resp. une partie minorée de $A' = ]-\infty, +\infty[$); $f$ est dite bornée dans $E$ si elle est à la fois majorée et minorée, c’est-à-dire si $f(E)$ est une partie bornée de $\mathbf{R}$ (rappelons que toute partie de $\overline{\mathbf{R}}$ est bornée).

Toute fonction bornée est donc finie ; la réciproque est inexacte comme le montre l’exemple de la fonction $1/x$ dans $\mathbf{R}_+^* = ]0, +\infty[$.

### 2. Fonctions numériques définies dans un ensemble filtré

#### Proposition 1 {#top-iv-s5-prop-1 .statement}

Soient $f$ et $g$ deux fonctions numériques, définies dans un ensemble $E$, filtré par un filtre $\mathcal{F}$. Si $\lim_{\mathcal{F}} f$ et $\lim_{\mathcal{F}} g$ existent, et si, pour toute partie $A \in \mathcal{F}$, il existe $x \in A$ tel que $f(x) \leq g(x)$, on a $\lim_{\mathcal{F}} f \leq \lim_{\mathcal{F}} g$.

Pour établir cette proposition, nous démontrerons l’énoncé suivant, qui lui est équivalent:

#### Proposition 2 {#top-iv-s5-prop-2 .statement}

Soient $f$ et $g$ deux fonctions numériques, définies dans un ensemble $E$, filtré par un filtre $\mathcal{F}$. Si $\lim_{\mathcal{F}} f$ et $\lim_{\mathcal{F}} g$ existent, et si $\lim_{\mathcal{F}} f > \lim_{\mathcal{F}} g$, il existe un ensemble $A \in \mathcal{F}$ tel que, pour tout $x \in A$, $f(x) > g(x)$.

Posons $a = \lim_{\mathcal{F}} f$, $b = \lim_{\mathcal{F}} g$, et soit $c$ tel que $b < c < a$. L’intervalle $]c, +\infty]$ de $\mathbf{R}$ (resp. $(-\infty, c[)$) est un voisinage de $a$ (resp. $b$); il existe donc un ensemble $M \in \mathcal{F}$ (resp. un ensemble $N \in \mathcal{F}$) tel que $f(x) > c$ pour tout $x \in M$ (resp. $g(x) < c$ pour tout $x \in N$); l’ensemble $A = M \cap N$ appartient à $\mathcal{F}$ et on a $f(x) > c > g(x)$ pour tout $x \in A$.

De la prop. 1, on déduit, comme cas particulier, le théorème suivant:

#### Théorème 1 (principe de prolongement des inégalités) {#top-iv-s5-thm-1 .statement}

Soient $f, g$ deux fonctions numériques, définies dans un ensemble $E$, filtré par un filtre $\mathcal{F}$. Si $\lim_{\mathcal{F}} f$ et $\lim_{\mathcal{F}} g$ existent, et si $f \leq g$, on a aussi $\lim_{\mathcal{F}} f \leq \lim_{\mathcal{F}} g$.

#### Remarque {#top-iv-s5-n2-rem-1 .statement}

Si on a en particulier $f(x) < g(x)$ pour tout $x \in E$ (ou seulement pour tous les points d’un ensemble du filtre $\mathcal{F}$), on peut en conclure, d’après le th. 1, que $\lim_{\mathcal{F}} f \leq \lim_{\mathcal{F}} g$; mais il ne faudrait pas croire qu’on puisse en déduire l’inégalité plus précise $\lim_{\mathcal{F}} f < \lim_{\mathcal{F}} g$. Par exemple, si on prend pour $E$ l’ensemble $\mathbf{N}$ des entiers naturels, filtré par le filtre de Fréchet, et si $f(n) = 0, g(n) = 1/n$, on a $f(n) < g(n)$ quel que soit $n$, mais $\lim_{n \to \infty} f(n) = \lim_{n \to \infty} g(n) = 0$.

D’une manière plus imagée, on peut dire qu’on perd en précision lorsqu’on passe à la limite dans une inégalité stricte.

#### Théorème 2 (théorème de la limite monotone) {#top-iv-s5-thm-2 .statement}

Soient $E$ un ensemble ordonné, $A$ une partie de $E$ filtrante à droite.\footnote{Cet énoncé suppose implicitement que la relation d’ordre dans $E$ est notée $x \leq y$. Si cette relation est notée $x(\sigma)y$, où $(\sigma)$ est un certain signe ou groupe de signes caractéristique de la relation envisagée, il faut remplacer, dans l’énoncé, les mots « filtrante à droite » par « filtrante pour la relation $(\sigma)$ ».} Toute fonction numérique monotone $f$ définie dans $A$ possède une limite suivant $A$ (I, p. 49); si $f$ est croissante (resp. décroissante), cette limite est égale à la borne supérieure (resp. inférieure) de l’ensemble $f(A) \subset \overline{\mathbf{R}}$.

Supposons par exemple que $f$ soit croissante, et soit $a = \sup f(A)$. Si $a = -\infty$, le théorème est trivial. Si $a > -\infty$, pour tout $b < a$, il existe $x \in A$ tel que $b < f(x) \leq a$; donc, si $S_x$ est la section de $A$ relative à $x$ (ensemble des $y \geq x$, cf. I, p. 38), $f(S_x)$ est contenu dans le voisinage $]b, +\infty]$ de $a$, d’où le théorème. Démonstration analogue lorsque $f$ est décroissante.

#### Corollaire {#top-iv-s5-n2-cor-1 .statement}

Pour qu’une fonction numérique croissante (resp. décroissante), définie dans une partie filtrante $A$ d’un ensemble ordonné $E$, ait une limite finie suivant $A$, il faut et il suffit qu’elle soit majorée (resp. minorée) dans $A$.

Si on applique le th. 2 au cas où $A = E = \mathbf{N}$ (ordonné par la relation $\leqslant$), on a la proposition suivante:
**Proposition 3.** — *Toute suite monotone de nombres réels a une limite dans $\overline{\mathbf{R}}$.*

En particulier, toute suite croissante (resp. décroissante) de nombres *finis* converge vers un nombre réel fini si elle est majorée (resp. minorée), vers $+\infty$ (resp. $-\infty$) dans le cas contraire. Par exemple, la suite des entiers positifs converge vers $+\infty$.

C’est ce fait qui est à l’origine de la notation $\lim_{n \to \infty} u_n$ pour désigner la limite d’une suite (I, p. 48).

De même, toute suite d’entiers $(p_n)$ *strictement croissante* converge vers $+\infty$, car on voit, par récurrence, que $p_n \geqslant p_0 + n$ quel que soit $n$.

### 3. Limites à droite et à gauche d’une fonction d’une variable réelle

Soit $A$ une partie non vide de $\overline{\mathbf{R}}$, et $a \neq -\infty$ un point de $\overline{\mathbf{R}}$ adhérent à l’ensemble $B = A \cap (-\infty, a[$. L’ensemble $B$ est filtrant pour la relation $\leqslant$, et son filtre des sections $\mathcal{F}$ est identique à la *trace* sur $B$ du filtre des voisinages de $a$ dans $\overline{\mathbf{R}}$.

#### Définition 2 {#top-iv-s5-def-2 .statement}

*Soit $f$ une fonction définie dans la partie $A$ de $\overline{\mathbf{R}}$, à valeurs dans un espace topologique $E$. Une limite de $f$ suivant le filtre $\mathcal{F}$, si elle existe, s’appelle limite à gauche de $f$ au point $a$, relativement à $A$, et se note $\lim_{x \to a, x < a, x \in A} f(x)$, ou $f(a-)$ lorsque $E$ est séparé.*

On définit de même, lorsque $a \neq +\infty$ est adhérent à l’ensemble $A \cap ]a, +\infty]$, une *limite à droite* (si elle existe) de $f$ au point $a$ qu’on note $\lim_{x \to a, x > a, x \in A} f(x)$, ou $f(a+)$ lorsque $E$ est séparé.

Le th. 2 de IV, p. 18 entraîne immédiatement la proposition suivante:
**Proposition 4.** — *Soient $A$ une partie de $\overline{\mathbf{R}}$, $a \neq -\infty$ un point adhérent à l’intersection $A \cap (-\infty, a[$; si $f$ est une fonction numérique monotone définie dans $A$, elle a une limite à gauche $f(a-)$ au point $a$, relativement à $A$.*

### 4. Bornes d’une fonction numérique

#### Définition 3 {#top-iv-s5-def-3 .statement}

*Soit $f$ une fonction numérique définie dans un ensemble $E$; on appelle borne supérieure (resp. borne inférieure) de $f$ dans une partie non vide $A$ de $E$, et on note $\sup_{x \in A} f(x)$ (resp. $\inf_{x \in A} f(x)$) la borne supérieure (resp. borne inférieure) dans $\overline{\mathbf{R}}$ de l’ensemble $f(A)$.

En particulier, si $A$ est une partie non vide de $\overline{\mathbf{R}}$, on a
$$
\sup A = \sup_{x \in A} x.
$$
(1)

Il est souvent plus commode d’utiliser la notation du second membre pour désigner la borne supérieure de A.

Le nombre $a = \sup_{x \in A} f(x)$ est caractérisé par les deux propriétés suivantes:
1° Quel que soit $x \in A, f(x) \leq a$.
2° Quel que soit $b < a$, il existe $x \in A$ tel que $b < f(x) \leq a$.
Les nombres $\sup_{x \in A} f(x)$ et $\inf_{x \in A} f(x)$ appartiennent à l’adhérence de $f(A)$ dans $\overline{\mathbf{R}}$.
On a $\inf_{x \in A} f(x) \leq \sup_{x \in A} f(x)$; pour que ces deux nombres soient égaux, il faut et il suffit que $f$ soit constante dans A.

Pour qu’une fonction numérique $f$, définie dans un ensemble E, soit majorée (resp. minorée) dans une partie non vide A de E, il faut et il suffit que $\sup_{x \in A} f(x) < +\infty$ (resp. $\inf_{x \in A} f(x) > -\infty$); on dit encore dans ce cas que $f$ est bornée supérieurement (resp. bornée inférieurement) dans A. Pour que $f$ soit bornée dans A, il faut et il suffit que $|f|$ soit majorée dans A, donc que $\sup_{x \in A} |f(x)| < +\infty$.

On a
$$
\inf_{x \in A} f(x) = -\sup_{x \in A} (-f(x)).
$$
Cette relation ramène toutes les propriétés de la borne inférieure à celles de la borne supérieure; aussi ne parlerons-nous en général que de ces dernières.

#### Proposition 5 {#top-iv-s5-prop-5 .statement}

Soit $f$ une fonction numérique définie dans un ensemble E. Dans l’ensemble $\mathcal{F}(E)$ des parties finies de E, ordonné filtrant pour la relation $\subset$, la fonction numérique $H \mapsto \sup_{x \in H} f(x)$ est croissante, la fonction numérique $H \mapsto \inf_{x \in H} f(x)$ est décroissante et on a
$$
\begin{cases}
\sup_{x \in E} f(x) = \lim_{H \in \mathcal{F}(E)} (\sup_{x \in H} f(x)) \\
\inf_{x \in E} f(x) = \lim_{H \in \mathcal{F}(E)} (\inf_{x \in H} f(x)).
\end{cases}
$$

Posons $\varphi(H) = \sup_{x \in H} f(x)$; il est clair que $\varphi$ est croissante; elle a donc une limite $a$ (IV, p. 18, th. 2), et comme $\varphi(H) \leq \sup_{x \in E} f(x)$ quel que soit $H$, $a \leq \sup_{x \in E} f(x)$ (IV, p. 18, th. 1). Si on avait $a < \sup_{x \in E} f(x)$, il existerait $x_0 \in E$ tel que $a < f(x_0)$, d’où contradiction puisque $\varphi(H) \geq f(x_0)$ dès que $x_0 \in H$.

En particulier, d’après (1) (IV, p. 19), on a, pour toute partie non vide A de $\overline{\mathbf{R}}$,
$$
\sup A = \lim_{H \in \mathcal{F}(A)} (\sup_{x \in H} x).
$$

#### Proposition 6 {#top-iv-s5-prop-6 .statement}

*Soient f et g deux fonctions numériques définies dans E. Si $f(x) \leq g(x)$ en tout point d’une partie non vide $A$ de $E$, on a*

$$
\begin{cases}
\sup_{x \in A} f(x) \leq \sup_{x \in A} g(x) \\
\inf_{x \in A} f(x) \leq \inf_{x \in A} g(x).
\end{cases}
$$

(5)

#### Proposition 7 {#top-iv-s5-prop-7 .statement}

*Soit f une fonction numérique définie dans E; si A et B sont deux parties non vides de E telles que $A \subset B$, on a*

$$
\sup_{x \in A} f(x) \leq \sup_{x \in B} f(x).
$$

(6)

#### Proposition 8 {#top-iv-s5-prop-8 .statement}

*Soient f une fonction numérique définie dans E, et $(A_i)_{i \in I}$ une famille de parties non vides de E; on a*

$$
\sup_{x \in \bigcup_{i \in I} A_i} f(x) = \sup_{i \in I} (\sup_{x \in A_i} f(x)).
$$

(7)

Ces propositions sont des cas particuliers de E, III, p. 11, prop. 6 et 7 et cor. de la prop. 5.

Soit f une fonction numérique définie dans un ensemble produit $E_1 \times E_2$; si $A_2$ est une partie non vide de $E_2$, on notera $\sup_{x_2 \in A_2} f(x_1, x_2)$ la borne supérieure dans $A_2$ de la fonction numérique $x_2 \mapsto f(x_1, x_2)$ définie dans $E_2$. De la prop. 8, on déduit en particulier:

#### Proposition 9 {#top-iv-s5-prop-9 .statement}

*Soit f une fonction numérique définie dans un ensemble produit $E_1 \times E_2$. Quelles que soient les parties non vides $A_1$ de $E_1$, $A_2$ de $E_2$, on a*

$$
\sup_{(x_1, x_2) \in A_1 \times A_2} f(x_1, x_2) = \sup_{x_1 \in A_1} (\sup_{x_2 \in A_2} f(x_1, x_2)) = \sup_{x_2 \in A_2} (\sup_{x_1 \in A_1} f(x_1, x_2)).
$$

(8)

### 5. Enveloppes d’une famille de fonctions numériques

#### Définition 4 {#top-iv-s5-def-4 .statement}

*Soit $(f_i)_{i \in I}$ une famille de fonctions numériques, définies dans un ensemble E. On appelle enveloppe supérieure (resp. enveloppe inférieure) de la famille $(f_i)$, et on note $\sup_{i \in I} f_i$ ou $\sup_i f_i$ (resp. $\inf_{i \in I} f_i$ ou $\inf_i f_i$), la fonction numérique définie dans E, dont la valeur en tout point $x \in E$ est $\sup_{i \in I} (f_i(x))$ (resp. $\inf_{i \in I} (f_i(x))$).

L’enveloppe supérieure de la famille $(f_i)$ n’est autre que la *borne supérieure* de cette famille dans l’ensemble ordonné réticulé $\overline{\mathbf{R}}^E$ des fonctions numériques définies dans E, ce qui justifie la notation $\sup_i f_i$.

En outre, si on munit $\overline{\mathbf{R}}^E$ de la *topologie produit* de celles de ses facteurs (tous identiques à $\overline{\mathbf{R}}$), on a la proposition suivante:

#### Proposition 10 {#top-iv-s5-prop-10 .statement}

*Dans l’espace produit $\overline{\mathbf{R}}^E$, l’enveloppe supérieure $\sup_i f_i$ d’une famille* de fonctions numériques $(f_i)_{i \in I}$ est la limite, suivant l’ensemble filtrant $\mathcal{F}(I)$ des parties finies de $I$, de l’application $H \mapsto \sup_{i \in H} f_i$ (qui, à tout partie finie $H$ de $I$, fait correspondre l’enveloppe supérieure de la sous-famille finie $(f_i)_{i \in H}$).

Cela résulte aussitôt de la prop. 5 de IV, p. 20, et de I, p. 51, cor. 2.

On peut donc écrire

$$
\sup_{i \in I} f_i = \lim_{H \in \mathcal{F}(I)} (\sup_{i \in H} f_i).
$$

#### Définition 5 {#top-iv-s5-def-5 .statement}

Une famille $(f_i)_{i \in I}$ de fonctions numériques, définies dans un ensemble $E$, est dite uniformément majorée (resp. uniformément minorée) dans $E$, s’il existe un nombre fini $a$ tel que $f_i(x) \leq a$ (resp. $f_i(x) \geq a$) quels que soient $x \in E$ et $i \in I$. La famille $(f_i)$ est dite uniformément bornée dans $E$ si elle est à la fois uniformément majorée et uniformément minorée dans $E$.

Pour que $(f_i)$ soit uniformément majorée dans $E$, il faut et il suffit donc que l’enveloppe supérieure de cette famille soit majorée dans $E$. Pour que $(f_i)$ soit uniformément bornée dans $E$, il faut et il suffit que l’enveloppe supérieure de la famille $(|f_i|)$ soit majorée dans $E$ (c’est-à-dire qu’il existe un nombre fini $a \geq 0$ tel que, pour tout $i \in I$ et tout $x \in E$, $|f_i(x)| \leq a$).

### 6. Limite supérieure et limite inférieure d’une fonction numérique suivant un filtre

Soit $f$ une fonction numérique, définie dans un ensemble $E$, filtré par un filtre $\mathcal{G}$. On sait (I, p. 39) que $\mathcal{G}$ est un ensemble ordonné filtrant pour la relation $\supseteq$. Considérons, pour tout ensemble $X \in \mathcal{G}$, le nombre réel $\sup_{x \in X} f(x)$; on définit ainsi une application $X \mapsto \sup_{x \in X} f(x)$ de $\mathcal{G}$ dans $\overline{\mathbf{R}}$, qui est décroissante dans $\mathcal{G}$, d’après la prop. 7 de IV, p. 21. Elle a donc une limite suivant l’ensemble filtrant $\mathcal{G}$, d’après le th. 2 de IV, p. 18.

#### Définition 6 {#top-iv-s5-def-6 .statement}

On appelle limite supérieure de $f$ suivant le filtre $\mathcal{G}$, et on note $\lim.\sup_{\mathcal{G}} f$, ou $\lim.\sup_{x,\mathcal{G}} f(x)$, la limite de la fonction numérique $X \mapsto \sup_{x \in X} f(x)$ suivant l’ensemble filtrant $\mathcal{G}$.

On définit de même la limite inférieure de $f$ suivant le filtre $\mathcal{G}$, qu’on note $\lim.\inf_{\mathcal{G}} f$, ou $\lim.\inf_{x,\mathcal{G}} f(x)$.

On a donc, par définition

$$
\begin{cases}
\lim.\sup_{\mathcal{G}} f = \lim_{X \in \mathcal{G}} (\sup_{x \in X} f(x)) \\
\lim.\inf_{\mathcal{G}} f = \lim_{X \in \mathcal{G}} (\inf_{x \in X} f(x)).
\end{cases}
$$

On se dispense souvent d’indiquer le filtre $\mathcal{G}$ dans les notations, et on écrit simplement $\lim.\sup f$, ou $\lim.\sup_x f(x)$, ou $\lim.\sup f(x)$, lorsqu’il ne peut en résulter de confusion.

D’après les formules (10) et le th. 1 de IV, p. 18, on a
$$
\inf_{x \in E} f(x) \leq \lim.\inf_{\mathcal{G}} f \leq \lim.\sup_{\mathcal{G}} f \leq \sup_{x \in E} f(x).
$$
D’après IV, p. 18, th. 2, on peut aussi écrire
$$
\begin{cases}
\lim.\sup_{\mathcal{G}} f = \inf_{X \in \mathcal{G}} (\sup_{x \in X} f(x)) \\
\lim.\inf_{\mathcal{G}} f = \sup_{X \in \mathcal{G}} (\inf_{x \in X} f(x)).
\end{cases}
$$
On peut d’ailleurs remplacer, aux seconds membres des formules (10) et (12), le filtre $\mathcal{G}$ par une quelconque de ses *bases* $\mathfrak{B}$.
D’après (2) (IV, p. 20) et (10), on a
$$
\lim.\inf_{\mathcal{G}} f = -\lim.\sup_{\mathcal{G}} (-f),
$$
ce qui permet de n’étudier que les propriétés de la limite supérieure.

#### Théorème 3 {#top-iv-s5-thm-3 .statement}

*La limite supérieure d’une fonction numérique $f$ suivant un filtre $\mathcal{G}$ est égale à la plus grande valeur d’adhérence de $f$ suivant $\mathcal{G}$.*
En effet, soit $b$ une valeur d’adhérence de $f$ suivant $\mathcal{G}$; pour tout $X \in \mathcal{G}$, $b$ est adhérent à $f(X)$, donc $b \leq \sup_{x \in X} f(x)$, ce qui entraîne, d’après (12),
$b \leq \lim.\sup_{\mathcal{G}} f = a$.
D’autre part, soit $V$ un voisinage ouvert quelconque du point $a$ dans $\overline{\mathbf{R}}$; il existe $X_0 \in \mathcal{G}$ tel que, pour tout $X \in \mathcal{G}$ contenu dans $X_0$, on ait $\sup_{x \in X} f(x) \in V$; comme $V$ est ouvert, on en déduit que $f(X)$ rencontre $V$; donc $a$ est une *valeur d’adhérence* de $f$ suivant $\mathcal{G}$, ce qui achève la démonstration.

#### Corollaire 1 {#top-iv-s5-thm-3-cor-1 .statement}

*Pour que $\lim.\sup_{\mathcal{G}} f = \lim.\inf_{\mathcal{G}} f$, il faut et il suffit que $f$ ait une limite suivant le filtre $\mathcal{G}$; on a alors*
$$
\lim_{\mathcal{G}} f = \lim.\sup_{\mathcal{G}} f = \lim.\inf_{\mathcal{G}} f.
$$
En effet, comme $\overline{\mathbf{R}}$ est compact, pour que la base de filtre $f(\mathcal{G})$ ait un point limite, il faut et il suffit que l’ensemble de ses points adhérents se réduise à un point (I, p. 60, corollaire).

#### Corollaire 2 {#top-iv-s5-thm-3-cor-2 .statement}

*Si $\mathfrak{H}$ est un filtre plus fin que $\mathcal{G}$, on a*
$$
\lim.\inf_{\mathcal{G}} f \leq \lim.\inf_{\mathfrak{H}} f \leq \lim.\sup_{\mathfrak{H}} f \leq \lim.\sup_{\mathcal{G}} f.
$$
En effet, toute valeur d’adhérence de $f$ suivant $\mathfrak{H}$ est aussi valeur d’adhérence de $f$ suivant $\mathcal{G}$ (I, p. 49).
En particulier, si $\lim_{\mathfrak{H}} f$ existe, on a
$$
\lim.\inf_{\mathcal{G}} f \leq \lim_{\mathfrak{H}} f \leq \lim.\sup_{\mathcal{G}} f.
$$

#### Corollaire 3 {#top-iv-s5-thm-3-cor-3 .statement}

Soit $A$ un ensemble du filtre $\mathcal{G}$ et soient $\mathcal{G}_A$ le filtre induit sur $A$ par $\mathcal{G}$, $f_A$ la restriction de $f$ à $A$; on a
$$
\limsup_{\mathcal{G}_A} f_A = \limsup_{\mathcal{G}} f.
$$
En effet, tout point adhérent à la base de filtre $f(\mathcal{G})$ est adhérent à la base de filtre $f_A(\mathcal{G}_A)$, et réciproquement.

En raison de ce fait, lorsque $f$ n’est définie que sur une partie $A$ de $E$ appartenant à $\mathcal{G}$, on écrit souvent $\limsup_{\mathcal{G}} f$, au lieu de $\limsup_{\mathcal{G}_A} f_A$, par abus de langage.

#### Proposition 11 {#top-iv-s5-prop-11 .statement}

Soient $f$ et $g$ deux fonctions numériques définies dans un ensemble filtré $E$. La relation $f \leq g$ entraîne
$$
\begin{cases}
\limsup f \leq \limsup g \\
\liminf f \leq \liminf g.
\end{cases}
$$
(14)
C’est une conséquence immédiate des relations (12) (IV, p. 23).

Lorsque $E$ est un espace topologique, et $\mathcal{G}$ le filtre des voisinages d’un point $a$ de $E$, on écrit $\limsup_{x \to a} f(x)$ (resp. $\liminf_{x \to a} f(x)$) au lieu de $\limsup_{\mathcal{G}} f$ (resp. $\liminf_{\mathcal{G}} f$); on a évidemment
$$
\liminf_{x \to a} f(x) \leq f(a) \leq \limsup_{x \to a} f(x).
$$
(15)
Plus généralement, lorsque $E$ est un sous-espace d’un espace topologique $F$, et $\mathcal{G}$ la trace sur $E$ du filtre des voisinages d’un point $a \in \overline{E}$, on écrit $\limsup_{x \to a, x \in E} f(x)$ (resp. $\liminf_{x \to a, x \in E} f(x)$) au lieu de $\limsup_{\mathcal{G}} f$ (resp. $\liminf_{\mathcal{G}} f$); on dit que $\limsup_{x \to a, x \in E} f(x)$ est la limite supérieure de $f(x)$ lorsque $x$ tend vers $a$, en restant dans $E$. Lorsque $E$ est le complémentaire de $\{a\}$, on remplace, dans ces notations, « $x \in E$ » par « $x \neq a$ ».

Si $A$ est une partie de $E$ telle que $a \in \overline{A}$, on a (IV, p. 23, cor. 2)
$$
\liminf_{x \to a, x \in E} f(x) \leq \liminf_{x \to a, x \in A} f(x) \leq \limsup_{x \to a, x \in A} f(x) \leq \limsup_{x \to a, x \in E} f(x)
$$
Si $V$ est un voisinage de $a$ dans $F$, on a (cor. 3)
$$
\limsup_{x \to a, x \in \overline{V} \cap E} f(x) = \limsup_{x \to a, x \in E} f(x).
$$
Autrement dit, les notions de limite inférieure et de limite supérieure, en un point d’un espace topologique, ont, comme celle de limite, un caractère local.

Enfin, lorsque $\mathcal{G}$ est le filtre de Fréchet sur $\mathbf{N}$, la limite supérieure (resp. inférieure) suivant $\mathcal{G}$ de l’application $n \mapsto u_n$ de $\mathbf{N}$ dans $\overline{\mathbf{R}}$ se note $\limsup_{n \to \infty} u_n$ (resp. $\liminf_{n \to \infty} u_n$) et s’appelle limite supérieure (resp. limite inférieure) de la suite de nombres réels $u_n$.

La relation $\limsup_{n \to \infty} u_n = a \in \mathbf{R}$ est donc équivalente à la suivante: quel que soit $\varepsilon > 0$, il existe un entier $n_0$ tel que, pour tout $n \geq n_0$, $u_n \leq a + \varepsilon$, et, pour une infinité de valeurs de $n$, $u_n \geq a - \varepsilon$. On traduit de même la définition de la limite supérieure d’une suite lorsqu’elle a pour valeur $+\infty$ ou $-\infty$.

Étant donné une suite $(f_n)$ de fonctions numériques définies sur un ensemble $E$, on désignera par $\limsup_{n \to \infty} f_n$ (resp. $\liminf_{n \to \infty} f_n$) la fonction numérique dont la valeur, en un point quelconque $x \in E$, est $\limsup_{n \to \infty} f_n(x)$ (resp. $\liminf_{n \to \infty} f_n(x)$). D’après (10) (IV, p. 22) et (12) (IV, p. 23), on a

$$
\begin{cases}
\limsup_{n \to \infty} f_n = \inf_{n \in \mathbf{N}} (\sup_{m \geq n} f_m) \leq \lim_{n \to \infty} (\sup_{m \geq n} f_m) \\
\liminf_{n \to \infty} f_n = \sup_{n \in \mathbf{N}} (\inf_{m \geq n} f_m) = \lim_{n \to \infty} (\inf_{m \geq n} f_m)
\end{cases}
$$

les limites étant prises dans l’espace produit $\overline{\mathbf{R}}^E$. Pour que la suite $(f_n)$ ait une limite dans $\overline{\mathbf{R}}^E$, il faut et il suffit que $\limsup_{n \to \infty} f_n = \liminf_{n \to \infty} f_n$ (IV, p. 23, cor. 1 et I, p. 51, cor. 1).

### 7. Opérations algébriques sur les fonctions numériques

Soient $f$ et $g$ deux fonctions numériques définies dans un ensemble $E$; si la somme $f(x) + g(x)$ (resp. le produit $f(x)g(x)$) a un sens quel que soit $x \in E$, on notera encore $f + g$ (resp. $fg$) la fonction numérique $x \mapsto f(x) + g(x)$ (resp. $x \mapsto f(x)g(x)$). De même, si $1/f(x)$ a un sens quel que soit $x \in E$, on notera $1/f$ la fonction $x \mapsto 1/f(x)$.

Cette dernière fonction est donc définie lorsque $f$ ne prend pas la valeur 0; lorsque $f$ prend ses valeurs dans l’intervalle $[0, +\infty)$ (resp. dans $(- \infty, 0])$, on peut encore considérer que $1/f(x)$ est partout défini en posant $1/0 = +\infty$ (resp. $1/0 = -\infty$); la fonction $1/f$ sera encore définie dans ce cas.

Supposons $E$ filtré par un filtre $\mathcal{F}$, et que $\lim_{\mathcal{F}} f$ et $\lim_{\mathcal{F}} g$ existent; si, d’une part, la fonction $f + g$ (resp. $fg$, resp. $1/f$) est définie, et si, d’autre part, l’expression $\lim_{\mathcal{F}} f + \lim_{\mathcal{F}} g$ (resp. $\lim_{\mathcal{F}} f . \lim_{\mathcal{F}} g$, resp. $1/\lim_{\mathcal{F}} f$) a un sens, alors $\lim_{\mathcal{F}} (f + g)$ (resp. $\lim_{\mathcal{F}} fg$, resp. $\lim_{\mathcal{F}} (1/f)$) existe et est égale à cette expression, en vertu de la continuité de la fonction $x + y$ (resp. $xy$, resp. $1/x$) aux points où elle est définie.

#### Proposition 12 {#top-iv-s5-prop-12 .statement}

*Soient $f$ et $g$ deux fonctions numériques définies dans un ensemble $E$, et $A$ une partie non vide de $E$.*

1° *On a*

$$
\sup_{x \in A} (f(x) + g(x)) \leq \sup_{x \in A} f(x) + \sup_{x \in A} g(x)
$$
$$
\sup_{x \in A} f(x) + \inf_{x \in A} g(x) \leq \sup_{x \in A} (f(x) + g(x))
$$

lorsque les deux membres de ces inégalités sont définis.

2° *Si $f(x)$ et $g(x)$ sont $\geq 0$ pour tout $x \in A$, on a*

$$
\sup_{x \in A} (f(x)g(x)) \leq \sup_{x \in A} f(x) . \sup_{x \in A} g(x)
$$
$$
\sup_{x \in A} f(x) . \inf_{x \in A} g(x) \leq \sup_{x \in A} (f(x)g(x))
$$

lorsque les deux membres de ces inégalités sont définis.

3° Si $f(x) \geqslant 0$ quel que soit $x \in A$,

$$
\sup_{x \in A} (1/f(x)) = 1/\inf_{x \in A} f(x)
$$
(en posant $1/0 = +\infty$).

Soit en effet $H$ une partie *finie* quelconque de $A$; si $x_0$ est un des points de $H$ où $f + g$ prend sa plus grande valeur, on a
$$
f(x_0) + g(x_0) \leqslant \sup_{x \in H} f(x) + \sup_{x \in H} g(x);
$$
d’autre part, si $x_1$ est un des points de $H$ où $f$ prend sa plus grande valeur, on a
$$
f(x_1) + g(x_1) \geqslant \sup_{x \in H} f(x) + \inf_{x \in H} g(x);
$$
donc
$$
\sup_{x \in H} f(x) + \inf_{x \in H} g(x) \leqslant \sup_{x \in H} (f(x) + g(x)) \leqslant \sup_{x \in H} f(x) + \sup_{x \in H} g(x).
$$

Les inégalités (17) et (18) en résultent, en appliquant la prop. 5 de IV, p. 20 et le th. 1 de IV, p. 18. Démonstrations analogues pour les autres inégalités.

#### Corollaire 1 {#top-iv-s5-prop-12-cor-1 .statement}

*Soient $f$ une fonction numérique définie dans $E$, et $k$ un nombre réel. On a*
$$
\sup_{x \in A} (f(x) + k) = k + \sup_{x \in A} f(x)
$$
*lorsque les deux membres sont définis, et, pour $k \geqslant 0$,

$$
\sup_{x \in A} (k f(x)) = k \cdot \sup_{x \in A} f(x)
$$
*lorsque les deux membres sont définis*.

#### Corollaire 2 {#top-iv-s5-prop-12-cor-2 .statement}

*Soient $f_1$ et $f_2$ deux fonctions numériques définies respectivement dans des ensembles $E_1$ et $E_2$; quelles que soient les parties non vides $A_1 \subset E_1, A_2 \subset E_2$, on a*
$$
\sup_{(x_1, x_2) \in A_1 \times A_2} (f_1(x_1) + f_2(x_2)) = \sup_{x_1 \in A_1} f_1(x_1) + \sup_{x_2 \in A_2} f_2(x_2)
$$
*lorsque les deux membres sont définis; si $f_1$ et $f_2$ sont $\geqslant 0$ dans $A_1$ et $A_2$ respectivement, on a*
$$
\sup_{(x_1, x_2) \in A_1 \times A_2} (f_1(x_1) f_2(x_2)) = \sup_{x_1 \in A_1} f_1(x_1) \cdot \sup_{x_2 \in A_2} f_2(x_2)
$$
*lorsque les deux membres sont définis*

C’est une conséquence du corollaire précédent, et de IV, p. 21, prop. 9.

En particulier, si $A$ et $B$ sont deux parties de $\overline{\mathbf{R}}$ telles que l’ensemble $A + B$ des sommes $x + y$ ($x \in A, y \in B$) soit défini, on a
$$
\sup(A + B) = \sup A + \sup B
$$

si le second membre a un sens. De même, si A et B sont deux parties de $(0, +\infty)$, on a
(27)
$$
\sup AB = \sup A . \sup B
$$
lorsque les deux membres ont un sens.

#### Proposition 13 {#top-iv-s5-prop-13 .statement}

*Soient f et g deux fonctions numériques définies dans un ensemble filtré E.*

$1^\circ$ *On a*
(28)
$$
\lim . \sup (f + g) \leq \lim . \sup f + \lim . \sup g
$$
(29)
$$
\lim . \sup f + \lim . \inf g \leq \lim . \sup (f + g)
$$
*lorsque les deux membres de ces inégalités sont définis.*

$2^\circ$ *Si f et g sont $\geq 0$ dans E, on a*
(30)
$$
\lim . \sup fg \leq (\lim . \sup f)(\lim . \sup g)
$$
(31)
$$
(\lim . \sup f)(\lim . \inf g) \leq \lim . \sup fg
$$
*lorsque les deux membres de ces inégalités sont définis.*

$3^\circ$ *Si f $\geq 0$ dans E,
(32)
$$
\lim . \sup (1/f) = 1/(\lim . \inf f)
$$
(en posant $1/0 = +\infty$).

Ce sont des conséquences de la prop. 12 (IV, p. 25) et des relations (10) (IV, p. 22).

#### Corollaire 1 {#top-iv-s5-prop-13-cor-1 .statement}

*Soient f et g deux fonctions numériques définies dans un ensemble filtré E. Si $\lim g$ existe, on a*
(33)
$$
\lim . \sup (f + g) = \lim . \sup f + \lim g
$$
*lorsque les deux membres sont définis, et*
(34)
$$
\lim . \sup fg = (\lim . \sup f)(\lim g)
$$
*lorsque les deux membres sont définis, et que f et g sont $\geq 0$.*

#### Corollaire 2 {#top-iv-s5-prop-13-cor-2 .statement}

*Soient f et g deux fonctions numériques définies dans un ensemble filtré E. Si $\lim f = +\infty$, $\lim . \inf g > -\infty$, et si $f + g$ est définie, on a $\lim (f + g) = +\infty$. Si $\lim f = +\infty$, $\lim . \inf g > 0$ et si $fg$ est défini, on a $\lim fg = +\infty$.*

## EXERCICES {#top-iv-s5-exercises}

See the [exercises for § 5](exercises/s5/).
