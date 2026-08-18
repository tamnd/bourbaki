---
book: ts
book_title: Théories spectrales
chapter: III
chapter_title: APPLICATIONS LINÉAIRES COMPACTES ET PERTURBATIONS
section: 6
section_title: Propriétés spectrales des endomorphismes des espaces de Banach
lang: fr
source: ts-iii-v-fr
book_pages: TS III.82-TS III.101, TS III.128-TS III.142
pdf_pages: 0096-0115, 0142-0156
extraction: native
subsections:
    - "no": 1
      title: Points isolés et points sensibles du spectre
      page: 82
      pdf_page: 96
    - "no": 2
      title: Une partition du spectre
      page: 85
      pdf_page: 99
    - "no": 3
      title: Spectre du transposé d’un endomorphisme
      page: 88
      pdf_page: 102
    - "no": 4
      title: Perturbation par un opérateur compact
      page: 89
      pdf_page: 103
    - "no": 5
      title: Spectre d’un opérateur compact
      page: 89
      pdf_page: 103
    - "no": 6
      title: Cas des espaces hilbertiens
      page: 92
      pdf_page: 106
    - "no": 7
      title: Le théorème de Krein–Rutman
      page: 93
      pdf_page: 107
statements: 36
exercises: 30
content_sha256: 0b4a1f35a2c9ae551613fb1073dcd1d3eca2dfb2aefcf71da2e900fb42943f61
---

## § 6. PROPRIÉTÉS SPECTRALES DES ENDOMORPHISMES DES ESPACES DE BANACH

Sauf mention du contraire, les espaces vectoriels considérés dans ce paragraphe sont des espaces vectoriels sur $\mathbf{C}$. Le spectre d’un endomorphisme d’un espace normable complet E est le spectre relatif à l’algèbre unifère $\mathscr{L}(E) ($cf. n$^o7$ de I, p. 127).

### 1. Points isolés et points sensibles du spectre

Soit E un espace normable complet et soit $u$ un endomorphisme de E. Soit $\lambda$ un point isolé du spectre de $u$. On rappelle qu’on note $e_{\lambda}(u)$ le projecteur spectral associé à $u$ et à l’ensemble fermé et ouvert $\{\lambda \}$ du spectre de $u$ (n$^o3$ de I, p. 131). L’endomorphisme $u-\lambda 1_E$ induit un automorphisme de Ker($e_{\lambda}(u)$) et un endomorphisme quasi-nilpotent de Im($e_{\lambda}(u)$) $($loc. cit.).

#### Définition 1 {#ts-iii-s6-def-1 .statement tag=02UE}

On dit que $\lambda$ est de multiplicité spectrale finie pour $u$ si le projecteur spectral $e_{\lambda}(u)$ est de rang fini ; dans ce cas, l’entier $m_{\lambda}(u) =$ dim(Im($e_{\lambda}(u)$)) s’appelle la multiplicité spectrale de $\lambda$ pour $u$.

#### Définition 2 {#ts-iii-s6-def-2 .statement tag=02UF}

On appelle points sensibles du spectre de $u$ les points isolés de Sp($u$) de multiplicité spectrale finie. L’ensemble des points sensibles de Sp($u$) s’appelle le spectre sensible de $u$ et se note Sp$_s(u)$.[^1] On appelle spectre essentiel de $u$ et on note Sp$_e(u)$ l’ensemble complémentaire Sp($u$) - Sp$_s(u)$.

Comme l’ensemble Sp$_s(u)$ se compose de points isolés de Sp($u$), il est ouvert dans Sp($u$), discret, et dénombrable (III, p. 78, lemme 3) ; il est aussi borné. L’ensemble Sp$_e(u)$ est fermé dans Sp($u$), donc compact.

D’après la prop. 14 de III, p. 54, les points sensibles du spectre de $u$ sont les nombres complexes $\lambda$ tels que $u-\lambda 1_E$ soit un endomorphisme de Riesz de E qui n’est pas un automorphisme de E.

Pour tout nombre complexe $\lambda$, on note $N_{\lambda}(u)$ et $I_{\lambda}(u)$ le nilespace et le conilespace de l’endomorphisme $u-\lambda 1_E$ de E. Puisque E est un espace de Fréchet, $u-\lambda 1_E$ est un endomorphisme de Riesz si et seulement si $N_{\lambda}(u)$ est de dimension finie et $I_{\lambda}(u)$ est de codimension finie (prop. 13 de III, p. 53) ; lorsque c’est le cas, $u-\lambda 1_E$ est inversible si et seulement si $N_{\lambda}(u)$ est réduit à 0 (III, p. 47, prop. 6). Les points sensibles du spectre de $u$ sont donc les nombres complexes $\lambda$ tels que $N_{\lambda}(u)$ soit de dimension finie non nulle et $I_{\lambda}(u)$ soit de codimension finie dans E (III, p. 54, prop. 14). La multiplicité spectrale $m_{\lambda}(u)$ de $\lambda$ est alors la dimension de $N_{\lambda}(u)$, l’endomorphisme $u-\lambda 1_E$ définit par restriction un automorphisme de $I_{\lambda}(u)$ et un endomorphisme nilpotent de $N_{\lambda}(u)$. Comme $N_{\lambda}(u)$ n’est pas réduit à 0, il en découle que $\lambda$ est une valeur propre de $u$. Le plus petit entier $n\geqslant 1$ tel que Ker(($u-\lambda 1_E$)$^n)$ soit égal à $N_{\lambda}(u)$ est l’ordre du pôle de la résolvante de $u$ au point $\lambda$ (n$^o3$ de I, p. 131), qui est majoré par $m_{\lambda}(u)$.

En particulier, on a donc démontré :

#### Proposition 1 {#ts-iii-s6-prop-1 .statement tag=02UG}

Les points sensibles du spectre de $u$ sont des valeurs propres de multiplicité spectrale finie.

Le spectre essentiel de $u$ se compose des nombres complexes $\lambda$ tels que $u-\lambda 1_E$ ne soit pas un endomorphisme de Riesz de E. En particulier, si $u$ est compact, alors tout $\lambda \in$ Sp($u$)$-\{0\}$ est un point sensible du spectre (cor. 2 de III, p. 77).

#### Proposition 2 {#ts-iii-s6-prop-2 .statement tag=02UH}

Soient E un espace normable complet et $u$ un endomorphisme de E. Soit H une partie finie de Sp$_s(u)$. L’ensemble H est ouvert et fermé dans Sp($u$). Le projecteur spectral $e_H(u)$ est de rang fini, a pour image $\sum_{\lambda\in H}N_{\lambda}(u)$ et pour noyau $\bigcap_{\lambda\in H}I_{\lambda}(u)$.

Cela résulte du n$^o3$ de I, p. 131 puisque, pour tout $\lambda \in$ Sp$_s(u)$, les sous-espaces $N_{\lambda}(u)$ et $I_{\lambda}(u)$ sont respectivement l’image et le noyau du projecteur spectral $e_{\lambda}(u)$.

#### Corollaire 1 {#ts-iii-s6-prop-2-cor-1 .statement tag=02UI}

Soit V un voisinage de Sp$_e(u)$.

a) Il existe une décomposition de E en somme directe topologique $F\oplus$ G telle que F soit de dimension finie, que F et G soient stables par tout endomorphisme permutable à $u$, et que le spectre de l’endomorphisme de G déduit de $u$ soit contenu dans V ;

b) Supposons V non vide. Il existe un élément $v$ du bicommutant de $u$ dans $\mathscr{L}(E)$ dont le spectre est contenu dans V et tel que $v-u$ soit de rang fini.

Posons H = Sp($u$)$\cap (\mathbf{C}-\mathring{V})$. L’ensemble H est contenu dans Sp$_s(u)$, donc est discret ; comme il est fermé dans l’espace compact Sp($u$), il est fini. On peut prendre pour F et G l’image et le noyau du projecteur spectral $e_H(u)$ (prop. 2).

Supposons que V n’est pas vide. Soit $\mu\in V$ et notons $v$ l’endomorphisme de E qui coïncide avec l’homothétie de rapport $\mu$ dans F et avec $u$ dans G. Son spectre est contenu dans $\{\mu\} \cup$ (Sp($u$) - H), donc dans V, et $v-u$ est de rang fini puisque F est de dimension finie.

