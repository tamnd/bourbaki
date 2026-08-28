---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: ""
chapter_title: ""
section: 0
section_title: INTRODUCTION AUX CHAPITRES IV, V ET VI
kind: introduction
lang: fr
source: lie-iv-vi-fr
pdf_pages: 0006-0007
extraction: ocr
statements: 0
exercises: 0
content_sha256: 2522e998fc93388b521f6dfdf19ae664d5a75bb651bb96244e8ba4133bd364d3
---

## INTRODUCTION AUX CHAPITRES IV, V ET VI

L’étude des groupes semi-simples (analytiques ou algébriques) et de leurs algèbres de Lie conduit à la considération des structures de systèmes de racines, groupes de Coxeter et systèmes de Tits. Les chapitres IV, V et VI sont consacrés à ces structures.

Pour orienter le lecteur, nous en donnons ci-dessous quelques exemples.

I. Soient $ g $ une algèbre de Lie semi-simple complexe et $ \mathfrak{h} $ une sous-algèbre de Cartan de $ g $ (*). Une racine de $ g $ par rapport à $ \mathfrak{h} $ est une forme linéaire non nulle $ \alpha $ sur $ \mathfrak{h} $ telle qu’il existe un élément $ x $ non nul de $ g $ avec $[h, x] = \alpha(h)x$ pour tout $ h \in \mathfrak{h} $. Ces racines forment dans l’espace vectoriel $ \mathfrak{h}^* $ dual de $ \mathfrak{h} $ un système de racines réduit $ R $. La donnée de $ R $ détermine $ g $ à un isomorphisme près et tout système de racines réduit est isomorphe à un système de racines obtenu de cette manière. Un automorphisme de $ g $ laissant stable $ \mathfrak{h} $ définit un automorphisme de $ \mathfrak{h}^* $ laissant $ R $ invariant, et l’on obtient ainsi tout automorphisme de $ R $. Le groupe de Weyl de $ R $ se compose des automorphismes de $ \mathfrak{h}^* $ définis par les automorphismes intérieurs de $ g $ laissant stable $ \mathfrak{h} $; c’est un groupe de Coxeter.

Soient $ G $ un groupe de Lie complexe connexe, d’algèbre de Lie $ g $, et $ \Gamma $ le sous-groupe de $ \mathfrak{h} $ formé des éléments $ h $ tels que $ \exp_G(2\pi i h) = 1 $. Soit $ R^\vee $ le système de racines dans $ \mathfrak{h} $ inverse de $ R $, soit $ Q(R^\vee) $ le sous-groupe de $ \mathfrak{h} $ engendré par $ R^\vee $ et soit $ P(R^\vee) $ le sous-groupe associé au sous-groupe $ Q(R) $ de $ \mathfrak{h}^* $ engendré par $ R $ (i.e. l’ensemble des $ h \in \mathfrak{h} $ tels que $ \lambda(h) $ soit entier pour tout $ \lambda \in Q(R) $). On a alors $ P(R^\vee) \supset \Gamma \supset Q(R^\vee) $. De plus le centre de $ G $ est canoniquement isomorphe à $ P(R^\vee)/\Gamma $ et le groupe fondamental de $ G $ à $ \Gamma/Q(R^\vee) $. En particulier, $ \Gamma $ est égal à $ P(R^\vee) $ si $ G $ est le groupe adjoint et $ \Gamma $ est égal à $ Q(R^\vee) $ si $ G $ est simplement connexe. Enfin les poids des représentations linéaires de dimension finie de $ G $ sont les éléments du sous-groupe de $ \mathfrak{h}^* $ associé à $ \Gamma $.

(*) Nous utilisons librement dans cette Introduction la terminologie traditionnelle ainsi que les notions définies dans les chapitres IV, V et VI.

II. Soit G un groupe de Lie réel compact connexe semi-simple et soit g son algèbre de Lie. Soient T un tore maximal de G, d’algèbre de Lie t, et X le groupe des caractères de T. Soit R l’ensemble des éléments α non nuls de X tels qu’il existe un élément x non nul de g avec (Ad t).x = α(t)x pour tout t ∈ T. Identifions X à un réseau de l’espace vectoriel réel V = X ⊗_Z R; alors R est un système de racines réduit dans V. Soit N le normalisateur de T dans G; l’action de N sur T définit un isomorphisme du groupe N/T sur le groupe de Weyl de R. On a P(R) ⊃ X ⊃ Q(R); de plus, on a X = P(R) si G est simplement connexe et X = Q(R) si le centre de G est réduit à l’élément neutre.

L’algèbre de Lie g_{(C)} complexifiée de g est semi-simple et t_{(C)} en est une sous-algèbre de Cartan. Il existe un isomorphisme canonique de V_{(C)} sur le dual de t_{(C)} qui transforme R en le système de racines de g_{(C)} par rapport à t_{(C)}.

III. Soit G un groupe algébrique semi-simple connexe sur un corps commutatif k. Soient T un élément maximal de l’ensemble des tores de G déployés sur k et X le groupe des caractères de T (homomorphismes de T dans le groupe multiplicatif). On identifie X à un réseau de l’espace vectoriel réel V = X ⊗_Z R. Les racines de G par rapport à T sont les éléments α non nuls de X tels qu’il existe un élément x non nul de l’algèbre de Lie g de G avec (Ad t).x = α(t)x pour tout point t de T. On obtient ainsi un système de racines R dans V, qui n’est pas nécessairement réduit. Soient N le normalisateur et Z le centralisateur de T dans G et soient N(k) et Z(k) leurs groupes de points rationnels sur k. L’action de N(k) sur T définit un isomorphisme de N(k)/Z(k) sur le groupe de Weyl de R.

Soit U un élément maximal de l’ensemble des sous-groupes unipotents de G, définis sur k et normalisés par Z. Posons P = Z . U. On a P(k) = Z(k) . U(k) et P(k) ∩ N(k) = Z(k). De plus, il existe une base (α₁, ..., αₙ) de R telle que les poids de T dans U soient les racines de R positives pour cette base; le quadruplet (G(k), P(k), N(k), S), où S désigne l’ensemble des éléments de N(k)/Z(k) correspondant grâce à l’isomorphisme défini plus haut aux symétries s_{αᵢ} ∈ W(R) associées aux racines αᵢ, est un système de Tits.

IV. Dans la théorie des groupes algébriques semi-simples sur un corps local, on rencontre des systèmes de Tits dont le groupe W est le groupe de Weyl affine d’un système de racines. Soit, par exemple, G = SL(n + 1, Q_p) (avec n ≥ 1). Soit B le groupe des matrices (a_{ij}) ∈ SL(n + 1, Z_p) telles que a_{ij} ∈ pZ_p pour i < j et soit N le sous-groupe de G formé des matrices n’ayant qu’un seul élément non nul dans chaque ligne et dans chaque colonne. Il existe alors une partie S de N/(B ∩ N) telle que le quadruplet (G, N, B, S) soit un système de Tits. Le groupe W = N/(B ∩ N) est le groupe de Weyl affine d’un système de racines de type A_n; c’est un groupe de Coxeter infini.

Pour la rédaction de ces trois chapitres, de nombreuses conversations avec J. Tits nous ont apporté une aide précieuse. Nous l’en remercions très amicalement.
