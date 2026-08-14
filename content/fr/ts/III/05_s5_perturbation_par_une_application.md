---
book: ts
book_title: Théories spectrales
chapter: III
chapter_title: APPLICATIONS LINÉAIRES COMPACTES ET PERTURBATIONS
section: 5
section_title: Perturbation par une application linéaire compacte
lang: fr
source: ts-iii-v-fr
book_pages: A III.71-A III.82, A III.125-A III.128
pdf_pages: 0085-0096, 0139-0142
extraction: native
subsections:
    - "no": 1
      title: Morphismes stricts et propreté
      page: 71
      pdf_page: 85
    - "no": 2
      title: Perturbation des applications linéaires injectives ou surjec- tives
      page: 72
      pdf_page: 86
    - "no": 3
      title: Perturbation des applications de Fredholm
      page: 73
      pdf_page: 87
    - "no": 4
      title: Perturbation des endomorphismes de Riesz
      page: 75
      pdf_page: 89
    - "no": 5
      title: La théorie de Frédéric Riesz
      page: 77
      pdf_page: 91
    - "no": 6
      title: Alternative de Fredholm
      page: 79
      pdf_page: 93
statements: 19
exercises: 11
content_sha256: 35e0a105157ed1d8224d87b237d1b1e82b058529a3bc71a4273044ff48b03903
---

## § 5. PERTURBATION PAR UNE APPLICATION LINÉAIRE COMPACTE

### 1. Morphismes stricts et propreté

#### Lemme 1 {#ts-iii-s5-lem-1 .statement tag=02TK}

Soient E et F des espaces vectoriels topologiques, $u$ une application linéaire continue de E dans F et U un voisinage de 0 dans E. On suppose que $u$ induit un homéomorphisme de U sur une partie fermée de F. Alors l’image I de $u$ est fermée et $u$ induit un homéomorphisme de E sur I.

L’ensemble $u(U)$ est un voisinage de 0 dans I ; il est fermé dans F, donc le sous-groupe I de F est localement fermé en 0, et par conséquent il est fermé (TG, III, p. 7, prop. 4).

Comme Ker($u$) ne rencontre U qu’en 0, on a Ker($u$) $=\{0\}$ et l’application $u$ est injective. Soit V un voisinage fermé de 0 dans E contenu dans U. Comme $u(\mathring{V})$ est un voisinage de 0 dans $u$(V), il existe un voisinage équilibré W de 0 dans F tel que $u(V)\cap W\subset u(\mathring{V})$. L’ensemble $\overset{-1}{u}(W)$ est équilibré, donc connexe. Il contient 0 et est contenu dans $\mathring{V}\cup (E$ - V). Comme $\mathring{V}$ et E- V sont des parties ouvertes disjointes de E, l’ensemble $\overset{-1}{u}(W)$ est contenu dans $\mathring{V}$, d’où $W\cap I\subset u(\mathring{V})$. Par suite $u(\mathring{V})$ est un voisinage de 0 dans I. Cela implique que $u$ induit un homéomorphisme de E sur I.

#### Proposition 1 {#ts-iii-s5-prop-1 .statement tag=02TL}

Soient E un espace localement convexe séparé, F un espace localement convexe et $u$ une application linéaire continue de E dans F. Les conditions suivantes sont équivalentes :

(i) L’application $u$ est un morphisme strict, son noyau est de dimension finie et son image est fermée dans F ;

(ii) Il existe un voisinage fermé V de 0 dans E tel que la restriction de $u$ à V soit propre (TG, I, p. 72).

(i) $=\Rightarrow$ (ii) : Supposons que $u$ vérifie la condition (i). Comme le noyau de $u$ est de dimension finie, il possède un supplémentaire topologique $E_1$ dans E (III, p. 55, prop. 1), et il existe un voisinage compact C de 0 dans Ker($u$). Identifions E à $E_1\times$ Ker($u$); l’ensemble $V = E_1\times C$ est alors un voisinage fermé de 0 dans E. La restriction de $u$ à V est composée de la projection de $E_1\times C$ sur $E_1$ qui est propre (TG, I, p. 77, cor. 5) et de la restriction $u_1$ de $u$ à $E_1$. Or $u_1$ est un homéomorphisme de $E_1$ sur un sous-espace fermé de F, donc est propre (TG, I, p. 72, prop. 2). La composée de deux applications propres est propre (TG, I, p. 73, prop. 5, a)), donc la restriction de $u$ à V est propre.

