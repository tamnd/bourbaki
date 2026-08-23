---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Algèbres de Lie
section: 3
section_title: Représentations
lang: fr
source: lie-i-fr
pdf_pages: 0036-0052, 0111-0116
extraction: ocr
subsections:
    - "no": 1
      title: Représentations
      page: 0
      pdf_page: 36
    - "no": 2
      title: Produit tensoriel de représentations
      page: 0
      pdf_page: 40
    - "no": 3
      title: Représentations dans des modules d’homomorphismes
      page: 0
      pdf_page: 41
    - "no": 4
      title: Exemples
      page: 0
      pdf_page: 44
    - "no": 5
      title: Éléments invariants
      page: 0
      pdf_page: 45
    - "no": 6
      title: Formes bilinéaires invariantes
      page: 0
      pdf_page: 47
    - "no": 7
      title: Élément de Casimir
      page: 0
      pdf_page: 49
    - "no": 8
      title: '*Extension de l’anneau de base*'
      page: 0
      pdf_page: 50
statements: 23
exercises: 12
content_sha256: 4a2bc3686ddeac9ac51ff5d229aad35352c08baf68da65d756656f944f20a49c
---

## § 3. Représentations

### 1. Représentations

#### Définition 1 {#lie-i-s3-def-1 .statement}

Soient g une algèbre de Lie sur K, et M un K-module. Un homomorphisme de g dans l’algèbre de Lie gl(M) s’appelle une représentation de g dans le module M. Une représentation injective est dite fidèle. Si K est un corps, la dimension (finie ou infinie) de M sur K s’appelle la dimension de la représentation. La représentation $ x \mapsto \mathrm{ad}\, x $ de g dans le K-module g s’appelle la représentation adjointe de g.

Une représentation de g dans M est donc une application K-linéaire $ \rho $ de g dans le module des endomorphismes de M telle que
$$
\rho([x, y]) \cdot m = \rho(x)\rho(y) \cdot m - \rho(y)\rho(x) \cdot m
$$
quels que soient $ x \in g, y \in g, m \in M $.

*Exemple. — Soient G un groupe de Lie réel, g son algèbre de Lie, θ une représentation analytique de G dans un espace vectoriel réel E de dimension finie. Alors l’homomorphisme correspondant de g dans gl(E) est une représentation de g dans E.*

Soit U l’algèbre enveloppante de g. La proposition 1 du § 2, no 1 définit une correspondance biunivoque entre l’ensemble des représentations de g dans M et l’ensemble des représentations de U dans M. On sait d’autre part (Alg., chap. VIII, § 13, no 1) qu’il y a équivalence entre la notion de représentation de l’algèbre associative U et celle de U-module à gauche.

#### Définition 2 {#lie-i-s3-def-2 .statement}

Soient g une algèbre de Lie sur K, et U son algèbre enveloppante. Un module unitaire à gauche sur U est appelé un g-module à gauche, ou simplement un g-module.

Si M est un g-module, et si x ∈ U, on notera $ x_M $ l’homothétie de M définie par x (cf. Alg., chap. VIII, § 1, no 2).

Un module unitaire à droite sur U s’appelle un g-module à droite. Un tel module s’identifie à un U⁰-module à gauche, c’est-à-dire (§ 2, no 4) à un g⁰-module à gauche.

Soit φ l’antiautomorphisme principal de U. Si M est un g-module à droite, on définit sur M une structure de g-module à gauche en posant $ a.m = m.\varphi(a) $ pour $ m \in M $ et $ a \in U $.

On peut traduire en langage de représentations les notions et résultats de la théorie des modules :

1) Deux représentations ρ et ρ’ de g dans M et M’ sont dites semblables ou isomorphes si les g-modules M et M’ sont isomorphes. Pour cela, il faut et il suffit qu’il existe un isomorphisme u du K-module M sur le K-module M’ tel que :

$$
\rho'(x) = u \circ \rho(x) \circ u^{-1}
$$

quel que soit $ x \in g $.

2) Pour tout $ i \in I $, soit $ \rho_i $ une représentation de g dans $ M_i $. Soit M le g-module somme directe des g-modules $ M_i $. Il lui correspond une représentation $ \rho $ de g dans M, appelée somme directe des ρ_i et notée $ \sum_{i \in I} \rho_i $ (où $ \rho_1 + \cdots + \rho_n $ dans le cas de $ n $ représentations $ \rho_1, \ldots, \rho_n $). Si $ m = (m_i)_{i \in I} $ est un élément de M, et si $ x \in g $, on a $ \rho(x).m = (\rho_i(x).m_i)_{i \in I} $.

3) Une représentation $ \rho $ de g dans M est dite simple ou irréductible si le g-module associé est simple. Il revient au même de dire qu’il n’existe pas de sous-K-module de M (autre que $ \{0\} $ et M) stable pour tous les $ \rho(x), x \in g $. Une classe de g-modules simples (Alg., chap. VIII, § 3, no 2) définit une classe de représentations simples de g.

4) Une représentation $ \rho $ de g dans M est dite semi-simple ou complètement réductible si le g-module associé est semi-simple. Il revient au même de dire que $ \rho $ est semblable à une somme directe de représentations simples, ou que tout sous-K-module de M stable pour les $ \rho(x) $ ($ x \in g $) possède un supplémentaire stable pour les $ \rho(x) $ ($ x \in g $) (cf. Alg., chap. VIII, § 3, no 3).

5) Soit $ \delta $ une classe de représentations simples de g, correspondant à une classe C de g-modules simples. Soit d’autre part $ \rho $ une représentation de g dans M. Le composant isotypique $ M_c $ d’espèce C du g-module M (Alg., chap. VIII, § 3, no 4) s’appelle aussi le composant isotypique d’espèce $ \delta $ de M. Ce composant est la somme des sous-K-modules de M stables pour les $ \rho(x) $ et dans lesquels les $ \rho(x) $ induisent une représentation de classe $ \delta $; il est somme directe de certains de ces sous-modules; si $ M_c $ est de longueur $ n $, on dit que $ \rho $ contient $ n $ fois $ \delta $. La somme des différents $ M_c $ est directe; elle est égale à M si et seulement si $ \rho $ est semi-simple.

