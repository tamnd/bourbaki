---
book: int
book_title: Integration
chapter: V
chapter_title: Intégration des mesures
section: 2
section_title: Familles sommables de mesures positives
lang: fr
source: int-v-fr
pdf_pages: 0017-0021, 0109-0109
extraction: ocr
subsections:
    - "no": 1
      title: Définition des familles sommables de mesures
      page: 0
      pdf_page: 17
    - "no": 2
      title: Intégration par rapport à une somme de mesures positives
      page: 0
      pdf_page: 18
    - "no": 3
      title: Décomposition d’une mesure en somme de mesures à supports compacts
      page: 0
      pdf_page: 20
statements: 12
exercises: 4
content_sha256: 03f0941434ec8b948e9def7b5701827263f136902378b12840888ea1d359c421
---

## § 2. Familles sommables de mesures positives

### 1. Définition des familles sommables de mesures

Soit $(\lambda_\alpha)_{\alpha \in A}$ une famille de mesures positives sur un espace localement compact X ; on dit que la famille $(\lambda_\alpha)_{\alpha \in A}$ est une famille sommable de mesures si elle est sommable dans l’espace vectoriel $\mathcal{M}(X)$ des mesures réelles sur X, muni de la topologie vague (Top. Gén., chap. III, 3e éd., § 5, n° 1). Cela revient à dire que, pour toute fonction $f \in \mathcal{H}(X)$, la famille des nombres $\lambda_\alpha(f)$ est sommable dans $\mathbf{R}$. En effet, cette condition est évidemment nécessaire ; inversement, si elle est réalisée, la forme linéaire $f \mapsto \sum_{\alpha \in A} \lambda_\alpha(f)$ sur $\mathcal{H}(X)$ est positive, c’est donc une mesure positive $\nu$ (chap. III, 2e éd., § 3, th. 1), et l’on vérifie aussitôt que les sommes partielles finies de la famille $(\lambda_\alpha)$ convergent vaguement vers $\nu$, suivant le filtre des sections de l’ensemble des parties finies de A (Top. Gén., chap. III, 3e éd., § 5, n° 1, déf. 1).

Tout élément de $\mathcal{H}(X)$ étant différence de deux éléments de $\mathcal{H}_+(X)$, la famille $(\lambda_\alpha)$ est sommable si et seulement si l’on a

(1)
$$
\sum_{\alpha \in A} \lambda_\alpha(f) < +\infty
$$
pour toute fonction $f \in \mathcal{H}_+(X)$. Cette condition équivaut encore à la suivante :

(2)
$$
\sum_{\alpha \in A} \lambda_\alpha(K) < +\infty
$$
pour tout compact $K \subset X$.

#### Remarque 1 {#int-v-s2-n1-rem-1 .statement}

Il est immédiat que, lorsque la famille $(\lambda_\alpha)_{\alpha \in A}$ est sommable, sa somme est la borne supérieure, dans $\mathcal{M}_+(X)$, des sommes partielles finies $\sum_{\alpha \in J} \lambda_\alpha$, où J parcourt l’ensemble des parties finies de A.

#### Remarque 2 {#int-v-s2-n1-rem-2 .statement}

Soit $(\theta_\alpha)_{\alpha \in A}$ une famille de mesures complexes sur X ; on dira que la famille $(\theta_\alpha)$ est sommable si la famille $(|\theta_\alpha|)$ de mesures positives est sommable ; *il ne suffit pas pour cela* que la famille $(\theta_\alpha)$ soit sommable dans l’espace vectoriel $\mathcal{M}(X; \mathbf{C})$ muni de la topologie vague (cf. exerc. 3).

### 2. Intégration par rapport à une somme de mesures positives

Dans tout ce numéro, X désigne un espace localement compact, $(\lambda_\alpha)_{\alpha \in A}$ une famille sommable de mesures positives sur X, et $\nu$ la mesure $\sum_{\alpha \in A} \lambda_\alpha$.

#### Proposition 1 {#int-v-s2-prop-1 .statement}

Soit $f$ une fonction numérique positive définie dans X. On a

(3)
$$
\nu^\bullet(f) = \sum_{\alpha \in A} \lambda_\alpha^\bullet(f).
$$

Cela résulte aussitôt de la remarque 1, de la prop. 11 du § 1, n° 3 et de la prop. 3 du § 1, n° 1.

#### Corollaire 1 {#int-v-s2-prop-1-cor-1 .statement}

Pour tout partie compacte (resp. ouverte et relativement compacte) M de X, on a
$$
\nu(M) = \sum_{\alpha \in A} \lambda_\alpha(M).
$$

#### Corollaire 2 {#int-v-s2-prop-1-cor-2 .statement}

Pour qu’une partie N de X soit localement $\nu$-négligeable, il faut et il suffit que, pour tout $\alpha \in A$, N soit localement $\lambda_\alpha$-négligeable.

