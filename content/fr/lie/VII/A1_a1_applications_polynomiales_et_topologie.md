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
pdf_pages: 0045-0047, 0060-0060
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
statements: 7
exercises: 4
content_sha256: db151ea1252edec71e801c2899e9ef64f21f7fda511f58e837bb68236437f289
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

## EXERCICES {#lie-vii-a1-exercises}

On note $V$ un espace vectoriel de dimension finie sur $k$.

See the [exercises for Appendix 1](exercises/a1/).
