---
book: ac
book_title: Commutative Algebra
chapter: I
chapter_title: Modules plats
section: 1
section_title: Diagrammes et suites exactes
lang: fr
source: ac-i-iv-fr
pdf_pages: 0012-0020, 0056-0057
extraction: ocr
subsections:
    - "no": 1
      title: Diagrammes.
      page: 0
      pdf_page: 12
    - "no": 2
      title: Diagrammes commutatifs.
      page: 0
      pdf_page: 12
    - "no": 3
      title: Suites exactes.
      page: 0
      pdf_page: 14
    - "no": 4
      title: Le diagramme du serpent.
      page: 0
      pdf_page: 15
statements: 7
exercises: 7
content_sha256: ce055ee638cb307cbacad4f748d112d368d0a0bf40e424626d097fe771250063
---

## § 1. Diagrammes et suites exactes

### 1. Diagrammes.

Soient par exemple A, B, C, D, E cinq ensembles, et soient $f$ une application de A dans B, $g$ une application de B dans C, $h$ une application de D dans E, $u$ une application de B dans D et $\varphi$ une application de C dans E. Pour résumer une situation de ce genre, on fait souvent usage de diagrammes ; par exemple, on résumera la situation précédente par le diagramme suivant (Ens., chap. II, § 3, n° 4) :

$$
\begin{array}{ccc}
A & \xrightarrow{f} & B \xrightarrow{g} C \\
u \downarrow & & \downarrow v \\
D & \xrightarrow{h} & E
\end{array}
$$

Dans un tel diagramme, le groupe de signes $A \xrightarrow{f} B$ schématise le fait que $f$ est une application de A dans B. Lorsqu’il ne peut y avoir d’ambiguïté sur $f$, on supprime la lettre $f$, et on écrit simplement $A \to B$.

Lorsque A, B, C, D, E sont des groupes (resp. des groupes commutatifs) et $f, g, h, u, \varphi$ des homomorphismes de groupes, on dit pour abréger que le diagramme (1) est un diagramme de groupes (resp. de groupes commutatifs).

En principe, un diagramme n’est pas un objet mathématique, mais seulement une figure, destinée à faciliter la lecture d’un raisonnement. En pratique, on se sert souvent des diagrammes comme de symboles abréviateurs, qui évitent de nommer tous les ensembles et toutes les applications que l’on veut considérer ; on dit ainsi « considérons le diagramme (1) » au lieu de dire : « soient A, B, C, D, E cinq ensembles... et $\varphi$ une application de C dans E » ; voir par exemple l’énoncé de la prop. 2 du n° 4.

### 2. Diagrammes commutatifs.

Considérons par exemple le diagramme suivant :

$$
\begin{array}{ccccccc}
A & \xrightarrow{f} & B & \xrightarrow{g} & C & \xrightarrow{h} & D \\
a \downarrow & & b \downarrow & & c \downarrow & & d \downarrow \\
A' & \xrightarrow{f'} & B' & \xrightarrow{g'} & C' & \xrightarrow{h'} & D'
\end{array}
$$

A tout chemin composé d’un certain nombre de segments du diagramme parcouru dans le sens indiqué par les flèches, on fait correspondre une application de l’ensemble représenté par l’origine du premier segment dans l’ensemble représenté par l’extrémité du dernier segment, savoir la composée des applications représentées par les divers segments parcourus. Pour tout sommet du diagramme, par exemple B, on convient qu’il y a un chemin réduit à B, et on lui fait correspondre l’application identique $1_B$.

Dans (2), il y a par exemple trois chemins partant de A et aboutissant à C’ ; les applications correspondantes sont $c \circ g \circ f$, $g' \circ b \circ f$ et $g' \circ f' \circ a$. On dit qu’un diagramme est commutatif si, pour tout couple de chemins du diagramme ayant même origine et même extrémité, les deux applications correspondantes sont égales ; en particulier si un chemin a son extrémité confondue avec son origine, l’application correspondante doit être l’identité.

Pour que le diagramme (2) soit commutatif, il faut et il suffit que l’on ait les relations :

$$
f' \circ a = b \circ f, \quad g' \circ b = c \circ g, \quad h' \circ c = d \circ h;
$$