6) Soient $ \rho, \rho' $ deux représentations de g. On dit que $ \rho' $ est une sous-représentation (resp. une représentation quotient) de $ \rho $ si le module de $ \rho' $ est un sous-module (resp. un module quotient) du module de $ \rho $.

Soit M un K-module. La représentation nulle de g dans M définit sur M une structure de g-module. Muni de cette structure, M est appelé un g-module trivial.

Soit M un g-module. Les g-modules quotients des sous-g-modules de M sont aussi les sous-g-modules des modules quotients de M : ils s’obtiennent en considérant deux sous-g-modules U, U’ de M tels que U ⊃ U’ et en formant le g-module U/U’. Ceci posé, si tous les modules simples du type précédent sont isomorphes à un g-module simple donné N, on dit que M est un g-module pur d’espèce N. Si ρ et σ sont les représentations de g correspondant à M et N, on dit aussi que ρ est pure d’espèce σ.

Soit M’ un sous-g-module de M. Pour que M soit pur d’espèce N, il faut et il suffit que M’ et M/M’ soient purs d’espèce N. En effet, la condition est évidemment nécessaire. Supposons-la vérifiée; et soient U, U’ des sous-g-modules de M tels que U’ ⊂ U et que U/U’ soit simple ; soit φ l’homomorphisme canonique de M sur M/M’ ; si φ(U) ≠ φ(U’), U/U’ est isomorphe à φ(U)/φ(U’), donc isomorphe à N ; si φ(U) = φ(U’), on a U ⊂ U’ + M’, donc U/U’ est isomorphe à un sous-module simple de (U’ + M’)/U’, et ce dernier module est lui-même isomorphe à M’/(U’ ∩ M’) ; donc U/U’ est encore isomorphe à N, de sorte que M est pur d’espèce N.

Soit toujours M un g-module, et supposons que l’ensemble des sous-g-modules de M qui sont purs d’espèce N admette un élément maximal M’. Alors, tout sous-module M’’ de M qui est pur d’espèce N est contenu dans M’. En effet, M’’/(M’ ∩ M’’) et M’ sont purs d’espèce N, donc M’ + M’’ est pur d’espèce N d’après ce qui précède, donc M’ + M’’ ⊂ M’.

Supposons que le g-module M admette une suite de Jordan-Hölder (M_i)_{0 \leq i \leq n}. Pour que M soit pur d’espèce N, il faut et il suffit que M_0/M_1, M_1/M_2, ..., M_{n-1}/M_n soient isomorphes à N ; en effet, la condition est évidemment nécessaire ; sa suffisance résulte aussitôt, par récurrence sur n, de ce qu’on a vu plus haut.

#### Proposition 1 {#lie-i-s3-prop-1 .statement}

Soient g une algèbre de Lie sur K, et a un idéal de g. Soient M un g-module, et N un a-module simple. Considérons M comme un a-module et supposons que l’ensemble des sous-a-modules de M qui sont purs d’espèce N admette un élément maximal M’. Alors M’ est un sous-g-module de M.

Soit y \in g. Soient φ l’application canonique de M sur M/M’, et f l’application m \mapsto φ(y_M.m) de M’ dans M/M’. Il suffit de montrer que f(M’) = \{0\}. Soit x \in a. Pour m \in M, on a

x_{M/M’} . f(m) = φ(x_M y_M . m) = φ(y_M x_M . m) + φ([x, y]_M . m).

Or, $[x, y] \in \alpha$, d’où $\varphi([x, y]_M \cdot m) = 0$; par ailleurs, $\varphi(y_M x_M \cdot m) = f(x_M \cdot m)$. Donc $x_{M/M'} \cdot f(m) = f(x_M \cdot m)$. Il en résulte que $f(M')$ est un sous-$\alpha$-module de $M/M'$ isomorphe à un quotient de $M'$, donc pur d’espèce $N$; d’où $f(M') = \{0\}$.

#### Corollaire {#lie-i-s3-n1-cor-1 .statement}

Soient $g$ une algèbre de Lie sur $K$, et $\alpha$ un idéal de $g$. Soit $M$ un $g$-module simple, de longueur finie en tant que $K$-module. Il existe un $\alpha$-module simple $N$ tel que $M$ soit un $\alpha$-module pur d’espèce $N$.

Puisque le $\alpha$-module $M$ est de longueur finie, il existe un élément minimal $N$ dans l’ensemble des sous-$\alpha$-modules de $M$ : c’est un sous-$\alpha$-module simple de $M$. Le plus grand sous-$\alpha$-module de $M$ qui est pur d’espèce $N$ est alors $\neq \{0\}$, et est un sous-$g$-module de $M$ (prop. 1), donc est identique à $M$.

### 2. Produit tensoriel de représentations

Nous avons défini, au n° 1, la somme directe d’une famille de représentations de $g$. Nous allons maintenant définir d’autres opérations sur les représentations.

Soient $g_1$, $g_2$ deux algèbres de Lie sur $K$, et $M_i$ un $g_i$-module ($i = 1, 2$). Soient $U_i$ l’algèbre enveloppante de $g_i$, et $\sigma_i$ l’application canonique de $g_i$ dans $U_i$. Alors $M_i$ est un $U_i$-module à gauche, donc $M_1 \otimes_K M_2$ est canoniquement muni d’une structure de $(U_1 \otimes_K U_2)$-module à gauche. Or $U_1 \otimes_K U_2$ est l’algèbre enveloppante de $g_1 \times g_2$, et l’application $(x_1, x_2) \mapsto \sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2)$ est l’application canonique de $g_1 \times g_2$ dans cette algèbre enveloppante (\S 2, n° 2). Donc il existe une structure de $(g_1 \times g_2)$-module sur $M = M_1 \otimes_K M_2$ telle que :

$$
\begin{align*}
(x_1, x_2)_M \cdot (m_1 \otimes m_2) &= (\sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2)) \cdot (m_1 \otimes m_2) \\
&= ((x_1)_{M_1} \cdot m_1) \otimes m_2 + m_1 \otimes ((x_2)_{M_2} \cdot m_2).
\end{align*}
$$

Cette structure définit une représentation de $g_1 \times g_2$ dans $M$.