Pour toute partie compacte S de $\mathbf{C}$, on note $\mathscr{O}(S)$ l’algèbre des germes de fonctions holomorphes au voisinage de S et à valeurs dans $\mathbf{C}$ (I, p. 49, §4, n$^o1)$.

#### Corollaire 2 {#ts-iii-s6-prop-2-cor-2 .statement tag=02UJ}

Soit $f\in \mathscr{O}$(Sp($u$)) et soit $\mu$ un nombre complexe. Soit H l’ensemble des $\lambda \in$ Sp($u$) tels que $f(\lambda ) =\mu$. Alors $\mu$ est un point sensible du spectre de $f(u)$ si et seulement si H est fini, non vide, et contenu dans le spectre sensible de $u$. Sous ces conditions, le projecteur spectral $e_\mu(f(u))$ est égal au projecteur $e_H(u)$ associé à $u$ et H. On a

$$
N_\mu(f(u)) =\bigoplus_{\lambda\in H}N_{\lambda}(u),I_\mu(f(u)) =\bigcap_{\lambda\in H}I_{\lambda}(u)
$$

et la multiplicité spectrale de $\mu$ pour $f(u)$ est la somme des multiplicités spectrales des éléments de H, c’est-à-dire

$$
m_\mu(f(u)) =\sum_{\lambda\in H}m_{\lambda}(u)
$$

Le nombre complexe $\mu$ appartient à $f$(Sp($u$)), et donc au spectre de $f(u)$ (prop. 8 de I, p. 75), si et seulement si H n’est pas vide. On a alors $e_\mu(f(u)) =e_H(u)$ (n$^o1$ de I, p. 127). Les autres assertions s’en déduisent par la prop. 2.

#### Exemple 1 {#ts-iii-s6-n1-exa-1 .statement tag=02UK}

Soient E un espace vectoriel de dimension finie et $u$ un endomorphisme de E. Le spectre de $u$ est fini et coïncide avec Sp$_s(u)$. Ses éléments sont les racines du polynôme caractéristique $\chi_u$ de $u$; ce sont les valeurs propres de $u$. La multiplicité spectrale $m_{\lambda}(u)$ d’un élément $\lambda \in$ Sp($u$) est la multiplicité de $\lambda$ comme racine du polynôme $\chi_u$ (A, VII, p. 36, cor.). D’après le cor. 2 ci-dessus, on a

$$
\chi_{f(u)}(T) =\prod_{\lambda\in Sp(u)}(T-f(\lambda ))^{m_{\lambda}}
$$

pour tout $f\in \mathscr{O}$(Sp($u$)). Cela généralise la prop. 10 de A, VII, p. 36.

#### Exemple 2 {#ts-iii-s6-n1-exa-2 .statement tag=02UL}

Soient X une partie compacte de $\mathbf{C}$ et $\mathscr{C}(X)$ l’espace de Banach des fonctions continues sur X à valeurs complexes. Notons $u$ l’endomorphisme de $\mathscr{C}(X)$ qui à $f\in \mathscr{C}(X)$ associe la fonction $z\mapsto zf(z)$ de $\mathscr{C}(X)$. Le spectre de $u$ est égal à X, ses points sensibles sont les points isolés de X et leurs multiplicités spectrales sont égales à 1.

### 2. Une partition du spectre

Notons $\overline{\mathbf{Z}}$ le sous-ensemble $\mathbf{Z}\cup  \{-\infty ,+\infty \}$ de $\overline{\mathbf{R}}$. Si $u$ est une application linéaire dont le noyau ou le conoyau est de dimension finie, on appelle indice de $u$ l’élément ind($u$) de $\overline{\mathbf{Z}}$ défini par

ind($u$) $=$ dim Coker($u$)$-$ dim Ker($u$)

(cf. n$^o6$ de III, p. 67).

#### Définition 3 {#ts-iii-s6-def-3 .statement tag=02UM}

Soient E un espace normable complet et $u$ un endomorphisme de E. Pour tout $n\in \overline{\mathbf{Z}}$, on note Sp$_n(u)$ l’ensemble des nombres complexes $\lambda \in$ Sp$_e(u)$ tels que $u-\lambda 1_E$ soit un morphisme strict, dont le noyau ou le conoyau est de dimension finie, et dont l’indice est $n$. On note Sp$_{\omega}(u)$ le complémentaire dans Sp$_e(u)$ de l’union des sous-ensembles Sp$_n(u)$ pour $n\in \mathbf{Z}$.

Les ensembles Sp$_s(u)$, Sp$_n(u)$ pour $n\in \overline{\mathbf{Z}}$ et Sp$_{\omega}(u)$ forment une partition du spectre de $u$.

Tout endomorphisme de E dont le conoyau est de dimension finie est strict (III, p. 52, lemme 6). Les endomorphismes de Fredholm de E sont les endomorphismes de E dont le noyau et le conoyau sont de dimension finie (III, p. 52, prop. 11). L’ensemble $\mathbf{C}-$ Sp$_e(u)$ se compose des $\lambda \in \mathbf{C}$ tels que $u-\lambda 1_E$ soit un endomorphisme de Riesz de E, et un tel endomorphisme est un endomorphisme de Fredholm de E d’indice 0.

Par suite, pour $\lambda \in \mathbf{C}$ et pour $n\in \mathbf{Z}-\{0\}$, on a :

$\lambda \in \mathbf{C}-$ Sp($u$)$\Leftarrow \Rightarrow u-\lambda 1_E$ est un automorphisme ;

$\lambda \in$ Sp$_s(u)\Leftarrow \Rightarrow u-\lambda 1_E$ est un endomorphisme de Riesz, mais

n’est pas un automorphisme ;

$\lambda \in$ Sp$_0(u)\Leftarrow \Rightarrow u-\lambda 1_E$ est un endomorphisme de Fredholm

d’indice 0 de E mais n’est pas un endomorphisme de Riesz de E ;

$\lambda \in$ Sp$_n(u)\Leftarrow \Rightarrow u-\lambda 1_E$ est un endomorphisme de Fredholm

$(n\not = 0)$ d’indice $n$ de E ;

$\lambda \in$ Sp$_{-\infty}(u)\Leftarrow \Rightarrow u-\lambda 1_E$ est strict, son noyau est de dimension

infinie et son conoyau est de dimension finie ; $\lambda \in$ Sp$_{+\infty}(u)\Leftarrow \Rightarrow u-\lambda 1_E$ est strict, son noyau est de dimension

finie et son conoyau est de dimension infinie ; $\lambda \in$ Sp$_{\omega}(u)\Leftarrow \Rightarrow$ soit $u-\lambda 1_E$ n’est pas strict, soit son noyau

et son conoyau sont de dimension infinie.

#### Remarque {#ts-iii-s6-n2-rem-1 .statement tag=02UN}

Notons $\pi$ l’homomorphisme canonique de $\mathscr{L}(E)$ sur l’algèbre de Calkin $\mathscr{C}$alk(E) de E (cf. n$^o4$ de III, p. 75). Le spectre de $\pi (u)$ relativement à l’algèbre $\mathscr{C}$alk(E) est parfois appelé le spectre stable de $u$. Ses éléments sont les nombres complexes $\lambda$ tels que $u-\lambda 1_E$ ne soit pas un endomorphisme de Fredholm de E (cor. 1 du th. 3 de III, p. 73). Il est donc égal à Sp$_{\omega}(u)\cup$ Sp$_{-\infty}(u)\cup$ Sp$_{+\infty}(u)$.

Soit A l’ensemble des endomorphismes de E permutables à $u$. L’adhérence B de $\pi (A)$ dans $\mathscr{C}$alk(E) est une algèbre normable complète et le spectre de $\pi (u)$ relativement à B est le spectre essentiel Sp$_e(u)$ de $u$ (III, p. 77, prop. 3). D’après le cor. de la prop. 6 de I, p. 28, appliqué à la sous-algèbre B de $\mathscr{C}$alk(E), l’ensemble Sp$_e(u)$ est la réunion de Sp$_{\omega}(u)\cup$ Sp$_{-\infty}(u)\cup$ Sp$_{+\infty}(u)$ et de certaines composantes connexes bornées de son complémentaire.

#### Théorème 1 {#ts-iii-s6-thm-1 .statement tag=02UO}

Soient E un espace normable complet et $u$ un endomorphisme de E.

a) L’ensemble Sp$_{\omega}(u)$ est compact. Il n’est pas vide si E est de dimension infinie;

