---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 1
section_title: Definition of real numbers
lang: en
source: top-i-iv
pdf_pages: 0335-0340, 0384-0387
extraction: ocr
subsections:
    - "no": 1
      title: THE ORDERED GROUP OF RATIONAL NUMBERS
      page: 0
      pdf_page: 335
    - "no": 2
      title: THE RATIONAL LINE
      page: 0
      pdf_page: 336
    - "no": 3
      title: THE REAL LINE AND REAL NUMBERS
      page: 0
      pdf_page: 337
    - "no": 4
      title: PROPERTIES OF INTERVALS IN $ \mathbf{R} $
      page: 0
      pdf_page: 338
    - "no": 5
      title: LENGTH OF AN INTERVAL
      page: 0
      pdf_page: 339
    - "no": 6
      title: ADDITIVE UNIFORMITY OF $\mathbf{R}$
      page: 0
      pdf_page: 340
statements: 10
exercises: 2
content_sha256: c8730b6ed3baf481340205505e89db2058463f5d870ee4ad6c6bb5892ecc991e
---

## 1. DEFINITION OF REAL NUMBERS

### 1. THE ORDERED GROUP OF RATIONAL NUMBERS

We have defined the ordering $ x \leq y $ on the set $ \mathbf{Q} $ of rational numbers; we have seen that this ordering makes $ \mathbf{Q} $ a *linearly ordered* set, and that it is *compatible* with the *additive group* structure of $ \mathbf{Q} $, i.e. for each $ z \in \mathbf{Q} $ the relation $ x \leq y $ is equivalent to $ x + z \leq y + z $ (that is, *the ordering is invariant under translations*). We recall the notation (which is used in any linearly ordered group)

$$
x^+ = \sup (x, 0), \\
x^- = \sup (-x, 0) = (-x)^+, \\
|x| = \sup (x, -x);
$$

$ |x| $ is called the *absolute value* of $ x $, and we have

$$
x = x^+ - x^-, \qquad |x| = x^+ + x^-
$$

and the *triangle inequality*

(1)
$$
|x + y| \leq |x| + |y|,
$$
together with the inequality
(2)
$$
||x| - |y|| \leq |x - y|
$$
which is an immediate consequence of (1); moreover
(3)
$$
|x^+ - y^+| \leq |x - y|.
$$

The relations $ x \geq 0,\ x = x^+,\ x^- = 0,\ |x| = x $ (resp. $ x \leq 0,\ x = -x^-,\ x^+ = 0,\ |x| = -x $) are *equivalent*. The relation $ |x| = 0 $ is equivalent to $ x = 0 $; if $ a \geq 0 $, the relation $ |x| \leq a $ is equivalent to $ -a \leq x \leq a $, and the relation $ |x| \geq a $ is equivalent to "$ x \geq a $ or $ x \leq -a $". For all $ x, y $ in $ \mathbf{Q} $, we have

(4)
$$
\sup (x, y) + z = \sup (x + z, y + z),
$$
(5)
$$
\inf (x, y) = - \sup (-x, -y),
$$

and, as particular cases,

(6)
$$
\sup (x, y) = x + (y - x)^+ = x + (x - y)^-,
$$
(7)
$$
\inf (x, y) = x - (y - x)^- = x - (x - y)^+.
$$

Finally, let $ \mathbf{Q}_+ $ denote the set of rational numbers $ \geq 0 $; we have then

(8)
$$
\mathbf{Q}_+ + \mathbf{Q}_+ \subset \mathbf{Q}_+,
$$
(9)
$$
\mathbf{Q}_+ \cap (- \mathbf{Q}_+) = \{ 0 \},
$$
(10)
$$
\mathbf{Q}_+ \cup (- \mathbf{Q}_+) = \mathbf{Q}.
$$

The relation $ x \leq y $ is *equivalent* to $ y - x \in \mathbf{Q}_+ $.

We shall use this ordering to define *a topology on $ \mathbf{Q} $ compatible with its additive group structure*.

### 2. THE RATIONAL LINE