Si maintenant $g_1 = g_2 = g$, l’homomorphisme $x \mapsto (x, x)$ de $g$ dans $g \times g$, composé avec la représentation précédente, définit une représentation de g dans M, donc une structure de g-module sur M, telle que :

(2) $ x_M \cdot (m_1 \otimes m_2) = (x_{M_1} \cdot m_1) \otimes m_2 + m_1 \otimes (x_{M_2} \cdot m_2). $

Par un raisonnement analogue, on voit que :

#### Proposition 2 {#lie-i-s3-prop-2 .statement}

Soient g une algèbre de Lie sur K, et $ M_i $ un g-module ($ 1 \leq i \leq n $). Dans le produit tensoriel $ M_1 \otimes_K M_2 \otimes \cdots \otimes_K M_n $ il existe une structure de g-module et une seule telle que

(3) $ x_M \cdot (m_1 \otimes \cdots \otimes m_n) = \sum_{i=1}^n m_1 \otimes \cdots \otimes (x_{M_i} \cdot m_i) \otimes \cdots \otimes m_n $

quels que soient $ x \in g, m_1 \in M_1, \ldots, x_n \in M_n $.

La représentation correspondante s’appelle le produit tensoriel des représentations données de g dans les $ M_i $.

En particulier, si M est un g-module, la prop. 2 définit une structure de g-module sur chaque $ M_p = \bigotimes^p M $, donc dans l’algèbre tensorielle T de M.

La formule (3) montre que, pour tout $ x \in g $, $ x_T $ est l’unique dérivation de l’algèbre T qui prolonge $ x_M $. On sait (§ 2, no 8) que $ x_T $ définit par passage aux quotients une dérivation de l’algèbre symétrique S de M. Donc S peut être considéré comme un g-module quotient de T, et les $ x_S $ sont des dérivations de S.

Plus particulièrement encore, considérons g comme un g-module grâce à la représentation adjointe de g. Soit U l’algèbre enveloppante de g. D’après la prop. 7 du § 2, $ x_M $ définit par passage aux quotients une dérivation de U qui n’est autre que la dérivation intérieure définie par $ \sigma(x) $ ($ \sigma $ désignant l’application canonique de g dans U). Donc U peut être considéré comme un g-module quotient de T. Si K est un corps de caractéristique 0, l’isomorphisme canonique de S sur U est un isomorphisme de g-modules (§ 2, no 8).

### 3. Représentations dans des modules d’homomorphismes

Soient encore $ g_1 $ et $ g_2 $ deux algèbres de Lie sur K, et $ M_i $ un $ g_i $-module ($ i = 1, 2 $). Soient $ U_i $ l’algèbre enveloppante de $ g_i $, et $ \sigma_i $ l’application canonique de $ g_i $ dans $ U_i $. Alors $ M_i $ est un $ U_i $-module à gauche, donc $ \mathcal{L}_K(M_1, M_2) $ est canoniquement muni d’une structure de $ (U_1^0 \otimes U_2)$-module à gauche. Or, $ U_1^0 \otimes_K U_2 $ est l’algèbre enveloppante de $ g_1^0 \times g_2 $, et l’application

$$
(x_1, x_2) \mapsto \sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2)
$$

est l’application canonique de $ g_1^0 \times g_2 $ dans cette algèbre enveloppante. Donc il existe une structure de $ (g_1^0 \times g_2)$-module sur $ M = \mathcal{L}_K(M_1, M_2) $ telle que

$$
((x_1, x_2)_M \cdot u) \cdot m_1 = ((\sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2)) \cdot u) \cdot m_1 \\
= u((x_1)_{M_1} \cdot m_1) + (x_2)_{M_2} \cdot u(m_1)
$$

quels que soient $ u \in \mathcal{L}_K(M_1, M_2) $, $ m_1 \in M_1 $. Cette structure définit une représentation de $ g_1^0 \times g_2 $ dans $ M $.

Si maintenant $ g_1 = g_2 = g $, l’homomorphisme $ x \mapsto (-x, x) $ de $ g $ dans $ g^0 \times g $, composé avec la représentation précédente, définit une représentation de $ g $ dans $ M $, donc une structure de $ g $-module sur $ M $, telle que

$$
(x_M \cdot u) \cdot m_1 = x_{M_2} \cdot u(m_1) - u(x_{M_1} \cdot m_1)
$$

ou

$$
x_M \cdot u = x_{M_2} u - u x_{M_1}.
$$

En combinant ce résultat avec la prop. 2, on voit que :

#### Proposition 3 {#lie-i-s3-prop-3 .statement}

*Soient $ g $ une algèbre de Lie sur $ K $, et $ M_i $ un $ g $-module ($ 1 \leq i \leq n+1 $). Soit $ N $ le $ K $-module $ \mathcal{L}_K(M_1, \ldots, M_n ; M_{n+1}) $ des applications multilinéaires de $ \prod_{i=1}^n M_i $ dans $ M_{n+1} $. Il existe une structure de $ g $-module et une seule sur $ N $ telle que*

$$
(x_N \cdot u)(m_1, \ldots, m_n) = - \sum_{i=1}^n u(m_1, \ldots, x_{M_i} \cdot m_i, \ldots, m_n) \\
+ x_{M_{n+1}} \cdot u(m_1, \ldots, m_n)
$$

quels que soient $ x \in g $, $ u \in N $ et les $ m_i \in M_i $ ($ 1 \leq i \leq n $).

En particulier, soient $ g $ une algèbre de Lie sur $ K $, $ M $ un $ g $-module. Considérons d’autre part $ K $ comme un $ g $-module trivial.

La prop. 3 définit dans $ \mathcal{L}_K(M, K) = M^* $ une structure de g-module. La représentation correspondante est appelée représentation *duale* de la représentation $ x \mapsto x_M $. On a :

(8)
$$
(x_{M^*} \cdot f)(m) = -f(x_M \cdot m)
$$
quels que soient $ x \in g, f \in M^*, m \in M $. Autrement dit :

(9)
$$
x_{M^*} = -{}^t x_M.
$$

Lorsque K est un corps et que M est de dimension finie, le g-module M est simple (resp. semi-simple) si et seulement si le g-module $ M^* $ est simple (resp. semi-simple).

#### Proposition 4 {#lie-i-s3-prop-4 .statement}

