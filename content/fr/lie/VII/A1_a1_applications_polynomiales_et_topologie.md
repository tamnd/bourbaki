---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: Sous-algèbres de Cartan. Éléments réguliers
section: 1
section_title: Applications polynomiales et topologie de Zariski
appendix: true
lang: fr
source: lie-vii-viii-fr
pdf_pages: 0045-0049
extraction: ocr
subsections:
    - "no": 1
      title: Topologie de Zariski
      page: 0
      pdf_page: 45
    - "no": 2
      title: Applications polynomiales dominantes
      page: 0
      pdf_page: 46
statements: 10
exercises: 0
content_sha256: b0e358a55949c56323f16579e6b156c21b5a698fe5a7c1c68f36f6da38a197df
---

## APPENDICE 1

# Applications polynomiales et topologie de Zariski

Dans cet appendice, k est supposé infini.

### 1. Topologie de Zariski

Soit V un espace vectoriel de dimension finie. On note $A_V$ l’algèbre des fonctions polynomiales sur V à valeurs dans $k$ (A, IV, § 5, n° 10, déf. 4). C’est une algèbre graduée; sa composante de degré 1 est le dual $V^*$ de V, et l’injection de $V^*$ dans $A_V$ se prolonge en un *isomorphisme de l’algèbre symétrique* $S(V^*)$ *sur* $A_V$ (Λ, IV, § 5, n° 11, *Rem. 2*).

Si $(e_1, \ldots, e_n)$ est une base de V, et $(X_1, \ldots, X_n)$ une suite d’indéterminées, l’application de $k[X_1, \ldots, X_n]$ dans $A_V$ qui transforme tout élément $f$ de $k[X_1, \ldots, X_n]$ en la fonction

$$
\sum_{i=1}^n \lambda_i e_i \mapsto f(\lambda_1, \ldots, \lambda_n)
$$

est un isomorphisme d’algèbres (A, IV, § 5, n° 10, cor. à la prop. 19).

#### Proposition 1 {#lie-vii-a1-prop-1 .statement tag=00XC}

*Soit H l’ensemble des homomorphismes d’algèbres de $A_V$ dans $k$. Pour tout $x \in V$, soit $h_x$ l’homomorphisme $f \mapsto f(x)$ de $A_V$ dans $k$. Alors l’application $x \mapsto h_x$ est une bijection de V sur H.*

En effet, soit $H'$ l’ensemble des homomorphismes d’algèbres de $k[X_1, \ldots, X_n]$ dans $k$. L’application $\chi \mapsto (\chi(X_1), \ldots, \chi(X_n))$ est évidemment une bijection de $H'$ sur $k^n$.

#### Corollaire {#lie-vii-a1-n1-cor-1 .statement tag=00XD}

*Pour tout $x \in V$, soit $m_x = \mathrm{Ker}(h_x)$. Alors l’application $x \mapsto m_x$ est une bijection de V sur l’ensemble des idéaux $m$ de $A_V$ tels que $A_V/m = k$.*

Un sous-ensemble F de V sera dit *fermé* s’il existe une famille $(f_i)_{i \in I}$ d’éléments de $A_V$ telle que

$$
x \in F \Leftrightarrow x \in V \text{ et } f_i(x) = 0 \text{ pour tout } i \in I.
$$

Il est clair que $\emptyset$ et V sont fermés, et que toute intersection d’ensembles fermés est fermée. Si F est défini par l’annulation des $f_i$ et $F'$ par celle des $f_j'$, $F \cup F'$ est défini par l’annulation des $f_i f_j'$, donc est fermé. Il existe donc une topologie sur V telle que les ensembles fermés pour cette topologie soient exactement les ensembles fermés au sens précédent. Cette topologie s’appelle la *topologie de Zariski* de V. Pour tout $f \in A_V$, nous noterons $V_f$ l’ensemble des $x \in V$ tels que f(x) \neq 0 ; c'est une partie ouverte de V. Il est clair que les $V_f$ forment une base de la topologie de Zariski. (Si $k$ est un corps topologique, la topologie canonique de V est plus fine que la topologie de Zariski.)

L'application $x \mapsto m_x$ du cor. de la prop. 1 peut être considérée comme une application $\varepsilon$ de V dans le spectre premier $\mathrm{Spec}(A_V)$ de $A_V$ (AC, II, § 4, n° 3, déf. 4). Il est immédiat que la topologie de Zariski est l'image réciproque par $\varepsilon$ de la topologie de $\mathrm{Spec}(A_V)$.

#### Proposition 2 {#lie-vii-a1-prop-2 .statement tag=00XE}

*L'espace vectoriel V, muni de la topologie de Zariski, est un espace noethérien irréductible. En particulier, toute partie ouverte non vide de V est dense.*

