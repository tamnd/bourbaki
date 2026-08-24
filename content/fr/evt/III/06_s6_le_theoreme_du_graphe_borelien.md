---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: ESPACES D’APPLICATIONS LINÉAIRES CONTINUES
section: 6
section_title: Le théorème du graphe borélien
lang: fr
source: evt-i-v-fr
book_pages: EVT III.50-EVT III.51
pdf_pages: 0169-0173, 0185-0186
extraction: ocr
subsections:
    - "no": 1
      title: Le théorème du graphe borélien
      page: 34
      pdf_page: 169
    - "no": 2
      title: Espaces localement convexes lusiniens
      page: 35
      pdf_page: 170
    - "no": 3
      title: Applications linéaires mesurables sur un espace de Banach¹
      page: 36
      pdf_page: 171
statements: 8
exercises: 6
content_sha256: 65a02eb27ea20638633e6046ecf9cd54842558a6fede6ce1afd230d1dc20a47f
---

## § 6. LE THÉORÈME DU GRAPHE BORÉLIEN

### 1. Le théorème du graphe borélien

#### Théorème 1 {#evt-iii-s6-thm-1 .statement}

Soient E un espace localement convexe limite inductive d’espaces de Banach, F un espace localement convexe souslinien, par exemple lusinien (TG, IX, p. 59 et p. 62), et u une application linéaire de E dans F. Si le graphe de u est un sous-ensemble borélien de $ E \times F $, alors u est continue.
Soient $ (E_i) $ une famille d’espaces de Banach et $ (u_i) $ une famille d’applications linéaires continues $ u_i : E_i \to E $ telles que la topologie de E soit la topologie localement convexe la plus fine rendant continues les $ u_i $. Il suffit de démontrer que les applications composées $ u \circ u_i $ sont continues, ou encore (TG, IX, p. 17, prop. 10) que la restriction de $ u \circ u_i $ à tout sous-espace fermé de type dénombrable G de $ E_i $ est continue. Le graphe de cette restriction est l’image réciproque du graphe de u par l’application continue $ u_i \times \mathrm{Id}_F : G \times F \to E \times F $, donc est borélien dans $ G \times F $. De plus $ G \times F $ est un espace souslinien et toute partie borélienne d’un espace souslinien est souslinienne (TG, IX, p. 61, prop. 10). Le th. 1 résulte alors du th. 4 de TG, IX, p. 69.

#### Remarque {#evt-iii-s6-n1-rem-1 .statement}

Rappelons (III, p. 12) que tout espace bornologique séparé et semi-complet, par exemple tout espace de Fréchet, est limite inductive d’espaces de Banach.
\* Il en est de même du dual fort d’un espace de Fréchet réflexif (IV, p. 23, prop. 4). \*

### 2. Espaces localement convexes lusiniens

#### Proposition 1 {#evt-iii-s6-prop-1 .statement}

Soit E un espace localement convexe séparé. On suppose qu’il existe une suite $(E_n)_{n \in \mathbf{N}}$ d’espaces de Fréchet de type dénombrable, et des applications linéaires continues $u_n : E_n \to E$ telles que $E = \bigcup_{n \in \mathbf{N}} u_n(E_n)$. Alors E est lusinien.

Soit $P_n$ le noyau de $u_n$; alors $u_n$ définit par passage au quotient une application bijective continue de $E_n/P_n$ sur $u_n(E_n)$. Comme $E_n/P_n$ est un espace de Fréchet de type dénombrable (TG, IX, p. 25), donc polonais (TG, IX, p. 57, déf. 1), $u_n(E_n)$ est un sous-espace lusinien de E (TG, IX, p. 62, prop. 11). En vertu de TG, IX, p. 68, cor. du th. 3, l’espace E, qui est régulier (TG, III, p. 20), est donc lusinien.

#### Exemple 1 {#evt-iii-s6-n2-exa-1 .statement}

Tout espace de Fréchet de type dénombrable est polonais, donc lusinien. Sont par suite lusiniens les espaces $\mathscr{C}(X)$ où X est localement compact à base dénombrable (la topologie de $\mathscr{C}(X)$ étant celle de la convergence compacte, cf. TG, X, p. 25, corollaire et p. 9, cor. 3); \* les espaces $\mathscr{C}^\infty(U)$, où U est une partie ouverte de $\mathbf{R}^n$ (III, p. 9) et $\mathscr{H}(U)$, où U est une partie ouverte de $\mathbf{C}^n$ (III, p. 10).

La prop. 1 montre alors que sont lusiniens les espaces $\mathscr{C}_0^\infty(U)$, où U est ouvert dans $\mathbf{R}^n$ (III, p. 10), $\mathscr{G}_s(I)$, où I est un intervalle compact de $\mathbf{R}$ et $s \geq 1$ (III, p. 10) et $\mathscr{H}(K)$, où K est une partie compacte de $\mathbf{C}^n$ (III, p. 10). \*

