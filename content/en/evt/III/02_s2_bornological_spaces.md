---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: SPACES OF CONTINUOUS LINEAR MAPPINGS
section: 2
section_title: Bornological spaces
lang: en
source: evt-i-v
book_pages: TVS III.11-TVS III.13, TVS III.40-TVS III.41
pdf_pages: 0143-0145, 0172-0173
extraction: ocr
statements: 6
exercises: 4
content_sha256: 0d07a448890f2831b0cc23b615935ec8e079f5380d64f4b62a604498fffec8be
---

## § 2. BORNOLOGICAL SPACES

In this paragraph, E denotes a locally convex space, and $\mathcal{B}$ its canonical bornology (III, p. 3, def. 5).

#### Lemma 1 {#evt-iii-s2-lem-1 .statement}

— *Let G be a semi-normed space, p its semi-norm, and u a linear mapping from G into E. The following conditions are equivalent* :

(i) *u is continuous* ;
(ii) *the image of the unit ball of G under u is bounded in E* ;
(iii) *for every sequence $(x_n)$ of points of G tending to 0, the sequence $(u(x_n))$ is bounded in E*.

It is immediate that (i) implies (ii) (III, p. 4, cor. 1) and that (ii) implies (iii). Let V be a neighbourhood of 0 in E ; if $u^{-1}(V)$ is not a neighbourhood of 0 in G, then there exists a sequence $(y_n)$ of points of $G - u^{-1}(V)$ such that $p(y_n) \leq \frac{1}{n^2}$. Hence the sequence $x_n = n y_n$ tends to 0 in G and $u(x_n) \notin nV$, which implies that the sequence $(u(x_n))$ is not bounded. Therefore (iii) implies (i).

*Proposition 1.* — *The following conditions are equivalent* :
(i) *Every semi-norm on E which is bounded on bounded subsets of E is continuous*.
(i') *Every convex balanced subset of E which absorbs the bounded subsets of E* (I, p. 7, def. 4) *is a neighbourhood of 0 in E*.
(ii) *E is the inductive limit of the semi-normed spaces $E_A$, where A ranges over the directed increasing set of closed, convex, balanced and bounded subsets of E*.
(ii') *There exists a family $(E_i)_{i \in I}$ of semi-normed spaces, and for every $i \in I$, a linear mapping $u_i : E_i \to E$ such that the topology of E is the finest locally convex topology for which the $u_i$ are continuous*.
(iii) *For an arbitrary locally convex space F, a linear mapping $u : E \to F$ is continuous if and only if for every sequence $(x_n)$ of points in E tending to 0, the sequence $(u(x_n))$ is bounded in F*.

(iii') *For an arbitrary semi-normed space F, a linear mapping u : E → F is continuous if and only if u(X) is bounded in F for every bounded set X in E.*

It is immediate that (i) and (i') are equivalent in view of the correspondence between semi-norms and convex, balanced, absorbent subsets (II, p. 20). If p is a semi-norm on E, which is continuous on each E_A, then p is bounded on bounded subsets of E; hence (i) implies (ii) (II, p. 27, prop. 5). It is clear that (ii) implies (ii').

Now let (E_i, u_i)_{i \in I} be as in (ii') and let u be a linear mapping from E into a locally convex space F, such that (u(x_n)) is bounded in F for every sequence (x_n) of points of E tending to 0. It follows from lemma 1 of III, p. 11 that the linear mapping u \circ u_i : E_i \to F is continuous for all i \in I. Hence, if the topology of E is the finest locally convex topology for which the u_i are continuous, then u is continuous (II, p. 27, prop. 5). This proves that (ii') implies (iii).

It is immediate that (iii) implies (iii') (III, p. 3, cor.) Finally, if p is a semi-norm on E, which is bounded on bounded subsets of E, the condition (iii') asserts that the identity map is continuous from E into the semi-normed space (E, p); in other words, p is continuous. This proves that (iii') implies (i).

#### Definition 1 {#evt-iii-s2-def-1 .statement}

*A locally convex space is said to be bornological if it satisfies the equivalent conditions of prop. 1.*

#### Example {#evt-iii-s2-n0-exa-1 .statement}

— 1) Every semi-normed space is bornological.
2) In particular, every finite dimensional locally convex space is bornological.
3) On account of the transitivity of final locally convex topologies (II, p. 28, cor. 2), we deduce at once from condition (ii') that if (E_i)_{i \in I} is a family of locally convex bornological spaces and if E is assigned the finest locally convex topology for which the linear mappings u_i : E_i \to E (for i \in I) are continuous, then E is bornological. In particular, *an inductive limit, a direct sum, a quotient space of bornological spaces are bornological spaces*.

On the other hand, a closed subspace of a bornological space is not necessarily bornological (IV, p. 63, exerc. 8).

#### Corollary {#evt-iii-s2-n0-cor-1 .statement}

*Every Hausdorff and semi-complete bornological space is an inductive limit of Banach spaces.*

In fact, the spaces E_A, where A is closed and bounded are Banach spaces (III, p. 8, corollary).

#### Proposition 2 {#evt-iii-s2-prop-2 .statement}

*A locally convex metrizable space is bornological.*

Suppose E is metrizable, and p a semi-norm on E which is bounded on bounded subsets of E, but which is not continuous. Let A be the set of all $x \in E$ such that $p(x) < 1$. Let $(V_n)_{n \geq 1}$ be a decreasing sequence forming a fundamental system of neighbourhoods of 0 in E. Since p is not continuous, A is not a neighbourhood of 0; hence for every $n > 0$, we have $A \not\supseteq n^{-1} V_n$ and there exists a point $x_n$ in $V_n$, such that $n^{-1} x_n \notin A$, that is, $p(x_n) \geq n$. The sequence $(x_n)$ tends to 0, hence is bounded (III, p. 3, corollary); this contradicts the hypothesis on p.

#### Corollary {#evt-iii-s2-n0-cor-2 .statement}

— *Every Fréchet space* (II, p. 24) *is the inductive limit of Banach spaces*.

### Exercises {#evt-iii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
