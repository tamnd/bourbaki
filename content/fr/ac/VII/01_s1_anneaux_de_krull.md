---
book: ac
book_title: Commutative Algebra
chapter: VII
chapter_title: Diviseurs
section: 1
section_title: Anneaux de Krull
lang: fr
source: ac-v-vii-fr
pdf_pages: 0195-0216, 0275-0285
extraction: ocr
subsections:
    - "no": 1
      title: Idéaux divisoriels d’un anneau intègre
      page: 0
      pdf_page: 195
    - "no": 2
      title: '*Structure de monoïde sur $ D(A) $*'
      page: 0
      pdf_page: 198
    - "no": 3
      title: Anneaux de Krull
      page: 0
      pdf_page: 200
    - "no": 4
      title: Valuations essentielles d’un anneau de Krull
      page: 0
      pdf_page: 203
    - "no": 5
      title: Approximation pour les valuations essentielles
      page: 0
      pdf_page: 206
    - "no": 6
      title: Idéaux premiers de hauteur 1 d’un anneau de Krull
      page: 0
      pdf_page: 207
    - "no": 7
      title: 'Application: nouvelles caractérisations des anneaux de valuation discrète'
      page: 0
      pdf_page: 209
    - "no": 8
      title: Fermeture intégrale d’un anneau de Krull dans une extension finie de son corps des fractions
      page: 0
      pdf_page: 209
    - "no": 9
      title: Anneaux de polynômes sur un anneau de Krull
      page: 0
      pdf_page: 210
    - "no": 10
      title: Classes de diviseurs dans les anneaux de Krull
      page: 0
      pdf_page: 212
statements: 44
exercises: 32
content_sha256: c2fbb9b6472cadb4ecad9a1c10511397e20e3bfe2dfef6c268b5fc08e7a6fd8d
---

## § 1. Anneaux de Krull

### 1. Idéaux divisoriels d’un anneau intègre

#### Définition 1 {#ac-vii-s1-def-1 .statement}

Soient A un anneau intègre, K son corps des fractions. On appelle idéal fractionnaire de A (ou de K, par abus de langage) tout sous-A-module a de K tel qu’il existe un élément d ≠ 0 de A pour lequel da ⊂ A.

Tout sous-A-module a de type fini de K est un idéal fractionnaire : en effet, si $ (a_i)_{1 \leq i \leq n} $ est un système de générateurs de a, on peut écrire $ a_i = b_i / d_i $ où $ b_i \in A, d_i \in A $ et $ d_i \neq 0 $; si $ d = d_1 \cdots d_n $, il est clair que $ da \subset A $. En particulier les sous-A-modules monogènes de K sont des idéaux fractionnaires (rappelons qu’ils ont été appelés idéaux principaux fractionnaires en Alg., chap. VI, § 1, n° 5). Si A est noethérien, tout idéal fractionnaire est un A-module de type fini. Tout sous-A-module d’un idéal fractionnaire de A est un idéal fractionnaire. Tout idéal de A est un idéal fractionnaire ; pour éviter des confusions, on dit encore que ce sont les idéaux entiers de A.

Nous noterons I(A) l’ensemble des idéaux fractionnaires non nuls de A. Etant donnés deux éléments a, b de I(A), nous écrirons $ a < b $ (ou $ b > a $) la relation « tout idéal principal fractionnaire contenant a contient aussi b »; il est clair que cette relation est

Pour tout $ a \in I(A) $ il existe par hypothèse un $ d \neq 0 $ dans $ A $ tel que $ a \subset Ad^{-1} $; l’intersection $ \tilde{a} $ des idéaux principaux fractionnaires contenant $ a $ est donc un élément de $ I(A) $. Il est clair que la relation $ a < b $ est équivalente à la relation $ \tilde{a} \supset \tilde{b} $; la relation $ a \supset b $ entraîne donc $ a < b $. Pour que deux éléments $ a, b $ de $ I(A) $ soient équivalents modulo $ R $, il faut et il suffit que $ \tilde{a} = \tilde{b} $.

#### Définition 2 {#ac-vii-s1-def-2 .statement}

*On appelle idéal fractionnaire divisoriel de* $ A $ *tout élément* $ a $ *de* $ I(A) $ *tel que* $ a = \tilde{a} $.

Autrement dit un idéal divisoriel n’est autre qu’une intersection non nulle d’une famille non vide d’idéaux principaux fractionnaires. Toute intersection non nulle d’idéaux divisoriels est un idéal divisoriel. Si $ a $ est divisoriel, il en est de même de $ ax $ pour tout $ x \in K^* $, l’application $ b \to bx $ étant une bijection de l’ensemble des idéaux principaux fractionnaires sur lui-même. Pour tout $ a \in I(A) $, $ \tilde{a} $ est le plus petit idéal divisoriel contenant $ a $, et est équivalent à $ a $ modulo $ R $. D’ailleurs, si $ b $ est un idéal divisoriel équivalent à $ a $ modulo $ R $, on a $ \tilde{a} = \tilde{b} = b $. Donc $ \tilde{a} $ est l’unique idéal divisoriel $ b $ tel que div $ a = $ div $ b $ (autrement dit, la restriction de l’application $ a \to $ div $ a $ à l’ensemble des idéaux *divisoriels* est *injective*).

Soient $ a $ et $ b $ deux idéaux fractionnaires de $ K $. Rappelons (chap. I, § 2, n° 10) qu’on note $ b : a $ l’ensemble des $ x \in K $ tels que $ xa \subset b $; c’est évidemment un $ A $-module; si $ b \in I(A) $ et $ a \in I(A) $, on a $ b : a \in I(A) $; en effet, si $ d $ est un élément non nul de $ A $ tel que $ db \subset A $ et $ da \subset A $ et si $ a $ est un élément non nul de $ A \cap a $, on a $ da(b : a) \subset A $; d’autre part, si $ b \neq 0 $ appartient à $ b $, on a $ bda \subset b $, donc $ bd \in b : a $ et $ b : a \neq 0 $.

La définition de $ b : a $ peut encore s’écrire:

(1)
$$
b : a = \bigcap_{x \in a, x \neq 0} bx^{-1}.
$$

n° 1

ANNEAUX DE KRULL

#### Proposition 1 {#ac-vii-s1-prop-1 .statement}

a) Si b est un idéal divisoriel, et si $ a \in I(A) $, $ b : a $ est divisoriel.

b) Soient $ a, b $ dans $ I(A) $. Pour que div $ a = \mathrm{div}\ b $, il faut et il suffit que $ A : a = A : b $.

c) Pour tout $ a \in I(A) $, on $ a\ \tilde{a} = A : (A : a) $.

L’assertion a) résulte aussitôt de la formule (1) puisque, si b est divisoriel, il en est de même de $ bx^{-1} $ pour tout $ x \neq 0 $.

Pour démontrer b), notons $ P(a) $ l’ensemble des idéaux principaux fractionnaires contenant $ a $; la relation $ Ax \in P(a) $ équivaut à $ x^{-1}a \subset A $, donc à $ x^{-1} \in A : a $. Comme la relation div $ a = \mathrm{div}\ b $ est par définition équivalente à $ P(a) = P(b) $, elle est aussi équivalente à $ A : a = A : b $.

Enfin, comme $ a(A : a) \subset A $, on a $ a \subset A : (A : a) $. Remplaçant $ a $ par $ A : a $ dans cette formule, on voit que $ A : a \subset A : (A : (A : a)) $; d’autre part, la relation $ a \subset A : (A : a) $ implique

$$
A : a \supset A : (A : (A : a)).
$$

On a donc $ A : a = A : (A : (A : a)) $, et il résulte de b) que div $ a = \mathrm{div}(A : (A : a)) $. Comme $ A : (A : a) $ est divisoriel en vertu de a), on a bien $ \tilde{a} = A : (A : a) $, ce qui prouve c).

#### Remarque {#ac-vii-s1-n1-rem-1 .statement}

Au cours de la démonstration précédente, on a prouvé que $ A : a = A : (A : (A : a)) $ pour tout idéal $ a \in I(A) $, ce qui est un cas particulier de Ens., chap. III, 3e éd., § 1, n° 5, prop. 2.

#### Proposition 2 {#ac-vii-s1-prop-2 .statement}

(i) Dans $ D(A) $, tout ensemble majoré non vide admet une borne supérieure. Plus précisément, si $ (\alpha_i) $ est une famille majorée non vide d’éléments de $ I(A) $, on a

$$
\sup (\mathrm{div}\ \alpha_i) = \mathrm{div} \left( \bigcap_i \tilde{\alpha}_i \right).
$$

(ii) Dans $ D(A) $, tout ensemble minoré non vide admet une borne inférieure. Plus précisément, si $ (\alpha_i) $ est une famille minorée non vide d’éléments de $ I(A) $, on a

$$
\inf (\mathrm{div}\ \alpha_i) = \mathrm{div} \left( \sum_i \alpha_i \right).
$$

(iii) L’ensemble $ D(A) $ est réticulé.

Soit $ (\alpha_i) $ une famille majorée non vide d’éléments de $ I(A) $. Dire qu’un idéal divisoriel $ b $ majore cette famille revient à dire qu’il est contenu dans tous les $ \tilde{\alpha}_i $, c’est-à-dire que $ b $ est contenu dans $ \bigcap_i \tilde{\alpha}_i $. On a donc $ \bigcap_i \tilde{\alpha}_i \neq (0) $, et $ \bigcap_i \tilde{\alpha}_i $ est par suite un idéal divisoriel, ce qui démontre (i).

