---
book: alg
book_title: Algebra
chapter: X
chapter_title: ALGÈBRE HOMOLOGIQUE
section: 1
section_title: Compléments d’algèbre linéaire
lang: fr
source: alg-x-fr
book_pages: A X.168-A X.173
pdf_pages: 0007-0029, 0174-0179
extraction: ocr
subsections:
    - "no": 1
      title: Diagrammes commutatifs
      page: 0
      pdf_page: 7
    - "no": 2
      title: Le diagramme du serpent
      page: 3
      pdf_page: 9
    - "no": 3
      title: Modules plats
      page: 8
      pdf_page: 14
    - "no": 4
      title: Modules de présentation finie
      page: 10
      pdf_page: 16
    - "no": 5
      title: Homomorphismes d’un module de présentation finie
      page: 12
      pdf_page: 18
    - "no": 6
      title: Structure des modules plats
      page: 13
      pdf_page: 19
    - "no": 7
      title: Modules injectifs
      page: 15
      pdf_page: 21
    - "no": 8
      title: Modules cogénérateurs injectifs
      page: 18
      pdf_page: 24
    - "no": 9
      title: Enveloppes injectives
      page: 19
      pdf_page: 25
    - "no": 10
      title: Structure des modules injectifs
      page: 22
      pdf_page: 28
statements: 54
exercises: 17
content_sha256: bd3c41963bcd4825d6836308d2ec8fec47621486e6b81283e3fadd4d739f6f4a
---

## § 1. COMPLÉMENTS D’ALGÈBRE LINÉAIRE

Dans ce paragraphe, la lettre $\mathbf{A}$ désigne un anneau. Sauf mention expresse du contraire, tous les modules considérés sont des modules à gauche, tous les idéaux considérés sont des idéaux à gauche.

Les définitions et les résultats s’appliquent aux modules à droite, en les considérant comme modules à gauche sur l’anneau opposé.

Si $\mathbf{M}$ est un $\mathbf{A}$-module et si $a \in \mathbf{A}$, on note $a_M$ l’homothétie $x \mapsto ax$ de $\mathbf{M}$. On a donc $1_M = \mathrm{Id}_M$ (application identique de $\mathbf{M}$) ; lorsqu’il n’y a pas de confusion possible, on écrit parfois simplement $1$ au lieu de $1_M$.

Enfin, on note $0$ un $\mathbf{A}$-module réduit à son élément neutre, choisi une fois pour toutes (cf. II, p. 8).

### 1. Diagrammes commutatifs

Soient par exemple B, C, D, E, F cinq ensembles, et soient $f$ une application de E dans F, $g$ une application de B dans C, $h$ une application de D dans E, $u$ une application de B dans D et $v$ une application de C dans E. Pour résumer une situation de ce genre, on fait souvent usage de diagrammes ; par exemple, on résumera la situation précédente par le diagramme suivant (E, II, p. 14) :

$$
\begin{array}{ccc}
B & \xrightarrow{g} & C \\
u \downarrow & & v \downarrow \\
D & \xrightarrow{h} & E \xrightarrow{f} F .
\end{array}
$$

Dans un tel diagramme, le groupe de signes $E \xrightarrow{f} F$ schématise le fait que $f$ est une application de E dans F. Lorsqu’il ne peut y avoir d’ambiguïté sur $f$, on supprime la lettre $f$, et on écrit simplement $E \to F$.

Lorsque B, C, D, E, F sont des groupes (resp. des $\mathbf{A}$-modules) et $f, g, h, u, v$ des homomorphismes de groupes (resp. A-modules), on dit pour abréger que le diagramme (1) est un *diagramme de groupes* (resp. de A-modules).

En principe, un diagramme n’est pas un objet mathématique, mais seulement une *figure*, destinée à faciliter la lecture d’un raisonnement. En pratique, on se sert souvent des diagrammes comme de *symboles abréviateurs*, qui évitent de nommer tous les ensembles et toutes les applications que l’on veut considérer ; on dit ainsi « considérons le diagramme (1) » au lieu de dire : « soient B, C, D, E, F cinq ensembles... et $v$ une application de C dans E » ; voir par exemple l’énoncé de la prop. 1 du no 2.

Considérons par exemple le diagramme suivant :

$$
\begin{array}{ccccccc}
B & \xrightarrow{\ f\ } & C & \xrightarrow{\ g\ } & D & \xrightarrow{\ h\ } & E\\
{\scriptstyle b}\downarrow && {\scriptstyle c}\downarrow && {\scriptstyle d}\downarrow && {\scriptstyle e}\downarrow\\
B' & \xrightarrow{\ f'\ } & C' & \xrightarrow{\ g'\ } & D' & \xrightarrow{\ h'\ } & E'
\end{array}
\tag{2}
$$

A tout chemin composé d’un certain nombre de segments du diagramme parcouru dans le sens indiqué par les flèches, on fait correspondre une application de l’ensemble représenté par l’origine du premier segment dans l’ensemble représenté par l’extrémité du dernier segment, savoir la composée des applications représentées par les divers segments parcourus. Pour tout sommet du diagramme, par exemple C, on convient qu’il y a un chemin réduit à C et on lui fait correspondre l’application identique $1_C$.

Dans (2), il y a par exemple trois chemins partant de B et aboutissant à D$'$ ; les applications correspondantes sont $d\circ g\circ f$, $g'\circ c\circ f$ et $g'\circ f'\circ b$. On dit qu’un diagramme est *commutatif* si, pour tout couple de chemins du diagramme ayant même origine et même extrémité, les deux applications correspondantes sont égales ; en particulier si un chemin a son extrémité confondue avec son origine, l’application correspondante doit être l’identité.

Pour que le diagramme (2) soit commutatif, il faut et il suffit que l’on ait les relations :

$$
\tag{3}
f'\circ b=c\circ f,\qquad
g'\circ c=d\circ g,\qquad
h'\circ d=e\circ h ;
$$

autrement dit, il faut et il suffit que les trois diagrammes carrés extraits de (2) soient commutatifs. En effet, les relations (3) entraînent $d\circ g\circ f=g'\circ c\circ f$ puisque $d\circ g=g'\circ c$ et $g'\circ c\circ f=g'\circ f'\circ b$ puisque $c\circ f=f'\circ b$ ; donc les trois chemins partant de B et aboutissant à D$'$ donnent la même application. On vérifie de même que les quatre chemins partant de B et aboutissant à E$'$ (resp. les trois chemins partant de C et aboutissant à E$'$) donnent la même application. Les relations (3) signifient que les deux chemins partant de B (resp. C, D) et aboutissant à C$'$ (resp. D$'$, E$'$) donnent la même application. Tous les autres couples de sommets de (2) ne peuvent être joints que par un chemin au plus, et le diagramme (2) est donc bien commutatif.

Par la suite, nous laisserons au lecteur le soin de formuler et de vérifier des résultats analogues pour d’autres types de diagrammes.

### 2. Le diagramme du serpent

#### Proposition 1 {#alg-x-s1-prop-1 .statement}

Considérons un diagramme commutatif de A-modules

$$
\tag{4}
\begin{array}{ccccc}
M & \xrightarrow{u} & N & \xrightarrow{v} & P\\
\downarrow f & & \downarrow g & & \downarrow h\\
M' & \xrightarrow{u'} & N' & \xrightarrow{v'} & P'
\end{array}
$$

On suppose que les deux lignes de (4) sont exactes. Alors :

(i) Si $h$ est injectif, on a

$$
\tag{5}
\operatorname{Im}(g)\cap\operatorname{Im}(u')=\operatorname{Im}(u'\circ f)=\operatorname{Im}(g\circ u).
$$

(ii) Si $f$ est surjectif, on a

$$
\tag{6}
\operatorname{Ker}(g)+\operatorname{Im}(u)=\operatorname{Ker}(v'\circ g)=\operatorname{Ker}(h\circ v).
$$

Prouvons (i). Il est clair que l’on a

$$
\operatorname{Im}(u'\circ f)=\operatorname{Im}(g\circ u)\subset\operatorname{Im}(g)\cap\operatorname{Im}(u').
$$

Inversement, soit $y'\in\operatorname{Im}(g)\cap\operatorname{Im}(u')$. Il existe $y\in N$ tel que $y'=g(y)$. Comme $v'\circ u'=0$, on a $0=v'(y')=v'(g(y))=h(v(y))$, d’où $v(y)=0$ puisque $h$ est injectif. Comme $(u,v)$ est une suite exacte, il existe $x\in M$ tel que $y=u(x)$, d’où $y'=g(u(x))$.

Prouvons (ii). Comme $v\circ u=0$ et $v'\circ u'=0$, il est clair que

$$
\operatorname{Ker}(g)+\operatorname{Im}(u)\subset\operatorname{Ker}(v'\circ g)=\operatorname{Ker}(h\circ v).
$$

Inversement, soit $y\in\operatorname{Ker}(v'\circ g)$. Alors $g(y)\in\operatorname{Ker}(v')$, et il existe $x'\in M'$ tel que $u'(x')=g(y)$ puisque la suite $(u',v')$ est exacte. Comme $f$ est surjectif, il existe $x\in M$ tel que $f(x)=x'$, d’où $g(y)=u'(f(x))=g(u(x))$ ; on en conclut que $y-u(x)\in\operatorname{Ker}(g)$, ce qui termine la démonstration.

#### Lemme 1 {#alg-x-s1-lem-1 .statement}

Considérons un diagramme commutatif de A-modules

$$
\tag{7}
\begin{array}{ccc}
M & \xrightarrow{u} & N\\
\downarrow f & & \downarrow g\\
M' & \xrightarrow{u'} & N'
\end{array}
$$

Alors il existe un homomorphisme et un seul $u_1:\operatorname{Ker}(f)\to\operatorname{Ker}(g)$, et un homomorphisme et un seul $u_2:\operatorname{Coker}(f)\to\operatorname{Coker}(g)$, tels que les diagrammes

$$
\tag{8}
\begin{array}{ccc}
\operatorname{Ker}(f) & \xrightarrow{u_1} & \operatorname{Ker}(g)\\
\downarrow i & & \downarrow j\\
M & \xrightarrow{u} & N
\end{array}
$$

et

$$
\begin{array}{ccc}
M' & \xrightarrow{u'} & N' \\
p \downarrow & & q \downarrow \\
\text{Coker } (f) & \xrightarrow{u_2} & \text{Coker } (g)
\end{array}
$$

soient commutatifs, i et j désignant les injections canoniques, p et q les surjections canoniques.

En effet, si $x \in \text{Ker } (f)$, on a $f(\bar{x}) = 0$ et $g(u(x)) = u'(f(x)) = 0$, donc $u(x) \in \text{Ker } (g)$, et l’existence et l’unicité de $u_1$ sont alors immédiates. De même, on a
$$
u'(f(M)) = g(u(M)) \subset g(N),
$$
donc $u'$ donne par passage aux quotients un homomorphisme
$$
u_2 : \text{Coker } (f) \to \text{Coker } (g),
$$
qui est le seul homomorphisme pour lequel (9) soit commutatif.