autrement dit, il faut et il suffit que les trois diagrammes carrés extraits de (2) soient commutatifs. En effet, les relations (3) entraînent $c \circ g \circ f = g' \circ b \circ f$ puisque $c \circ g = g' \circ b$, et $g' \circ b \circ f = g' \circ f' \circ a$ puisque $b \circ f = f' \circ a$ ; donc les trois chemins partant de A et aboutissant à C’ donnent la même application. On vérifie de même que les quatre chemins partant de A et aboutissant à D’ (resp. les trois chemins partant de B et aboutissant à D’) donnent la même application. Les relations (3) signifient que les deux chemins partant de A (resp. B, C) et aboutissant à B’ (resp. C’, D’) donnent la même application. Tous les autres couples de sommets de (2) ne peuvent être joints que par un chemin au plus, et le diagramme (2) est donc bien commutatif.

Par la suite, nous laisserons au lecteur le soin de formuler et de vérifier des résultats analogues pour d’autres types de diagrammes.

### 3. Suites exactes.

Rappelons la définition suivante (Alg., chap. II, 3e éd., § 1, n° 4) :

#### Définition 1 {#ac-i-s1-def-1 .statement}

Soient A un anneau, F, G, H trois A-modules à droite (resp. à gauche), f un homomorphisme de F dans G et g un homomorphisme de G dans H. On dit que le couple (f, g) est une suite exacte si l’on a $\bar{g}^{-1}(0) = f(F)$, c’est-à-dire si le noyau de g est égal à l’image de f.

On dit aussi alors que le diagramme

$$
\begin{array}{ccc}
F & \xrightarrow{f} & G \\
& & \xrightarrow{g} \\
& & H
\end{array}
$$

est une suite exacte.

Considérons de même un diagramme formé de quatre modules et de trois homomorphismes :

$$
E \xrightarrow{f} F \xrightarrow{g} G \xrightarrow{h} H.
$$

On dit que ce diagramme est exact en F si le diagramme $E \xrightarrow{f} F \xrightarrow{g} G$ est une suite exacte ; on dit qu’il est exact en G si $F \xrightarrow{g} G \xrightarrow{h} H$ est une suite exacte. Si (5) est exact en F et en G, on dit qu’il est exact, ou encore que c’est une suite exacte. On définit de même les suites exactes à un nombre quelconque de termes.

Rappelons aussi les résultats suivants (loc. cit.), où E, F, G désignent des A-modules à droite (resp. à gauche), les flèches représentent des homomorphismes, et 0 désigne un module réduit à son élément neutre :

a) Dire que $0 \to E \xrightarrow{f} F$ est une suite exacte équivaut à dire que $f$ est injectif.

b) Dire que $E \xrightarrow{f} F \to 0$ est une suite exacte équivaut à dire que $f$ est surjectif.

c) Dire que $0 \to E \xrightarrow{f} F \to 0$ est une suite exacte équivaut à dire que $f$ est bijectif, c’est-à-dire que $f$ est un isomorphisme de E sur F.

d) Si F est un sous-module de E et si l’on note i l’injection canonique de F dans E et p la surjection canonique de E sur E/F, le diagramme

(6)
$$
0 \longrightarrow F \xrightarrow{i} E \xrightarrow{p} E/F \longrightarrow 0
$$
est une suite exacte.

e) Si $f : E \to F$ est un homomorphisme, le diagramme

(7)
$$
0 \longrightarrow \overline{f}(0) \xrightarrow{i} E \xrightarrow{f} F \xrightarrow{p} F/f(E) \longrightarrow 0
$$
(où $i$ est l’injection canonique de $\overline{f}(0)$ dans E, et $p$ la surjection canonique de F sur $F/f(E)$) est une suite exacte.

f) Pour qu’un diagramme

(8)
$$
E \xrightarrow{f} F \xrightarrow{g} G
$$
soit une suite exacte, il faut et il suffit qu’il existe des modules S, T et des homomorphismes $a : E \to S$, $b : S \to F$, $c : F \to T$ et $d : T \to G$ tels que $f = b \circ a$, $g = d \circ c$, et que les trois suites

(9)
$$
\begin{array}{c}
E \xrightarrow{a} S \longrightarrow 0 \\
0 \longrightarrow S \xrightarrow{b} F \xrightarrow{c} T \longrightarrow 0 \\
0 \longrightarrow T \xrightarrow{d} G
\end{array}
$$
soient exactes.