(ii) $=\Rightarrow$ (i) : Soit V un voisinage fermé de 0 dans E tel que la restriction $v$ de $u$ à V soit propre. L’ensemble $V\cap$ Ker($u$) $=\overset{-1}{v}(\{0\})$ est alors compact (TG, I, p. 75, th. 1) ; par suite, l’espace vectoriel Ker($u$) est localement compact, donc de dimension finie (EVT, I, p. 15, th. 3). Soit $E_1$ un supplémentaire topologique de Ker($u$) dans E (prop. 1 de III, p. 55) ; posons $V_1= E_1\cap V$. L’ensemble $V_1$ est fermé dans V. L’application $u|V_1$ est propre (TG, I, p. 74, cor. 1) et injective, donc est un homéomorphisme de $V_1$ sur une partie fermée de F (TG, I, p. 72, prop. 2). D’après le lemme 1, la restriction de $u$ à $E_1$ est un homéomorphisme de $E_1$ sur un sous-espace fermé de F, donc $u$ est un morphisme strict d’image fermée.

### 2. Perturbation des applications linéaires injectives ou surjec- tives

#### Théorème 1 {#ts-iii-s5-thm-1 .statement tag=02TM}

Soient E et F des espaces localement convexes séparés et $u$ un morphisme strict de E dans F, dont le noyau est de dimension finie et dont l’image est fermée. Soit $h$ une application linéaire compacte de E dans F. L’application linéaire $u+h$ est un morphisme strict, son noyau est de dimension finie et son image est fermée.

D’après la prop. 1 de III, p. 71, il existe un voisinage fermé V de 0 dans E tel que la restriction de $u$ à V soit propre. Puisque $h$ est compacte, il existe un voisinage fermé W de 0 contenu dans V tel que l’ensemble $h(W)$ soit relativement compact. Posons $C =h(W)$. La restriction de $u$ à W est propre (TG, I, p. 74, cor. 1). L’application $\alpha :x\mapsto (u(x), h(x))$ de W dans $F\times C$ est propre car l’application pr$_1\circ \alpha =u|W$ de W dans F est propre (TG, I, p. 73, prop. 5, d)). L’application $\beta : (y, z)\mapsto (y+z, z)$ de $F\times C$ dans $F\times C$ est un homéomorphisme, et l’application pr$_1$ de $F\times C$ dans F est propre (TG, I, p. 77, cor. 5). L’application composée pr$_1\circ \beta \circ \alpha$ de W dans F est donc propre (TG, I, p. 73, prop. 5, a)). Or cette application n’est autre que la restriction de $u+h$ à W. D’après la prop. 1 de III, p. 71$,u+h$ est un morphisme strict, son noyau est de dimension finie et son image est fermée.

#### Lemme 2 {#ts-iii-s5-lem-2 .statement tag=02TN}

Soient E et F des espaces de Fréchet et $u\in \mathscr{L}(E; F)$. Les conditions suivantes sont équivalentes :

(i) Le conoyau de $u$ est de dimension finie ;

(ii) L’application $^tu: F'_c\rightarrow E'_c$ est un morphisme strict d’image fermée dont le noyau est de dimension finie.

(i) $=\Rightarrow$ (ii) : Supposons que le conoyau de $u$ est de dimension finie. L’application $u$ est alors un morphisme strict (lemme 6 de III, p. 52). D’après la prop. 2 de EVT, IV, p. 27, l’image de $^tu$ est fermée dans $E'$ muni de la topologie faible, et a fortiori dans $E'_c$. Le noyau de $^tu$ est l’orthogonal de l’image de $u($loc. cit.) ; il est donc de dimension finie. Enfin, $^tu$ est un morphisme strict de $F'_c$ dans $E'_c$ d’après le théorème 1 de EVT, IV, p. 28.

(ii) $=\Rightarrow$ (i) : Supposons que $^tu: F'_c\rightarrow E'_c$ soit un morphisme strict. D’après EVT, IV, p. 28, th. 1, l’image de $u$ est fermée. Le noyau de $^tu$ est l’orthogonal de Im($u$) (EVT, IV, p. 27, prop. 2) ; si ce noyau est de dimension finie, l’image de $u$ est de codimension finie dans F.

#### Théorème 2 {#ts-iii-s5-thm-2 .statement tag=02TO}

Soient E et F des espaces de Fréchet, $u: E\rightarrow F$ une application linéaire continue dont le conoyau est de dimension finie, et $h: E\rightarrow F$ une application linéaire compacte. L’application linéaire $u+h$ est un morphisme strict, son conoyau est de dimension finie et son image est fermée.