Partons maintenant d’un diagramme commutatif (4) de A-modules ; il lui correspond en vertu du lemme 1 un diagramme commutatif

$$
\begin{array}{ccccccccc}
\text{Ker } (f) & \xrightarrow{u_1} & \text{Ker } (g) & \xrightarrow{v_1} & \text{Ker } (h) \\
i \downarrow & & j \downarrow & & k \downarrow \\
M & \xrightarrow{u} & N & \xrightarrow{v} & P \\
f \downarrow & & g \downarrow & & h \downarrow \\
M' & \xrightarrow{u'} & N' & \xrightarrow{v'} & P' \\
p \downarrow & & q \downarrow & & r \downarrow \\
\text{Coker } (f) & \xrightarrow{u_2} & \text{Coker } (g) & \xrightarrow{v_2} & \text{Coker } (h)
\end{array}
$$

où $i, j, k$ sont les injections canoniques, $p, q, r$ les surjections canoniques, $u_1, u_2$ (resp. $v_1, v_2$) les homomorphismes déduits de $u, u'$ (resp. $v, v'$) par le lemme 1.

#### Proposition 2 {#alg-x-s1-prop-2 .statement}

Supposons que dans le diagramme commutatif (4), les suites $(u, v)$ et $(u', v')$ soient exactes. Alors :
(i) On a $v_1 \circ u_1 = 0$; si $u'$ est injectif, la suite $(u_1, v_1)$ est exacte.
(ii) On a $v_2 \circ u_2 = 0$; si $v$ est surjectif, la suite $(u_2, v_2)$ est exacte.
(iii) Supposons $u'$ injectif et $v$ surjectif. Il existe alors un homomorphisme et un seul $d : \text{Ker } (h) \to \text{Coker } (f)$ ayant la propriété suivante : si $z \in \text{Ker } (h), y \in N$ et $x' \in M'$ vérifient les relations $v(y) = k(z)$ et $u'(x') = g(y)$, on a $d(z) = p(x')$. De plus la suite
(*) $\text{Ker } (f) \xrightarrow{u_1} \text{Ker } (g) \xrightarrow{v_1} \text{Ker } (h) \xrightarrow{d} \text{Coker } (f) \xrightarrow{u_2} \text{Coker } (g) \xrightarrow{v_2} \text{Coker } (h)$
est exacte.

$$
\begin{array}{ccccc}
\operatorname{Ker}(f)&\xrightarrow{u_1}&\operatorname{Ker}(g)&\xrightarrow{v_1}&\operatorname{Ker}(h)\\
\downarrow\scriptstyle i&&\downarrow\scriptstyle j&&\downarrow\scriptstyle k\\
M&\xrightarrow{u}&N&\xrightarrow{v}&P\\
\downarrow\scriptstyle f&&\downarrow\scriptstyle g&&\downarrow\scriptstyle h\\
M'&\xrightarrow{u'}&N'&\xrightarrow{v'}&P'\\
\downarrow\scriptstyle p&&\downarrow\scriptstyle q&&\downarrow\scriptstyle r\\
\operatorname{Coker}(f)&\xrightarrow{u_2}&\operatorname{Coker}(g)&\xrightarrow{v_2}&\operatorname{Coker}(h)
\end{array}
$$

Prouvons (i). Comme $u_1$ et $v_1$ ont mêmes graphes que les restrictions de $u$ et $v$ à $\operatorname{Ker}(f)$ et $\operatorname{Ker}(g)$ respectivement, on a $v_1\circ u_1=0$. On a

$$
\operatorname{Ker}(v_1)=\operatorname{Ker}(g)\cap\operatorname{Ker}(v)=\operatorname{Ker}(g)\cap\operatorname{Im}(u)=\operatorname{Im}(j)\cap\operatorname{Im}(u).
$$

Mais d’après la prop. 1 (i), on a $\operatorname{Ker}(v_1)=\operatorname{Im}(j\circ u_1)=\operatorname{Im}(u_1)$ si $u'$ est injectif.

Prouvons (ii). Comme $u_2$ et $v_2$ proviennent de $u$ et $v$ par passage aux quotients, il est clair que $v_2\circ u_2=0$. Supposons $v$ surjectif; comme $q$ et $p$ sont surjectifs, on a, en vertu des hypothèses et de la prop. 1 (ii)

