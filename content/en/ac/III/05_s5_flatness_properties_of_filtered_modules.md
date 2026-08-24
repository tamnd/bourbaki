---
book: ac
book_title: Commutative Algebra
chapter: III
chapter_title: GRADUATIONS. FILTRATIONS AND TOPOLOGIES
section: 5
section_title: Flatness properties of filtered modules
lang: en
source: ac-i-vii
book_pages: 226-231, 259-260
pdf_pages: 0246-0251, 0279-0280
extraction: ocr
subsections:
    - "no": 1
      title: IDEALLY HAUSDORFF MODULES
      page: 226
      pdf_page: 246
    - "no": 2
      title: STATEMENT OF THE FLATNESS CRITERION
      page: 227
      pdf_page: 247
    - "no": 3
      title: PROOF OF THE FLATNESS CRITERION
      page: 228
      pdf_page: 248
    - "no": 4
      title: APPLICATIONS
      page: 230
      pdf_page: 250
statements: 11
exercises: 8
content_sha256: 33bce3ef055753218cc68b75a010c6127c9782712ba7a3b649efe320275f38ab
---

## 5. FLATNESS PROPERTIES OF FILTERED MODULES

### 1. IDEALLY HAUSDORFF MODULES

#### Definition 1 {#ac-iii-s5-def-1 .statement}

*Let A be a commutative ring and $ \mathfrak{g} $ an ideal of A. An A-module M is called ideally Hausdorff with respect to 3 (or simply ideally Hausdorff if there is no ambiguity) if, for every finitely generated ideal $ \mathfrak{a} $ of A, the A-module $ \mathfrak{a} \otimes_A M $ is Hausdorff with the 3-adic topology.*

Putting $ \mathfrak{a} = A $ in this definition, we have already seen that M is necessarily *Hausdorff* with the 3-adic topology.

*Examples*

#### Example 1 {#ac-iii-s5-n1-exa-1 .statement}

If A is Noetherian and $ \mathfrak{g} $ is contained in the Jacobson radical of A (in other words if A is a Zariski ring with the 3-adic topology), every *finitely generated* A-module is ideally Hausdorff (*§3*, no. 3, Proposition 6).

#### Example 2 {#ac-iii-s5-n1-exa-2 .statement}

Every direct sum of ideally Hausdorff modules is an ideally Hausdorff module, by virtue of the relations
$$
\mathfrak{g}^n \left( a \otimes_A \bigoplus_{\lambda \in L} M_\lambda \right) = \mathfrak{g}^n \bigoplus_{\lambda \in L} (a \otimes_A M_\lambda) = \bigoplus_{\lambda \in L} \mathfrak{g}^n (a \otimes_A M_\lambda).
$$

#### Example 3 {#ac-iii-s5-n1-exa-3 .statement}

If an A-module M is flat and Hausdorff with the $ \mathfrak{g} $-adic topology it is ideally Hausdorff, for $ a \otimes_A M $ is then identified with a submodule of M and the $ \mathfrak{g} $-adic topology on $ a \otimes_A M $ is finer than the topology induced on $ a \otimes_A M $ by the $ \mathfrak{g} $-adic topology on M, which is Hausdorff by hypothesis.

### 2. STATEMENT OF THE FLATNESS CRITERION
Let A be a ring, $ \mathfrak{z} $ a two-sided ideal of A, M a left-module and gr(A) and gr(M) the graded ring and graded gr(A)-module associated respectively with the ring A and with the module M with the $ \mathfrak{g} $-adic filtrations (\S 2, no. 3). We have seen (loc. cit.) that for every integer $ n \geq 0 $ there is a surjective $ \mathbf{Z} $-module homomorphism
$$
\gamma_n : (\mathfrak{g}^n / \mathfrak{g}^{n+1}) \otimes_{A/\mathfrak{g}} (M / \mathfrak{g}M) \to \mathfrak{g}^n M / \mathfrak{g}^{n+1} M
$$
and a graded homomorphism of degree 0 of graded gr(A)-modules
$$
\gamma_M : \mathrm{gr}(A) \otimes_{\mathrm{gr}_0(A)} \mathrm{gr}_0(M) \to \mathrm{gr}(M)
$$
whose restriction to $ \mathrm{gr}_n(A) \otimes_{\mathrm{gr}_0(A)} \mathrm{gr}_0(M) $ is $ \gamma_n $ for all $ n $ and which is therefore surjective.