b) Soit $n\in \overline{\mathbf{Z}}$. L’ensemble Sp$_n(u)$ est réunion d’une famille de composantes connexes bornées de $\mathbf{C}-$ Sp$_{\omega}(u)$. Il est ouvert dans $\mathbf{C}$, et sa frontière dans $\mathbf{C}$ est contenue dans Sp$_{\omega}(u)$.

L’ensemble $\mathbf{C}-$ Sp$_{\omega}(u)$ se compose des nombres complexes $\lambda \in \mathbf{C}$ tels que $u-\lambda 1_E$ soit un morphisme strict, dont le noyau ou le conoyau est de dimension finie. D’après les prop. 11 de III, p. 67 et 13 de III, p. 70, il est ouvert. L’ensemble Sp$_{\omega}(u)$ est donc fermé. Comme il est borné, il est compact.

Démontrons b). Soit $n\in \overline{\mathbf{Z}}$. L’ensemble Sp$_n(u)$ est contenu dans $\mathbf{C}-$Sp$_{\omega}(u)$. Soit U une composante connexe de $\mathbf{C}-$ Sp$_{\omega}(u)$ qui rencontre Sp$_n(u)$. L’application $\lambda \mapsto$ ind($u-\lambda 1_E$) de $\mathbf{C}-$ Sp$_{\omega}(u)$ dans $\overline{\mathbf{Z}}$ étant localement constante (cor. 1 de la prop. 12 de III, p. 68 et cor. 1 de la prop. 13 de III, p. 70), l’indice de $u-\lambda 1_E$ est égal à $n$ pour tout $\lambda \in U$. Si $n\not = 0$, cela implique que U est contenu dans Sp$_n(u)$. Si $n= 0$, remarquons que l’ensemble U est une composante connexe de $\mathbf{C}-$ (Sp$_{\omega}(u)\cup$ Sp$_{-\infty}(u)\cup$ Sp$_{+\infty}(u))$. Puisque U rencontre Sp$_0(u)$ et donc Sp$_e(u)$, il résulte alors de la remarque 2 que l’ensemble U est contenu dans Sp$_e(u)$, et par suite dans Sp$_0(u)$. On conclut dans tous les cas que Sp$_n(u)$ est la réunion des composantes connexes de $\mathbf{C}-$ Sp$_{\omega}(u)$ qui rencontrent Sp$_n(u)$. Celles-ci sont nécessairement bornées puisque l’ensemble Sp($u$) est borné. Par suite, Sp$_n(u)$ est ouvert dans $\mathbf{C}$ et sa frontière est contenue dans Sp$_{\omega}(u)$. Cela démontre b).

Supposons finalement que l’ensemble Sp$_{\omega}(u)$ est vide. D’après b), chacun des ensembles Sp$_n(u)$, pour $n\in \overline{\mathbf{Z}}$, est alors vide. On a donc Sp($u$) $=$ Sp$_s(u)$. Le spectre de $u$ est par conséquent discret et compact, donc fini, et comme tous ses points sont de multiplicité spectrale finie, l’espace vectoriel E est de dimension finie (III, p. 83, prop. 2). Cela termine la démonstration de a).

#### Corollaire {#ts-iii-s6-n2-cor-1 .statement tag=02UP}

a) Soit Ω la composante connexe non bornée de $\mathbf{C}-$ Sp$_{\omega}(u)$. On a $\Omega \cap$ Sp($u$)$\subset$ Sp$_s(u)$;

b) Tout point adhérent à Sp$_s(u)$ qui n’appartient pas à Sp$_s(u)$ appartient à Sp$_{\omega}(u)$.

L’assertion a) est une conséquence directe de l’assertion b) du th. 1. Soit $\lambda$ un point adhérent à Sp$_s(u)$ qui n’appartient pas à Sp$_s(u)$. Il appartient au spectre de $u$, puisque celui-ci est fermé. Il n’appartient à aucun des ensembles Sp$_n(u)$, pour $n\in \overline{\mathbf{Z}}$, puisque ceux-ci sont ouverts (loc. cit.) et disjoints de Sp$_s(u)$. On a donc $\lambda \in$ Sp$_{\omega}(u)$, d’où b).

#### Proposition 3 {#ts-iii-s6-prop-3 .statement tag=02UQ}

Soient E et F des espaces normables complets, $u: E\rightarrow F$ et $v: F\rightarrow E$ des applications linéaires continues.

a) Les traces sur $\mathbf{C}-\{0\}$ des ensembles Sp($v\circ u$) et Sp($u\circ v$) $($resp. Sp$_s(v\circ u)$ et Sp$_s(u\circ v)$, resp. Sp$_n(v\circ u)$ et Sp$_n(u\circ v)$ pour $n\in \overline{\mathbf{Z}}$, resp. Sp$_{\omega}(v\circ u)$ et Sp$_{\omega}(u\circ v))$ sont égales ;

b) Soit $\lambda$ un élément de Sp$_s(v\circ u)$ distinct de 0. Les multiplicités spectrales de $\lambda$ pour $v\circ u$ et pour $u\circ v$ sont égales.

Soit $\mu$ un nombre complexe non nul et soit $n\in \overline{\mathbf{Z}}$. Pour que $\mu1_E-v\circ u$ soit un automorphisme (resp. un endomorphisme de Riesz, resp. un morphisme strict dont le noyau ou le conoyau est de dimension finie et dont l’indice est $n)$, il faut et il suffit que $\mu1_F-u\circ v$ en soit un (III, p. 49, prop. 10). L’assertion a) résulte alors des définitions.

Soit $\lambda$ un point de Sp$_s(v\circ u)$ distinct de 0. On a

dim Ker(($\lambda 1_E-v\circ u$)$^n) =$ dim Ker(($\lambda 1_F-u\circ v$)$^n)$

pour tout $n\geqslant 0 ($loc. cit.), donc les multiplicités spectrales de $\lambda$ pour $v\circ u$ et $u\circ v$ sont égales.

### 3. Spectre du transposé d’un endomorphisme

#### Proposition 4 {#ts-iii-s6-prop-4 .statement tag=02UR}

Soient E un espace normable complet, $E'$ l’espace dual de E et $u$ un endomorphisme de E.

a) On a Sp$_s(u) =$ Sp$_s(^tu)$, Sp$_n(u) =$ Sp$_{-n}(^tu)$ pour tout $n\in \overline{\mathbf{Z}}$ et Sp$_{\omega}(u) = Sp_{\omega}(^tu)$;

b) Tout point de Sp$_s(u)$ a même multiplicité spectrale pour $u$ et pour $^tu$.

L’assertion a) de la prop. 3 de I, p. 131 démontre que Sp($u$) $=$ Sp($^tu$), et l’assertion c) de loc. cit. implique que Sp$_s(u) =$ Sp$_s(^tu)$ et que l’assertion b) est valide.

Pour tout $\lambda \in \mathbf{C}$, le lemme 4 de III, p. 69 implique que $u-\lambda 1_E$ est un morphisme strict si et seulement si $^tu-\lambda 1_{E'}$ en est un, et que

dim Coker($^t(u-\lambda 1_E)$) $=$ dim Ker($u-\lambda 1_E$)

dim Ker($^t(u-\lambda 1_E)$) $=$ dim Coker($u-\lambda 1_E$)

dans $\overline{\mathbf{Z}}$. L’assertion a) en résulte, compte tenu des définitions des diverses parties du spectre (déf. 3 de III, p. 85).

### 4. Perturbation par un opérateur compact

#### Théorème 2 {#ts-iii-s6-thm-2 .statement tag=02US}

Soient E un espace normable complet, $u$ un endomorphisme de E et $h$ un endomorphisme compact de E. On a Sp$_{\omega}(u+h) =$ Sp$_{\omega}(u)$ et Sp$_n(u+h) =$ Sp$_n(u)$ pour tout $n\in \overline{\mathbf{Z}}-\{0\}$.

Soit $\lambda \in \mathbf{C}$. Pour que $u+h-\lambda 1_E$ soit un morphisme strict dont le noyau (resp. le conoyau) est de dimension finie, il faut et il suffit que $u-\lambda 1_E$ le soit, d’après le th. 1 de III, p. 72 (resp. le th. 2 de III, p. 73).

Les égalités

Sp$_{-\infty}(u+h) =$ Sp$_{-\infty}(u)$, Sp$_{+\infty}(u+h) =$ Sp$_{+\infty}(u)$,

