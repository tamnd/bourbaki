---
book: ta
book_title: Topologie algébrique
chapter: II
chapter_title: GROUPOÏDES
section: 1
section_title: Carquois
lang: fr
source: ta-i-iv-fr
book_pages: TA II.151-TA II.155, TA II.215-TA II.218
pdf_pages: 0167-0171, 0231-0234
extraction: native
subsections:
    - "no": 1
      title: Définition d’un carquois
      page: 151
      pdf_page: 167
    - "no": 2
      title: Sous-carquois
      page: 152
      pdf_page: 168
    - "no": 3
      title: Morphismes de carquois
      page: 152
      pdf_page: 168
    - "no": 4
      title: Produits de carquois
      page: 153
      pdf_page: 169
    - "no": 5
      title: Chemins et lacets dans un carquois
      page: 154
      pdf_page: 170
    - "no": 6
      title: Composantes connexes d’un carquois
      page: 154
      pdf_page: 170
statements: 2
exercises: 10
content_sha256: b5945a675f9d2e07ca143e96570aaf025abe6517cdfc0254d8c5e11cc1620c22
---

## § 1. CARQUOIS

Son monument, superbe entre les monuments,

Qui hérisse, au-dessus d’un mur de briques sèches, Son faîte de tours comme un carquois de flèches...

Victor Hugo, Légende des siècles

### 1. Définition d’un carquois

#### Définition 1 {#ta-ii-s1-def-1 .statement tag=01SS}

Un carquois est un quadruplet $(S,F, o, t)$, où S et F sont des ensembles et $o,t$ des applications de F dans S.

Soit $C = (S,F, o, t)$ un carquois. Les éléments de S s’appellent les sommets de C. Les éléments de F s’appellent les flèches de C. Soit $f$ une flèche de C ; le sommet $o(f)$ s’appelle l’origine ou la source de $f$, le sommet $t(f)$ s’appelle le terme, ou le but de $f$; on dit aussi que $f$ relie le sommet $o(f)$ au sommet $t(f)$. Les applications $o$ et $t$ s’appellent respectivement les applications source et but, ou origine et terme, du carquois C.

© N. Bourbaki et Springer-Verlag Berlin Heidelberg 2   016

N. Bourbaki, Topologie algébrique, DOI 10.1007/978-3-662-49361-8_2  151

Lorsque C est un carquois, Som(C), Fl(C) $o_C$ et $t_C$ désigneront respectivement l’ensemble des sommets, celui des flèches, l’application source et l’application but de C. Soient $a$ et $b$ des sommets de C; l’ensemble des flèches de C reliant $a$ à $b$ est noté Fl$_{a,b}(C)$, ou encore $C_{a,b}$.

Pour faciliter la compréhension des raisonnements, on peut représenter un carquois par un dessin composé de points et de traits fléchés correspondant respectivement aux sommets et aux flèches. Le dessin :

$$
f_1g
$$

$\bullet \bullet \bullet k$

$abc$

$f_2h$

représente un carquois dont les sommets sont $a,b,c$, les flèches sont $f_1, f_2, g, h, k$, et les applications source et but sont données par

$$
o(f_1) =o(f_2) =ao(g) =bo(h) =co(k) =c
$$

$$
t(f_1) =t(f_2) =bt(g) =ct(h) =bt(k) =c
$$

### 2. Sous-carquois

Soient C et $C'$ des carquois. On dit que $C'$ est un sous-carquois de C si l’on a Som(C$')\subset$ Som(C), Fl(C$')\subset$ Fl(C) et que les applications $o_{C'}$ et $t_{C'}$ coïncident dans Fl(C$')$ avec les applications $o_C$ et $t_C$. Si, de plus, toute flèche de C dont la source et le but appartiennent à Som(C$')$ est une flèche de $C'$, on dit que $C'$ est un sous-carquois plein de C.

