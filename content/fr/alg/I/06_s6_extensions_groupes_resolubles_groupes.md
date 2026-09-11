---
book: alg
book_title: Algebra
chapter: I
chapter_title: STRUCTURES ALGÉBRIQUES
section: 6
section_title: Extensions, groupes résolubles, groupes nilpotents
lang: fr
source: alg-i-iii-fr
book_pages: A I.62-A I.77, A I.134-A I.143
pdf_pages: 0072-0087, 0144-0153
extraction: ocr
subsections:
    - "no": 1
      title: Extensions
      page: 62
      pdf_page: 72
    - "no": 2
      title: Commutateurs
      page: 65
      pdf_page: 75
    - "no": 3
      title: Suite centrale descendante, groupes nilpotents
      page: 68
      pdf_page: 78
    - "no": 4
      title: Suite dérivée, groupes résolubles
      page: 71
      pdf_page: 81
    - "no": 5
      title: $p$-groupes
      page: 72
      pdf_page: 82
    - "no": 6
      title: Sous-groupes de Sylow
      page: 74
      pdf_page: 84
    - "no": 7
      title: Groupes nilpotents finis
      page: 76
      pdf_page: 86
statements: 68
exercises: 41
content_sha256: 9a17e5ddfce7be6cf12f2f03d20e1760bf61223d7661f7b621abde2958295d00
---

## § 6. EXTENSIONS, GROUPES RÉSOLUBLES, GROUPES NILPOTENTS

Dans tout ce paragraphe, les lois de groupe sont, sauf mention expresse du contraire, notées multiplicativement.

### 1. Extensions

#### Définition 1 {#alg-i-s6-def-1 .statement}

Soient $F$ et $G$ deux groupes. Une extension de $G$ par $F$ est un triplet $\mathcal{E} = (E, i, p)$, où $E$ est un groupe, $i$ un homomorphisme injectif de $F$ dans $E$ et $p$ un homomorphisme surjectif de $E$ sur $G$ tels que $\operatorname{Im}(i) = \operatorname{Ker}(p)$. On appelle section (resp. rétraction) de l’extension $\mathcal{E}$ un homomorphisme $s : G \to E$ (resp. $r : E \to F$) tel que $p \circ s = \operatorname{Id}_G$ (resp. $r \circ i = \operatorname{Id}_F$).

Une extension $\mathcal{E} = (E, i, p)$ de $G$ par $F$ est souvent désignée par le diagramme $\mathcal{E} : F \xrightarrow{i} E \xrightarrow{p} G$, dans lequel on omet parfois $i$ et $p$ lorsqu’aucune confusion n’est à craindre. On dit parfois simplement que le groupe $E$ est extension de $G$ par $F$.

Pour qu’un groupe E soit extension de G par F, il faut et il suffit qu’il contienne un sous-groupe distingué F’ isomorphe à F, tel que le groupe quotient E/F’ soit isomorphe à G.

Une extension $\mathcal{E}: F \xrightarrow{i} E \xrightarrow{p} G$ est dite centrale si l’image $i(F)$ est contenue dans le centre de E ; ceci n’est possible que si F est commutatif.

Soient $\mathcal{E}: F \xrightarrow{i} E \xrightarrow{p} G$ et $\mathcal{E}': F \xrightarrow{i'} E' \xrightarrow{p'} G$ deux extensions de G par F. On appelle morphisme de $\mathcal{E}$ dans $\mathcal{E}'$ un homomorphisme $u: E \to E'$ tel que $p' \circ u = p$ et $u \circ i = i'$, ou en d’autres termes, tel que le diagramme ci-après soit commutatif:

$$
\begin{array}{ccccc}
& & E \\
& i \searrow & \downarrow u & \swarrow p \\
F & & & & G \\
& i' \nearrow & \downarrow & \searrow p' \\
& & E'
\end{array}
$$

#### Proposition 1 {#alg-i-s6-prop-1 .statement}

*Soient $\mathcal{E}: F \xrightarrow{i} E \xrightarrow{p} G$ et $\mathcal{E}': F \xrightarrow{i'} E' \xrightarrow{p'} G$ des extensions de G par F. Si $u: E \to E'$ est un morphisme de $\mathcal{E}$ dans $\mathcal{E}'$, u est un isomorphisme de E sur $E'$ et $u^{-1}$ est un morphisme de $\mathcal{E}'$ dans $\mathcal{E}$.*

Soit $x \in E$ tel que $u(x) = e$. On a $p(x) = p'(u(x)) = e$ d’où $x \in i(F)$. Soit $y \in F$ tel que $x = i(y)$; on a $i'(y) = u(i(y)) = e$. Comme $i'$ est injectif, $y = e$ et $x = e$. Par suite $u$ est injectif. En vertu de I, p. 38, cor. 1, $u$ est surjectif puisque $u(i(F)) = i'(F)$. La dernière assertion est immédiate.

En d’autres termes, les extensions $\mathcal{E}$ et $\mathcal{E}'$ sont isomorphes si et seulement s’il existe un morphisme de $\mathcal{E}$ dans $\mathcal{E}'$.

Soient F et G deux groupes ; posons $E_0 = F \times G$; soient $i : F \to E_0$ l’injection canonique et $p : E_0 \to G$ la surjection canonique. Toute extension de G par F isomorphe à l’extension $\mathcal{E}_0 : F \xrightarrow{i} E_0 \xrightarrow{p} G$ est appelée extension triviale.

#### Proposition 2 {#alg-i-s6-prop-2 .statement}

*Soit $\mathcal{E}: F \xrightarrow{i} E \xrightarrow{p} G$ une extension de G par F. Les conditions suivantes sont équivalentes :
(i) $\mathcal{E}$ est une extension triviale ;
(ii) $\mathcal{E}$ possède une rétraction r ;
(iii) $\mathcal{E}$ possède une section s telle que $s(G)$ soit contenu dans le centralisateur de $i(F)$.*

Il est clair que (i) entraîne (ii) et (iii). Si (ii) est vérifiée, l’application $(r, p): E \to F \times G$ est un morphisme de $\mathcal{E}$ dans $\mathcal{E}_0$, d’où (i). Si (iii) est vérifiée, l’homomorphisme de $F \times G$ dans E correspondant à $(i, s)$ (I, p. 45, prop. 12) est un morphisme de $\mathcal{E}_0$ dans $\mathcal{E}$, d’où (i).

Il peut arriver qu’une extension $\mathcal{E}: F \to E \to G$ ne soit pas triviale, et que cependant le groupe $E$ soit isomorphe à $F \times G$ (I, p. 135, exerc. 6).

#### Définition 2 {#alg-i-s6-def-2 .statement}

Soient $F$ et $G$ deux groupes, et $\tau$ un homomorphisme de $G$ dans le groupe des automorphismes de $F$. Posons $\tau(g)(f) = ^g f$ pour $g \in G$ et $f \in F$. On appelle produit semi-direct externe de $G$ par $F$ relativement à $\tau$ l’ensemble $F \times G$ muni de la loi de composition

$$
((f, g), (f', g')) \mapsto (f, g) \cdot_{\tau} (f', g') = (f \cdot ^g f', gg').
$$

Le produit semi-direct externe de $G$ par $F$ relativement à $\tau$ se note $F \times_{\tau} G$.

#### Proposition 3 {#alg-i-s6-prop-3 .statement}

Le produit semi-direct externe $F \times_{\tau} G$ est un groupe. Les applications $i : F \to F \times_{\tau} G$ définie par $i(f) = (f, e)$, $p : F \times_{\tau} G \to G$ définie par $p(f, g) = g$, et $s : G \to F \times_{\tau} G$ définie par $s(g) = (e, g)$ sont des homomorphismes de groupes. Le triplet $(F \times_{\tau} G, i, p)$ est une extension de $G$ par $F$ et $s$ est une section de l’extension.