Puisque $A_V$ est noethérien, $\mathrm{Spec}(A_V)$ est noethérien (AC, II, § 4, n° 3, cor. 7 de la prop. 11), et tout sous-espace d'un espace noethérien est noethérien (*loc. cit.*, n° 2, prop. 8). Avec les notations du cor. de la prop. 1, l'intersection des $m_x$ est $\{0\}$, et $\{0\}$ est un idéal premier de $A_V$; donc V est irréductible (*loc. cit.*, n° 3, prop. 14).

### 2. Applications polynomiales dominantes

Soient V, W des espaces vectoriels de dimension finie. Soit $f$ une application polynomiale de V dans W (A, IV, § 5, n° 10, déf. 4). Si $\psi \in A_W$, on a $\psi \circ f \in A_V$ (*loc. cit.*, prop. 17). L'application $\psi \mapsto \psi \circ f$ est un homomorphisme de $A_W$ dans $A_V$, dit *associé à f*. Son noyau est formé des fonctions $\psi \in A_W$ qui sont nulles sur $f(V)$ (donc aussi sur l'*adhérence* de $f(V)$ pour la topologie de Zariski).

#### Définition 1 {#lie-vii-a1-def-1 .statement tag=00XF}

*Une application polynomiale $f : V \to W$ est dite dominante si l'homomorphisme de $A_W$ dans $A_V$ associé à $f$ est injectif.*

Vu ce qui précède, $f$ est dominante si et seulement si $f(V)$ est *dense* dans W pour la topologie de Zariski.

#### Proposition 3 {#lie-vii-a1-prop-3 .statement tag=00XG}

*Supposons k algébriquement clos. Soit $f : V \to W$ une application polynomiale dominante. L'image par $f$ de toute partie ouverte dense de V contient une partie ouverte dense de W.*

Il suffit de prouver que, pour tout élément non nul $\varphi$ de $A_V$, $f(V_\varphi)$ contient une partie ouverte dense de W. Identifions $A_W$ à une sous-algèbre de $A_V$ grâce à l'homomorphisme associé à $f$. Il existe un élément non nul $\psi$ de $A_W$ tel que tout homomorphisme $w : A_V \to k$ n'annulant pas $\psi$ se prolonge en un homomorphisme $v : A_V \to k$ n'annulant pas $\varphi$ (AC, V, § 3, n° 1, cor. 3 du th. 1). Or un tel $w$ (resp. un tel $v$) s'identifie à un élément de $W_\psi$ (resp. de $V_\varphi$) et dire que $v$ prolonge $w$ signifie que $f(v) = w$. On a donc $W_\psi \subset f(V_\varphi)$.

C.Q.F.D.

Soient $f : V \to W$ une application polynomiale, et $x_0 \in V$. L’application $h \mapsto f(x_0 + h)$ de $V$ dans $W$ est polynomiale. Décomposons-la en somme finie d’applications polynomiales homogènes :

$$
f(x_0 + h) = f(x_0) + D_1(h) + D_2(h) + \cdots
$$

où $D_i : V \to W$ est homogène de degré $i$ (A, IV, § 5, n° 10, prop. 19). L’application linéaire $D_1$ s’appelle l’application linéaire tangente à $f$ en $x_0$. On la note $Df(x_0)$.

#### Proposition 4 {#lie-vii-a1-prop-4 .statement tag=00XH}

*Soit $f : V \to W$ une application polynomiale. Supposons qu’il existe $x_0 \in V$ tel que $(Df)(x_0)$ soit surjective. Alors $f$ est dominante.*

Quitte à effectuer une translation sur $V$ et une autre sur $W$, on peut supposer que $x_0 = 0$ et que $f(x_0) = 0$. La décomposition de $f$ en somme d’éléments homogènes s’écrit alors

$$
f = f_1 + f_2 + \cdots \quad \text{avec} \quad \deg f_i = i,
$$

et l’application linéaire $f_1$ est surjective par hypothèse. Supposons que $f$ ne soit pas dominante. Il existe alors un élément non nul $\psi$ de $A_W$ tel que $\psi \circ f = 0$. Soit $\psi = \psi_m + \psi_{m+1} + \cdots$ la décomposition de $\psi$ en éléments homogènes, avec $\deg \psi_i = i$ et $\psi_m \neq 0$. Alors

$$
\begin{align*}
0 &= \psi \circ f = \psi_m \circ f + \psi_{m+1} \circ f + \cdots \\
&= \psi_m \circ f_1 + \rho
\end{align*}
$$

où $\rho$ est une somme d’applications polynomiales homogènes de degrés $> m$. On en déduit que $\psi_m \circ f_1 = 0$. Puisque $f_1$ est surjective, on a $\psi_m = 0$, ce qui est absurde.

#### Corollaire {#lie-vii-a1-n2-cor-1 .statement tag=00XI}