D’après le lemme 6 de III, p. 52, il suffit de montrer que le conoyau de $u+h$ est de dimension finie. Or, d’après la prop. 9 de III, p. 9, l’application $^th$ de $F'_c$ dans $E'_c$ est compacte ; le théorème 2 résulte du théorème 1 et du lemme 2.

### 3. Perturbation des applications de Fredholm

#### Théorème 3 {#ts-iii-s5-thm-3 .statement tag=02TP}

Soient E un espace localement convexe, F un espace localement convexe séparé, $u$ une application de Fredholm de E dans F et $h$ une application linéaire compacte de E dans F. Alors $u+h$ est une application de Fredholm, et l’on a ind($u+h$) $=$ ind($u$).

Nous prouverons le théorème en trois étapes.

A) On suppose que E et F sont des espaces de Banach. La prop. 2 de III, p. 42 montre que l’application linéaire $u$ est un morphisme strict d’image fermée dont le noyau et le conoyau sont de dimension finie. Puisque E et F sont des espaces de Banach, les th. 1 et 2 de III, p. 73 impliquent que, pour tout $t\in [0,1]$, l’application linéaire $u_t=u+th$ possède ces mêmes propriétés, et est donc une application de Fredholm (III, p. 42, prop. 2). L’application $t\mapsto u_t$ de $[0,1]$ dans l’ensemble $\mathscr{F}(E; F)$ des applications de Fredholm de E dans F est continue. D’après le th. 1 de III, p. 58, l’application $t\mapsto$ ind($u_t$) est localement constante. Comme l’intervalle $[0,1]$ de $\mathbf{R}$ est connexe, cette application est constante. On a donc ind($u$) $=$ ind($u+h$).

B) On suppose que E = F et $u= 1_E$. D’après la prop. 5 de III, p. 5, il existe un espace de Banach G, une application linéaire continue $p: E\rightarrow G$ et une application linéaire compacte $q: G\rightarrow E$ telle que $h=q\circ p$. L’endomorphisme $p\circ q$ de G est compact. D’après A), $1_G+p\circ q$ est un endomorphisme de Fredholm de G d’indice nul. Mais alors $1_E+h= 1_E+q\circ p$ est un endomorphisme de Fredholm de E d’indice nul (III, p. 49, prop. 10, f )).

C) Cas général. Soit $v$ un quasi-inverse de $u$. Les endomorphismes $u\circ v$ et $(u+h)\circ v$ de F diffèrent de $1_F$ par des applications linéaires compactes. D’après B), ce sont des endomorphismes de Fredholm de F d’indice nul. Il en résulte que $u+h$ est un endomorphisme de Fredholm (III, p. 40, n$^o2$) de même indice que $u($III, p. 43, n$^o3$, formule (2)).

#### Corollaire 1 {#ts-iii-s5-thm-3-cor-1 .statement tag=02TQ}

Soient E et F des espaces localement convexes séparés et $u\in \mathscr{L}(E; F)$. Pour que $u$ soit une application de Fredholm, il faut et il suffit qu’il existe une application $v\in \mathscr{L}(F; E)$ telle que les applications linéaires $1_E-v\circ u$ et $1_F-u\circ v$ soient compactes.

Comme une application linéaire continue de rang fini est compacte, la condition énoncée est nécessaire.

Soit $v$ un élément de $\mathscr{L}(F; E)$ tel que les applications linéaires $1_E-v\circ u$ et $1_F-u\circ v$ soient compactes. D’après le théorème 3$,v\circ u$ et $u\circ v$ sont des applications de Fredholm. Soit $p$ et $q$ des quasi-inverses de $v\circ u$ et $u\circ v$ respectivement. Posons $w=p\circ v$ et $w'=v\circ q$. Avec les notations du n$^o2$ de III, p. 40, on a $w\circ u\equiv 1_E$ et $u\circ w'\equiv 1_F$, d’où $w\equiv w\circ u\circ w'\equiv w'$. Il en résulte que $w$ est un quasi-inverse de $u$.

#### Corollaire 2 {#ts-iii-s5-thm-3-cor-2 .statement tag=02TR}

Soient E et F des espaces localement convexes séparés et $u\in \mathscr{L}(E; F)$. Les conditions suivantes sont équivalentes :

(i) L’application $u$ est une application de Fredholm d’indice nul;

(ii) Il existe un isomorphisme $v$ de E sur F tel que $u-v$ soit de rang fini ;

(iii) Il existe un isomorphisme $v$ de E sur F tel que $u-v$ soit compact.