On a:
$$
((f, g) \cdot_{\tau} (f', g')) \cdot_{\tau} (f'', g'') = (f \cdot ^g f', gg') \cdot_{\tau} (f'', g'') = (f \cdot ^g f' \cdot ^{gg'} f'', gg' g'');
$$
$$
(f, g) \cdot_{\tau} ((f', g') \cdot_{\tau} (f'', g'')) = (f, g) \cdot_{\tau} (f' \cdot ^{g'} f'', g' g'') = (f \cdot ^g (f' \cdot ^{g'} f''), gg' g'').
$$
On a $^g (f' \cdot ^{g'} f'') = ^g f' \cdot ^{gg'} f''$, ce qui montre que la loi de composition définie par (1) est associative. L’élément $(e, e)$ est neutre pour cette loi. L’élément $(f, g)$ admet pour inverse $(g^{-1} f^{-1}, g^{-1})$. Donc la loi de composition de $F \times_{\tau} G$ est une loi de groupe. Les autres assertions sont immédiates.

Avec les notations de la prop. 3, on notera $\mathcal{E}_{\tau}$ l’extension $F \xrightarrow{i} F \times_{\tau} G \xrightarrow{p} G$.

Soient $\mathcal{E}' : F \xrightarrow{i'} E' \xrightarrow{p'} G$ une extension de $G$ par $F$ et $s' : G \to E'$ une section de $\mathcal{E}'$. Définissons une loi d’opération $\tau$ de $G$ sur le groupe $F$ par:

$$
i'(\tau(g, f)) = s'(g)i'(f)s'(g)^{-1} = \operatorname{Int}(s'(g))(i'(f)).
$$

#### Proposition 4 {#alg-i-s6-prop-4 .statement}

Avec les notations ci-dessus, il existe un isomorphisme $u$ de $\mathcal{E}_{\tau}$ sur $\mathcal{E}'$ et un seul tel que $u \circ s = s'$.

On a $(f, g) = (f, e) \cdot_{\tau} (e, g) = i(f) \cdot_{\tau} s(g)$. Par suite, si $u$ répond à la question, on a nécessairement $u(f, g) = i'(f) \cdot s'(g)$, d’où l’unicité de $u$. Démontrons l’existence. Posons $u(f, g) = i'(f) \cdot s'(g)$. On a
$$
u(f, g) \cdot u(f', g') = i'(f)s'(g)i'(f')s'(g') = i'(f)(s'(g)i'(f')s'(g)^{-1})s'(g)s'(g')
$$
$$
= i'(f)i'(\tau(g, f')) \cdot s'(g)s'(g') = i'(f \cdot \tau(g, f')) \cdot s'(gg')
$$
$$
= u((f, g) \cdot_{\tau} (f', g')) .
$$
Par suite, $u$ est un homomorphisme de $F \times_{\tau} G$ dans $E'$. On a évidemment $u \circ i = i', p' \circ u = p$ et $u \circ s = s'$.

#### Remarque {#alg-i-s6-n1-rem-1 .statement}

La définition de l’opération $\tau$ par la formule (2) fait intervenir l’extension $\mathcal{E}'$ et la section $s'$. Lorsque $F$ est commutatif, l’opération $\tau$ ne dépend pas de $s'$. En effet, $\operatorname{Int}(s'(g))|i'(F)$ ne dépend alors que de la classe de $s'(g)$ mod. $i'(F)$.

Plus généralement, soit $\mathcal{E} : F \to E \to G$ une extension de $G$ par un groupe commutatif $F$ (on ne suppose pas que $\mathcal{E}$ admette une section). Le groupe $E$ opère sur $F$ par automorphismes intérieurs, et cette opération est triviale sur l’image de F, donc définit une opération de G sur F. Si $\mathcal{E}$ admet une section, cette opération est celle définie par la formule (2).

#### Corollaire {#alg-i-s6-n1-cor-1 .statement}

*Soient G un groupe, H et K deux sous-groupes de G tels que H soit distingué, H ∩ K = {e} et H.K = G. Soit $\tau$ l’opération de K sur H par automorphismes intérieurs de G. L’application $(h, k) \mapsto hk$ est un isomorphisme de $H \times_{\tau} K$ sur G.*

Sous les hypothèses de ce corollaire, on dit que G est *produit semi-direct* de K par H.