Sp$_{\omega}(u+h) =$ Sp$_{\omega}(u)$

en résultent. Par ailleurs, on a Sp$_n(u+h) =$ Sp$_n(u)$ d’après le th. 3 de III, p. 73 pour tout $n\in \mathbf{Z}-\{0\}$.

#### Corollaire {#ts-iii-s6-n4-cor-1 .statement tag=02UT}

Supposons que la composante connexe non bornée du complémentaire de Sp$_{\omega}(u)$ contienne 0. Alors $u+h$ est un endomorphisme de Riesz de E.

On a Sp$_{\omega}(u+h) =$ Sp$_{\omega}(u)$ (th. 2), donc 0 appartient à la composante connexe non bornée de $\mathbf{C}-$ Sp$_{\omega}(u+h)$. D’après le cor. du th. 1 de III, p. 87, ou bien 0 n’appartient pas au spectre de $u+h$, ou bien c’est un point sensible de ce spectre. Dans les deux cas, $u+h$ est un endomorphisme de Riesz de E.

### 5. Spectre d’un opérateur compact

#### Lemme 1 {#ts-iii-s6-lem-1 .statement tag=02UU}

Soit E un espace vectoriel topologique séparé de dimension $\geqslant 2$ sur $\mathbf{R}$ et soit X une partie dénombrable de E. L’ensemble complémentaire E - X est connexe.

Supposons d’abord que E est de dimension 2. On peut supposer que $E =\mathbf{R}^2$ muni de la norme euclidienne (EVT, I, p. 14, th. 2). Puisque X est dénombrable, il existe un nombre réel $r\in \mathbf{R}_+^*$ tel que le cercle C de centre 0 et de rayon $r$ ne rencontre pas X. Soit $x\in E$ - X ; si $x /\in C$, il existe un point $y\in C$ tel que la droite $L_x$ joignant $x$ et $y$ ne rencontre pas X, puisque X est dénombrable. L’ensemble E - X est la réunion de C, qui est connexe, et des ensembles connexes $L_x\cup C$ pour $x\in E$- $(X\cup C)$; ces ensembles contiennent tous C, et donc E- X est connexe (TG, I, p. 81, prop. 2).

Considérons le cas général. En remplaçant X par $X-x$ pour un élément $x\in E$ - X, on se ramène au cas où $0\in /X$. Comme E - X est la réunion des ensembles F - $(X\cap F)$ lorsque F parcourt l’ensemble des sous-espaces de dimension 2 de E, et que ceux-ci sont connexes d’après le cas précédent et contiennent 0, l’ensemble E - X est connexe (loc. cit.).

#### Lemme 2 {#ts-iii-s6-lem-2 .statement tag=02UV}

Soit $S\subset \mathbf{C}$ un ensemble infini, discret, borné et fermé dans $\mathbf{C}-\{0\}$. Alors S est l’ensemble des valeurs d’une suite $(\lambda_n)_{n\in\mathbf{N}}$ de nombres complexes non nuls, deux à deux distincts, telle que la suite $(|\lambda_n|)_{n\in\mathbf{N}}$ soit décroissante et converge vers 0.

Pour tout entier $i\geqslant 1$, l’ensemble $A_i$ des nombres complexes $\lambda \in S$ tels que $|\lambda |\geqslant \frac{1}{i}$ est compact et discret dans $\mathbf{C}$, donc fini. Notons $a_i$ son cardinal. Comme S est infini, la suite $(a_i)$ tend vers $+\infty$. Posons $A_0=\emptyset$ et $a_0= 0$. Pour tout $i\geqslant 1$, choisissons une bijection $n\mapsto \lambda_n$ de l’intervalle $[a_{i-1}, a_i[$ de $\mathbf{N}$ sur $A_i-A_{i-1}$ telle que l’application $n\mapsto  |\lambda_n|$ soit décroissante sur $[a_{i-1}, a_i[$. La suite $(\lambda_n)_{n\in\mathbf{N}}$ vérifie les propriétés demandées.

Soit E un espace normable complet de dimension infinie. L’algèbre $\mathscr{L}^c(E)$ est une sous-algèbre non unifère de $\mathscr{L}(E)$. Rappelons que pour tout endomorphisme compact $u\in \mathscr{L}^c$(E), le spectre Sp$'_{\mathscr{L}^c(E)}(u)$ est le spectre de $u$ relativement à la sous-algèbre unifère $\mathscr{L}^c(E)\oplus \mathbf{C}1_E$ de $\mathscr{L}(E) ($I, p. 4, n$^o4$).

#### Proposition 5 {#ts-iii-s6-prop-5 .statement tag=02UW}

Soit E un espace normable complet et soit $u$ un endomorphisme compact de E. Tout élément de Sp$_s(u)$ est une valeur propre de multiplicité spectrale finie. De plus :

a) Si E est de dimension finie, alors Sp($u$) $=$ Sp$_s(u)$;

b) Si E est de dimension infinie, alors Sp$_s(u) =$ Sp($u$)$-\{0\}$ et Sp$_{\omega}(u) =\{0\}$;

c) Si Sp$_s(u)$ est infini, c’est l’ensemble des valeurs d’une suite $(\lambda_n)_{n\in\mathbf{N}}$ de nombres complexes non nuls, deux à deux distincts, telle que la suite $(|\lambda_n|)_{n\in\mathbf{N}}$ soit décroissante et converge vers 0 ;

d) Si E est de dimension infinie, alors Sp($u$) $=$ Sp$'_{\mathscr{L}^c(E)}(u)$.

Tout élément de Sp$_s(u)$ est une valeur propre de multiplicité spectrale finie (prop. 1 de III, p. 83).

L’assertion a) est élémentaire (III, p. 85, exemple 1). Supposons maintenant que E est de dimension infinie.

Soit $\lambda \in$ Sp($u$)$-\{0\}$. Alors $u-\lambda 1_E$ est un endomorphisme de Riesz de E (cor. 2 de la prop. 2 de III, p. 75), donc $\lambda$ appartient à Sp$_s(u)$. Si E est de dimension infinie, alors Sp$_{\omega}(u)$ n’est pas vide (III, p. 87, th. 1, a)). On a nécessairement Sp$_{\omega}(u) =\{0\}$, d’où b).

L’ensemble Sp$_s(u)$ est discret et borné. Par ailleurs, on a Sp$_s(u) =$ Sp($u$)$\cap (\mathbf{C}-\{0\})$ d’après b), donc Sp$_s(u)$ est fermé dans $\mathbf{C}-\{0\}$. L’assertion c) résulte donc du lemme 2.

Le spectre de $u$ est dénombrable, et son complémentaire dans $\mathbf{C}$ est donc connexe (lemme 1). D’après le cor. de la prop. 6 de I, p. 28, appliqué à la sous-algèbre unifère $\mathscr{L}^c(E)\oplus \mathbf{C}1_E$ de $\mathscr{L}$ (E), on conclut que Sp($u$) $=$ Sp$'_{\mathscr{L}^c(E)}(u)$.

#### Proposition 6 {#ts-iii-s6-prop-6 .statement tag=02UX}

Soient E un espace normable complet sur $\mathbf{C}$ et $u$ un endomorphisme compact de E.

a) Soit $f\in \mathscr{O}$(Sp($u$)) telle que $f(0) = 0$. L’endomorphisme $f(u)$ est compact ;

b) Supposons que E est un espace hilbertien complexe et que $u$ est normal. Soit $f$ une fonction continue sur Sp($u$) telle que $f(0) = 0$. L’endomorphisme normal $f(u)$ est compact.

De plus, les assertions réciproques sont valides si E est de dimension infinie et la condition $f(0) = 0$ n’est pas nécessaire si E est de dimension finie.

On peut supposer que E est de dimension infinie.

Démontrons a) et sa réciproque. L’endomorphisme $u$ est un élément de l’algèbre de Banach $\mathscr{L}^c(E)$. Puisque E est de dimension infinie, on a l’égalité Sp($u$) $=$ Sp$'_{\mathscr{L}^c(E)}(u)$ d’après la prop. 5, d). L’élément $f(u)$ du calcul fonctionnel holomorphe de l’algèbre de Banach unifère déduite de $\mathscr{L}^c(E)$ par adjonction d’un élément unité appartient à $\mathscr{L}^c(E)$ si et seulement si $f(0) = 0 ($I, p. 88). Mais par ailleurs cet élément coïncide avec l’élément $f(u)$ de $\mathscr{L}(E)$ (prop. 7 de I, p. 75), donc $f(u)$ est compact si et seulement si $f(0) = 0$.