(i) $=\Rightarrow$ (ii) : Supposons que $u$ soit une application de Fredholm d’indice nul. Il existe des décompositions en somme directe topologique $E = E_1\oplus E_2$ et $F = F_1\oplus F_2$ avec $E_2$ et $F_2$ de dimension finie telles que $u$ s’annule sur $E_2$ et définisse par restriction un isomorphisme $u_1$ de $E_1$ sur $F_1($III, p. 42, prop. 2). Si ind($u$) $= 0$, alors les dimensions de $E_2$ et $F_2$ sont égales et il existe un isomorphisme $v$ de E sur F prolongeant $u_1$. Le noyau de $u-v$ contient $E_1$, donc $u-v$ est de rang fini.

On a (ii) $=\Rightarrow$ (iii) puisque toute application linéaire continue de rang fini de E dans F est compacte, et (iii) $=\Rightarrow$ (i) d’après le th. 3.

### 4. Perturbation des endomorphismes de Riesz

Soit E un espace de Banach. Rappelons (cf. III, p. 5, prop. 3) que l’ensemble $\mathscr{L}^c(E)$ des endomorphismes compacts de E est un idéal bilatère fermé de l’algèbre de Banach $\mathscr{L}(E)$. L’algèbre de Banach quotient est appelée l’algèbre de Calkin de E ; on la note $\mathscr{C}$alk(E). On note $\pi$ l’homomorphisme canonique de $\mathscr{L}(E)$ sur $\mathscr{C}$alk(E). D’après le cor. 1 de III, p. 74, un endomorphisme $u$ de E est un endomorphisme de Fredholm si et seulement si $\pi (u)$ est inversible dans l’algèbre $\mathscr{C}$alk(E).

#### Proposition 2 {#ts-iii-s5-prop-2 .statement tag=02TS}

Soit $u\in \mathscr{L}(E)$ tel que $\|1_E-\pi (u)\|<1$ dans l’algèbre $\mathscr{C}$alk(E). Alors $u$ est un endomorphisme de Riesz de E.

Soit $r\geqslant 1$ un entier tel que $\|1_E-\pi (u)\|^r<^1_2$. Soit $P\in \mathbf{C}[X]$ le polynôme $^{1-(1-X)^r}_X$. Notons $v= 1_E-(1_E-u)^r$. On a donc $v=uP(u)$ et $\|1_E-\pi (v)\|<^1_2$. Comme les endomorphismes $u$ et $P(u)$ de E commutent, il suffit de prouver que $v$ est un endomorphisme de Riesz de E (III, p. 49, prop. 9).

Puisque $\|1_E-\pi (v)\|<1/2$, il existe, par définition de la norme quotient dans l’espace $\mathscr{C}$alk(E), un endomorphisme compact $h$ de E et un endomorphisme $w$ de E tels que $v= 1_E+h+w$ et $\|w\|<^1_2$. D’après le corollaire 1 de I, p. 22, l’élément $1_E+w$ est un automorphisme de E. Comme $h$ est compact, $v= (1_E+w) +h$ est un endomorphisme de Fredholm de E d’indice 0 (cor. 2 de III, p. 74). Pour tout entier $n\geqslant 0$, notons $N_n$ le noyau de $v^n$. Pour démontrer que $v$ est un endomorphisme de Riesz de E, il suffit de prouver qu’il existe un entier $n\geqslant 0$ tel que $N_n= N_{n+1}($III, p. 46, déf. 2 et III, p. 46, remarque).

Raisonnons par l’absurde en supposant la suite $(N_n)$ strictement croissante. Pour tout $n\in \mathbf{N}$, soit $p_n$ l’application canonique de E sur l’espace normé $E/N_n$. Soit $c$ un nombre réel tel que $2\|w\|< c <1$. Soit $n\in \mathbf{N}$. Puisque $N_{n+1}$ est différent de $N_n$, il existe un élément $x_n\in N_{n+1}$ tel que $\|p_n(x_n)\|=c$ et tel que $\|x_n\|<1$ (en effet, il existe $y\in N_{n+1}/N_n$ de norme $c$ donc, pour tout $\varepsilon  >0$, il existe $x_n\in N_{n+1}$ tel que $p_n(x_n) =y$ et $\|x_n\|\leqslant c+\varepsilon )$.

Soient $m,n$ deux entiers tels que $m > n\geqslant 0$. On a

$$
\|h(x_m)-h(x_n)\|=\|v(x_m-x_n)-(1_E+w)(x_m-x_n)\|
$$

