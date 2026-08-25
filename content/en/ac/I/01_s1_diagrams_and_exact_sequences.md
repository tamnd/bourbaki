---
book: ac
book_title: Commutative Algebra
chapter: I
chapter_title: FLAT MODULES
section: 1
section_title: Diagrams and exact sequences
lang: en
source: ac-i-vii
book_pages: 1-9, 39-40
pdf_pages: 0021-0029, 0059-0060
extraction: ocr
subsections:
    - "no": 1
      title: DIAGRAMS
      page: 1
      pdf_page: 21
    - "no": 2
      title: COMMUTATIVE DIAGRAMS
      page: 2
      pdf_page: 22
    - "no": 3
      title: EXACT SEQUENCES
      page: 3
      pdf_page: 23
    - "no": 4
      title: THE SNAKE DIAGRAM
      page: 4
      pdf_page: 24
statements: 7
exercises: 7
content_sha256: 6790203cdd252786a633208363d3c57f4b6c7b2af0a1176438dd8ea954363ad2
---

## 1. DIAGRAMS AND EXACT SEQUENCES

### 1. DIAGRAMS

Let, for example, $A, B, C, D, E$ be five sets and let $f$ be a mapping from $A$ to $B$, $g$ a mapping from $B$ to $C$, $h$ a mapping from $D$ to $E$, $u$ a mapping from $B$ to $D$ and $v$ a mapping from $C$ to $E$. To summarize such a situation we often make use of diagrams; for example, the above situation is summarized by the following

(*) With the exception of § 4, the results of this chapter depend only on Books I to VI.

diagram (Set Theory, Chapter II, § 3, no. 4)

$$
\begin{array}{ccc}
A & \xrightarrow{f} & B \\
& & \downarrow u \\
& & D \\
& & \downarrow v \\
& & E \\
& & \xrightarrow{h}
\end{array}
$$

(1)

In such a diagram the group of symbols $A \xrightarrow{f} B$ expresses schematically the fact that $f$ is a mapping from $A$ to $B$. Where there is no ambiguity about $f$, we suppress the letter $f$ and write simply $A \to B$.

When $A, B, C, D, E$ are groups (resp. commutative groups) and $f, g, h, u, v$ group homomorphisms, diagram (1) is called, by way of abbreviation, a diagram of groups (resp. commutative groups).

In principle, a diagram is not a mathematical object, but only a figure designed to facilitate reading an argument. In practice, diagrams are often used as abbreviatory symbols to avoid naming all the sets and mappings under consideration; we therefore say "Consider the diagram (1)" instead of saying "Let A, B, C, D, E be five sets ... and $v$ a mapping from C to E"; see for example the statement of Proposition 2 in no. 4.

### 2. COMMUTATIVE DIAGRAMS

Consider, for example, the following diagram:

$$
\begin{array}{cccccc}
A & \xrightarrow{f} & B & \xrightarrow{g} & C & \xrightarrow{h} & D \\
a \downarrow & & b \downarrow & & c \downarrow & & d \downarrow \\
A' & \xrightarrow{f'} & B' & \xrightarrow{g'} & C' & \xrightarrow{h'} & D'
\end{array}
$$

(2)

To every path composed of a certain number of segments of the diagram traversed in the direction shown by the arrows corresponds a mapping of the set represented by the beginning of the first segment to the set represented by the end of the last segment, namely the composition of the mappings represented by the various segments traversed. For each vertex of the diagram, for example B, by way of convention there is a path reduced to B, to which corresponds the identity mapping 1,

In (2) there are for example three paths beginning at $A$ and ending at $C'$; the corresponding mappings are $c \circ g \circ f, g' \circ b \circ f$ and $g' \circ f' \circ a$. A diagram is said to be commutative if, for every pair of paths in the diagram with the same beginning and end, the two corresponding mappings are equal; in particular if the beginning and end of a path coincide the corresponding mapping must be the identity.