*Si $k$ est algébriquement clos et si $f$ vérifie les hypothèses de la prop. 4, l’image par $f$ de toute partie ouverte dense de $V$ contient une partie ouverte dense de $W$.*

Cela résulte des prop. 3 et 4.

APPENDICE II

Une propriété de connexion

#### Lemme 1 {#lie-vii-a1-lem-1 .statement}

*Soient $X$ un espace topologique connexe et $\Omega$ un ouvert dense dans $X$. Si, quel que soit $x \in X$, il existe un voisinage $V$ de $x$ tel que $V \cap \Omega$ soit connexe, alors $\Omega$ est connexe.*

Soit en effet $\Omega_0$ une partie ouverte et fermée non vide de $\Omega$. Soit $x \in X$ et soit $V$ un voisinage de $x$ tel que $V \cap \Omega$ soit connexe. Si $x \in \overline{\Omega}_0$, on a

$$
(V \cap \Omega) \cap \Omega_0 = V \cap \Omega_0 \neq \emptyset,
$$

donc $V \cap \Omega \subset \Omega_0$. Puisque $\Omega$ est dense dans $X$, $\overline{\Omega}_0$ est donc un voisinage de $x$.

Par conséquent, $\overline{\Omega}_0$ est ouvert et fermé, non vide, et puisque $X$ est connexe, $\overline{\Omega}_0 = X$. Puisque $\Omega_0$ est fermé dans $\Omega$, ceci entraîne $\Omega_0 = \Omega \cap \overline{\Omega}_0 = \Omega$, ce qui prouve que $\Omega$ est connexe.

#### Lemme 2 {#lie-vii-a1-lem-2 .statement}

Soient $U$ une boule ouverte de $\mathbf{C}^n$ et $f : U \to \mathbf{C}$ une fonction holomorphe non identiquement nulle. Soit $A$ une partie de $U$ telle que $f = 0$ sur $A$. Alors $U - A$ est dense dans $U$ et connexe.

La densité de $U - A$ résulte de VAR, R, 3.2.5. Supposons d’abord $n = 1$. Si $a \in A$, le développement de $f$ en série entière au point $a$ (VAR, R, 3.2.1) n’est pas réduit à 0, et on en déduit qu’il existe un voisinage $V_a$ de $a$ dans $U$ tel que $f$ ne s’annule pas sur $V_a - \{a\}$. Ainsi, $a$ est isolé dans $A$, ce qui prouve que $A$ est une partie discrète de $U$, donc dénombrable puisque $U$ est dénombrable à l’infini. Soient $x, y \in U - A$. La réunion des droites affines réelles joignant $x$ (resp. $y$) à un point de $A$ est maigre (TG, IX, § 5, p. 53). Il existe donc $z \in U - A$ tel qu’aucun des segments $[x, z]$ et $[y, z]$ ne rencontre $A$. Les points $x, y, z$ appartiennent donc à une même composante connexe de $U - A$, ce qui démontre le lemme dans le cas $n = 1$. Passons au cas général. On peut supposer que $A$ est l’ensemble des zéros de $f$ (TG, I, p. 81, prop. 1). Soient $x, y \in U - A$ et soit $L$ une droite affine contenant $x$ et $y$. La restriction de $f$ à $L \cap U$ n’est pas identiquement nulle puisque $x \in L \cap U$. D’après ce qui précède, $x$ et $y$ appartiennent à une même composante connexe de $(L \cap U) - (L \cap A)$ donc à une même composante connexe de $U - A$.

#### Lemme 3 {#lie-vii-a1-lem-3 .statement}

Soit $X$ une variété analytique complexe connexe de dimension finie et soit $A$ une partie de $X$ vérifiant la condition:
Pour tout $x \in X$, il existe un germe de fonction analytique $f_x$ non nul en $x$ tel que le germe de $A$ en $x$ soit contenu dans le germe en $x$ de l’ensemble des zéros de $f_x$.
Alors $X - A$ est dense dans $X$ et connexe.

La densité de $X - A$ résulte de VAR, R, 3.2.5. On peut supposer que $A$ est fermé (TG, I, p. 81, prop. 1). Pour tout $x \in X$, il existe un voisinage ouvert $V$ de $x$ et un isomorphisme $c$ de $V$ sur une boule ouverte de $\mathbf{C}^n$ tels que $c(A \cap V)$ soit contenu dans l’ensemble des zéros d’une fonction holomorphe non identiquement nulle sur $c(V)$. D’après le lemme 2, $V \cap (X - A)$ est alors connexe. Compte tenu du lemme 1, ceci prouve que $X - A$ est connexe.

Exercices

Les algèbres de Lie et les modules sur ces algèbres sont supposés de dimension finie sur k; à partir du § 3, on suppose k de caractéristique zéro.