*Exemples. —* 1) Soient G un groupe et E un G-ensemble principal homogène. Notons $\Gamma$ le groupe des automorphismes de G. Soit A l’ensemble des permutations $f$ de E possédant la propriété suivante:
Il existe $\gamma \in \Gamma$ tel que $f$ soit un $\gamma$-morphisme de E dans E (autrement dit, $f(gb) = \gamma(g)f(b)$ pour $b \in E$ et $g \in G$).
La formule $f(gb) = \gamma(g)f(b)$ précédente montre que, si $f \in A$, il existe *un seul* $\gamma \in \Gamma$ tel que $f$ soit un $\gamma$-morphisme; nous le noterons $p(f)$.
Soient $f, f'$ dans A, $\gamma = p(f), \gamma' = p(f')$. On a, pour tout $b \in E$ et tout $g \in G$,
$$
(f' \circ f)(gb) = f'(\gamma(g)f(b)) = \gamma'(\gamma(g))f'(f(b))
$$
ce qui prouve que $f' \circ f \in A$ et que $p(f' \circ f) = p(f')p(f)$. D’autre part, on a $f(\gamma^{-1}(g)f^{-1}(b)) = gb$, d’où $f^{-1}(gb) = \gamma^{-1}(g)f^{-1}(b)$ et $f^{-1} \in A$. Ainsi A est un sous-groupe de $\mathfrak{S}_E$ et $p$ est un homomorphisme de A dans $\Gamma$. Le noyau de $p$ est l’ensemble $\mathrm{Aut}_G(E)$ des automorphismes du G-ensemble E.
Fixons $a \in E$. Nous avons défini dans I, p. 59 un isomorphisme $\psi_a$ de $G^0$ sur $\mathrm{Aut}_G(E)$ tel que $\psi_a(x)(ga) = gxa$ quels que soient $g, x$ dans G. D’autre part, pour $\gamma \in \Gamma$, soit $s_a(\gamma)$ la permutation de E définie par $s_a(\gamma)(ga) = \gamma(g)a$ pour tout $g \in G$; on vérifie aussitôt que $s_a$ est un homomorphisme de $\Gamma$ dans A tel que $p \circ s_a = \mathrm{Id}_{\tau}$. Ainsi,
$$
G^0 \xrightarrow{\psi_a} A \xrightarrow{p} \Gamma
$$
est une *extension* de $\Gamma$ par $G^0$ et $s_a$ est une *section* de cette extension. Cette extension et cette section définissent une opération de $\Gamma$ sur $G^0$, $s_a(\Gamma)$ agissant sur $\psi_a(G^0)$ par automorphismes intérieurs; nous noterons exponentiellement cette opération. Montrons que *cette opération est l’opération naturelle* (I, p. 24, *Exemple 3*): en effet, pour $x, g$ dans G et $\gamma \in \Gamma$, on a
$$
(\psi_a(\gamma x))(ga) = (s_a(\gamma) \circ \psi_a(x) \circ s_a(\gamma)^{-1})(ga) =
(s_a(\gamma) \circ \psi_a(x))(\gamma^{-1}(g)a) = s_a(\gamma)(\gamma^{-1}(g)xa) = g\gamma(x)a = \psi_a(\gamma(x))ga
$$
d’où, $\gamma x = \gamma(x)$.
La prop. 4 montre alors que A est isomorphe au produit semi-direct de $\Gamma = \mathrm{Aut}(G)$ par $G^0$ pour l’opération naturelle de $\mathrm{Aut}(G)$ sur $G^0$. On notera que l’isomorphisme que nous avons construit dépend en général du choix de l’élément $a \in E$.
2) \*Soit A un anneau commutatif. Le groupe trigonal supérieur $T(n, A)$ est produit semi-direct du sous-groupe diagonal $D(n, A)$ par le sous-groupe trigonal strict supérieur $T_1(n, A)$.\*

### 2. Commutateurs

#### Définition 3 {#alg-i-s6-def-3 .statement}

*Soient G un groupe, $x$ et $y$ deux éléments de G. On appelle* commutateur *de $x$ et $y$ l’élément $x^{-1}y^{-1}xy$ de G.*

On note $(x, y)$ le commutateur de $x$ et $y$. On a évidemment

$$
(y, x) = (x, y)^{-1}.
$$

Pour que $x$ et $y$ commutent, il faut et il suffit que $(x, y) = e$. Plus généralement, on a

$$
xy = yx(x, y).
$$

Posons d’autre part

(3) $$ x^{y} = y^{-1}xy = x(x, y) = (y, x^{-1})x. $$

Comme l’application $x \mapsto x^{y}$ est l’automorphisme intérieur $\mathrm{Int}(y^{-1})$, on a $(x, y)^{z} = (x^{z}, y^{z})$ quels que soient $x, y, z \in G$.

Démontrons, pour $x, y, z \in G$, les relations suivantes:

(4) $$ (x, yz) = (x, z).(x, y)^{z} = (x, z).(z, (y, x)).(x, y) $$
(4 bis) $$ (xy, z) = (x, z)^{y}.(y, z) = (x, z).((x, z), y).(y, z) $$
(5) $$ (x^{y}, (y, z)).(y^{z}, (z, x)).(z^{x}, (x, y)) = e $$
(6) $$ (x, yz).(z, xy).(y, zx) = e $$
(6 bis) $$ (xy, z).(yz, x).(zx, y) = e. $$

En effet, on a $(x, yz) = x^{-1}z^{-1}y^{-1}xyz = (x, z)z^{-1}x^{-1}y^{-1}xyz = (x, z)(x, y)^{z} = (x, z)(z, (x, y)^{-1})(x, y)$ d’après (3), ce qui démontre (4). La formule (4 bis) se démontre de la même manière. D’autre part, on a

$$
\begin{align*}
(x^{y}, (y, z)) &= (x^{y})^{-1}(z, y)(x^{y})(y, z) \\
&= y^{-1}x^{-1}yz^{-1}y^{-1}zyy^{-1}xyy^{-1}z^{-1}yz \\
&= (yzy^{-1}xy)^{-1}(zxz^{-1}yz).
\end{align*}
$$

Posons alors $u = yzy^{-1}xy, v = zxz^{-1}yz$ et $w = xyx^{-1}zx$; on a

$$(x^{y}, (y, z)) = u^{-1}v.$$

Par permutation circulaire de $x, y, z$, on en déduit $(y^{z}, (z, x)) = v^{-1}w$ et $(z^{x}, (x, y)) = w^{-1}u$, ce qui entraîne aussitôt (5). Enfin, (6) se démontre en multipliant membre à membre les trois formules obtenues en permutant circulairement $x, y, z$ dans la formule $(x, yz) = x^{-1}z^{-1}y^{-1}xyz = (yzx)^{-1}(xyz)$, et de même pour (6 bis).

Si A et B sont deux sous-groupes de G, on note (A, B) le sous-groupe engendré par les commutateurs $(a, b)$ pour $a \in A$ et $b \in B$.\footnote{Nous nous écartons ici de la convention posée dans I, p. 2 pour la notation de l’extension aux parties d’une loi de composition.} On a $(A, B) = \{e\}$ si et seulement si A centralise B. On a $(A, B) \subset A$ si et seulement si B normalise A. Si A et B sont distingués (resp. caractéristiques), il en est de même de (A, B).

#### Proposition 5 {#alg-i-s6-prop-5 .statement}

*Soient A, B, C trois sous-groupes de G.*

(i) *Le sous-groupe A normalise le sous-groupe (A, B).*

(ii) *Si le sous-groupe (B, C) normalise A, le sous-groupe (A, (B, C)) est engendré par les éléments $(a, (b, c))$ pour $a \in A, b \in B$ et $c \in C$.*

(iii) *Si A, B et C sont distingués, on a*

$$(A, (B, C)) \subset (C, (B, A)).(B, (C, A)).$$

D’après (4 bis), on a, pour $a, a'$ dans A et $b \in B$,

$$(a, b)^{a'} = (aa', b).(a', b)^{-1}$$

d’où (i). Supposons maintenant que (B, C) normalise A. Pour $a \in A,\ b \in B,\ c \in C$ et $x \in G$, on a d’après (4)

$$
(a, (b, c).x) = (a, x)\ (x, ((b, c), a))\ (a, (b, c))
$$

et $((b, c), a) \in A$ puisque (B, C) normalise A, d’où par récurrence sur $p$ le fait que $(a, \prod_{i=1}^p (b_i, c_i))$, pour $b_i \in B,\ c_i \in C$, appartient au sous-groupe engendré par les éléments de la forme $(a, (b, c))$. Si enfin A, B et C sont distingués, il en est de même des sous-groupes (A, (B, C)), (C, (B, A)) et (B, (C, A)). Il suffit donc d’après (ii) de montrer que

$$
(a, (b, c)) \in (C, (B, A)).(B, (C, A))
$$

quels que soient $a \in A,\ b \in B$ et $c \in C$. Or on a d’après (5), en posant $a^{b^{-1}} = u$,

$$
(a, (b, c)) = (u^b, (b, c)) = (c^u, (u, b))^{-1}.(b^c, (c, u))^{-1}
$$

d’où (iii).

#### Définition 4 {#alg-i-s6-def-4 .statement}

Soit G un groupe. On appelle groupe dérivé de G le sous-groupe engendré par les commutateurs d’éléments de G.

Le groupe dérivé de G est donc le sous-groupe (G, G). On le note aussi D(G). Par abus de langage, on l’appelle parfois le groupe des commutateurs de G, bien qu’il soit en général distinct de l’ensemble des commutateurs d’éléments de G (I, p. 137, exerc. 16). On a D(G) = {e} si et seulement si G est commutatif.

#### Proposition 6 {#alg-i-s6-prop-6 .statement}

Soit $f : G \to G'$ un homomorphisme de groupes. On a

$$
f(D(G)) \subset D(G').
$$

Si f est surjectif, l’homomorphisme de D(G) dans D(G') restriction de f est surjectif.

L’image par f d’un commutateur d’éléments de G est un commutateur d’éléments de G'. Si f est surjectif, l’image par f de l’ensemble des commutateurs de G est l’ensemble des commutateurs de G'. La proposition résulte donc de I, p. 32, cor. 3.

#### Corollaire 1 {#alg-i-s6-prop-6-cor-1 .statement}

Le groupe dérivé d’un groupe G est un sous-groupe caractéristique de G. En particulier, c’est un sous-groupe distingué de G.

#### Corollaire 2 {#alg-i-s6-prop-6-cor-2 .statement}

Soit G un groupe. Le groupe quotient $G/D(G)$ est commutatif. Soit $\pi : G \to G/D(G)$ l’homomorphisme canonique. Tout homomorphisme f de G dans un groupe commutatif G' se met de façon unique sous la forme $f = \bar{f} \circ \pi$, où $\bar{f} : G/D(G) \to G'$ est un homomorphisme.

On a $\pi(D(G)) = \{e\}$. Comme $\pi$ est surjectif, on en déduit $D(G/D(G)) = \{e\}$, d’où la première assertion. La seconde résulte de I, p. 35, prop. 5.

#### Corollaire 3 {#alg-i-s6-prop-6-cor-3 .statement}

Soit H un sous-groupe de G. Les conditions suivantes sont équivalentes.
(i) $H \supset D(G)$;
(ii) H est un sous-groupe distingué et $G/H$ est commutatif.

On a (ii) ⇒ (i) par le cor. 2 et (i) ⇒ (ii) par I, p. 39, th. 4, tout sous-groupe d’un groupe commutatif étant distingué.

#### Corollaire 4 {#alg-i-s6-prop-6-cor-4 .statement}

Soient G un groupe et X une partie de G qui engendre G. Le groupe D(G) est le sous-groupe distingué de G engendré par les commutateurs d’éléments de X.

Soient H le sous-groupe distingué de G engendré par les commutateurs d’éléments de X et φ : G → G/H l’homomorphisme canonique. L’ensemble φ(X) engendre G/H. Les éléments de φ(X) sont deux à deux permutables, donc H est commutatif (I, p. 32, cor. 2). Donc (cor. 3) H contient D(G). Par ailleurs on a évidemment H ⊂ D(G).

#### Remarque 1 {#alg-i-s6-n2-rem-1 .statement}

Le cor. 2 peut encore s’énoncer en disant que G/D(G), muni de π, est solution du problème d’application universelle pour G, relativement aux groupes commutatifs et aux homomorphismes de G dans les groupes commutatifs.

#### Remarque 2 {#alg-i-s6-n2-rem-2 .statement}

Sous les hypothèses du cor. 4, le sous-groupe engendré par les commutateurs d’éléments de X est contenu dans D(G), mais n’est pas en général égal à D(G) (cf. I, p. 137, exerc. 15c).

#### Exemple 1 {#alg-i-s6-n2-exa-1 .statement}

Si G est un groupe simple non commutatif, on a D(G) = G. Par suite, tout homomorphisme de G dans un groupe commutatif est trivial.

#### Exemple 2 {#alg-i-s6-n2-exa-2 .statement}

Le groupe dérivé du groupe symétrique $\mathfrak{S}_n$ est le groupe alterné $\mathfrak{A}_n$. En effet, $\mathfrak{A}_n$ est engendré par les produits de deux transpositions; si $\tau = \tau_{x,y}$ et $\tau' = \tau_{x',y'}$ sont deux transpositions, soit $\sigma$ une permutation telle que $\sigma(x') = x$ et $\sigma(y') = y$. On a $\tau' = \sigma^{-1} \tau \sigma$ et $\tau \tau' = \tau^{-1} \tau' = \tau^{-1} \sigma^{-1} \tau \sigma$ est un commutateur. Donc $\mathfrak{A}_n \subset D(\mathfrak{S}_n)$. Comme $\mathfrak{S}_n / \mathfrak{A}_n$ est commutatif, on a $\mathfrak{A}_n \supset D(\mathfrak{S}_n)$ (cor. 3).

### 3. Suite centrale descendante, groupes nilpotents

Soient G un groupe, H un sous-groupe de G et K un sous-groupe distingué de G. L’image de H dans G/K est contenue dans le centre de G/K si et seulement si (G, H) ⊂ K.

#### Définition 5 {#alg-i-s6-def-5 .statement}

Soit G un groupe. On appelle suite centrale descendante de G, la suite $(C^n(G))_{n \geq 1}$ de sous-groupes de G définie par récurrence par:

$$
C^1(G) = G, \qquad C^{n+1}(G) = (G, C^n(G)).
$$

Soit $f : G \to G'$ un homomorphisme de groupes. On voit, par récurrence sur n, que $f(C^n(G)) \subset C^n(G')$ et que si f est surjectif $f(C^n(G)) = C^n(G')$. En particulier, pour tout $n \geq 1$, $C^n(G)$ est un sous-groupe caractéristique (donc distingué) de G. Pour tout $n \geq 1$, $C^n(G)/C^{n+1}(G)$ est contenu dans le centre de $G/C^{n+1}(G)$.

Soit $(G_1, G_2, \ldots)$ une suite décroissante de sous-groupes distingués de G tels que 1) $G_1 = G$; 2) pour tout i, $G_i/G_{i+1}$ est contenu dans le centre de $G/G_{i+1}$. Alors $C^i(G) \subset G_i$ comme on le voit par récurrence sur i.

On a:

(7)
$$
(C^m(G), C^n(G)) \subset C^{m+n}(G).
$$

En effet, si nous notons $(F_{m,n})$ cette formule, on déduit de $(F_{m,n})$, compte tenu de I, p. 66, prop. 5, (iii),

$$
(C^m(G), C^{n+1}(G)) \subset (G, (C^m(G), C^n(G))).(C^n(G), (G, C^m(G)))
$$
$$
\subset C^{m+n+1}(G).(C^{m+1}(G), C^n(G)).
$$

Donc $((F_{m,n}) \text{ et } (F_{m+1,n})) \Rightarrow (F_{m,n+1})$. Comme $(F_{m,1})$ et $(F_{1,n})$ sont évidentes, on obtient $(F_{m,n})$ par récurrence.

#### Définition 6 {#alg-i-s6-def-6 .statement}

On dit qu’un groupe $G$ est nilpotent s’il existe un entier $n$ tel que $C^{n+1}(G) = \{e\}$. On appelle classe de nilpotence d’un groupe nilpotent $G$ le plus petit entier $n$ tel que $C^{n+1}(G) = \{e\}$.

Si $n \in \mathbf{N}$, un groupe de classe de nilpotence $n$ est appelé groupe nilpotent de classe $n$. On dit parfois que la classe de nilpotence d’un groupe $G$ est finie si $G$ est nilpotent.

#### Exemple 1 {#alg-i-s6-n3-exa-1 .statement}

Un groupe est nilpotent de classe 0 (resp. $\leq 1$) si et seulement s’il est réduit à l’élément neutre (resp. est commutatif).

#### Exemple 2 {#alg-i-s6-n3-exa-2 .statement}

*Pour tout anneau commutatif $A$ et tout entier $n \geq 1$, le groupe trigonal strict supérieur $T_1(n, A)$ est nilpotent de classe $\leq n - 1$ (et même de classe $n - 1$ si $A \neq \{0\}$).*

#### Exemple 3 {#alg-i-s6-n3-exa-3 .statement}

Soit $G$ un groupe nilpotent de classe $n$. Tout sous-groupe (resp. tout groupe quotient) de $G$ est nilpotent de classe $\leq n$. En effet, si $H$ est un sous-groupe de $G$, on a $C^n(H) \subset C^n(G)$. Si $G'$ est un groupe quotient de $G$ et $\pi : G \to G'$ l’homomorphisme canonique, on a $C^n(G') = \pi(C^n(G))$.

#### Exemple 4 {#alg-i-s6-n3-exa-4 .statement}

Un produit fini de groupes nilpotents est nilpotent.

#### Proposition 7 {#alg-i-s6-prop-7 .statement}

Soient $G$ un groupe et $n$ un entier. Les conditions suivantes sont équivalentes :
a) $G$ est nilpotent de classe $\leq n$.
b) Il existe une suite de sous-groupes de $G$ :

$$
G = G^1 \supset G^2 \supset \ldots \supset G^{n+1} = \{e\}
$$

telle que $(G, G^{k'}) \subset G^{k+1}$ pour tout $k \in \{1, n\}$.
c) Il existe un sous-groupe $A$ de $G$ contenu dans le centre de $G$, tel que $G/A$ soit nilpotent de classe $\leq n - 1$.
a) $\Rightarrow$ b) : il suffit de prendre $G^k = C^k(G)$.
b) $\Rightarrow$ a) : on a, par récurrence sur $k$, $C^k(G) \subset G^k$.
a) $\Rightarrow$ c) : il suffit de prendre $A = C^n(G)$.
c) $\Rightarrow$ a) : soit $\pi : G \to G/A$ l’homomorphisme canonique ; on a $\pi(C^n(G)) = C^n(G/A) = \{e\}$, donc $C^n(G) \subset A$, d’où $C^{n+1}(G) = \{e\}$.

