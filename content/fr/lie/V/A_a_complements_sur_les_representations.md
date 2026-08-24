---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: V
chapter_title: Groupes engendrés par des réflexions
section: 0
section_title: Compléments sur les représentations linéaires
appendix: true
lang: fr
source: lie-iv-vi-fr
pdf_pages: 0123-0126
extraction: ocr
statements: 4
exercises: 0
content_sha256: 5030e6ba635c4b042a90838c91b709300aa5b48183891f0ac0f0d2ce8c2cc151
---

## ANNEXE

# COMPLÉMENTS SUR LES REPRÉSENTATIONS LINÉAIRES

La proposition suivante généralise la prop. 13 du chap. I, § 3, n° 8.

#### Proposition 1 {#lie-v-a0-prop-1 .statement}

Soient K un corps commutatif, A une K-algèbre, V et W deux A-modules à gauche qui sont des espaces vectoriels de dimension finie sur K. S’il existe une extension L de K telle que les (A \otimes_K L)-modules V \otimes_K L et W \otimes_K L soient isomorphes, alors les A-modules V et W sont isomorphes.

a) Supposons d’abord que L soit une extension de K de degré fini n. Comme V \otimes_K L et W \otimes_K L sont isomorphes en tant que (A \otimes_K L)-modules, ils sont isomorphes en tant que A-modules; mais, en tant que A-modules, ils sont isomorphes respectivement à V^n et W^n. Or V et W sont des A-modules de longueur finie; donc V (resp. W) est somme directe d’une famille (M_i^{r_i})_{1 \leq i \leq p} (resp. (N_j^{s_j})_{1 \leq j \leq q}) de sous-modules tels que les M_i (resp. N_j) soient indécomposables, et que deux M_i (resp. N_j) d’indices distincts soient non isomorphes (Alg., chap. VIII, § 2, n° 2, th. 1). Alors V^n (resp. W^n) est somme directe des M_i^{n r_i} (resp. N_j^{n s_j}); on en conclut (loc. cit.) que p = q et qu’après permutation éventuelle des N_j, M_i est isomorphe à N_i et n r_i égal à n s_i pour 1 \leq i \leq p. Donc V est isomorphe à W.

b) Supposons que K soit un corps infini. L’hypothèse entraîne que V et W ont même dimension sur K. Soient (e_i)_{1 \leq i \leq m}, (e'_i)_{1 \leq i \leq m} des bases de V et W sur K, (a_\lambda) une base de A sur K. Un isomorphisme u : V \otimes_K L \to W \otimes_K L est une application L-linéaire bijective qui est en même temps un (A \otimes_K L)-homomorphisme, autrement dit qui vérifie les conditions :

(1)
$$
a_\lambda u(e_i) = u(a_\lambda e_i) \quad \text{pour tout } \lambda \text{ et tout } i.
$$

Posons $ a_\lambda e_i = \sum_j \gamma_{\lambda i j} e_j, \quad a_\lambda e'_i = \sum_j \gamma'_{\lambda i j} e'_j, $ où les $ \gamma_{\lambda i j} $ et $ \gamma'_{\lambda i j} $ appartiennent à K,
et $ u(e_i) = \sum_j \xi_{i j} e'_j, $ où les $ \xi_{i j} $ appartiennent à L. Les conditions (1) s’écrivent

(2)
$$
\sum_j \xi_{i j} \gamma'_{\lambda j k} = \sum_j \gamma_{\lambda i j} \xi_{j k}
$$

quels que soient $ \lambda, i, k $. Par hypothèse, les équations linéaires homogènes (2) ont une solution $ (\xi_{ij}) \in L^{m^*} $ telle que $ \det(\xi_{ij}) \neq 0 $. Comme les coefficients du système (2) appartiennent à $ K $, on sait (Alg., chap. II, 3e éd., § 8, no 5, prop. 6) que ce système admet aussi des solutions non triviales dans $ K^{m^*} $; soit $ E $ le sous-espace vectoriel de $ M_m(K) = K^{m^*} $, non réduit à 0, formé par ces solutions. Soit $ (c_l)_{1 \leq l \leq p} $ une base de $ E $, et posons $ (\xi_{ij}) = \sum_i \eta_i c_i $ pour toute matrice $ (\xi_{ij}) \in E $; alors $ \det(\xi_{ij}) $ est un polynôme $ P(\eta_1, \eta_2, \ldots, \eta_p) $ à coefficients dans $ K $. En outre, on sait (loc. cit.) que les solutions de (2) dans $ L^{m^*} $ sont de la forme $ \sum_i \zeta_i c_i $, avec cette fois $ \zeta_i \in L $; pour une telle solution, $ \det(\xi_{ij}) $ est égal à $ P(\zeta_1, \ldots, \zeta_p) $. Ceci posé, si on avait $ P(\eta_1, \ldots, \eta_p) = 0 $ quels que soient $ \eta_1, \ldots, \eta_p \in K $, les coefficients de $ P $ seraient nuls puisque $ K $ est infini; on aurait alors $ P(\zeta_1, \ldots, \zeta_p) = 0 $ quels que soient $ \zeta_1, \ldots, \zeta_p \in L $, ce qui est contraire à l’hypothèse. On peut donc trouver une matrice $ (\xi_{ij}) \in E $ telle que $ \det(\xi_{ij}) \neq 0 $, et l’application linéaire correspondante $ V \to W $ est un isomorphisme.

c) *Cas général.* Soient $ \Omega $ une extension algébriquement close de $ L $, $ K_0 $ la clôture algébrique de $ K $ dans $ \Omega $. L’hypothèse entraîne que $ V \otimes_K \Omega $ et $ W \otimes_K \Omega $ sont des $ (A \otimes_K \Omega) $-modules isomorphes. Comme $ K_0 $ est infini, la partie b) montre que $ V \otimes_K K_0 $ et $ W \otimes_K K_0 $ sont des $ (A \otimes_K K_0) $-modules isomorphes. Gardant les notations de b), le système (2) admet une solution $ (\xi_{ij}) \in K_0^{m^*} $ telle que $ \det(\xi_{ij}) \neq 0 $. Mais les $ \xi_{ij} $ appartiennent à une même extension algébrique $ K_1 $ de degré fini de $ K $. Les $ (A \otimes_K K_1) $-modules $ V \otimes_K K_1 $ et $ W \otimes_K K_1 $ sont isomorphes, et on conclut à l’aide de a).