$$
\geqslant \|(v-1_E)(x_m-x_n)\| - \|w(x_m-x_n)\|
$$

$$
\geqslant \|(v-1_E)(x_m-x_n)\| -2\|w\| \tag{1}
$$

puisque $\|x_m\|\leqslant 1$ et $\|x_n\|\leqslant 1$. Par ailleurs, notons que

$$
(v-1_E)(x_m-x_n) =v(x_m-x_n) +x_n-x_m
$$

Mais comme $n < m$ et $v(N_{m+1})\subset N_m$, on a $v(x_m-x_n) +x_n\in N_m$, d’où

$$
\|v(x_m-x_n) +x_n-x_m\|\geqslant \|p_m(x_m)\|=c
$$

L’inégalité (1) fournit donc la minoration

$$
\|h(x_m)-h(x_n)\|\geqslant c-2\|w\|>0 \tag{2}
$$

La suite $(h(x_m))_{m\in\mathbf{N}}$ n’a donc aucune valeur d’adhérence dans E, ce qui contredit le fait que l’image par $h$ de la boule unité de E est relativement compacte, puisque $h$ est compact (remarque 1 de III, p. 2).

#### Corollaire 1 {#ts-iii-s5-prop-2-cor-1 .statement tag=02TT}

Soit E un espace localement convexe séparé et soit $u\in \mathscr{L}(E)$. Pour que $u$ soit un endomorphisme de Riesz, il faut et il suffit qu’il existe un élément $v$ de $\mathscr{L}(E)$ qui commute à $u$ et tel que $1_E-u\circ v$ soit compact.

Comme toute application linéaire continue de rang fini est compacte, la condition est nécessaire (III, p. 47, prop. 6 d)). Démontrons qu’elle est suffisante. Soit $v$ un élément de $\mathscr{L}(E)$ qui commute à $u$ et tel que l’endomorphisme $h= 1_E-u\circ v$ de E soit compact. Il existe un espace de Banach G, une application linéaire continue $p: E\rightarrow G$ et une application linéaire compacte $q: G\rightarrow E$ tels que $h=q\circ p($III, p. 5, prop. 5). L’endomorphisme $p\circ q$ de G est compact. D’après la prop. 2, l’application linéaire $1_G-p\circ q$ est un endomorphisme de Riesz de G. Mais alors $u\circ v= 1_E-q\circ p$ est un endomorphisme de Riesz de E (III, p. 49, prop. 10, g)). Comme $u$ et $v$ commutent, $u$ est un endomorphisme de Riesz de E (III, p. 49, prop. 9).

#### Corollaire 2 {#ts-iii-s5-prop-2-cor-2 .statement tag=02TU}

Soient E un espace localement convexe séparé, $u$ un endomorphisme de Riesz de E et $h\in \mathscr{L}(E)$ une application linéaire compacte. Si $u$ et $h$ commutent, alors $u+h$ est un endomorphisme de Riesz de E.

Soit $v$ le quasi-inverse canonique de $u$. Il commute à $u$ et à $h($III, p. 47, prop. 6), donc à $u+h$. L’endomorphisme $1_E-(u+h)\circ v$ de E est somme de l’application linéaire continue de rang fini $1_E-u\circ v$ et de l’application linéaire compacte $-h\circ v$, donc est compact. Il en résulte que $u+h$ est un endomorphisme de Riesz de E (corollaire 1).

#### Proposition 3 {#ts-iii-s5-prop-3 .statement tag=02TV}

Soit E un espace de Banach. Soit $u$ un endomorphisme de E, soit A son commutant dans $\mathscr{L}(E)$. L’adhérence B de $\pi (A)$ dans l’algèbre $\mathscr{C}$alk(E) est une algèbre de Banach. Pour que $u$ soit un endomorphisme de Riesz de E, il faut et il suffit que $\pi (u)$ soit inversible dans B.

Puisque $\pi (A)$ est une sous-algèbre unifère de $\mathscr{C}$alk(E), son adhérence B est une algèbre de Banach. Si $u$ est un endomorphisme de Riesz de E, l’élément $\pi (u)$ possède un inverse dans $\pi (A)$ (cor. 1), donc dans B. Réciproquement, supposons que $\pi (u)$ ait un inverse $s$ dans B. Par définition de B, il existe un élément $v$ de A tel que

1

$$
\|s-\pi (v)\|<
$$

$$
\|\pi (u)\|
$$