*Soient* $ M_1, M_2 $ *deux g-modules*. *Les applications* K-linéaires canoniques (*Alg.*, chap. II, 3e éd., § 4, no 2, prop. 2 et no 1, prop. 1) :
$$
M_1^* \otimes_K M_2 \xrightarrow{\varphi} \mathcal{L}_K(M_1, M_2), \quad \mathcal{L}_K(M_1, M_2^*) \xrightarrow{\psi} (M_1 \otimes_K M_2)^*
$$
*(où la deuxième est bijective)* sont des homomorphismes de g-modules.

Posons
$$
N = M_1^* \otimes M_2, \quad P = \mathcal{L}(M_1, M_2), \quad Q = \mathcal{L}(M_1, M_2^*), \quad R = (M_1 \otimes M_2)^*.
$$
On a, pour $ x \in g, f \in M_1^*, m_1 \in M_1, m_2 \in M_2 $,
$$
((\varphi x_N)(f \otimes m_2)) \cdot m_1 = (\varphi(x_{M_1^*} f \otimes m_2 + f \otimes x_{M_2} m_2)) \cdot m_1 \\
= \langle x_{M_1^*} f, m_1 \rangle m_2 + \langle f, m_1 \rangle x_{M_2} m_2
$$
$$
((x_P \varphi)(f \otimes m_2)) \cdot m_1 = x_{M_2}(\varphi(f \otimes m_2) \cdot m_1) - \varphi(f \otimes m_2)(x_{M_1} m_1) \\
= \langle f, m_1 \rangle x_{M_2} m_2 - \langle f, x_{M_1} m_1 \rangle m_2
$$
donc $ \varphi x_N = x_P \varphi $. D’autre part, pour $ x \in g, u \in \mathcal{L}(M_1, M_2^*), m_1 \in M_1, m_2 \in M_2 $, on a :
$$
(\psi x_Q u)(m_1 \otimes m_2) = \langle (x_Q u) \cdot m_1, m_2 \rangle = \langle x_{M_2^*} u m_1 - u x_{M_1} m_1, m_2 \rangle
$$
$$
(x_R \psi u)(m_1 \otimes m_2) = -\langle \psi u, x_{M_1} m_1 \otimes m_2 + m_1 \otimes x_{M_2} m_2 \rangle \\
= -\langle u x_{M_1} m_1, m_2 \rangle - \langle u m_1, x_{M_2} m_2 \rangle
$$
donc $ \psi x_Q = x_R \psi $, ce qui achève la démonstration.

On identifie les g-modules $ \mathcal{L}(M_1, M_2^*) $ et $ (M_1 \otimes M_2)^* $ par l’isomorphisme $ \psi $. Si $ M_1 $ et $ M_2 $ ont des bases finies, $ \varphi $ est un isomor-

### 4. Exemples

#### Exemple 1 {#lie-i-s3-n4-exa-1 .statement}

Soient g une algèbre de Lie sur K, M un g-module. La structure de g-module de M et la structure de g-module trivial de K définissent une structure de g-module sur le K-module $ N = \mathcal{L}(M, M; K) $ des formes bilinéaires sur M. On a
$$
(x_N.\beta)(m, m') = -\beta(x_M.m, m') - \beta(m, x_M.m')
$$
quels que soient $ x \in g $, $ m, m' $ dans M, $ \beta \in N $. Si $ \beta $ est un élément donné de N, l’ensemble des $ x \in g $ tels que $ x_N.\beta = 0 $ est une sous-algèbre de g.

Soient M un K-module, $ \beta $ une forme bilinéaire sur M. D’après ce qui précède, l’ensemble des $ x \in \mathrm{gl}(M) $ tels que
$$
\beta(x.m, m') + \beta(m, x.m') = 0
$$
quels que soient $ m \in M $ et $ m' \in M $ est une sous-algèbre de Lie de $ \mathrm{gl}(M) $. Supposons que K soit un corps, que M soit de dimension finie sur K, et que $ \beta $ soit non dégénérée. Alors, tout $ x \in \mathrm{gl}(M) $ admet un adjoint à gauche $ x^* $ partout défini (relativement à $ \beta $), et la sous-algèbre considérée est l’ensemble des $ x \in \mathrm{gl}(M) $ tels que $ x^* = -x $. On peut construire par ce procédé deux exemples importants d’algèbres de Lie :

a) Prenons $ M = K^n $, et
$$
\beta((\xi_1, \ldots, \xi_n), (\eta_1, \ldots, \eta_n)) = \xi_1 \eta_1 + \cdots + \xi_n \eta_n.
$$
Identifions canoniquement $ \mathrm{gl}(K^n) $ à $ \mathbf{M}_n(K) $. Alors, l’algèbre de Lie obtenue est l’algèbre de Lie des matrices antisymétriques.
*(Lorsque $ K = \mathbf{R} $, cette algèbre est l’algèbre de Lie du groupe orthogonal $ \mathbf{O}(n, \mathbf{R}) $.)*

b) Prenons $ M = K^{2m} $, et
$$
\beta((\xi_1, \ldots, \xi_{2m}), (\eta_1, \ldots, \eta_{2m})) = \xi_1 \eta_{m+1} - \eta_1 \xi_{m+1} + \cdots + \xi_m \eta_{2m} - \eta_m \xi_{2m}.
$$
La matrice de $ \beta $ par rapport à la base canonique de $ K^{2m} $ est la matrice $ \begin{pmatrix} 0 & I_m \\ -I_m & 0 \end{pmatrix} $. Soit $ U = \begin{pmatrix} A & B \\ C & D \end{pmatrix} $ la matrice par rapport à la base canonique de $ K^{2m} $ d’un élément $ u $ de $ \mathrm{gl}(M) $ ($ A, B, C, D $ dans $ \mathbf{M}_m(K) $). D’après la formule (50) d’Alg., chap. IX, § 1, no 10, $ u^* $ admet par rapport à la même base la matrice
$$
\begin{pmatrix} 0 & -I_m \\ I_m & 0 \end{pmatrix}
\begin{pmatrix} {}^tA & {}^tC \\ {}^tB & {}^tD \end{pmatrix}
\begin{pmatrix} 0 & I_m \\ -I_m & 0 \end{pmatrix}
= \begin{pmatrix} {}^tD & -{}^tB \\ -{}^tC & {}^tA \end{pmatrix}.
$$
La condition $ u^* = -u $ équivaut donc aux conditions
$$
D = -{}^tA \quad B = {}^tB \quad C = {}^tC.
$$
*Lorsque $ K = \mathbf{R} $, l’algèbre de Lie obtenue est l’algèbre de Lie du groupe symplectique $ \mathbf{Sp} (2m, \mathbf{R}) $.*