Soit maintenant $ (\alpha_i) $ une famille minorée non vide d’éléments de $ I(A) $. Dire qu’un idéal divisoriel $ b $ minore cette famille veut dire qu’il contient tous les $ \tilde{a}_i $, c’est-à-dire (puisque $ b $ est divisoriel) qu’il contient tous les $ a_i $, ou encore qu’on $ a \supset b \supset \sum_i a_i $. Ceci démontre (ii).

Enfin, pour prouver (iii), il suffit, en vertu de (i) et (ii), de prouver que, si $ a, b $ sont dans $ I(A) $, l’ensemble $ \{ a, b \} $ est à la fois majoré et minoré dans $ I(A) $; or il est majoré par $ a \cap b $ (qui est différent de (0)). Il est minoré par $ a + b $, car on a $ a + b \in I(A) $: en effet, si $ d $ et $ d' $ sont des éléments non nuls de $ A $ tels que $ da \subset A $ et $ d'b \subset A $, on a $ dd'(a + b) \subset A $.

#### Corollaire {#ac-vii-s1-n1-cor-1 .statement}

*Si $ x, y $ et $ x + y $ sont dans $ K^* $, on a* div$(x + y) \geq \inf(\mathrm{div}(x), \mathrm{div}(y))$.
En effet $ A(x + y) \subset Ax + Ay $, donc $ \mathrm{div}(x + y) \geq \mathrm{div}(Ax + Ay) $.

### 2. *Structure de monoïde sur $ D(A) $*

#### Proposition 3 {#ac-vii-s1-prop-3 .statement}

*Soient $ a, a', b, b' $ des éléments de $ I(A) $. Les relations $ a > a' $ et $ b > b' $ impliquent $ ab > a'b' $.
On peut se borner au cas où $ b = b' $. Soit alors $ Ax $ un idéal principal fractionnaire contenant $ a'b $; pour tout élément non nul $ y $ de $ b $, on a $ Ax \supset a'y $, donc $ Axy^{-1} \supset a' $, d’où $ Axy^{-1} \supset a $ et $ Ax \supset ay $. Faisant varier $ y $, on voit que $ Ax \supset ab $, d’où $ ab > a'b $.

C.Q.F.D.

Il résulte de la prop. 3 que la multiplication dans $ I(A) $ définit, par passage au quotient, une loi de composition dans $ D(A) $, qui est évidemment associative et commutative. On la note additive-ment, de sorte qu’on peut écrire:

(2)
$$
\mathrm{div}(ab) = \mathrm{div}\, a + \mathrm{div}\, b,
$$
pour $ a, b $ dans $ I(A) $. Il est clair que $ \mathrm{div}(1) $ est un élément neutre pour cette addition; on note cet élément 0. La prop. 3 prouve en outre que la structure d’ordre sur $ D(A) $ est *compatible* avec cette addition (*Alg.*, chap. VI, § 1, n° 1), et de façon plus précise, on a (n° 1, prop. 2, (ii)):
$$
\inf(\mathrm{div}\, a + \mathrm{div}\, b, \mathrm{div}\, a + \mathrm{div}\, c) = \inf(\mathrm{div}(ab), \mathrm{div}(ac)) = \mathrm{div}(ab + ac)
$$
$$
= \mathrm{div}(a(b + c)) = \mathrm{div}\, a + \mathrm{div}(b + c) = \mathrm{div}\, a + \inf(\mathrm{div}\, b, \mathrm{div}\, c).
$$
Pour qu’un idéal fractionnaire $ a \neq 0 $ soit tel que $ \mathrm{div}\, a \geq 0 $ dans $ D(A) $, il faut et il suffit que $ a \subset A $ (autrement dit, que $ a $ soit un idéal *entier* de $ A $).

« il existe $ x \in K^* $ tel que $ P = Q + \mathrm{div}(x) $ »

est donc une relation d’équivalence, puisque la relation $ P = Q + \mathrm{div}(x) $ est équivalente à $ Q = P + \mathrm{div}(x^{-1}) $; si $ P $ et $ Q $ sont congrus modulo $ S $, on dit que ce sont des diviseurs équivalents de $ A $. Il est clair en outre que la relation $ S $ est compatible avec la loi du monoïde $ D(A) $, et cette dernière définit donc, par passage aux quotients, une structure de monoïde sur $ D(A)/S $; on dit que ce monoïde est le monoïde des classes de diviseurs de $ A $.

#### Proposition 4 {#ac-vii-s1-prop-4 .statement}

*Soient $ a, b $ deux idéaux fractionnaires divisoriels de $ A $. Les propriétés suivantes sont équivalentes*:
a) $ \mathrm{div}\ a $ et $ \mathrm{div}\ b $ sont des diviseurs équivalents;
b) *il existe $ x \in K^* $ tel que $ b = xa $*.

En effet, si $ \mathrm{div}\ b = \mathrm{div}\ a + \mathrm{div}(x) $ pour un $ x \in K^* $, on a $ \mathrm{div}\ b = \mathrm{div}(xa) $ et comme $ b $ et $ xa $ sont divisoriels, on a $ b = xa $, ce qui prouve la proposition.

Soit $ a $ un idéal fractionnaire *inversible* (chap. II, § 5, no 6); on a alors $ a = A : (A : a) $ (*loc. cit.*, prop. 10), donc $ a $ est *divisoriel* (no 1, prop. 1). Le groupe $ J(A) $ des idéaux fractionnaires inversibles s’identifie donc à un sous-groupe du monoïde $ D(A) $, et l’image canonique de $ J(A) $ dans $ D(A)/S $ au groupe des classes des $ A $-modules *projectifs de rang* 1 (chap. II, § 5, no 7, cor. 2 de la prop. 12 et *Remarque* 1).

#### Théorème 1 {#ac-vii-s1-thm-1 .statement}

*Soit $ A $ un anneau intègre. Pour que le monoïde $ D(A) $ des diviseurs de $ A $ soit un groupe, il faut et il suffit que $ A $ soit complètement intégralement clos*.

Supposons que $ D(A) $ soit un groupe. Soit $ x \in K $; supposons que $ A[x] $ soit contenu dans un sous-A-module de type fini de $ K $. Alors, on a vu (no 1) que $ a = A[x] $ est un élément de $ I(A) $. On a $ xa \subset a $, donc $ \mathrm{div}(x) + \mathrm{div}\ a \geqslant \mathrm{div}\ a $. Puisque $ D(A) $ est un groupe ordonné, on en conclut que $ \mathrm{div}(x) \geqslant 0 $, d’où $ x \in A $. Ainsi $ A $ est complètement intégralement clos (chap. V, § 1, no 4, déf. 5).

Réciproquement, supposons $ A $ complètement intégralement clos. Soit $ a $ un idéal divisoriel. Nous allons montrer que $ \operatorname{div} a + \operatorname{div}(A : a) = 0 $, ce qui prouvera que $ D(A) $ est un groupe. Comme on a $ a(A : a) \subset A $, il suffit (n° 1) de voir que tout idéal principal fractionnaire $ Ax^{-1} $ qui contient $ a(A : a) $ contient aussi $ A $. Or, pour $ y \in K^* $, la relation $ Ay \supset a $ entraîne $ y^{-1} \in A : a $, d’où $ y^{-1}a \subset a(A : a) \subset Ax^{-1} $, donc $ xa \subset Ay $. Comme $ a $ est divisoriel, on en déduit $ xa \subset a $, d’où $ x^n a \subset a $ pour tout $ n \in \mathbf{N} $. Il existe des éléments $ x_0, x_1 $ de $ K^* $ tels que $ Ax_0 \subset a \subset Ax_1 $; on a donc $ x^n x_0 \in Ax_1 $, d’où $ x^n \in Ax_1 x_0^{-1} $. Comme $ A $ est complètement intégralement clos, on a $ x \in A $, c’est-à-dire $ Ax^{-1} \supset A $, ce qui achève la démonstration.

On notera que si $ A $ est complètement intégralement clos (et même noethérien), un idéal divisoriel de $ A $ n’est pas nécessairement inversible, autrement dit, on a en général $ J(A) \neq D(A) $ (exerc. 2 et § 3, n° 2, prop. 1).

#### Corollaire {#ac-vii-s1-n2-cor-1 .statement}

Soient $ A $ un anneau complètement intégralement clos, $ a $ un idéal fractionnaire divisoriel de $ A $. Alors, pour tout idéal fractionnaire $ b \neq 0 $ de $ A $, on a $ \operatorname{div}(a : b) = \operatorname{div} a - \operatorname{div} b $.

En vertu de la formule (1) du n° 1, on a :
$$
\operatorname{div}(a : b) = \operatorname{div}\left( \bigcap_{y \in b, y \neq 0} y^{-1} a \right) = \sup_{y \in b, y \neq 0} \operatorname{div}(y^{-1} a)
$$
compte tenu de la prop. 2 et du fait que les idéaux fractionnaires $ y^{-1} a $ sont divisoriels. Mais puisque $ D(A) $ est un groupe ordonné, on a (Alg., chap. VI, § 1, n° 8) :
$$
\sup_{y \in b, y \neq 0} \operatorname{div}(y^{-1} a) = \sup_{y \in b, y \neq 0} (\operatorname{div} a - \operatorname{div}(y)) = \operatorname{div} a - \inf_{y \in b, y \neq 0} \operatorname{div}(y)
$$
$$
= \operatorname{div} a - \operatorname{div} b.
$$