#### Theorem 1 {#ac-iii-s5-thm-1 .statement}

Let A be a commutative ring, $ \mathfrak{g} $ an ideal of A and M an A-module. Consider the following properties:
(i) M is afat A-module.
(ii) $ \mathrm{Tor}_1^A(N, M) = 0 $ for every A-module N annihilated by $ \mathfrak{z} $.
(iii) $ M / \mathfrak{g}M $ is ajlat $ (A / \mathfrak{g}) $-module and the canonical mapping $ \mathfrak{z} \otimes_A M \to \mathfrak{g}M $ is bijective (the latter condition being equivalent to $ \mathrm{Tor}_1^A(A / \mathfrak{g}, M) = 0 $ by virtue of the relation $ \mathrm{Tor}_1^A(A, M) = 0 $ and the exact sequence
$$
\mathrm{Tor}_1^A(A, M) \to \mathrm{Tor}_1^A(A / \mathfrak{g}, M) \to \mathfrak{z} \otimes_A M \to M ).
$$
(iv) $ M / \mathfrak{g}M $ is ajlat $ (A / \mathfrak{g}) $-module and the canonical homomorphism
$$
\gamma_M : \mathrm{gr}(A) \otimes_{\mathrm{gr}_0(A)} \mathrm{gr}_0(M) \to \mathrm{gr}(M)
$$
is bijective (property (GR) of \S 2, no. 8).
(v) For all $ n \geq 1 $, $ M / \mathfrak{g}^n M $ is a flat $ (A / \mathfrak{g}^n) $-module.
Then (i) $ \Rightarrow $ (ii) $ \Leftrightarrow $ (iii) $ \Rightarrow $ (iv) $ \Leftrightarrow $ (v).
If further $ \mathfrak{g} $ is nilpotent or if A is Noetherian and M is ideally Hausdorff, properties (i), (ii), (iii), (iv) and (v) are equivalent.

#### Remark {#ac-iii-s5-n1-rem-1 .statement}

If $ A / \mathfrak{g} $ is a field (as often happens in applications) the condition "M/ $ \mathfrak{g}M $ is a flat $ (A / \mathfrak{g}) $-module" holds automatically for every A-module M, which simplifies the statement of properties (iii) and (iv); moreover, in this case, property (v) is equivalent to saying that $ M / \mathfrak{g}^n M $ is a free $ (A / \mathfrak{g}^n) $-module for every integer $ n \geq 1 $ (Chapter 11, \S 3, no. 2, Corollary 2 to Proposition 5).

### 3. PROOF OF THE FLATNESS CRITERION

(A) *The implications* (i) $ \Rightarrow $ (ii) $ \Leftrightarrow $ (iii)

The implication (i) $ \Rightarrow $ (ii) is immediate (Chapter I, § 4). The equivalence (ii) $ \Leftrightarrow $ (iii) is a special case of Chapter I, § 4, Proposition 2 applied to $ R = A, S = A/\mathfrak{g}, F = M, E = N $, taking account of the fact that being given an $(A/\mathfrak{g})$-module structure on $ N $ is equivalent to being given an $ A $-module structure under which $ N $ is annihilated by 3.

*Remark* (1). Condition (ii) is also equivalent to the following:

(ii') $ \operatorname{Tor}_1^A(N, M) = 0 $ *for every* $ A $*-module* $ N $ *annihilated by a power of* 3.

Clearly (ii') implies (ii). Conversely, if (ii) holds, then in particular $ \operatorname{Tor}_1^A(\mathfrak{g}^n N / \mathfrak{g}^{n+1} N, M) = 0 $ for all $ n $; from the exact sequence
$$
0 \to \mathfrak{g}^{n+1} N \to \mathfrak{g}^n N \to \mathfrak{g}^n N / \mathfrak{g}^{n+1} N \to 0
$$
we derive the exact sequence
$$
\operatorname{Tor}_1^A(\mathfrak{g}^{n+1} N, M) \to \operatorname{Tor}_1^A(\mathfrak{g}^n N, M) \to \operatorname{Tor}_1^A(\mathfrak{g}^n N / \mathfrak{g}^{n+1} N, M)
$$
and, as there exists an integer $ m $ such that $ \mathfrak{g}^m N = 0 $, we deduce by descending induction on $ n $ that $ \operatorname{Tor}_1^A(\mathfrak{g}^n N, M) = 0 $ for all $ n \leq m $ and in particular for $ n = 0 $.

It follows from this that if 9 is *nilpotent*, (ii) implies (i), for (ii') then means that $ \operatorname{Tor}_1^A(N, M) = 0 $ for *every* $ A $*-module* $ N $ and hence that $ M $ is flat (Chapter I, § 4).

(B) Let us prove the following proposition:

#### Proposition 1 {#ac-iii-s5-prop-1 .statement}

*Let* $ A $ *be a commutative ring, 3 an ideal of* $ A $ *and* $ M $ *an* $ A $*-module*. *The following conditions are equivalent*:
(a) *For all* $ n \geq 1 $, $ \operatorname{Tor}_1^A(A/\mathfrak{g}^n, M) = 0 $.
(b) *For all* $ n \geq 1 $, *the canonical homomorphism*
$$
\theta_n : \mathfrak{g}^n \otimes_A M \to \mathfrak{g}^n M
$$
*is bijective*.

*Moreover these conditions imply* :
(c) *The canonical homomorphism* $ \gamma_M : \operatorname{gr}(A) \otimes_{\operatorname{gr}_0(A)} \operatorname{gr}_r(M) \to \operatorname{gr}(M) $ *is bijective*. *Conversely, if* $ \mathfrak{g} $ *is nilpotent, (c) implies (a) and (b)*.

The equivalence of (a) and (b) follows from the exact sequence
$$
0 = \operatorname{Tor}_1^A(A, M) \to \operatorname{Tor}_1^A(A/\mathfrak{g}^n, M) \to \mathfrak{g}^n \otimes_A M \to M.
$$

Consider next the diagram
$$
\begin{array}{ccccccccc}
\mathfrak{g}^{n+1} \otimes_A M & \longrightarrow & \mathfrak{g}^n \otimes_A M & \longrightarrow & (\mathfrak{g}^n / \mathfrak{g}^{n+1}) \otimes_A (M / \mathfrak{g} M) & \longrightarrow & 0 \\
\downarrow \theta_{n+1} & & \downarrow \theta_n & & \downarrow \gamma_n & & \\
0 & \longrightarrow & \mathfrak{g}^{n+1} M & \longrightarrow & \mathfrak{g}^n M & \longrightarrow & \operatorname{gr}_n(M) & \longrightarrow & 0
\end{array}
$$

where we note that $ (\mathfrak{g}^n/\mathfrak{g}^{n+1}) \otimes_A (M/\mathfrak{g}M) $ is canonically identified with $ (\mathfrak{g}^n/\mathfrak{g}^{n+1}) \otimes_{A/\mathfrak{g}} (M/\mathfrak{g}M) $. This diagram is commutative by definition of $ \gamma_n $ and its rows are exact. If (b) holds, $ 0 $, and $ \theta_{n+1} $ are bijective and so therefore is $ \gamma_n $ by definition of cokernel, hence (b) implies (c). Conversely, assuming that $ \mathfrak{g} $ is nilpotent, let us show that (c) implies (b); we shall argue by descending induction on $ n $, since $ \mathfrak{g}^n \otimes_A M = \mathfrak{g}^n M = 0 $ for $ n $ sufficiently large. Suppose then that in diagram (1), $ \gamma_n $ and $ \theta_{n+1} $ are bijective; then so is $ \theta_n $ by virtue of Chapter I, § 1, no. 4, Corollary 1 to Proposition 2.

(C) *The implication* (ii) $ \Rightarrow $ (iv)

If (ii) holds, so does (ii') by *Remark* 1; Proposition 1 then shows that $ \gamma_M $ is an isomorphism. On the other hand, we already know that (ii) implies (iii) and hence $ M/\mathfrak{g}M $ is a flat $ (A/\mathfrak{g}) $-module, which completes the proof that (ii) implies (iv).

*Remark* (2). Proposition 1 shows that, if $ \mathfrak{g} $ is nilpotent, (iv) implies (iii); taking account of *Remark* 1, we have therefore proved in this case that (i), (ii), (iii) and (iv) are equivalent.

(D) *The equivalence* (iv) $ \Leftrightarrow $ (v)

For all $ n \geq 1 $, $ M/\mathfrak{g}^n M $ has a canonical $ (A/\mathfrak{g}^n) $-module structure. If it is filtered by the $ (\mathfrak{g}/\mathfrak{g}^n) $-adic filtration, it is immediate that $ \mathrm{gr}_m(M/\mathfrak{g}^n M) = \mathrm{gr}_m(M) $ if $ m < n $ and $ \mathrm{gr}_m(M/\mathfrak{g}^n M) = 0 $ if $ m \geq n $. For all $ k \geq 1 $, let $ A_k = A/\mathfrak{g}^k $, $ \mathfrak{g}_k = \mathfrak{g}/\mathfrak{g}^k $, $ M_k = M/\mathfrak{g}^k M $; let (iv), (resp. $ (v)_k $) denote the assertion derived from (iv) (resp. (v)) by replacing $ A, \mathfrak{g}, M $ by $ A_k, \mathfrak{g}_k, M_k $. It follows from what has just been said that (iv) is equivalent to "for all $ k \geq 1 $, $ (iv)_k $" and obviously (v) is equivalent to "for all $ k \geq 1 $, $ (v)_k $". Then it will suffice to establish the equivalence $ (iv)_k \Leftrightarrow (v)_k $ for all $ k $ or also to show that (iv) $ \Leftrightarrow $ (v) when $ 3 $ is *nilpotent*. Now (*Remark* 2) we have seen that in that case (iv) is equivalent to (i). As $ M/\mathfrak{g}^n M $ is isomorphic to $ M \otimes_A (A/\mathfrak{g}^n) $, (i) implies (v) (Chapter I, § 2, no. 7, Corollary 2 to Proposition 8); moreover clearly (v) then implies (i). We have therefore shown the equivalence (iv) $ \Leftrightarrow $ (v) in all cases and also that of all the properties of the theorem in the case where $ 3 $ is nilpotent.

(E) *The implication* (v) $ \Rightarrow $ (i) *when* $ A $ *is Noetherian and* $ M $ *ideally Hausdorff*

It is sufficient to prove that for every ideal $ a $ of $ A $ the canonical mapping $ j : a \otimes_A M \to M $ is *injective* (Chapter I, § 2, no. 3, Proposition 1). Let $ x \in \mathrm{Ker}\, j $;
$ a \otimes_A M $ is Hausdorff with the $ \mathfrak{g} $-adic topology, it suffices to verify that, for every integer $ n > 0 $, $ x \in \mathfrak{g}^n(a \otimes_A M) $. Let $ f : \mathfrak{g}^n a \to a $ be the canonical injection; it suffices to show that $ x \in \mathrm{Im}(f \otimes 1_M) $; for if $ b \in \mathfrak{g}^n $, $ a \in a $ and $ m \in M $, the image under $ f \otimes 1 $, of the element $ (ba) \otimes m $ of $ (\mathfrak{g}^n a) \otimes_A M $ is the element $ (ba) \otimes m = b(a \otimes m) $ of $ a \otimes_A M $ and hence $ \mathrm{Im}(f \otimes 1_M) \subset \mathfrak{g}^n(a \otimes_A M) $. By virtue of Krull's Theorem (§ 3, no. 2, Theorem 2), there exists an integer $ k $ such that $ a_j = a \cap \mathfrak{g}^k \subset \mathfrak{g}^n a $; if $ i : a_j \to a $ is the canonical injection, it will then be sufficient to show that $ x \in \operatorname{Im}(i \otimes 1_M) $. Now, denoting by $ p : a \to a/a_k $ and $ h : a/a_k \to A/\mathfrak{g}^k $ the canonical mappings, there is a commutative diagram

$$
\begin{array}{ccccccccc}
a_k \otimes_A M & \xrightarrow{i \otimes 1_M} & a \otimes_A M & \xrightarrow{p \otimes 1_M} & (a/a_k) \otimes_A M & \longrightarrow & 0 \\
& & \downarrow & & \downarrow h \otimes 1_M & & \\
& & M & \longrightarrow & (A/\mathfrak{g}^k) \otimes_A M & &
\end{array}
$$

in which the first row is exact. It suffices to prove that $ x \in \operatorname{Ker}(p \otimes 1_M) $ and, as $ x \in \operatorname{Ker} j $ by hypothesis, it will suffice to verify that the mapping $ h \otimes 1_1 $, is injective. Now, it may also be written (Algebra, Chapter II, § 3, no. 6, Corollary 3 to Proposition 6)

$$
h \otimes 1_{M/\mathfrak{g}^k M} : (a/a_k) \otimes_{A/\mathfrak{g}^k} (M/\mathfrak{g}^k M) \to M/\mathfrak{g}^k M
$$

and, as $ h $ is injective and, by (v), $ M/\mathfrak{g}^k M $ is a flat $ (A/\mathfrak{g}^k) $-module, this completes the proof.

### 4. APPLICATIONS

#### Proposition 2 {#ac-iii-s5-prop-2 .statement}

Let $ A $ be a commutative ring, $ \mathfrak{g} $ an ideal of $ A $ and $ B $ a commutative Noetherian $ A $-algebra such that $ B $ is contained in the Jacobson radical of $ B $. Then every finitely generated $ B $-module $ M $ is an ideally Hausdorff $ A $-module with respect to $ \mathfrak{g} $.

We shall see more generally that for every finitely generated $ A $-module $ N $, $ N \otimes_A M $ is Hausdorff with the $ 3 $-adic topology. For $ N_{(B)} = N \otimes_A B $ is a finitely generated $ B $-module and the $ B $-module $ N \otimes_A M $ is canonically identified with $ N_{,,} \otimes_B M $ by virtue of the associativity of the tensor product. Let $ \mathfrak{L} $ be the Jacobson radical of $ B $; as $ \mathfrak{g} B $ is contained in $ \mathfrak{L} $, the $ \mathfrak{g} $-adic topology on $ N \otimes_A M $ is therefore identified with a finer topology than the $ \mathfrak{L} $-adic topology on $ N_{(B)} \otimes_B M $; but this latter topology is Hausdorff since $ N_{,,} \otimes_B M $ is a finitely generated $ B $-module (no. 1, Example 1), whence the conclusion.

#### Proposition 3 {#ac-iii-s5-prop-3 .statement}

Let $ A $ be a commutative ring, $ B $ a commutative $ A $-algebra, $ \mathfrak{g} $ an ideal of $ A $ and $ M $ a $ B $-module. Suppose that $ B $ is a Noetherian ring and a flat $ A $-module and that $ M $ is ideally Hausdorff with respect to $ \mathfrak{g} B $. The following conditions are equivalent:
(a) $ M $ is a flat $ B $-module.
(b) $ M $ is a flat $ A $-module and $ M/\mathfrak{g} M = M/(\mathfrak{g} B) M $ is a flat $ (B/\mathfrak{g} B) $-module.
If further the canonical homomorphism $ A/\mathfrak{g} \to B/\mathfrak{g} B $ is bijective, conditions (a) and (b) are also equivalent to:
(c) $ M $ is a flat $ A $-module.

Condition (a) implies (b) by Chapter I, §2, no. 7, Corollaries 2 and 3 to Proposition 8 and the fact that $ M/\mathfrak{g} M $ is isomorphic to $ M \otimes_B (B/\mathfrak{g} B) $. Suppose condition (b) holds; to show that $ M $ is a flat $ B $-module, we shall apply Theorem 1 of no. 2 with $ A $ replaced by $ B $ and $ \mathfrak{g} $ by $ \mathfrak{g} B $. It will therefore be sufficient to show that the canonical mapping $ f : \mathfrak{J}B \otimes_B M \to \mathfrak{J}M $ is injective. Let $ f_1 $ be the canonical mapping $ \mathfrak{J} \otimes_A B \to \mathfrak{J}B $ and $ f_2 $ the canonical isomorphism $ \mathfrak{J} \otimes_A M \to (\mathfrak{J} \otimes_A B) \otimes_B M ; f \circ (f_1 \circ 1_M) \circ f_2 $ is the canonical mapping $ f' : \mathfrak{J} \otimes_A M \to \mathfrak{J}M $, as is easily verified. Now $ f' $ is an isomorphism since $ M $ is a flat $ A $-module, whilst $ f_1 $ is an isomorphism because $ B $ is flat over $ A ; f $ is then an isomorphism.

Let $ p : A/\mathfrak{J} \to B/\mathfrak{J}B $ be the canonical homomorphism; the $ (A/\mathfrak{J}) $-module structure on $ M/\mathfrak{J}M $ derived by means of $ p $ from its $ (B/\mathfrak{J}B) $-module structure is isomorphic to that on $ M \otimes_A (A/\mathfrak{J}) $. Then it follows that, if $ M $ is a flat $ A $-module, $ M/\mathfrak{J}M $ is a flat $ (A/\mathfrak{J}) $-module and hence also a flat $ (B/\mathfrak{J}B) $-module if $ p $ is an isomorphism; we have thus proved that (c) $ \Rightarrow $ (b) in that case.

#### Corollary {#ac-iii-s5-n4-cor-1 .statement}

*Let $ A $ be a commutative Noetherian ring, $ \mathfrak{J} $ an ideal of $ A $, $ \hat{A} $ the Hausdorff completion of $ A $ with respect to the $ \mathfrak{J} $-adic topology and $ M $ an ideally Hausdorff $ \hat{A} $-module with respect to $ \mathfrak{J} \hat{A} $. For $ M $ to be a flat $ A $-module, it is necessary and sufficient that $ M $ be a flat $ \hat{A} $-module.*

We know in fact that $ \hat{A} $ is a Noetherian ring ($ \S 3 $, no. **4**, Proposition 8) and a flat $ A $-module ($ \S 3 $, no. **4**, Theorem 3), that $ \mathfrak{J} \hat{A} = \hat{\mathfrak{J}} $ ($ \S 2 $, no. 12, Proposition **16**) and that the canonical homomorphism $ A/\mathfrak{J} \to \hat{A}/\hat{\mathfrak{J}} $ is bijective ($ \S 2 $, no. 12, Proposition 15); Proposition **3** can therefore be applied.

#### Proposition 4 {#ac-iii-s5-prop-4 .statement}

*Let $ A $ and $ B $ be two commutative Noetherian rings, $ h : A \to B $ a ring homomorphism, $ 3 $ an ideal of $ A $ and $ 2 $ an ideal of $ B $ containing $ \mathfrak{J}B $ and contained in the Jacobson radical of $ B $. Let $ \hat{A} $ be the Hausdorff completion of $ A $ with respect to the $ 3 $-adic topology and $ \hat{B} $ the Hausdorff completion of $ B $ with respect to the $ 2 $-adic topology; $ h $ is continuous with these topologies and $ h : \hat{A} \to \hat{B} $ therefore makes $ \mathbf{8} $ into an $ \hat{A} $-algebra. Let $ M $ be a finitely generated $ B $-module and $ \hat{M} $ its Hausdorff completion with respect to the $ 2 $-adic topology; the following properties are equivalent:
(a) $ M $ is a flat $ A $-module.
(b) $ \hat{M} $ is a flat $ A $-module.
(c) $ \hat{M} $ is a flat $ \hat{A} $-module.*

As $ B $ with the $ 2 $-adic topology is a Zariski ring, $ \hat{B} $ is a faithfully flat $ B $-module ($ \S 3 $, no. 5, Proposition 9) and $ M $ is canonically isomorphic to $ M \otimes_B \hat{B} $ ($ \S 3 $, no. **4**, Theorem 3); it is immediately verified that this canonical isomorphism is an isomorphism of the $ A $-module structure on $ \hat{M} $ onto the $ A $-module structure on $ M \otimes_B \hat{B} $ derived from that on $ M $. Applying Proposition 4 of Chapter I, $ \S 3 $, no. 2 with $ R $ replaced by $ B $, $ S $ by $ A $, $ E $ by $ \hat{B} $, $ F $ by $ M $, we see that for $ M $ to be a flat $ A $-module, it is necessary and sufficient that $ \hat{M} $ be a flat $ A $-module. Moreover, $ \hat{M} $ is a finitely generated $ \hat{B} $-module and $ \mathfrak{J} \hat{B} $ is contained in $ \mathfrak{Q} = \mathfrak{Q} \hat{B} $ and hence in the Jacobson radical of $ \hat{B} $ ($ \S 3 $, no. **4**, Proposition 8); therefore $ \hat{M} $ is an ideally Hausdorff $ A $-module with respect to $ \mathfrak{J} \hat{A} $ (Proposition 2). Conditions (b) and (c) are therefore equivalent by the Corollary to Proposition 3.

### Exercises {#ac-iii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