#### Exemple 2 {#lie-i-s3-n4-exa-2 .statement}

Conservons les notations de l’exemple 1.
La structure de g-module de M définit dans le K-module $ P = \mathcal{L}_K(M, M) $ des endomorphismes de M une structure de g-module. D’après (6), on a, quels que soient $ x \in g $, et $ u \in P $:
$$(11)$$
$$
x_P \cdot u = [x_M, u] = (\operatorname{ad} x_M) \cdot u
$$
$ \operatorname{ad} x_M $ désignant l’image de $ x_M $ dans la représentation adjointe de $ \mathrm{gl}(M) $. Autrement dit :
$$(12)$$
$$
x_P = \operatorname{ad} x_M
$$
dans $ \mathcal{L}(\mathcal{L}(M, M)) = \mathcal{L}(\mathrm{gl}(M)) $.

### 5. Éléments invariants

#### Définition 3 {#lie-i-s3-def-3 .statement}

*Soient g une algèbre de Lie, M un g-module. Un élément $ m \in M $ est dit invariant (pour la structure de g-module de M, ou pour la représentation correspondante de g) si $ x_M \cdot m = 0 $ pour tout $ x \in g $.*

*Soient G un groupe de Lie réel connexe, g son algèbre de Lie, $ \theta $ une représentation analytique de G dans un espace vectoriel réel E de dimension finie, $ \rho $ la représentation correspondante de g dans E. Soit $ m \in E $. L’élément $ m $ est invariant pour $ \rho $ si et seulement si $ \theta(g) \cdot m = m $ quel que soit $ g \in G $. Ceci justifie l’emploi du mot « invariant ».*

#### Exemple 1 {#lie-i-s3-n5-exa-1 .statement}

Soient M, N deux g-modules, et P = $ \mathcal{L}_K(M, N) $. Pour qu’un élément f de P soit invariant, il faut et il suffit, d’après (6), que f soit un homomorphisme du g-module M dans le g-module N. En particulier, si M = N et $ x_M = x_N $ pour tout $ x \in g $, f est invariant si et seulement si f est permutable aux $ x_M $.

#### Exemple 2 {#lie-i-s3-n5-exa-2 .statement}

Soit M un K-module admettant une base finie. Si M est muni d’une structure de g-module, $ \mathcal{L}(M, M) $ et $ M^* \otimes M $ sont munis de structures de g-modules, et l’application canonique de $ M^* \otimes M $ dans $ \mathcal{L}(M, M) $ est un isomorphisme de g-modules (prop. 4). Comme $ 1 \in \mathcal{L}(M, M) $ est évidemment un invariant (cf. exemple 1), l’élément correspondant u de $ M^* \otimes M $ est un invariant. Si $ (e_i)_{1 \leq i \leq n} $ est une base de M, et si $ (e_i^*)_{1 \leq i \leq n} $ est la base duale, on a $ u = \sum_{i=1}^n e_i^* \otimes e_i $.

#### Exemple 3 {#lie-i-s3-n5-exa-3 .statement}

Soit M un g-module. Soit $ \beta $ une forme bilinéaire sur M, et soit f l’élément correspondant de $ \mathcal{L}(M, M^*) $. Pour que $ \beta $ soit invariante, il faut et il suffit que f soit un homomorphisme de g-modules (prop. 4 et exemple 1). Supposons que K soit un corps, et que $ \dim_K M < +\infty $. Une forme bilinéaire $ \beta $ sur M invariante et non dégénérée définit un isomorphisme du g-module M sur le g-module $ M^* $, donc un isomorphisme du g-module $ M \otimes M $ sur le g-module $ M^* \otimes M $. Ainsi, compte tenu de l’exemple 2, la donnée de $ \beta $ définit canoniquement un élément invariant c dans le g-module $ M \otimes M $, qu’on peut construire de la manière suivante : soit $ (e_i)_{1 \leq i \leq n} $ une base de M, $ (e_i')_{1 \leq i \leq n} $ la base de M telle que $ \beta(e_i, e_j') = \delta_{ij} $; alors $ c = \sum_{i=1}^n e_i \otimes e_i' $.

#### Proposition 5 {#lie-i-s3-prop-5 .statement}

Soient g une K-algèbre de Lie, h un idéal de g, $ \rho $ une représentation de g dans M, et $ \rho' $ la restriction de $ \rho $ à h. Alors l’ensemble N des éléments de M invariants pour $ \rho' $ est stable pour $ \rho(g) $.

En effet, soient $ n \in N $ et $ y \in g $; quel que soit $ x \in h $, on a $ [x, y] \in h $, donc $ \rho(x)\rho(y)n = \rho([x, y])n + \rho(y)\rho(x)n = 0 $; donc $ \rho(y)n \in N $.

#### Proposition 6 {#lie-i-s3-prop-6 .statement}

Soit M un g-module semi-simple. Alors le sous-module $ M_0 $ des éléments invariants de M admet un et un seul supplémentaire stable pour les $ x_M $, à savoir le sous-module $ M_1 $ engendré par les $ x_M \cdot m $ ($ x \in g, m \in M $).

En effet, soit $ M' $ un sous-module de $ M $ stable pour les $ x_M $ et supplémentaire de $ M_0 $ dans $ M $. Pour tout $ m \in M $, on a $ m = m_0 + m' $ avec $ m_0 \in M_0,\ m' \in M' $, donc $ x_M m = x_M m' \in M' $. Donc $ M_1 \subset M' $. Soit $ M_2 $ un sous-module de $ M' $ stable pour les $ x_M $ et supplémentaire de $ M_1 $ dans $ M' $. Pour tout $ m \in M_2 $, on a $ x_M m \in M_2 \cap M_1 = \{0\} $ quel que soit $ x \in g $, donc $ m \in M_0 $, donc $ m = 0 $. Donc $ M_2 = \{0\} $, ce qui prouve que $ M_1 = M' $.