### 3. Anneaux de Krull

#### Définition 3 {#ac-vii-s1-def-3 .statement}

On dit qu’un anneau $ A $ est un anneau de Krull s’il est intègre, et s’il existe une famille $ (v_i)_{i \in I} $ de valuations du corps des fractions $ K $ de $ A $ possédant les propriétés suivantes :
(AK_I) les valuations $ v_i $ sont discrètes ;
(AK_{II}) l’intersection des anneaux des $ v_i $ est $ A $ ;
(AK_{III}) pour tout $ x \in K^* $, l’ensemble des indices $ i \in I $ tels que $ v_i(x) \neq 0 $ est fini.

Il suffit évidemment de vérifier la condition (AK_{III}) pour les éléments x de A − (0).

#### Exemple 1 {#ac-vii-s1-n3-exa-1 .statement}

Tout anneau de valuation discrète est un anneau de Krull.

#### Exemple 2 {#ac-vii-s1-n3-exa-2 .statement}

Plus généralement, tout anneau principal A est un anneau de Krull. En effet soit $ (p_i)_{i \in I} $ un système représentatif d’éléments extrémaux de A, et soit $ v_i $ la valuation du corps des fractions de A définie par $ p_i $ (chap. VI, § 3, n° 3, Exemple 4). On voit aussitôt que la famille $ (v_i)_{i \in I} $ vérifie les propriétés (AK_I), (AK_{II}) et AK_{III}.

#### Exemple 3 {#ac-vii-s1-n3-exa-3 .statement}

Soient F un corps, et $ (R_i)_{1 \leq i \leq n} $ une famille finie de sous-anneaux de F qui soient des anneaux de Krull. Alors leur intersection $ S = \bigcap_{j=1}^n R_j $ est un anneau de Krull. En effet, pour $ 1 \leq j \leq n $, soit $ (v_{ji})_{i \in I_j} $ une famille de valuations du corps des fractions de $ R_j $ vérifiant (AK_I), (AK_{II}), (AK_{III}) (où A est remplacé par $ R_j $). Notons $ w_{ji} $ la restriction de $ v_{ji} $ au corps des fractions de S. Alors la famille $ (v_{ji})_{1 \leq j \leq n, i \in I_j} $ vérifie évidemment (AK_{II}) (où A est remplacé par S), et aussi (AK_{III}) puisque l’ensemble des indices j est fini. Les valuations $ w_{ji} $ sont, soit discrètes, soit impropres. En ne gardant que celles qui sont discrètes, on obtient évidemment une famille vérifiant (AK_I), (AK_{II}) et (AK_{III}) (où A est remplacé par S). Donc S est bien un anneau de Krull.

#### Exemple 4 {#ac-vii-s1-n3-exa-4 .statement}

En particulier, si A est un anneau de Krull et K’ un sous-corps du corps des fractions K de A, $ K' \cap A $ est un anneau de Krull.

#### Théorème 2 {#ac-vii-s1-thm-2 .statement}

Soit A un anneau intègre. Pour que A soit un anneau de Krull, il faut et il suffit que les deux conditions suivantes soient satisfaites:

a) A est complètement intégralement clos;
b) toute famille non vide d’idéaux entiers divisoriels de A admet un élément maximal (pour la relation $ \subset $).

En outre, si P(A) est l’ensemble des éléments extrémaux de D(A), P(A) est alors une base du $ \mathbf{Z}$-module D(A) et les éléments positifs de D(A) sont les combinaisons linéaires des éléments de P(A) à coefficients $ \geq 0 $.

Soit A un anneau de Krull. Il est complètement intégralement clos (chap. VI, § 4, n° 5, cor. de la prop. 9). Soit $ (v_i)_{i \in I} $ une famille de valuations du corps des fractions K de A vérifiant (AK_I), (AK_{II}) et (AK_{III}). On peut supposer les $ v_i $ normées (chap. VI,

$$
v_i(a) = \sup_{a \subset Ax} (v_i(x));
$$

on a $ v_i(a) \in \mathbf{Z} $, car si $ a $ est un élément non nul de $ a $, la relation $ Ax \supset Aa $ implique $ v_i(x) \leq v_i(a) $ (d’après (AK$_{II}$)), ce qui montre que la famille des $ v_i(x) $ ($ a \subset Ax $) est majorée. Etablissons les propriétés suivantes :

1) *Soit $ a $ un idéal fractionnaire divisoriel ; pour que $ y \in a $, il faut et il suffit que $ v_i(y) \geq v_i(a) $ pour tout $ i \in I $.

En effet, comme $ a $ est divisoriel, la relation $ y \in a $ équivaut à la relation « $ a \subset Ax $ implique $ y \in Ax $ ». Or, en vertu de (AK$_{II}$), la relation $ y \in Ax $ équivaut à « $ v_i(y) \geq v_i(x) $ pour tout $ i \in I $ ». D’où 1).

2) *Soient $ a $ et $ b $ deux idéaux fractionnaires divisoriels de $ A $; pour que $ a \subset b $, il faut et il suffit que $ v_i(a) \geq v_i(b) $ pour tout $ i \in I $.

Ceci résulte aussitôt de la propriété 1).

3) *Si $ x \in K^* $, on a $ v_i(Ax) = v_i(x) $.

En effet, si $ Ay \supset Ax $, on a $ v_i(y) \leq v_i(x) $ d’après (AK$_{II}$), et la valeur maximum de $ v_i(y) $ est prise pour $ y = x $.

4) *Pour tout $ a \in I(A) $, les indices $ i \in I $ tels que $ v_i(a) \neq 0 $ sont en nombre fini.

En effet, il existe $ x, y $ dans $ K^* $ tels que $ Ax \subset a \subset Ay $. D’après les propriétés 2) et 3), on a $ v_i(x) \geq v_i(a) \geq v_i(y) $ pour tout $ i \in I $. Il suffit alors d’appliquer (AK$_{III}$).

Nous avons donc démontré le lemme suivant :

#### Lemme 1 {#ac-vii-s1-lem-1 .statement}

*Si $ A $ est un anneau de Krull, et $ (v_i)_{i \in I} $ une famille de valuations normées de $ K $ vérifiant (AK$_I$), (AK$_{II}$) et (AK$_{III}$), l’application $ a \to (v_i(a))_{i \in I} $ est une application injective décroissante de l’ensemble des idéaux entiers divisoriels de $ A $ (ordonné par $ \subset $) dans l’ensemble des éléments positifs du groupe ordonné somme directe $ \mathbf{Z}^{(I)} $.

Cela étant, tout ensemble non vide d’éléments positifs de $ \mathbf{Z}^{(I)} $ possède un élément minimal (*Alg.*, chap. VI, § 1, n° 13, th. 2). Donc $ A $ vérifie bien la propriété *b*) de l’énoncé.

Réciproquement, soit $ A $ un anneau intègre vérifiant les propriétés *a*) et *b*) de l’énoncé. Puisque $ A $ est complètement intégralement clos, $ D(A) $ est un groupe ordonné (n° 2, th. 1). Ce groupe est réticulé (n° 1, prop. 2). D’après la condition *b*) de l’énoncé, toute famille non vide d’éléments positifs de $ D(A) $ possède un élément minimal. Soit $ P(A) $ l’ensemble des éléments

Ainsi, pour $ x \in K^* $, on définit des entiers rationnels $ v_P(x) $ (pour $ P \in P(A) $) en posant:

$$
\text{div}(x) = \sum_{P \in P(A)} v_P(x) \cdot P.
$$

Posons aussi $ v_P(0) = + \infty $.
Des relations

$$
\text{div}(xy) = \text{div}(x) + \text{div}(y)
$$

et

$$
\text{div}(x + y) \geq \inf(\text{div}(x), \text{div}(y)),
$$

pour $ x, y $ et $ x + y $ dans $ K^* $, on déduit que les $ v_P $ sont des valuations discrètes sur $ K $. Pour que $ x \in A $, il faut et il suffit que $ \text{div}(x) \geq 0 $, c’est-à-dire que $ v_P(x) \geq 0 $ pour tout $ P \in P(A) $. Ainsi les $ v_P $ vérifient les conditions (AK_I) et (AK_II), et évidemment aussi (AK_III).

C.Q.F.D.

#### Corollaire {#ac-vii-s1-n3-cor-1 .statement}

Pour qu’un anneau noethérien soit un anneau de Krull, il faut et il suffit qu’il soit intégralement clos.

En effet un anneau noethérien intégralement clos est complètement intégralement clos (chap. V, § 1, n° 4).

Il y a des anneaux de Krull non noethériens, par exemple l’anneau de polynômes $ K[X_n]_{n \in \mathbf{N}} $ sur un corps $ K $, à une infinité d’indéterminées (cf. exerc. 8).

### 4. Valuations essentielles d’un anneau de Krull

Soient A un anneau de Krull, K son corps des fractions. On appelle valuations essentielles de K (ou de A) les valuations $ v_P $ définies par la formule (4) du n° 3 (pour $ x \in K^* $).

