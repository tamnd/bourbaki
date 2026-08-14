---
book: ts
book_title: Théories spectrales
chapter: II
chapter_title: GROUPES LOCALEMENT COMPACTS COMMUTATIFS
section: 0
section_title: GROUPES LOCALEMENT COMPACTS COMMUTATIFS
kind: front
lang: fr
source: ts-i-ii-fr
book_pages: A II.199-A II.200
pdf_pages: 0211-0212
extraction: native
statements: 0
exercises: 0
content_sha256: 29ae5756e4274b0cc9d0a00975d3dadb705f894055c8de00b1f1aeaeb88e2079
---

## CHAPITRE II

# Groupes localement compacts commutatifs

Dans tout ce chapitre, la lettre G désigne, sauf mention du contraire, un groupe localement compact commutatif muni d’une mesure de Haar notée généralement $dx$; pour $p\in [1,+\infty ]$, l’espace $L^p(G, dx)$ sera simplement noté $L^p(G)$, et sa norme sera notée $f\mapsto  \|f\|_p$. On identifie $L^1(G)$ à un sous-espace de $\mathscr{M}^1(G)$ par l’application $f\mapsto f\cdot dx$. On rappelle que le support de la mesure de Haar est égal à G (INT, VII, §1, n$^o1$, remarque 3) ; en particulier (INT, III, §2, n$^o2$, proposition 9), l’application canonique de l’espace $\mathscr{K}(G)$ dans $L^p(G)$ est injective pour $p\in [1,+\infty ]$. Pour $p\not= +\infty$, on identifiera $L^p(G)$ à un sous-espace de l’espace $\widetilde{\mathscr{F}}(G;\mathbf{C})$ des classes de fonctions à valeurs complexes sur G définies et finies presque partout (INT, IV, §3, n$^o5$, n$^o6)$. En particulier, la notation $L^1(G)\cap L^2(G)$ désigne l’intersection de $L^1(G)$ et $L^2(G)$ dans cet espace. On note $f\mapstochar \rightarrow \widetilde{f}$ l’involution sur l’algèbre involutive $L^1(G)$ (exemple 4 de I, p. 99) ; on a $\widetilde{f}(x) =f(x^{-1})$ pour tout $x$ dans G.

On rappelle (INT, V, §5, n$^o3$, th. 1) que si $\mu$ est une mesure complexe sur un espace topologique localement compact X et si $f$ est une fonction localement $\mu$-intégrable sur X, alors la mesure $\nu$ de densité $f$ par rapport à $\mu$ est notée $f\cdot \mu$ ou encore $f \mu$. Une fonction $g$ de X dans $\mathbf{C}$ est essentiellement intégrable pour la mesure $\nu$ si, et seulement si, $gf$ est essentiellement intégrable pour $\mu$; on a alors

$$
(f\cdot \mu)(g) =\int_Xgd(f\cdot \mu) =\int_Xgf d\mu=\mu(gf)
$$

Si G est un groupe topologique compact, on appelle mesure de Haar normalisée sur G l’unique mesure de Haar $\mu$ sur G telle que $\mu(G) = 1$.

Si X est un espace topologique discret, on appelle mesure de comptage sur X la mesure discrète $\mu$ sur X telle que $\mu(\{x\}) = 1$ pour tout $x\in X$. Si G est un groupe topologique discret, la mesure de comptage sur G est une mesure de Haar sur G.

Nous ferons aussi usage des deux lemmes suivants.

**Lemme 1.** — Soient X un espace topologique localement compact et $\mu$ une mesure positive sur X. Soit $x$ un élément du support de $\mu$. Soit U un voisinage ouvert de $x$. Il existe une fonction $f\in \mathscr{K}_+(X)$ de support contenu dans U telle que $\int f d\mu= 1$.

Par définition du support d’une mesure (INT, III, §2, n$^o2$, déf. 1), il existe une fonction $g\in \mathscr{K}(X)$ à support contenu dans U telle que $\mu(g)\not= 0$. On a alors $\mu(|g|)>0$ puisque $\mu$ est positive, et la fonction $f=\mu(|g|)^{-1}|g|$ a les propriétés voulues.

**Lemme 2.** — Soient G et H des groupes topologiques d’éléments neutres $e_G$ et $e_H$; supposons que le groupe topologique G est séparé. Soit $f$ un morphisme de groupes topologiques de G dans H. Supposons que pour tout voisinage U de $e_G$ dans G, il existe un voisinage W de

$-1$

$e_H$ dans H tel que $f(W)\subset U$. Alors, le morphisme $f$ est injectif et strict (TG, III, p. 16, déf. 1).

Les hypothèses impliquent que Ker($f$) est contenu dans tout voisinage de $e_G$ dans G, donc que Ker($f$) $=\{e_G\}$ puisque G est séparé. L’homomorphisme de G dans $f(G)$ déduit de $f$ par passage aux sous-espaces est alors bijectif ; notons $g:f(G)\rightarrow G$ l’homomorphisme réciproque. Les hypothèses entraînent alors que $g$ est continu en $e_H$, donc continu (TG, III, p. 15, prop. 23).
