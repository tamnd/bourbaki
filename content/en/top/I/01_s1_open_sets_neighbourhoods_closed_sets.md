---
book: top
book_title: General Topology
chapter: I
chapter_title: Topological Structures
section: 1
section_title: Open sets, neighbourhoods, closed sets
lang: en
source: top-i-iv
pdf_pages: 0023-0031, 0123-0125
extraction: ocr
subsections:
    - "no": 1
      title: OPEN SETS
      page: 0
      pdf_page: 23
    - "no": 2
      title: NEIGHBOURHOODS
      page: 0
      pdf_page: 24
    - "no": 3
      title: FUNDAMENTAL SYSTEMS OF NEIGHBOURHOODS; BASES OF A TOPOLOGY
      page: 0
      pdf_page: 27
    - "no": 4
      title: CLOSED SETS
      page: 0
      pdf_page: 27
    - "no": 5
      title: LOCALLY FINITE FAMILIES
      page: 0
      pdf_page: 28
    - "no": 6
      title: INTERIOR, CLOSURE, FRONTIER OF A SET; DENSE SETS
      page: 0
      pdf_page: 29
statements: 23
exercises: 9
content_sha256: caad119969fe95e177cdfb89bfa13ff8d0159e399ab5d7c4149c74762c8819a5
---

## 1. OPEN SETS, NEIGHBOURHOODS, CLOSED SETS

### 1. OPEN SETS

#### Definition 1 {#top-i-s1-def-1 .statement}

*A topological structure* (or, more briefly, *a topology*) *on a set* $ X $ *is a structure given by a set* $ \mathcal{D} $ *of subsets of* $ X $, *having the following properties* (called *axioms of topological structures*):

(O_I) *Every union of sets of* $ \mathcal{D} $ *is a set of* $ \mathcal{D} $.

(O_{II}) *Every finite intersection of sets of* $ \mathcal{D} $ *is a set of* $ \mathcal{D} $.

*The sets of* $ \mathcal{D} $ *are called open sets of the topological structure defined by* $ \mathcal{D} $ *on* $ X $.

#### Definition 2 {#top-i-s1-def-2 .statement}

*A topological space is a set endowed with a topological structure*.

The elements of a topological space are often called *points*. When a topology has been defined on a set $ X $, this set is said to be the set *underlying* the topological space $ X $.

Axiom (O_I) implies in particular that the union of the empty subset of $ \mathcal{D} $, i.e. the *empty set* belongs to $ \mathcal{D} $. Axiom (O_{II}) implies that the intersection of the empty subset of $ \mathcal{D} $, i.e. *the set* $ X $, belongs to $ \mathcal{D} $.

To show that a set $ \mathcal{D} $ of subsets of $ X $ satisfies (O_{II}), it is often convenient to prove separately that it satisfies the following two axioms, whose conjunction is equivalent to (O_{II}):
(O_{II\ a}) *The intersection of two sets of* $ \mathcal{D} $ *belongs to* $ \mathcal{D} $.
(O_{II\ b}) $ X $ *belongs to* $ \mathcal{D} $.

Examples of topologies. Given any set $ X $, the set of subsets of $ X $ consisting of $ X $ and $ \varnothing $ satisfies axioms $ (O_1) $ and $ (O_{II}) $ and therefore defines a topology on $ X $. So does the set $ \mathcal{P}(X) $ of all subsets of $ X $: the topology it defines is the discrete topology on $ X $, and the set $ X $ with this topology is called a discrete space.

A covering $ (U_i)_{i \in I} $ of a subset $ A $ of a topological space $ X $ is said to be open if all the $ U_i $ are open in $ X $.

#### Definition 3 {#top-i-s1-def-3 .statement}

*A homeomorphism of a topological space $ X $ onto a topological space $ X' $ is an isomorphism of the topological structure of $ X $ onto that of $ X' $;* that is to say, in accordance with the general definitions *a bijection of $ X $ onto $ X' $ which transforms the set of open subsets of $ X $ into the set of open subsets of $ X' $*.

$ X $ and $ X' $ are said to be *homeomorphic* if there is a homeomorphism of $ X $ onto $ X' $.