On a remarqué, au cours de la démonstration du th. 2, que les valuations $ v_P $ vérifient les propriétés (AK_I), (AK_II) et (AK_III) de la déf. 3. En outre, ces valuations discrètes $ v_P $ sont normées : en effet, pour tout diviseur extrémal $ P \in P(A) $, on a $ P < 2P $, donc, si $ a $ et $ b $ sont les idéaux divisoriaux correspondant à $ P $ et $ 2P $, on a $ a \supset b $ et $ a \neq b $; pour $ x \in a - b $, on a $ \text{div}(x) \geq P $ et $ \text{div}(x) \not\geq 2P $, d’où $ v_P(x) = 1 $, ce qui démontre notre assertion.

#### Proposition 5 {#ac-vii-s1-prop-5 .statement}

Soient $ A $ un anneau de Krull, $ K $ son corps des fractions, et $ (v_P)_{P \in P(A)} $ la famille de ses valuations essentielles. Soit $ (n_P)_{P \in P(A)} $ une famille d’entiers rationnels, nuls sauf pour un nombre fini d’indices. Alors l’ensemble des $ x \in K $ tels que $ v_P(x) \geq n_P $ pour tout $ P \in P(A) $ est l’idéal divisoriel $ a $ de $ A $ tel que $ \operatorname{div} a = \sum_{P \in P(A)} n_P \cdot P $.

Soit $ x \in K^* $. Pour que $ x \in a $, il faut et il suffit que $ Ax \subset a $, donc que $ \operatorname{div}(x) \geq \operatorname{div} a $, donc, d’après (4), que $ v_P(x) \geq n_P $ pour tout $ P \in P(A) $.

#### Proposition 6 {#ac-vii-s1-prop-6 .statement}

Soient $ A $ un anneau de Krull, $ K $ son corps des fractions, $ (v_i)_{i \in I} $ une famille de valuations de $ K $ possédant les propriétés de la déf. 3, et $ A_i $ l’anneau de $ v_i $. Soient $ S $ une partie multiplicative de $ A $ ne contenant pas $ 0 $, et $ J $ l’ensemble des indices $ i \in I $ tels que $ v_i $ soit nulle dans $ S $. Alors on a $ S^{-1}A = \bigcap_{i \in J} A_i $; en particulier $ S^{-1}A $ est un anneau de Krull.

Posons $ B = \bigcap_{i \in J} A_i $. On a $ S^{-1} \subset B $ et $ A \subset B $, donc $ S^{-1}A \subset B $.
Inversement, soit $ x \in B $. Notons $ J' $ l’ensemble fini des indices $ i $ tels que $ v_i(x) < 0 $. Si $ i \in J' $, on a $ x \notin A_i $, donc $ i \notin J $, donc il existe $ s_i \in S $ tel que $ v_i(s_i) > 0 $. Soit $ n(i) $ un entier $ > 0 $ tel que $ v_i(s_i^{n(i)}x) \geq 0 $; posons $ s = \prod_{i \in J'} s_i^{n(i)} $. On a alors $ v_i(sx) \geq 0 $ pour tout $ i \in I $, donc $ sx \in A $, et $ x \in S^{-1}A $. Ainsi $ B = S^{-1}A $.

#### Corollaire 1 {#ac-vii-s1-prop-6-cor-1 .statement}

Soient $ P $ un diviseur extrémal de $ A $, et $ p $ l’idéal divisoriel correspondant. Alors $ p $ est premier, l’anneau de $ v_p $ est $ A_p $ et le corps résiduel de $ v_p $ s’identifie au corps des fractions de $ A/p $.

Soit $ S = A - p $. D’après la prop. 5, $ v_p $ est nulle dans $ S $ et $ > 0 $ dans $ p $. Donc $ p $ est l’intersection de $ A $ et de l’idéal de $ v_p $, et par suite est premier. D’autre part, pour tout diviseur extrémal $ Q \neq P $, on a $ Q \not\supseteq P $, donc l’idéal divisoriel $ q $ correspondant à $ Q $ n’est pas contenu dans $ p $; ainsi $ q \cap S \neq \emptyset $, donc, d’après la prop. 5, $ v_Q $ n’est pas nulle dans $ S $. Ceci étant, le corollaire résulte de la prop. 6 et du chap. II, § 3, n° 1, prop. 3.

#### Corollaire 2 {#ac-vii-s1-prop-6-cor-2 .statement}

Soient $ A $ un anneau de Krull, $ K $ son corps des fractions, et $ (v_i)_{i \in I} $ une famille de valuations possédant les propriétés de la déf. 3. Alors toute valuation essentielle de $ A $ est équivalente à l’une des $ v_i $.

Soient $ P $ un diviseur extrémal de $ A $, et $ p $ l’idéal divisoriel

#### Proposition 7 {#ac-vii-s1-prop-7 .statement}

*Soient A un anneau de Krull, $(v_p)_{P \in P(A)}$ la famille de ses valuations essentielles, et $ a \in I(A) $. Alors le coefficient de P dans div $ a $ est $ \inf_{y \in a} (v_p(y)) $. Si $ p $ est l’idéal premier divisoriel correspondant au diviseur extrémal P, on a $ aA_p = \tilde{a}A_p $.

Comme $ a = \sum_{x \in a} Ax $, la prop. 2, b) (n° 1) montre qu’on a $ \operatorname{div}(a) = \inf_{x \in a} (\operatorname{div}(Ax)) $, d’où notre première assertion. La seconde s’en déduit aussitôt, puisque $ \operatorname{div} \tilde{a} = \operatorname{div} a $ et que $ A_p $ est l’anneau de la valuation discrète $ v_p $.

#### Proposition 8 {#ac-vii-s1-prop-8 .statement}

*Soit A un anneau noethérien intégralement-clos.

a) Soient P un diviseur extrémal de A et $ p $ l’idéal premier divisoriel correspondant; pour $ n \in \mathbf{N} $. posons $ p^{(n)} = p^n A_p \cap A $; alors $ p^{(n)} $ est l’ensemble des $ x \in A $ tels que $ v_p(x) \geq n $, et est un idéal $ p $-primaire.

b) Soient $ a $ un idéal entier divisoriel, $ n_1 P_1 + \cdots + n_r P_r $ le diviseur de $ a $ (les $ P_i $ étant des diviseurs extrémaux distincts), et $ p_i $ l’idéal premier divisoriel correspondant à $ P_i $. Alors $ a = \bigcap_{i=1}^r p_i^{(n_i)} $ est l’unique décomposition primaire réduite de $ a $ et les $ p_i $ sont non immergés.

D’après le cor. 1 de la prop. 6, la relation $ x \in p^n A_p = (pA_p)^n $ équivaut à $ v_p(x) \geq n $; d’autre part, comme $ A_p $ est un anneau de valuation discrète, $ (pA_p)^n $ est $ (pA_p) $-primaire (chap. IV, § 2, n° 1, Exemple 4), donc $ p^{(n)} $ est $ p $-primaire (chap. IV, § 2, n° 1, prop. 3); ceci démontre a). La prop. 5 montre qu’on a bien $ a = \bigcap_{i=1}^r p_i^{(n_i)} $. Comme on a $ p_i \not\subset p_j $ pour $ i \neq j $ cette décomposition primaire est réduite: en effet, si on avait $ p_i^{(n_i)} \supset \bigcap_{j \neq i} p_j^{(n_j)} \supset \prod_{j \neq i} p_j^{n_j} $, $ p_i $ contiendrait l’un des $ p_j $ pour $ j \neq i $ (chap. II, § 1, n° 1, prop. 1). L’unicité résulte du chap. IV, § 2, n° 3, prop. 5.

### 5. Approximation pour les valuations essentielles

Comme les valuations essentielles d’un anneau de Krull sont discrètes et normées, elles sont deux à deux inéquivalentes, donc indépendantes (chap. VI, § 7, n° 2). On peut donc leur appliquer le cor. 1 du théorème d’approximation (loc. cit., th. 1) : étant donnés des $ n_i \in \mathbf{Z} $ et des valuations essentielles $ v_i $ en nombre fini, deux à deux distinctes, il existe $ x \in \mathbf{K} $ tel que $ v_i(x) = n_i $ pour tout $ i $. Mais on a ici un résultat plus précis :

#### Proposition 9 {#ac-vii-s1-prop-9 .statement}

Soient $ v_1, \ldots, v_r $ des valuations essentielles, deux à deux distinctes, d’un anneau de Krull $ \mathbf{A} $, et $ n_1, \ldots, n_r $ des entiers rationnels. Il existe un élément $ x $ du corps des fractions $ \mathbf{K} $ de $ \mathbf{A} $ tel que $ v_i(x) = n_i $ pour $ 1 \leq i \leq r $, et que $ v(x) \geq 0 $ pour toute valuation essentielle $ v $ de $ \mathbf{A} $ distincte de $ v_1, \ldots, v_r $.