**Proposition 2** (Maschke). — *Soient A un anneau ayant un élément unité, E un A-module à gauche, F un sous-module facteur direct, G un groupe fini d’ordre q, ρ une représentation linéaire de G dans E. On suppose que q.1 est inversible dans A et que F est stable par G. Il existe alors un supplémentaire de F dans E stable par G.*

Soit $ p $ un projecteur de $ E $ sur $ F $. Pour tout $ x \in E $, posons

$$
f(x) = q^{-1} \sum_{s \in G} \rho(s)^{-1} p(\rho(s)x).
$$

On a $ f(x) \in F $ et $ f(y) = y $ pour tout $ y \in F $, donc $ f $ est un projecteur de $ E $ sur $ F $. D’autre part, si $ t \in G $, on a

$$
\begin{align*}
\rho(t)f(x) &= q^{-1} \sum_{s \in G} \rho(st^{-1})^{-1} p(\rho(s)x) \\
&= q^{-1} \sum_{s \in G} \rho(s)^{-1} p(\rho(st)x) \\
&= f(\rho(t)x).
\end{align*}
$$

Donc $ f $ commute à $ \rho(G) $, de sorte que $ \operatorname{Ker} f $ est un supplémentaire de $ E $ stable par $ G $.

#### Corollaire {#lie-v-a0-n0-cor-1 .statement}

Soient $ G $ un groupe fini d’ordre $ q $, $ K $ un corps commutatif dont la caractéristique ne divise pas $ q $. Alors l’algèbre de $ G $ relativement à $ K $ est semi-simple.
En effet, d’après la prop. 2, tout module sur cette algèbre est semi-simple.

#### Proposition 3 {#lie-v-a0-prop-3 .statement}

Soient $ A $ un anneau commutatif, $ M $ un $ A $-module, $ G $ un groupe fini opérant dans $ M $, et $ A' $ un $ A $-module. On suppose que l’ordre $ q $ de $ G $ est inversible dans $ A $.
Soit $ M^G $ l’ensemble des éléments de $ M $ invariants par $ G $. Alors l’homomorphisme canonique de $ M^G \otimes_A A' $ dans $ M \otimes_A A' $ définit un isomorphisme de $ M^G \otimes_A A' $ sur le module $ (M \otimes_A A')^G $ des éléments de $ M \otimes_A A' $ invariants par $ G $.
En effet, soit $ Q $ le projecteur de $ M $ sur $ M^G $ défini par $ Q(x) = q^{-1} \sum_{g \in G} g(x) $ pour tout $ x \in M $. Si $ i $ désigne l’injection canonique de $ M^G $ dans $ M $, $ Q \circ i $ est l’application identique de $ M^G $, donc $ (Q \otimes 1_{A'}) \circ (i \otimes 1_{A'}) $ est l’application identique de $ M^G \otimes_A A' $. Comme $ Q \otimes 1_{A'} = q^{-1} \sum_{g \in G} (g \otimes 1_{A'}) $, l’image de $ i \otimes 1_{A'} $ est $ (M \otimes A')^G $. D’autre part, $ i \otimes 1_{A'} $ est injectif d’après ce qui précède.

#### Remarque {#lie-v-a0-n0-rem-1 .statement}

La proposition précédente s’applique notamment lorsque $ A' $ est une $ A $-algèbre. Dans ce cas, $ M^G \otimes_A A' $ est un sous-$ A' $-module de $ M \otimes_A A' $.

Exercises