#### Example {#top-i-s1-n1-exa-1 .statement}

If $ X $ and $ X' $ are two discrete spaces, any bijection of $ X $ onto $ X' $ is a homeomorphism.

The following criterion follows immediately from the definition of a homeomorphism: *for a bijection $ f $ of a topological space $ X $ onto a topological space $ X' $ to be a homeomorphism, it is necessary and sufficient that the image under $ f $ of each open set in $ X $ is an open set in $ X' $, and that the inverse image under $ f $ of each open set in $ X' $ is an open set in $ X $*.

### 2. NEIGHBOURHOODS

#### Definition 4 {#top-i-s1-def-4 .statement}

*Let $ X $ be a topological space and $ A $ any subset of $ X $. A neighbourhood of $ A $ is any subset of $ X $ which contains an open set containing $ A $. The neighbourhoods of a subset $ \{ x \} $ consisting of a single point are also called neighbourhoods of the point $ x $*.

It is clear that every neighbourhood of a subset $ A $ of $ X $ is also a neighbourhood of each subset $ B \subset A $; in particular, it is a neighbourhood of each point of $ A $. Conversely, suppose $ A $ is a neighbourhood of each of the points of a set $ B $, and let $ U $ be the union of the open sets contained in $ A $; then $ U \subset A $, and since each point of $ B $ belongs to an open set contained in $ A $, we have $ B \subset U $; but $ U $ is open by virtue of $ (O_1) $, hence $ A $ is a neighbourhood of $ B $. In particular:

#### Proposition 1 {#top-i-s1-prop-1 .statement}

*A set is a neighbourhood of each of its points if and only if it is open.*

The everyday sense of the word "neighbourhood" is such that many of the properties which involve the mathematical idea of neighbourhood appear as the mathematical expression of intuitive properties; the choice of this term thus has the advantage of making the language more expressive. For this purpose it is also permissible to use the expressions "sufficiently near" and "as near as we please" in some statements. For example, Proposition 1 can be stated in the following form: a set $ A $ is open if and only if, for each $ x \in A $, all the points *sufficiently near* $ x $ belong to $ A $. More generally, we shall say that a property holds for all points *sufficiently near* a point $ x $, if it holds at all points of some neighbourhood of $ x $.

Let us denote by $ \mathcal{B}(x) $ the set of all neighbourhoods of $ x $. The sets $ \mathcal{B}(x) $ have the following properties:

(V_I) *Every subset of $ X $ which contains a set belonging to $ \mathcal{B}(x) $ itself belongs to $ \mathcal{B}(x) $.*

(V_{II}) *Every finite intersection of sets of $ \mathcal{B}(x) $ belongs to $ \mathcal{B}(x) $.*

(V_{III}) *The element $ x $ is in every set of $ \mathcal{B}(x) $.*

Indeed, these three properties are immediate consequences of Definition 4 and axiom (O_{II}).

(V_{IV}) *If $ V $ belongs to $ \mathcal{B}(x) $, then there is a set $ W $ belonging to $ \mathcal{B}(x) $ such that, for each $ y \in W $, $ V $ belongs to $ \mathcal{B}(y) $.*

By Proposition 1, we may take $ W $ to be any open set which contains $ x $ and is contained in $ V $.

This property may be expressed in the form that *a neighbourhood of $ x $ is also a neighbourhood of all points sufficiently near to $ x $*.

These four properties of the sets $ \mathcal{B}(x) $ are *characteristic*. To be precise, we have:

#### Proposition 2 {#top-i-s1-prop-2 .statement}

*If to each element $ x $ of a set $ X $ there corresponds a set $ \mathcal{B}(x) $ of subsets of $ X $ such that the properties (V_I), (V_{II}), (V_{III}) and (V_{IV}) are satisfied, then there is a unique topological structure on $ X $ such that, for each $ x \in X $, $ \mathcal{B}(x) $ is the set of neighbourhoods of $ x $ in this topology.*