Soient, en effet, $ p_1, \ldots, p_r $ les idéaux divisoriels de $ \mathbf{A} $ correspondant aux valuations $ v_1, \ldots, v_r $. Il existe $ y \in \mathbf{K} $ tel que $ v_i(y) = n_i $ pour $ 1 \leq i \leq r $ (chap. VI, § 7, n° 2, cor. 1 du th. 1). Les valuations essentielles $ w_1, \ldots, w_s $ de $ \mathbf{A} $ distinctes des $ v_i $ pour lesquelles l’entier $ w_j(y) = -m_j $ est $ < 0 $ sont en nombre fini ; soient $ q_1, \ldots, q_s $ les idéaux divisoriels correspondants. Il n’existe aucune relation d’inclusion entre $ p_1, \ldots, p_r, q_1, \ldots, q_s $ puisque ces idéaux correspondent à des diviseurs extrémaux, et ces idéaux sont premiers (cor. 1 de la prop. 6). Donc l’idéal entier $ a = q_1^{m_1} \ldots q_s^{m_s} $ n’est contenu dans aucun des $ p_i $ (chap. II, § 1, n° 1, prop. 1), et n’est par conséquent pas contenu dans leur réunion (loc. cit., prop. 2). Par suite, il existe $ z \in a $ tel que $ z \notin p_i $ pour $ 1 \leq i \leq r $; on a $ v_1(z) = \ldots = v_r(z) = 0 $, et $ w_j(z) \geq m_j $ pour $ 1 \leq j \leq s $; donc l’élément $ x = yz $ répond à la question.

#### Corollaire 1 {#ac-vii-s1-prop-9-cor-1 .statement}

Soient $ \mathbf{A} $ un anneau de Krull, $ \mathbf{K} $ son corps des fractions, $ a, b, c $ trois idéaux fractionnaires divisoriels de $ \mathbf{A} $ tels que $ a \subset b $. Il existe $ x \in \mathbf{K} $ tel que $ a = b \cap xc $.

En effet, soit $ (v_\iota)_{\iota \in I} $ la famille des valuations essentielles de $ \mathbf{A} $, et soit $ (m_\iota) $ (resp. $ (n_\iota), (p_\iota) $) la famille d’entiers rationnels (nuls sauf pour un nombre fini d’indices) telle que $ a $ (resp. $ b, c $) soit l’ensemble des $ x \in \mathbf{K} $ pour lesquels $ v_\iota(x) \geq m_\iota $ (resp. $ n_\iota, p_\iota $), quel que soit $ \iota \in I $ (prop. 5, n° 4). L’ensemble $ J $ des $ \iota \in I $ tels que $ m_\iota > n_\iota $ est fini. Comme on a $ p_\iota = m_\iota = 0 $ sauf pour un nombre fini d’indices, la prop. 9 montre qu’il existe $ x \in \mathbf{K}^* $ tel que $ v_\iota(x^{-1}) + m_\iota = p_\iota $ pour $ \iota \in J $ et $ v_\iota(x^{-1}) + m_\iota \geq p_\iota $ pour $ \iota \in I - J $. On a alors, pour tout $ \iota \in I $, $ m_\iota = \sup(n_\iota, v_\iota(x) + p_\iota) $. D’où $ a = b \cap xc $.

#### Corollaire 2 {#ac-vii-s1-prop-9-cor-2 .statement}

Soit $ A $ un anneau de Krull. Pour qu’un idéal fractionnaire $ a $ de $ A $ soit divisoriel, il faut et il suffit qu’il soit intersection de deux idéaux principaux fractionnaires.

La suffisance est évidente (n° 1, déf. 2). La nécessité se déduit du cor. 1 : on prend $ b $ et $ c $ principaux et tels que $ b \supseteq a $.

### 6. Idéaux premiers de hauteur 1 d’un anneau de Krull

#### Définition 4 {#ac-vii-s1-def-4 .statement}

Soit $ A $ un anneau intègre. Un idéal premier $ p $ de $ A $ est dit de hauteur 1 s’il est minimal parmi les idéaux premiers non nuls de $ A $.

Nous dirons aussi que l’idéal (0) dans $ A $ est de hauteur 0 ; un idéal premier de hauteur $ \leqslant 1 $ est donc par définition égal à (0) ou de hauteur 1.

Nous définirons ultérieurement, de manière générale, la hauteur d’un idéal premier.

#### Théorème 3 {#ac-vii-s1-thm-3 .statement}

Soient $ A $ un anneau de Krull, et $ p $ un idéal entier de $ A $. Pour que $ p $ soit l’idéal divisoriel correspondant à un diviseur extrémal, il faut et il suffit que $ p $ soit un idéal premier de hauteur 1.

Si $ p $ est l’idéal divisoriel correspondant à un diviseur extrémal, on sait (n° 4, cor. 1 de la prop. 6) que $ p $ est premier et que $ A_p $ est un anneau de valuation discrète ; comme $ A_p $ n’a d’autres idéaux premiers que (0) et $ pA_p $, (0) et $ p $ sont les seuls idéaux premiers de $ A $ contenus dans $ p $ (chap. II, § 3, n° 1, prop. 3) ; donc $ p $ est de hauteur 1. Réciproquement, nous montrerons d’abord que tout idéal premier $ p \neq (0) $ de $ A $ contient un idéal premier divisoriel $ q $ correspondant à un diviseur extrémal : en effet, comme $ A_p \neq K $, $ A_p $ est l’intersection d’une famille non vide ($ A_i $) d’anneaux de valuations essentielles (n° 4, prop. 6) ; chaque $ A_i $ est de la forme $ A_{q_i} $ (n° 4, cor. 1 de la prop. 6), et, de $ A_p \subset A_{q_i} $ on déduit $ q_i \subset p $. Ainsi, si $ p $ est de hauteur 1, on a $ p = q $, ce qui montre que $ p $ est l’idéal divisoriel correspondant à un diviseur extrémal.

#### Corollaire 1 {#ac-vii-s1-thm-3-cor-1 .statement}

Dans un anneau de Krull, tout idéal premier non nul $ m $ contient un idéal premier de hauteur 1. Si $ m $ n’est pas de hauteur 1, on a $ \operatorname{div} m = 0 $ et $ A : m = A $.

La première assertion a été vue au cours de la démonstration du th. 3. Si $ m $ n’est pas de hauteur 1 et si $ p $ est un idéal premier de hauteur 1 contenu dans $ m $, on a $ p \subset \tilde{m} $ et $ p \neq \tilde{m} $; comme $ \operatorname{div} p $ est extrémal, on a nécessairement div $ m = \operatorname{div} \tilde{m} = 0 $; donc $ \operatorname{div}(A : m) = 0 $ et comme $ A : m $ est divisoriel (n° 1, prop. 1), $ A : m = A $.

#### Corollaire 2 {#ac-vii-s1-thm-3-cor-2 .statement}

Soient $ A $ un anneau de Krull, $ K $ son corps des fractions, $ v $ une valuation de $ K $ positive sur $ A $, et $ p $ l’ensemble des $ x \in A $ tels que $ v(x) > 0 $. Si l’idéal premier $ p $ est de hauteur 1, $ v $ est équivalente à une valuation essentielle de $ A $.

Soient $ B $ l’anneau de $ v $ et $ m $ son idéal. On a $ m \cap A = p $, donc $ A_p \subset B $. Or $ A_p $ est un anneau de valuation discrète (th. 3, et cor. 1 de la prop. 6). Comme $ p \neq (0) $, on a $ B \neq K $, donc $ B = A_p $ (chap. VI, § 4, n° 5, prop. 6).

#### Théorème 4 {#ac-vii-s1-thm-4 .statement}

Soient $ A $ un anneau intègre, $ M $ l’ensemble de ses idéaux premiers de hauteur 1. Pour que $ A $ soit un anneau de Krull, il faut et il suffit que les propriétés suivantes soient vérifiées :
(i) Pour tout $ p \in M $, $ A_p $ est un anneau de valuation discrète.
(ii) $ A $ est l’intersection des $ A_p $ pour $ p \in M $.
(iii) Pour tout $ x \neq 0 $ dans $ A $, il n’existe qu’un nombre fini d’idéaux $ p \in M $ tels que $ x \in p $.

En outre, les valuations correspondant aux $ A_p $ pour $ p \in M $ sont les valuations essentielles de $ A $.

Les conditions sont trivialement suffisantes. Leur nécessité résulte aussitôt du th. 3, du n° 4, cor. 1 de la prop. 6 et du fait que les valuations essentielles de $ A $ vérifient les conditions de la déf. 3 du n° 3.

#### Proposition 10 {#ac-vii-s1-prop-10 .statement}

Soient $ A $ un anneau noethérien intégralement clos, et $ a $ un idéal entier de $ A $. Les conditions suivantes sont équivalentes :
a) $ a $ est divisoriel ;
b) les idéaux premiers associés à $ A/a $ sont de hauteur 1.

Rappelons que, si $ a = \bigcap_{i=1}^n q_i $ est une décomposition primaire réduite de $ a $, et que si $ p_i $ désigne l’idéal premier correspondant à $ q_i $, les idéaux premiers associés à $ A/a $ ne sont autres que les $ p_i $ (chap. IV, § 2, n° 3, prop. 4). Le fait que $ a $ implique $ b $ résulte alors de la prop. 8 du n° 4. Réciproquement, si, avec les notations précédentes, les $ p_i $ sont de hauteur 1, $ A_{p_i} $ est un anneau de valuation discrète (th. 4); or, $ q_i = q_i A_{p_i} \cap A $ (chap. IV, § 2, n° 1, prop. 3); notant $ v_i $ la valuation essentielle correspondant à $ p_i $, il existe donc un entier $ n_i $ tel que $ q_i $ soit l’ensemble des $ x \in A $ tels que $ v_i(x) \geq n_i $; ceci montre que les $ q_i $ sont divisoriels (n° 4, prop. 5), donc aussi $ a $.

### 7. Application: nouvelles caractérisations des anneaux de valuation discrète

