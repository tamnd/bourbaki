---
book: alg
book_title: Algebra
chapter: II
chapter_title: ALGÈBRE LINÉAIRE
section: 0
section_title: Pseudomodules
appendix: true
lang: fr
source: alg-i-iii-fr
book_pages: A II.210
pdf_pages: 0353-0355, 0387-0387
extraction: ocr
subsections:
    - "no": 1
      title: Adjonction d’un élément unité à un pseudo-anneau
      page: 176
      pdf_page: 353
    - "no": 2
      title: Pseudomodules
      page: 177
      pdf_page: 354
statements: 0
exercises: 1
content_sha256: d1d81eabc2be6768af1f9aa999692e418b79979ac3ddd846772e2e1ebfabcdf9
---

## APPENDICE

# PSEUDOMODULES

### 1. Adjonction d’un élément unité à un pseudo-anneau

Soit A un pseudo-anneau (I, p. 93). Sur l’ensemble A′ = Z × A, définissons les lois de composition suivantes:
(1)
$$
\begin{cases}
(m, a) + (n, b) = (m + n, a + b) \\
(m, a)(n, b) = (mn, mb + na + ab).
\end{cases}
$$

On vérifie aussitôt que $A'$, muni de ces deux lois de composition, est un anneau, dans lequel l’élément $(1, 0)$ est l’élément unité. L’ensemble $\{0\} \times A$ est un idéal bilatère de $A'$ et $i : x \mapsto (0, x)$ est un isomorphisme du pseudo-anneau $A$ sur le sous-pseudo-anneau $\{0\} \times A$, au moyen duquel on identifie $A$ et $\{0\} \times A$. On dit que $A'$ est l’anneau déduit du pseudo-anneau $A$ par adjonction d’un élément unité.

Si $A$ admet déjà un élément unité $\varepsilon$, l’élément $e = (0, \varepsilon)$ de $A'$ est un idempotent appartenant au centre de $A'$ et tel que
$$
A = eA' = A'e.
$$
Alors $(eA', (1 - e)A')$ est une décomposition directe (I, p. 105) de $A'$, et l’anneau $(1 - e)A'$ est isomorphe à $\mathbf{Z}$.

### 2. Pseudomodules

Étant donné un pseudo-anneau $A$ ayant ou non un élément unité, on appelle pseudomodule à gauche sur $A$ un groupe commutatif $E$ (noté additivement) admettant $A$ comme ensemble d’opérateurs et vérifiant les axiomes $(M_I)$, $(M_{II})$ et $(M_{III})$ de II, p. 1, déf. 1. On définit de même les pseudomodules à droite sur $A$.

Soit $A'$ l’anneau obtenu par adjonction à $A$ d’un élément unité. Si $E$ est un pseudomodule à gauche sur $A$, on lui associe sur $E$ une structure de $A'$-module à gauche en posant, pour tout $x \in E$ et tout élément $(n, a) \in A'$
$$(2)$$
$$(n, a).x = nx + ax.$$

On vérifie en effet aussitôt les axiomes $(M_I)$ à $(M_{IV})$ de II, p. 1, déf. 1 ; en outre, en restreignant à $\{0\} \times A$ (identifié à $A$) l’ensemble d’opérateurs de cette structure de module, on obtient sur $E$ la structure de pseudomodule donnée initialement.

Pour qu’une partie $M$ de $E$ soit un sous-groupe à opérateurs du pseudomodule $E$ (auquel cas la structure induite est évidemment encore une structure de pseudomodule à gauche sur $A$), il faut et il suffit que $M$ soit un sous-module du $A'$-module $E$ associé, et ce sous-$A'$-module est associé au pseudomodule $M$. En outre, le $A'$-module quotient $E/M$ est alors associé au groupe à opérateurs quotient $E/M$, qui est évidemment un pseudomodule sur $A$.

Si $E$, $F$ sont deux pseudomodules sur $A$, il y a identité entre les homomorphismes de groupes à opérateurs $E \to F$ et les applications $A'$-linéaires $E \to F$ des $A'$-modules associés respectivement aux pseudomodules $E$ et $F$. Si $(E_t)_{t \in I}$ est une famille de pseudomodules sur $A$, les groupes à opérateurs $\prod_{t \in I} E_t$ et $\bigoplus_{t \in I} E_t$ sont des pseudomodules sur $A$, et les $A'$-modules associés sont respectivement le produit et la somme directe des $A'$-modules $E_t$ associés. On a des résultats analogues pour les limites projectives et inductives de pseudomodules. La théorie des pseudomodules sur $A$ est ainsi ramenée à celle des $A'$-modules.

Exercices

## EXERCICES {#alg-ii-a0-exercises}

See the [exercises for Appendix 0](exercises/a0/).