$$
\begin{aligned}
\operatorname{Ker}(v_2)&=q(\operatorname{Ker}(v_2\circ q))=q(\operatorname{Ker}(v')+\operatorname{Im}(g))=q(\operatorname{Ker}(v'))\\
&=q(\operatorname{Im}(u'))=\operatorname{Im}(q\circ u')=\operatorname{Im}(u_2\circ p)=\operatorname{Im}(u_2).
\end{aligned}
$$

Prouvons enfin (iii). Pour $z\in\operatorname{Ker}(h)$, il existe $y\in N$ tel que $v(y)=k(z)$ puisque $v$ est surjectif; en outre, on a $v'(g(y))=h(k(z))=0$, et par suite il existe un unique $x'\in M'$ tel que $u'(x')=g(y)$ puisque $u'$ est injectif. Montrons que l’élément $p(x')\in\operatorname{Coker}(f)$ est indépendant de l’élément $y\in N$ tel que $v(y)=k(z)$. En effet, si $y_1\in N$ est un second élément tel que $v(y_1)=k(z)$, on a $y_1=y+u(x)$ où $x\in M$; montrons que si $x'_1\in M'$ est tel que $u'(x'_1)=g(y_1)$, on a $x'_1=x'+f(x)$; en effet, on a $u'(x'+f(x))=u'(x')+u'(f(x))=g(y)+g(u(x))=g(y+u(x))=g(y_1)$. Enfin, on en conclut que $p(x'_1)=p(x')+p(f(x))=p(x')$. On peut donc poser $d(z)=p(x')$ et on a ainsi défini une application $d:\operatorname{Ker}(h)\to\operatorname{Coker}(f)$.

Si maintenant $z_1,z_2$ sont des éléments de $\operatorname{Ker}(h)$, si $\lambda_1,\lambda_2\in A$ et $z=\lambda_1z_1+\lambda_2z_2$, on prendra des éléments $y_1$ et $y_2$ de $N$ tels que $v(y_1)=k(z_1)$ et $v(y_2)=k(z_2)$ et on choisira pour $y\in N$ l’élément $\lambda_1y_1+\lambda_2y_2$; il est alors immédiat que

$$
d(z)=\lambda_1d(z_1)+\lambda_2d(z_2),
$$

donc $d$ est un homomorphisme.

Supposons que $z=v_1(t)$ pour un $t\in\operatorname{Ker}(g)$; on prendra alors pour $y\in N$ l’élément $j(t)$. Comme $g(j(t))=0$, on en conclut $d(z)=0$, donc $d\circ v_1=0$. Inversement, supposons que $d(z)=0$. Avec les notations précédentes, on a donc $x'=f(x)$, où x ∈ M. Dans ce cas, on a $g(y) = u'(f(x)) = g(u(x))$, ou encore $g(y - u(x)) = 0$. L’élément $y - u(x)$ est donc de la forme $j(n)$ pour $n \in \mathrm{Ker}\,(g)$, et on a

$$
k(z) = v(y) = v(u(x) + j(n)) = v(j(n)) = k(v_1(n));
$$

comme $k$ est injectif, $z = v_1(n)$, ce qui prouve que la suite (*) est exacte en $\mathrm{Ker}\,(h)$.

Enfin, on a (toujours avec les mêmes notations)

$$
u_2(d(z)) = u_2(p(x')) = q(u'(x')) = q(g(y)) = 0 \quad \text{donc} \quad u_2 \circ d = 0 .
$$

Inversement, supposons qu’un élément $w = p(x')$ de $\mathrm{Coker}\,(f)$ soit tel que

$$
u_2(w) = u_2(p(x')) = 0 \quad (\text{avec } x' \in \mathbf{M}') .
$$

On a donc $q(u'(x')) = 0$, et par suite $u'(x') = g(y)$ pour un $y \in \mathbf{N}$; comme $v'(u'(x')) = 0$, on a $v'(g(y)) = 0$, donc $h(v(y)) = 0$, autrement dit $v(y) = k(z)$ pour un $z \in \mathrm{Ker}\,(h)$, et par définition $w = d(z)$, ce qui montre que la suite (*) est exacte en $\mathrm{Coker}\,(f)$. On a vu dans (i) qu’elle est exacte en $\mathrm{Ker}\,(g)$ et dans (ii) qu’elle est exacte en $\mathrm{Coker}\,(g)$, ce qui achève de prouver (iii).

#### Corollaire 1 {#alg-x-s1-prop-2-cor-1 .statement}

Supposons que le diagramme (4) soit commutatif et ait ses lignes exactes. Alors :

(i) Si $u', f$ et $h$ sont injectifs, $g$ est injectif.
(ii) Si $v, f$ et $h$ sont surjectifs, $g$ est surjectif.

L’assertion (i) est conséquence de l’assertion (i) de la prop. 2 : en effet on a $\mathrm{Ker}\,(f) = 0$ et $\mathrm{Ker}\,(h) = 0$, donc $\mathrm{Ker}\,(g) = 0$.

L’assertion (ii) est conséquence de l’assertion (ii) de la prop. 2 : en effet, on a $\mathrm{Coker}\,(f) = 0$ et $\mathrm{Coker}\,(h) = 0$, donc $\mathrm{Coker}\,(g) = 0$.

#### Corollaire 2 {#alg-x-s1-prop-2-cor-2 .statement}

Supposons que le diagramme (4) soit commutatif et ait ses lignes exactes. Dans ces conditions :

(i) Si $g$ est injectif et si $f$ et $v$ sont surjectifs, alors $h$ est injectif.
(ii) Si $g$ est surjectif et si $h$ et $u'$ sont injectifs, alors $f$ est surjectif.

Pour prouver (i), considérons le diagramme

$$
\begin{array}{ccccc}
u(\mathbf{M}) & \xrightarrow{w} & \mathbf{N} & \xrightarrow{v} & \mathbf{P} \\
f' \downarrow & & g \downarrow & & h \downarrow \\
u'(\mathbf{M}') & \xrightarrow{w'} & \mathbf{N}' & \xrightarrow{v'} & \mathbf{P}'
\end{array}
$$

où $f'$ est l’application ayant même graphe que la restriction de $g$ à $u(\mathbf{M})$, $w$ et $w'$ les injections canoniques ; il est clair que ce diagramme est commutatif et a ses lignes exactes. En outre $w'$ est injectif, et par hypothèse $v$ est surjectif ; on a donc par la prop. 2 (iii), une suite exacte

$$
\mathrm{Ker}\,(g) \longrightarrow \mathrm{Ker}\,(h) \xrightarrow{d} \mathrm{Coker}\,(f');
$$

puisque $g$ est injectif et que $f'$ est surjectif, on a donc $\mathrm{Ker}\,(h) = 0$.

Pour prouver (ii), considérons le diagramme

$$
\begin{array}{ccccc}
M&\xrightarrow{u}&N&\xrightarrow{w}&\nu(N)\\
{\scriptstyle f}\downarrow&&{\scriptstyle g}\downarrow&&{\scriptstyle h'}\downarrow\\
M'&\xrightarrow{u'}&N'&\xrightarrow{w'}&\nu'(N')
\end{array}
$$

où cette fois $h'$ est l’application ayant même graphe que la restriction de $h$ à $\nu(N)$, et $w$ et $w'$ ont respectivement mêmes graphes que $\nu$ et $\nu'$; ce diagramme est commutatif et ses lignes sont exactes. En outre $w$ est surjectif et par hypothèse $u'$ est injectif ; on a donc, par la prop. 2 (iii), une suite exacte

$$
\operatorname{Ker}(h')\xrightarrow{d}\operatorname{Coker}(f)\longrightarrow\operatorname{Coker}(g);
$$

puisque $g$ est surjectif et que $h'$ est injectif, on a donc $\operatorname{Coker}(f)=0$.

**Corollaire 3 (Lemme des cinq).** — Considérons un diagramme commutatif de $A$-modules

$$
\begin{array}{ccccccccc}
M_1&\xrightarrow{u_1}&M_2&\xrightarrow{u_2}&M_3&\xrightarrow{u_3}&M_4&\xrightarrow{u_4}&M_5\\
{\scriptstyle f_1}\downarrow&&{\scriptstyle f_2}\downarrow&&{\scriptstyle f_3}\downarrow&&{\scriptstyle f_4}\downarrow&&{\scriptstyle f_5}\downarrow\\
M'_1&\xrightarrow{u'_1}&M'_2&\xrightarrow{u'_2}&M'_3&\xrightarrow{u'_3}&M'_4&\xrightarrow{u'_4}&M'_5
\end{array}
$$

où les lignes sont exactes.

(i) Si $f_2$ et $f_4$ sont injectifs et $f_1$ surjectif, $f_3$ est injectif.

(ii) Si $f_2$ et $f_4$ sont surjectifs et $f_5$ injectif, $f_3$ est surjectif.

En particulier, si $f_1$, $f_2$, $f_4$ et $f_5$ sont des isomorphismes, il en est de même de $f_3$.

Pour prouver (i), posons $\widetilde M_2=\operatorname{Coker}(u_1)$, $\widetilde M'_2=\operatorname{Coker}(u'_1)$ et notons $\widetilde f_2:\widetilde M_2\to\widetilde M'_2$ l’application déduite de $f_2$. Il résulte du cor. 2 (i) que $\widetilde f_2$ est injectif. En appliquant le cor. 1 (i) au diagramme

$$
\begin{array}{ccccc}
\widetilde M_2&\xrightarrow{\widetilde u_2}&M_3&\xrightarrow{u_3}&M_4\\
{\scriptstyle \widetilde f_2}\downarrow&&{\scriptstyle f_3}\downarrow&&{\scriptstyle f_4}\downarrow\\
\widetilde M'_2&\xrightarrow{\widetilde u'_2}&M'_3&\xrightarrow{u'_3}&M'_4
\end{array}
$$

où $\widetilde u_2$ et $\widetilde u'_2$ sont déduits de $u_2$ et $u'_2$, on voit que $f_3$ est injectif.

Pour prouver (ii), posons $\widetilde M_4=\operatorname{Ker}(u_4)$, $\widetilde M'_4=\operatorname{Ker}(u'_4)$ et notons $\widetilde f_4:\widetilde M_4\to\widetilde M'_4$ l’application induite par $f_4$. Il résulte du cor. 2 (ii) que $\widetilde f_4$ est surjectif. En appliquant le cor. 1 (ii) au diagramme

$$
\begin{array}{ccccc}
M_2&\xrightarrow{u_2}&M_3&\xrightarrow{\widetilde u_3}&\widetilde M_4\\
{\scriptstyle f_2}\downarrow&&{\scriptstyle f_3}\downarrow&&{\scriptstyle \widetilde f_4}\downarrow\\
M'_2&\xrightarrow{u'_2}&M'_3&\xrightarrow{\widetilde u'_3}&\widetilde M'_4
\end{array}
$$

où $\widetilde u_3$ et $\widetilde u'_3$ ont même graphe que $u_3$ et $u'_3$, on voit que $f_3$ est surjectif.

### 3. Modules plats

#### Définition 1 {#alg-x-s1-def-1 .statement}

On dit que le A-module E est plat, si pour toute suite exacte de A-modules à droite et d’homomorphismes

(11) $M' \xrightarrow{u} M \xrightarrow{v} M''$,

la suite d’applications $\mathbf{Z}$-linéaires

(12) $M' \otimes_A E \xrightarrow{u \otimes 1} M \otimes_A E \xrightarrow{v \otimes 1} M'' \otimes_A E$

est exacte.

#### Proposition 3 {#alg-x-s1-prop-3 .statement}

Pour que le A-module E soit plat, il faut et il suffit que, pour tout A-homomorphisme injectif $u : M' \to M$ de A-modules à droite, l’application $u \otimes 1 : M' \otimes_A E \to M \otimes_A E$ soit injective.

Si E est plat et $u : M' \to M$ injectif, la suite $0 \to M' \xrightarrow{u} M$ est exacte, donc aussi la suite $0 \longrightarrow M' \otimes_A E \xrightarrow{u \otimes 1} M \otimes_A E$, et $u \otimes 1$ est injectif. Inversement, considérons la suite exacte (11); posons $M''_1 = v(M)$, et soit $i : M''_1 \to M''$ l’injection canonique et $p : M \to M''_1$ l’application $m \mapsto v(m)$. La suite $M' \xrightarrow{u} M \xrightarrow{p} M''_1 \longrightarrow 0$ est exacte; d’après II, p. 58, prop. 5, la suite $M' \otimes_A E \xrightarrow{u \otimes 1} M \otimes_A E \xrightarrow{p \otimes 1} M''_1 \otimes_A E$ est donc exacte. Par ailleurs, on a $v = i \circ p$, donc $(v \otimes 1) = (i \otimes 1) \circ (p \otimes 1)$; si E satisfait à la condition de l’énoncé, alors $i \otimes 1$ est injectif, donc

$$
\operatorname{Ker}(v \otimes 1) = \operatorname{Ker}(p \otimes 1) = \operatorname{Im}(u \otimes 1)
$$

et la suite (12) est exacte.

#### Proposition 4 {#alg-x-s1-prop-4 .statement}

(i) Soient $(E_i)_{i \in I}$ une famille de A-modules, $E = \bigoplus_{i \in I} E_i$ leur somme directe. Pour que le A-module E soit plat, il faut et il suffit que chacun des $E_i$ le soit.

(ii) Soient I un ensemble préordonné filtrant à droite, $(E_\alpha, f_{\beta \alpha})$ un système inductif de A-modules relatif à I, $E = \varinjlim E_\alpha$ sa limite inductive. Si chacun des A-modules $E_\alpha$ est plat, alors E est plat.

Soit $M' \to M \to M''$ une suite exacte de A-modules à droite.

(i) Pour que la suite $\bigoplus_{i \in I} (M' \otimes_A E_i) \to \bigoplus_{i \in I} (M \otimes_A E_i) \to \bigoplus_{i \in I} (M'' \otimes_A E_i)$ soit exacte, il faut et il suffit que chacune des suites $M' \otimes_A E_i \to M \otimes_A E_i \to M'' \otimes_A E_i$ le soit (II, p. 13, prop. 7) ce qui démontre (i) puisque $\bigoplus (M \otimes_A E_i)$ s’identifie canoniquement à $M \otimes_A E$ (II, p. 61, prop. 7).

(ii) Par hypothèse, chacune des suites $M' \otimes_A E_i \to M \otimes_A E_i \to M'' \otimes_A E_i$ est exacte, donc aussi la suite $M' \otimes_A E \to M \otimes_A E \to M'' \otimes_A E$, puisque le passage à la limite inductive commute avec le produit tensoriel (II, p. 93, prop. 7) et conserve l’exactitude (II, p. 91, prop. 3).

#### Exemple 1 {#alg-x-s1-n3-exa-1 .statement}

Il est clair que $A_s$ est un $A$-module plat; il résulte alors de la prop. 4 (i) que tout $A$-module libre, et plus généralement tout $A$-module projectif, est plat (voir aussi II, p. 63, cor. 6).

\* Inversement, tout $A$-module plat de présentation finie est projectif (no 5). \*

#### Exemple 2 {#alg-x-s1-n3-exa-2 .statement}

D’après la prop. 4 (ii), tout $A$-module qui est limite inductive d’un système inductif filtrant de $A$-modules libres est plat. Nous démontrerons une réciproque au no 6.

#### Exemple 3 {#alg-x-s1-n3-exa-3 .statement}

Si $A$ est semi-simple, tout $A$-module est projectif (VIII, § 5, no 1, prop. 1) donc plat.

#### Exemple 4 {#alg-x-s1-n3-exa-4 .statement}

\* Si $A$ est un anneau local artinien (non nécessairement commutatif), un $A$-module est plat si et seulement s’il est libre (AC II, § 3, no 2, cor. 2 de la prop. 5). \*

#### Exemple 5 {#alg-x-s1-n3-exa-5 .statement}

Si $A$ est intègre, le corps des fractions $K$ de $A$ est un $A$-module plat (II, p. 118, prop. 27).

#### Exemple 6 {#alg-x-s1-n3-exa-6 .statement}

\* En AC II et III, nous étudierons deux exemples importants de $A$-modules plats lorsque $A$ est commutatif : les anneaux de fractions $S^{-1} A$, et lorsque $A$ est nœthérien, les séparés complétés de $A$ pour les topologies J-adiques. \*

#### Exemple 7 {#alg-x-s1-n3-exa-7 .statement}

Soit $a \in A$ tel que l’application $a_A : x \mapsto ax$ de $A$ dans $A$ soit injective (« $a$ n’est pas diviseur à gauche de 0 »). Si $E$ est un $A$-module plat, alors l’homothétie $a_E$ est injective, puisque s’identifiant à $a_A \otimes 1 : A_d \otimes_A E \to A_d \otimes_A E$. En particulier, si $A$ est intègre, tout $A$-module plat est sans torsion. Inversement, si $A$ est principal, tout $A$-module sans torsion est plat : en effet, si le $A$-module $E$ est sans torsion, tout sous-module de type fini de $E$ est libre (VII, § 4, no 4, cor. 2 au th. 4), et $E$ est réunion filtrante croissante de sous-modules plats, donc est plat (prop. 4 (ii)).

#### Exemple 8 {#alg-x-s1-n3-exa-8 .statement}

Soient $B$ un anneau et $\rho : A \to B$ un homomorphisme. Si $E$ est un $A$-module plat, le $B$-module $E_{(B)} = B \otimes_A E$ est plat. Soit en effet $u : N' \to N$ un homomorphisme injectif de $B$-modules à droite ; alors $u \otimes_B 1_{E_{(B)}}$ s’identifie canoniquement à l’homomorphisme $u \otimes_A 1_E : N' \otimes_A E \to N \otimes_A E$, qui est injectif si $E$ est plat.

#### Exemple 9 {#alg-x-s1-n3-exa-9 .statement}

Supposons que $A = K[X, Y]$, où $K$ est un corps. Alors l’idéal maximal $m$ engendré par $X$ et $Y$ est un $A$-module sans torsion, mais non plat. Considérons en effet l’anneau $B = A/(Y)$, qui est isomorphe à $K[X]$, donc intègre. Le $B$-module $m_{(B)}$ est isomorphe à $m/Ym = (X, Y)/(XY, Y^2)$ dans lequel la classe de $Y$ est de torsion. Par suite, $m_{(B)}$ n’est pas un $B$-module plat, donc $m$ n’est pas plat.

#### Exemple 10 {#alg-x-s1-n3-exa-10 .statement}

Supposons $A$ commutatif. Soit $B$ l’algèbre $A[X_1, ..., X_n]/(P)$, où $P$ est un polynôme non nul. Pour tout idéal premier $p$ de $A$, notons $\kappa(p)$ le corps des fractions de l’anneau intègre $A/p$, $E(p)$ l’algèbre $\kappa(p)[X_1, ..., X_n]$ et $P(p)$ l’image de $P$ dans $E(p)$ par l’application canonique.

On peut montrer que, pour que $B$ soit un $A$-module plat, il suffit que $P(p) \neq 0$ pour tout idéal premier $p$ de $A$. Si $A$ est intègre, cette condition est nécessaire.

\* En langage géométrique, considérons la projection $\pi : \mathrm{Spec}(B) \to \mathrm{Spec}(A)$. Pour tout $p \in \mathrm{Spec}(A)$, la fibre $\pi^{-1}(p)$ s’identifie à la sous-variété $V_p$ de l’espace affine $\mathbf{A}_{\kappa(p)}^n = \mathrm{Spec}(E(p))$ définie par $P(p)$, et l’ensemble $F$ des $p$ pour lesquels cette sous-variété est l’espace tout entier (*i.e.* pour lesquels $P(p) = 0$) est un fermé de

Spec (A). La condition précédente signifie que ce fermé est vide, autrement dit que pour tout $p$ la sous-variété $V_p$ est une hypersurface dans $\mathbf{A}_{k(p)}^n$.

#### Exemple 11 {#alg-x-s1-n3-exa-11 .statement}

\* Soient S et X deux espaces analytiques complexes et $f : X \to S$ un morphisme. On dit que $f$ est plat en un point $x$ de X si $\mathcal{O}_{X,x}$, considéré comme $\mathcal{O}_{S,f(x)}$-module au moyen de l’homomorphisme $f^* : \mathcal{O}_{S,f(x)} \to \mathcal{O}_{X,x}$, est plat. L’ensemble des points de X où $f$ est plat est un ouvert de X, et la restriction de $f$ à cet ouvert est une application ouverte. Si X et S sont des variétés analytiques connexes de dimension finie, $f$ est plat (en tout point de X) si et seulement si $f(X)$ est ouvert dans S et les fibres $f^{-1}(s)$, pour $s \in f(X)$, ont toutes la même dimension. \*

### 4. Modules de présentation finie

On appelle présentation (ou présentation de longueur 1) d’un A-module E une suite exacte

$$
L_1 \to L_0 \to E \to 0
$$

de A-modules où $L_0$ et $L_1$ sont libres.

Tout A-module E admet une présentation. On sait en effet (II, p. 27, prop. 20) qu’il existe un homomorphisme surjectif $u : L_0 \to E$, où $L_0$ est libre ; si R est le noyau de $u$, il existe de même un homomorphisme surjectif $v : L_1 \to R$ où $L_1$ est libre. Si l’on considère $v$ comme un homomorphisme de $L_1$ dans $L_0$, la suite $L_1 \xrightarrow{v} L_0 \xrightarrow{u} E \to 0$ est exacte par définition, d’où notre assertion.

Si $\rho : A \to B$ est un homomorphisme d’anneaux, toute présentation (13) de E fournit une présentation de $E_{(B)} = B \otimes_A E$ :

$$
B \otimes_A L_1 \to B \otimes_A L_0 \to B \otimes_A E \to 0
$$

en vertu de II, p. 58, prop. 5 et du fait que $B \otimes_A L$ est un B-module libre lorsque L est libre.

On dit qu’une présentation (13) d’un module E est finie si les modules libres $L_0$ et $L_1$ ont des bases finies. Il est clair que si la présentation (13) est finie, il en est de même de la présentation (14). On dit que E est un A-module de présentation finie s’il admet une présentation finie.

#### Proposition 5 {#alg-x-s1-prop-5 .statement}

(i) Tout module admettant une présentation finie est de type fini.
(ii) Si A est un anneau noethérien à gauche, tout A-module de type fini admet une présentation finie.
(iii) Tout module projectif de type fini admet une présentation finie.

L’assertion (i) résulte trivialement des définitions. Supposons A noethérien à gauche et E de type fini. Il existe alors un homomorphisme surjectif $u : L_0 \to E$, où $L_0$ est un A-module libre ayant une base finie ; le noyau R de $u$ est de type fini, donc il y a un homomorphisme surjectif $v : L_1 \to R$ où $L_1$ est libre de base finie, et la suite exacte $L_1 \xrightarrow{v} L_0 \xrightarrow{u} E \to 0$ est une présentation finie de E ; d’où (ii).

Enfin, supposons que E soit un module projectif de type fini ; il est alors facteur direct d’un module libre de type fini L_0 (II, p. 40, cor. 1) ; le noyau R de l’homomorphisme surjectif L_0 → E est alors isomorphe à un quotient de L_0, donc est de type fini, et on termine comme ci-dessus.

#### Proposition 6 {#alg-x-s1-prop-6 .statement}

Soient A un anneau, E un A-module de présentation finie. Pour toute suite exacte

$$
0 \to F \xrightarrow{j} G \xrightarrow{p} E \to 0
$$

où G est de type fini, le module F est de type fini.

Soit L_1 \xrightarrow{r} L_0 \xrightarrow{s} E \to 0 une présentation finie ; si (e_i) est une base de L_0, il existe pour chaque i un élément g_i \in G tel que p(g_i) = s(e_i) ; l’homomorphisme u : L_0 \to G tel que u(e_i) = g_i pour tout i est donc tel que s = p \circ u. Comme s \circ r = 0, on a u(r(L_1)) \subset \mathrm{Ker}\ p, et comme Ker p est isomorphe à F, on voit qu’il y a un homomorphisme v : L_1 \to F tel que le diagramme

$$
\begin{array}{ccccccc}
L_1 & \xrightarrow{r} & L_0 & \xrightarrow{s} & E & \to & 0 \\
v \downarrow & & u \downarrow & & 1_E \downarrow & & \\
F & \xrightarrow{j} & G & \xrightarrow{p} & E & \to & 0
\end{array}
$$

soit commutatif. Comme j est injectif et s surjectif, on peut appliquer la proposition 2 de X, p. 4, autrement dit il y a une suite exacte

$$
\mathrm{Ker}\ 1_E \xrightarrow{d} \mathrm{Coker}\ v \to \mathrm{Coker}\ u \to \mathrm{Coker}\ 1_E.
$$

Ceci montre que Coker v est isomorphe à G/u(L_0), qui est de type fini par hypothèse. On a en outre la suite exacte

$$
0 \to v(L_1) \to F \to \mathrm{Coker}\ v \to 0
$$

et comme v(L_1) et Coker v sont de type fini, il en est de même de F (II, p. 17, cor. 5).

#### Proposition 7 {#alg-x-s1-prop-7 .statement}

Soit M un A-module. Il existe un ensemble ordonné I filtrant à droite et un système inductif de A-modules de présentation finie (M_\alpha, \varphi_{\beta\alpha}) relatif à I tel que M soit isomorphe à \lim_\alpha M_\alpha. Si M possède un système générateur de n éléments, on peut supposer qu’il en est de même des M_\alpha.

Considérons une présentation

$$
A_s^{(K)} \xrightarrow{u} A_s^{(L)} \xrightarrow{v} M \to 0 ;
$$

soit I l’ensemble des couples \alpha = (K', L'), où K' (resp. L') est une partie finie de K (resp.L), tels que u induise une application u_\alpha du sous-module A_s^{K'} de A_s^{(K)} dans le sous-module A_s^{L'} de A_s^{(L)} ; pour \alpha \in I, soit M_\alpha le conoyau de u_\alpha et v_\alpha : A_s^{L'} \to M_\alpha l’application canonique, de sorte que l’on a un diagramme commutatif à lignes exactes :

$$
\begin{array}{ccccccc}
A_s^{(K)} & \xrightarrow{u} & A_s^{(L)} & \xrightarrow{l} & M & \to & 0 \\
i_\alpha \uparrow & & j_\alpha \uparrow & & f_\alpha \uparrow \\
A_s^{K'} & \xrightarrow{u_\alpha} & A_s^{L'} & \xrightarrow{v_\alpha} & M_\alpha & \to & 0 ,
\end{array}
$$

où $i_\alpha$ et $j_\alpha$ sont les injections canoniques, et où $f_\alpha$ est déduit de $j_\alpha$ par passage aux quotients. Ordonnons l’ensemble I par la relation

$$
\alpha = (K',L') \leq \beta = (K'',L'') \quad \text{si}\quad K' \subset K'',\quad L' \subset L'' ;
$$

pour $\alpha\leq\beta$, soit $\varphi_{\beta\alpha}:M_\alpha\longrightarrow M_\beta$ l’homomorphisme déduit par passage aux quotients de l’inclusion de $A_s^{L'}$ dans $A_s^{L''}$. On vérifie alors aussitôt que l’ensemble ordonné I est filtrant, que $(M_\alpha,\varphi_{\beta\alpha})$ est un système inductif de A-modules et que $(\varphi_\alpha)$ est un système inductif de A-homomorphismes. Par passage à la limite inductive, on obtient un diagramme commutatif

$$
\begin{array}{ccccc}
A_s^{(K)} & \xrightarrow{u} & A_s^{(L)} & \xrightarrow{v} & M \longrightarrow 0\\
\uparrow\scriptstyle i && \uparrow\scriptstyle j && \uparrow\scriptstyle\varphi\\
\underset{\longrightarrow}{\lim}\,A_s^{K'} & \longrightarrow & \underset{\longrightarrow}{\lim}\,A_s^{L'} & \longrightarrow & \underset{\longrightarrow}{\lim}\,M_\alpha \longrightarrow 0
\end{array}
\tag{15}
$$

les lignes de ce diagramme sont exactes (II, p. 91, prop. 3) ; puisque $i$ et $j$ sont bijectifs, $\varphi$ l’est aussi (X, p. 7, cor. 3), d’où la proposition.

### 5. Homomorphismes d’un module de présentation finie

Soit E un A-module. Si I est un ensemble préordonné filtrant et $(G_i,u_{ji})$ un système inductif de A-modules relatif à I, les applications canoniques $G_i\longrightarrow\underset{\longrightarrow}{\lim}\,G_i$ induisent des homomorphismes $\operatorname{Hom}_A(E,G_i)\longrightarrow\operatorname{Hom}_A(E,\underset{\longrightarrow}{\lim}\,G_i)$, d’où un homomorphisme dit *canonique*

$$
\underset{\substack{\longrightarrow\\ i\in I}}{\lim}\operatorname{Hom}_A(E,G_i)
\longrightarrow
\operatorname{Hom}_A\left(E,\underset{\substack{\longrightarrow\\ i\in I}}{\lim}G_i\right).
\tag{16}
$$

Soient B un autre anneau, F un B-module, G un (A, B)-bimodule ; on a défini en II, p. 75 un homomorphisme canonique :

$$
\operatorname{Hom}_A(E,G)\otimes_B F
\longrightarrow
\operatorname{Hom}_A(E,G\otimes_B F).
\tag{17}
$$

#### Proposition 8 {#alg-x-s1-prop-8 .statement}

a) *Si le A-module E est de type fini (resp. de présentation finie), l’homomorphisme canonique (16) est injectif (resp. bijectif).*

*b) Supposons que le B-module F soit plat ; si le A-module E est de type fini (resp. de présentation finie), l’homomorphisme canonique (17) est injectif (resp. bijectif).*

Démontrons par exemple b), la démonstration de a) étant analogue. Considérons A, B, F, G comme fixés, et, pour tout A-module à droite E, posons