En termes plus brefs : un groupe est nilpotent de classe $\leq n$ s’il s’obtient par $n$ extensions centrales successives à partir du groupe $\{e\}$.

#### Corollaire {#alg-i-s6-n3-cor-1 .statement}

Une extension centrale d’un groupe nilpotent (par un groupe nécessairement commutatif) est nilpotent.

#### Proposition 8 {#alg-i-s6-prop-8 .statement}

Soit G un groupe nilpotent de classe $\leq n$, et soit H un sous-groupe de G. Il existe une suite de sous-groupes
$$
G = H^1 \supset H^2 \supset \ldots \supset H^{n+1} = H,
$$
telle que $H^{k+1}$ soit distingué dans $H^k$ et $H^k/H^{k+1}$ commutatif pour tout $k \leq n$.

On choisit une suite $(G^k)$ de sous-groupes de G vérifiant les conditions de la prop. 7 b) (I, p. 69); pour tout $k$, $G^k$ est distingué dans G. On pose:
$$
H^k = H.G^k.
$$
Il faut voir que $H^{k+1}$ est normalisé par $H^k = H.G^k$; comme il l’est par H, il suffit de voir qu’il l’est par $G^k$. Or, si $s \in G^k$ et $h \in H$, on a
$$
shs^{-1} = shs^{-1}h^{-1}.h \in (G, G^k).H
$$
et $(G, G^k).H$ est contenu dans $G^{k+1}.H = H^{k+1}$; d’où $s.H^{k+1}.s^{-1} = H^{k+1}$, ce qui montre bien que $H^{k+1}$ est distingué dans $H^k$.