For the diagram (2) to be commutative it is necessary and sufficient that the relations
$$
f' \circ a = b \circ f, \quad g' \circ b = c \circ g, \quad h' \circ f = d \circ h;
$$
hold; in other words, it is necessary and sufficient that the three square diagrams contained in (2) be commutative. For the relations (3) imply $c \circ g \circ f = g' \circ b \circ f$ since $c \circ g = g' \circ b$, and $g' \circ b \circ f = g' \circ f' \circ a$ since $b \circ f = f' \circ a$; thus the three paths beginning at $A$ and ending at $C'$ give the same mapping. It can be similarly verified that the four paths beginning at $A$ and ending at $D'$ (resp. the three paths beginning at $B$ and ending at $D'$) give the same mapping. The relations (3) signify that the two paths beginning at $A$ (resp. B, C) and ending at $B'$ (resp. C', D') give the same mapping. None of the other pairs of vertices of (2) can be joined by more than one path and the diagram (2) is therefore commutative.

In what follows we shall leave the reader to verify analogous results for other types of diagrams.

### 3. EXACT SEQUENCES

Recall the following definition (Algebra, Chapter II, § 1, no. 4):

#### Definition 1 {#ac-i-s1-def-1 .statement}

Let $A$ be a ring, $F, G, H$ three right (resp. left) $A$-modules, $f$ a homomorphism of $F$ to $G$ and $g$ a homomorphism of $G$ to $H$. The ordered pair $(f, g)$ is called an exact sequence if $\overline{g}^{-1}(0) = f(F)$, that is if the kernel of $g$ is equal to the image of $f$.

The diagram
$$
\begin{array}{ccc}
F & \xrightarrow{f} & G \\
& & \xrightarrow{g} \\
& & H
\end{array}
$$
is also called an exact sequence.

Consider similarly a diagram consisting of four modules and three homomorphisms:
$$
E \xrightarrow{f} F \xrightarrow{g} G \xrightarrow{h} H.
$$
This diagram is said to be exact at $F$ if the diagram $E \xrightarrow{f} F \xrightarrow{g} G$ is an exact sequence; it is said to be exact at $G$ if $F \xrightarrow{g} G \xrightarrow{h} H$ is an exact sequence. If (5) is exact at $F$ and $G$, it is said to be exact or also an exact sequence. Exact sequences with any number of terms are similarly defined.

Recall the following results (loc. cit.), where $E, F, G$ denote right (resp. left)

A-modules, the arrows represent homomorphisms and $0$ denotes a module reduced to its identity element:

(a) To say that $0 \to E \xrightarrow{f} F$ is an exact sequence is equivalent to saying that $f$ is injective.

(b) To say that $E \xrightarrow{f} F \to 0$ is an exact sequence is equivalent to saying that $f$ is surjective.

(c) To say that $0 \to E \xrightarrow{f} F \to 0$ is an exact sequence is equivalent to saying that $f$ is bijective, that is that $f$ is an isomorphism of $E$ onto $F$.

(d) If $F$ is a submodule of $E$ and $i$ denotes the canonical injection of $F$ into $E$ and $p$ the canonical surjection of $E$ onto $E/F$, the diagram
$$
\begin{array}{cccccc}
0 & \longrightarrow & F & \xrightarrow{i} & E & \xrightarrow{p} & E/F \longrightarrow 0
\end{array}
$$
is an exact sequence.

(e) Iff: $E \to F$ is a homomorphism, the diagram
$$
\begin{array}{cccccc}
0 & \longrightarrow & f^{-1}(0) & \xrightarrow{i} & E & \xrightarrow{f} & F & \xrightarrow{p} & F/f(E) \longrightarrow 0
\end{array}
$$
(where $i$ is the canonical injection off $(0)$ into $E$ and $p$ the canonical projection of $F/f(E)$) is an exact sequence.

(f) For the diagram
$$
\begin{array}{ccc}
E & \xrightarrow{f} & F & \xrightarrow{g} & G
\end{array}
$$
to be an exact sequence, it is necessary and sufficient that there exist modules $S$, $T$ and homomorphisms $a : E \to S$, $b : S \to F$, $c : F \to T$ and $d : T \to G$ such that $f = b \circ a$, $g = d \circ c$ and the three sequences
$$
\begin{array}{ccc}
E & \xrightarrow{a} & S & \longrightarrow & 0 \\
0 & \longrightarrow & S & \xrightarrow{b} & F & \xrightarrow{c} & T & \longrightarrow & 0 \\
0 & \longrightarrow & T & \xrightarrow{d} & G
\end{array}
$$
be exact.

Recall finally that iff: $E \to F$ is an A-module homomorphism, we set $\operatorname{Ker}(f) = f^{-1}(0)$, $\operatorname{Im}(f) = f(E)$, $\operatorname{Coim}(f) = E/f^{-1}(0)$ and $\operatorname{Coker}(f) = F/f(E)$. With this notation it is possible to take, in (9), $S = \operatorname{Im}(f) = \operatorname{Ker}(g)$ and $T = \operatorname{Im}(g)$ (canonically isomorphic to $\operatorname{Coker}(f)$).

### 4. THE SNAKE DIAGRAM

#### Proposition 1 {#ac-i-s1-prop-1 .statement}

Consider a commutative diagram of commutative groups:
$$
\begin{array}{ccc}
A & \xrightarrow{u} & B & \xrightarrow{v} & C \\
a \downarrow & & b \downarrow & & c \downarrow \\
A' & \xrightarrow{u'} & B' & \xrightarrow{v'} & C'
\end{array}
$$

