---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 9
section_title: 'Application: locally compact fields'
lang: en
source: ac-i-vii
book_pages: 431-434, 470-471
pdf_pages: 0449-0452, 0488-0489
extraction: ocr
subsections:
    - "no": 1
      title: THE MODULUS FUNCTION ON A LOCALLY COMPACT FIELD
      page: 431
      pdf_page: 449
    - "no": 2
      title: EXISTENCE OF REPRESENTATIVES
      page: 432
      pdf_page: 450
    - "no": 3
      title: STRUCTURE OF LOCALLY COMPACT FIELDS
      page: 433
      pdf_page: 451
statements: 10
exercises: 5
content_sha256: d6135c6e7390164e0213d8aebe0c179fa81f38f798cfd152a69cde189ff2353d
---

## 9. APPLICATION: LOCALLY COMPACT FIELDS

### 1. THE MODULUS FUNCTION ON A LOCALLY COMPACT FIELD

Let $K$ be a locally compact field (not necessarily commutative). Recall that the function mod (or mod,) has been defined (Integration, Chapter VII, § 1, no. 10, Definition 6) on $K$ as follows: $\operatorname{mod}_K(0) = 0$ and for $x \neq 0$ in $K$, the number $\operatorname{mod}_K(x)$ is the modulus of the automorphism $y \mapsto xy$ of the additive group of $K$.

#### Proposition 1 {#ac-vi-s9-prop-1 .statement}

*If $K$ is a locally compactfield, thefunction mod, belongs to $\mathcal{V}(K)$ (\S 6, no. 1). Moreover:*
(i) *If $s > 0$ is such that $(\operatorname{mod}_K)^s = g$ is an absolute value, then $g$ defines the topology on $K$.*
(ii) *If $K$ is not discrete and mod, is an ultrametric absolute value, there exists a normed discrete valuation $v$ on $K$ whose ring is compact and whose residuefield is finite with $q$ elements, so that $\operatorname{mod}, = q^{-v}$. The topology on $K$ is defined by $v$.*

This follows from \S 6, no. 1, Proposition 1, \S 5, no. 1, Proposition 2 and Integration, Chapter VII, § 1, no. 10, Propositions 12 and 13.

#### Proposition 2 {#ac-vi-s9-prop-2 .statement}

*Let $K, K'$ be two (not necessarily commutative) locally compact fields such that $K$ is a topological subfield of $K'$ and $K$ is not discrete. Then:*
(i) *$K'$ is a finite dimensional left (resp. right) vector space over $K$.*
(ii) *If $K$ is contained in the centre of $K'$, then, for all $x \in K'$.*
(1)
$$
\operatorname{mod}_{K'}(x) = \operatorname{mod}_K(N_{K'/K}(x)).
$$
As $K$ is a complete valued field which is not discrete, assertion (i) follows from Topological Vector Spaces, Chapter I, § 2, no. 4, Theorem 3; assertion (ii) is just Integration, Chapter VII, § 1, no. 11, Proposition 17.

#### Corollary 1 {#ac-vi-s9-prop-2-cor-1 .statement}

*Every locally compactfield whose centre is not discrete is of finite rank over its centre.*

The centre $Z$ of a locally compact field $K$ is closed in $K$ and therefore locally Compact.

#### Corollary 2 {#ac-vi-s9-prop-2-cor-2 .statement}