By Proposition 1, if there is a topology on $ X $ satisfying these conditions, the set of open sets for this topology is necessarily the set $ \mathcal{D} $ of subsets $ A $ of $ X $ such that *for each $ x \in A $ we have $ A \in \mathcal{B}(x) $*; hence the *uniqueness* of this topology if it exists.

The set $ \mathcal{D} $ certainly satisfies axioms (O_I) and (O_{II}): for (O_I), this follows immediately from (V_I), and for (O_{II}), from (V_{II}). It

![Diagram showing sets V, U, W, and points x, y, z](https://i.imgur.com/3Q5z5QG.png)

Figure 1.

remains to show that, in the topology defined by $ \mathcal{D} $, $ \mathcal{B}(x) $ is the set of neighbourhoods of $ x $ for each $ x \in X $. It follows from (V_I) that every neighbourhood of $ x $ belongs to $ \mathcal{B}(x) $. Conversely, let $ V $ be a set belonging to $ \mathcal{B}(x) $, and let $ U $ be the set of points $ y \in X $ such that $ V \in \mathcal{B}(y) $; if we can show that $ x \in U, U \subset V $ and $ U \in \mathcal{D} $, then the proof will be complete. We have $ x \in U $ since $ V \in \mathcal{B}(x) $; also $ U \subset V $, for every point $ y \in U $ belongs to $ V $ by reason of (V_III) and the hypothesis $ V \in \mathcal{B}(y) $. It remains to show that $ U \in \mathcal{D} $, i.e. that $ U \in \mathcal{B}(y) $ for each $ y \in U $; now (Fig. 1) if $ y \in U $ then by (V_IV) there is a set $ W $ such that for each $ z \in W $ we have $ V \in \mathcal{B}(z) $; since $ V \in \mathcal{B}(z) $ means that $ z \in U $, it follows that $ W \subset U $, and therefore, by (V_I), that $ U \in \mathcal{B}(y) $.

Q.E.D.

Proposition 2 shows that a topology on $ X $ can be defined by means of the sets $ \mathcal{B}(x) $ of neighbourhoods of points of $ X $, subject only to the axioms (V_I), (V_II), (V_III) and (V_IV).

#### Example {#top-i-s1-n2-exa-1 .statement}

We may define a topology on the set $ Q $ of rational numbers by taking for open sets all unions of bounded open intervals; the set of these subsets certainly satisfies (O_I), and to see that it satisfies (O_II) it is enough to remark that if the intersection of two open intervals $ ]a, b[ $ and $ ]c, d[ $ is not empty, then it is the interval $ ]\alpha, \beta[ $, where $ \alpha = \sup(a, c) $ and $ \beta = \inf(b, d) $. We get the same topology by defining for each $ x \in Q $ the set $ \mathcal{B}(x) $ of neighbourhoods of $ x $ to be the set of subsets containing an open interval to which $ x $ belongs. The topological space obtained by assigning this topology to $ Q $ is called the rational line (cf. Chapter IV, § 1, no. 2). Notice that in this space every open interval is an open set. \* We can define a topology on the set $ R $ of real numbers in the same way; $ R $ with this topology is called the real line (cf. § 2, Exercise 5 and Chapter IV, § 1, no. 3). \*

### 3. FUNDAMENTAL SYSTEMS OF NEIGHBOURHOODS; BASES OF A TOPOLOGY

#### Definition 5 {#top-i-s1-def-5 .statement}

In a topological space $ X $, a fundamental system of neighbourhoods of a point $ x $ (resp. of a subset $ A $ of $ X $) is any set $ \mathcal{G} $ of neighbourhoods of $ x $ (resp. $ A $) such that for each neighbourhood $ V $ of $ x $ (resp. $ A $) there is a neighbourhood $ W \in \mathcal{G} $ such that $ W \subset V $.

If $ \mathcal{G} $ is a fundamental system of neighbourhoods of a subset $ A $ of $ X $, then every finite intersection of sets of $ \mathcal{G} $ contains a set of $ \mathcal{G} $.

Examples. 1) In a discrete space (no. 1) the set $ \{ x \} $ alone constitutes a fundamental system of neighbourhoods of the point $ x $.
2) On the rational line $ \mathbf{Q} $ the set of all open intervals containing a point $ x $ is a fundamental system of neighbourhoods of this point. So is the set of open intervals $ ]x - 1/n, x + 1/n[ $, and the set of closed intervals $ [x - 1/n, x + 1/n] $, where $ n $ runs through all the integers $ > 0 $, or through any infinite strictly increasing sequence of integers $ > 0 $.
\* There are analogous results for the real line. \*

#### Definition 6 {#top-i-s1-def-6 .statement}

A base of the topology of a topological space $ X $ is any set $ \mathcal{B} $ of open subsets of $ X $ such that every open subset of $ X $ is the union of sets belonging to $ \mathcal{B} $.

#### Proposition 3 {#top-i-s1-prop-3 .statement}

If $ X $ is a topological space, then for a set $ \mathcal{B} $ of open subsets of $ X $ to be a base of the topology of $ X $ it is necessary and sufficient that for each $ x \in X $ the set of $ V \in \mathcal{B} $ such that $ x \in V $ is a fundamental system of neighbourhoods of $ x $.

It is clear that the condition is necessary. Conversely, if it is satisfied, then given any open set $ U $ and any $ x \in U $ there is an open set $ V_x \in \mathcal{B} $ such that $ x \in V_x \subset U $. The union of the sets $ V_x $ for $ x \in U $ is therefore equal to $ U $. This completes the proof.

#### Example 1 {#top-i-s1-n3-exa-1 .statement}

The discrete topology has as a base the set of subsets of $ X $ which consist of a single point.
2) The set of bounded open intervals is by definition a base of the topology of the rational line (no. 2). \* Likewise, the set of bounded open intervals is a base of the topology of the real line. \*