Rappelons enfin que si $f : E \to F$ est un homomorphisme de A-modules, on pose $\mathrm{Ker}\,(f) = \overline{f}(0)$, $\mathrm{Im}\,(f) = f(E)$, $\mathrm{Coim}\,(f) = E/\overline{f}(0)$ et $\mathrm{Coker}\,(f) = F/f(E)$. Avec ces notations, on peut prendre, dans (9), $S = \mathrm{Im}\,(f) = \mathrm{Ker}\,(g)$ et $T = \mathrm{Im}\,(g)$ (isomorphe canoniquement à $\mathrm{Coker}\,(f)$).

### 4. Le diagramme du serpent.

#### Proposition 1 {#ac-i-s1-prop-1 .statement}

Considérons un diagramme commutatif de groupes commutatifs :

(10)
$$
\begin{array}{ccccc}
A & \xrightarrow{u} & B & \xrightarrow{v} & C \\
a \downarrow & & b \downarrow & & c \downarrow \\
A' & \xrightarrow{u'} & B' & \xrightarrow{v'} & C'
\end{array}
$$

On suppose que les deux lignes de (10) sont exactes. Alors :

(i) Si c est injectif, on a

(11) $\operatorname{Im}(b) \cap \operatorname{Im}(u') = \operatorname{Im}(u' \circ a) = \operatorname{Im}(b \circ u).$

(ii) Si a est surjectif, on a

(12) $\operatorname{Ker}(b) + \operatorname{Im}(u) = \operatorname{Ker}(\varphi' \circ b) = \operatorname{Ker}(c \circ \varphi).$

Prouvons (i). Il est clair que l’on a

$$
\operatorname{Im}(u' \circ a) = \operatorname{Im}(b \circ u) \subset \operatorname{Im}(b) \cap \operatorname{Im}(u').
$$

Inversement, soit $x \in \operatorname{Im}(b) \cap \operatorname{Im}(u')$. Il existe $y \in B$ tel que $x = b(y)$. Comme $\varphi' \circ u' = 0$, on a $0 = \varphi'(x) = \varphi'(b(y)) = c(\varphi(y))$, d’où $\varphi(y) = 0$ puisque c est injectif. Comme $(u, \varphi)$ est une suite exacte, il existe $z \in A$ tel que $y = u(z)$, d’où $x = b(u(z))$.

Prouvons (ii). Comme $\varphi \circ u = 0$ et $\varphi' \circ u' = 0$, il est clair que

$$
\operatorname{Ker}(b) + \operatorname{Im}(u) \subset \operatorname{Ker}(\varphi' \circ b) = \operatorname{Ker}(c \circ \varphi).
$$

Inversement, soit $x \in \operatorname{Ker}(\varphi' \circ b)$. Alors $b(x) \in \operatorname{Ker}(\varphi')$, et il existe $y' \in A'$ tel que $u'(y') = b(x)$ puisque la suite $(u', \varphi')$ est exacte. Comme $a$ est surjectif, il existe $y \in A$ tel que $a(y) = y'$, d’où $b(x) = u'(a(y)) = b(u(y))$; on en conclut que $x - u(y) \in \operatorname{Ker}(b)$, ce qui termine la démonstration.

#### Lemme 1 {#ac-i-s1-lem-1 .statement}

Considérons un diagramme commutatif de groupes commutatifs :

$$
\begin{array}{ccc}
A & \xrightarrow{u} & B \\
a \downarrow & & \downarrow b \\
A' & \xrightarrow{u'} & B'
\end{array}
$$

Alors il existe un homomorphisme et un seul $u_1 : \operatorname{Ker}(a) \to \operatorname{Ker}(b)$, et un homomorphisme et un seul $u_2 : \operatorname{Coker}(a) \to \operatorname{Coker}(b)$, tels que les diagrammes

$$
\begin{array}{ccc}
\operatorname{Ker}(a) & \xrightarrow{u_1} & \operatorname{Ker}(b) \\
i \downarrow & & \downarrow j \\
A & \xrightarrow{u} & B
\end{array}
$$

et

$$
\begin{array}{ccc}
A' & \xrightarrow{u'} & B' \\
p \downarrow & & \downarrow q \\
\operatorname{Coker}(a) & \xrightarrow{u_2} & \operatorname{Coker}(b)
\end{array}
$$