Enfin, l’homomorphisme canonique $G^k/G^{k+1} \to H^k/H^{k+1}$ est évidemment surjectif; comme le premier groupe est commutatif, le second l’est aussi.

#### Corollaire 1 {#alg-i-s6-prop-8-cor-1 .statement}

Soient G un groupe nilpotent et H un sous-groupe de G. Si H est distinct de G, le normalisateur $N_G(H)$ de H dans G est distinct de H.

Soit k le plus grand indice tel que $H^k \neq H$. Le groupe $H^k$ normalise H, et est distinct de H.

#### Corollaire 2 {#alg-i-s6-prop-8-cor-2 .statement}

Soient G un groupe nilpotent et H un sous-groupe de G. Si H est distinct de G, il existe un sous-groupe distingué N de G, contenant H, distinct de G, et tel que $G/N$ soit commutatif.

Soit k le plus petit indice tel que $H^k \neq G$. Le groupe $H^k$ répond à la question.

#### Corollaire 3 {#alg-i-s6-prop-8-cor-3 .statement}

Soient G un groupe nilpotent et H un sous-groupe de G. Si $G = H.(G, G)$, on a $G = H$.

En effet, tout sous-groupe N de G qui contient H et tel que G/N soit commutatif contient H.(G, G). Le cor. 3 résulte donc du cor. 2.

Le cor. 3 peut encore se formuler ainsi: soit X une partie de G. Pour que X engendre G, il faut et il suffit que l’image de X dans G/D(G) engendre G/D(G).

#### Corollaire 4 {#alg-i-s6-prop-8-cor-4 .statement}

Soit $f : G' \to G$ un homomorphisme de groupes. Supposons que:
a) G est nilpotent.
b) L’homomorphisme $f_1 : G'/(G', G') \to G/(G, G)$, déduit de f par passage au quotient, est surjectif.
Alors f est surjectif.
Cela résulte du cor. 3 appliqué au sous-groupe $H = f(G')$.

#### Proposition 9 {#alg-i-s6-prop-9 .statement}

Soit G un groupe nilpotent de classe $\leq n$, et soit N un sous-groupe distingué de G. Il existe une suite de sous-groupes
$$
N = N^1 \supset N^2 \supset \ldots \supset N^{n+1} = \{e\}
$$
telle que $(G, N^k) \subset N^{k+1}$ pour $k = 1, \ldots, n$.

Si $(G^{lc})$ vérifie la condition b) de la prop. 7 (I, p. 69), on prend
$$
N^{lc} = G^{lc} \cap N.
$$

#### Corollaire 1 {#alg-i-s6-prop-9-cor-1 .statement}

*Soient $G$ un groupe nilpotent, $Z$ le centre de $G$, et $N$ un sous-groupe distingué de $G$. Si $N \neq \{e\}$, on a $N \cap Z \neq \{e\}$.

Soit $k$ le plus grand indice tel que $N^{lc} \neq \{e\}$. Le groupe $N^{lc}$ est contenu dans $N$. D’autre part, $(G, N^{lc}) \subset N^{lc+1} = \{e\}$; donc $N^{lc}$ est contenu dans le centre $Z$ de $G$.

#### Corollaire 2 {#alg-i-s6-prop-9-cor-2 .statement}

*Soit $f$ un homomorphisme d’un groupe nilpotent $G$ dans un groupe $G'$. Si la restriction de $f$ au centre de $G$ est injective, $f$ est injectif.

C’est le cor. 1 appliqué à $\mathrm{Ker}(f)$.

### 4. Suite dérivée, groupes résolubles

#### Définition 7 {#alg-i-s6-def-7 .statement}

*Soit $G$ un groupe. On appelle suite dérivée de $G$ la suite $(D^n(G))_{n \in \mathbf{N}}$ définie par récurrence par:
$$
D^0(G) = G; \quad D^{n+1}(G) = D(D^n(G)) \quad \text{pour } n \in \mathbf{N}.
$$
On a $D^0(G) = C^1(G) = G,\ D^1(G) = C^2(G) = D(G) = (G, G)$. Pour tout $n \in \mathbf{N}$, on a $D^n(G) \subset C^{2^n}(G)$, comme on le voit par récurrence sur $n$ en utilisant la formule (7) de I, p. 68.

Soit $f : G \to G'$ un homomorphisme de groupes. On voit, par récurrence sur $n$, que $f(D^n(G)) \subset D^n(G')$, et que si $f$ est surjectif, $f(D^n(G)) = D^n(G')$. En particulier, pour tout $n \in \mathbf{N}$, $D^n(G)$ est un sous-groupe caractéristique (donc distingué) de $G$. Pour tout $n \in \mathbf{N}$, le groupe $D^n(G)/D^{n+1}(G)$ est un sous-groupe distingué commutatif (mais en général non central) de $G/D^{n+1}(G)$.

Soit $(G_0, G_1, \ldots)$ une suite décroissante de sous-groupes de $G$ tels que: 1) $G_0 = G$; 2) pour tout $i$, $G_{i+1}$ est distingué dans $G_i$ et $G_i/G_{i+1}$ est commutatif. Alors $D^i(G) \subset G_i$ pour tout $i$, comme on le voit par récurrence sur $i$.

#### Définition 8 {#alg-i-s6-def-8 .statement}

*On dit qu’un groupe $G$ est résoluble s’il existe un entier $n$ tel que $D^n(G) = \{e\}$. Si $G$ est un groupe résoluble, le plus petit entier $n$ tel que $D^n(G) = \{e\}$ est appelé la classe de résolvabilité de $G$.

Un groupe résoluble de classe de résolvabilité $n$ est appelé un groupe résoluble de classe $n$. On dit parfois qu’un groupe est de classe de résolvabilité finie s’il est résoluble.