d’où $\|1_E-\pi (u\circ v)\|<1$. D’après la prop. 2, l’application linéaire $u\circ v$ est un endomorphisme de Riesz de E. Il en est de même de $u$ puisque $u$ et $v$ commutent (III, p. 49, prop. 9).

### 5. La théorie de Frédéric Riesz

Soit E un espace localement convexe séparé et soit $h$ un endomorphisme compact de E. Soit $\lambda \in K$. L’endomorphisme $\lambda h$ est compact, donc $1_E-\lambda h$ est un endomorphisme de Riesz de E (cor. 2 de la prop. 2 de III, p. 75) ; notons $N_{\lambda}$ et $I_{\lambda}$ son nilespace et son conilespace. D’après la prop. 6 de III, p. 47, on a les propriétés suivantes :

(i) Les sous-espaces vectoriels $I_{\lambda}$ et $N_{\lambda}$ de E sont fermés et stables par $h$;

(ii) L’espace localement convexe E est somme directe topologique de $I_{\lambda}$ et $N_{\lambda}$;

(iii) L’application $1_E-\lambda h$ définit par restriction un automorphisme de $I_{\lambda}$;

(iv) L’espace vectoriel $N_{\lambda}$ est de dimension finie, et il existe un entier $n_{\lambda}\geqslant 0$ tel que $(1_E-\lambda h)^{n_{\lambda}}(x) = 0$ pour tout $x\in N_{\lambda}$.

Ces propriétés déterminent les espaces $I_{\lambda}$ et $N_{\lambda}$ de manière unique (A, VIII, p. 26, remarque 2).

#### Lemme 3 {#ts-iii-s5-lem-3 .statement tag=02TW}

Soit X un espace topologique dont la topologie possède une base dénombrable. Toute partie discrète de X est dénombrable.

Soit $\mathscr{B}$ une base dénombrable de la topologie de X et soit D une partie discrète de X. Pour chaque élément $x$ de D, il existe un élément $B_x$ de $\mathscr{B}$ tel que $B_x\cap D =\{x\}$. L’application de D dans $\mathscr{B}$ définie par $x\mapsto B_x$ est injective, d’où le lemme.

#### Théorème 4 {#ts-iii-s5-thm-4 .statement tag=02TX}

Soit E un espace localement convexe séparé et soit $h$ un endomorphisme compact de E. L’ensemble Σ des $\lambda \in K$ tels que $1_E-\lambda h$ ne soit pas un automorphisme de E est une partie dénombrable, fermée et discrète du corps K.

L’ensemble Σ est aussi l’ensemble des $\lambda \in K$ tels que $1_E-\lambda h$ ne soit pas injectif et l’ensemble des $\lambda \in K$ tels que $1_E-\lambda h$ ne soit pas surjectif.

Il existe un espace de Banach G, une application linéaire continue $p: E\rightarrow G$ et une application linéaire compacte $q: G\rightarrow E$ tels que $h=q\circ p($III, p. 5, prop. 5). L’endomorphisme $h'=p\circ q$ de G est compact, et pour que $1_E-\lambda h$ soit un automorphisme de E, il faut et il suffit que $1_G-\lambda h'$ soit un automorphisme de G (prop. 10 de III, p. 49, e)). Il nous suffit donc de démontrer le théorème lorsque E est un espace de Banach, ce que nous supposons désormais.

Soit $\lambda \in K$. Puisque l’indice d’un endomorphisme de Riesz est nul, il revient au même de dire que l’application $1_E-\lambda h$ est un automorphisme de E, ou qu’elle est injective, ou encore qu’elle est surjective.

L’ensemble Σ est fermé dans K puisque l’ensemble des automorphismes de E est ouvert dans $\mathscr{L}(E)$. Soit $\lambda$ un élément de Σ. On a $\lambda \not = 0$. Notons N le nilespace de $h$ et I son conilespace, et notons $h_I$ et $h_N$ les endomorphismes de I et de N que $h$ définit par passage aux sous-espaces. Alors $1_I-\lambda h_I$ est un automorphisme de I, et il existe un voisinage U de $\lambda$ dans K tel que $1_I-\mu h_I$ soit un automorphisme de I pour tout $\mu\in U$. L’endomorphisme $1_N-\lambda h_N$ de N est nilpotent ; pour tout $\mu\not =\lambda$, on a

$$
\lambda -\mu\mu
$$

$$
1_N-\mu h_N=1_N+(1_N-\lambda h_N)
$$

$$
\lambda \lambda -\mu
$$

donc $1_N-\mu h_N$ est un automorphisme de N. Par suite, l’ensemble $U\cap \Sigma$ est réduit au seul élément $\lambda$ et l’ensemble Σ est discret. Il est dénombrable d’après le lemme 3.