La preuve de l’assertion b) et de sa réciproque est toute identique en considérant le calcul fonctionnel continu de l’algèbre stellaire $\mathscr{L}^c(E)$ (I, p. 110, déf. 5).

#### Corollaire {#ts-iii-s6-n5-cor-1 .statement tag=02UY}

Soient E et F des espaces hilbertiens et soit $u$ une application linéaire continue de E dans F. L’application linéaire $u$ est compacte si et seulement si l’endomorphisme $|u|$ de E est compact.

Soit $(j,|u|)$ la décomposition polaire de $u$ (déf. 4 de I, p. 140). Puisque

$$
\surd
$$

$u=j|u|$ et $|u|=u^*u$ (prop. 10 de I, p. 139), l’équivalence résulte de la prop. 3 de III, p. 5 et de l’assertion b) de la proposition précédente.

### 6. Cas des espaces hilbertiens

Dans ce numéro, E désigne un espace hilbertien sur $\mathbf{C}$. On note $\pi$ l’homomorphisme canonique de $\mathscr{L}(E)$ sur l’algèbre stellaire $\mathscr{C}$alk(E).

#### Proposition 7 {#ts-iii-s6-prop-7 .statement tag=02UZ}

Soit $u\in \mathscr{L}(E)$.

a) Si $u$ est normal, alors $u$ est un endomorphisme de Riesz si et seulement si $u$ est un endomorphisme de Fredholm d’indice 0.

b) Si $u$ est hermitien, alors $u$ est un endomorphisme de Fredholm si et seulement si $u$ est un endomorphisme de Riesz.

Tout endomorphisme de Riesz est un endomorphisme de Fredholm d’indice 0 (proposition 5 de III, p. 46). Réciproquement, supposons que $u$ est un endomorphisme de Fredholm d’indice 0, et que $u$ est normal. Son nilespace coïncide alors avec son noyau (EVT, V, p. 43, prop. 8), et est donc de dimension finie. Il résulte alors du lemme 2 de III, p. 45 et de la définition que $u$ est un endomorphisme de Riesz.

Démontrons b). D’après a), il suffit de vérifier que l’indice d’un endomorphisme de Fredholm hermitien $u$ est nul. Mais l’orthogonal de l’image de $u$ (qui est fermée) est alors égal au noyau de $u$ (EVT, V, p. 41, prop. 4), d’où l’assertion.

#### Corollaire {#ts-iii-s6-n6-cor-1 .statement tag=02V0}

Soit $u\in \mathscr{L}(E)$. Si $u$ est normal, alors Sp$_0(u)$ est vide, et si $u$ est hermitien, alors Sp$_e(u)$ coïncide avec le spectre de $\pi (u)$ relatif à l’algèbre $\mathscr{C}$alk(E).

Les deux assertions résultent de la proposition et de la définition des ensembles Sp$_n(u)$ pour $n\in \overline{\mathbf{Z}}$ et de Sp$_{\omega}(u)$, qui forment une partition du spectre essentiel de $u$ (déf. 2 de III, p. 83).

#### Théorème 3 (Weyl) {#ts-iii-s6-thm-3 .statement tag=02V1}

Soit $u\in \mathscr{L}(E)$ un endomorphisme normal de $u$. Le spectre essentiel de $u$ est l’intersection des ensembles Sp($u+h$) pour $h$ parcourant $\mathscr{L}^c(E)$.

Soit $h\in \mathscr{L}^c(E)$. Comme Sp$_0(u)$ est vide (corollaire ci-dessus), le théorème 2 de III, p. 89 implique que Sp$_e(u+h) =$ Sp$_e(u)$. L’intersection des ensembles Sp($u+h$) contient donc Sp$_e(u)$.

Soit $\lambda \in$ Sp$_s(u)$. Notons $E_{\lambda}$ le sous-espace propre de $u$ relatif à $\lambda$, et $F_{\lambda}$ l’image du projecteur spectral associé à $u$ et $\mathbf{C}-\{\lambda \}$. L’espace E est somme directe topologique de $E_{\lambda}$ et $F_{\lambda}$. Soit $h$ l’endomorphisme de rang fini de E qui est nul sur $F_{\lambda}$ et coïncide sur $E_{\lambda}$ avec l’identité. L’endomorphisme $u+h$ est inversible, donc $\lambda  /\in$ Sp($u+h$). Le théorème en résulte.

Ainsi, si $u$ est un endomorphisme normal de E, et si $h\in \mathscr{L}^c$(E), le spectre de $u+h$ ne peut différer du spectre de $u$ que par des points isolés qui sont de multiplicité spectrale finie.

### 7. Le théorème de Krein–Rutman

#### Lemme 3 {#ts-iii-s6-lem-3 .statement tag=02V2}

Soit $(a_n)_{n\geqslant 0}$ une suite de nombres réels positifs tels que la série entière

$$
f(z) =\sum_{n\geqslant 0}a_nz^n
$$

ait un rayon de convergence fini $r >0$. Soit $D\subset \mathbf{C}$ le disque ouvert de centre 0 et de rayon $r$. Il n’existe pas de fonction holomorphe $\widetilde{f}$ définie sur un voisinage ouvert U de $r$ dans $\mathbf{C}$ qui coïncide avec $f$ sur $U\cap D$.

Supposons qu’il existe une telle fonction holomorphe $\widetilde{f}$ définie sur un voisinage ouvert U de $r$. Il existe des nombres réels $s < r$ et $\delta  >0$ tels que $s+\delta  > r$ et que le disque ouvert $D'$ de centre $s$ et de rayon $\delta$ est contenu dans U. Le développement en série entière de $\widetilde{f}$ au point $s$ (VAR, R1, p. 26, 3.2.1) converge alors pour tout $z$ dans le disque de centre 0 et de rayon $\delta$ (VAR, R1, p. 29, 3.3.4). Cette série est

$+\infty (n)+\infty (n)$

$\widetilde{f}_s(z) =\sum\widetilde{f}n$!$(s)z_n=\sum fn$!$(s)z_n$

$n=0n=0$ (VAR, R1, p. 27, 3.2.4). Comme $s\in D$, on a

$$
f^{(n)}(s) =\sum_{k=n}^{+\infty}k(k-1)\cdots (k-n+ 1)a_ks^{k-n}
$$

(VAR, R1, p. 28, 3.2.11). Prenons $z$ tel que $0< z < \delta$. Puisque $a_k\geqslant 0$, on a

$\widetilde{f}_s(z) =\sum^{+\infty}(\sum^{+\infty}k(k-1)\cdots n($!$k-n+ 1)a_ks_{k-n})z_n$

$n=0k=n$ $+\infty k+\infty$

$=\sum(a_k\sum n$!($kk-$! $n$)! $s^{k-n}z^n)=\sum a_k(s+z)^k$

$k=0n=0k=0$

(TG, III, p. 40). Lorsque $s+z > r$, la convergence de cette expression contredit l’hypothèse selon laquelle le rayon de convergence de la série entière $f$ est égal à $r$.

Soit E un espace de Banach réel. Soit C un cône convexe pointé dans E. L’espace vectoriel engendré par C est égal à $C-C$ (EVT, II, p. 12, cor. 1). En particulier, le cône C est total dans E si et seulement $C-C$ est dense dans E. Rappelons que C est dit saillant si $C\cap (-C)$ est réduit à 0 (EVT, II, p. 11).

Le polaire $C^{\circ}$ de C est l’ensemble des formes linéaires continues $\ell \in E'$ telles que $\ell (x)\geqslant 0$ pour tout $x\in C$ (EVT, II, p. 47, prop. 4). D’après le théorème des bipolaires (EVT, II, p. 48, th. 1), si C est un cône fermé convexe pointé, on a $C^{\circ \circ}= C$.

#### Lemme 4 {#ts-iii-s6-lem-4 .statement tag=02V3}

Soit E un espace de Banach réel et $u\in \mathscr{L}(E_{(\mathbf{C})})$ un endomorphisme non nul de $E_{(\mathbf{C})}$. Soit C un cône convexe total dans E. Il existe $x\in C$ tel que $u(x)\not = 0$.

