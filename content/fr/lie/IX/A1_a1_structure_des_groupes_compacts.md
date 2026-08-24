---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: GROUPES DE LIE RÉELS COMPACTS
section: 1
section_title: STRUCTURE DES GROUPES COMPACTS
appendix: true
lang: fr
source: lie-ix-fr
book_pages: LIE IX.99-LIE IX.102
pdf_pages: 0102-0105, 0135-0141
extraction: ocr
subsections:
    - "no": 1
      title: Plongement d’un groupe compact dans un produit de groupes de Lie
      page: 99
      pdf_page: 102
    - "no": 2
      title: Limites projectives de groupes de Lie
      page: 100
      pdf_page: 103
    - "no": 3
      title: Structure des groupes compacts connexes
      page: 101
      pdf_page: 104
statements: 9
exercises: 1
content_sha256: f71cc519d454262675e06cb126581e6921af9721c539a8f1f4140ff9aa98693f
---

## APPENDICE 1

# Structure des groupes compacts

### 1. Plongement d’un groupe compact dans un produit de groupes de Lie

#### Proposition 1 {#lie-ix-a1-prop-1 .statement tag=01II}

Tout groupe topologique compact $ G $ est isomorphe à un sous-groupe fermé d’un produit de groupes de Lie compacts.

Notons $ \hat{G} $ l’ensemble des classes de représentations continues irréductibles unitaires de G dans des espaces hilbertiens complexes de dimension finie (TS, à paraître). Pour tout $ u \in \hat{G} $, soient $ H_u $ l’espace de $ u $ et $ \rho_u : G \to U(H_u) $ l’homomorphisme associé à $ u $. D’après le théorème de Peter-Weyl (TS, à paraître), l’homomorphisme continu $ \rho = (\rho_u)_{u \in \hat{G}} $ de G dans $ \prod_{u \in \hat{G}} U(H_u) $ est injectif ; puisque G est compact, $ \rho $ induit un isomorphisme de G sur un sous-groupe fermé du groupe $ \prod_{u \in \hat{G}} U(H_u) $.

#### Corollaire 1 {#lie-ix-a1-prop-1-cor-1 .statement tag=01IJ}

Soit V un voisinage de l’élément neutre dans G. Alors V contient un sous-groupe fermé distingué H de G tel que le quotient $ G/H $ soit un groupe de Lie.

Soit $ (K_\lambda)_{\lambda \in L} $ une famille de groupes de Lie compacts telle que G s’identifie à un sous-groupe fermé de $ \prod_{\lambda \in L} K_\lambda $; pour $ \lambda \in L $, notons $ p_\lambda : G \to K_\lambda $ la restriction à G de la projection canonique. Il existe un ensemble fini $ J \subset L $, et pour chaque $ \lambda \in J $ un voisinage de l’origine $ V_\lambda $ dans $ K_\lambda $, tels que V contienne $ \bigcap_{\lambda \in J} p_\lambda^{-1}(V_\lambda) $. Il suffit alors de poser $ H = \bigcap_{\lambda \in J} \mathrm{Ker}(p_\lambda) $.

Notons $ (H_\alpha)_{\alpha \in I} $ la famille filtrante décroissante des sous-groupes fermés distingués de G, tels que le quotient $ G/H_\alpha $ soit un groupe de Lie. Considérons le système projectif des groupes de Lie compacts $ G/H_\alpha $ (cf. TG, III, p. 60).

#### Corollaire 2 {#lie-ix-a1-prop-1-cor-2 .statement tag=01IK}

L’application canonique $ G \to \lim_{\leftarrow \alpha} G/H_\alpha $ est un isomorphisme de groupes topologiques.

En effet le cor. 1 entraîne que la condition (AP) de TG, III, p. 60 est vérifiée ; l’assertion résulte alors de la prop. 2 de loc. cit.

#### Corollaire 3 {#lie-ix-a1-prop-1-cor-3 .statement tag=01IL}

Pour que G soit un groupe de Lie, il faut et il suffit qu’il existe un voisinage de l’élément neutre e de G qui ne contienne aucun sous-groupe distingué distinct de {e}.

La nécessité de cette condition a déjà été prouvée (III, § 4, n° 2, cor. 1 au th. 2), et la suffisance est une conséquence immédiate du cor. 1.

