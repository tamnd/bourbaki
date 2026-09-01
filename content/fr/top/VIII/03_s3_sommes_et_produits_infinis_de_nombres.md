---
book: top
book_title: General Topology
chapter: VIII
chapter_title: NOMBRES COMPLEXES
section: 3
section_title: Sommes et produits infinis de nombres complexes
lang: fr
source: top-v-x-fr
book_pages: TG VIII.15-TG VIII.18
pdf_pages: 0101-0104, 0112-0113
extraction: ocr
subsections:
    - "no": 1
      title: Sommes infinies de nombres complexes
      page: 15
      pdf_page: 101
    - "no": 2
      title: Familles multipliables dans $\mathbf{C}^*$
      page: 16
      pdf_page: 102
    - "no": 3
      title: Produits infinis de nombres complexes
      page: 18
      pdf_page: 104
statements: 9
exercises: 6
content_sha256: dfc5bf42c2a7ee87ba34b689a70b65955af6a338078b9603d340699bb6df4878
---

## § 3. SOMMES ET PRODUITS INFINIS DE NOMBRES COMPLEXES

### 1. Sommes infinies de nombres complexes

Le groupe additif du corps $\mathbf{C}$ étant identique au groupe additif $\mathbf{R}^2$, il n’y a pas à revenir sur l’étude des familles sommables et des séries dans $\mathbf{C}$, qui rentre dans la théorie générale faite dans VII, p. 16–18; nous laissons au lecteur le soin de traduire les résultats de cette théorie dans le langage de la théorie des nombres complexes. Signalons seulement la proposition suivante, corollaire de la prop. 3 de VII, p. 17:

#### Proposition 1 {#top-viii-s3-prop-1 .statement}

Si $(u_\lambda)_{\lambda \in L}$ et $(v_\mu)_{\mu \in M}$ sont deux familles sommables de nombres complexes, la famille $(u_\lambda v_\mu)_{(\lambda, \mu) \in L \times M}$ est sommable, et l’on a

$$
\sum_{(\lambda, \mu) \in L \times M} u_\lambda v_\mu = \left( \sum_{\lambda \in L} u_\lambda \right) \left( \sum_{\mu \in M} v_\mu \right).
$$

Nous laissons au lecteur le soin d’énoncer la proposition analogue pour les quaternions.

### 2. Familles multipliables dans $\mathbf{C}^*$

Dans le groupe multiplicatif $\mathbf{C}^*$ des nombres complexes $\neq 0$, une famille $(z_i)_{i \in I}$ ne peut être multipliable que si $\lim z_i = 1$ suivant le filtre des complémentaires des parties finies de I (III, p. 38, prop. 1); en outre, tout point de $\mathbf{C}^*$ ayant un système fondamental dénombrable de voisinages, l’ensemble des $i$ tels que $z_i \neq 1$ est dénombrable si la famille $(z_i)$ est multipliable (III, p. 38, corollaire).

#### Proposition 2 {#top-viii-s3-prop-2 .statement}

Pour qu’une famille $(z_i)$ de nombres complexes

$$
z_i = r_i (\cos \theta_i + i \sin \theta_i)
$$

soit multipliable dans $\mathbf{C}^*$, il faut et il suffit que la famille $(r_i)$ des valeurs absolues des $z_i$ soit multipliable dans $\mathbf{R}_+^*$, et que la famille $(\theta_i)$ des amplitudes des $z_i$ soit sommable dans le groupe des angles $\mathfrak{A}$.

D’après la structure du groupe $\mathbf{C}^*$ (VIII, p. 4, prop. 1), la proposition est une conséquence immédiate de la prop. 4 de III, p. 41.

L’application qui, à tout angle $\theta$, fait correspondre celle de ses mesures (de base $a$ quelconque) appartenant à l’intervalle $] - a/2, a/2 ]$ est un isomorphisme local de $\mathfrak{A}$ à $\mathbf{R}$ (VIII, p. 10); comme $\lim \theta_i = 0$ suivant le filtre des complémentaires des parties finies de I, on peut, dans l’énoncé de la prop. 2, remplacer la condition que la famille $(\theta_i)$ soit sommable dans $\mathfrak{A}$ par la condition que la famille $(t_i)$ des mesures des angles $\theta_i$ appartenant à $] - a/2, a/2 ]$ soit sommable dans $\mathbf{R}$.

Le théorème suivant donne un autre critère pour qu’une famille de nombres complexes, mise sous la forme $(1 + u_i)$, soit multipliable dans $\mathbf{C}^*$ (critère qui généralise le th. de IV, p. 35; voir IX, p. 81, prop. 1):

#### Théorème 1 {#top-viii-s3-thm-1 .statement}

Pour qu’une famille $(1 + u_i)_{i \in I}$ soit multipliable dans $\mathbf{C}^*$, il faut et il suffit que la famille $(|u_i|)$ soit sommable dans $\mathbf{R}$.

Pour toute partie finie J de I, posons

$$
p_J = \prod_{i \in J} (1 + a_i), \quad s_J = \sum_{i \in J} a_i, \quad \sigma_J = \sum_{i \in J} |a_i|.
$$

#### Lemme 1 {#top-viii-s3-lem-1 .statement}