En effet, si $u$ s’annule sur C, alors $u$ s’annule sur $C-C$, donc sur E, et donc sur $E_{(\mathbf{C})}$.

#### Théorème 4 (Krein–Rutman) {#ts-iii-s6-thm-4 .statement tag=02V4}

Soit E un espace normable complet sur $\mathbf{R}$. Soit C un cône convexe fermé total saillant dans E et soit $u\in \mathscr{L}(E)$ une application linéaire compacte telle que $u(C)\subset C$. Si le rayon spectral $\varrho (u)$ est $>0$, alors $\varrho (u)$ est un point isolé du spectre de $u$, et il existe un vecteur propre non nul $x\in C$ de $u$ pour la valeur propre $\varrho (u)$.

Soit $E_{(\mathbf{C})}$ l’espace complexifié de E et $u_{(\mathbf{C})}$ l’endomorphisme de $E_{(\mathbf{C})}$ obtenu par extension des scalaires à partir de $u$. Le rayon spectral de $u_{(\mathbf{C})}$ est égal à $\varrho (u) ($I, p. 86) ; on le note simplement $\varrho$. Puisque $\varrho  >0$, le spectre complexe de $u$ n’est pas réduit à 0. Il existe donc $\lambda_0\in$ Sp$_s(u_{(\mathbf{C})})$ tel que $|\lambda_0|=\varrho$ (prop. 5 de III, p. 90). Soit $e_0$ le projecteur spectral de $u_{(\mathbf{C})}$ associé à $\lambda_0$.

La résolvante $\lambda \mapsto R(u_{(\mathbf{C})}, \lambda ) = (\lambda -u_{(\mathbf{C})})^{-1}$ est holomorphe sur le complémentaire du spectre de $u_{(\mathbf{C})}$ (th. 1 de I, p. 24). Le nombre complexe $\lambda_0$ est un pôle de la résolvante et son résidu est le projecteur spectral $e_0($I, p. 131).

Soient $y$ et $y'$ des éléments de E tels que $y+iy'\in E_{(\mathbf{C})}$ soit un vecteur propre de $u_{(\mathbf{C})}$ pour la valeur propre $\lambda_0$. Puisque $e_0(y+iy') =y+iy'\not = 0$, il existe un élément $x_0\in C$ tel que $e_0(x_0)\not = 0$ (lemme 4). Comme C est fermé et saillant, son polaire $C^{\circ}$ est total (EVT, II, p. 48, cor. 1), et il existe alors une forme linéaire $\ell_0\in C^{\circ}$ telle que $\langle e_0(x_0), \ell_0\rangle  \not = 0$.

Considérons la fonction $f$ définie par $f(0) = 0$ et par

$$
f(z) =\langle R(u_{(\mathbf{C})}, z^{-1})x_0, \ell_0\rangle
$$

pour $z\in \mathbf{C}$ tel que $z^{-1}\in /$ Sp($u_{(\mathbf{C})}$). Cette fonction vérifie

$$
f(z) =\ell_0((\sum^{+\infty}_{n=0}z^{n+1}u^n_{(\mathbf{C})})x_0)=\sum_{n=0}^{\infty}\langle u^n(x_0), \ell_0\rangle z^{n+1} \tag{1}
$$

pour $|z|<1/\varrho$ (théorème 1 de I, p. 24, d)) et est donc holomorphe dans le disque de centre 0 et de rayon $1/\varrho$.

Il existe une fonction holomorphe $\widetilde{R}$ définie sur un voisinage ouvert U de $\lambda_0$ et à valeurs dans $\mathscr{L}(E)$ telle que pour $z$ appartenant à U$-\{\lambda_0\}$, on a

$$
R(u_{(\mathbf{C})}, z) =\widetilde{R}(z) +\sum_{n=0}^{+\infty}(z-\lambda_0)^{-n-1}(u_{(\mathbf{C})}-\lambda_0)^ne_0
$$

(prop. 17 de I, p. 83). Pour $z$ tel que $z^{-1}\in U$ et $z\not = 1/\lambda_0$, on a donc

$$
f(z) =\langle \widetilde{R}(z^{-1})x_0, \ell_0\rangle +\sum_{n=0}^{+\infty}(z^{-1}-\lambda_0)^{-n-1}\langle (u_{(\mathbf{C})}-\lambda_0)^ne_0(x_0), \ell_0\rangle
$$

Le terme de la série correspondant à $n= 0$ est $(z^{-1}-\lambda_0)^{-1}\langle e_0(x_0), \ell_0\rangle$. Comme $\langle e_0(x_0), \ell_0\rangle  \not = 0$, l’unicité du développement de Laurent (VAR, R1, p. 30, 3.3.9) implique que $f$ ne se prolonge pas en une fonction holomorphe au voisinage de $1/\lambda_0$. En particulier, le rayon de convergence du développement en série entière (1) de la fonction $f$ au point 0 est égal à $1/\varrho$.

Les coefficients de la série entière (1) sont $\langle u^n(x_0), \ell_0\rangle \geqslant 0$ puisque $u(C)\subset C$ et $\ell_0\in C^{\circ}$. D’après le lemme 3, la fonction $f$ ne se prolonge pas en une fonction holomorphe au voisinage de $1/\varrho$. La résolvante de $u_{(\mathbf{C})}$ ne peut donc pas être prolongée en une fonction holomorphe au voisinage de $\varrho$, c’est-à-dire que $\varrho \in$ Sp($u$). Cela implique que $\varrho$ est une valeur propre de $u_{(\mathbf{C})}$ (prop. 5 de III, p. 90). Comme $\varrho$ est réel, c’est aussi une valeur propre de $u$.

Soit $d\geqslant 1$ l’ordre du pôle de la résolvante de $u_{(\mathbf{C})}$ en $\varrho$. Soit $e$ l’endomorphisme

$e=$ lim$_{z\rightarrow\varrho}(z-\varrho )^dR(u_{(\mathbf{C})}, z)$.

Il est non nul et permutable à $u_{(\mathbf{C})}$, et son image est contenue dans l’espace propre de $u_{(\mathbf{C})}$ relatif à $\varrho ($cf. n$^o3$ de I, p. 131). Soit maintenant $\ell$ un élément de $C^{\circ}$ et $x$ un élément de C. D’après le théorème 1 de I, p. 24, d), on a

$\langle e(x), \ell \rangle =$ lim$_{zz>\varrho\rightarrow\varrho}(z-\varrho )^d\sum_{n\geqslant 0}\langle u^n(x), \ell \rangle z^{-n-1}\geqslant 0$.

Le théorème des bipolaires (EVT, II, p 48, th. 1) implique que $e(x)\in C$ pour tout $x\in C$. Puisque C est total, il existe $x\in C$ tel que $e(x)\not = 0$ (lemme 4), et alors $e(x)$ appartient à C et est un vecteur propre de $u$ pour la valeur propre $\varrho$, comme désiré.

#### Corollaire {#ts-iii-s6-n7-cor-1 .statement tag=02V5}

Soit E un espace normable complet sur $\mathbf{R}$. Soient C un cône convexe fermé total saillant dans E et $u\in \mathscr{L}(E)$ une application linéaire compacte telle que $u(C)\subset C$. Si le rayon spectral $\varrho (u)$ de $u$ est $>0$, alors $\varrho (^tu) =\varrho (u)$ est une valeur propre de $^tu$, et $^tu$ admet un vecteur propre relatif à $\varrho (u)$ dans $C^{\circ}$.

On a $\varrho (^tu) =\varrho (u)$ (prop. 3 de I, p. 131). D’après le corollaire 1 de III, p. 9, l’endomorphisme $^tu$ de $E'$ est compact. De plus on a $^tu(C^{\circ})\subset C^{\circ}$; l’assertion résulte alors du théorème de Krein–Rutman appliqué à $^tu$, et au cône convexe fermé $C^{\circ}$, puisque celui-ci est saillant (car C est total) et total (car C est saillant).

#### Remarque {#ts-iii-s6-n7-rem-1 .statement tag=02V6}

L’hypothèse $\varrho (u)>0$ ne saurait être omise en général dans le théorème de Krein–Rutman. Par exemple, soit V l’endomorphisme de l’espace de Banach $\mathscr{C}([0,1])$ défini par

$$
V(f)(x) =\int_0^xf(y)dy
$$