#### Théorème 2 {#evt-iii-s6-thm-2 .statement}

Soit E un espace localement convexe, limite inductive d’une suite croissante $(E_n)_{n \in \mathbf{N}}$ de sous-espaces de E, munis de topologies d’espaces de Fréchet de type dénombrable. On suppose que toute partie compacte de E est contenue dans l’un des $E_n$ et compacte dans cet espace. Soit F un espace de Fréchet de type dénombrable. Alors l’espace $\mathscr{L}_c(E; F)$ est lusinien.

L’espace E est bornologique (III, p. 12), donc l’espace $\mathscr{L}_c(E; F)$ est complet (III, p. 23, prop. 12). L’application linéaire $j : f \mapsto (f|E_n)_{n \in \mathbf{N}}$ est une injection de $\mathscr{L}_c(E; F)$ dans l’espace produit $\prod_{n \in \mathbf{N}} \mathscr{L}_c(E_n; F)$; en vertu de l’hypothèse sur les parties compactes de E et de la définition des $\mathfrak{S}$-topologies, j est un isomorphisme de $\mathscr{L}_c(E; F)$ sur son image (munie de la topologie induite par la topologie produit); en outre, puisque $\mathscr{L}_c(E; F)$ est complet, cette image est un sous-espace fermé de $\prod_{n \in \mathbf{N}} \mathscr{L}_c(E_n; F)$ (TG, II, p. 16, prop. 8). D’après TG, IX, p. 62, il suffit donc de prouver que chacun des espaces $\mathscr{L}_c(E_n; F)$ est lusinien. Pour la suite de la démonstration, on supposera donc que E est un espace de Fréchet de type dénombrable.

Comme F est un espace de Fréchet de type dénombrable, il est isomorphe à un sous-espace fermé d’un produit dénombrable d’espaces de Banach $F_n$, dont chacun est un quotient de F (II, p. 5), donc de type dénombrable. L’application linéaire $j' : f \mapsto (\mathrm{pr}_n \circ f)_{n \in \mathbf{N}}$ est une injection de $\mathscr{L}_c(E; F)$ dans l’espace produit $\prod_{n \in \mathbf{N}} \mathscr{L}_c(E; F_n)$, et en vertu de la définition des $\mathfrak{S}$-topologies et des ouverts dans un produit, $j'$ est un isomorphisme de $\mathscr{L}_c(E; F)$ sur son image; en outre, puisque $\mathscr{L}_c(E; F)$ est complet, cette image est un sous-espace fermé de $\prod_{n \in \mathbf{N}} \mathscr{L}_c(E; F_n)$. Il suffira donc de prouver que chacun des $\mathscr{L}_c(E; F_n)$ est lusinien (TG, IX, p. 62), et on peut par suite supposer que F est un espace de Banach de type dénombrable.

L’espace $ \mathcal{L}_c(E; F) $ est alors réunion d’une famille dénombrable de parties équicontinues et fermées (III, p. 19, cor. 1 et TG, X, p. 15, prop. 6). Or toute partie équicontinue H de $ \mathcal{L}_c(E; F) $ est métrisable de type dénombrable (III, p. 18, prop. 6 et TG, X, p. 16, th. 1); si H est fermée, c’est un espace complet pour la structure uniforme induite par celle de $ \mathcal{L}_c(E; F) $, puisque ce dernier est complet. Autrement dit, H est un espace polonais, et *a fortiori* lusinien ; par suite l’espace régulier $ \mathcal{L}_c(E; F) $ est lusinien (TG, IX, p. 68, cor. du th. 3).

#### Corollaire {#evt-iii-s6-n2-cor-1 .statement}

*Les hypothèses sur E étant celles du th. 2, supposons de plus que toute partie bornée de E soit relativement compacte. Alors le dual fort de E est lusinien.* *En particulier, le dual fort d’un espace de Fréchet de type dénombrable qui est aussi un espace de Montel, est lusinien.*

\* Exemple 2. — Soit U une partie ouverte de $ \mathbf{R}^n $. Le corollaire s’applique en particulier à l’espace de Fréchet $ E = \mathscr{C}^\infty(U) $; son dual $ \mathscr{C}_o^{-\infty}(U) $ (espace des distributions à support compact sur U) est donc un espace lusinien.

L’espace $ \mathscr{C}_o^\infty(U) $ est limite inductive stricte d’une suite d’espaces de Fréchet $ \mathscr{C}_{K_n}^\infty(U) $ de type dénombrable (III, p. 9). On peut montrer que chacun des espaces $ \mathscr{C}_{K_n}^\infty(U) $ est un espace de Montel ; de plus, toute partie bornée de $ \mathscr{C}_o^\infty(U) $ est contenue dans l’un des espaces $ \mathscr{C}_{K_n}^\infty(U) $ (III, p. 5, prop. 6). On peut donc appliquer le corollaire du th. 2. Le dual $ \mathscr{C}^{-\infty}(U) $ de $ \mathscr{C}_o^\infty(U) $ (espace des distributions sur U) est donc lusinien pour la topologie forte.

