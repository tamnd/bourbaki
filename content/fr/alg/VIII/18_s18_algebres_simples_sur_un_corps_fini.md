---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 18
section_title: Algèbres simples sur un corps fini
lang: fr
source: alg-viii-fr
book_pages: A VIII.347-A VIII.352
pdf_pages: 0350-0355
extraction: native
subsections:
    - "no": 1
      title: Polynômes sur un corps fini
      page: 347
      pdf_page: 350
    - "no": 2
      title: Algèbres simples sur un corps fini
      page: 348
      pdf_page: 351
statements: 10
exercises: 7
content_sha256: 5c5cb7e7e59e66b069178c7d5bb1b6e6ce390914bc0d9df9e79b78f2b4d44b9c
---

## § 18. ALGÈBRES SIMPLES SUR UN CORPS FINI

### 1. Polynômes sur un corps fini

#### Théorème 1 {#alg-viii-s18-thm-1 .statement tag=00SA}

Soit K un corps commutatif fini, de caractéristique $p$. Soient $n$ un entier $\geqslant 1$et $(f_i)_{i\in I}$ une famille finie d’éléments non nuls de $K[X_1, . . . ,X_n]$. Notons Z l’ensemble des éléments $\mathbf{x}$de $K^n$ tels que l’on ait $f_i(\mathbf{x}) = 0$ pour $i\in I$. Si l’on a $n >\sum_{i\in I}$ deg($f_i$), le cardinal de Z est divisible par $p$.

#### Lemme 1 {#alg-viii-s18-lem-1 .statement tag=00LB}

Soient L un corps, G un groupe fini et $\chi$ un homomorphisme non trivial de G dans le groupe multiplicatif $L^*$. On a $\sum_{x\in G}\chi (x) = 0$.

Par hypothèse, il existe un élément $a$ de G tel que $\chi (a)\not= 1$; comme la multiplication par $a$ est une permutation de G, on a

$$
_x\sum_{\in G}\chi (x) =_x\sum_{\in G}\chi (ax) =\chi (a)_x\sum_{\in G}\chi (x)
$$

d’où le lemme 1.

#### Lemme 2 {#alg-viii-s18-lem-2 .statement tag=00LC}

Soit $q$ le cardinal de K. Pour tout entier $m\geqslant 0$, posons $S_m$ = $\sum_{x\in K}x^m$. On a $S_m=-1$si $m$ est un multiple non nul de $q-1$et $S_m= 0$dans les autres cas.

Rappelons que $0^0= 1$ (I, p. 13). Supposons $m$ multiple de $q-1$. Comme le groupe commutatif $K^*$ est d’ordre $q-1$, on a $x^m= 1$ pour tout $x\in K^*$, et $S_m= 0^m+ (q-1)\cdot 1$, d’où l’assertion dans ce cas.

Supposons que $m$ ne soit pas multiple de $q-1$. Posons $\chi (x) =x^m$ pour $x\in K^*$. Comme le groupe multiplicatif $K^*$ est cyclique d’ordre $q-1$ (V, p. 89, prop. 1), il existe un élément $a$ de $K^*$ tel que $\chi (a)\not= 1$. D’après le lemme 1 appliqué à $G = K^*$, on a

$$
S_m= 0^m+_x\sum_{\in K^*}\chi (x) = 0
$$

d’où le lemme 2.

Prouvons maintenant le théorème 1. Soit $\mathbf{x} = (x_1, . . . , x_n)$ un élément de $K^n$; on a $1-f_i(\mathbf{x})^{q-1}= 0$ si $f_i(\mathbf{x})\not= 0$ et $1-f_i(\mathbf{x})^{q-1}= 1$ si $f_i(\mathbf{x}) = 0$. Posons $P =\prod^r_{i=1}(1-f_i^{q-1})$; on a

1 si $\mathbf{x}\in Z$,

$$
P(\mathbf{x}) = \tag{1}
$$

0 si $\mathbf{x}\notin Z$.

Développons le polynôme P sous la forme $\sum_{\alpha\in\mathbf{N}^n}c_{\alpha}X^{\alpha}$; il est de degré $<(q-1)n$ par hypothèse. Soit $\alpha$ un élément de $\mathbf{N}^n$ tel que $c_{\alpha}$ soit non nul ; puisque l’on a $\alpha_1+\cdots +\alpha_n<(q-1)n$, il existe donc un entier $\ell$ tel que $1\leqslant \ell \leqslant n$ et $0\leqslant \alpha_{\ell}<$ $q-1$. D’après le lemme 2, on a alors $\sum_{x\in K}x^{\alpha_{\ell}}= 0$, d’où