$$
T(E)=\operatorname{Hom}_A(E,G)\otimes_B F,\qquad
T'(E)=\operatorname{Hom}_A(E,G\otimes_B F)
$$

et notons $\nu_E$ l’homomorphisme (17) ; pour tout homomorphisme $v:E\to E'$ de A-modules à droite, posons $T(v)=\operatorname{Hom}(v,1_G)\otimes 1_F$ et $T'(v)=\operatorname{Hom}(v,1_G\otimes 1_F)$.

Soit $L_1 \xrightarrow{v} L_0 \xrightarrow{w} E \to 0$ une présentation de $E$; nous supposons le module libre $L_0$ (resp. les modules libres $L_0$ et $L_1$) *de type fini*. Le diagramme

$$
\begin{array}{ccccccc}
0 & \to & T(E) & \xrightarrow{T(w)} & T(L_0) & \xrightarrow{T(v)} & T(L_1) \\
& & v_E \downarrow & & v_{L_0} \downarrow & & v_{L_1} \downarrow \\
0 & \to & T'(E) & \xrightarrow{T'(w)} & T'(L_0) & \xrightarrow{T'(v)} & T'(L_1)
\end{array}
$$

est commutatif, et sa seconde ligne est exacte (II, p. 36, th. 1); en outre, la suite