#### Proposition 11 {#ac-vii-s1-prop-11 .statement}

Soient $ A $ un anneau de Krull local (en particulier un anneau noethérien local et intégralement clos) et $ m $ son idéal maximal. Les conditions suivantes sont équivalentes:
a) $ A $ est un anneau de valuation discrète ;
b) $ m $ est inversible ;
c) on a $ A : m \neq A ; $
d) $ m $ est divisoriel ;
e) $ m $ est le seul idéal premier non nul de $ A $.

Comme tout idéal non nul d’un anneau de valuation discrète est principal (chap. VI, § 3, n° 6, prop. 9), il est inversible, donc $ a ) $ implique $ b ) $. Si $ m $ est inversible, son inverse est $ A : m $ (chap. II, § 5, n° 6, prop. 10), donc $ A : m \neq A ; $ ainsi $ b ) $ implique $ c ) $. Si $ A : m \neq A $, on a $ A : (A : m) \neq A ; $ or $ m \subset A : (A : m) ; $ donc $ m = A : (A : m) $ puisque $ m $ est maximal, de sorte que $ m $ est divisoriel (n° 1, prop. 1, c)); ainsi $ c ) $ implique $ d ) $. Le fait que $ d ) $ implique $ e ) $ résulte du th. 3 du n° 6. Enfin, si $ m $ est le seul idéal premier non nul de $ A $, il est de hauteur 1, donc $ A_m $ est un anneau de valuation discrète (n° 6, th. 4); comme $ A $ est local, on a $ A_m = A $, ce qui montre que $ e ) $ implique $ a ) $.

### 8. Fermeture intégrale d’un anneau de Krull dans une extension finie de son corps des fractions

#### Proposition 12 {#ac-vii-s1-prop-12 .statement}

Soient $ A $ un anneau de Krull, $ K $ son corps des fractions, $ K' $ une extension de degré fini de $ K $, et $ A' $ la fermeture intégrale de $ A $ dans $ K' $. Alors $ A' $ est un anneau de Krull. Les valuations essentielles de $ A' $ sont les valuations discrètes normées de $ K' $ qui sont équivalentes aux prolongements des valuations essentielles de $ A $.

Soit $ (v_i)_{i \in I} $ la famille des prolongements à $ K' $ des valuations essentielles de $ A $. Puisque le degré $ n = [K' : K] $ est fini, les $ v_i $ sont des valuations discrètes de $ K' $ (chap. VI, § 8, n° 1, cor. 3 de la prop. 1). Soit $ B_i $ l’anneau de $ v_i $; on a $ A' \subset \bigcap_{i \in I} B_i $ (chap. VI, § 1, n° 3, th. 3). Inversement, tout élément $ x $ de $ \bigcap_{i \in I} B_i $ est entier sur chacun des anneaux des valuations essentielles de $ A $ (chap. VI, § 1, n° 3, cor. 3 du th. 3); donc les coefficients du polynôme

Il reste à montrer que les $ v_i $ sont équivalentes à des valuations essentielles de $ A' $ (n° 4, cor. 2 de la prop. 6), c’est-à-dire (n° 6, cor. 2 du th. 3) que l’idéal premier $ p_i $, formé par les $ x \in A' $ tels que $ v_i(x) > 0 $, est de hauteur 1. S’il n’en était pas ainsi, il existerait un idéal premier $ q $ de $ A' $ tel que $ (0) \subset q \subset p_i $ distinct de $ (0) $ et de $ p_i $; on aurait alors $ (0) \subset q \cap A \subset p_i \cap A $, et $ q \cap A $ serait distinct de $ (0) $ et de $ p_i \cap A $ (chap. V, § 2, n° 1, cor. 1 de la prop. 1); l’idéal premier $ p_i \cap A $ ne serait donc pas de hauteur 1, ce qui contredit le fait qu’il correspond à une valuation essentielle de $ A $.

COROLLAIRE . — Soient $ p $ (resp. $ p' $) un idéal premier de hauteur 1 de $ A $ (resp. $ A' $), et $ v $ (resp. $ v' $) la valuation essentielle de $ A $ (resp. $ A' $) qui lui correspond. Pour que $ p' $ soit au-dessus de $ p $, il faut et il suffit que la restriction de $ v' $ à $ K $ soit équivalente à $ v $.

La valuation $ v' $ est équivalente au prolongement d’une valuation essentielle $ w $ de $ A $ (prop. 12). Soit $ q = p' \cap A $, qui est un idéal premier de hauteur 1 de $ A $. Pour que la restriction de $ v' $ à $ K $ soit équivalente à $ v $, il faut et il suffit que $ w = v $, donc que $ q = p $.

### 9. Anneaux de polynômes sur un anneau de Krull

#### Proposition 13 {#ac-vii-s1-prop-13 .statement}

Soient $ A $ un anneau de Krull, $ X_1, X_2, \ldots, X_n $ des indéterminées. L’anneau $ A[X_1, \ldots, X_n] $ est un anneau de Krull.

Raisonnant par récurrence sur $ n $, il suffit de montrer que, si $ X $ est une indéterminée, $ A[X] $ est un anneau de Krull. Soit $ K $ le corps des fractions de $ A $. Le corps des fractions de $ A[X] $ est $ K(X) $. Soit $ I $ l’ensemble des polynômes unitaires de $ K[X] $ irréductibles sur $ K $; pour tout $ f \in I $, soit $ v_f $ la valuation de $ K(X) $ définie par $ f $ (chap. VI, § 3, n° 3, Exemple 4). D’autre part, pour toute valuation essentielle $ w $ de $ A $, soit $ \bar{w} $ le prolongement de $ w $ à $ K(X) $ défini par
$$
\bar{w}\left( \sum_j a_j X^j \right) = \inf_j(w(a_j)) \text{ pour } \sum_j a_j X^j \in K[X] \text{ (chap. VI, § 10, n° 1, lemme 1).}
$$
Il est clair que les $ v_f $ et les $ \bar{w} $ sont discrètes, normées, et que, pour tout $ u \in K[X] $, on a $ v_f(u) = 0 $ (resp. $ \bar{w}(u) = 0 $), sauf pour un nombre fini de valuations $ v_f $ (resp. $ \bar{w} $).

Pour démontrer la proposition, il suffit donc de montrer que $ A[X] $ est l’intersection des anneaux des valuations $ v_f $ et $ \bar{w} $. Or l’intersection des anneaux des valuations $ v_f $ est $ K[X] $. D’autre part, pour $ \sum_j a_j X^j \in K[X] $, la relation $ \bar{w} \left( \sum_j a_j X^j \right) \geqslant 0 $ équivaut à « $ w(a_j) \geqslant 0 $ pour tout $ j $ »; donc la relation « $ \bar{w} \left( \sum_j a_j X^j \right) \geqslant 0 $ pour toute valuation $ \bar{w} $ » équivaut à « $ w(a_j) \geqslant 0 $ pour tout $ j $ et toute valuation essentielle $ w $ de $ A $ ». Ceci démontre notre assertion.

#### Remarque {#ac-vii-s1-n9-rem-1 .statement}

Les valuations $ v_f $ et $ \bar{w} $ introduites dans la démonstration de la prop. 13 sont les valuations essentielles de $ A[X] $. Il nous suffira de montrer que si $ V $ est l’ensemble des valuations $ v_f $ ($ f $ irréductible) et $ \bar{w} $ ($ w $ essentielle), alors, pour toute $ v' \in V $, il existe un élément $ g \in K(X) $ non dans $ A[X] $ tel que $ v''(g) \geqslant 0 $ pour toutes les valuations $ v'' \in V $ distinctes de $ v' $; cela prouvera que $ V - \{ v' \} $ ne vérifie pas (AK$_{II}$) et la conclusion résultera donc du n° 4, cor. 2 de la prop. 6. Supposons d’abord que $ v' $ soit de la forme $ \bar{w} $: on peut alors prendre pour $ g $ un élément $ b \in K $ tel que $ w(b) < 0,\ w'(b) \geqslant 0 $ pour les valuations essentielles $ w' $ de $ A $ distinctes de $ w $, car on aura alors $ v_f(b) = 0 $ pour tout polynôme unitaire irréductible $ f $ de $ K[X] $; l’existence d’un élément $ b $ vérifiant les conditions précédentes résulte du n° 5, prop. 9. Supposons en second lieu que $ v' $ soit de la forme $ v_f $ pour un polynôme unitaire irréductible $ f \in K[X] $ de degré $ m $; on peut alors prendre $ g = a/f $ avec $ a \in A $. En effet, on aura $ v_h(g) \geqslant 0 $ pour tout polynôme unitaire irréductible $ h \neq f $ de $ K[X] $; reste à choisir $ a \in A $ tel que pour toute valuation essentielle $ w $ de $ A $, $ w(a) $ soit au moins égal à la borne inférieure des éléments $ w(c_i) $, où les $ c_i $ sont les coefficients de $ f $ ($ 1 \leqslant i \leqslant m $); or l’existence d’un tel $ a \in A $ résulte de (AK$_{III}$) et du n° 5, prop. 9.

On peut encore dire (n° 6, th. 4) que les idéaux premiers de hauteur 1 de $ A[X] $ sont :

1) les idéaux premiers de la forme $ pA[X] $, où $ p $ est un idéal premier de hauteur 1 de $ A $;

