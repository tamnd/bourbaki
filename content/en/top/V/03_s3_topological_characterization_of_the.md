---
book: top
book_title: General Topology
chapter: V
chapter_title: One-parameter groups
section: 3
section_title: Topological characterization of the groups R and T
lang: en
source: top-v-x
pdf_pages: 0023-0025, 0031-0034
extraction: ocr
statements: 5
exercises: 1
content_sha256: d8eafb662de42224e3be882319afed0add9e2505ad6b120528d7ea1bc667db2f
---

## 3. TOPOLOGICAL CHARACTERIZATION OF THE GROUPS $ \mathbf{R} $ AND $ \mathbf{T} $

#### Theorem 1 {#top-v-s3-thm-1 .statement}

*A topological group* $ G $ *in which there exists a neighbourhood of the identity element homeomorphic to an open interval of* $ \mathbf{R} $ *is locally isomorphic to* $ \mathbf{R} $.

The significance of this theorem is that it allows us to deduce, from a purely topological property of a group $ G $, a property of the *group structure* of $ G $.

We are concerned here with a phenomenon which is peculiar to the group $ \mathbf{R} $ and has no analogue for the groups $ \mathbf{R}^n $ when $ n > 1 $ (cf. Chapter VIII, § 1, no. 4). Groups locally isomorphic to $ \mathbf{R} $ are sometimes called *one-parameter groups*.

To prove Theorem 1 we shall reduce it to Proposition 2 of § 2. By hypothesis, there is a homeomorphism $ \varphi $ of an open neighbourhood $ U $ of the identity element $ e $ of $ G $ onto an open interval in $ \mathbf{R} $. By means of the inverse of the mapping $ \varphi $ we can transport to $ U $ the linear order structure of the interval $ \varphi(U) $; the topology of $ U $ (induced by that of $ G $) then has a base consisting of all the open intervals of $ U $ (Chapter

We show that, if x, y, z belong to V, the relation x < y implies xz < yz and zx < zy. Indeed, the functions f_1(z) = φ(yz) − φ(xz) and f_2(z) = φ(zy) − φ(zx) are continuous on V; they are > 0 for z = e and do not vanish in V [e.g., if we had φ(yz) = φ(xz), we should have yz = xz and therefore y = x]. Since f_1(V) and f_2(V) are connected (Chapter I, § 11, no. 2, Proposition 4) and are therefore intervals in R (Chapter IV, § 2, no. 5, Theorem 4), and since these intervals each contain a number > 0 and do not contain 0, they are contained in R^*_+ : that is, we have f_1(z) > 0 and f_2(z) > 0 for all z ∈ V.

If x and y are two elements of V such that x ≥ e and y ≥ e, then in particular we have xy ≥ e. Let E denote the (linearly ordered) set of elements of U which are ≥ e, and let I denote the set of elements of V which are ≥ e; then the axioms (GR_I), (GR_{II}), (GR_{IIIa}) and (GR_{IVa}) of § 2 are satisfied (taking ω to be the element e, and the law of composition to be that of the group G). This is clear for (GR_I), (GR_{II}) and (GR_{IVa}), from what precedes. As to (GR_{IIIa}), it is enough to remark that, if e < x < y (x ∈ V, y ∈ V), we have x^{-1} ∈ V, hence x^{-1} < e < x^{-1}y and x^{-1}y < y; consequently z = x^{-1}y belongs to I and we have xz = y. By Proposition 2 of § 2 there exists therefore a strictly increasing mapping f of I onto an interval of R, with left-hand end-point 0, such that f(e) = 0 and f(xy) = f(x) + f(y) whenever x, y and xy belong to I (which will be the case whenever x and y belong to W ∩ I, W being a neighbourhood of e such that W.W ⊂ V).

For every element x ∈ V which does not belong to I we have x < e, hence x^{-1} > e; consequently we can extend f to a strictly increasing mapping $ \overline{f} $ of V onto an interval of R by putting $ \overline{f}(x) = -f(x^{-1}) $ for all x < e in V. The inverse image under $ \overline{f} $ of an open interval contained in $ \overline{f}(V) $ is an open interval of V, so that $ \overline{f} $ is continuous on V; conversely, the image under $ \overline{f} $ of an open interval of V is an open interval of $ \overline{f}(V) $, and therefore $ \overline{f} $ is a homeomorphism of V onto a neighbourhood of 0 in the group R. On the other hand, it is easily checked (as in Proposition 6 of § 1, no. 4, by considering the various possible cases) that we have $ \overline{f}(xy) = \overline{f}(x) + \overline{f}(y) $ whenever x, y and xy all belong to V; and we therefore conclude that $ \overline{f} $, restricted to a suitable neighbourhood of e in G, is a local isomorphism of G with R (Chapter III, § 1, no. 3, Proposition 3).

Q.E.D.

#### Theorem 2 {#top-v-s3-thm-2 .statement}

*A connected group* $ G $ *in which there exists a neighbourhood of the identity element homeomorphic to an open interval of* $ \mathbf{R} $ *is isomorphic to either* $ \mathbf{R} $ *or* $ \mathbf{T} $.

This is an immediate consequence of the preceding theorem, together with Proposition 7 of § 1, no. 4.

#### Remark 1 {#top-v-s3-rem-1 .statement}

To decide whether a group $ G $ which satisfies the conditions of Theorem 2 is isomorphic to $ \mathbf{T} $ or to $ \mathbf{R} $, it is enough to see whether $ G $ is compact or not.

#### Remark 2 {#top-v-s3-rem-2 .statement}

Theorem 2 shows in particular that every topological group which is *homeomorphic* to the group $ \mathbf{R} $ *is necessarily isomorphic* to $ \mathbf{R} $.

#### Remark 3 {#top-v-s3-rem-3 .statement}

The preceding topological characterization of the groups $ \mathbf{R} $ and $ \mathbf{T} $ involves the topological space $ \mathbf{R} $ as an auxiliary set. It is possible to characterize the topological group structures of $ \mathbf{R} $ and $ \mathbf{T} $ by means of axioms which do not involve any auxiliary set (see Exercises 4 and 5).

### Exercises {#top-v-s3-exercises}

See the [exercises for § 3](exercises/s3/).