#### Exemple 1 {#alg-i-s6-n4-exa-1 .statement}

Un groupe est résoluble de classe 0 (resp. $\leq 1$) si et seulement s’il est réduit à $e$ (resp. est commutatif).

#### Exemple 2 {#alg-i-s6-n4-exa-2 .statement}

Tout groupe nilpotent de classe $\leq 2^n - 1$ est résoluble de classe $\leq n$; cela résulte de la formule $D^n(G) \subset C^{2^n}(G)$ démontrée plus haut.

#### Exemple 3 {#alg-i-s6-n4-exa-3 .statement}

Soit $G$ un groupe résoluble de classe $\leq n$. Tout sous-groupe (resp. groupe quotient) de $G$ est résoluble de classe $\leq n$ (démonstration analogue à celle de I, p. 69, *Exemple 3*).

#### Exemple 4 {#alg-i-s6-n4-exa-4 .statement}

Si G est un groupe résoluble de classe $p$ et F un groupe résoluble de classe $q$, toute extension E de G par F est un groupe résoluble de classe $\leq p + q$. En effet, soit $\pi : E \to G$ la projection; on a $\pi(D^p(E)) \subset D^p(G) = \{e\}$ et par suite $D^p(E) \subset F$; on en déduit que $D^{p+q}(E) = D^q(D^p(E)) \subset D^q(F) = \{e\}$.

#### Exemple 5 {#alg-i-s6-n4-exa-5 .statement}

Le groupe symétrique $S_n$ est résoluble si et seulement si $n < 5$ (cf. I, p. 130, exerc. 10 et p. 131, exerc. 16).

#### Exemple 6 {#alg-i-s6-n4-exa-6 .statement}

*Si A est un anneau commutatif, le groupe trigonal supérieur $T(n, A)$ est résoluble mais non nilpotent en général.*

#### Proposition 10 {#alg-i-s6-prop-10 .statement}

*Soit G un groupe et soit n un entier. Les conditions suivantes sont équivalentes*:

(i) *G est résoluble de classe $\leq n$*.

(ii) *Il existe une suite de sous-groupes distingués de G*
$$
G = G^0 \supset G^1 \supset \ldots \supset G^n = \{e\}
$$
*telle que les groupes $G^k / G^{k+1}$ soient commutatifs*.

(iii) *Il existe une suite de sous-groupes de G*
$$
G = G^0 \supset G^1 \supset \ldots \supset G^n = \{e\}
$$
*telle que, pour tout k, $G^{k+1}$ soit un sous-groupe distingué de $G^k$, et que $G^k / G^{k+1}$ soit commutatif*.

(iv) *Il existe un sous-groupe commutatif distingué A de G tel que $G/A$ soit résoluble de classe $\leq n - 1$*.

On a (i) $\Rightarrow$ (ii): il suffit de prendre $G^k$ égal à $D^k(G)$. On a trivialement (ii) $\Rightarrow$ (iii). On a (iii) $\Rightarrow$ (i) car $D^k(G)$ est nécessairement contenu dans $G^k$. L’équivalence de (ii) et (iv) est immédiate par récurrence sur $n$.

En termes plus brefs: un groupe est résoluble de classe $\leq n$ s’il s’obtient par extensions successives de $n$ groupes commutatifs.

#### Corollaire {#alg-i-s6-n4-cor-1 .statement}

*Soient G un groupe fini et*
$$
G = G^0 \supset G^1 \supset \ldots \supset G^n = \{e\}
$$
*une suite de Jordan-Hölder de G. Pour que G soit résoluble, il faut et il suffit que les quotients $G^k / G^{k+1}$ soient cycliques d’ordre premier*.

En effet, si les quotients d’une suite de composition de G sont cycliques, donc commutatifs, G est résoluble d’après la prop. 10. Réciproquement, si G est résoluble, le groupe $G^k / G^{k+1}$ est, pour tout $k$, résoluble et simple (I, p. 41, prop. 9). Or, tout groupe simple résoluble H est cyclique d’ordre premier. En effet, $D(H)$ est un sous-groupe distingué de H; on ne peut avoir $D(H) = H$ car on aurait alors $D^k(H) = H$ pour tout $k$; on a donc $D(H) = \{e\}$, et H est commutatif. Le corollaire résulte alors de I, p. 48, corollaire de la prop. 20.

### 5. $p$-groupes

Dans ce numéro et le suivant, la lettre $p$ désigne un nombre premier (I, p. 48, déf. 16).

#### Définition 9 {#alg-i-s6-def-9 .statement}

*On appelle p-groupe un groupe fini dont l’ordre est une puissance de p.*

Soient G un $p$-groupe, $p^r$ son ordre. Tout diviseur de $p^r$ est une puissance de $p$ (I, p. 49, corollaire). Par suite, tout sous-groupe ou tout groupe quotient de G est un $p$-groupe (I, p. 34, corollaire); le cardinal de tout espace homogène sous G est une puissance de $p$ (I, p. 57, th. 1).

Une extension d’un $p$-groupe par un $p$-groupe est un $p$-groupe.

*Exemples. — 1) Un $p$-groupe commutatif est isomorphe à un produit de groupes cycliques $\mathbf{Z}/p^n\mathbf{Z}$ (cf. I, p. 138, exerc. 19, ainsi que VII, § 4, n° 7, prop. 7).
   2) Soit $k$ un corps fini de caractéristique $p$. Le groupe trigonal strict $T_1(n, k)$ est un $p$-groupe.
   3) Le groupe quaternionien $\{ \pm 1, \pm i, \pm j, \pm k \}$ est un 2-groupe (cf. I, p. 134, exerc. 4).*

#### Proposition 11 {#alg-i-s6-prop-11 .statement}

Soient E un ensemble fini et G un $p$-groupe opérant sur E. Notons $E^G$ l’ensemble des $x \in E$ tels que $gx = x$ pour tout $g \in G$ (points fixes). On a
$$
\operatorname{Card}(E^G) \equiv \operatorname{Card}(E) \pmod{p}.
$$
En effet, $E - E^G$ est réunion disjointe d’orbites non réduites à un point. Le cardinal d’une telle orbite est une puissance de $p$ différente de $p^0 = 1$, donc est un multiple de $p$.

#### Corollaire {#alg-i-s6-n5-cor-1 .statement}

Soit G un $p$-groupe. Si G n’est pas réduit à e, son centre n’est pas réduit à e.

Faisons opérer G sur lui-même par automorphismes intérieurs. L’ensemble des points fixes est le centre Z de G. D’après la prop. 11, on a
$$
\operatorname{Card}(Z) \equiv \operatorname{Card}(G) \equiv 0 \pmod{p},
$$
d’où $\operatorname{Card}(Z) \neq 1$ et $Z \neq \{e\}$.

#### Théorème 1 {#alg-i-s6-thm-1 .statement}

Soient G un $p$-groupe, $p^r$ son ordre. Il existe une suite de sous-groupes de G
$$
G = G^1 \supset G^2 \supset \ldots \supset G^{r+1} = \{e\},
$$
telle que $(G, G^k) \subset G^{k+1}$, pour $1 \leq k \leq r$, et que $G^k/G^{k+1}$, pour $1 \leq k \leq r$, soit cyclique d’ordre $p$.

Le théorème est vrai pour $G = \{e\}$. Démontrons-le par récurrence sur $\operatorname{Card}(G)$. Soient Z le centre de G, $x \neq e$ un élément de Z (cor. de la prop. 11) et $p^s$, avec $s \neq 0$, l’ordre de $x$. Alors $x^{p^{s-1}}$ est un élément d’ordre $p$ et par suite Z contient un sous-groupe $G^r$ cyclique d’ordre $p$. Par l’hypothèse de récurrence, le groupe $G' = G/G^r$ possède une suite de sous-groupes $({G'}^k)_{1 \leq k \leq r}$ ayant les propriétés demandées. Soit $\pi : G \to G'$ l’homomorphisme canonique. La suite de sous-groupes de G définie par $G^k = \pi^{-1}({G'}^k)$ pour $1 \leq k \leq r$, $G^{r+1} = \{e\}$, répond à la question, car $G^k/G^{k+1}$ est isomorphe à ${G'}^k/{G'}^{k+1}$ pour $1 \leq k < r$ (I, p. 39, th. 4).