pour $f\in \mathscr{C}([0,1])$. L’application V est compacte et son rayon spectral est nul (exercice 1 de I, p. 187). Elle préserve le cône convexe fermé total saillant dans $\mathscr{C}([0,1])$ formé des fonctions positives, et n’a pas de valeur propre (loc. cit.).

La proposition suivante décrit une condition suffisante pour qu’un endomorphisme préservant un cône ait un rayon spectral strictement positif, et précise alors le théorème de Krein–Rutman.

#### Proposition 8 {#ts-iii-s6-prop-8 .statement tag=02V7}

Soit E un espace normable complet sur $\mathbf{R}$ non nul. Soient C un cône convexe fermé saillant d’intérieur $\mathring{C}$ non vide dans E, et $u\in \mathscr{L}(E)$ une application linéaire compacte telle que $u(C-\{0\})\subset \mathring{C}$.

a) On a $\varrho (u)>0$ et il existe un vecteur propre $x_0$ de $u$ dans $\mathring{C}$ pour la valeur propre $\varrho (u)$;

b) Le projecteur spectral de $u$ correspondant à $\varrho (u)$ est de rang 1 ;

c) Pour toute valeur propre $\lambda \not =\varrho (u)$ de $u_{(\mathbf{C})}$, on a $|\lambda |< \varrho (u)$;

d) Soit F un sous-espace de E stable par $u$ tel que (C $-\{0\})\cap F$ est non vide. Alors $x_0\in F$. En particulier, les seuls vecteurs propres de $u$ dans C sont les multiples de $x_0$.

Démontrons deux lemmes préliminaires.

#### Lemme 5 {#ts-iii-s6-lem-5 .statement tag=02V8}

Soient E un espace de Banach réel, C un cône convexe dans E et $u\in \mathscr{L}(E)$ tels que $u(C-\{0\})\subset \mathring{C}$. Soit $\ell \in C^{\circ}$ un vecteur propre de $^tu$. Alors le noyau de $\ell$ est stable par $u$ et ne rencontre pas C $-\{0\}$.

Soit $\lambda \in \mathbf{R}$ tel que $^tu(\ell ) =\lambda \ell$. Pour tout $x\in$ Ker($\ell$ ), on a

$$
\langle u(x), \ell \rangle =\langle x,^tu(\ell )\rangle =\lambda \langle x, \ell \rangle = 0
$$

donc Ker($\ell$ ) est stable par $u$.

Soit $x$ un élément non nul de Ker($\ell$ ). Pour tout élément $y$ de E tel que $\langle y, \ell \rangle <0$, on a $\langle u(x) +y, \ell \rangle <0$, d’où il résulte que $u(x) +$ $y /\in C$ puisque $\ell \in C^{\circ}$. On en déduit que $u(x)$ n’appartient pas à $\mathring{C}$. Comme $u(C-\{0\})\subset \mathring{C}$, cela implique que $x /\in C$.

#### Lemme 6 {#ts-iii-s6-lem-6 .statement tag=02V9}

Soient E un espace vectoriel réel de dimension finie et B un voisinage convexe compact de 0 dans E. Soit $u$ un endomorphisme de E tel que $u(B)\subset \mathring{B}$. Le spectre complexe de $u$ est alors contenu dans le disque unité de $\mathbf{C}$ et, en particulier, il ne rencontre pas le cercle de centre 0 et de rayon 1 dans $\mathbf{C}$.

En remplaçant B par $B\cap (-B)$, on se ramène au cas où B est équilibré. La jauge $p$ de B (EVT, II, p. 28, ex. 3) est alors une norme sur E, qui définit sa topologie (EVT, I, p. 14, th. 2). L’hypothèse implique que $p(u(x))< p(x)$ pour tout élément $x$ de E $-\{0\}$, donc que le rayon spectral de $u$ est $<1$; comme c’est aussi le rayon spectral de $u_{(\mathbf{C})}($cf. I, p. 86), la conclusion en résulte.

Démontrons maintenant la proposition.

Notons $x\preccurlyeq y$ la relation d’ordre sur E associée au cône convexe C (EVT, II, p. 13, n$^o5)$, c’est-à-dire $x\preccurlyeq y$ si et seulement si $y-x\in C$. On a $u(x)\preccurlyeq u(y)$ si $x\preccurlyeq y$. Puisque $\mathring{C}$ est non vide, l’espace vectoriel $C-C$ engendré par C (EVT, II, p. 12, cor. 1) contient un voisinage de 0, donc le cône C est total.

Démontrons l’assertion a). Soit $\varrho =\varrho (u)$. Soit $y_0$ un élément de $\mathring{C}$. On a $y_0\not = 0$. Soit $r >0$ tel que la boule fermée de centre $y_0$ et de rayon $r$ est contenue dans C. Pour tout $y\in E-\{0\}$, on a $y_0-r\|y\|^{-1}y\in C$, donc $y\preccurlyeq r^{-1}\|y\|y_0$ pour tout $y\in E$.

Comme $y_0\not = 0$, les hypothèses impliquent que $u(y_0)\in \mathring{C}$. Il existe donc $t >0$ tel que $tu(y_0)-y_0\in C$. Notons $v=tu$. C’est un endomorphisme compact de E tel que $v(C)\subset C$ et $v(y_0)\succcurlyeq y_0$. Pour tout entier $n\geqslant 1$, on a

$$
y_0\preccurlyeq v^n(y_0)\preccurlyeq r^{-1}\|v^n(y_0)\|y_0\preccurlyeq r^{-1}\|v^n\| \|y_0\|y_0
$$

donc $(r^{-1}\|v^n\|\|y_0\| -1)y_0\in C$. Comme C est saillant, cela implique que $t^n\|u^n\|=\|v^n\|\geqslant r/\|y_0\|$, d’où $\varrho \geqslant t^{-1}>0 ($I, p. 20, prop. 1).

D’après le théorème de Krein–Rutman (th. 4), le nombre réel $\varrho$ est une valeur propre de $u$, et il existe un vecteur propre $x_0$ de $u$ dans C pour la valeur propre $\varrho$. On a $\varrho x_0=u(x_0)\in \mathring{C}$ par hypothèse, donc $x_0\in \mathring{C}$. Cela établit l’assertion a).

Soit K l’intersection du spectre de $u_{(\mathbf{C})}$ et du cercle de centre 0 et de rayon $\varrho$ dans $\mathbf{C}$. Comme $u$ est compact et $\varrho  >0$, l’ensemble K est fini et l’image du projecteur spectral $e_K$ est un sous-espace de $E_{(\mathbf{C})}$ de dimension finie (prop. 2 de III, p. 83 et prop. 5 de III, p. 90). Comme K est stable par la conjugaison complexe, l’image de $e_K$ est un sous-espace de $E_{(\mathbf{C})}$ rationnel sur $\mathbf{R}$ (A, V, p.60, prop. 6) ; notons F le sous-espace de E tel que $F_{(\mathbf{C})}$ est égal à l’image de $e_K$. L’espace F est stable par $u$ et contient le sous-espace propre de $u$ relatif à $\varrho$, donc F est non nul.

Pour démontrer les assertions b) et c), il suffit de démontrer que F est de dimension 1.

Notons $v$ l’endomorphisme de F déduit de $u$ par passage aux sous-espaces. Soit $C_F= C\cap F$. C’est un cône convexe fermé saillant d’intérieur non vide dans F (puisque $x_0\in \mathring{C}\cap F)$, donc total ; il vérifie $v(C_F-\{0\})\subset \mathring{C}_F$, et en particulier est stable par $v$. Comme $\varrho (v)\leqslant \varrho$ et $x_0\in F$, on a $\varrho (v) =\varrho$. D’après le corollaire du théorème 4, appliqué à $C_F$ et $v$, il existe un vecteur propre $\ell$ de $^tv$ dans $C^{\circ}_F$ pour la valeur propre $\varrho (v) =\varrho  >0$.

Le sous-espace Ker($\ell$ ) de F est stable par $v$. Soit $w$ l’endomorphisme de Ker($\ell$ ) déduit de $\varrho^{-1}v$ par passage aux sous-espaces ; son spectre est contenu dans le cercle unité. L’ensemble B des $y\in$ Ker($\ell$ ) tels que $x_0+y\in C_F$ est un voisinage convexe fermé de 0 dans Ker($\ell$ ). Pour tout $y\in B$ et tout $z\in$ Ker($\ell$ ), on a