2) les idéaux premiers de la forme $ m \cap A[X] $, où $ m $ est un idéal premier (nécessairement principal) de $ K[X] $.

Les seconds se caractérisent par le fait que leur intersection avec $ A $ est réduite à 0.

### 10. Classes de diviseurs dans les anneaux de Krull

Soit $ A $ un anneau de Krull. Rappelons que le groupe $ D(A) $ de diviseurs de $ A $ est le groupe commutatif libre engendré par l’ensemble $ P(A) $ de ses éléments extrémaux (n° 3, th. 2), et que $ P(A) $ s’identifie à l’ensemble des idéaux premiers de hauteur 1 de $ A $ (n° 6); pour $ p \in P(A) $, nous noterons $ v_p $ la valuation essentielle normée correspondant à $ p $ (n° 4); rappelons que l’anneau de $ v_p $ est $ A_p $ (n° 4, cor. 1 de la prop. 6). Nous noterons $ F(A) $ le sous-groupe de $ D(A) $ formé des diviseurs principaux, et par $ C(A) = D(A)/F(A) $ le groupe des classes de diviseurs de $ A $ (n° 2).

#### Proposition 14 {#ac-vii-s1-prop-14 .statement}

Soient $ A $ un anneau de Krull, et $ B $ un anneau de Krull contenant $ A $. On suppose vérifiée la condition suivante:
(PDE) Pour tout idéal premier $ \mathfrak{P} $ de hauteur 1 de $ B $, l’idéal premier $ \mathfrak{P} \cap A $ est nul ou de hauteur 1.
Pour $ p \in P(A) $, les $ \mathfrak{P} \in P(B) $ tels que $ \mathfrak{P} \cap A = p $ sont en nombre fini; posons
$$
i(p) = \sum_{\mathfrak{P} \in P(B), \mathfrak{P} \cap A = p} e(\mathfrak{P}/p) \mathfrak{P},
$$
où $ e(\mathfrak{P}/p) $ désigne l’indice de ramification de $ v_{\mathfrak{P}} $ par rapport à $ v_p $ (chap. VI, § 8, n° 1 ). Alors $ i $ définit, par linéarité, un homomorphisme croissant de $ D(A) $ dans $ D(B) $ qui jouit des propriétés suivantes:
a) pour tout élément non nul $ x $ du corps des fractions de $ A $, on a
$$
i(\operatorname{div}_A(x)) = \operatorname{div}_B(x);
$$
b) quels que soient $ D, D' $ dans $ D(A) $, on a
$$
i(\sup(D, D')) = \sup(i(D), i(D'));
$$
Soit, en effet, $ p \in P(A) $; considérons un élément non nul $ a $ de $ p $; les $ \mathfrak{P} \in P(B) $ qui contiennent $ a $ sont en nombre fini (n° 6, th. 4); $ a $ fortiori les $ \mathfrak{P} \in P(B) $ tels que $ \mathfrak{P} \cap A = p $ sont en nombre fini.
Démontrons maintenant $ a $. Par additivité, on peut supposer $ x \in A^* = A - \{0\} $. Par définition, on a $ \operatorname{div}_B(x) = \sum_{\mathfrak{P} \in P(B)} v_{\mathfrak{P}}(x) \cdot \mathfrak{P} $.
Pour tout $ \mathfrak{P} \in P(B) $ tel que $ v_{\mathfrak{P}}(x) > 0 $, $ \mathfrak{P} \cap A $ n’est pas nul (car $ x \in \mathfrak{P} $), et est donc de hauteur 1 d’après (PDE); posant $ p = \mathfrak{P} \cap A $, on a, par définition de l’indice de ramification, $ v_{\mathfrak{P}}(x) = e(\mathfrak{P}/p)v_p(x) $ (puisque $ v_p $ et $ v_{\mathfrak{P}} $ sont normées). Comme $ \operatorname{div}_A(x) = \sum_{p \in P(A)} v_p(x) \cdot p $, et que $ i(q) = 0 $ pour tout $ q \in P(A) $ qui n’est pas de la forme $ Q \cap A $ avec $ Q \in P(B) $, on en déduit $ a) $.

Pour démontrer $ b) $, posons
$$
D = \sum_{p \in P(A)} n(p) \cdot p \quad \text{et} \quad D' = \sum_{p \in P(A)} n'(p) \cdot p;
$$
le coefficient de $ p $ dans $ \sup(D, D') $ est $ \sup(n(p), n'(p)) $. Soit $ \mathfrak{P} $ un élément de $ P(B) $. Si $ \mathfrak{P} \cap A = (0) $, les coefficients de $ \mathfrak{P} $ dans $ i(D) $ et $ i(D') $, donc aussi dans $ \sup(i(D), i(D')) $, sont nuls ; par suite le coefficient de $ \mathfrak{P} $ dans $ i(\sup(D, D')) $ est nul. Si $ \mathfrak{P} \cap A \neq (0) $, c’est un idéal premier $ p $ de hauteur 1 (d’après (PDE)) ; posant $ e = e(\mathfrak{P}/p) $, les coefficients de $ \mathfrak{P} $ dans $ i(D), i(D') $ et $ i(\sup(D, D')) $ sont respectivement $ en(p), en'(p) $ et $ e \cdot \sup(n(p), n'(p)) $; celui de $ \sup(i(D), i(D')) $ est $ \sup(e \cdot n(p), e \cdot n'(p)) = e \cdot \sup(n(p), n'(p)) $. Ceci démontre $ b) $.

Sous les hypothèses de la prop. 14, il résulte de $ a) $ que $ i $ définit, par passage aux quotients, un homomorphisme $ \bar{i} $, dit canonique, de $ C(A) $ dans $ C(B) $, que nous écrirons encore parfois $ i $, par abus de notation.

La condition (PDE) est satisfaite dans les deux cas suivants :
1) B est entier sur A ; dans ce cas, pour que l’idéal premier $ \mathfrak{P} $ de B soit de hauteur 1, il faut et il suffit que $ p = \mathfrak{P} \cap A $ soit de hauteur 1. En effet, (0) est le seul idéal premier de B au-dessus de l’idéal (0) de A (chap. V, § 2, no 1, cor. 1 de la prop. 1); si $ \mathfrak{P} $ est de hauteur 1, on a donc $ p \neq 0 $; si $ p $ n’était pas de hauteur 1, il existerait un idéal premier $ p' $ de A, distinct de 0 et de $ p $ et tel que $ 0 \subset p' \subset p $; mais alors, comme B est intègre et A intégralement clos, il y aurait un idéal premier $ \mathfrak{P}' $ de B tel que $ \mathfrak{P}' \cap A = p' $ et $ \mathfrak{P}' \subset \mathfrak{P} $ (chap. V, § 2, no 4, th. 3), contrairement à l’hypothèse. Inversement, si $ p $ est de hauteur 1, il ne peut exister d’idéal premier $ \mathfrak{P}' $ de B, distinct de 0 et de $ \mathfrak{P} $ et tel que $ 0 \subset \mathfrak{P}' \subset \mathfrak{P} $, sans quoi on aurait $ 0 \subset \mathfrak{P}' \cap A \subset p $, et $ \mathfrak{P}' \cap A $ serait distinct de 0 et de $ p $ en vertu du chap. V, § 2, no 1, cor. 1 de la prop. 1.

2) B est un A-module plat. Plus précisément :

#### Proposition 15 {#ac-vii-s1-prop-15 .statement}

Soient A et B des anneaux de Krull tels que B contienne A et soit un A-module plat. Alors :
a) la condition (PDE) de la prop. 14 est satisfaite ;

b) pour tout idéal divisoriel $ a $ de $ A $, $ Ba $ est l’idéal divisoriel de $ B $ qui correspond au diviseur $ i(\operatorname{div}_A(a)) $.

Pour démontrer $ a) $, supposons qu’il existe un idéal premier $ \mathfrak{p} $ de hauteur 1 de $ B $ tel que $ \mathfrak{p} \cap A $ ne soit ni nul, ni de hauteur 1. Prenons un élément $ x \neq 0 $ dans $ \mathfrak{p} \cap A $. Les idéaux $ p_i $ de hauteur 1 de $ A $ qui contiennent $ x $ sont en nombre fini, et aucun ne contient $ \mathfrak{p} \cap A $; il existe donc un élément $ y $ de $ \mathfrak{p} \cap A $ tel que $ y \notin p_i $ pour tout $ i $ (chap. II, § 2, n° 1, prop. 2). Ainsi $ \operatorname{div}_A(x) $ et $ \operatorname{div}_A(y) $ sont des éléments étrangers du groupe ordonné $ P(A) $, de sorte que $ \sup(\operatorname{div}_A(x), \operatorname{div}_A(y)) = \operatorname{div}_A(x) + \operatorname{div}_A(y) = \operatorname{div}_A(xy) $; comme les idéaux $ Ax \cap Ay $ et $ Axy $ sont divisoriels, on en déduit $ Ax \cap Ay = Axy $. Puisque $ B $ est un $ A $-module plat, on a donc $ Bx \cap By = Bxy $ (chap. I, § 2, n° 6, prop. 6). Ceci implique $ \sup(v_{\mathfrak{p}}(x), v_{\mathfrak{p}}(y)) = v_{\mathfrak{p}}(xy) = v_{\mathfrak{p}}(x) + v_{\mathfrak{p}}(y) $, ce qui contredit les inégalités $ v_{\mathfrak{p}}(x) > 0,\ v_{\mathfrak{p}}(y) > 0 $ (qui ont lieu puisque $ x $ et $ y $ sont dans $ \mathfrak{p} $). Ainsi $ a) $ est démontré par l’absurde.

