---
book: var
book_title: Variétés différentielles et analytiques
chapter: "1"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 0
section_title: Polynômes-continus et séries formelles
appendix: true
lang: fr
source: var-fr
pdf_pages: 0086-0087
extraction: ocr
statements: 0
exercises: 0
content_sha256: 4f5da2d5f93a17339b36e8b289bea09365035864aa242bc99e5291d21d3b274d
---

## APPENDICE

# Polynômes-continus et séries formelles

Dans cet Appendice, on désigne par F un espace polynormé séparé sur K, par E_i (pour $1 \leq i \leq n$) un espace normé sur K et par E l’espace vectoriel topologique produit des E_i.

Pour $\alpha \in \mathbf{N}^n$, et $1 \leq j \leq |\alpha|$, on pose :

$$
\alpha(j) = \inf \{ k \in \mathbf{N} \mid 1 \leq k \leq n \text{ et } j > \alpha_1 + \cdots + \alpha_{k-1} \}
$$

(la suite des $\alpha(j)$ s’obtient donc en écrivant $\alpha_1$ fois 1, ..., $\alpha_n$ fois n).

On désigne par $E_\alpha$ l’espace vectoriel topologique produit de la famille des $E_{\alpha(j)}$ pour $1 \leq j \leq |\alpha|$. On désigne par $\mathrm{Hom}_\alpha(E_1, \ldots, E_n; F)$ l’espace des applications $|\alpha|$-multilinéaires de $E_\alpha$ dans F et par $\mathcal{L}_\alpha(E_1, \ldots, E_n; F)$ le sous-espace de $\mathrm{Hom}_\alpha(E_1, \ldots, E_n; F)$ formé des applications multilinéaires continues muni de la topologie de la convergence uniforme sur les parties bornées de $E_\alpha$; c’est un espace polynormé séparé, dont la topologie peut être définie par la famille de semi-normes $\|u\|_y$, où, pour une semi-norme $y$ continue sur F, on note $\|u\|_y$ la borne inférieure des nombres $a \geq 0$ tels que

$$
\|u(x_1, \ldots, x_{|\alpha|})\|_y \leq a \|x_1\| \cdots \|x_{|\alpha|}\|
$$

où chaque $x_j$ parcourt $E_{\alpha(j)}$.

On désigne par $p_i$ la projection canonique de E sur $E_i$. Pour $\alpha \in \mathbf{N}^n$ avec $\alpha \neq 0$, on note $p_\alpha$ l’application $x \mapsto (p_{\alpha(j)}(x))$ de E dans $E_\alpha$.

A.1. Une application $f$ de E dans F est appelée un polynôme multihomogène de multidegré $\alpha$ (avec $\alpha \in \mathbf{N}^n$) sur E à valeurs dans F s’il existe un élément

$$
u \in \mathrm{Hom}_\alpha(E_1, \ldots, E_n; F)
$$

tel que $f = u \circ p_\alpha$.

A.2. On désigne par $P_\alpha(E_1, \ldots, E_n; F)$ l’image de $\mathcal{L}_\alpha(E_1, \ldots, E_n; F)$ par l’application linéaire $u \mapsto u \circ p_\alpha$ de $\mathrm{Hom}_\alpha(E_1, \ldots, E_n; F)$ dans l’espace des applications de E dans F, munie de la topologie quotient de celle de $\mathcal{L}_\alpha(E_1, \ldots, E_n; F)$. Un élément de $P_\alpha(E_1, \ldots, E_n; F)$ est appelé un polynôme-continu multihomogène de multidegré $\alpha$ sur E à valeurs dans F. La topologie de $P_\alpha(E_1, \ldots, E_n; F)$ est définie par la famille de semi-normes :

$$
\|f\|_y = \inf_{u \in \mathcal{L}_\alpha(E_1, \ldots, E_n; F), f = u \circ p_\alpha} \|u\|_y
$$

pour $y$ décrivant l’ensemble des semi-normes continues sur F. Si F est un espace normé, de norme $\gamma$, on écrit $\|f\|$ au lieu de $\|f\|_y$. L’espace $P_\alpha(E_1, \ldots, E_n; F)$ et sa topologie ne changent pas si l’on substitue aux normes données sur chaque $E_i$ des normes équivalentes. On peut donc les définir lorsque les $E_i$ sont des espaces vectoriels topologiques normables.