Soit C un carquois et soit $(C_i)_{i\in I}$ une famille de sous-carquois de C. On appelle intersection de la famille $(C_i)_{i\in I}$ et l’on note $\bigcap_{i\in I}C_i$ le sous-carquois de C dont l’ensemble des sommets est $\bigcap_{i\in I}$ Som(C$_i)$ et dont l’ensemble des flèches est $\bigcap_{i\in I}$ Fl(C$_i)$.

### 3. Morphismes de carquois

Soient C et $C'$ des carquois. Un morphisme de carquois de C dans $C'$ est un couple $(u, v)$, où $u:$ Som(C) $\rightarrow$ Som(C$')$ et $v:$ Fl(C) $\rightarrow$ Fl(C$')$ sont des applications telles que $o_{C'}\circ v=u\circ o_C$ et $t_{C'}\circ v=u\circ t_C$.

Soit $\varphi = (u, v)$ un morphisme de carquois de C dans $C'$. Les applications $u$ et $v$ se notent Som($\varphi$ ) et Fl($\varphi$ ). Si $a$ est un sommet de C, on notera par abus $\varphi (a)$ l’image d’un sommet $a$ de C et on dira que $\varphi (a)$ est l’image de $a$ par $\varphi$. De même, si $f$ est une flèche de C, on notera par abus $\varphi (f)$ la flèche $v(f)$ de $C'$ et on dira qu’elle est l’image de $f$ par $\varphi$.

Soient C, $C',C''$ trois carquois, soit $\varphi = (u, v)$ un morphisme de C dans $C'$ et soit $\varphi '= (u', v')$ un morphisme de $C'$ dans $C''$. Alors $(u'\circ u, v'\circ v)$ est un morphisme de C dans $C''$ que l’on note $\varphi '\circ \varphi$ et que l’on appelle le composé de $\varphi '$ et de $\varphi$.

On note Id$_C$ le morphisme (Id$_{Som(C)}$, Id$_{Fl(C)})$ de C dans lui-même.

Soit $\varphi$ un morphisme de carquois de C dans $C'$. Pour que $\varphi$ soit un isomorphisme, il faut et il suffit que les applications Som($\varphi$ ) et Fl($\varphi$ ) soient bijectives (cf. E, IV, p. 6).

Ainsi, si l’on appelle structure de carquois sur des ensembles S et F la donnée de deux applications $o, t: F\rightarrow S$, on peut prendre les morphismes de carquois pour morphismes de cette structure (E, IV, p. 11).

Soit $\varphi$ un morphisme de carquois de C dans $C'$. Il existe un unique sous-carquois de $C'$ dont les ensembles de sommets et de flèches sont les images de Som($\varphi$ ) et Fl($\varphi$ ) respectivement. On le note $\varphi (C)$ et on l’appelle l’image de C par $\varphi$. On dit que $\varphi$ est injectif si les applications Som($\varphi$ ) et Fl($\varphi$ ) sont injectives ; dans ce cas, $\varphi$ induit un isomorphisme de C sur son image.

Soient $\varphi$ et $\psi$ des morphismes de carquois de C dans $C'$. Il existe un unique sous-carquois de C dont les sommets et les flèches sont respectivement les sommets et les flèches de C ayant même image par $\varphi$ et $\psi$. On l’appelle l’égalisateur de $\varphi$ et $\psi$.

### 4. Produits de carquois

Soit $(C_i)_{i\in I}$ une famille de carquois. Posons S = $\prod_{i\in I}$ Som(C$_i)$, $F =\prod_{i\in I}$ Fl(C$_i)$ et soient $o$ et $t$ les applications $\prod_{i\in I}o_{C_i}$ et $\prod_{i\in I}t_{C_i}$ respectivement. Le quadruplet $C = (S,F, o, t)$ est un carquois appelé carquois produit de la famille $(C_i)_{i\in I}$.

Il existe un unique morphisme de carquois pr$_i: C\rightarrow C_i$ tel que les applications Som(pr$_i)$ et Fl(pr$_i)$ soient respectivement les projections d’indice $i$ de Som(C) dans Som(C$_i)$ et de Fl(C) dans Fl(C$_i)$.