*Let $K'$ be a locally compact field and $K$ a closed subfield of $K'$ (neither necessarily commutative). If $K'$ is a left (resp. right) vector space of finite dimension $n$ over $K$, then*
(2)
$$
\operatorname{mod}_{K'}(x) = (\operatorname{mod}_K(x))^n \quad \text{for all } x \in K.
$$

In general it is known that in a (left or right) vector space of finite dimension $n$ over $K$, the homothety with ratio $x \in K$ has modulus equal to $(\mathrm{mod}_K(x))^n$; it suffices to apply this to $K'$.

### 2. EXISTENCE OF REPRESENTATIVES

#### Proposition 3 {#ac-vi-s9-prop-3 .statement}

*Let $K$ be a (not necessarily commutative) locally compact field which is not discrete and whose topology is defined by a discrete valuation $v$; let $A$ be the ring and $m$ the ideal of $v$ and let us write $\mathrm{Card}(A/m) = q = p^f$ (p prime). Then, there exists a system of representatives $S$ of $A/m$ in $A$ and a uniformizer $u$ for $v$ such that $O \in S$, $S^* = S \cap K^*$ is a cyclic subgroup of $K^*$ and $u^{-1} Su = S$. Moreover, every element of $A$ may be written uniquely in the form $\sum_{i=0}^\infty s_i u^i$, where $s_i \in S$.*

We shall use the following lemma:

#### Lemma 1 {#ac-vi-s9-lem-1 .statement}

*Let $x, y$ be two permutable elements of $A$ such that $x - y \in m^j \ (j \geq 1)$; then $x^{p^n} - y^{p^n} \in m^{j+n}$ for every integer $n \geq 0$.*

By induction on $n$, it is reduced to proving the lemma for $n = 1$. Then

$$
x^p - y^p = (x - y)(x^{p-1} + x^{p-2}y + \ldots + y^{p-1});
$$

the second factor is a sum of $p$ terms congruent to one another mod. $m$ and, as $A/m$ is of characteristic $p$, $p \cdot 1 \in m$ in $A$ and hence

$$
x^{p-1} + x^{p-2}y + \ldots + y^{p-1} \in m;
$$

whence $x^p - y^p \in m^{j+1}$.

We know that the multiplicative group $(A/m)^*$ is a cyclic group with $q - 1$ elements (*Algebra*, Chapter V, § 11, no. 1, Theorem 1); let $x$ be a representative in $A$ of a generator of this group; then $x^q - x \in m$, whence, by Lemma 1, $x^{q^{n+1}} - x^{q^n} \in m^{1+fn}$, since $x^q$ and $x$ are permutable. This proves that $(x^{q^n})_{n \geq 0}$ is a Cauchy sequence in $A$; as $A$ is compact and hence complete, this sequence has a limits in $A$ which obviously satisfies $s \equiv x \pmod{m}$ and $s^q = s$. As $s \neq 0$, $s^{q-1} = 1$, more precisely $s$ is a *primitive* $(q-1)$*-th root of unity* in $A$. Clearly the set $S$ consisting of $0$ and the powers $s^j \ (0 \leq j \leq q-2)$ is a *system of representatives* of the classes of $A$ mod. $m$ and is *invariant* under multiplication in $A$.

Now let $a$ be a uniformizer for $v$ and consider the inner automorphism $y \mapsto a^{-1}ya$ of $K$; it maps $A$ to itself, $m$ to itself and therefore, taking quotients, it defines an automorphism of the field $A/m$; it is known (*Algebra*, Chapter V, § 11, no. 4, Proposition 5) that such an automorphism is of the form $z \mapsto z^{p^r}$, where $0 \leq r \leq f-1$. Then $a^{-1}s^j a \equiv s^{jp^r} \pmod{m}$ for $0 \leq j \leq q-2$; as $a \in m$ and $s \notin m$, this implies that $s^{-j}as^{jp^r} \equiv a \pmod{m^2}$.

Let us write

$$
u = \sum_{i=0}^{q-2} s^{-1} a s^i p^r.
$$

Then $u \equiv (q - l) a \equiv -a (\text{mod. } m^2)$ since $p . 1 \in m$; we conclude that $u$ is also a uniformizer for $v$; moreover
(3)
$$
s^{-1} u s^{p^r} = u
$$
whence we deduce that $u^{-1} S u = S$.

Finally, for all $x \in A$ there exists a unique sequence $(s_i)$ ($i \in \mathbf{N}$) such that $s_i \in S$ for all $i$ and $x \equiv \sum s_i u^i$ (mod. $m^{n+1}$) for all $n \geq 0$: it is immediate by induction on $n$, every element $t$ of $m^{n+1}$ satisfying a relation of the form $t \equiv t' u^{n+1}$ (mod. $m^{n+2}$), where $t'$ is a uniquely determined element of $S$. Then $x = \sum_{i=0}^{\infty} s_i u^i$ and the family $(s_i)$ satisfying this relation and such that $s_i \in S$ for all $i$ is determined uniquely.

### 3. STRUCTURE OF LOCALLY COMPACT FIELDS

The completions $\mathbf{R}$ and $\mathbf{Q}_p$ of the field $\mathbf{Q}$ with respect to the non-improper absolute values on $\mathbf{Q}$ ($p$ any prime) are locally compact. On the other hand, for every power $q = p^f$ of a prime number $p$, the field $\mathbf{F}_q((T))$ of formal power series over the finite field $F$, with the valuation defined in § 3, no. 4, Example 3 is *locally compact*: for the maximal ideal of the valuation ring $\mathbf{F}_q[[T]]$ is generated by $T$; we know that this ring is complete with the (T)-adic topology (Chapter III, § 2, no. 6, Proposition 6) and, as the residue field $\mathbf{F}_q$ is finite, Proposition 2 of § 5, no. 1 proves our assertion. Conversely:

#### Theorem 1 {#ac-vi-s9-thm-1 .statement}

*Let K be a (not necessarily commutative) locally compact field which is not discrete.*

(i) *If K is of characteristic 0 and mod, is not an ultrametric absolute value then K is isomorphic to one of the fields $\mathbf{R}, \mathbf{C}$ or $\mathbf{H}$.*

(ii) *If K is of characteristic 0 and mod, is an ultrametric absolute value, K is an algebra of finite rank over a p-adic field $\mathbf{Q}_p$.*

(iii) *If K is of characteristic $p \neq 0$, it is isomorphic to a field with centre a field of formal power series $\mathbf{F}_q((T))$ (where $q$ is a power of $p$) and of finite rank over its centre.*

(i) It follows from Ostrowski's Theorem (§ 6, no. 4, Theorem 2) that K is a topological field isomorphic to an everywhere dense subfield of $\mathbf{R}, \mathbf{C}$ or $\mathbf{H}$ and, as K is complete, it is isomorphic to $\mathbf{R}, \mathbf{C}$ or $\mathbf{H}$.

(ii) Let A be the ring of the absolute value mod, and m its maximal ideal. We know that A/m is a finite field (§ 5, no. 1, Proposition 2) and hence the absolute value induced by mod, on $\mathbf{Q}$ has a finite residue field, which is only possible if it is equivalent to a $p$-adic absolute value ($\S 6$, no. 3, Proposition 4); the closure of $\mathbf{Q}$ in $K$ is therefore isomorphic to $\mathbf{Q}_p$ and is contained in the centre of $K$ since the latter is closed in $K$; we conclude using Proposition 2 of no. 1.

(iii) The second assertion follows from the first and the Corollary to Proposition 2 of no. 2. To show the first assertion, note that mod, is necessarily an ultrametric absolute value ($\S 6$, no. 2, Corollary to Proposition 3); in the notation of the proof of Proposition 3 of no. 2, the centre $Z$ of $K$ consists of the elements which commute with both $s$ and $u$; but by virtue of (3),

$$
u^{-q} s u^q = s^{q p^r} = s,
$$

so that $u^q \in Z$ and we conclude that $Z$ is not discrete. As $Z$ is locally compact, we may confine our attention to the case where $K$ is commutative. The sub-$\mathbf{F}_p$-algebra $\mathbf{F}_p[s]$ in $K$ is then a finite field since $s^{q-1} = 1$ and obviously $y^q = y$ for every element of this field, which is therefore identical with $S$ and isomorphic to $\mathbf{F}_q$ since $S \subset \mathbf{F}_p[s]$ has $q$ elements. Since the sum of two elements of $S$ is in $S$, the mapping which maps each formal power series $\sum_{i=0}^\infty s_i T^i \in \mathbf{F}_q[[T]]$ to the element $\sum_{i=0}^\infty s_i u^i$ is a bijective homomorphism of the ring $\mathbf{F}_q[[T]]$ onto the ring $A$, whence immediately the conclusion.

#### Corollary 1 {#ac-vi-s9-thm-1-cor-1 .statement}

*Every locally compact field* which is *not discrete* *is of finite rank* over its centre.

#### Corollary 2 {#ac-vi-s9-thm-1-cor-2 .statement}

Every locally *compact field* is connected *or* totally disconnected; *if* it is connected, it *is* isomorphic to $\mathbf{R}, \mathbf{C}$ *or* $\mathbf{H}$.

If the topology on a field $K$ is defined by an ultrametric absolute value, $K$ is totally disconnected with this topology.

#### Remark {#ac-vi-s9-n3-rem-1 .statement}

Let $s$ be an integer $> 0$; the subfield $\mathbf{F}_q((T^s)) = L$ of $K = \mathbf{F}_q((T))$ is closed in $K$ and $e(K/L) = s$ and $f(K/L) = 1$. It is therefore seen that there are closed subfields $L$ of $K$ which are not discrete and such that $e(K/L)$ (and *a fortiori* the degree $[K:L]$) is arbitrarily large (contrary to what happens for locally compact fields of characteristic 0, where every locally compact subfield $L$ of such a field $K$ necessarily contains $\mathbf{R}$ or $\mathbf{Q}_p$ and therefore $[K:L]$ is bounded).

### Exercises {#ac-vi-s9-exercises}

22. (a) If there exists a discrete valuation on a field K, show that the algebraic closure of K is infinite over K.

(b) Let K be a finitely generated extension of a field $K_0$. Show that, if K is not algebraic over $K_0$, there exists a discrete valuation $v$ on K such that $v(x) = 0$ on $K_0$.

39

See the [exercises for § 9](exercises/s9/).