En particulier, un élément de $P_k(E; F)$ est appelé un polynôme-continu homogène de degré total $k$ sur E à valeurs dans F. L’espace $P_k(E; F)$ est somme directe topologique des espaces $P_\alpha(E_1, \ldots, E_n; F)$ pour $|\alpha| = k$. L’espace $P_0(E; F)$ est l’espace des applications constantes de E dans F et on l’identifie à F.

A.3. On désigne par $P(E; F)$ ou $P(E_1, \ldots, E_n; F)$ le sous-espace vectoriel de l’espace vectoriel de toutes les applications de E dans F engendré par les sous-espaces $P_k(E; F)$.

Il est somme directe des sous-espaces $P_\alpha(E_1, \ldots, E_n; F)$ pour $\alpha \in \mathbf{N}^n$, et aussi des sous-espaces $P_k(E; F)$ pour $k \in \mathbf{N}$. Un élément de $P(E; F)$ est appelé un *polynôme-continu* sur $E$ à valeurs dans $F$.

A.4. Soient $G_j$ des espaces normés (pour $1 \leq j \leq m$). Soient $f_j \in P(E_1, \ldots, E_n; G_j)$ (pour $1 \leq j \leq m$) et soit $g \in P(G_1, \ldots, G_m; F)$. L’application
$$
h : x \mapsto g(f_1(x), \ldots, f_m(x))
$$
appartient à $P(E_1, \ldots, E_n; F)$. Si de plus $f_j \in P_\alpha(E_1, \ldots, E_n; G_j)$ pour $1 \leq j \leq m$ (avec $\alpha \in \mathbf{N}^n$) et $g \in P_\beta(G_1, \ldots, G_m; F)$, (avec $\beta \in \mathbf{N}^m$), on a $h \in P_{|\beta| \alpha}(E_1, \ldots, E_n; F)$ et
$$
\|h\|_\gamma \leq \|g\|_\gamma \cdot \|f\|^\beta
$$
pour toute semi-norme continue $\gamma$ sur $F$ (en posant $\|f\|^\beta = \prod_{1 \leq j \leq m} \|f_j\|^{\beta_j}$).

A.5. On désigne par $\hat{P}(E_1, \ldots, E_n; F)$ l’espace vectoriel produit des $P_\alpha(E_1, \ldots, E_n; F)$ pour $\alpha \in \mathbf{N}^n$, muni de la topologie produit des topologies *discrètes* sur chacun des facteurs. Cette topologie fait de $\hat{P}(E_1, \ldots, E_n; F)$ un groupe topologique séparé *et complet*. L’application linéaire de $P(E_1, \ldots, E_n; F)$ dans $\hat{P}(E_1, \ldots, E_n; F)$ prolongeant les injections canoniques des $P_\alpha(E_1, \ldots, E_n; F)$ est injective et son image est dense dans $\hat{P}(E_1, \ldots, E_n; F)$: on identifie en général un polynôme-continu sur $E$ à valeurs dans $F$ avec son image dans $\hat{P}(E_1, \ldots, E_n; F)$.

L’application identique de $P(E_1, \ldots, E_n; F) = P(E; F)$ se prolonge par continuité en un isomorphisme de $\hat{P}(E_1, \ldots, E_n; F)$ sur $\hat{P}(E; F)$.

Un élément de $\hat{P}(E_1, \ldots, E_n; F)$ est appelé une série *formelle à composantes continues* (ou par abus de langage une série *formelle*) sur le produit des $E_i$ à valeurs dans $F$.

A.6. Soient $G_j$ (pour $1 \leq j \leq m$) des espaces normés et soit $g \in P(G_1, \ldots, G_m; F)$. L’application $f \mapsto g \circ f$ de $\prod_{1 \leq j \leq m} P(E_1, \ldots, E_n; G_j)$ dans $P(E_1, \ldots, E_n; F)$ se prolonge par continuité en une application (notée encore $f \mapsto g \circ f$) de $\prod_{1 \leq j \leq m} \hat{P}(E_1, \ldots, E_n; G_j)$ dans $\hat{P}(E_1, \ldots, E_n; F)$.

Soient $f_j = (f_{j,\alpha})_{\alpha \in \mathbf{N}^n} \in \hat{P}(E_1, \ldots, E_n; G_j)$, avec $f_{j,0} = 0$. Posons $f = (f_j)$: l’application $g \mapsto g \circ f$ de $P(G_1, \ldots, G_m; F)$ dans $\hat{P}(E_1, \ldots, E_n; F)$ se prolonge par continuité en une application (notée encore $g \mapsto g \circ f$) de $\hat{P}(G_1, \ldots, G_m; F)$ dans $\hat{P}(E_1, \ldots, E_n; F)$.