Suppose that the two rows of (10) are exact. Then:

(i) If c is injective, we have

(11) $\operatorname{Im}(b) \cap \operatorname{Im}(u') = \operatorname{Im}(u' \circ a) = \operatorname{Im}(b \circ u).$

(ii) If a is surjective, we have

(12) $\operatorname{Ker}(b) + \operatorname{Im}(u) = \operatorname{Ker}(v' \circ b) = \operatorname{Ker}(c \circ v).$

Let us prove (i). Clearly

$$
\operatorname{Im}(u' \circ a) = \operatorname{Im}(b \circ u) \subset \operatorname{Im}(b) \cap \operatorname{Im}(u').
$$

Conversely, let $x \in \operatorname{Im}(b) \cap \operatorname{Im}(u')$. There exists $y \in B$ such that $x = b(y)$. As $v' \circ u' = 0$, we have $0 = v'(x) = v'(b(y)) = c(v(y))$, whence $v(y) = 0$ since c is injective. As $(u, v)$ is an exact sequence, there exists $z \in A$ such that $y = u(z)$, whence $x = b(u(z))$.

Let us prove (ii). As $v \circ u = 0$ and $v' \circ u' = 0$, it is clear that

$$
\operatorname{Ker}(b) + \operatorname{Im}(u) \subset \operatorname{Ker}(v' \circ b) = \operatorname{Ker}(c \circ v).
$$

Conversely, let $x \in \operatorname{Ker}(v' \circ b)$. Then $b(x) \in \operatorname{Ker}(v')$ and there exists $y' \in A'$ such that $u'(y') = b(x)$, since the sequence $(u', v')$ is exact. As a is surjective, there exists $y \in A$ such that $a(y) = y'$, whence $b(x) = u'(a(y)) = b(u(y))$; it follows that $x - u(y) \in \operatorname{Ker}(b)$, which completes the proof.

#### Lemma 1 {#ac-i-s1-lem-1 .statement}

Consider a commutative diagram of commutative groups:

$$
\begin{array}{ccc}
A & \xrightarrow{u} & B \\
a \downarrow & & b \downarrow \\
A' & \xrightarrow{u'} & B'
\end{array}
$$

Then there exists one and only one homomorphism $u_1 : \operatorname{Ker}(a) \to \operatorname{Ker}(b)$ and one and only one homomorphism $u_2 : \operatorname{Coker}(a) \to \operatorname{Coker}(b)$ such that the diagrams

$$
\begin{array}{ccc}
\operatorname{Ker}(a) & \xrightarrow{u_1} & \operatorname{Ker}(b) \\
i \downarrow & & j \downarrow \\
A & & B
\end{array}
$$

and

$$
\begin{array}{ccc}
A' & \xrightarrow{u'} & B' \\
p \downarrow & & q \downarrow \\
\operatorname{Coker}(a) & \xrightarrow{u_2} & \operatorname{Coker}(b)
\end{array}
$$