### 6. Alternative de Fredholm

#### Proposition 4 (Alternative de Fredholm) {#ts-iii-s5-prop-4 .statement tag=02TY}

Soit E un espace de Banach et soit $h$ un endomorphisme compact de E. Soit $\lambda$ un élément de K $-\{0\}$. Soient F le noyau de $1_E-\lambda h$ et G le noyau de $1_{E'}-\lambda^th$.

a) Les espaces F et G sont de même dimension finie $n\geqslant 0$;

b) Pour $y\in E$, il existe $x\in E$ tel que $x-\lambda h(x) =y$ si et seulement si $\langle y, \ell \rangle = 0$ pour tout $\ell \in G$;

c) Pour $\ell \in E'$, il existe $f\in E'$ tel que $f-\lambda^th(f) =\ell$ si et seulement si $\langle x, f\rangle = 0$ pour tout $x\in F$.

En particulier, une et une seule des conditions suivantes est valide :

(i) L’espace F est non nul ;

(ii) Pour tout $y\in E$, il existe $x\in E$ tel que $x-\lambda h(x) =y$.

En remplaçant $h$ par $\lambda h$, on se ramène au cas où $\lambda = 1$.

L’endomorphisme $^th$ est compact d’après le corollaire 1 de III, p. 9. Les endomorphismes $w= 1_E-h$ de E et $w'= 1_{E'}-^th$ de $E'$ sont donc des endomorphismes de Riesz (cor. 2 de la prop. 2 de III, p. 75). En particulier, leurs noyaux F et G sont de dimension finie. Comme $w'=^tw$ et que l’indice de $w$ est nul, la dimension de F est égale à celle de G d’après la formule (3) de III, p. 43.

Pour un élément $y$ de E, l’équation $x-h(x) =y$ a une solution $x\in E$ si et seulement si $x$ appartient à l’image de $w$. Comme le dual du conoyau de $w$ s’identifie au noyau G de Ker($^tw$) (EVT, IV, p. 27, prop. 2), c’est le cas si et seulement si $\langle y, \ell \rangle = 0$ pour tout $\ell \in G$.

Pour un élément $\ell$ de $E'$, l’équation $f-^th(f) =\ell$ a une solution $f\in E'$ si et seulement si $f$ appartient à l’image de $w'$. Comme l’image de $^tw$ est l’orthogonal du noyau F de $w$ (EVT, IV, p. 27, prop. 2) c’est le cas si et seulement si $\langle x, f\rangle = 0$ pour tout $x\in F$.

#### Exemple {#ts-iii-s5-n6-exa-1 .statement tag=02TZ}

Soient X un espace compact, $\mu$ une mesure sur X, réelle ou complexe suivant que K est égal à $\mathbf{R}$ ou $\mathbf{C}$, et $N : X\times X\rightarrow K$ une fonction continue.

Notons E l’espace de Banach $\mathscr{C}(X; K)$. Supposons donnée une fonction $a\in E$ et $\lambda \in K-\{0\}$. Étudions le problème de l’existence et de l’unicité des solutions $f\in E$ de l’équation intégrale

$$
f(x)-\lambda \int_XN(x, y)f(y)d\mu(y) =a(x)(x\in X) \tag{3}
$$

Pour cela, introduisons l’ensemble $F_{\lambda}$ des solutions $f\in E$ de l’équation homogène associée

$$
f(x)-\lambda \int_XN(x, y)f(y)d\mu(y) = 0(x\in X) \tag{4}
$$

et l’ensemble $G_{\lambda}$ des solutions $g\in E$ de l’équation homogène transposée de (4), c’est-à-dire

$$
g(y)-\lambda \int_XN(x, y)g(x)d\mu(x) = 0(y\in X) \tag{5}
$$

S’il n’est pas vide, l’ensemble des solutions de (3) est un sous-espace affine de E de direction $F_{\lambda}$.

Pour $f\in E$ et $x\in X$, posons

$$
h(f)(x) =\int_XN(x, y)f(y)d\mu(y)
$$

l’application $f\mapsto h(f)$ ainsi définie est un endomorphisme compact de l’espace de Banach E (cor. de la prop. 2 de III, p. 26). Le dual $E'$ de E se compose des mesures sur X, réelles ou complexes suivant que K est égal à $\mathbf{R}$ ou $\mathbf{C}$ (INT, III, p. 47, § 1, n$^o3$, déf. 2). La transposée $^th$ de $h$ est l’endomorphisme de $E'$ caractérisé par la relation $\langle f,^th(m)\rangle =\langle h(f), m\rangle$ pour $f\in E$ et $m\in E'$, c’est-à-dire