### 4. CLOSED SETS

#### Definition 7 {#top-i-s1-def-7 .statement}

In a topological space $ X $, the complements of the open sets of $ X $ are called closed sets.

Taking complements, we find that the axioms $(O_I)$ and $(O_{II})$ take the following form:

$(O'_I)$ *Every intersection of closed sets is a closed set.*

$(O'_{II})$ *Every finite union of closed sets is a closed set.*

The empty set and the whole space $X$ are closed (and therefore *both open and closed*; cf. § 11).

On the rational line, every interval of the form $[a, \rightarrow[$ is a closed set, for its complement ]\leftarrow, a[ is open; likewise, every interval of the form ]\leftarrow, a] is a closed set; hence so is every bounded closed interval $[a, b]$, since it is the intersection of the intervals $[a, \rightarrow[$ and ]\leftarrow, b].

The set $Z$ of rational integers is closed in the rational line, since its complement $\bigcup_{n \in Z} ]n, n+1[$ is open.

A *covering* $(F_i)_{i \in I}$ of a subset $A$ of a topological space $X$ is said to be *closed* if each of the $F_i$ is closed in $X$.

A *homeomorphism* $f$ of a topological space $X$ onto a topological space $X'$ (no. 1) can be characterized as a bijection of $X$ onto $X'$ *such that the image under $f$ of every closed subset of $X$ is a closed subset of $X'$ and the inverse image under $f$ of every closed subset of $X'$ is a closed subset of $X$*.

### 5. LOCALLY FINITE FAMILIES

#### Definition 8 {#top-i-s1-def-8 .statement}

*A family $(A_i)_{i \in I}$ of subsets of a topological space $X$ is said to be locally finite if for each $x \in X$ there is a neighbourhood $V$ of $x$ such that $V \cap A_i = \varnothing$ for all but a finite number of indices $i \in I$. A set $\mathcal{S}$ of subsets of $X$ is said to be locally finite if the family of subsets defined by the identity map of $\mathcal{S}$ onto itself is locally finite.*

It is clear that if $(A_i)_{i \in I}$ is a locally finite family of subsets and if $B_i \subset A_i$ for each $i \in I$, then the family $(B_i)_{i \in I}$ is locally finite.

Every *finite* family of subsets of a topological space $X$ is obviously locally finite; the converse is not true in general.

\* For example, in $\mathbf{R}$, the open covering formed by the interval ]\leftarrow, 1[ and the intervals ]$n, \rightarrow[$ for each integer $n \geqslant 0$ is locally finite; and each interval ]$n, \rightarrow[$ meets an infinite number of sets of this covering. \*

#### Proposition 4 {#top-i-s1-prop-4 .statement}

*The union of a locally finite family of closed subsets of a topological space $X$ is closed in $X$.*

Let $ (F_i)_{i \in I} $ be a locally finite family of closed subsets of $ X $, and suppose that $ x \in X $ does not belong to $ F = \bigcup_{i \in I} F_i $; then $ x $ has a neighbourhood $ V $ which meets only those $ F_i $ whose indices belong to a *finite* subset $ J $ of $ I $. For each $ i \in J $ let $ U_i $ be the complement of $ F_i $; then $ \complement F $ contains the set $ V \cap \bigcap_{i \in J} U_i $, which is a neighbourhood of $ x $ since each $ U_i $ is open and contains $ x $. Hence, by Proposition 1 of no. 2, $ \complement F $ is open and therefore $ F $ is closed in $ X $.

We note that the union of an *arbitrary* family of closed subsets of $ X $ is not necessarily closed; for example, on the rational line $ \mathbf{Q} $, the set $ ]2, 1[ $ is the union of the closed sets
$$
\left[ \frac{1}{n}, 1 - \frac{1}{n} \right] \quad \text{for } n > 2,
$$
but is not closed.

### 6. INTERIOR, CLOSURE, FRONTIER OF A SET; DENSE SETS

#### Definition 9 {#top-i-s1-def-9 .statement}

*In a topological space $ X $, a point $ x $ is said to be an interior point of a subset $ A $ of $ X $ if $ A $ is a neighbourhood of $ x $. The set of interior points of $ A $ is called the interior of $ A $ and is denoted by $ \dot{A} $.*

According to Definitions 9 and 4, a point $ x $ is an interior point of $ A $ if there is an open set contained in $ A $ which contains $ x $; it follows that $ \dot{A} $ is the union of all the open sets contained in $ A $, and hence is *the largest open set contained in* $ A $: in other words, if $ B $ is an *open* set contained in $ A $, then $ B \subset \dot{A} $. Consequently, if $ A $ and $ B $ are two subsets of $ X $ such that $ B \subset A $, then $ \dot{B} \subset \dot{A} $; and $ A $ is a neighbourhood of $ B $ if and only if $ B \subset \dot{A} $.

#### Remark {#top-i-s1-n6-rem-1 .statement}

The interior of a non-empty set can be empty; this is the case for a set consisting of a single point which is not open, for example on the rational line \* (or the real line) *.

Proposition 1 of no. 2 can be restated as follows:

*A set is open if and only if it coincides with its interior.*

The property $ (V_{II}) $ of no. 2 implies that every point which is an interior point of each of two subsets $ A $ and $ B $ is an interior point of $ A \cap B $; consequently
$$(1)$$ $$
\dot{A} \cap \dot{B} = \dot{A} \cap \dot{B}.
$$

Every point which is interior to the complement of a set $ A $ is said to be an *exterior* point of $ A $, and the set of these points is called the *exterior* of $ A $ in $ X $; a point $ x \in X $ which is an exterior point of $ A $ is therefore characterized by the property that *$ x $ has a neighbourhood which does not meet* $ A $.

#### Definition 10 {#top-i-s1-def-10 .statement}

*The closure of a subset* $ A $ *of a topological space* $ X $ *is the set of all points* $ x \in X $ *such that every neighbourhood of* $ x $ *meets* $ A $, *and is denoted by* $ \overline{A} $.

This definition can be reformulated by saying that a point $ x $ lies in the closure of a set $ A $ if there are points of $ A $ *as near* $ x $ *as we please to*.

Every point which is not in the closure of $ A $ is exterior to $ A $, and conversely; thus we have the formulae (which are duals of each other)

$$(2)$$
$$
\mathcal{C}\overline{A} = \widehat{\mathcal{C}}A,\qquad \mathcal{C}\dot{A} = \overline{\mathcal{C}}A.
$$

Hence, to any proposition on interiors of sets, there corresponds by *duality* a proposition on closures, and vice versa. In particular, the closure of a set $ A $ is *the smallest closed set which contains* $ A $; in other words, if $ B $ is a closed set such that $ A \subset B $, then $ \overline{A} \subset B $. If $ A $ and $ B $ are two subsets of $ X $ such that $ A \subset B $, then $ \overline{A} \subset \overline{B} $.

*A set is closed if and only if it coincides with its closure*.

The dual of formula (1) is

$$(3)$$
$$
\overline{A \cup B} = \overline{A} \cup \overline{B}.
$$

#### Proposition 5 {#top-i-s1-prop-5 .statement}

*Let* $ A $ *be an open set in* $ X $; *then for every subset* $ B $ *of* $ X $ *we have*

$$(4)$$
$$
A \cap \overline{B} \subset \overline{A \cap B}.
$$

For suppose $ x \in A \cap \overline{B} $; then if $ V $ is any neighbourhood of $ x $, $ V \cap A $ is a neighbourhood of $ x $, since $ A $ is open; hence $ V \cap A \cap B $ is not empty and therefore $ x $ lies in the closure of $ A \cap B $.

If $ x $ lies in the closure of $ A $ but not in $ A $, then every neighbourhood of $ x $ contains a point of $ A $ *other than* $ x $; but if $ x \in A $ it can happen that $ x $ has a neighbourhood which contains no point of $ A $ except $ x $. We say then that $ x $ is an *isolated point* of $ A $. In particular, $ x $ is isolated in the whole space $ X $ if and only if $ \{x\} $ is an open set.

A closed set which has no isolated points is called a *perfect* set.

#### Definition 11 {#top-i-s1-def-11 .statement}

In a topological space $ X $, a point $ x $ is said to be a frontier point of a set $ A $ if $ x $ lies in the closure of $ A $ and in the closure of $ \overline{CA} $. The set of frontier points of $ A $ is called the frontier of $ A $.

The frontier of $ A $ is therefore the set $ \overline{A} \cap \overline{\overline{CA}} $, which is closed. A frontier point $ x $ of $ A $ is characterized by the property that every neighbourhood of $ x $ contains at least one point of $ A $ and at least one point of $ \overline{CA} $; $ x $ may or may not belong to $ A $. The frontier of $ A $ is the same as the frontier of $ \overline{CA} $. The interior of $ A $, the exterior of $ A $ and the frontier of $ A $ are mutually disjoint and their union is the whole space $ X $.

#### Definition 12 {#top-i-s1-def-12 .statement}

A subset $ A $ of a topological space $ X $ is said to be dense in $ X $ (or simply dense, if there is no ambiguity about $ X $) if $ \overline{A} = X $, i.e. if every non-empty open set $ U $ of $ X $ meets $ A $.

#### Example {#top-i-s1-n6-exa-1 .statement}

* We shall see in Chapter IV, § 1 that the set of rational numbers and its complement are dense on the real line. *
In a discrete space $ X $ the only dense subset of $ X $ is $ X $ itself. On the other hand, every non-empty subset of $ X $ is dense in the topology on $ X $ for which the only open sets are $ \varnothing $ and $ X $.

#### Proposition 6 {#top-i-s1-prop-6 .statement}

If $ \mathcal{B} $ is a base of the topology of a topological space $ X $, there is a dense set $ D $ in $ X $ such that $ \mathrm{Card}(D) \leq \mathrm{Card}(\mathcal{B}) $.

We may restrict ourselves to the case in which none of the sets of $ \mathcal{B} $ is empty (the non-empty sets of $ \mathcal{B} $ already form a base of the topology of $ X $). For each $ U \in \mathcal{B} $, let $ x_V $ be a point of $ U $; it follows from Proposition 3 of no. 3 that the set $ D $ of the points $ x_U $ is dense in $ X $, and we have $ \mathrm{Card}(D) \leq \mathrm{Card}(\mathcal{B}) $ (Set Theory, Chapter III, § 3, no. 2, Proposition 3).

### Exercises {#top-i-s1-exercises}

See the [exercises for § 1](exercises/s1/).