are commutative, i and j denoting the canonical injections and p and q the canonical surjections.

If $x \in \mathrm{Ker}(a)$, then $a(x) = 0$ and $b(u(x)) = u'(a(x)) = 0$, hence $u(x) \in \mathrm{Ker}(b)$, and the existence and uniqueness of $u_1$ are then immediate. Similarly, we have $u'(a(A)) = b(u(A)) \subset b(B)$, then by taking quotients $u'$ gives a homomorphism $u_2 : \mathrm{Coker}(a) + \mathrm{Coker}(b)$, which is the only homomorphism for which (15) is commutative.

Let us now start with the *commutative* diagram (10) of commutative groups; there corresponds to it by Lemma 1 a diagram

$$
\begin{array}{ccccccccc}
\mathrm{Ker}(a) & \xrightarrow{u_1} & \mathrm{Ker}(b) & \xrightarrow{v_1} & \mathrm{Ker}(c) \\
i \downarrow & & j \downarrow & & k \downarrow \\
A & \xrightarrow{u} & B & \xrightarrow{v} & C \\
a \downarrow & & b \downarrow & & c \downarrow \\
A' & \longrightarrow & B' & \longrightarrow & C' \\
\vdots & & \vdots & & \vdots \\
\cdots \to \mathrm{Coker}(a) & \xrightarrow{u_2} & \mathrm{Coker}(b) & \xrightarrow{v_2} & \mathrm{Coker}(c)
\end{array}
$$

where $i, j, k$ are the canonical injections, $p, q, r$ the canonical surjections and $u_1, u_2$ (resp. $v_1, v_2$) the homomorphisms canonically associated with $u, u'$ (resp. $v, u'$) by Lemma 1. It is immediately verified that this diagram is commutative.

#### Proposition 2 {#ac-i-s1-prop-2 .statement}

*Suppose that in the commutative diagram (10) the sequences $(u, v)$ and $(u', u')$ are exact. Then:*

(i) $v_1 \circ u_1 = 0$; if $u'$ is injective, the sequence $(u_1, v_1)$ is exact.
(ii) $v_2 \circ u_2 = 0$; if $v$ is surjective, the sequence $(u_2, v_2)$ is exact.
(iii) *Suppose that $u'$ is injective and $v$ is surjective. Then there exists one and only one homomorphism $d : \mathrm{Ker}(c) \to \mathrm{Coker}(a)$ with the following property: if $x \in \mathrm{Ker}(c)$, $y \in B$ and $t' \in A'$ satisfy the relations $v(y) = k(x)$ and $u'(t') = b(y)$, then $d(x) = p(t')$. Moreover the sequence*

(*) $$
\begin{array}{cccccc}
\mathrm{Ker}(a) & \xrightarrow{u_1} & \mathrm{Ker}(b) & \xrightarrow{v_1} & \mathrm{Ker}(c) & \xrightarrow{d} \\
& & & & & \\
& & & & & \\
& & & & & \\
\mathrm{Coker}(a) & \xrightarrow{u_2} & \mathrm{Coker}(b) & \xrightarrow{v_2} & \mathrm{Coker}(c)
\end{array}
$$

is exact.

