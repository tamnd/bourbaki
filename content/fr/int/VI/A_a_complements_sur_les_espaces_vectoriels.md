---
book: int
book_title: Integration
chapter: VI
chapter_title: Intégration vectorielle
section: 0
section_title: Compléments sur les espaces vectoriels topologiques
appendix: true
lang: fr
source: int-vi-fr
pdf_pages: 0073-0077
extraction: ocr
subsections:
    - "no": 1
      title: Formes bilinéaires et applications linéaires.
      page: 0
      pdf_page: 73
    - "no": 2
      title: Quelques types d’espaces possédant la propriété (GDF).
      page: 0
      pdf_page: 75
statements: 6
exercises: 0
content_sha256: fc4e5a9873ecd9d043f4e4ef61316cb2d7a3a32d9e81413132fba59d4389faf2
---

## APPENDICE

# Compléments sur les espaces vectoriels topologiques

### 1. Formes bilinéaires et applications linéaires.

Soient $(F_1, G_1), (F_2, G_2)$ deux couples d’espaces vectoriels (réels ou complexes) en dualité (*Esp. vect. top.*, chap. IV, § 1, n° 1) ; supposons chacun de ces espaces muni de la topologie *faible* correspondante (*loc. cit.*, n° 2) ; si $A$ et $B$ sont deux quelconques de ces espaces, on désignera comme d’ordinaire par $\mathcal{L}(A; B)$ l’espace vectoriel des applications linéaires continues de $A$ dans $B$, et on notera $\mathcal{B}(A, B)$ l’espace vectoriel des formes bilinéaires *séparément continues* sur $A \times B$.

Pour toute forme bilinéaire $\Phi$ séparément continue sur $F_1 \times F_2$, $x_1 \to \Phi(x_1, x_2)$ est une forme linéaire continue sur $F_1$, donc il existe un élément et un seul $^r\Phi(x_2) \in G_1$ tel que

(1)
$$
\Phi(x_1, x_2) = \langle x_1, ^r\Phi(x_2) \rangle
$$
pour $x_1 \in F_1, x_2 \in F_2$ (*Esp. vect. top.*, chap. IV, § 1, n° 2, prop. 1). En outre cette formule montre que l’application $x_2 \to ^r\Phi(x_2)$ est linéaire et continue pour les topologies (faibles) de $F_2$ et de $G_1$. Inversement, pour toute application linéaire continue $u$ de $F_2$ dans $G_1$,
$(x_1, x_2) \to \Phi(x_1, x_2) = \langle x_1, u(x_2) \rangle$ est une forme bilinéaire séparément continue sur $F_1 \times F_2$, et on a $^r\Phi = u$. On a ainsi défini un isomorphisme $r : \Phi \to ^r\Phi$ de $\mathcal{B}(F_1, F_2)$ sur $\mathcal{L}(F_2; G_1)$, dit *canonique*.

La formule

(2)
$$
\Phi(x_1, x_2) = \langle ^l\Phi(x_1), x_2 \rangle
$$

définit de même un *isomorphisme canonique* $l : \Phi \to {}^t\Phi$ de $\mathcal{B}(F_1, F_2)$ sur $\mathcal{L}(F_1; G_2)$; et on a évidemment le diagramme commutatif

$$
\begin{array}{ccc}
& & \mathcal{B}(F_1, F_2) \\
& \swarrow & \downarrow r^{-1} \\
\mathcal{L}(F_1; G_2) & \leftarrow t \rightarrow & \mathcal{L}(F_2; G_1) \\
& \searrow & \downarrow l^{-1} \\
& & \mathcal{L}(F_1; G_2)
\end{array}
$$

où $t$ est l’isomorphisme de transposition $u \to {}^t u$. Vu la définition des topologies faibles sur $G_1$ et $G_2$, il est immédiat en outre que, lorsqu’on munit $\mathcal{B}(F_1, F_2)$, $\mathcal{L}(F_1; G_2)$ et $\mathcal{L}(F_2; G_1)$ de la topologie de la convergence simple, les isomorphismes du diagramme précédent sont des isomorphismes pour les structures d’espace vectoriel topologique.