#### Corollaire 3 {#int-v-s2-prop-1-cor-3 .statement}

On a pour toute fonction $f \in \mathcal{F}_+(X)$

(4)
$$
\nu^*(f) \geq \sum_{\alpha \in A} \lambda_\alpha^*(f).
$$

Cette inégalité est évidente si $f$ n’est pas $\nu$-modérée, car alors $\nu^*(f) = +\infty$ ($\S 1$, n° 2, prop. 7). Si $f$ est $\nu$-modérée, $f$ est $\lambda_\alpha$-modérée pour tout $\alpha \in A$, car tout ouvert $\nu$-intégrable est $\lambda_\alpha$-intégrable ; la relation (4) résulte alors aussitôt de (3), et de la prop. 7 du $\S 1$, n° 2.

Il peut arriver que les deux membres de (4) ne soient pas égaux, même lorsque $A$ est dénombrable, et que chacune des mesures $\lambda_\alpha$ est ponctuelle ($\S 1$, exerc. 4a)).

#### Proposition 2 {#int-v-s2-prop-2 .statement}

Soit $f$ une application de $X$ dans un espace topologique $G$. Pour que $f$ soit $\nu$-mesurable, il faut et il suffit que $f$ soit $\lambda_\alpha$-mesurable pour tout $\alpha \in A$.

Cela résulte immédiatement du cor. 2 de la prop. 11 du $\S 1$.

#### Proposition 3 {#int-v-s2-prop-3 .statement}

Pour qu’une application $f$ de $X$ dans un espace de Banach $F$ soit essentiellement $\nu$-intégrable, il faut et il suffit que $f$ soit essentiellement $\lambda_\alpha$-intégrable pour tout $\alpha \in A$, et qu’on ait

$$
\sum_{\alpha \in A} \int^* |f| \, d\lambda_\alpha < +\infty.
$$

La famille $(\int f \, d\lambda_\alpha)_{\alpha \in A}$ est alors absolument sommable dans $F$, et l’on a :

$$
\int f \, d\nu = \sum_{\alpha \in A} \int f \, d\lambda_\alpha.
$$

En effet, pour que $f$ soit essentiellement $\nu$-intégrable (resp. essentiellement $\lambda_\alpha$-intégrable), il faut et il suffit que $f$ soit mesurable pour la mesure $\nu$ (resp. $\lambda_\alpha$), et qu’on ait $\nu^*(|f|) < +\infty$ (resp. $\lambda_\alpha^*(|f|) < +\infty$), en vertu de la prop. 9 du $\S 1$, n° 3. La première partie de l’énoncé résulte donc aussitôt des prop. 2 et 1. Si $f$ est essentiellement $\nu$-intégrable, l’inégalité

$$
\sum_{\alpha \in A} \left| \int f \, d\lambda_\alpha \right| \leq \sum_{\alpha \in A} \int |f| \, d\lambda_\alpha = \nu(|f|)
$$

entraîne que la famille $(\int f \, d\lambda_\alpha)$ est absolument sommable dans $F$, et que la norme de sa somme est au plus égale à la norme de $f$ dans $\mathcal{L}_F^1(\nu)$. L’ensemble des $f \in \mathcal{L}_F^1(\nu)$ qui satisfont à (6) est donc un sous-espace fermé $\mathcal{H}$ de $\mathcal{L}_F^1(\nu)$; or ce sous-espace est aussi dense dans $\mathcal{L}_F^1(\nu)$, car il contient les fonctions de la forme $f . a$, où $a \in F$, et où $f$ désigne une fonction intégrable finie et positive (prop. 1). On a donc $\mathcal{H} = \mathcal{L}_F^1(\nu)$, et la proposition est établie.

La prop. 3 peut aussi se déduire du théorème général d’intégration qui sera prouvé au paragraphe 3 (n° 3, th. 1).

#### Corollaire 1 {#int-v-s2-prop-3-cor-1 .statement}

Supposons que $f$ soit $v$-intégrable ; $f$ est alors $\lambda_\alpha$-intégrable pour tout $\alpha \in A$, et on a la formule (6). Inversement, si l’ensemble $A$ est fini, et si $f$ est $\lambda_\alpha$-intégrable pour tout $\alpha \in A$, la fonction $f$ est $v$-intégrable.

Si $f$ est $v$-intégrable, $f$ est essentiellement $v$-intégrable et $v$-modérée (\S 1, n° 3, cor. de la prop. 9); $f$ est donc essentiellement $\lambda_\alpha$-intégrable et $\lambda_\alpha$-modérée, donc $\lambda_\alpha$-intégrable, pour tout $\alpha \in A$. Inversement, si $A$ est fini, et si $f$ est $\lambda_\alpha$-intégrable pour tout $\alpha \in A$, $f$ est essentiellement $v$-intégrable d’après la prop. 3, et il suffit de vérifier que $v^*(|f|) < +\infty$; cela résulte aussitôt de la relation $v^* = \sum_{\alpha \in A} \lambda_\alpha^*$ (chap. IV, \S 1, n° 4, prop. 15).