soient commutatifs, i et j désignant les injections canoniques, p et q les surjections canoniques.

En effet, si $x \in \mathrm{Ker}\,(a)$, on a $a(x) = 0$ et $b(u(x)) = u'(a(x)) = 0$, donc $u(x) \in \mathrm{Ker}\,(b)$, et l’existence et l’unicité de $u_1$ sont alors immédiates. De même, on a $u'(a(A)) = b(u(A)) \subset b(B)$, donc $u'$ donne par passage aux quotients un homomorphisme $u_2 : \mathrm{Coker}\,(a) \to \mathrm{Coker}\,(b)$, qui est le seul homomorphisme pour lequel (15) soit commutatif.

Partons maintenant d’un diagramme commutatif (10) de groupes commutatifs ; il lui correspond en vertu du lemme 1 un diagramme

$$
\begin{array}{ccccccccc}
\mathrm{Ker}\,(a) & \xrightarrow{u_1} & \mathrm{Ker}\,(b) & \xrightarrow{v_1} & \mathrm{Ker}\,(c) \\
i \downarrow & & i \downarrow & & k \downarrow \\
A & \xrightarrow{u} & B & \xrightarrow{v} & C \\
a \downarrow & & b \downarrow & & c \downarrow \\
A' & \xrightarrow{u'} & B' & \xrightarrow{v'} & C' \\
p \downarrow & & q \downarrow & & r \downarrow \\
\mathrm{Coker}\,(a) & \xrightarrow{u_2} & \mathrm{Coker}\,(b) & \xrightarrow{v_2} & \mathrm{Coker}\,(c)
\end{array}
$$

où $i, j, k$ sont les injections canoniques, $p, q, r$ les surjections canoniques, $u_1, u_2$ (resp. $v_1, v_2$) les homomorphismes canoniquement associés à $u, u'$ (resp. $v, v'$) par le lemme 1. On vérifie aussitôt que ce diagramme est commutatif.

#### Proposition 2 {#ac-i-s1-prop-2 .statement}

*Supposons que dans le diagramme commutatif (10), les suites $(u, v)$ et $(u', v')$ soient exactes. Alors* :

(i) *On a $v_1 \circ u_1 = 0$; si $u'$ est injectif, la suite $(u_1, v_1)$ est exacte.*

(ii) *On a $v_2 \circ u_2 = 0$; si $v$ est surjectif, la suite $(u_2, v_2)$ est exacte.*

(iii) *Supposons $u'$ injectif et $v$ surjectif. Il existe alors un homomorphisme et un seul $d : \mathrm{Ker}\,(c) \to \mathrm{Coker}\,(a)$ ayant la propriété suivante : si $x \in \mathrm{Ker}\,(c)$, $y \in B$ et $t' \in A'$ vérifient les relations $v(y) = k(x)$ et $u'(t') = b(y)$, on a $d(x) = p(t')$. De plus la suite*

(*)

$$
\mathrm{Ker}\,(a) \xrightarrow{u_1} \mathrm{Ker}\,(b) \xrightarrow{v_1} \mathrm{Ker}\,(c) \xrightarrow{d} \mathrm{Coker}\,(a) \xrightarrow{u_2} \mathrm{Coker}\,(b) \xrightarrow{v_2} \mathrm{Coker}\,(c)
$$

*est exacte.*

Prouvons (i). Comme $u_1$ et $v_1$ ont mêmes graphes que les restrictions de $u$ et $v$ à $\mathrm{Ker}(a)$ et $\mathrm{Ker}(b)$ respectivement, on a $v_1 \circ u_1 = 0$. On a $\mathrm{Ker}(v_1) = \mathrm{Ker}(b) \cap \mathrm{Ker}(v) = \mathrm{Ker}(b) \cap \mathrm{Im}(u) = \mathrm{Im}(j) \cap \mathrm{Im}(u)$. Mais d’après la prop. 1, (i), on a $\mathrm{Ker}(v_1) = \mathrm{Im}(j \circ u_1) = \mathrm{Im}(u_1)$ si $u'$ est injectif.

Prouvons (ii). Comme $u_2$ et $v_2$ proviennent de $u$ et $v$ par passage aux quotients, il est clair que $v_2 \circ u_2 = 0$. Supposons $v$ surjectif ; comme $q$ et $p$ sont surjectifs, on a, en vertu des hypothèses et de la prop. 1, (ii)