$$
0 \to \mathrm{Hom}_A(E, G) \to \mathrm{Hom}_A(L_0, G) \to \mathrm{Hom}_A(L_1, G)
$$

est exacte (*loc. cit.*), et comme $F$ est *plat*, la première ligne de (18) est aussi une suite exacte (X, p. 8, déf. 1). Cela étant, on sait que $v_{L_0}$ est bijectif (resp. que $v_{L_0}$ et $v_{L_1}$ sont bijectifs) (II, p. 75, prop. 2). Si on suppose seulement $v_{L_0}$ bijectif, il résulte de (18) que $v_{L_0} \circ T(w) = T'(w) \circ v_E$ est injectif, donc $v_E$ l’est aussi. Si on suppose que $v_{L_0}$ et $v_{L_1}$ sont tous deux bijectifs, on déduit du cor. 2 (ii) de X, p. 6 que $v_E$ est surjectif, et comme on vient de voir que $v_E$ est injectif, il est bijectif.

**COROLLAIRE. — Tout module plat et de présentation finie est projectif.**

Soit en effet $E$ un $A$-module plat et de présentation finie. Appliquant (*b*) au cas $B = A, G = {}_sA_d, F = E$, on voit que l’homomorphisme canonique

$$
\mathrm{Hom}_A(E, A) \otimes_A E \to \mathrm{Hom}_A(E, E)
$$

est surjectif. Cela implique que $E$ est projectif (II, p. 77, remarque 1).

D’après le corollaire précédent et la prop. 5 de X, p. 10, il y a identité entre modules plats de présentation finie et modules projectifs de type fini. En revanche, il existe des modules plats de type fini qui ne sont pas de présentation finie, donc qui ne sont pas projectifs (*cf.* X, p. 170, exercice 17, voir toutefois X, p. 169, exercices 13 et 14).

### 6. Structure des modules plats

**Lemme 2. — Soient I un ensemble ordonné filtrant à droite, $(E_\alpha, \varphi_{\beta\alpha})$ un système inductif d’ensembles relatif à I, E sa limite inductive et $\varphi_\alpha : E_\alpha \to E, \alpha \in I$, les applications canoniques. Soit $f : I \to I$ une application telle que $f(\alpha) > \alpha$ pour $\alpha \in I$, et supposons donnés, pour chaque $\alpha \in I$, un ensemble $L_\alpha$ et des applications $u_\alpha : E_\alpha \to L_\alpha$ et $v_\alpha : L_\alpha \to E_{f(\alpha)}$ telles que $v_\alpha \circ u'_\alpha = \varphi_{f(\alpha), \alpha}$. Soit J l’ensemble ordonné obtenu en munissant I de la relation « $\alpha \leq \beta$ si $\alpha = \beta$ ou $f(\alpha) \leq \beta$ ». Si $\alpha, \beta \in J$ avec $\alpha \leq \beta$, soit $\psi_{\beta\alpha} : L_\alpha \to L_\beta$ l’application telle que $\psi_{\beta\alpha} = \mathrm{Id}$ si $\alpha = \beta$, $\psi_{\beta\alpha} = u_\beta \circ \varphi_{\beta, f(\alpha)} \circ v_\alpha$ si $f(\alpha) \leq \beta$. Si $\alpha \in J$, soit $\psi_\alpha : L_\alpha \to E$ l’application $\varphi_{f(\alpha)} \circ v_\alpha$. Alors l’ensemble ordonné J est filtrant, $(L_\alpha, \psi_{\beta\alpha})$ est un système inductif relatif à J, $(\psi_\alpha)$ est un système inductif d’applications et l’application $\psi : \lim_{\alpha \in J} L_\alpha \to E$ déduite des $\psi_\alpha$ est bijective.

Il est clair que J est filtrant. Si $\alpha, \beta \in J$ avec $\alpha < \beta$, on a
$$
\psi_\beta \circ \psi_{\beta \alpha} = \varphi_{f(\beta)} \circ v_\beta \circ u_\beta \circ \varphi_{\beta, f(\alpha)} \circ v_\alpha \\
= \varphi_{f(\beta)} \circ \varphi_{f(\beta), \beta} \circ \varphi_{\beta, f(\alpha)} \circ v_\alpha = \varphi_{f(\alpha)} \circ v_\alpha = \psi_\alpha ;
$$
de même, si $\alpha, \beta, \gamma \in J$ avec $\alpha < \beta < \gamma$, on a
$$
\psi_{\gamma \beta} \circ \psi_{\beta \alpha} = u_\gamma \circ \varphi_{\gamma, f(\beta)} \circ v_\beta \circ u_\beta \circ \varphi_{\beta, f(\alpha)} \circ v_\alpha \\
= u_\gamma \circ \varphi_{\gamma, f(\beta)} \circ \varphi_{f(\beta), \beta} \circ \varphi_{\beta, f(\alpha)} \circ v_\alpha = u_\gamma \circ \varphi_{\gamma, f(\alpha)} \circ v_\alpha = \psi_{\gamma \alpha} .
$$
Démontrons la dernière assertion : pour chaque $\alpha \in J$, on a
$$
\psi_\alpha \circ u_\alpha = \varphi_{f(\alpha)} \circ v_\alpha \circ u_\alpha = \varphi_{f(\alpha)} \circ \varphi_{f(\alpha), \alpha} = \varphi_\alpha ,
$$
donc $\varphi_\alpha(E_\alpha) = \psi_\alpha(u_\alpha(E_\alpha)) \subset \psi_\alpha(L_\alpha)$, et $\psi$ est surjective. Soit $\alpha \in J$ et soient $x, y \in L_\alpha$ avec $\psi_\alpha(x) = \psi_\alpha(y)$, i.e. $\varphi_{f(\alpha)}(v_\alpha(x)) = \varphi_{f(\alpha)}(v_\alpha(y))$; il existe $\beta \in I$, $\beta \geq f(\alpha)$ tel que
$$
\varphi_{\beta, f(\alpha)}(v_\alpha(x)) = \varphi_{\beta, f(\alpha)}(v_\alpha(y)) ,
$$
donc
$$
\psi_{\beta, \alpha}(x) = u_\beta(\varphi_{\beta, f(\alpha)}(v_\alpha(x))) = u_\beta(\varphi_{\beta, f(\alpha)}(v_\alpha(y))) = \psi_{\beta, \alpha}(y) .
$$
et $\psi$ est injective.

#### Théorème 1 (D. Lazard) {#alg-x-s1-thm-1 .statement}

Pour tout A-module E, les conditions suivantes sont équivalentes :
(i) E est plat.
(ii) Pour tout A-module P de présentation finie, l’homomorphisme canonique
$$
\operatorname{Hom}_A(P, A) \otimes_A E \to \operatorname{Hom}_A(P, E)
$$
est surjectif.
(iii) Pour tout A-module P de présentation finie et tout homomorphisme $u : P \to E$, il existe un A-module L libre de type fini et des homomorphismes $v : P \to L$ et $w : L \to E$ tels que $u = w \circ v$.
(iv) Il existe un ensemble ordonné filtrant J, un système inductif de modules libres de type fini $(L_j)_{j \in J}$ et un isomorphisme de E sur $\lim \overrightarrow{L_j}$.
(iv) $\Rightarrow$ (i) : cela résulte de la prop. 4 (ii) de X, p. 8.
(i) $\Rightarrow$ (ii) : cela résulte de la prop. 8b) de X, p. 12.
(ii) $\Rightarrow$ (iii) : soient P un A-module de présentation finie et $u : P \to E$ un homomorphisme ; d’après (ii), il existe $v_1, \ldots, v_n \in \operatorname{Hom}_A(P, A)$, $w_1, \ldots, w_n \in E$ tels que $u(x) = \sum v_i(x) w_i$ pour tout $x \in P$ ; si $v : P \to A^n$ est l’homomorphisme de composantes $(v_i)$ et $w : A^n \to E$ l’homomorphisme $(a_i) \mapsto \sum a_i w_i$, on a bien $u = w \circ v$.
(iii) $\Rightarrow$ (iv) : supposons (iii) vérifiée, et soit $(E_\alpha, \varphi_{\beta, \alpha})$ un système inductif, relatif à un ensemble filtrant I, de A-modules de présentation finie, de limite inductive E