$$
\int_Xf(x)d(^th(m))(x) =\int_Xh(f)(x)dm(x)
$$

$$
=\int_X\int_XN(x, y)f(y)d\mu(y)dm(x)
$$

$$
=\int_X\int_XN(x, y)dm(x)f(y)d\mu(y) \tag{6}
$$

pour $m\in E'$ et $f\in E$ (INT, III, p. 84, § 4, n$^o1$, th. 2).

#### Lemme 4 {#ts-iii-s5-lem-4 .statement tag=02U0}

L’application linéaire de $G_{\lambda}$ dans $E'$ définie par $g\mapsto g\cdot \mu$ est injective, et son image est le noyau de $1_{E'}-\lambda^th$.

Si $g\in G_{\lambda}$ vérifie $g\cdot \mu= 0$, alors la formule (5) implique $g= 0$, donc l’application $g\mapsto g\cdot \mu$ est injective.

Soit $m\in E'$ une mesure appartenant au noyau de $1_{E'}-\lambda^th$. D’après la relation (6), on a

$$
\int_Xf(x)dm(x) =\lambda \int_X\int_XN(x, y)dm(x)f(y)d\mu(y) \tag{7}
$$

pour toute fonction continue $f: X\rightarrow K$. La mesure $m$ est donc égale à la mesure $g\cdot \mu$, où $g$ est la fonction continue de X dans K définie par

$$
g(y) =\lambda \int_XN(x, y)dm(x) \tag{8}
$$

pour tout $y\in X$. La formule (8) implique alors que la fonction $g$ appartient à $G_{\lambda}$.

Réciproquement, soit $g: X\rightarrow K$ une fonction continue appartenant à $G_{\lambda}$ et posons $m=g\cdot \mu$. Pour toute fonction continue $f: X\rightarrow K$, on a donc

$$
\int_Xf(y)dm(y) =\int_Xg(y)f(y)d\mu(y)
$$

$$
=\lambda \int_X\int_XN(x, y)g(x)d\mu(x)f(y)d\mu(y)
$$

$$
=\lambda \int_Xf(x)dm(x)
$$

de sorte que $^th(m) =\lambda m$. Cela démontre le lemme 4.

En appliquant la proposition 4 et le théorème 4 de III, p. 78. à l’endomorphisme $h$, on obtient alors les énoncés suivants.

#### Théorème 5 {#ts-iii-s5-thm-5 .statement tag=02U1}

Soit $\lambda \in K$.

a) Les ensembles $F_{\lambda}$ et $G_{\lambda}$ sont des sous-espaces vectoriels de dimension finie de $\mathscr{C}(X; K)$ et leur dimensions sont égales ;

b) Pour que l’équation (3) ait au moins une solution $f\in \mathscr{C}(X,K)$, il faut et il suffit que l’on ait $\int_Xa(x)g(x)d\mu(x) = 0$ pour toute fonction $g\in G_{\lambda}$. L’ensemble des solutions de (3) est alors un sous-espace affine de $\mathscr{C}(X; K)$ de direction $F_{\lambda}$;

c) Une des conditions suivantes, qui s’excluent mutuellement, est satisfaite :

(i) Pour toute fonction $a\in \mathscr{C}(X; K)$, il existe une unique

solution $f\in \mathscr{C}(X; K)$ de l’équation intégrale (3) ;

(ii) L’équation homogène (4) possède une solution non nulle

$$
f\in \mathscr{C}(X; K)
$$

#### Corollaire {#ts-iii-s5-n6-cor-1 .statement tag=02U2}

L’ensemble des $\lambda \in K$ pour lesquels l’espace $F_{\lambda}$ n’est pas nul est une partie dénombrable, fermée et discrète de K.

## EXERCICES {#ts-iii-s5-exercises}

Dans les exercices suivants, lorsque E est un espace de Banach, on note $\mathscr{C}$alk(E) l’algèbre de Calkin $\mathscr{L}(E)/\mathscr{L}^c(E)$. On note $\pi$ la projection canonique de $\mathscr{L}(E)$ dans $\mathscr{C}$alk(E).

Si E est un espace hilbertien complexe, on munit $\mathscr{C}$alk(E) de l’involution déduite de l’involution de $\mathscr{L}(E)$ par passage au quotient.

See the [exercises for § 5](exercises/s5/).