$$
x_0+ (w(y) +z) =\varrho^{-1}(v(x_0+y) +\varrho z)
$$

qui appartient à $C_F$ si la norme de $z$ est assez petite, donc $w(y)\in \mathring{B}$.

L’ensemble B est borné : en effet, s’il existait une suite $(y_n)_{n\in\mathbf{N}}$ dans Ker($\ell$ ) telle que $\|y_n\| \rightarrow +\infty$ et $x_0+y_n\in C_F$ alors, quitte à extraire une sous-suite, on aurait $y_n/\|y_n\| \rightarrow y$ où $y\in$ Ker($\ell$ ) est non nul, et $y=$ lim $\|y_n\|^{-1}(x_0+y_n)$ appartiendrait à $C_F$, contredisant le lemme 5. L’ensemble B est donc compact.

On déduit alors du lemme 6, appliqué à Ker($\ell$ ), à B et à $w$, que le spectre complexe de $w$ ne rencontre pas le cercle de centre 0 et de rayon 1 ; cela entraîne que le spectre de $w$ est vide, ce qui signifie que Ker($\ell$ ) est réduit à $\{0\}$, donc que F est de dimension 1. Les assertions b) et c) sont donc établies.

L’application linéaire $^tu$ est compacte (corollaire 1 de III, p. 9) et $^tu(C^{\circ})\subset C^{\circ}$; de plus $\varrho (^tu) =\varrho  >0$ (prop. 3 de I, p. 131). D’après le corollaire du théorème 4, il existe dans $C^{\circ}$ un vecteur propre $\ell \not = 0$ de $^tu$ pour la valeur propre $\varrho$. Le noyau de $\ell$ est stable par $u$ et ne rencontre pas C $-\{0\}$ (lemme 5). En particulier, on a $x_0\in /$ Ker($\ell$ ).

Soit F un sous-espace de E stable par $u$. On a la décomposition $F = (F\cap \mathbf{R}x_0)\oplus (F\cap$ Ker($\ell$ )). Si F ne contient pas $x_0$, on a donc $F\subset$ Ker($\ell$ ), donc F ne rencontre pas C$-\{0\}$. Cela établit d) et conclut la preuve de la proposition.

#### Corollaire {#ts-iii-s6-n7-cor-2 .statement tag=02VA}

Soit E un espace normable complet non nul sur $\mathbf{R}$. Soient C un cône convexe fermé saillant d’intérieur $\mathring{C}$ non vide dans E, et $u$ un endomorphisme compact de E telle que $u(C)\subset C$. On suppose qu’il existe un entier $k\geqslant 1$ tel que $u^k(C-\{0\})\subset \mathring{C}$.

a) On a $\varrho (u)>0$ et il existe un vecteur propre $x_0$ de $u$ dans $\mathring{C}$ pour la valeur propre $\varrho (u)$;

b) Le projecteur spectral de $u$ correspondant à $\varrho (u)$ est de rang 1 ;

c) Pour toute valeur propre $\lambda \not =\varrho (u)$ de $u_{(\mathbf{C})}$, on a $|\lambda |< \varrho (u)$;

d) Les seuls vecteurs propres de $u$ dans C sont les multiples de $x_0$.

Posons $\varrho =\varrho (u)$. On peut appliquer le th. 4 à $u$ et la prop. 8 à $u^k$. Il existe donc un vecteur propre $x_0$ de $u$ dans C pour la valeur propre $\varrho$. Comme $0< \varrho (u^k) =\varrho^k$ (formule (4) de I, p. 21), on a en particulier $\varrho  >0$, et puisque $x_0$ est vecteur propre de $u^k$ pour la valeur propre $\varrho (u^k)$, on a $x_0\in \mathring{C}$.

On a Sp($u^k_{(\mathbf{C})}$) $=$ Sp($u_{(\mathbf{C})}$)$^k$ (remarque 4 de I, p. 2), donc toute valeur propre $\lambda \in \mathbf{C}$ de $u_{(\mathbf{C})}$ telle que $|\lambda |=\varrho$ vérifie $\lambda^k=\varrho^k$, et comme tout vecteur propre correspondant à $\lambda$ est vecteur propre de $u^k$ pour $\varrho^k$, donc proportionnel à $x_0$, on a $\lambda =\varrho$.

Si le projecteur spectral de $u$ pour la valeur propre $\varrho$ était de rang au moins 2, il en serait de même de celui de $u^k$ pour la valeur propre $\varrho^k($cf. n$^o2$ de I, p. 129).

Finalement, si $x\in C$ est vecteur propre de $u$, il l’est aussi pour $u^k$, donc est proportionnel à $x_0$.

Soit $n$ un entier $\geqslant 1$. L’ensemble $\mathbf{R}_+^n$ est un cône convexe fermé pointé saillant dans $\mathbf{R}^n$, d’intérieur non vide égal à $(\mathbf{R}_+^*)^n$.

Soit A $= (a_{i,j})$ une matrice réelle de type $(n, n)$, et $u_A$ l’endomorphisme $x\mapsto Ax$ de $\mathbf{R}^n$. Soit $\varrho =\varrho (u_A)$ son rayon spectral.

#### Lemme 7 {#ts-iii-s6-lem-7 .statement tag=02VB}

On a $u_A(\mathbf{R}^n_+)\subset \mathbf{R}_+^n$ si et seulement si $a_{i,j}\geqslant 0$ pour tous $i$ et $j$, et $u_A(\mathbf{R}^n_+-\{0\})\subset (\mathbf{R}_+^*)^n$ si et seulement si $a_{i,j}>0$ pour tous $i$ et $j$.

Soit $(e_1, . . . , e_n)$ la base canonique de $\mathbf{R}^n$. Les vecteurs $e_i$ appartiennent à $\mathbf{R}_+^n$ et $u_A(e_i)\in \mathbf{R}_+^n$ pour tout $i$ (resp. $u_A(e_i)\in (\mathbf{R}_+^*)^n$ pour tout $i)$ si et seulement si $a_{i,j}\geqslant 0$ pour tous $i$ et $j$ (resp. $a_{i,j}>0$ pour tous $i$ et $j)$. Le résultat en découle par linéarité.

#### Théorème 5 (Perron–Frobenius) {#ts-iii-s6-thm-5 .statement tag=02VC}

a) Si $a_{i,j}\geqslant 0$ pour tous $i$ et $j$ dans $\{1, . . . , n\}$, alors le nombre réel $\varrho$ est une valeur propre de A;

b) Si $a_{i,j}>0$ pour tous $i$ et $j$ dans $\{1, . . . , n\}$, alors $\varrho  >0$ et l’espace primaire de $u_A$ relatif à $\varrho$, c’est-à-dire le nilespace de $A-\varrho 1_{\mathbf{R}^n}$, est de dimension 1 et est engendré par un vecteur $x_0\in (\mathbf{R}_+^*)^n$. Il n’existe pas d’autre valeur propre de A admettant un vecteur propre dans $\mathbf{R}^n_+$, et toutes les valeurs propres complexes $\lambda \not =\varrho$ de A vérifient $|\lambda |< \varrho$.

Si $\varrho = 0$, l’assertion a) est élémentaire car 0 est alors une valeur propre de A. Si $\varrho  >0$, l’assertion a) découle du théorème 4 compte tenu du lemme 7. L’assertion b) est elle, pour la même raison, une conséquence de la proposition 8.

#### Remarque {#ts-iii-s6-n7-rem-2 .statement tag=02VD}

On suppose qu’il existe un entier $k\geqslant 1$ tel que tous les coefficients de $A^k$ sont $>0$ (une telle matrice est parfois appelée primitive). Alors, d’après le cor. de la prop. 8, le rayon spectral $\varrho$ est une valeur propre de A, l’espace primaire de $u_A$ relatif à $\varrho$ est de dimension 1, et est engendré par un vecteur $x_0\in (\mathbf{R}^*_+)^n$. De plus, il n’existe pas d’autre valeur propre complexe de A admettant un vecteur propre dans $\mathbf{R}_+^n$ et toutes les valeurs propres complexes $\lambda \not =\varrho$ de A vérifient $|\lambda |< \varrho$.

## EXERCICES {#ts-iii-s6-exercises}

See the [exercises for § 6](exercises/s6/).

[^1]: Certains auteurs parlent de « point fini » du spectre, ou de « spectre discret ».