(X, p. 11, prop. 7). Quitte à remplacer I par le produit lexicographique I × N, avec E_{(α,n)} = E_α pour tout n, on peut supposer que I n’a pas de plus grand élément. Pour chaque α ∈ I, soient L_α un A-module libre de type fini et u_α : E_α → L_α, v'_α : L_α → E des homomorphismes tels que v'_α ∘ u_α soit l’application canonique φ_α de E_α dans E ; puisque L_α est libre de type fini et I sans plus grand élément, il existe un indice β > α et un homomorphisme v''_α : L_α → E_β tels que v'_α = φ_β ∘ v''_α ; puisque φ_β ∘ v''_α ∘ u_α = φ_β ∘ φ_β,α et que E_α est de présentation finie, il résulte de la prop. 8a) de X, p. 12, qu’il existe γ ≥ β tel que φ_{γβ} ∘ v''_α ∘ u_α = φ_{γβ} ∘ φ_{βα} = φ_{γα} ; posons γ = f(α) et soit v_α l’homomorphisme φ_{γβ} ∘ v''_α de L_α dans E_{f(α)} ; on a v_α ∘ u_α = φ_{f(α),α}. On peut alors appliquer le lemme 2, d’où (iv).

#### Corollaire {#alg-x-s1-n6-cor-1 .statement}

Supposons A commutatif. Pour tout A-module plat E, les A-modules T(E), S(E), Λ(E), T^n(E), S^n(E), Λ^n(E) sont plats.

En effet, E est la limite inductive d’un système filtrant (L_j) de A-modules libres de type fini, donc T(E) (resp. S(E), etc.) est limite inductive du système filtrant des A-modules libres T(L_j) (resp. S(L_j), etc.), donc est plat (cf. III, p. 61, prop. 6, p. 62, th. 1, p. 73, prop. 8, p. 75, th. 1, p. 83, prop. 9, et p. 86, th. 1).

#### Remarque {#alg-x-s1-n6-rem-1 .statement}

Considérant dans (ii) une présentation finie A_s^J \xrightarrow{c} A_s^I \to P \to 0, on obtient la condition (ii’) encore équivalente aux précédentes :

(ii’) Pour toute matrice finie (c_{ij})_{i \in I, j \in J} d’éléments de A, toute solution

$$
e = (e_i)_{i \in I} \in E^I
$$

du système d’équations linéaires et homogènes

$$
\sum_{i \in I} c_{ij} e_i = 0,\quad j \in J,
$$

peut s’écrire b_1 z_1 + \cdots + b_n z_n, où b_1, ..., b_n \in E et où, pour r = 1, ..., n, z_r = (z_{r,i})_{i \in I} est une solution dans A^I du système d’équations

$$
\sum_{i \in I} z_{r,i} c_{ij} = 0,\quad j \in J.
$$

### 7. Modules injectifs

#### Définition 2 {#alg-x-s1-def-2 .statement}

On dit que le A-module E est injectif si, pour toute suite exacte de A-modules et d’homomorphismes

(19)
$$
M' \xrightarrow{u} M \xrightarrow{v} M'',
$$
la suite d’applications $\mathbf{Z}$-linéaires

(20)
$$
\operatorname{Hom}_A(M'', E) \xrightarrow{\operatorname{Hom}_A(v, 1)} \operatorname{Hom}_A(M, E) \xrightarrow{\operatorname{Hom}_A(u, 1)} \operatorname{Hom}_A(M', E)
$$
est exacte.

#### Lemme 3 {#alg-x-s1-lem-3 .statement}

*Pour que le A-module E soit injectif, il faut et il suffit que, pour toute application A-linéaire injective $u : M' \to M$, l’application*

$$
\operatorname{Hom}_A(u,1) : \operatorname{Hom}_A(M,E) \to \operatorname{Hom}_A(M',E)
$$

*soit surjective.*

Si $E$ est injectif et si $u : M' \to M$ est injectif, alors la suite $0 \to M' \xrightarrow{u} M$ est exacte, donc aussi la suite $\operatorname{Hom}(M,E) \xrightarrow{\operatorname{Hom}(u,1)} \operatorname{Hom}(M',E) \to 0$, et $\operatorname{Hom}(u,1)$ est surjectif. Inversement considérons la suite exacte (19) ; posons $M''_1=\nu(M)$ et soient $i : M''_1 \to M''$ l’injection canonique et $p : M \to M''_1$ l’application $m\mapsto \nu(m)$. La suite $M' \xrightarrow{u} M \xrightarrow{p} M''_1 \to 0$ est exacte ; d’après II, p. 36, th. 1, la suite

$$
\operatorname{Hom}_A(M''_1,E)
\xrightarrow{\operatorname{Hom}(p,1)}
\operatorname{Hom}_A(M,E)
\xrightarrow{\operatorname{Hom}(u,1)}
\operatorname{Hom}_A(M',E)
$$

est exacte. Par ailleurs, on a $\operatorname{Hom}(\nu,1)=\operatorname{Hom}(p,1)\circ\operatorname{Hom}(i,1)$. Si $E$ satisfait à la condition du lemme, $\operatorname{Hom}(i,1)$ est surjectif, donc l’image de $\operatorname{Hom}(\nu,1)$ est aussi celle de $\operatorname{Hom}(p,1)$, et la suite (20) est exacte.

#### Remarque {#alg-x-s1-n7-rem-1 .statement}

Soient $E$ un A-module injectif, $u : M' \to M$ et $f : M' \to E$ des homomorphismes de A-modules. Si $\operatorname{Ker}u\subset\operatorname{Ker}f$, il existe un homomorphisme $g : M \to E$ tel que $g\circ u=f$. Cela résulte en effet de ce qui précède appliqué à l’homomorphisme injectif $M'/\operatorname{Ker}u \to M$ déduit de $u$.

#### Proposition 9 {#alg-x-s1-prop-9 .statement}

*Soient $(E_i)_{i\in I}$ une famille de A-modules, $E=\prod_{i\in I}E_i$ leur produit. Pour que le A-module $E$ soit injectif, il faut et il suffit que chacun des $E_i$ le soit.*

Soit $u : M' \to M$ un homomorphisme injectif de A-modules. Pour que l’homomorphisme produit

$$
\prod_{i\in I}\operatorname{Hom}_A(M,E_i)
\longrightarrow
\prod_{i\in I}\operatorname{Hom}_A(M',E_i)
$$

soit surjectif, il faut et il suffit que chacun des homomorphismes $\operatorname{Hom}_A(M,E_i)\to\operatorname{Hom}_A(M',E_i)$ le soit (II, p. 10, prop. 5) ; cela démontre la proposition puisque $\prod_{i\in I}\operatorname{Hom}_A(M,E_i)$ s’identifie canoniquement à $\operatorname{Hom}_A(M,E)$.

#### Proposition 10 {#alg-x-s1-prop-10 .statement}

*Soit $E$ un A-module. Pour que $E$ soit injectif, il faut et il suffit que, pour tout idéal $a$ de $A$ et tout A-homomorphisme $f : a\to E$, il existe $e\in E$ tel que*

$$
f(a)=ae
$$

*pour tout $a\in a$.*

Supposons $E$ injectif ; soient $a$ un idéal de $A$, $f : a\to E$ un A-homomorphisme, et notons $i : a\to A$ l’injection canonique. Alors l’application

$$
\operatorname{Hom}_A(i,1) : \operatorname{Hom}_A(A,E)\to\operatorname{Hom}_A(a,E)
$$

est surjective (déf. 2) ; si $g\in\operatorname{Hom}_A(A,E)$ est tel que $f=g\circ i$, on a

$$
f(a)=g(a)=ag(1)
$$

pour tout $a\in a$.

Inversement, supposons la condition de l’énoncé vérifiée, soient $M$ un A-module, $N$ un sous-module de $M$, $u : N\to E$ un A-homomorphisme, et prouvons qu’il existe un A-homomorphisme $\bar u : M\to E$ prolongeant $u$ (cf. *lemme* 3). Soit $\mathcal P$ l’ensemble des couples $(P,v)$ où $P$ est un sous-module de $M$ contenant $N$ et $v$ un homomorphisme de $P$ dans $E$ prolongeant $u$. L’ensemble $\mathcal P$ ordonné par la relation de prolongement est *inductif* : si $(P_j, v_j)$ est une famille totalement ordonnée d’éléments de $\mathcal{P}$, posons $Q = \cup P_j$ et soit $w : Q \to E$ l’unique application induisant $v_j$ sur $P_j$ pour tout $j$; alors $(Q, w) \in \mathcal{P}$ et $(Q, w)$ majore $(P_j, v_j)$ pour tout $j$. Soit alors $(P, v)$ un élément maximal de $\mathcal{P}$ (E, III, p. 20, th. 2); il suffit de prouver que $P = M$. Soit $x \in M$ et soit $\alpha$ l’idéal des $a \in A$ tels que $ax \in P$; posons $f(a) = v(ax)$ pour $a \in \alpha$; on obtient ainsi un $A$-homomorphisme $f : \alpha \to E$. Soit alors $e$ un élément de $E$ tel que $f(a) = ae$ pour tout $a \in \alpha$. Posons $P' = P + Ax$ et soit $v' : P' \to E$ l’unique $A$-homomorphisme tel que $v'(p + ax) = v(p) + ae$ pour $p \in P, a \in A$; alors $(P', v')$ appartient à $\mathcal{P}$ et majore $(P, v)$, donc $P' = P$, c’est-à-dire $x \in P$, ce qui achève la démonstration.

#### Corollaire 1 {#alg-x-s1-prop-10-cor-1 .statement}

*Si l’anneau $A$ est nœthérien à gauche, tout module somme directe de $A$-modules injectifs est injectif.*

Soit $(E_i)_{i \in I}$ une famille de $A$-modules injectifs, soient $E$ leur somme directe, $\alpha$ un idéal de $A$ et $u : \alpha \to E$ un $A$-homomorphisme. Comme $A$ est nœthérien, $\alpha$ est de type fini, et par suite l’application canonique

$$
\varphi : \bigoplus_{i \in I} \operatorname{Hom}_A(\alpha, E_i) \to \operatorname{Hom}_A(\alpha, E)
$$

est bijective ; soit $(u_i)$ l’image réciproque de $u$ par $\varphi$. Puisque chaque $E_i$ est injectif, et la famille $(u_i)$ à support fini, il existe un élément $(e_i)_{i \in I}$ de $E$ tel que $u_i(a) = ae_i$ pour tout $a \in \alpha$ et tout $i \in I$, donc $u(a) = a((e_i))$ pour tout $a \in \alpha$, et $E$ est injectif.

#### Remarque {#alg-x-s1-n7-rem-2 .statement}

Si tout $A$-module somme directe de $A$-modules injectifs est injectif, l’anneau $A$ est nœthérien à gauche (X, p. 170, exercice 21).

Supposons $A$ intègre. On dit que le $A$-module $E$ est *divisible* si l’homothétie $a_E$ est surjective pour tout élément non nul $a$ de $A$.

#### Corollaire 2 {#alg-x-s1-prop-10-cor-2 .statement}

*Supposons $A$ intègre.*
  *a)* *Tout $A$-module injectif est divisible.*
  *b)* *Tout $A$-module sans torsion (II, p. 115) et divisible est injectif.*
  *c)* *Si $A$ est principal, tout $A$-module divisible est injectif.*

Si $a \in A$ est non nul, alors $a_A$ est injectif ; d’autre part, pour tout $A$-module $E$, l’homothétie $a_E$ s’identifie canoniquement à

$$
\operatorname{Hom}(a_A, 1) : \operatorname{Hom}_A(A, E) \to \operatorname{Hom}_A(A, E),
$$

donc $E$ est divisible si et seulement si $\operatorname{Hom}(a_E, 1_E)$ est surjectif pour tout $a \in A$ non nul. L’assertion *a)* résulte donc de la définition 2 (X, p. 15).

Soit $E$ un $A$-module divisible ; supposons $A$ principal (resp. $E$ sans torsion) et prouvons que $E$ est injectif par application de la prop. 10. Soient $\alpha$ un idéal de $A$ et $f : \alpha \to E$ un $A$-homomorphisme. Soit $x \in \alpha$ tel que $\alpha = Ax$ (resp. tel que $x \neq 0$ si $\alpha \neq 0$), et soit $e \in E$ tel que $xe = f(x)$. Prouvons que pour tout $a \in \alpha$, on a

$$
f(a) = ae;
$$

cela est clair si $a \in Ax$, d’où l’assertion dans le cas où A est principal ; si E est sans torsion et si $xa \in a$, on a $xf(a) = f(ax) = axe$, donc $f(a) = ae$ puisque $x$ est non nul si $a \neq 0$.

#### Exemple 1 {#alg-x-s1-n7-exa-1 .statement}

Si A est intègre, le corps des fractions K de A est un A-module injectif. Si A est principal, $K/A$ est un A-module injectif.
2) Par exemple, les $\mathbf{Z}$-modules $\mathbf{Q}$ et $\mathbf{Q}/\mathbf{Z}$ sont injectifs.
3) Soit A un anneau principal et soit $a$ un élément *non nul* de A. Alors $A/aA$ est un $A/aA$-module injectif (X, p. 170, exercice 20).