$$
\begin{align*}
\mathrm{Ker}(v_2) &= q(\mathrm{Ker}(v_2 \circ q)) = q(\mathrm{Ker}(v') + \mathrm{Im}(b)) = q(\mathrm{Ker}(v')) \\
&= q(\mathrm{Im}(u')) = \mathrm{Im}(q \circ u') = \mathrm{Im}(u_2 \circ p) = \mathrm{Im}(u_2).
\end{align*}
$$

Prouvons enfin (iii). Pour $x \in \mathrm{Ker}(c)$, il existe $y \in B$ tel que $v(y) = k(x)$ puisque $v$ est surjectif ; en outre, on a $v'(b(y)) = c(k(x)) = 0$, et par suite il existe un unique $t' \in A'$ tel que $u'(t') = b(y)$ puisque $u'$ est injectif. Montrons que l’élément $p(t') \in \mathrm{Coker}(a)$ est indépendant de l’élément $y \in B$ tel que $v(y) = k(x)$. En effet, si $y' \in B$ est un second élément tel que $v(y') = k(x)$, on a $y' = y + u(z)$ où $z \in A$ ; montrons que si $t'' \in A'$ est tel que $u'(t'') = b(y')$ on a $t'' = t' + a(z)$ ; en effet on a $u'(t' + a(z)) = u'(t') + u'(a(z)) = b(y) + b(u(z)) = b(y + u(z)) = b(y')$. Enfin, on en conclut que $p(t'') = p(t') + p(a(z)) = p(t')$. On peut donc poser $d(x) = p(t')$ et on a ainsi défini une application $d : \mathrm{Ker}(c) \to \mathrm{Coker}(a)$.

Si maintenant $x_1, x_2$ sont des éléments de $\mathrm{Ker}(c)$ et $x = x_1 + x_2$, on prendra des éléments $y_1$ et $y_2$ de $B$ tels que $v(y_1) = k(x_1)$ et $v(y_2) = k(x_2)$ et on choisira pour $y \in B$ l’élément $y_1 + y_2$ ; il est alors immédiat que $d(x) = d(x_1) + d(x_2)$, donc $d$ est un homomorphisme.

Supposons que $x = v_1(x')$ pour un $x' \in \mathrm{Ker}(b)$ ; on prendra alors pour $y \in B$ l’élément $j(x')$. Comme $b(j(x')) = 0$, on en conclut $d(x) = 0$, donc $d \circ v_1 = 0$. Inversement, supposons que $d(x) = 0$. Avec les notations précédentes, on a donc $t' = a(s)$, où $s \in A$. Dans ce cas, on a $b(y) = u'(t') = u'(a(s)) = b(u(s))$, ou encore $b(y - u(s)) = 0$. L’élément $y - u(s)$ est donc de la forme $j(n)$ pour $n \in \mathrm{Ker}(b)$, et on a $k(x) = v(y) = v(u(s) + j(n)) = v(j(n)) = k(v_1(n))$ ; comme $k$ est injectif, $x = v_1(n)$, ce qui prouve que la suite (*) est exacte en $\mathrm{Ker}(c)$.

Enfin, on a (toujours avec les mêmes notations) $u_2(d(x)) =$ u_2(p(t')) = q(u'(t')) = q(b(y)) = 0 donc u_2 \circ d = 0. Inversement, supposons qu’un élément $w = p(t')$ de Coker (a) soit tel que $u_2(w) = u_2(p(t')) = 0$ (avec $t' \in \mathbf{A}'$). On a donc $q(u'(t')) = 0$, et par suite $u'(t') = b(y)$ pour un $y \in \mathbf{B}$; comme $\varphi'(u'(t')) = 0$, on a $\varphi'(b(y)) = 0$, donc $c(\varphi(y)) = 0$, autrement dit $\varphi(y) = k(x)$ pour un $x \in \mathrm{Ker}\,(c)$, et par définition $w = d(x)$, ce qui montre que la suite (*) est exacte en Coker (a). On a vu dans (i) qu’elle est exacte en Ker (b) et dans (ii) qu’elle est exacte en Coker (b), ce qui achève de prouver (iii).

#### Remarque {#ac-i-s1-n4-rem-1 .statement}

Lorsque les groupes du diagramme (10) sont tous des modules (à droite par exemple) sur un anneau $\Lambda$ et les homomorphismes des homomorphismes de $\Lambda$-modules, on vérifie aussitôt que l’homomorphisme $d$ défini dans la prop. 2, (iii) est encore un homomorphisme de $\Lambda$-modules : si $x \in \mathrm{Ker}\,(c)$ et $\alpha \in \Lambda$, et si $y \in \mathbf{B}$ est tel que $\varphi(y) = k(x)$, il suffit de remarquer que $\varphi(y\alpha) = k(x\alpha)$.

#### Corollaire 1 {#ac-i-s1-prop-2-cor-1 .statement}

Supposons que le diagramme (10) soit commutatif et ait ses lignes exactes. Alors :
(i) Si $u'$, $a$ et $c$ sont injectifs, $b$ est injectif.
(ii) Si $\varphi$, $a$ et $c$ sont surjectifs, $b$ est surjectif.

L’assertion (i) est conséquence de l’assertion (i) de la prop. 2 : en effet on a $\mathrm{Ker}\,(a) = 0$ et $\mathrm{Ker}\,(c) = 0$, donc $\mathrm{Ker}\,(b) = 0$.

L’assertion (ii) est conséquence de l’assertion (ii) de la prop. 2 : en effet, on a $\mathrm{Coker}\,(a) = 0$ et $\mathrm{Coker}\,(c) = 0$, donc $\mathrm{Coker}\,(b) = 0$.

#### Corollaire 2 {#ac-i-s1-prop-2-cor-2 .statement}

Supposons que le diagramme (10) soit commutatif et ait ses lignes exactes. Dans ces conditions :
(i) Si $b$ est injectif et si $a$ et $\varphi$ sont surjectifs, alors $c$ est injectif.
(ii) Si $b$ est surjectif et si $c$ et $u'$ sont injectifs, alors $a$ est surjectif.

Pour prouver (i), considérons le diagramme

$$
\begin{array}{cccc}
u(\mathbf{A}) & \xrightarrow{w} & \mathbf{B} \xrightarrow{\varphi} \mathbf{C} \\
a' \downarrow & & b \downarrow & c \downarrow \\
u'(\mathbf{A}') & \xrightarrow{w'} & \mathbf{B}' \xrightarrow{\varphi'} \mathbf{C}'
\end{array}
$$

où $a'$ est l’application ayant même graphe que la restriction de $b$ à $u(\mathbf{A})$, $w$ et $w'$ les injections canoniques ; il est clair que ce diagramme est commutatif et a ses lignes exactes. En outre $w'$ est injectif, et par hypothèse $\varphi$ est surjectif ; on a donc par la prop. 2, (iii), une suite exacte.

$$
0 = \mathrm{Ker}\,(b) \to \mathrm{Ker}\,(c) \xrightarrow{d} \mathrm{Coker}\,(a') = 0
$$

puisque $b$ est injectif et que $a'$ est surjectif ; d’où $\mathrm{Ker}\,(c) = 0$.

Pour prouver (ii), considérons le diagramme

$$
\begin{array}{ccccc}
A & \xrightarrow{u} & B & \xrightarrow{w} & \varphi(B) \\
a \downarrow & & b \downarrow & & c' \downarrow \\
A' & \xrightarrow{u'} & B' & \xrightarrow{w'} & \varphi'(B')
\end{array}
$$

où cette fois $c'$ est l’application ayant même graphe que la restriction de $c$ à $\varphi(B)$, et $w$ et $w'$ ont respectivement mêmes graphes que $\varphi$ et $\varphi'$ ; ce diagramme est commutatif et ses lignes sont exactes. En outre $w$ est surjectif et par hypothèse $u'$ est injectif ; on a donc, par la prop. 2, (iii), une suite exacte

$$
0 = \mathrm{Ker}\,(c') \xrightarrow{d} \mathrm{Coker}\,(a) \to \mathrm{Coker}\,(b) = 0
$$

puisque $b$ est surjectif et que $c'$ est injectif ; d’où $\mathrm{Coker}\,(a) = 0$.

## EXERCICES {#ac-i-s1-exercises}

See the [exercises for § 1](exercises/s1/).