Consider the set $ \mathfrak{F} $ of *symmetric open intervals* $ ]-a, +a[ $, where $ a $ runs through the set of rational numbers $ > 0 $; we shall show that $ \mathfrak{F} $ is a *fundamental system of neighbourhoods of* $ 0 $ in a topology compatible with the additive group structure of $ \mathbf{Q} $.

The group $ \mathbf{Q} $ is commutative, and axiom $ (\mathrm{GV}'_{\mathrm{II}}) $ is clearly satisfied; it is therefore enough to show that axiom $ (\mathrm{GV}'_{\mathrm{I}}) $ is also satisfied, in other words, that for each $ a > 0 $ there exists $ b > 0 $ such that the conditions $ |x| < b $ and $ |y| < b $ together imply $ |x + y| < a $. The triangle inequality shows that we may take $ b = a/2 $.

#### Definition 1 {#top-iv-s1-def-1 .statement}

*The rational line is the topological space consisting of the set $ \mathbf{Q} $ together with the additive group topology for which the symmetric open intervals $ ]-a, +a[ $ $ (a > 0) $ form a fundamental system of neighbourhoods of $ 0 $.*

*The topological group $ \mathbf{Q} $ thus defined is called the additive group of the rational line.*

If $ a $ is any rational number $ > 0 $, there is an integer $ n > 0 $ such that $ 1/n < a $; hence the open intervals $ ]-\frac{1}{n}, +\frac{1}{n}[ $ $ (n = 1, 2, \ldots) $ form a fundamental system of neighbourhoods of $ 0 $ on the rational line.

§ 1.3

We obtain a fundamental system of neighbourhoods of any point $ x \in \mathbf{Q} $ by taking the open intervals $ ]x - a, x + a[ $, where $ a $ runs through the set of rational numbers $ > 0 $ (or the set of numbers $ 1/n $).

Definition 1 is therefore equivalent to that given in Chapter I, § 1, no. 2.

For each pair of rational numbers $ (a, b) $ such that $ a < b $, there exists $ c \in \mathbf{Q} $ such that $ a < c < b $ [for example $ c = (a + b)/2 $]; it follows that the rational line is a non-discrete Hausdorff space.

For each $ a > 0 $, let $ U_a $ be the set of pairs $ (x, y) $ in $ \mathbf{Q} \times \mathbf{Q} $ such that $ |x - y| < a $. As $ a $ runs through the set of rational numbers $ > 0 $ (or just the set of numbers $ 1/n $), the sets $ U_a $ form a fundamental system of entourages of the uniformity of the additive group $ \mathbf{Q} $ of the rational line. Relations (2) and (3) show that $ |x|, x^+ $ and $ x^- $ are uniformly continuous on $ \mathbf{Q} $. It follows that the functions $ \sup(x, y) $ and $ \inf(x, y) $ are uniformly continuous on $ \mathbf{Q} \times \mathbf{Q} $.

### 3. THE REAL LINE AND REAL NUMBERS

#### Definition 2 {#top-iv-s1-def-2 .statement}

Let $ \mathbf{R} $ denote the topological group which is the completion of the additive group $ \mathbf{Q} $ of the rational line. The elements of $ \mathbf{R} $ are called real numbers; as a topological space, $ \mathbf{R} $ is called the real line; as a topological group, $ \mathbf{R} $ is called the additive group of the real line.

We shall always identify $ \mathbf{Q} $ with the dense subgroup of $ \mathbf{R} $ to which it is canonically isomorphic. With this convention, every rational number is a real number. Every real number which is not rational is said to be irrational; we have seen in Chapter II, § 3, no. 3 that such numbers exist (we shall show this in another way in § 3, no. 3 of this chapter; see also Exercise 2 to § 2); hence (Chapter III, § 2, no. 1) the set $ \mathbf{CQ} $ of irrational numbers is dense in $ \mathbf{R} $.

We shall show that the order structure of $ \mathbf{Q} $ can be extended to $ \mathbf{R} $ in such a way that the extended ordering is still compatible with the additive group structure of $ \mathbf{R} $:

#### Proposition 1 {#top-iv-s1-prop-1 .statement}

The relation $ y - x \in \overline{\mathbf{Q}}_+ $ is an ordering on $ \mathbf{R} $ which makes $ \mathbf{R} $ into a linearly ordered set; is compatible with the additive group structure on $ \mathbf{R} $, and induces the ordering $ x \leq y $ on $ \mathbf{Q} $.

We begin by showing that the relations $ y - x \in \overline{\mathbf{Q}}_+ $ and $ z - y \in \overline{\mathbf{Q}}_+ $ imply $ z - x \in \overline{\mathbf{Q}}_+ $. Indeed, the function $ x + y $ is continuous on $ \mathbf{R} \times \mathbf{R} $, and therefore by (8) we have $ \overline{\mathbf{Q}}_+ + \overline{\mathbf{Q}}_+ \subset \overline{\mathbf{Q}}_+ $ (Chapter I, § 2, no. 1, Theorem 1). Next, we shall show that the relations $ y - x \in \overline{\mathbf{Q}}_+ $ and $ x - y \in \overline{\mathbf{Q}}_+ $ imply $ x = y $; this will establish that $ y - x \in \overline{\mathbf{Q}}_+ $ is an

By (10), we have $ \overline{\mathbf{Q}}_+ \cup (-\overline{\mathbf{Q}}_+) = \mathbf{R} $, and hence $ \mathbf{R} $ is *linearly ordered* by the ordering $ y - x \in \overline{\mathbf{Q}}_+ $.

Furthermore, since the relations $ y - x \in \overline{\mathbf{Q}}_+ $ and $ (y + z) - (x + z) \in \overline{\mathbf{Q}}_+ $ are equivalent, the ordering $ y - x \in \overline{\mathbf{Q}}_+ $ is compatible with the additive group structure of $ \mathbf{R} $.

Finally, if $ x $ and $ y $ belong to $ \mathbf{Q} $ the relations $ y - x \in \overline{\mathbf{Q}}_+ $ and $ y - x \in \mathbf{Q}_+ $ are equivalent, and therefore the relation $ y - x \in \overline{\mathbf{Q}}_+ $ induces the relation $ x \leq y $ on $ \mathbf{Q} $. This completes the proof.

The relation $ y - x \in \overline{\mathbf{Q}}_+ $ is again denoted by $ x \leq y $. The set $ \overline{\mathbf{Q}}_+ $ is the set of all $ x \geq 0 $ in $ \mathbf{R} $ and is denoted by $ \mathbf{R}_+ $; it is a *closed set*. The set of all $ x > 0 $ is denoted by $ \mathbf{R}_+^* $; it is the complement of $ -\mathbf{R}_+ $ and is therefore *open* in $ \mathbf{R} $.

### 4. PROPERTIES OF INTERVALS IN $ \mathbf{R} $

#### Proposition 2 {#top-iv-s1-prop-2 .statement}

*Every closed (resp. open) interval in $ \mathbf{R} $ is a closed (resp. open) set in $ \mathbf{R} $.*

The sets $ [a, \to[ = a + \mathbf{R}_+ $ and $ ]\leftarrow, a] = a - \mathbf{R}_+ $ are obtained by translation from $ \mathbf{R}_+ $ and $ -\mathbf{R}_+ $ respectively and are therefore closed (Chapter III, § 1, no. 1); the sets $ ]\leftarrow, a[ $ and $ ]a, \to[, $ which are their complements, are open; finally, the closed interval $ [a, b] $ (resp. the open interval $ ]a, b[ $) is the intersection of $ [a, \to[ $ and $ ]\leftarrow, b] $ (resp. of $ ]a, \to[ $ and $ ]\leftarrow, b[ $) and is therefore a closed (resp. open) set.

The closed intervals $ [-a, +a] $ ($ a > 0 $) in $ \mathbf{R} $ are therefore neighbourhoods of 0. Let us show that they form a *fundamental system of neighbourhoods* of 0 as $ a $ runs through $ \mathbf{R}_+^* $. For this it is enough to establish the following proposition:

#### Proposition 3 {#top-iv-s1-prop-3 .statement}

*As $ r $ runs through the set of rational numbers $ > 0 $, the intervals $ s_r = [-r, +r] $ in $ \mathbf{R} $ form a fundamental system of neighbourhoods of 0.*

By Proposition 7 of Chapter III, § 3, no. 4 we obtain a fundamental system of neighbourhoods of 0 in $ \mathbf{R} $ by taking the *closures* in $ \mathbf{R} $ of the intervals

S_r \cap \mathbf{Q} = [-r, +r] \textit{of} \mathbf{Q}. The proof will be complete if we show that S_r is the closure of S_r \cap \mathbf{Q}. Now S_r is closed in \mathbf{R}, and we need therefore only prove that, if x is a real number such that -r < x < r, then x is in the closure of S_r \cap \mathbf{Q}. The interval ]-r, +r[ is an open set in \mathbf{R} and therefore for all sufficiently small neighbourhoods V of o in \mathbf{R} we have x + V \subset ]-r, +r[; but \mathbf{Q} being dense in \mathbf{R}, there is a rational number r' \in x + V, so that -r < r' < r and therefore r' \in S_r \cap \mathbf{Q}.

#### Corollary {#top-iv-s1-n4-cor-1 .statement}

*Every point of the real line has a countable fundamental system of neighbourhoods.*

#### Proposition 4 {#top-iv-s1-prop-4 .statement}

*If (x, y) is any pair of real numbers such that x < y, there is a rational number r such that x < r < y.*

Since \mathbf{Q} is dense in \mathbf{R}, it is enough to show that ]x, y[ is not empty; by translation we may assume x = 0 and y > 0. Now \mathbf{R} is a Hausdorff space and therefore, by Proposition 3, there is a rational number r > 0 such that y \notin ]-r, +r[, and this implies that 0 < r < y.

#### Proposition 5 {#top-iv-s1-prop-5 .statement}

*Let I be any interval in \mathbf{R}. Then the topology induced on I by the topology of \mathbf{R} is generated by the open intervals of I (where I is considered as linearly ordered by the relation x \leq y).*

Every open interval of I is the trace on I of an open interval of \mathbf{R}. This is clear for a bounded interval, and the unbounded interval ]a, \to[ of I is the trace of the unbounded interval ]a, \to[ of \mathbf{R}. We may therefore restrict ourselves to the case I = \mathbf{R}; but in this case the result follows from Proposition 3, since every neighbourhood of a point x \in \mathbf{R} contains an open interval ]x - a, x + a[.

#### Remark {#top-iv-s1-n4-rem-1 .statement}

If A is a dense subset of \mathbf{R}, the topology of \mathbf{R} is generated by the open intervals whose end-points belong to A. For if

$$ ]x - a, x + a[ $$

is an open interval containing x, there exist two points y, z of A such that x - a < y < x and x < z < x + a; hence ]y, z[ contains x and is contained in ]x - a, x + a[. This proof shows, moreover, that the intervals under consideration form a base (Chapter I, § 1, no. 3) of the topology of \mathbf{R}. In particular, if we take A = \mathbf{Q}, we see that the topology of \mathbf{R} has a countable base.

### 5. LENGTH OF AN INTERVAL

#### Definition 3 {#top-iv-s1-def-3 .statement}

*The length of a bounded interval with end-points a and b (a \leq b) is defined to be b - a.*

Every bounded interval which contains more than one point therefore has length > 0. If $ a \leq b $, the four intervals $[a, b], ]a, b[, [a, b[$ and $]a, b[$ all have the same length. An interval with end-points $a + c$ and $b + c$ has the same length as an interval with end-points $a$ and $b$; in other words, *the length of an interval is invariant under translation*.

If $a \leq c \leq d \leq b$ we have $d - c \leq b - a$. Hence if a bounded interval $I$ is contained in a bounded interval $I'$, the length of $I$ is less than or equal to the length of $I'$.

If $n$ mutually disjoint open intervals $I_1, I_2, \ldots, I_n$ are contained in the interval $[a, b]$ ($a < b$) it is easily seen by induction on $n$ that, if $I_k = ]c_k, d_k[$, there is a permutation $\sigma$ of the indices $k$ ($1 \leq k \leq n$) such that $d_{\sigma(k)} \leq c_{\sigma(k+1)}$ for $1 \leq k \leq n - 1$. It follows immediately that the sum of the lengths of the intervals $I_k$ is at most equal to the length of $[a, b]$, and that equality holds if and only if $c_{\sigma(1)} = a, d_{\sigma(n)} = b$ and $d_{\sigma(k)} = c_{\sigma(k+1)}$ for $1 \leq k \leq n - 1$.

### 6. ADDITIVE UNIFORMITY OF $\mathbf{R}$

Since the group $\mathbf{R}$ is linearly ordered, the functions $x^+, x^-$ and $|x|$ are defined on $\mathbf{R}$ in the same way as on $\mathbf{Q}$ and satisfy all the relations listed above for $\mathbf{Q}$, notably relations (1) to (7). Let $a$ be a real number > 0 and let $U_a$ be the set of all pairs $(x, y) \in \mathbf{R} \times \mathbf{R}$ such that $|x - y| < a$; as $a$ runs through the set of real numbers > 0 (or the set of numbers $1/n$), the sets $U_a$ form a fundamental system of entourages of the uniformity of the additive group $\mathbf{R}$ of the real line (called the *additive uniformity of the real line*).

The functions $|x|$, $x^+$ and $x^-$ are *uniformly continuous* on $\mathbf{R}$, and the functions $\sup(x, y)$ and $\inf(x, y)$ are *uniformly continuous* on $\mathbf{R} \times \mathbf{R}$; these functions therefore coincide with those obtained by extending by continuity the corresponding functions defined on $\mathbf{Q}$ and $\mathbf{Q} \times \mathbf{Q}$, respectively.

### Exercises {#top-iv-s1-exercises}

See the [exercises for § 1](exercises/s1/).