$$
_{\mathbf{x}}\sum_{\in K^n}\mathbf{x}^{\alpha}=_j\prod_{=1}^n((\sum_{x\in K}x^{\alpha_j})= 0
$$

On a donc

$$
_{\mathbf{x}}\sum_{\in K^n}P(\mathbf{x}) =_{\alpha}\sum_{\in\mathbf{N}^n}c_{\alpha}((\sum_{\mathbf{x}\in K^n}\mathbf{x}^{\alpha})= 0
$$

Or, d’après la formule (1), on a $\sum_{\mathbf{x}\in K^n}P(\mathbf{x}) =$ Card(Z) $\cdot 1$, d’où Card(Z) $\cdot 1 = 0$, ce qui signifie que Card(Z) est divisible par $p$.

#### Corollaire {#alg-viii-s18-n1-cor-1 .statement tag=00LD}

Soient V un espace vectoriel de dimension finie $n$ sur K, I un ensemble fini, et pour chaque $i\in I$, soit $F_i: V\rightarrow K$une application polynomiale homogène de degré $d_i>0$. Si l’on a $\sum_{i\in I}d_i< n$, il existe un élément non nul $x$ de V tel que $F_i(x) = 0$pour tout $i\in I$.

Soit $(e_1, . . . , e_n)$ une base de V sur K. Par définition des applications polynomiales homogènes (IV, p. 52, déf. 3), il existe pour tout $i\in I$ un polynôme $f_i$ dans $K[X_1, . . . ,X_n]$ homogène de degré $d_i$, tel que l’on ait $F_i(\xi_1e_1, . . . , \xi_ne_n) =$ $f_i(\xi_1, . . . , \xi_n)$. Soit Z l’ensemble des éléments $x$ de V tels que $F_i(x) = 0$ pour tout $i\in I$. D’après le théorème 1, le cardinal de Z est divisible par $p$ et, comme 0 appartient à S, on a Card(Z) $\geqslant p >1$.

### 2. Algèbres simples sur un corps fini

#### Théorème 2 {#alg-viii-s18-thm-2 .statement tag=00SB}

Tout corps fini est commutatif.

Soit D un corps fini et soit K son centre. La K-algèbre D est centrale et simple, de degré $m^2$, où $m$ est un entier strictement positif. La norme réduite est une application polynomiale Nrd$: D\rightarrow K$, homogène de degré $m$ (VIII, p. 338, prop. 6) et l’on a Nrd($a$)$\not= 0$ pour tout $a\not= 0$ dans D (VIII, p. 334, prop. 3). Le corollaire ci-dessus entraîne $m\geqslant m^2$, d’où $m= 1$. On a donc D = K.

#### Corollaire 1 {#alg-viii-s18-thm-2-cor-1 .statement tag=00LE}

Tout anneau simple fini est isomorphe à un anneau de matrices $\mathbf{M}_n(L)$où $n$ est un entier strictement positif et L un corps commutatif fini.

Cela résulte du théorème 2 et du théorème de structure des anneaux simples (VIII, p. 116, th. 1).

#### Corollaire 2 {#alg-viii-s18-thm-2-cor-2 .statement tag=00LF}

Soit K un corps commutatif fini. Toute algèbre simple centrale sur K est isomorphe à une algèbre de matrices $\mathbf{M}_n(K)$où $n$ est un entier strictement positif.

Cela résulte du théorème 2 et du théorème de structure des algèbres centrales simples (VIII, p. 248, th. 1).

#### Remarque 1 {#alg-viii-s18-n2-rem-1 .statement tag=00LG}

Voici une autre démonstration du théorème 2. Soit D un corps fini, soit K son centre et soit L un sous-corps commutatif maximal de D. Soit $x$ un élément de $D^*$; il appartient à un sous-corps commutatif maximal $L_1$ de D ; on a l’égalité

$$
[D : K] = [L : K]^2= [L_1: K]^2
$$

d’après le cor. 2 de VIII, p. 261, d’où $[L : K] = [L_1: K]$. D’après la prop. 3 de V, p. 90, les extensions L et $L_1$ de K sont isomorphes. D’après VIII, p. 259, cor., il existe un élément $a$ de $D^*$ tel que $aLa^{-1}= L_1$, donc $a^{-1}xa$ appartient à L. On a alors $(ay)^{-1}x(ay) =a^{-1}xa$ pour tout $y\in L^*$. Par suite, si S est un ensemble de représentants de classes à gauche dans $D^*$ modulo $L^*$, tout élément de $D^*-\{1\}$ s’écrit $sxs^{-1}$, avec $s\in S$ et $x\in L^*-\{1\}$. Notons $d$ l’ordre de $D^*$ et $\ell$ celui de $L^*$; comme le cardinal de S est égal à $d/\ell$, on a $d-1\leqslant (d/\ell )(\ell -1) =d-d/\ell$; on en déduit $\ell =d$, d’où L = D, ce qui prouve que le corps D est commutatif.

#### Remarque 2 {#alg-viii-s18-n2-rem-2 .statement tag=00LH}

Soit L un corps commutatif qui satisfait à la propriété suivante :

$(C_1)$Soit V un espace vectoriel de dimension finie $n$ sur le corps L, soit $d$ tel que $0< d < n$. Pour toute application polynomiale homogène $F : V\rightarrow L$de degré $d$, il existe un élément non nul $x$ de V tel que $F(x) = 0$.

La démonstration du théorème 2 prouve que tout corps de centre L et de degré fini sur L est égal à L.

D’après le cor. de VIII, p. 348 tout corps fini possède la propriété $(C_1)$. On peut prouver (VIII, p. 352, exerc. 7) que les corps suivants possèdent la propriété $(C_1) :$ – toute extension algébrique d’un corps fini ;

– tout corps de fractions rationnelles en une indéterminée à coefficients dans un corps algébriquement clos (théorème de Tsen). – $*$tout corps muni d’une valuation discrète, pour laquelle il est complet, et dont le

corps résiduel est algébriquement clos (VIII, p. 327, exerc. 17$).*$

#### Remarque 3 {#alg-viii-s18-n2-rem-3 .statement tag=00LI}

Supposons que le corps K satisfasse à la condition suivante :

– Si L est une extension de degré fini de K, elle est cyclique et l’application norme $N : L^*\rightarrow K^*$ est surjective.

Cette condition est en particulier vérifiée si le corps K est fini (V, p. 91, prop. 4). On peut alors démontrer que tout corps de centre K, de degré fini sur K, est égal à K (exerc. 10 de VIII, p. 325).

## EXERCICES {#alg-viii-s18-exercises}

See the [exercises for § 18](exercises/s18/).