### 2. Limites projectives de groupes de Lie

#### Lemme 1 {#lie-ix-a1-lem-1 .statement tag=01IM}

Soient $(G_\alpha, f_{\alpha\beta})$ un système projectif de groupes topologiques relatif à un ensemble d’indices I filtrant, G sa limite. On suppose que les applications canoniques $f_\alpha : G \to G_\alpha$ sont surjectives.

a) Les sous-groupes $\overline{D(G_\alpha)}$ (resp. $C(G_\alpha)$, resp. $C(G_\alpha)_0$) forment un système projectif de parties des $G_\alpha$.

b) On a $\overline{D(G)} = \lim_\alpha \overline{D(G_\alpha)}$ et $C(G) = \lim_\alpha C(G_\alpha)$.

c) Si $G_\alpha$ est compact pour tout $\alpha \in I$, on a $C(G)_0 = \lim_\alpha C(G_\alpha)_0$.

Soient $\alpha, \beta$ deux éléments de I, avec $\alpha \leq \beta$. On a $f_{\alpha\beta}(D(G_\beta)) \subset D(G_\alpha)$, et $f_{\alpha\beta}(C(G_\beta)) \subset C(G_\alpha)$ puisque $f_{\alpha\beta}$ est surjectif ; comme $f_{\alpha\beta}$ est continu, on en déduit $f_{\alpha\beta}(D(G_\beta)) \subset D(G_\alpha)$ et $f_{\alpha\beta}(C(G_\beta)_0) \subset C(G_\alpha)_0$, d’où a). Puisque $f_\alpha$ est surjectif, on a $f_\alpha(D(G)) = D(G_\alpha)$ (A, I, p. 67, prop. 6), d’où $\overline{D(G)} = \lim_\alpha \overline{D(G_\alpha)}$ (TG, I, p. 29, corollaire). La surjectivité de $f_\alpha$ entraîne aussi l’inclusion $f_\alpha(C(G)) \subset C(G_\alpha)$ et donc $C(G) \subset \lim_\alpha C(G_\alpha)$; l’inclusion opposée est immédiate. Enfin l’assertion c) résulte de b) et de TG, III, p. 62, prop. 4.

#### Lemme 2 {#lie-ix-a1-lem-2 .statement tag=01IN}

Soient $(S_a)_{a \in A}, (T_b)_{b \in B}$ deux familles finies de groupes de Lie simplement connexes presque simples (III, § 9, n° 8, déf. 3), et soit $u : \prod_{a \in A} S_a \to \prod_{b \in B} T_b$ un morphisme surjectif. Il existe alors une application injective $l : B \to A$ et des isomorphismes $u_b : S_{l(b)} \to T_b$ ($b \in B$) tels qu’on ait $u((s_a)_{a \in A}) = (u_b(s_{l(b)}))_{b \in B}$ pour tout élément $(s_a)_{a \in A}$ de $\prod_{a \in A} S_a$.

Notons $s_a$ (resp. $t_b$) l’algèbre de Lie de $S_a$ (resp. $T_b$) pour $a \in A$ (resp. $b \in B$), et considérons l’homomorphisme $L(u) : \prod_{a \in A} s_a \to \prod_{b \in B} t_b$. Son noyau est un idéal de l’algèbre de Lie semi-simple $\prod_{a \in A} s_a$, donc est de la forme $\prod_{a \in A''} s_a$, avec $A'' \subset A$ (I, § 6, n° 2, cor. 1). Posons $A' = A - A''$. Par restriction, $L(u)$ induit un isomorphisme $f : \prod_{a \in A'} s_a \to \prod_{b \in B} t_b$. D’après loc. cit., pour tout $a$ dans $A'$, l’idéal $f(s_a)$ est égal à l’un des $t_b$; il existe donc une bijection $l : B \to A'$ telle que $f(s_{l(b)}) = t_b$ pour $b \in B$, et $f$ induit un isomorphisme $f_b : s_{l(b)} \to t_b$. Puisque les groupes $S_a$ et $T_b$ sont simplement connexes, il existe des isomorphismes $u_b : S_{l(b)} \to T_b$ tels que $L(u_b) = f_b$ pour $b \in B$ (III, § 6, n° 3, th. 3).