Pour toute partie finie J de I, soit $\varphi(J) = \sup_{L \subset J} |p_L - 1|$. Pour toute partie L de J, on a
$$
|p_L - 1 - s_L| \leq \varphi(J) \sigma_L.
$$
Le lemme est évident si L est vide; démontrons-le par récurrence sur Card(L). Soit $L = K \cup \{\lambda\}$, où $\lambda \notin K$; alors $p_L = p_K(1 + a_\lambda)$ et $s_L = s_K + a_\lambda$, d’où
$$
p_L - 1 - s_L = (p_K - 1 - s_K) + (p_K - 1)a_\lambda
$$
et en vertu de l’hypothèse de récurrence et de la définition de $\varphi(J)$
$$
|p_L - 1 - s_L| \leq \varphi(J)\sigma_K + \varphi(J)|a_\lambda| = \varphi(J)\sigma_L,
$$
ce qui prouve le lemme.

#### Lemme 2 {#top-viii-s3-lem-2 .statement}

Si J est une partie finie de I telle que $\varphi(J) < \frac{1}{4}$, on a
$$
|\sigma_J| \leq 4\varphi(J)/(1 - 4\varphi(J)).
$$
En effet, comme $\sigma_L \leq \sigma_J$ pour toute partie L de J, on a, d’après (2),
$$
|s_L| \leq \varphi(J)\sigma_J + |p_L - 1| \leq (1 + \sigma_J)\varphi(J);
$$
mais en vertu de VII, p. 16, prop. 2, on a $|\sigma_J| \leq 4 \sup_{L \subset J} |s_L|$, donc on en déduit $\sigma_J \leq 4\varphi(J)(1 + \sigma_J)$, d’où le lemme.

Cela étant, prouvons d’abord que la condition de l’énoncé du th. 1 est suffisante. L’hypothèse entraîne que la famille $(1 + |u_i|)$ est multipliable dans $\mathbf{R}_+^*$ (IV, p. 35, th. 4); pour tout $\varepsilon > 0$, il y a donc une partie finie $J_0$ de I telle que, pour toute partie finie L de I ne rencontrant pas $J_0$, on ait
$$
\prod_{i \in L} (1 + |u_i|) - 1 \leq \varepsilon.
$$
Mais on peut écrire $\prod_{i \in L} (1 + u_i) - 1 = \sum_M \left( \prod_{i \in M} u_i \right)$, où M parcourt l’ensemble des parties non vides de L; comme $\left| \prod_{i \in M} u_i \right| = \prod_{i \in M} |u_i|$, on a
$$
\left| \prod_{i \in L} (1 + u_i) - 1 \right| \leq \sum_M \left( \prod_{i \in M} |u_i| \right) = \prod_{i \in L} (1 + |u_i|) - 1 \leq \varepsilon
$$
ce qui prouve notre assertion en vertu du critère de Cauchy, puisque $\mathbf{C}^*$ est un groupe complet.

Montrons maintenant que la condition est nécessaire. En effet, si $(1 + u_i)_{i \in I}$ est une famille multipliable dans $\mathbf{C}^*$, il existe une partie finie J de I telle que, pour toute partie finie H de I ne rencontrant pas J, on ait $\left| \prod_{i \in H} (1 + u_i) - 1 \right| \leq \frac{1}{8}$. D’après le lemme 2, on en déduit $\sum_{i \in H} |u_i| \leq 1$ pour toute partie finie H de I ne rencontrant pas J, ce qui entraîne que la famille $(|u_i|)$ est sommable dans $\mathbf{R}$ (IV, p. 32, th. 1).

Nous donnerons plus tard de ce théorème une démonstration plus simple, fondée sur les propriétés différentielles des fonctions exponentielles et logarithmiques (FVR, V, § 4, n° 3). L’avantage de la démonstration précédente est que son principe s’applique aussi à des produits infinis (ordonnés) dans certains corps et algèbres non commutatifs (voir IX, p. 78).

### 3. Produits infinis de nombres complexes

Pour qu’un produit infini de nombres complexes $\neq 0$, de facteur général $z_n = r_n (\cos \theta_n + i \sin \theta_n)$ soit convergent dans $\mathbf{C}^*$, il faut et il suffit d’après la structure du groupe $\mathbf{C}^*$, que le produit de facteur général $r_n$ soit convergent dans $\mathbf{R}_+^*$, et que la série de terme général $t_n$ (mesure de $\theta_n$ appartenant à l’intervalle $] - a/2, a/2 ]$) soit convergente dans $\mathbf{R}$.

#### Définition 1 {#top-viii-s3-def-1 .statement}

Un produit infini de nombres complexes, de facteur général $1 + u_n$, est dit absolument convergent, si le produit de facteur général $1 + |u_n|$ est convergent (ou, ce qui revient au même, si la série de terme général $|u_n|$ est convergente).

#### Proposition 3 {#top-viii-s3-prop-3 .statement}

Pour qu’un produit infini de nombres complexes soit commutativement convergent, il faut et il suffit qu’il soit absolument convergent.

Cela résulte de la prop. 9 de III, p. 44, et du th. 1 de VIII, p. 16.

#### Remarque 1 {#top-viii-s3-n3-rem-1 .statement}

Le produit de facteur général $|1 + u_n|$ peut être convergent, et même absolument convergent dans $\mathbf{R}_+^*$, sans que le produit de facteur général $1 + |u_n|$ le soit (voir VIII, p. 26, exerc. 4); cela ne peut naturellement se produire lorsque tous les $1 + u_n$ sont réels et $> 0$ à partir d’un certain rang.

#### Remarque 2 {#top-viii-s3-n3-rem-2 .statement}

Comme on l’a déjà signalé pour les produits de facteurs $> 0$, la convergence de la série de terme général $u_n$ n’est ni nécessaire ni suffisante pour assurer la convergence du produit de facteur général $1 + u_n$.

## EXERCICES {#top-viii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