### 8. Modules cogénérateurs injectifs

#### Proposition 11 {#alg-x-s1-prop-11 .statement}

*Soient B un anneau, F un B-module et P un (B, A)-bimodule. Si F est un B-module injectif et P un A-module plat, $\mathrm{Hom}_B(P, F)$ est un A-module injectif.*

Soit $u : M' \to M$ un homomorphisme injectif de A-modules. On a un diagramme commutatif

$$
\begin{array}{ccc}
\mathrm{Hom}_A(M, \mathrm{Hom}_B(P, F)) & \xrightarrow{\mathrm{Hom}_A(u, 1)} & \mathrm{Hom}_A(M', \mathrm{Hom}_B(P, F)) \\
\beta \downarrow & & \beta' \downarrow \\
\mathrm{Hom}_B(P \otimes_A M, F) & \xrightarrow{\mathrm{Hom}(1_P \otimes u, 1_F)} & \mathrm{Hom}_B(P \otimes_A M', F)
\end{array}
$$

où $\beta$ et $\beta'$ sont les isomorphismes canoniques de II, p. 74. Comme P est plat sur A, l’homomorphisme $1_P \otimes u : P \otimes_A M' \to P \otimes_A M$ est injectif. Comme F est injectif, $\mathrm{Hom}(1_P \otimes u, 1_F)$ est surjectif, donc aussi $\mathrm{Hom}_A(u, 1)$, ce qui prouve que $\mathrm{Hom}_F(P, F)$ est un A-module injectif (X, p. 16, lemme 3).

#### Définition 3 {#alg-x-s1-def-3 .statement}

*On dit que le A-module E est cogénérateur si, pour tout A-module M et tout élément non nul x de M, il existe un A-homomorphisme $u : M \to E$ tel que $u(x) \neq 0$.*

On dit que le A-module L est *générateur* si, pour tout A-module M et tout élément x de M, il existe un A-homomorphisme $u : L \to M$ tel que $x \in u(L)$. Par exemple, le A-module $A_s$ est générateur.

#### Proposition 12 {#alg-x-s1-prop-12 .statement}

*Soit E un A-module injectif. Pour que E soit cogénérateur, il faut et il suffit que $\mathrm{Hom}_A(S, E) \neq 0$ pour tout A-module simple S.*

La condition est évidemment nécessaire. Inversement, soient M un A-module et x un élément non nul de M ; le sous-module $Ax$ de M possède un quotient simple S (VIII, § 2, no 1, prop. 3). Si $\mathrm{Hom}_A(S, E) \neq 0$, alors $\mathrm{Hom}_A(Ax, E) \neq 0$ et il existe un homomorphisme $f : Ax \to E$ tel que $f(x) \neq 0$; comme E est injectif, $f$ se prolonge en un homomorphisme $u$ de M dans E et on a $u(x) = f(x) \neq 0$.

#### Exemple {#alg-x-s1-n8-exa-1 .statement}

Le $\mathbf{Z}$-module injectif $\mathbf{Q}/\mathbf{Z}$ (X, p. 18, exemple 2) est cogénérateur.
En effet, tout $\mathbf{Z}$-module simple est isomorphe à un module $\mathbf{Z}/p\mathbf{Z}$, $p\ne 0$, et $\operatorname{Hom}_{\mathbf{Z}}(\mathbf{Z}/p\mathbf{Z},\mathbf{Q}/\mathbf{Z})$ est non nul (il contient par exemple l’élément de $\mathbf{Z}/p\mathbf{Z}$ déduit par passage aux quotients de l’homomorphisme $x\mapsto x/p$ de $\mathbf{Z}$ dans $\mathbf{Q}$).

#### Proposition 13 {#alg-x-s1-prop-13 .statement}

Soient $B$ un anneau, $F$ un $B$-module injectif cogénérateur, $P$ un $(B,A)$-bimodule. Supposons $P$ plat sur $A$ et tel que $P\otimes_A S\ne 0$ pour tout $A$-module simple $S$ (* c’est-à-dire fidèlement plat sur $A$ au sens de AC, I, §). Alors le $A$-module $\operatorname{Hom}_B(P,F)$ est cogénérateur et injectif.

En effet, $\operatorname{Hom}_B(P,F)$ est injectif d’après la prop. 11. D’autre part, pour tout $A$-module simple $S$, $\operatorname{Hom}_A(S,\operatorname{Hom}_B(P,F))$ est isomorphe à $\operatorname{Hom}_B(P\otimes_A S,F)$, donc est non nul puisque $P\otimes_A S\ne 0$ et que le $B$-module $F$ est cogénérateur ; le $A$-module $\operatorname{Hom}_B(P,F)$ est donc cogénérateur d’après la prop. 12.

#### Corollaire 1 {#alg-x-s1-prop-13-cor-1 .statement}

Le $A$-module $E_A=\operatorname{Hom}_{\mathbf{Z}}(A,\mathbf{Q}/\mathbf{Z})$ est injectif et cogénérateur.

On applique la prop. 13 avec $B=\mathbf{Z}$, $F=\mathbf{Q}/\mathbf{Z}$ (exemple) et $P=A_d$.

Pour tout $A$-module $M$, posons

$$
I^0(M)=E_A^{\operatorname{Hom}(M,E_A)}
$$

et soit $e_M:M\to I^0(M)$ l’homomorphisme qui associe à $m\in M$ l’élément

$$
(\varphi(m))_{\varphi\in\operatorname{Hom}(M,E_A)}\in I^0(M).
$$

Alors :

#### Corollaire 2 {#alg-x-s1-prop-13-cor-2 .statement}

Le $A$-module $I^0(M)$ est injectif et le $A$-homomorphisme $e_M:M\to I^0(M)$ est injectif.

En effet, $I^0(M)$ est injectif, puisque $E_A$ est injectif (X, p. 16, prop. 9), d’autre part $e_M$ est injectif puisque $E_A$ est cogénérateur.

#### Corollaire 3 {#alg-x-s1-prop-13-cor-3 .statement}

Tout $A$-module est isomorphe à un sous-module d’un $A$-module injectif.

#### Corollaire 4 {#alg-x-s1-prop-13-cor-4 .statement}

Pour que le $A$-module $E$ soit injectif, il faut et il suffit que tout $A$-homomorphisme injectif $f:E\to F$ possède une rétraction $A$-linéaire.

Supposons $E$ injectif et soit $f:E\to F$ un $A$-homomorphisme injectif. Alors

$$
\operatorname{Hom}_A(f,1_E):\operatorname{Hom}_A(F,E)\to\operatorname{Hom}_A(E,E)
$$

est surjectif ; il existe donc $r\in\operatorname{Hom}_A(F,E)$ tel que $r\circ f=1_E$ et $r$ est une rétraction $A$-linéaire de $f$. Inversement, il existe un $A$-module injectif $I$ et un $A$-homomorphisme injectif $f:E\to I$ (cor. 2) ; si $f$ possède une rétraction $A$-linéaire, $E$ est injectif d’après la prop. 9 de X, p. 16.

### 9. Enveloppes injectives

#### Définition 4 {#alg-x-s1-def-4 .statement}

Soit $M$ un $A$-module. Une enveloppe injective de $M$ est un couple $(I,i)$, où $I$ est un $A$-module injectif et $i:M\to I$ un homomorphisme possédant la propriété suivante :

(E) pour qu’un sous-module P de I soit nul, il faut et il suffit que i^{-1}(P) soit nul.

Notons que (E) implique que i est injectif. On identifie souvent M au sous-module i(M) de I, et on dit alors que I est une enveloppe injective de M.

Exemple 1. Supposons A intègre et M sans torsion. Soient K le corps des fractions de A et i : M → K ⊗_A M l’homomorphisme canonique. Alors (K ⊗_A M, i) est une enveloppe injective de M (II, p. 116, prop. 26 et X, p. 17, cor. 2).

#### Théorème 2 {#alg-x-s1-thm-2 .statement}

Soit M un A-module.
a) M possède des enveloppes injectives.
b) Si (I, i) et (J, j) sont deux enveloppes injectives de M, il existe un isomorphisme f : I → J tel que f ∘ i = j.

On notera que l’homomorphisme f dont l’existence est affirmée dans b) n’est pas uniquement déterminé en général.

a) On peut supposer que M est un sous-module d’un A-module injectif E (X, p. 19, cor. 3). Considérons l’ensemble ordonné par inclusion F des sous-modules I de E, contenant M, et tels que l’injection canonique i : M → I satisfasse à la propriété (E). Puisque F est inductif, il possède un élément maximal (E, III, p. 20); soit I un élément maximal de F. Il suffit de prouver que I est un sous-module facteur direct de E. Soit N un sous-module de E tel que N ∩ I = 0, et maximal pour cette propriété (un tel N existe d’après loc. cit.). L’homomorphisme composé