### 6. Formes bilinéaires invariantes

Soit $ g $ une algèbre de Lie sur $ K $. La représentation adjointe de $ g $ dans $ g $ et la représentation nulle de $ g $ dans $ K $ définissent dans le $ K $-module $ N = \mathcal{L}(g, g; K) $ des formes bilinéaires sur $ g $ une structure de $ g $-module. On dit brièvement qu’une forme bilinéaire $ \beta $ sur $ g $ est *invariante* si elle est invariante pour la représentation $ x \mapsto x_N $. D’après la formule (10), la condition nécessaire et suffisante pour qu’il en soit ainsi est que :

$$
\beta([x, y], z) = \beta(x, [y, z])
$$

quels que soient $ x, y, z $ dans $ g $.

Maintenant, soit $ \mathfrak{d} $ l’algèbre de Lie des dérivations de $ g $. La représentation identique de $ \mathfrak{d} $ et la représentation nulle de $ \mathfrak{d} $ dans $ K $ définissent une représentation $ D \mapsto D_N $ de $ \mathfrak{d} $ dans $ N $. On dit brièvement qu’une forme bilinéaire sur $ g $ est *complètement invariante* si elle est invariante pour la représentation $ D \mapsto D_N $. Une forme bilinéaire complètement invariante est invariante. Pour qu’une forme bilinéaire $ \beta $ sur $ g $ soit complètement invariante, il faut et il suffit qu’on ait :

$$
\beta(Dx, y) + \beta(x, Dy) = 0
$$

quels que soient $ x, y $ dans $ g $ et $ D \in \mathfrak{d} $.

#### Proposition 7 {#lie-i-s3-prop-7 .statement}

*Soient $ g $ une algèbre de Lie, $ \beta $ une forme bilinéaire symétrique invariante sur $ g $, et $ a $ un idéal de $ g $.*

a) *L’orthogonal $ a' $ de $ a $ pour $ \beta $ est un idéal de $ g $.*

b) Si $ a $ est caractéristique, et si $ \beta $ est complètement invariante, $ a' $ est caractéristique.

c) Si $ \beta $ est non dégénérée, $ a \cap a' $ est commutatif.

Soit D une dérivation de g. Supposons que $ a $ soit stable pour D et que $ \beta(Dx, y) + \beta(x, Dy) = 0 $ pour $ x, y $ dans g. Alors, $ z \in a' $ entraîne $ Dz \in a' $, car pour tout $ t \in a $, on a $ Dt \in a $, donc $ \beta(Dz, t) = -\beta(z, Dt) = 0 $. Ainsi, $ a' $ est stable pour D. Ceci établit a) et b).

Soit maintenant b un idéal de g, et supposons que la restriction de $ \beta $ à b soit nulle. Pour $ x, y $ dans b et $ z \in g $, on a $ \beta([x, y], z) = \beta(x, [y, z]) = 0 $, car $[y, z] \in b$. Ainsi, $[b, b]$ est orthogonal à g. Si $ \beta $ est non dégénérée, b est donc commutatif. Ce résultat, appliqué à $ a \cap a' $, prouve c).

#### Définition 4 {#lie-i-s3-def-4 .statement}

Soient g une K-algèbre de Lie, M un g-module. Supposons que M, considéré comme K-module, admette une base finie. On appelle forme bilinéaire associée au g-module M (ou à la représentation correspondante) la forme bilinéaire symétrique $(x, y) \mapsto \operatorname{Tr}(x_M y_M)$ sur g. Si la représentation considérée est la représentation adjointe, la forme bilinéaire associée s’appelle la forme de Killing de g.

#### Proposition 8 {#lie-i-s3-prop-8 .statement}

Soient g une algèbre de Lie, M un g-module. Supposons que M, considéré comme K-module, admette une base finie. La forme bilinéaire associée à M est invariante.

En effet, pour $ x, y, z $ dans g, on a :

$$
\operatorname{Tr}([x, y]_M z_M) = \operatorname{Tr}(x_M y_M z_M) - \operatorname{Tr}(y_M x_M z_M) = \operatorname{Tr}(x_M y_M z_M) - \operatorname{Tr}(x_M z_M y_M)
= \operatorname{Tr}(x_M [y, z]_M).
$$

#### Proposition 9 {#lie-i-s3-prop-9 .statement}

Supposons que K soit un corps et que l’algèbre de Lie g soit de dimension finie sur K. Soient a un idéal de g, $ \beta $ la forme de Killing de g, et $ \beta' $ celle de a. Alors, $ \beta' $ est la restriction de $ \beta $ à a.

En effet, soit u un endomorphisme de l’espace vectoriel g qui laisse stable a. Soient $ \nu $ la restriction de u à a, et $ \varphi $ l’endomorphisme de l’espace vectoriel $ g/a $ déduit de u par passage au quotient. On a $ \operatorname{Tr} u = \operatorname{Tr} \nu + \operatorname{Tr} \varphi $ comme on le voit en prenant une base $(x_1, \ldots, x_n)$ de g dont les p premiers éléments constituent une base de $ a $. Ceci posé, soient $ x \in a,\ y \in a $, et appliquons la formule précédente au cas où $ u = (\mathrm{ad}_g x)(\mathrm{ad}_g y) $. On a $ v = (\mathrm{ad}_a x)(\mathrm{ad}_a y) $, et $ w = 0 $. Donc $ \beta(x, y) = \beta'(x, y) $.

#### Proposition 10 {#lie-i-s3-prop-10 .statement}

*Supposons que K soit un corps, et que l’algèbre de Lie g soit de dimension finie sur K. La forme de Killing $ \beta $ de g est complètement invariante.*

Soit D une dérivation de g. Il existe une algèbre de Lie $ g' $ contenant g comme idéal de codimension 1, et un élément $ x_0 $ de $ g' $, tels que $ Dx = [x_0, x] $ pour tout $ x \in g $ (\S 1, no 8, exemple 1). Soit $ \beta' $ la forme de Killing de $ g' $. Pour $ x, y $ dans g, on a $ \beta'([x, x_0], y) = \beta'(x, [x_0, y]) $, c’est-à-dire $ \beta'(Dx, y) + \beta'(x, Dy) = 0 $. Or, la restriction de $ \beta' $ à g est $ \beta $ (prop. 9). D’où la proposition.