On prouve de même que pour toute partie ouverte U de $ \mathbf{C}^n $, et toute partie compacte K de $ \mathbf{C}^n $, le dual fort de $ \mathscr{H}(U) $ et le dual fort de $ \mathscr{H}(K) $ sont lusiniens. \*

#### Remarque {#evt-iii-s6-n2-rem-1 .statement}

Soit E comme dans le th. 2 ; soit F un espace localement convexe séparé, réunion des images d’une suite d’applications linéaires continues $ u_n : F_n \to F $, où chaque $ F_n $ est un espace de Fréchet de type dénombrable ; alors $ \mathcal{L}_c(E; F) $ est lusinien. Comme dans la prop. 1, on se ramène au cas où chaque $ u_n $ est injective ; puis, comme dans la preuve du th. 2, on peut supposer que E est un espace de Fréchet de type dénombrable. En vertu de I, p. 20, prop. 1, $ \mathcal{L}(E; F) $ est alors réunion des $ \mathcal{L}(E; F_n) $; en outre, l’injection canonique $ \mathcal{L}_c(E; F_n) \to \mathcal{L}_c(E; F) $ est continue (TG, X, p. 5, prop. 3). Comme chaque espace $ \mathcal{L}_c(E; F_n) $ est lusinien d’après le th. 2, $ \mathcal{L}(E; F_n) $ est aussi lusinien pour la topologie induite par celle de $ \mathcal{L}_c(E; F) $ (TG, IX, p. 62, prop. 11); $ \mathcal{L}_c(E; F) $ est par suite lusinien en vertu de TG, IX, p. 68, corollaire du th. 3.

### \*3. Applications linéaires mesurables sur un espace de Banach¹

#### Proposition 2 {#evt-iii-s6-prop-2 .statement}

*Soient E un espace de Banach, F un espace localement convexe et u une application linéaire de E dans F. On suppose que, pour toute partie fermée B de F, tout compact X de E et toute mesure $ \mu $ sur X, l’intersection $ X \cap u^{-1}(B) $ est $ \mu $-mesurable. Alors u est continue.*

Supposons tout d’abord que F est le corps de base. Pour tout compact X de E et toute mesure $ \mu $ sur X, la restriction de u à X est $ \mu $-mesurable (INT, IV). Supposons que u ne soit pas continue. On peut alors trouver une suite de points $ (x_n) $ de E telle que $ \sum_n \|x_n\| < \infty $ et $ |u(x_n)| \geq n $ pour tout entier n. Considérons l’application

¹ Les résultats de ce numéro dépendent du livre d’Intégration.

g : (t_n) \mapsto \sum_n t_n x_n du cube C = \{0, 1\}^\mathbf{N} dans E ; il est clair que g est continue. Par suite f = u \circ g est mesurable pour toute mesure sur C (INT, V), en particulier pour la mesure $ \mu $ produit des mesures de Lebesgue sur les facteurs de C. Il existe donc une partie compacte D de C telle que $ \mu(D) > \frac{1}{2} $ et que la restriction de f à D soit continue, donc bornée. Soit M la borne supérieure de $ |f| $ sur D et soit $ p \in \mathbf{N} $ tel que $ p \geq 4M $. Soient $ s = (s_n) $ et $ t = (t_n) $ deux points de D tels que $ s_n = t_n $ pour $ n \neq p $. On a

$$
f(s) - f(t) = u(\sum_n s_n x_n - \sum_n t_n x_n) = (s_p - t_p) u(x_p) .
$$

Comme $ |f(s) - f(t)| \leq 2M $ et $ |u(x_p)| \geq p \geq 4M $, on en déduit

$$
|s_p - t_p| \leq \frac{1}{2} .
$$

Le th. de Lebesgue-Fubini (INT, V, 2e éd., § 8, no 3, cor. 2 de la prop. 7) entraîne alors $ \mu(D) \leq \frac{1}{2} $, d’où une contradiction. Par suite, $ u $ est bien continue.

Passons maintenant au cas général. Pour tout $ v \in F' $, la forme linéaire $ v \circ u $ est continue d’après ce qui précède. Soit $ (x_n)_{n \in \mathbf{N}} $ une suite de points de E tendant vers 0 ; la suite $ (u(x_n))_{n \in \mathbf{N}} $ tend alors vers 0 dans F muni de la topologie $ \sigma(F, F') $ ; elle est donc bornée pour $ \sigma(F, F') $ et par suite elle est bornée dans F (III, p. 28, cor. 3). Comme E est bornologique (III, p. 12, prop. 2), l’application linéaire $ u : E \to F $ est continue.

Exercises

## EXERCICES {#evt-iii-s6-exercises}

See the [exercises for § 6](exercises/s6/).
