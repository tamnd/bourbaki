---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 0
section_title: Pseudomodules
appendix: true
lang: en
source: alg-i-iii
source_edition: 1998, Springer
pdf_pages: 0402-0403, 0449-0449
extraction: ocr
subsections:
    - "no": 1
      title: ADJUNCTION OF A UNIT ELEMENT TO A PSEUDO-RING
      page: 0
      pdf_page: 402
    - "no": 2
      title: PSEUDOMODULES
      page: 0
      pdf_page: 402
statements: 0
exercises: 1
content_sha256: 8dadb62bfc1bd59df992f75ed61678738e3e2027654e5a156885bd2ce862c8d4
---

## APPENDIX

# PSEUDOMODULES

### 1. ADJUNCTION OF A UNIT ELEMENT TO A PSEUDO-RING

Let A be a pseudo-ring (I, § 8, no. 1). On the set $ A' = \mathbf{Z} \times A $ we define the following laws of composition:

$$
\begin{cases}
(m, a) + (n, b) = (m + n, a + b) \\
(m, a)(n, b) = (mn, mb + na + ab).
\end{cases}
$$

It is immediately verified that $ A' $ with these two laws of composition is a ring in which the element $ (1, 0) $ is the unit element. The set $ \{0\} \times A $ is a two-sided ideal of $ A' $ and $ i : x \mapsto (0, x) $ is an isomorphism of the pseudo-ring A onto the sub-pseudo-ring $ \{0\} \times A $ by means of which A and $ \{0\} \times A $ are identified. $ A' $ is called the ring derived from the pseudo-ring A by adjoining a unit element.

If A already has an identity element $ \varepsilon $, the element $ e = (0, \varepsilon) $ of $ A' $ is an idempotent belonging to the centre of $ A' $ and such that

$$
A = eA' = A'e.
$$

Then $ (eA', (1 - e)A') $ is a direct decomposition (I, § 8, no. 11) of $ A' $ and the ring $ (1 - e)A' $ is isomorphic to $ \mathbf{Z} $.

### 2. PSEUDOMODULES

Given a pseudo-ring A with or without a unit element, a left pseudomodule over A is a commutative group E (written additively) admitting A as set of operators and satisfying axioms $ (\mathrm{M}_I), (\mathrm{M}_{II}) $ and $ (\mathrm{M}_{III}) $ of § 1, no. 1, Definition 1. Right pseudomodules over A are defined similarly.

Let $ A' $ be the ring obtained by adjoining a unit element to A. If E is a left pseudomodule over A, a left $ A' $-module structure on E is associated with it by writing, for all $ x \in E $ and every element $ (n, a) \in A' $,

$$
(n, a) . x = nx + ax.
$$

Axioms $ (\mathrm{M}_I) $ to $ (\mathrm{M}_{IV}) $ of § 1, no. 1, Definition 1 are immediately verified;

moreover, by restricting the set of operators of this module structure to $ \{0\} \times A $ (identified with $ A $), we obtain on $ E $ the pseudomodule structure given initially.

For a subset $ M $ of $ E $ to be a subgroup with operators of the pseudomodule $ E $ (in which case the induced structure is obviously also a left pseudomodule structure over $ A $), it is necessary and sufficient that $ M $ be a submodule of the associated $ A' $-module $ E $ and this sub-$ A' $-module is associated with the pseudomodule $ M $. Moreover, the quotient $ A' $-module $ E/M $ is then associated with the quotient group with operators $ E/M $, which is obviously a pseudomodule over $ A $.

If $ E, F $ are two pseudomodules over $ A $, the homomorphisms $ E \to F $ of groups with operators are identical with the $ A' $-linear mappings $ E \to F $ of the $ A' $-modules associated respectively with the pseudomodules $ E $ and $ F $. If $ (E_i)_{i \in I} $ is a family of pseudomodules over $ A $, the groups with operators $ \prod_{i \in I} E_i $ and $ \bigoplus_{i \in I} E_i $ are pseudomodules over $ A $ and the associated $ A' $-modules are respectively the product and direct sum of the associated $ A' $-modules $ E_i $. There are analogous results for inverse and direct limits of pseudomodules. The theory of pseudomodules over $ A $ can thus be entirely reduced to that of $ A' $-modules.

### Exercises {#alg-ii-a0-exercises}

See the [exercises for Appendix 0](exercises/a0/).