### 7. Élément de Casimir

#### Proposition 11 {#lie-i-s3-prop-11 .statement}

*Soient g une algèbre de Lie sur un corps K, U son algèbre enveloppante, $ h $ un idéal de dimension finie de g, et $ \beta $ une forme bilinéaire invariante sur g, dont la restriction à $ h $ soit non dégénérée. Soient $ (e_i)_{1 \leq i \leq n},\ (e'_j)_{1 \leq j \leq n} $ deux bases de $ h $ telles que $ \beta(e_i, e'_j) = \delta_{ij} $. Alors l’élément $ c = \sum_{i=1}^n e_i e'_i $ de U appartient au centre de U et est indépendant du choix de la base $ (e_i) $.

Pour $ x \in g $, soit $ x_h $ la restriction à $ h $ de $ \mathrm{ad}_g x $. Alors, $ x \mapsto x_h $ est une représentation de g dans l’espace $ h $, et la restriction $ \beta' $ de $ \beta $ à $ h $ est invariante pour cette représentation. D’après le no 5, exemple 3, le tenseur $ \sum_{i=1}^n e_i \otimes e'_i $ est indépendant du choix de la base $ (e_i) $, et est un élément invariant de l’algèbre tensorielle de $ h $. C’est aussi un élément de l’algèbre tensorielle T de g, invariant pour la représentation déduite de la représentation adjointe de g. Son image canonique dans U, c’est-à-dire c, est donc indépendante du choix de la base $ (e_i) $, et est un invariant pour la représentation de g dans U considérée à la fin du no 2. Cet élément est donc permutable à tout élément de g, et par suite appartient au centre de U.

Lorsque $ \beta $ est la forme bilinéaire associée à un g-module M, on dit que l’élément c de la proposition 11 est l’élément de Casimir associé à M (ou à la représentation correspondante). Cet élément existe si la restriction de $ \beta $ à $ \mathfrak{h} $ est non dégénérée.

#### Proposition 12 {#lie-i-s3-prop-12 .statement}

*Soient g une algèbre de Lie sur un corps K, $ \mathfrak{h} $ un idéal de dimension finie n de g, et M un g-module de dimension finie sur K. Soit c l’élément de Casimir (supposé exister) associé à M et $ \mathfrak{h} $.

a) *On a* $ \mathrm{Tr}\,(c_M) = n $.

b) *Si M est simple, et si n n’est pas divisible par la caractéristique de K, $ c_M $ est un automorphisme de M.*