On a la propriété universelle suivante : Soit $C'$ un carquois ; pour toute famille $(\varphi_i)_{i\in I}$, où, pour tout $i\in I,\varphi_i: C'\rightarrow C_i$ est un morphisme de carquois, il existe un unique morphisme de carquois $\varphi : C'\rightarrow C$ tel que $\varphi_i=$ pr$_i\circ \varphi$ pour tout $i\in I$.

### 5. Chemins et lacets dans un carquois

#### Définition 2 {#ta-ii-s1-def-2 .statement tag=01ST}

Soit C un carquois. Un chemin dans C est une suite $c= (a_0, f_1, a_1, . . . , a_{n-1}, f_n, a_n)$, où $n$ est un entier $\geqslant 0,a_0, . . . , a_n$ sont des sommets de C et où, pour $1\leqslant i\leqslant n,f_i$ est une flèche de C reliant $a_{i-1}$ à $a_i$. On dit que le chemin $c$ est de longueur $n$.

Soit $c= (a_0, f_1, a_1, . . . , a_{n-1}, f_n, a_n)$ un chemin de longueur $n$ dans C. Le sommet $a_0$ s’appelle l’origine, ou la source, de $c$; le sommet $a_n$ s’appelle le terme, ou le but, de $c$; on dit aussi que $c$ relie le sommet $a_0$ au sommet $a_n$. Le sommet $a_i$, pour $0\leqslant i\leqslant n$, s’appelle le sommet d’indice $i$; la flèche $f_i$, pour $1\leqslant i\leqslant n$, s’appelle la $i$-ème flèche, ou la flèche d’indice $i$. Un chemin de longueur $\geqslant 1$ est déterminé par la suite de ses flèches.

Un chemin dont l’origine est égale au terme est appelé un lacet. Un chemin de longueur 0 est un lacet, dit constant.

On dit que des chemins

$c= (a_0, f_1, a_1, . . . , a_{n-1}, f_n, a_n)$ et $c'= (a'_0, f'_1, a'_1, . . . , a'_{m-1}, f'_m, a'_m)$

dans C sont juxtaposables si le terme $a_n$ de $c$ est l’origine $a'_0$ de $c'$. Dans ce cas, la suite $(a_0, f_1, a_1, . . . , a_{n-1}, f_n, a_n, f'_1, a'_1, . . . , f'_m, a'_m)$ est un chemin dans C que l’on note $c*c'$ et que l’on appelle le chemin juxtaposé de $c$ et $c'$. Il relie l’origine de $c$ au terme de $c'$; sa longueur est la somme des longueurs des chemins $c$ et $c'$.

### 6. Composantes connexes d’un carquois

Soit $C = (S,F, o, t)$ un carquois. Considérons la relation d’équivalence $R_C$ dans S la plus fine telle que la relation $R_C\{o(f), t(f)\}$ soit satisfaite pour toute flèche $f$ de C. Deux sommets $a,b$ de C sont équivalents pour cette relation si et seulement s’il existe un entier $n\geqslant 0$, des sommets $a_0, . . . , a_n$ de C et des flèches $f_1, . . . , f_n$ de C tels que $a_0=a,a_n=b$ et tels que, pour $1\leqslant i\leqslant n$, la flèche $f_i$ relie ou bien $a_{i-1}$ à $a_i$, ou bien $a_i$ à $a_{i-1}$.

Les classes d’équivalence de cette relation d’équivalence s’appellent les composantes connexes de C. On note $\pi_0(C)$ l’ensemble des composantes connexes de C. On dit enfin que C est connexe s’il a au plus une composante connexe.

Soit $\varphi : C\rightarrow C'$ un morphisme de carquois. L’application Som($\varphi$ ) définit par passage aux quotients une application de $\pi_0(C)$ dans $\pi_0(C')$ qu’on notera $\pi_0(\varphi )$.

## EXERCICES {#ta-ii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