#### Corollaire 2 {#int-v-s2-prop-3-cor-2 .statement}

Soit $\theta$ une mesure complexe sur $X$; on pose $\theta_1 = (\Re \theta)^+$, $\theta_2 = (\Re \theta)^-$, $\theta_3 = (\Im \theta)^+$, $\theta_4 = (\Im \theta)^-$. Pour qu’une application $f$ de $X$ dans un espace topologique $G$ (resp. dans un espace de Banach $F$) soit mesurable (resp. essentiellement intégrable, intégrable) pour la mesure $\theta$, il faut et il suffit qu’elle soit mesurable (resp. essentiellement intégrable, intégrable) pour chacune des mesures $\theta_i$ ($i = 1, 2, 3, 4$).

Si $f$ est mesurable (resp. essentiellement intégrable, intégrable) pour $\theta$, $f$ est par définition mesurable (resp. essentiellement intégrable, intégrable) pour la mesure $|\theta|$, donc aussi pour les mesures $\theta_i$, qui sont majorées par $|\theta|$. Inversement, si $f$ est mesurable (resp. essentiellement intégrable, intégrable) pour les mesures $\theta_i$, la prop. 2 (resp. la prop. 3, le cor. 1 de la prop. 3) entraîne que $f$ est mesurable (resp. essentiellement intégrable, intégrable) pour la mesure $\theta_1 + \theta_2 + \theta_3 + \theta_4$, qui majore $|\theta|$.

### 3. Décomposition d’une mesure en somme de mesures à supports compacts

#### Proposition 4 {#int-v-s2-prop-4 .statement}

Soit $\mu$ une mesure positive sur un espace localement compact $T$, et soit $\mathcal{R}$ un ensemble $\mu$-dense de parties compactes de $T$. Il existe une famille sommable $(\mu_\alpha)_{\alpha \in A}$ de mesures positives sur $T$, telle qu’on ait $\mu = \sum_{\alpha \in A} \mu_\alpha$, que les supports des mesures $\mu_\alpha$ appartiennent à $\mathcal{R}$, et forment une famille localement dénombrable de compacts deux à deux disjoints.

Si la mesure $\mu$ est modérée, l’ensemble d’indices $A$ peut être supposé dénombrable.

$$
\mu_\alpha(f) = \mu(f \varphi_{K_\alpha});
$$

la forme linéaire $\mu_\alpha$ sur $\mathcal{K}(T)$ est positive, c’est donc une mesure positive, de support contenu dans $K_\alpha$. Comme tout compact contenu dans un élément de $A$ appartient à $A$, on a $\operatorname{Supp}(\mu_\alpha) \in A$ pour tout $\alpha \in A$. Il reste seulement à montrer que la famille $(\mu_\alpha)$ est sommable, et que sa somme est égale à $\mu$; autrement dit, qu’on a $\sum_{\alpha \in A} \mu_\alpha(f) = \mu(f)$ pour toute fonction $f \in \mathcal{K}_+(T)$. Or, soit S le support (compact) de $f$, et soit $A'$ l’ensemble dénombrable constitué par les $\alpha \in A$ tels que $S \cap K_\alpha \neq \varnothing$. L’ensemble $N \cap S$ étant $\mu$-négligeable, on a

$$
\begin{align*}
\mu(f) &= \mu(f \varphi_S) = \sum_{\alpha \in A'} \mu(f \varphi_{S \cap K_\alpha}) = \sum_{\alpha \in A'} \mu(f \varphi_{K_\alpha}) \\
&= \sum_{\alpha \in A} \mu(f \varphi_{K_\alpha}) = \sum_{\alpha \in A} \mu_\alpha(f).
\end{align*}
$$

Cela achève la démonstration du cas général. Si $\mu$ est modérée, l’ensemble $T$ est $\mu$-modéré, et $T$ est donc réunion d’une suite $(L_n)$ de compacts et d’un ensemble négligeable ($§ 1$, n° 2, prop. 5); soit $A'$ l’ensemble dénombrable des $\alpha \in A$ tels que $K_\alpha$ rencontre l’un des $L_n$. On a $\mu_\alpha = 0$ pour $\alpha \notin A'$, et la dernière phrase de l’énoncé en résulte immédiatement.

#### Remarque {#int-v-s2-n3-rem-1 .statement}

Une mesure positive peut être somme d’une suite de mesures à support compact, et ne pas être modérée (voir l’exerc. 4a) du § 1).

## EXERCICES {#int-v-s2-exercises}

See the [exercises for § 2](exercises/s2/).