Démontrons $ b) $. Si $ a $ est un idéal divisoriel de $ A $, c’est l’intersection de deux idéaux principaux fractionnaires (n° 5, cor. 2 de la prop. 9), soit $ a = d^{-1}(Aa \cap Ab) $ avec $ a, b, d $ dans $ A^* $; comme $ B $ est plat sur $ A $, on a $ Ba = d^{-1}(Ba \cap Bb) $ (chap. I, § 2, n° 6, prop. 6), ce qui montre que $ Ba $ est divisoriel. Ceci montre aussi que $ \operatorname{div}_B(Ba) = \sup(\operatorname{div}_B(a), \operatorname{div}_B(b)) - \operatorname{div}_B(d) $; utilisant la prop. 14, $ a) $ et $ b) $, on voit que $ \operatorname{div}_B(Ba) = \sup(i(\operatorname{div}_A(a)), i(\operatorname{div}_A(b))) - i(\operatorname{div}_A(d)) $
$ = i(\sup(\operatorname{div}_A(a), \operatorname{div}_A(b))) - i(\operatorname{div}_A(d)) = i(\operatorname{div}_A(Aa \cap Ab)) - i(\operatorname{div}_A(d)) $
$ = i(\operatorname{div}_A(d^{-1}(Aa \cap Ab))) = i(\operatorname{div}_A(a)) $.

#### Corollaire {#ac-vii-s1-n10-cor-1 .statement}

Soient $ A $ un anneau de Krull local, et $ B $ un anneau de valuation discrète tel que $ B $ domine $ A $ et soit un $ A $-module plat. Alors $ A $ est un corps ou un anneau de valuation discrète.

Soit, en effet, $ \mathfrak{m} $ l’idéal maximal de $ B $. D’après (PDE), $ \mathfrak{m} \cap A $ est nul ou de hauteur 1. Comme c’est, par hypothèse, l’idéal maximal de $ A $, notre assertion résulte de la prop. 11 du n° 7.

#### Remarque {#ac-vii-s1-n10-rem-1 .statement}

Dans le premier des deux cas précédents, l’application $ i : D(A) \to D(B) $ est injective : comme les éléments de $ P(B) $ forment une base de $ D(B) $ et que deux idéaux distincts de $ P(A) $ ne peuvent être traces sur $ A $ du même idéal de $ P(B) $, tout revient à voir que $ i(p) \neq 0 $ pour tout $ p \in P(A) $; or, cela résulte du chap. V, § 2, n° 1, th. 1. On voit de même que lorsque $ B $ est un $ A $-module fidèlement plat, $ i $ est injective (chap. II, § 2, n° 5, cor. 4 de la prop. 11).

Dans ce qui suit, nous nous proposons d’étudier l’homomorphisme canonique $ i $ de $ C(A) $ dans $ C(B) $ pour certains couples d’anneaux de Krull $ A, B $.

#### Proposition 16 {#ac-vii-s1-prop-16 .statement}

*Soit $ A $ un anneau de Zariski tel que son complété $ \hat{A} $ soit un anneau de Krull. Alors $ A $ est un anneau de Krull, et l’homomorphisme canonique $ i $ de $ C(A) $ dans $ C(\hat{A}) $ (qui est défini puisque $ \hat{A} $ est un $ A $-module plat ; cf. chap. III, § 3, n° 4, th. 3) est injectif.*

Comme $ \hat{A} $ est intègre et $ A \subset \hat{A} $, $ A $ est intègre. Soient $ L $ le corps des fractions de $ \hat{A} $, et $ K \subset L $ celui de $ A $. Comme $ A = \hat{A} \cap K $ (chap. III, § 3, n° 5, cor. 4 de la prop. 9), $ A $ est un anneau de Krull (n° 3, *Exemple 4*). L’injectivité de $ i : C(A) \to C(\hat{A}) $ résulte de la prop. 15b) et du fait que, si $ b\hat{A} $ est principal, $ b $ est principal (chap. III, § 3, n° 5, cor. 3 de la prop. 9).

C.Q.F.D.

Soient maintenant $ A $ un anneau de Krull, et $ S $ une partie *multiplicative* de $ A $ ne contenant pas 0. Le groupe $ D(A) $ (resp. $ D(S^{-1}A) $) est le groupe commutatif libre ayant pour base l’ensemble des $ \mathrm{div}(p) $ (resp. $ \mathrm{div}(S^{-1}p) $), où $ p $ parcourt l’ensemble des idéaux premiers de hauteur 1 de $ A $ (resp. l’ensemble des idéaux premiers de hauteur 1 de $ A $ tels que $ p \cap S = \phi $) (n° 4, prop. 6) et si $ p \cap S = \phi $ on a $ i(\mathrm{div}(p)) = \mathrm{div}(S^{-1}p) $. Ainsi $ D(S^{-1}A) $ s’identifie au *facteur direct* de $ D(A) $ engendré par les éléments $ \mathrm{div}(p) $ tels que $ p \cap S = \phi $, et admet pour supplémentaire le sous-groupe commutatif libre de $ D(A) $ ayant pour base l’ensemble des $ \mathrm{div}(p) $ tels que $ p \cap S \neq \phi $; nous noterons $ G $ ce supplémentaire. Comme $ i : D(A) \to D(S^{-1}A) $ est surjectif, il en est de même de $ i : C(A) \to C(S^{-1}A) $; et on a :

(5) $$
G/(G \cap F(A)) = (G + F(A))/F(A) = \mathrm{Ker}(i);
$$

en effet, si un élément de $ D(S^{-1}A) $ est égal à $ \mathrm{div}_{S^{-1}A}(x/s) $ où $ x \in A $ et $ s \in S $, il est l’image par $ i $ du diviseur principal $ \mathrm{div}_A(x) $ (prop. 14).

Supposons maintenant que $ S $ soit engendrée par une famille d’éléments $ (p_i)_{i \in I} $ de $ A $ tels que les idéaux principaux $ Ap_i $ soient tous *premiers*. Alors, si $ p $ est un idéal premier de hauteur 1 de $ A $ tel que $ p \cap S \neq \phi $, $ p $ contient un produit de puissances des $ p_i $, et donc l’un des $ p_i $, soit $ p_\alpha $; comme $ Ap_\alpha $ est non nul et premier, et que $ p $ est de hauteur 1, il en résulte que $ p = Ap_\alpha $. Avec les notations ci-dessus, on a donc $ G \subset F(A) $, et (5) montre que le noyau de $ i $ est nul. On a donc démontré le résultat suivant :

#### Proposition 17 {#ac-vii-s1-prop-17 .statement}

Soient $ A $ un anneau de Krull, et $ S $ une partie multiplicative de $ A $ ne contenant pas $ 0 $. Alors l’homomorphisme canonique $ i $ de $ C(A) $ dans $ C(S^{-1}A) $ est surjectif. Si, de plus, $ S $ est engendrée par une famille d’éléments $ p_i $ tels que les idéaux principaux $ Ap_i $ soient tous premiers, alors $ i $ est bijectif.

Comme seconde application de la formule (5), considérons la situation suivante : soit $ R $ un anneau de Krull ; prenons pour $ A $ l’anneau de polynômes $ A = R[X] $ (n° 9, prop. 13), et pour $ S $ l’ensemble $ R - (0) $ des polynômes constants non nuls de $ A $. Les idéaux premiers $ p $ de hauteur 1 de $ A $ tels que $ p \cap S \neq \phi $ sont ceux de la forme $ p_0A $, où $ p_0 $ est un idéal premier de hauteur 1 de $ R $ (n° 9, Remarque). Donc, avec les notations introduites ci-dessus, $ G $ s’identifie à $ D(R) $ en identifiant $ \operatorname{div}_A(p_0A) $ à $ \operatorname{div}_R(p_0) $. D’autre part $ G \cap F(A) $ s’identifie à $ F(R) $ : en effet, si un idéal $ a_0 $ de $ R $ engendre un idéal principal $ a_0A = f(X)A $ dans $ A = R[X] $, on a $ f(0) \in a_0A $ puisque $ a_0A $ est un idéal gradué de l’anneau $ A $ (gradué par le degré usuel des polynômes), donc $ f(0) \in a_0 $; de plus, pour $ a \in a_0 $, on a $ a = f(X)g(X) $ avec $ g(X) \in R $, d’où par comparaison des termes de degré 0, $ a = f(0)g(0) $; il s’ensuit que $ a_0 $ est l’idéal principal de $ R $ engendré par $ f(0) $. Enfin, en notant $ K $ le corps des fractions de $ R $, $ S^{-1}A $ s’identifie à l’anneau de polynômes $ K[X] $, qui est principal ; donc $ C(S^{-1}A) = (0) $. Ainsi, en vertu de (5), $ C(A) = \operatorname{Ker}(i) $ s’identifie à $ C(R) $, et on a démontré le résultat suivant :

#### Proposition 18 {#ac-vii-s1-prop-18 .statement}

Soient $ R $ un anneau de Krull, et $ A $ l’anneau de polynômes $ R[X] $. L’homomorphisme canonique de $ C(R) $ dans $ C(R[X]) $ est bijectif.

## EXERCICES {#ac-vii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