$$
I \xrightarrow{u} E \xrightarrow{v} E/N,
$$

où u et v sont les homomorphismes canoniques, est injectif; puisque E est injectif, il existe donc un homomorphisme w : E/N → E tel que w ∘ v ∘ u = u, c’est-à-dire w ∘ v(x) = x pour x ∈ I. Posons I′ = Im(w) = Im(w ∘ v) et soit i′ : M → I′ l’injection canonique. Alors I ⊂ I′; pour achever la démonstration, il suffit de prouver que i′ satisfait à la condition (E): cela entraîne que I = I′ (caractère maximal de I) donc que w ∘ v est un projecteur de E sur I.

Soit donc P un sous-module de I′ tel que P ∩ M = 0. On a P = w ∘ v(Q), où Q est un sous-module de E contenant N; de plus

$$
Q \cap M = w \circ v(Q \cap M) \subset P \cap M = 0,
$$

donc Q ∩ I = 0 puisque i : M → I possède la propriété (E). D’après le caractère maximal de N, cela implique Q = N, c’est-à-dire v(Q) = 0, donc P = 0, ce qu’il fallait démontrer.

b) Soient (I, i) et (J, j) deux enveloppes injectives de M. Puisque J est injectif, il existe un homomorphisme f : I → J tel que f ∘ i = j; on a

$$
i^{-1}(\mathrm{Ker}\,f') = \mathrm{Ker}\,j = 0,
$$

donc Ker f = 0 et f est injectif. Alors f(I) est un sous-module injectif de J, donc facteur direct; puisque j satisfait à (E), cela implique f(I) = J et f est bijectif.

#### Remarque 1 {#alg-x-s1-n9-rem-1 .statement}

Soient (I, i) une enveloppe injective de M et $j : M \to J$ un homomorphisme injectif de M dans un A-module injectif J. D’après la démonstration ci-dessus, il existe un homomorphisme *injectif* $f : I \to J$ tel que $f \circ i = j$.

#### Remarque 2 {#alg-x-s1-n9-rem-2 .statement}

Soit (I, i) une enveloppe injective de M. Identifions M au sous-module $i(M)$ de I. Pour tout sous-module N de M, il existe un sous-module injectif de I qui est une enveloppe injective de N (appliquer la *remarque* 1 à N). Inversement, tout sous-module injectif J de I est enveloppe injective de $J \cap M$.

#### Proposition 14 {#alg-x-s1-prop-14 .statement}

*Soit I un A-module injectif non nul. Les conditions suivantes sont équivalentes*:
(i) *I est indécomposable* (VII, § 4, no 8, déf. 3);
(ii) *0 n’est pas intersection de deux sous-modules non nuls de I*;
(iii) *I est l’enveloppe injective de tous ses sous-modules non nuls*;
(iv) *l’anneau* $\mathrm{End}_A(I)$ *est local* (VIII, § 1, no 4, déf. 4).

(i) $\Rightarrow$ (iii) : soit M un sous-module non nul de I. D’après la *remarque* 2 ci-dessus, il existe un sous-module I’ de I, qui est une enveloppe injective de M. Comme I’ est non nul et facteur direct dans I, on a $I = I'$ si I est indécomposable.

(iii) $\Rightarrow$ (ii) : soient E et F deux sous-modules de I, tels que $E \cap F = 0$. Si $E \neq 0$, alors I est enveloppe injective de E d’après (iii), donc « $E \cap F = 0$ » implique « $F = 0$ ».

(ii) $\Rightarrow$ (i) : c’est trivial.

(iv) $\Rightarrow$ (i) : cela résulte de VIII, § 1, no 6, prop. 13.

(i) $\Rightarrow$ (iv) : supposons I indécomposable. Notons d’abord que tout endomorphisme injectif $f$ de I est bijectif (puisque $f(I)$ est alors un sous-module facteur direct non nul de I). Par ailleurs, tout endomorphisme $f$ de I, dont la restriction à un sous-module E non nul de I est injective, est injectif (en effet, puisque (i) $\Rightarrow$ (iii), I est enveloppe injective de E, donc « $E \cap \mathrm{Ker}\ f = 0$ » implique « $\mathrm{Ker}\ f = 0$ »). Cela étant, soit $f$ un élément non inversible de $\mathrm{End}_A(M)$; d’après VIII, § 1, no 4, prop. 9, il s’agit de prouver que $1 - f$ est inversible. Comme $f$ n’est pas injectif, on a $\mathrm{Ker}\ f \neq 0$; comme la restriction de $1 - f$ à $\mathrm{Ker}\ f$ est injective, $1 - f$ est injectif, donc bijectif.

#### Corollaire 1 {#alg-x-s1-prop-14-cor-1 .statement}

*La relation « I est une classe de A-modules injectifs indécomposables » est collectivisante*.

En effet, d’après (iii) tout A-module injectif indécomposable est enveloppe injective d’un A-module monogène.

#### Corollaire 2 {#alg-x-s1-prop-14-cor-2 .statement}

*Soient M un A-module, I une enveloppe injective de M. Pour que I soit indécomposable, il faut et il suffit que 0 ne soit pas intersection de deux sous-modules non nuls de M*.

La condition est nécessaire d’après la prop. 14 ((i) $\Rightarrow$ (ii)). Inversement, si I est somme directe des sous-modules non nuls $I_1$ et $I_2$, on a :

$$
I_1 \cap M \neq 0,\quad I_2 \cap M \neq 0\quad \text{et}\quad (I_1 \cap M) \cap (I_2 \cap M) = 0 .
$$

#### Exemple 2 {#alg-x-s1-n9-exa-2 .statement}

Si A est commutatif et nœthérien, les A-modules injectifs indécomposables sont exactement les enveloppes injectives des modules A/p où p est un idéal premier (X, p. 171, exercice 27).

### 10. Structure des modules injectifs

#### Lemme 4 {#alg-x-s1-lem-4 .statement}

Soient M un A-module nœthérien non nul, I une enveloppe injective de M. Alors I possède un sous-module injectif indécomposable.

On peut évidemment supposer que M est un sous-module de I. Soit N un sous-module de M, tel que I ne soit pas une enveloppe injective de N et maximal pour cette propriété. D’après la remarque 2 (X, p. 21), il existe un sous-module I₁ de I qui est une enveloppe injective de N ; alors I₁ est facteur direct dans I, soit J un supplémentaire. On a J ≠ 0, montrons que J est indécomposable. Si J′ est un sous-module facteur direct non nul de J, on a J′ ∩ M ≠ 0 et

$$(J' \cap M) \cap N \subset J' \cap I_1 = 0.$$

Le sous-module N′ = (J′ ∩ M) + N de M est somme directe de J′ ∩ M et N, donc contient strictement N. Par ailleurs N′ est contenu dans le sous-module J′ + I₁ de J, qui est somme directe de J′ et I₁, donc injectif. D’après le caractère maximal de N, cela implique J′ + I₁ = I, donc J′ = J, et J est indécomposable.

Notons $\mathcal{I}$ l’ensemble (X, p. 21, cor. 1) des classes de A-modules injectifs indécomposables.

Rappelons (X, p. 17, cor. 1) que, si A est nœthérien à gauche, tout A-module somme directe de A-modules injectifs est injectif.

#### Théorème 3 {#alg-x-s1-thm-3 .statement}

Soit I un A-module injectif.

a) Si I est l’enveloppe injective d’un A-module nœthérien M, I est somme directe d’une famille finie de sous-modules (injectifs) indécomposables.

b) Si A est nœthérien à gauche, I est somme directe d’une famille de sous-modules (injectifs) indécomposables.

c) Si I est somme directe de sous-modules (injectifs) indécomposables, il existe une famille de cardinaux $(a_E)_{E \in \mathcal{I}}$, et une seule, telle que I soit isomorphe à

$$\bigoplus_{E \in \mathcal{I}} E^{(a_E)}.$$

Notons d’abord que c) résulte de la prop. 14 (X, p. 21) et de VIII, § 1, n° 7, théorème 2. Démontrons a).

Soit N un sous-module de M dont les enveloppes injectives soient somme directe d’une famille finie de sous-modules indécomposables, et maximal pour cette propriété (il en existe puisque M est nœthérien). D’après la remarque 2 (X, p. 21), il existe un sous-module I₁ de I qui est une enveloppe injective de N. Si I₁ = I, la démonstration est achevée ; sinon, soit $J$ un supplémentaire de $I_1$ dans $I$. Alors $J$ est enveloppe injective du module nœthérien $J\cap M$ (loc. cit.), donc possède un sous-module injectif indécomposable $J'$ (lemme 4). Alors $I_1+J'$ est injectif, somme directe d’une famille finie de sous-modules indécomposables, et enveloppe injective du sous-module $(I_1+J')\cap M$ de $M$ qui majore strictement $N$, d’où une contradiction.

Supposons $A$ nœthérien à gauche et démontrons b). Soit $X$ l’ensemble somme des ensembles $\operatorname{Hom}_A(E,I)$ pour $E\in\mathcal{J}$. A chaque partie $Y$ de $X$ associons un $A$-module $E_Y$ et un $A$-homomorphisme $f_Y:E_Y\to I$ de la façon suivante : $Y$ est la somme d’une famille $(Y(E))_{E\in\mathcal{J}}$ où $Y(E)\subset\operatorname{Hom}_A(E,I)$, on pose

$$
E_Y=\bigoplus_{E\in\mathcal{J}}E^{(Y(E))}
$$

et la composante de $f$ sur le facteur direct de $E_Y$ correspondant à l’élément $y$ de $Y(E)\subset\operatorname{Hom}_A(E,I)$ est $y:E\to I$. Soit $Y$ une partie de $X$, telle que $f_Y$ soit injectif et que $Y$ soit maximal pour cette propriété (une telle partie existe d’après E, III, p. 20) ; il suffit de prouver que $f_Y$ est bijectif. Sinon, soit $J$ un supplémentaire du sous-module injectif $\operatorname{Im}(f_Y)$ de $I$ ; puisque $J$ est non nul, il possède un sous-module nœthérien non nul (parce que $A$ est supposé nœthérien), donc aussi un sous-module injectif $J'$ non nul enveloppe injective d’un module nœthérien. D’après a), $J'$ est somme directe d’une famille finie non vide de sous-modules indécomposables. Il existe donc une partie finie $Y'$ non vide de $X$ telle que $f_{Y'}$ applique bijectivement $E_{Y'}$ sur $J'$. Comme $\operatorname{Im}(f_Y)\cap J'=0$, on a $Y\cap Y'=\varnothing$ et $f_{Y\cup Y'}$ est injectif ; cela contredit le caractère maximal de $Y$ et achève la démonstration.

## EXERCICES {#alg-x-s1-exercises}

See the [exercises for § 1](exercises/s1/).