#### Corollaire {#alg-i-s6-n5-cor-2 .statement}

Tout $p$-groupe est nilpotent.

Ceci résulte de I, p. 69, prop. 7.

#### Proposition 12 {#alg-i-s6-prop-12 .statement}

Soit G un $p$-groupe et soit H un sous-groupe de G distinct de G. Alors:
a) Le normalisateur $N_G(H)$ de H dans G est distinct de G.
b) Il existe un sous-groupe distingué N de G, d’indice $p$ dans G, qui contient H.

L’assertion a) résulte de I, p. 70, cor. 1. Démontrons b). D’après I, p. 70, cor. 2, il existe un sous-groupe distingué N’ de G contenant H, distinct de G et tel que G/N’ soit commutatif. Soit N un sous-groupe distinct de G contenant N’ et maximal. Alors N est distingué (I, p. 67, cor. 3) et G/N est un $p$-groupe commutatif simple, donc cyclique d’ordre $p$ (I, p. 48, corollaire).

#### Corollaire {#alg-i-s6-n5-cor-3 .statement}

*Soit G un $p$-groupe. Tout sous-groupe d’indice $p$ de G est distingué.*

### 6. Sous-groupes de Sylow

#### Définition 10 {#alg-i-s6-def-10 .statement}

*Soit G un groupe fini. On appelle $p$-sous-groupe de Sylow de G tout sous-groupe P de G vérifiant les deux conditions suivantes:
a) P est un $p$-groupe;
b) $(G : P)$ n’est pas un multiple de $p$.

Si l’on écrit l’ordre de G sous la forme $p^r m$, où $m$ n’est pas un multiple de $p$, les conditions a) et b) sont équivalentes à $\mathrm{Card}(P) = p^r$.

*Exemples. — 1) Dans le groupe $\mathfrak{S}_p$, soit $\zeta$ un cycle d’ordre $p$. Le sous-groupe engendré par $\zeta$ est un $p$-sous-groupe de Sylow de $\mathfrak{S}_p$ car $p$ ne divise pas $(p - 1)!$.
2) *Soit k un corps fini de caractéristique $p$, et soit n un entier positif. Le groupe trigonal strict $T_1(n, k)$ est un $p$-sous-groupe de Sylow du groupe $\mathbf{GL}(n, k)$.*

#### Théorème 2 {#alg-i-s6-thm-2 .statement}

*Tout groupe fini contient un $p$-sous-groupe de Sylow.*

La démonstration s’appuie sur le lemme suivant.

#### Lemme {#alg-i-s6-n6-lem-1 .statement}

*Soit $n = p^r m$ où $m$ est un entier non multiple de $p$. On a*
$$
\binom{n}{p^r} \not\equiv 0 \pmod{p}.
$$

Soient S un groupe d’ordre $p^r$ (par exemple $\mathbf{Z}/p^r \mathbf{Z}$) et T un ensemble à $m$ éléments. Posons X = S × T et soit E l’ensemble des parties de X ayant $p^r$ éléments. On a $\mathrm{Card}(X) = n$ d’où $\mathrm{Card}(E) = \binom{n}{p^r}$ (E, III, p. 42, cor. 1).

Faisons opérer S sur X par $s.(x, y) = (sx, y)$ ($s, x$ dans S, $y \in T$), et considérons l’extension canonique de cette opération à E. Avec les notations de I, p. 73, prop. 11, l’ensemble $E^S$ est l’ensemble des orbites de X, c’est-à-dire l’ensemble des parties Y ⊂ X de la forme S × {t}, $t \in T$, d’où $\mathrm{Card}(E^S) = m$. D’après I, p. 73, prop. 11, on a
$$
\binom{n}{p^r} = \mathrm{Card}(E) \equiv \mathrm{Card}(E^S) = m \not\equiv 0 \pmod{p},
$$
ce qui démontre le lemme.

Démontrons maintenant le théorème. Soit G un groupe fini, $n$ son ordre;

écrivons $n = p^r m$ où $m$ n’est pas multiple de $p$. Soit $E$ l’ensemble des parties à $p^r$ éléments de $G$. On a
$$
\operatorname{Card}(E) = \binom{n}{p^r};
$$
d’où, en vertu du lemme, $\operatorname{Card}(E) \not\equiv 0 \pmod{p}$. Considérons l’extension à $E$ de l’opération de $G$ sur lui-même par translations à gauche. Il existe $X \in E$ dont l’orbite a un cardinal non nul mod. $p$. Si $H_X$ désigne le stabilisateur de $X$, on a donc $(G : H_X) \not\equiv 0$ mod. $p$, ce qui signifie que $p^r$ divise $\operatorname{Card}(H_X)$. Mais $H_X$ est formé des $s \in G$ tels que $sX = X$; si $x \in X$, on a donc $H_X \subset X.x^{-1}$, d’où $\operatorname{Card}(H_X) \leq \operatorname{Card}(X) = p^r$. On a donc $\operatorname{Card}(H_X) = p^r$.

#### Corollaire {#alg-i-s6-n6-cor-1 .statement}

*Si l’ordre de $G$ est divisible par $p$, le groupe $G$ contient un élément d’ordre $p$.*

Grâce au th. 2, on se ramène au cas où $G$ est un $p$-groupe $\neq \{e\}$; si $x \in G$ est différent de $e$, le groupe cyclique engendré par $x$ est alors d’ordre $p^n$ avec $n \geq 1$ et il contient donc un sous-groupe d’ordre $p$.

#### Remarque {#alg-i-s6-n6-rem-1 .statement}

Pour tout nombre premier $q$ divisant $\operatorname{Card}(G)$, soit $P_q$ un $q$-sous-groupe de Sylow de $G$. Alors le sous-groupe $H$ de $G$ engendré par les $P_q$ est d’ordre multiple de $\operatorname{Card}(P_q)$ pour chaque $q$ et d’ordre divisant $\operatorname{Card}(G)$, donc est égal à $G$.

#### Théorème 3 {#alg-i-s6-thm-3 .statement}

*Soit $G$ un groupe fini.*

a) *Les $p$-sous-groupes de Sylow de $G$ sont conjugués entre eux. Leur nombre est congru à 1 mod. $p$.*

b) *Tout sous-groupe de $G$ qui est un $p$-groupe est contenu dans un $p$-sous-groupe de Sylow.*

Soit $P$ un $p$-sous-groupe de Sylow de $G$ (I, p. 74, th. 2), et soit $H$ un $p$-sous-groupe de $G$. Soit $E = G/P$, et considérons l’opération de $H$ sur $G/P$. Comme $\operatorname{Card}(E) \not\equiv 0$ mod. $p$, la prop. 11 de I, p. 73, montre qu’il existe $x \in G/P$ tel que $hx = x$ pour tout $h \in H$. Si $g$ est un représentant de $x$ dans $G$, cela signifie que $H \subset gPg^{-1}$, d’où l’assertion b).

Si $H$ est un $p$-sous-groupe de Sylow, on a $\operatorname{Card}(H) = \operatorname{Card}(P) = \operatorname{Card}(gPg^{-1})$, d’où $H = gPg^{-1}$, ce qui prouve la première assertion de a).