Notons $\tilde{u} : \prod_{a \in A} S_a \to \prod_{b \in B} T_b$ le morphisme défini par $\tilde{u}((s_a)_{a \in A}) = (u_b(s_{l(b)}))_{b \in B}$. On a par construction $L(\tilde{u}) = f = L(u)$, d’où $\tilde{u} = u$, ce qui démontre le lemme.

#### Lemme 3 {#lie-ix-a1-lem-3 .statement tag=01IO}

Sous les hypothèses du lemme 1, on suppose que les $ G_\alpha $ sont des groupes de Lie compacts simplement connexes. Le groupe topologique $ G $ est alors isomorphe au produit d'une famille de groupes de Lie compacts, presque simples, simplement connexes.

Pour tout $ \alpha \in I $, le groupe $ G_\alpha $ est produit direct d'une famille finie de sous-groupes presque simples simplement connexes $ (S^\lambda_\alpha)_{\lambda \in L_\alpha} $ (III, § 9, no 8, prop. 28). Soit $ \beta \in I $, $ \beta \geq \alpha $. D'après le lemme 2, il existe une application $ l_{\beta \alpha}: L_\alpha \to L_\beta $ telle que $ f_{\alpha \beta}(S^{l_{\beta \alpha}(\lambda)}_\beta) = S^\lambda_\alpha $ pour $ \lambda \in L_\alpha $. On a $ l_{\gamma \beta} \circ l_{\beta \alpha} = l_{\gamma \alpha} $ pour $ \alpha \leq \beta \leq \gamma $, de sorte que $ (L_\alpha, l_{\beta \alpha}) $ est un système inductif d'ensembles relatif à $ I $. Soit $ L $ sa limite ; les applications $ l_{\beta \alpha} $ étant injectives, on peut identifier $ L_\alpha $ à un sous-ensemble de $ L $, de sorte qu'on a $ L = \bigcup_{\alpha \in I} L_\alpha $.

Soit $ \lambda \in L $. Posons $ S^\lambda_\alpha = \{1\} $ lorsque $ \lambda \notin L_\alpha $, et notons $ \varphi^\lambda_{\alpha \beta}: S^\lambda_\beta \to S^\lambda_\alpha $ le morphisme déduit de $ f_{\alpha \beta} $; on obtient ainsi un système projectif de groupes topologiques $ (S^\lambda_\alpha, \varphi^\lambda_{\alpha \beta}) $, dont la limite $ S_\lambda $ est isomorphe à $ S_\lambda $ pour $ \alpha $ assez grand. L'homomorphisme canonique de groupes topologiques

$$
\lim_{\leftarrow \alpha \in I} (\prod_{\lambda \in L} S^\lambda_\alpha) \to \prod_{\lambda \in L} (\lim_{\leftarrow \alpha \in I} S^\lambda_\alpha)
$$

est bijectif (E, III, p. 57, cor. 2); c'est donc un isomorphisme puisque les groupes considérés sont compacts. Or le premier de ces groupes s'identifie à $ G $ et le second au produit des $ S_\lambda $, d'où le lemme.

### 3. Structure des groupes compacts connexes

Soit $ G $ un groupe compact commutatif. Rappelons (TS, II, § 1, no 9, prop. 11) que $ G $ est alors isomorphe au groupe topologique dual d'un groupe commutatif discret $ \hat{G} $. Le groupe $ G $ est connexe si et seulement si $ \hat{G} $ est sans torsion (TS, II, § 2, no 2, cor. 1 à la prop. 4).

Les propriétés suivantes sont équivalentes (TS, II, § 2, no 2, cor. 2 à la prop. 4 et § 1, no 9, cor. 2 à la prop. 11):
(i) $ G $ est totalement discontinu ;
(ii) $ \hat{G} $ est un groupe de torsion ;
(iii) le groupe topologique $ G $ est isomorphe à la limite d'un système projectif de groupes (commutatifs) finis, munis de la topologie discrète.
La proposition ci-dessous généralise le cor. 1 à la prop. 4 du § 1, no 4.

#### Proposition 2 {#lie-ix-a1-prop-2 .statement tag=01IP}