Soient maintenant $E, F$ deux espaces localement convexes séparés, $E', F'$ leurs duals respectifs ; désignons par $E_\sigma, F_\sigma$ les espaces $E, F$ munis des topologies affaiblies $\sigma(E, E')$, $\sigma(F, F')$, par $E'_s, F'_s$ les espaces $E', F'$ munis des topologies faibles $\sigma(E', E)$, $\sigma(F', F)$. Les remarques précédentes établissent donc des isomorphismes canoniques entre les trois espaces $\mathcal{B}(E_\sigma, F'_s)$, $\mathcal{L}(E_\sigma; F_\sigma)$ et $\mathcal{L}(F'_s; E'_s)$, et aussi entre les trois espaces $\mathcal{B}(E_\sigma, F_s)$, $\mathcal{L}(E_\sigma; F'_s)$ et $\mathcal{L}(F_s; E'_s)$. On remarquera que $\mathcal{B}(E_\sigma, F_\sigma)$ est aussi égal à l’espace $\mathcal{B}(E, F)$ des formes bilinéaires séparément continues sur $E \times F$ ($E$ et $F$ étant munis de leurs topologies initiales), puisque toute forme linéaire continue dans $E$ (resp. $F$) est continue dans $E_\sigma$ (resp. $F_\sigma$) et réciproquement (*Esp. vect. top.*, chap. IV, § 1, no 1 et no 2, prop. 1).

Soit $\mathcal{B}(E, F)$ l’espace des formes bilinéaires continues sur $E \times F$ ($E$ et $F$ étant munis de leurs topologies initiales) ; on a $\mathcal{B}(E, F) \subset \mathcal{B}(E, F)$.

#### Proposition 1 {#int-vi-a0-prop-1 .statement}

*Pour qu’une forme bilinéaire* $\Phi \in \mathcal{B}(E, F)$ *appartienne à* $\mathcal{B}(E, F)$, *il faut et il suffit qu’il existe un voisinage de* 0 *dans* $E$ *dont l’image par* ${}^t\Phi$ *soit une partie équicontinue de* $F'$.

En effet, dire que $\Phi$ est continue signifie qu’il existe un voisinage convexe équilibré $V$ (resp. $W$) de 0 dans $E$ (resp. $F$) tels que $|\Phi(x, y)| \leq 1$ pour $x \in V,\ y \in W$; cela s’écrit $|\langle {}^t\Phi(x), y \rangle| \leq 1$, pour $x \in V$ et $y \in W$, ou encore $l'\Phi(V) \subset W^0$; d'où la proposition, compte tenu du fait que toute partie équicontinue de $F'$ est contenue dans le polaire d'un voisinage de 0 dans $F$.

#### Corollaire {#int-vi-a0-n1-cor-1 .statement}

*Si $\Phi$ est une forme bilinéaire continue dans $E \times F$, $l'\Phi$ est une application linéaire continue de $E$ dans le dual fort $F'_b$ de $F$. Si en outre $E$ et $F$ sont normés, on a $\|l'\Phi\| = \|\Phi\|$.*

La première assertion résulte de la prop. 1 et du fait que tout voisinage de 0 dans $F'_b$ absorbe toute partie équicontinue de $F'$. Si $E$ et $F$ sont normés, on a

$$
\begin{align*}
\|\Phi\| &= \sup_{\|x\| \leq 1, \|y\| \leq 1} |\Phi(x, y)| = \sup_{\|x\| \leq 1} (\sup_{\|y\| \leq 1} |\langle l'\Phi(x), y \rangle|) \\
&= \sup_{\|x\| \leq 1} \|l'\Phi(x)\| = \|l'\Phi\|
\end{align*}
$$

d'où la seconde assertion.

En échangeant les rôles de $E$ et $F$, on obtient des résultats analogues à la prop. 1 et à son corollaire pour les applications linéaires $r'\Phi$; nous laissons au lecteur le soin de les énoncer.

### 2. Quelques types d’espaces possédant la propriété (GDF).

Nous savons déjà que tout espace de Fréchet possède la propriété (GDF) (*Esp. vect. top.*, chap. I, § 3, no 3, cor. 5 du th. 1).

#### Proposition 2 {#int-vi-a0-prop-2 .statement}

*Soient $E$ un espace vectoriel, $(F_\alpha)_{\alpha \in \Lambda}$ une famille d’espaces localement convexes possédant la propriété (GDF), et pour chaque $\alpha \in \Lambda$, soit $h_\alpha$ une application linéaire de $F_\alpha$ dans $E$. Si on munit $E$ de la topologie localement convexe la plus fine rendant continues les $h_\alpha$, $E$ possède la propriété (GDF).*

Soit $u$ une application linéaire de $E$ dans un espace de Banach $B$, telle que toute limite dans $E \times B$ de toute suite convergente de points du graphe $\Gamma$ de $u$ appartienne encore à $\Gamma$. Il suffit de montrer que, pour tout $\alpha \in \Lambda$, $u \circ h_\alpha$ est continue dans $F_\alpha$ (*Esp. vect. top.*, chap. II, § 2, no 2, cor. de la prop. 1). Or, soit $(x_n)$ une suite d’éléments de $F_\alpha$ ayant une limite $a$ et telle que la suite $(u(h_\alpha(x_n)))$ ait une limite $b \in B$. Comme $h_\alpha$ est continue, $h_\alpha(a)$ est une limite de la suite $(h_\alpha(x_n))$ dans $E$; par hypothèse, on a donc $b = u(h_\alpha(a))$, et comme $F_\alpha$ possède la propriété (GDF), $u \circ h_\alpha$ est continue.

#### Corollaire {#int-vi-a0-n2-cor-1 .statement}

*Tout espace quotient d’un espace localement convexe possédant la propriété* (GDF) *possède la propriété* (GDF).

#### Proposition 3 {#int-vi-a0-prop-3 .statement}

*Le dual fort d’un espace de Fréchet réflexif possède la propriété* (GDF).

C’est une conséquence de la prop. 2 et du lemme suivant :

#### Lemme 1 {#int-vi-a0-lem-1 .statement}

*Soient F un espace de Fréchet, F' son dual fort, F'' son bidual. Si toute partie de F'', bornée pour $\sigma(F'', F')$, est contenue dans l’adhérence (pour $\sigma(F'', F')$) d’une partie bornée de F, alors F' est limite inductive d’une suite d’espaces de Banach.*

Soit en effet $(V_n)$ une suite fondamentale décroissante de voisinages convexes, équilibrés et fermés de 0 dans F. Pour tout entier $n$, soit $G_n$ le sous-espace de $F'$ engendré par le polaire $V_n^0$ de $V_n$. Dans $G_n$, $V_n^0$ est un ensemble convexe absorbant, donc sa jauge $p_n$ est une norme sur $G_n$; en outre $V_n^0$ est une partie complète du dual fort $F'$ (*Esp. vect. top.*, chap. III, § 3, no 7, th. 4); donc $G_n$, muni de la norme $p_n$, est un espace de Banach (*Esp. vect. top.*, chap. I, § 1, no 5, cor. de la prop. 8). Nous allons montrer que la topologie forte sur $F'$ est limite inductive de ces topologies d’espace de Banach sur les $G_n$, ou encore que, pour qu’une partie convexe, équilibrée et fortement fermée U de $F'$ soit un voisinage fort de 0, il faut et il suffit qu’elle absorbe chacun des $V_n^0$. Il est évident que cette condition est nécessaire; pour voir qu’elle est suffisante, il nous suffira de prouver que U contient un *tonneau* de $F'$. En effet, son polaire $U^0$ dans $F''$ sera alors borné pour $\sigma(F'', F')$, donc sera contenu par hypothèse dans l’adhérence (pour $\sigma(F'', F')$) d’une partie bornée B de F, et on en conclura que U (qui est fermé pour $\sigma(F', F'')$) contient le voisinage fort $B^0$ de 0 (*Esp. vect. top.*, chap. IV, § 1, no 3, prop. 3).

Par hypothèse, pour tout entier $n$, il existe un nombre $\lambda_n > 0$ tel que $\lambda_n V_n^0 \subset \frac{1}{2} U$; soit $A_n$ l’enveloppe convexe de la réunion des $\lambda_i V_i^0$ pour $i \leq n$. On a $A_n \subset \frac{1}{2} U$ pour tout $n$; soit W la réunion des

A_n : W est un ensemble convexe, équilibré, absorbant, contenu dans $\frac{1}{2} U$ et il nous suffit de montrer que son adhérence forte (qui est un tonneau) est contenue dans U.

Soit donc $x'$ un point de $F'$ n’appartenant pas à U. Comme chacun des $V_n^0$ est compact pour $\sigma(F', F)$, il en est de même de $A_n$ ($Esp.\ vect.\ top.$, chap. II, § 4, no 1, prop. 1), et comme $x' \notin 2A_n$, il existe un élément $x_n$ appartenant au polaire de $A_n$ dans F et tel que $\langle x', x_n \rangle = 2$ ($Esp.\ vect.\ top.$, chap. II, § 3, no 3, prop. 4). La suite $(x_n)$ est bornée dans F : en effet, tout $y' \in F'$ appartient à un des $V_k^0$, et on a par suite $|\langle y', x_n \rangle| \leq \lambda_k^{-1}$ pour $n \geq k$, d’où notre assertion ($Esp.\ vect.\ top.$, chap. IV, § 2, no 4, th. 3). Soit C un ensemble borné convexe équilibré de F contenant tous les $x_n$; C$^0$ est alors un voisinage de 0 dans $F'$, et le polaire $C^{00}$ de $C^0$ dans $F''$ est compact pour $\sigma(F'', F')$ ($Esp.\ vect.\ top.$, chap. IV, § 2, no 2, prop. 2). On voit donc que la suite $(x_n)$ admet une valeur d’adhérence $x''$ dans $F''$ pour $\sigma(F'', F')$; on a évidemment $\langle x', x'' \rangle = 2$ et d’autre part, $x''$ appartient au polaire de $A_n$ dans $F''$ pour tout $n$, donc au polaire $W^0$ de W dans $F''$. On en conclut que $x' \notin W^{00}$, donc n’est pas adhérent à W pour $\sigma(F', F'')$ ($Esp.\ vect.\ top.$, chap. IV, § 1, no 3, prop. 3), ni a fortiori pour la topologie forte, ce qui achève la démonstration.