Démontrons la seconde assertion de a). Soit $\mathcal{S}$ l’ensemble des $p$-sous-groupes de Sylow de $G$, et faisons opérer $P$ sur $\mathcal{S}$ par automorphismes intérieurs. L’élément $P \in \mathcal{S}$ est point fixe pour cette opération; montrons que c’est le seul. Soit $Q \in \mathcal{S}$ un point fixe; $Q$ est un sous-groupe de Sylow de $G$ normalisé par $P$, donc $P$ est contenu dans le normalisateur $N$ de $Q$. Les groupes $P$ et $Q$ sont des $p$-sous-groupes de Sylow de $N$; il existe donc $n \in N$ tel que $P = nQn^{-1} = Q$. D’après I, p. 73, prop. 11, on a $\operatorname{Card}(\mathcal{S}) \equiv \operatorname{Card}(\mathcal{S}^P) = 1$ (mod. $p$).

#### Corollaire 1 {#alg-i-s6-thm-3-cor-1 .statement}

*Soit $P$ un $p$-sous-groupe de Sylow de $G$, soit $N$ son normalisateur dans $G$, et soit $M$ un sous-groupe de $G$ contenant $N$. Le normalisateur de $M$ dans $G$ est égal à $M$.*

Soit $s \in G$ tel que $sMs^{-1} = M$. Le sous-groupe $sPs^{-1}$ de $M$ est un $p$-sous-groupe de Sylow de $M$. Il existe donc $t \in M$ tel que $sPs^{-1} = tPt^{-1}$; on a alors $t^{-1}s \in N$, d’où $s \in tN \subset M$.

#### Corollaire 2 {#alg-i-s6-thm-3-cor-2 .statement}

*Soit $f : G_1 \to G_2$ un homomorphisme de groupes finis. Pour tout $p$-sous-groupe de Sylow $P_1$ de $G_1$, il existe un $p$-sous-groupe de Sylow $P_2$ de $G_2$ tel que $f(P_1) \subset P_2$.*

Cela résulte du th. 3, b), appliqué au sous-groupe $f(P_1)$ de $G_2$.

#### Corollaire 3 {#alg-i-s6-thm-3-cor-3 .statement}

a) *Soit $H$ un sous-groupe de $G$. Pour tout $p$-sous-groupe de Sylow $P$ de $H$, il existe un $p$-sous-groupe de Sylow $Q$ de $G$ tel que $P = Q \cap H$.*
b) *Réciproquement, si $Q$ est un $p$-sous-groupe de Sylow de $G$, et si $H$ est distingué dans $G$, le groupe $Q \cap H$ est un $p$-sous-groupe de Sylow de $H$.*
a) Le $p$-groupe $P$ est contenu dans un $p$-sous-groupe de Sylow $Q$ de $G$, et $Q \cap H$ est un $p$-sous-groupe de $H$ contenant $P$, donc égal à $P$.
b) Soit $P'$ un $p$-sous-groupe de Sylow de $H$. Il existe un élément $g \in G$ tel que $gP'g^{-1} \subset Q$. Comme $H$ est distingué, $P = gP'g^{-1}$ est contenu dans $H$, donc dans $Q \cap H$. Comme $Q \cap H$ est un $p$-sous-groupe de $H$ et $P$ un $p$-sous-groupe de Sylow de $H$, on a $P = Q \cap H$.

#### Corollaire 4 {#alg-i-s6-thm-3-cor-4 .statement}

*Soit $N$ un sous-groupe distingué de $G$. L’image dans $G/N$ d’un $p$-sous-groupe de Sylow de $G$ est un $p$-sous-groupe de Sylow de $G/N$, et tout $p$-sous-groupe de Sylow de $G/N$ s’obtient de cette façon.*

Soient $G' = G/N$ et $P'$ l’image dans $G'$ d’un $p$-sous-groupe de Sylow $P$ de $G$. Le groupe $G$ opère transitivement sur $G'/P'$, donc $G'/P'$ est équipotent à $G/S$, où $S$ est un sous-groupe de $G$ contenant $P$. Par suite $(G': P')$ divise $(G: P)$, donc n’est pas multiple de $p$, et le $p$-groupe $P'$ est un $p$-sous-groupe de Sylow de $G'$. Soit $Q'$ un autre $p$-sous-groupe de Sylow de $G'$; on a $Q' = g'P{g'}^{-1}$ pour un $g' \in G'$; si $g \in G$ est un représentant de $g'$, le groupe $Q'$ est l’image de $Q = gPg^{-1}$.

### 7. Groupes nilpotents finis

#### Théorème 4 {#alg-i-s6-thm-4 .statement}

*Soit $G$ un groupe fini. Les conditions suivantes sont équivalentes :*
a) $G$ est nilpotent.
b) $G$ est un produit de $p$-groupes.
c) *Pour tout nombre premier $p$, il existe un $p$-sous-groupe de Sylow de $G$ distingué.*
On a b) $\Rightarrow$ a) (I, p. 73, cor. du th. 1).
Supposons a) vérifiée, et soit $P$ un $p$-sous-groupe de Sylow de $G$. Si $N$ est le normalisateur de $P$ dans $G$, le cor. 1 de I, p. 75 montre que $N$ est son propre normalisateur. D’après le cor. 1 de I, p. 70, cela montre que $N = G$. Donc a) $\Rightarrow$ c).
Supposons c) vérifiée, et soit $I$ l’ensemble des nombres premiers divisant $\mathrm{Card}(G)$. Pour tout $p \in I$, soit $P_p$ un $p$-sous-groupe de Sylow de $G$ distingué dans

G. Pour tout $p \neq q$, $P_p \cap P_q$ est réduit à $e$, car c’est à la fois un $p$-groupe et un $q$-groupe, donc $P_p$ et $P_q$ se centralisent mutuellement (I, p. 46, prop. 15). Soit $\varphi$ l’homomorphisme canonique (I, p. 45, prop. 12) de $\prod_{p \in I} P_p$ dans G. L’homomorphisme $\varphi$ est surjectif d’après la Remarque de I, p. 75. Comme Card $(\prod_{p \in I} P_p) = \mathrm{Card}(G)$, il en résulte que $\varphi$ est bijectif.

#### Remarque 1 {#alg-i-s6-n7-rem-1 .statement}

Soit G un groupe fini et soit $p$ un nombre premier. D’après I, p. 75, th. 3, a), et I, p. 74, th. 2, les conditions suivantes sont équivalentes:
(i) il existe un $p$-sous-groupe de Sylow de G distingué;
(ii) tout $p$-sous-groupe de Sylow de G est distingué;
(iii) il existe un seul $p$-sous-groupe de Sylow de G.

#### Remarque 2 {#alg-i-s6-n7-rem-2 .statement}

Soit G un groupe fini nilpotent. Soit I l’ensemble des diviseurs premiers de Card G. D’après le th. 4 et la Remarque 1, on a $G = \prod_{p \in I} G_p$, où $G_p$ est l’unique $p$-groupe de Sylow de G.

#### Remarque 3 {#alg-i-s6-n7-rem-3 .statement}

Appliqué aux groupes commutatifs, le th. 4 donne la décomposition en produit de composantes primaires des groupes finis commutatifs, qui sera étudiée d’un autre point de vue au chap. VII.

#### Exemple {#alg-i-s6-n7-exa-1 .statement}

Le groupe $\mathfrak{S}_3$ est d’ordre 6. Il contient un 3-sous-groupe de Sylow distingué d’ordre 3 : le groupe $A_3$. Il contient trois 2-sous-groupes de Sylow d’ordre 2 : les groupes $\{e, \tau\}$, où $\tau$ est une transposition. Le groupe $\mathfrak{S}_3$ n’est donc pas nilpotent.

## EXERCICES {#alg-i-s6-exercises}

See the [exercises for § 6](exercises/s6/).