Soit $ G $ un groupe compact connexe.
a) $ C(G)_0 $ est un groupe compact connexe commutatif; $ D(G) $ est un groupe compact connexe, égal à son groupe dérivé.
b) L'homomorphisme continu $ (x, y) \mapsto xy $ de $ C(G)_0 \times D(G) $ dans $ G $ est surjectif et son noyau est un sous-groupe central de $ C(G)_0 \times D(G) $, compact et totalement discontinu.

c) Il existe une famille $(S_\lambda)_{\lambda \in L}$ de groupes de Lie compacts presque simples et un homomorphisme continu surjectif $\prod_{\alpha \in L} S_\alpha \to D(G)$, dont le noyau est un sous-groupe central compact totalement discontinu.

Soit $(G_\alpha, f_{\alpha\beta})$ un système projectif de groupes de Lie compacts, relatif à un ensemble filtrant $I$, tel que $G$ soit isomorphe à $\lim_{\leftarrow} G_\alpha$ et que les applications canoniques $f_\alpha : G \to G_\alpha$ soient surjectives (cor. 2 à la prop. 1). Pour $\alpha \in I$, soit $\pi_\alpha : \tilde{D}(G_\alpha) \to D(G_\alpha)$ un revêtement universel du groupe $D(G_\alpha)$. On déduit des $f_{\alpha\beta}$ des morphismes $\tilde{f}_{\alpha\beta} : \tilde{D}(G_\beta) \to \tilde{D}(G_\alpha)$, de sorte que $(\tilde{D}(G_\alpha), \tilde{f}_{\alpha\beta})$ est un système projectif de groupes topologiques satisfaisant aux hypothèses du lemme 3.

Il résulte de ce lemme que le groupe topologique $\lim_{\leftarrow} \tilde{D}(G_\alpha)$ est isomorphe au produit d'une famille $(S_\lambda)_{\lambda \in L}$ de groupes de Lie compacts presque simples. La limite du système projectif d'homomorphismes $(\pi_\alpha)$ s'identifie d'après le lemme 1 à un homomorphisme continu $\pi : \prod_{\lambda \in L} S_\lambda \to \overline{D(G)}$, qui est surjectif (TG, I, p. 65, cor. 2).

Observons maintenant que le groupe $\prod_{\lambda \in L} S_\lambda$ est égal à son groupe dérivé : cela résulte du § 4, no 5, cor. à la prop. 10. Il en est donc de même pour $\overline{D(G)}$, puisque $\pi$ est surjectif. On a par conséquent $D(G) \supset D(\overline{D(G)}) = \overline{D(G)}$. Ainsi le groupe $D(G)$ est compact et égal à son groupe dérivé ; ceci prouve $a)$, car les assertions concernant $C(G)_0$ sont triviales.

D'autre part le noyau de $\pi : \prod_{\lambda \in L} S_\lambda \to D(G)$ s'identifie à $\lim_{\leftarrow} \mathrm{Ker}(\pi_\alpha)$ (A, II, p. 89, remarque 1), donc à un sous-groupe central, compact et totalement discontinu, d'où $c)$.

Prouvons $b)$. Pour tout $\alpha$ dans $I$, le morphisme $s_\alpha : C(G_\alpha)_0 \times D(G_\alpha) \to G_\alpha$ tel que $s_\alpha(x, y) = xy$ pour $x \in C(G_\alpha)_0,\ y \in D(G_\alpha)$, est surjectif et a pour noyau un sous-groupe fini central (\S 1, no 4, cor. 1 à la prop. 4). Les $s_\alpha$ forment un système projectif d'applications, dont la limite s'identifie d'après ce qui précède à l'homomorphisme $(x, y) \mapsto xy$ de $C(G)_0 \times D(G)$ dans $G$. On voit alors comme précédemment que celui-ci est surjectif et que son noyau est central et totalement discontinu, d'où $b)$.

#### Corollaire {#lie-ix-a1-n3-cor-1 .statement tag=01IQ}

Tout groupe compact connexe résoluble est commutatif.

En effet le groupe dérivé est alors résoluble et égal à son groupe dérivé (prop. 2, $a$)), donc réduit à l'élément neutre.

## EXERCICES {#lie-ix-a1-exercises}

See the [exercises for Appendix 1](exercises/a1/).