Let us prove (i). As $u_1$ and $v_1$ have the same graphs as the restrictions of $u$ and $v$ to $\mathrm{Ker}(a)$ and $\mathrm{Ker}(b)$ respectively, we have $v_1 \circ u_1 = 0$. Then
$$
\mathrm{Ker}(v_1) = \mathrm{Ker}(b) \cap \mathrm{Ker}(v) = \mathrm{Ker}(b) \cap \mathrm{Im}(u) = \mathrm{Im}(j) \cap \mathrm{Im}(u).
$$
But, by Proposition 1, (i), $\mathrm{Ker}(v_1) = \mathrm{Im}(j \circ u_1) = \mathrm{Im}(u_1)$ if $u'$ is injective.

Let us prove (ii). As $u_2$ and $v_2$ are obtained from $u$ and $v$ by taking quotients, it is clear that $v_2 \circ u_2 = 0$. Suppose that $v$ is surjective; as $q$ and $p$ are surjective, it follows from the hypotheses and Proposition 1, (ii) that
$$
\begin{align*}
\mathrm{Ker}(v_2) &= q(\mathrm{Ker}(v_2 \circ q)) = q(\mathrm{Ker}(v') + \mathrm{Im}(b)) = q(\mathrm{Ker}(v')) = q(\mathrm{Im}(u')) \\
&= \mathrm{Im}(q \circ u') = \mathrm{Im}(u_2 \circ p) = \mathrm{Im}(u_2).
\end{align*}
$$

Finally let us prove (iii). For $x \in \mathrm{Ker}(c)$ there exists $y \in B$ such that $v(y) = k(x)$ since $v$ is surjective; moreover $v'(b(y)) = c(k(x)) = 0$ and consequently there exists a *unique* $t' \in A'$ such that $u'(t') = b(y)$, since $u'$ is injective. We now show that the element $p(t') \in \mathrm{Coker}(a)$ is *independent* of the element $y \in B$ such that $v(y) = k(x)$. For if $y' \in B$ is another element such that $v(y') = k(x)$, then $y' = y + u(z)$, where $z \in A$; we show that if $t'' \in A'$ is such that $u'(t'') = b(y')$ then $t'' = t' + a(z)$; for
$$
u'(t' + a(z)) = u'(t') + u'(a(z)) = b(y) + b(u(z)) = b(y + u(z)) = b(y').
$$
Finally, it follows that $p(t'') = p(t') + p(a(z)) = p(t')$. Then it is possible to set $d(x) = p(t')$ and the mapping $d : \mathrm{Ker}(c) \to \mathrm{Coker}(a)$ has thus been defined.

If now $x_1, x_2$ are elements of $\mathrm{Ker}(c)$ and $x = x_1 + x_2$, we take elements $y_1, y_2$ of $B$ such that $v(y_1) = k(x_1)$ and $v(y_2) = k(x_2)$ and choose for $y \in B$ the element $y_1 + y_2$; it is then immediate that $d(x) = d(x_1) + d(x_2)$ and hence $d$ is a *homomorphism*.

Suppose that $x = v_1(x')$ for some $x' \in \mathrm{Ker}(b)$; then take $y \in B$ to be the element $j(x')$. As $b(j(x')) = 0$, it follows that $d(x) = 0$, hence $d \circ v_1 = 0$. Conversely, suppose that $d(x) = 0$. In the above notation we then have $t' = a(s)$, where $s \in A$. In this case we have $b(y) = u'(t') = u'(a(s)) = b(u(s))$, or $b(y - u(s)) = 0$. The element $y - u(s)$ is therefore of the form $j(n)$, where $n \in \mathrm{Ker}(b)$, and we have $k(x) = v(y) = v(u(s) + j(n)) = v(j(n)) = k(v_1(n))$; as $k$ is injective, $x = v_1(n)$, which proves that the sequence (*) is exact at $\mathrm{Ker}(c)$.

Finally, we have (always in the same notation)
$$
u_2(d(x)) = u_2(p(t')) = q(u'(t')) = q(b(y)) = 0
$$
and hence $u_2 \circ d = 0$. Conversely, suppose that an element $w = p(t')$ of $\mathrm{Coker}(a)$ is such that $u_2(w) = u_2(p(t')) = 0$ (where $t' \in A$). Then $q(u'(t')) = 0$ and consequently $u'(t') = b(y)$ for some $y \in B$; as $v'(u'(t')) = 0$, we have $v'(b(y)) = 0$, hence $c(v(y)) = 0$, in other words $v(y) = k(x)$ for some $x \in \mathrm{Ker}(c)$, and by definition $w = d(x)$, which shows that the sequence (*) is exact at

Coker(a). It has been seen in (i) that it is exact at Ker(b) and in (ii) it is exact at Coker(b), which completes the proof of (iii).

#### Remark {#ac-i-s1-n4-rem-1 .statement}

If the groups of the diagram (10) are all (for example, right) modules over a ring $\mathbf{A}$ and the homomorphisms are A-module homomorphisms, it is soon verified that the homomorphism d defined in Proposition 2, (iii) is also a A-module homomorphism: if $x \in \mathrm{Ker}(c)$ and $a \in \Lambda$, and $y \in B$ is such that $v(y) = k(x)$, it is sufficient to note that $v(ya) = k(xa)$.

#### Corollary 1 {#ac-i-s1-prop-2-cor-1 .statement}

Suppose that the diagram (10) is commutative and the two rows are exact. Then:

(i) If $u'$, a and c are injective, b is injective.
(ii) If v, a and c are surjective, b is surjective.

Assertion (i) is a consequence of assertion (i) of Proposition 2: for $\mathrm{Ker}(a) = 0$ and $\mathrm{Ker}(c) = 0$, hence $\mathrm{Ker}(b) = 0$.

Assertion (ii) is a consequence of assertion (ii) of Proposition 2: for $\mathrm{Coker}(a) = 0$ and $\mathrm{Coker}(c) = 0$, hence $\mathrm{Coker}(b) = 0$.

#### Corollary 2 {#ac-i-s1-prop-2-cor-2 .statement}

Suppose that the diagram (10) is commutative and the two rows are exact. Under these conditions:

(i) If b is injective and if a and v are surjective, then c is injective.
(ii) If b is surjective and if c and $u'$ are injective, then a is surjective.

To prove (i) consider the diagram

$$
\begin{array}{ccc}
u(A) & \xrightarrow{w} & B & \xrightarrow{v} & C \\
a' \downarrow & & b \downarrow & & c \downarrow \\
u'(A') & \xrightarrow{w'} & B' & \xrightarrow{v'} & C'
\end{array}
$$

where $a'$ is the mapping with the same graph as the restriction of b to $u(A)$ and w and $w'$ are the canonical injections; clearly this diagram is commutative and its rows exact. Moreover $w'$ is injective and by hypothesis v is surjective; then by Proposition 2, (iii) we have an exact sequence

$$
0 = \mathrm{Ker}(b) \longrightarrow \mathrm{Ker}(c) \xrightarrow{d} \mathrm{Coker}(a') = 0
$$

since b is injective and $a'$ is surjective; whence $\mathrm{Ker}(c) = 0$.

To prove (ii) consider the diagram

$$
\begin{array}{ccc}
A & \xrightarrow{u} & B & \xrightarrow{w} & v(B) \\
a' \downarrow & & b \downarrow & & c' \downarrow \\
A' & \xrightarrow{w'} & B' & \xrightarrow{\sigma'} & v'(B')
\end{array}
$$

where this time $c'$ is the mapping with the same graph as the restriction of c to v(B) and w and w' have respectively the same graphs as v and v'; this diagram is commutative and its rows exact. Moreover w is surjective and by hypothesis u' is injective; then by Proposition 2, (iii) we have an exact sequence

$$
0 = \operatorname{Ker}(c') \xrightarrow{d} \operatorname{Coker}(a) \longrightarrow \operatorname{Coker}(b) = 0
$$

since b is surjective and c' is injective; whence Coker (a) = 0.

### Exercises {#ac-i-s1-exercises}

See the [exercises for § 1](exercises/s1/).