Reprenant les notations de la prop. 11, on a $ \mathrm{Tr}\,(c_M) = \sum_{i=1}^n \mathrm{Tr}\,((e_i)_M(e_i')_M) = \sum_{i=1}^n \beta(e_i, e_i') = n $. Donc, si n n’est pas divisible par la caractéristique de K, $ c_M \neq 0 $. D’autre part, comme c appartient au centre de U, $ c_M $ est permutable à tous les $ x_M, x \in g $. Si de plus M est simple, $ c_M $ est donc inversible dans $ \mathcal{L}(M) $ (*Alg.*, chap. VIII, § 4, no 3, prop. 2).

### 8. *Extension de l’anneau de base*

Soient $ K_1 $ un anneau commutatif à élément unité, $ \varphi $ un homomorphisme de K dans $ K_1 $ transformant 1 en 1. Soient g une K-algèbre de Lie, U son algèbre enveloppante, et M un g-module à gauche, c’est-à-dire un U-module à gauche. Alors, $ M_{(K_1)} $ est canoniquement muni d’une structure de $ U_{(K_1)} $-module à gauche, donc de $ g_{(K_1)} $-module à gauche. Soient $ \rho $ et $ \rho_{(K_1)} $ les représentations de g et $ g_{(K_1)} $ correspondant à M et $ M_{(K_1)} $ : on dit que $ \rho_{(K_1)} $ se déduit de $ \rho $ par *extension de l’anneau de base*, et on peut appliquer les résultats d’*Alg.*, chap. VIII, § 13, no 4. Si $ x \in g $, $ \rho_{(K_1)}(x) $ n’est autre que l’endomorphisme $ \rho(x) \otimes 1 $ de $ M_{(K_1)} = M \otimes_K K_1 $.

Supposons que K soit un corps, que $ K_1 $ soit une extension de K, et que $ \varphi $ soit l’injection canonique de K dans $ K_1 $. Soient V et $ V' $ des sous-espaces vectoriels de M. Soit $ a $ le sous-espace vectoriel de g formé des $ x \in g $ tels que $ \rho(x)(V) \subset V' $. Soit $ a' $ le sous-espace vectoriel de $ g_{(K_1)} $ formé des $ x' \in g_{(K_1)} $ tels que $ \rho_{(K_1)}(x')(V_{(K_1)}) \subset V'_{(K_1)} $. Alors, $ a' = a_{(K_1)} $. Il est clair en effet que $ a_{(K_1)} \subset a' $. Soit maintenant x' \in a'. On peut écrire $ x' = \sum_{i=1}^n \lambda_i x_i $, où les $ x_i $ sont dans $ g $, et où les $ \lambda_i $ sont des éléments de $ K_1 $ linéairement indépendants sur $ K $. Pour tout $ u \in V $, on a $ \rho(x').u \in V'_{(K_1)} $, c’est-à-dire $ \sum_{i=1}^n \lambda_i \rho(x_i).u \in V'_{(K_1)} $, d’où $ \rho(x_i).u \in V' $, donc $ x_i \in a $ et $ x' \in a_{(K_1)} $. Ceci montre bien que $ a' = a_{(K_1)} $. En particulier, le centre de $ g_{(K_1)} $ se déduit du centre de $ g $ par extension de $ K $ à $ K_1 $ : il suffit d’appliquer ce qui précède à la représentation adjointe de $ g $. Il en résulte que $ C_p(g_{(K_1)}) = (C_p g)_{(K_1)} $ pour tout $ p $. De même, soient $ h $ une sous-algèbre de $ g $, et $ n $ le normalisateur de $ h $ dans $ g $. Alors, le normalisateur de $ h_{(K_1)} $ dans $ g_{(K_1)} $ est $ n_{(K_1)} $.

Soient $ K, K_1, g, \rho, M $ comme dans l’alinéa précédent. Soient $ b $ un sous-espace vectoriel de $ g $, et $ W $ un sous-espace vectoriel de $ M $. Soit $ V $ le sous-espace vectoriel de $ M $ formé des $ m \in M $ tels que $ \rho(b).m \subset W $. Soit $ V' $ le sous-espace vectoriel de $ M_{(K_1)} $ formé des $ m' \in M_{(K_1)} $ tels que $ \rho_{(K_1)}(b_{(K_1)}).m' \subset W_{(K_1)} $. On voit comme ci-dessus que $ V' = V_{(K_1)} $. En particulier, le sous-espace vectoriel des invariants de $ M_{(K_1)} $ se déduit du sous-espace vectoriel des invariants de $ M $ par extension du corps de base de $ K $ à $ K_1 $.

Soient $ K, K_1 $ et $ \varphi $ comme au début de ce no. Soient $ g $ une $ K $-algèbre de Lie, $ M $ et $ N $ des $ g $-modules. Si $ M $ et $ N $ sont des $ g $-modules isomorphes, $ M_{(K_1)} $ et $ N_{(K_1)} $ sont des $ g_{(K_1)} $-modules isomorphes. Inversement :

#### Proposition 13 {#lie-i-s3-prop-13 .statement}

*Soient K un corps, K₁ une extension de K, g une K-algèbre de Lie, M, N deux g-modules de dimension finie sur K. Si M_{(K₁)} et N_{(K₁)} sont des g_{(K₁)}-modules isomorphes, M et N sont des g-modules isomorphes.*

La démonstration se fait en deux étapes.

1° Supposons d’abord que $ K_1 $ soit une extension de $ K $ de *degré fini* $ n $. Soit $ U $ l’algèbre enveloppante de $ g $, de sorte que l’algèbre enveloppante de $ g_{(K_1)} $ est $ U_{(K_1)} = U \otimes_K K_1 $ (\S 2, no 9). Étant isomorphes en tant que $ U_{(K_1)} $-modules, $ M_{(K_1)} $ et $ N_{(K_1)} $ le sont *a fortiori* en tant que $ U $-modules ; mais en tant que $ U $-modules, ils sont respectivement isomorphes à $ M^n $ et $ N^n $. Or, $ M $ et $ N $ sont des $ U $-modules de longueur finie ; $ M $ (resp. $ N $) est donc somme directe d’une famille $ (P_i^{r_i})_{1 \leq i \leq p} $ (resp. $ (Q_j^{s_j})_{1 \leq j \leq q} $) de sous-modules tels que les $ P_i $ (resp. $ Q_j $) soient indécomposables et deux $ P_i $ (resp. $ Q_j $) d’in-

2° Cas général. Soient $ P $ le g-module $ \mathcal{L}_K(M, N) $ et $ Q $ le sous-espace des invariants de $ P $, c’est-à-dire l’ensemble des homomorphismes du g-module $ M $ dans le g-module $ N $. Dans le $ g_{(K_1)} $-module $ \mathcal{L}_{K_1}(M_{(K_1)}, N_{(K_1)}) = (\mathcal{L}_K(M, N))_{(K_1)} $, le sous-espace des invariants est $ Q_{(K_1)} $. L’hypothèse que $ M_{(K_1)} $ et $ N_{(K_1)} $ sont isomorphes entraîne que $ M $ et $ N $ ont même dimension sur $ K $, et qu’il existe dans $ Q_{(K_1)} $ un élément $ g $ qui est un isomorphisme de $ M_{(K_1)} $ sur $ N_{(K_1)} $. Soit $ (f_1, \ldots, f_d) $ une base de $ Q $ sur $ K $. Choisissons d’autre part des bases de $ M $ et $ N $ sur $ K $. Si $ \lambda_k \in K_1 $ pour $ 1 \leq k \leq d $, la matrice de $ f = \sum_{k=1}^d \lambda_k f_k $ par rapport à ces bases a un déterminant qui est un polynôme $ D(\lambda_1, \ldots, \lambda_d) $ à coefficients dans $ K $. Lorsque $ f = g $, ce déterminant est non nul, donc les coefficients de $ D $ ne sont pas tous nuls. Par suite, si $ \Omega $ est la clôture algébrique de $ K $, il existe (puisque $ \Omega $ est infini) des éléments $ \mu_k \in \Omega $ ($ 1 \leq k \leq d $) tels que $ D(\mu_1, \ldots, \mu_d) \neq 0 $ (Alg., chap. IV, § 2, n° 5, prop. 8). Si $ K_2 $ est l’extension algébrique de $ K $ engendrée par les $ \mu_k $ ($ 1 \leq k \leq d $), on en conclut que $ \sum_{k=1}^d \mu_k f_k $ est un isomorphisme de $ M_{(K_2)} $ sur $ N_{(K_2)} $; mais $ K_2 $ est de degré fini sur $ K $ (Alg., chap. V, § 3, n° 2, prop. 5), donc $ M $ et $ N $ sont isomorphes en vertu de la première partie du raisonnement.

Soient à nouveau $ K $, $ K_1 $ et $ \varphi $ comme au début de ce n°. Soit $ \rho $ une représentation de $ g $ dans un $ K $-module $ M $ possédant une base finie $ (x_1, \ldots, x_n) $. Alors, la forme bilinéaire sur $ g_{(K_1)} $ associée à $ \rho_{(K_1)} $ se déduit de la forme bilinéaire associée à $ \rho $ par extension à $ K_1 $ de l’anneau de base (car, si $ u \in \mathcal{L}_K(M) $, $ u $ a même matrice par rapport à $ (x_1, \ldots, x_n) $ que $ u \otimes 1 $ par rapport à $ (x_1 \otimes 1, \ldots, x_n \otimes 1) $, donc $ u $ et $ u \otimes 1 $ ont même trace). En particulier, si le $ K $-module $ g $ possède une base finie, la forme de Killing de $ g_{(K_1)} $ se déduit de celle de $ g $ par extension à $ K_1 $ de l’anneau de base.

## EXERCICES {#lie-i-s3-exercises}

See the [exercises for § 3](exercises/s3/).
