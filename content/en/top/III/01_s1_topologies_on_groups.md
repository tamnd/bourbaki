---
book: top
book_title: General Topology
chapter: III
chapter_title: Topological Groups
section: 1
section_title: Topologies on groups
lang: en
source: top-i-iv
book_pages: 219-225, 296-298
pdf_pages: 0225-0231, 0302-0304
extraction: ocr
subsections:
    - "no": 1
      title: TOPOLOGICAL GROUPS
      page: 219
      pdf_page: 225
    - "no": 2
      title: NEIGHBOURHOODS OF A POINT IN A TOPOLOGICAL GROUP
      page: 221
      pdf_page: 227
    - "no": 3
      title: ISOMORPHISMS AND LOCAL ISOMORPHISMS
      page: 224
      pdf_page: 230
statements: 11
exercises: 9
content_sha256: f71f82bff625e103d0a3fb544959913a24fd65f8bf1e933f0d5f6ba6a6f353ff
---

## 1. TOPOLOGIES ON GROUPS

### 1. TOPOLOGICAL GROUPS

In the first four sections of this chapter the law of composition of a group will generally be written multiplicatively, and e shall denote the identity element; translation of results into additive notation (which, we recall, is reserved exclusively to commutative groups) is usually left to the reader.

#### Definition 1 {#top-iii-s1-def-1 .statement}

A topological group is a set G which carries a group structure and a topology and satisfies the following two axioms:

(GT_I). The mapping $(x, y) \to xy$ of $G \times G$ into $G$ is continuous.

(GT_{II}). The mapping $x \to x^{-1}$ of $G$ into $G$ (the symmetry of the group G) is continuous.

A group structure and a topology on a set G are said to be compatible if they satisfy (GT_I) and (GT_{II}).

#### Example 1 {#top-iii-s1-n1-exa-1 .statement}

The discrete topology on a group G is compatible with the group structure. A topological group whose topology is discrete is called a discrete group.

Again, the coarsest topology (Chapter I, § 2, no. 2) on G is compatible with the group structure of G.

#### Example 2 {#top-iii-s1-n1-exa-2 .statement}

In Chapter IV we shall see that the topology of the rational line Q (resp. the real line R) is compatible with the additive group structure of Q (resp. R).

#### Example 3 {#top-iii-s1-n1-exa-3 .statement}

If G is a topological group, its topology is compatible with the structure of the group $G^0$ which is the opposite of G; $G^0$, with this topology, is said to be the topological group opposite to G.

Axioms $(\mathrm{GT}_\mathrm{I})$ and $(\mathrm{GT}_\mathrm{II})$ are equivalent to the following:

(GT'). *The mapping* $(x, y) \to xy^{-1}$ *of* $G \times G$ *into* $G$ *is continuous*.

Clearly $(\mathrm{GT}_\mathrm{I})$ and $(\mathrm{GT}_\mathrm{II})$ together imply (GT'). Conversely, (GT') implies $(\mathrm{GT}_\mathrm{II})$, for $x \to ex^{-1} = x^{-1}$ is then continuous; and (GT') and $(\mathrm{GT}_\mathrm{II})$ together imply $(\mathrm{GT}_\mathrm{I})$, for $(x, y) \to x(y^{-1})^{-1} = xy$ is then continuous.

If $a$ is any element of $G$, the *left translation* $x \to ax$ (resp. the *right translation* $x \to xa$) is continuous, by $(\mathrm{GT}_\mathrm{I})$, and is therefore a *homeomorphism* of $G$ onto $G$. The mappings $x \to axb$, as $a$ and $b$ run through $G$, thus form a *group of homeomorphisms* of $G$; the mappings $x \to axa^{-1}$ (resp. $x \to ax, x \to xa$), where $a$ runs through $G$, form a subgroup of this group of homeomorphisms. Again, since the symmetry $x \to x^{-1}$ is an involutory permutation of $G$, axiom $(\mathrm{GT}_\mathrm{II})$ shows that this mapping is a *homeomorphism* of $G$ onto $G$.

If $A$ is an open (resp. closed) subset of $G$, and if $x$ is any point of $G$, then the sets $x.A, A.x$ and $A^{-1} (*)$ are open (resp. closed), for they are the transforms of $A$ under one of the preceding homeomorphisms. If $A$ is *open* and $B$ is any subset of $G$, then $AB$ and $BA$ are *open*, because they are unions of open sets [axiom $(\mathrm{O}_\mathrm{I})$]. If $V$ is a neighbourhood of $e$ in $G$, then $VA$ and $AV$ are *neighbourhoods* of $A$; for if $W$ is an open neighbourhood of $e$ contained in $V$, then $WA$ and $AW$ are open and contain $A$.

On the other hand, $AB$ need not be closed when $A$ is closed, even if $B$ is closed too (cf. § 4, no. 1, Corollary 1 to Proposition 1).

\* For example, in the additive group of the real line $\mathbf{R}$, the subgroup $\mathbf{Z}$ of the rational integers is closed, and so is the subgroup $\theta \mathbf{Z}$ consisting of all integer multiples $n\theta$ of an *irrational* number $\theta$; but the subgroup $\mathbf{Z} + \theta \mathbf{Z}$ of $\mathbf{R}$, which is the set of all real numbers $m + n\theta$ (where $m$ and $n$ take all integer values) is not closed in $\mathbf{R}$, as we shall see in Chapter V, § 1.

Again, let $A$ be the subset of the additive group of $\mathbf{R} \times \mathbf{R}$ which consists of all $(x, y)$ pairs such that $x \geqslant 0$ and $0 \leqslant y \leqslant 1 - \frac{1}{x+1}$; and let $B$ be the set of all pairs $(x, 0)$, as $x$ runs through $\mathbf{R}$. $A$ and $B$ are closed, but $A + B$ is the set of all pairs $(x, y)$ such that $0 \leqslant y < 1$, and is not closed in $\mathbf{R} \times \mathbf{R}$. \*

Let $X$ be a topological space and let $f$ and $g$ be two mappings of $X$ into a topological group $G$. If $f$ and $g$ are continuous at a point $x_0$

(*) We recall that if $A$ and $B$ are two subsets of a group $G$, then $A.B$ or $AB$ denotes the set of all products $xy$ where $x \in A$ and $y \in B$; $A^{-1}$ denotes the set of all elements $x^{-1}$ where $x \in A$. If $B$ consists of a single element $x$, we write $x.A$ or $xA$ (resp. $A.x$ or $Ax$) in place of $\{ x \}.A$ (resp. $A.\{ x \}$).

of X, then so are $f^{-1}$ and $fg$(*), by Theorem 2 of Chapter I, § 2, no. 1. In particular, the continuous mappings of X into G form a subgroup of the group $G^X$ of all mappings of X into G.

Again, let $f$ and $g$ be two mappings of a set X, filtered by a filter $\mathfrak{F}$, into a Hausdorff topological group G. If $\lim_{\mathfrak{F}} f$ and $\lim_{\mathfrak{F}} g$ exist, then so do $\lim_{\mathfrak{F}} f^{-1}$ and $\lim_{\mathfrak{F}} fg$, and we have (Chapter I, § 7, no. 4, Proposition 9, Corollary 1)

(1) $$
\lim_{\mathfrak{F}} f^{-1} = (\lim_{\mathfrak{F}} f)^{-1},
$$
(2) $$
\lim_{\mathfrak{F}} fg = (\lim_{\mathfrak{F}} f) (\lim_{\mathfrak{F}} g).
$$

When G is a commutative group, written additively, the axiom (GT') indicates that $(x, y) \to x - y$ is a continuous mapping. If $f$ and $g$ are mappings of a topological space X into G, continuous at a point $x_0$, then $f - g$ is continuous at this point. The formulas (1) and (2) can be transcribed similarly.

### 2. NEIGHBOURHOODS OF A POINT IN A TOPOLOGICAL GROUP

Let $\mathcal{B}$ be the neighbourhood filter of the identity element $e$ in a topological group G, and let $a$ be any point of G. Since $x \to ax$ and $x \to xa$ are homeomorphisms, it follows that the neighbourhood filter of $a$ is the family $a.\mathcal{B}$ of sets $a.V$, where V runs through $\mathcal{B}$, and is also the family $\mathcal{B}.a$ of sets $V.a$. Thus we know the neighbourhood filter of any point of a topological group as soon as we know the neighbourhood filter of the identity element $e$ of the group.

If we say that $xy$ and $x^{-1}$ are continuous at $x = y = e$, we obtain (Chapter I, § 2, no. 1):

(GV_I). *Given any* $U \in \mathcal{B}$, *there exists* $V \in \mathcal{B}$ *such that* $V.V \subset U$.

(GV_{II}). *Given any* $U \in \mathcal{B}$, *we have* $\overline{U} \in \mathcal{B}$.

Every filter $\mathcal{B}$ on G which satisfies (GV_I) and (GV_{II}) also satisfies (GV_a). *Given any* $U \in \mathcal{B}$, *there exists* $V \in \mathcal{B}$ *such that* $V.V^{-1} \subset U$. For by (GV_I), there exists $W \in \mathcal{B}$ such that $W.W \subset U$, and by (GV_{II}) there exists $V \in \mathcal{B}$ such that $V \subset W \cap W^{-1}$; hence $V^{-1} \subset W$ and therefore $V.V^{-1} \subset W.W \subset U$.

Conversely, if a filter $\mathcal{B}$ on G satisfies (GV_a), it follows first of all that $e$ belongs to every set $U \in \mathcal{B}$; for if $V \in \mathcal{B}$ is such that $V.V^{-1} \subset U$,

(*) We recall that $f^{-1}$ is the mapping $x \to (f(x))^{-1}$ and $fg$ the mapping $x \to f(x)g(x)$; they should not be confused with $f^{-1}$ and $f \circ g$ (when these are defined) (*Set Theory*, R, § 2, nos. 6 and 11).

then, since $V$ is not empty, we have $x.x^{-1} = e \in U$ for every $x \in V$. The condition $(GV_a)$ therefore implies that $V^{-1} \subset V.V^{-1} \subset U$, so that $U^{-1} \in \mathcal{B}$ whenever $U \in \mathcal{B}$. Finally, if $V \in \mathcal{B}$ is such that $V.V^{-1} \subset U$, and $W \in \mathcal{B}$ is such that $W \subset V \cap V^{-1}$, we have $W.W \subset U$. We see thus that $(GV_a)$ is *equivalent* to the conjunction of $(GV_1)$ and $(GV_{II})$.

Finally, since $x \to axa^{-1}$ is a homeomorphism which leaves $e$ fixed, $\mathcal{B}$ has the following property:

$(GV_{III}).$ *For all* $a \in G$ *and all* $V \in \mathcal{B}$, *we have* $a.Va^{-1} \in \mathcal{B}$.

These three properties of the filter $\mathcal{B}$ are *characteristic*:

#### Proposition 1 {#top-iii-s1-prop-1 .statement}

*Let* $G$ *be a group and let* $\mathcal{B}$ *be a filter on* $G$ *satisfying the axioms* $(GV_1)$, $(GV_{II})$ *and* $(GV_{III})$. *Then there is a unique topology on* $G$, *compatible with the group structure of* $G$, *for which* $\mathcal{B}$ *is the neighbourhood filter of the identity element* $e$. *For this topology the neighbourhood filter of any point* $a \in G$ *is the same as each of the two filters* $a.\mathcal{B}$ *and* $\mathcal{B}.a$.

If there is a topology with the required properties, then by what has been said above the neighbourhood filter of $a$ coincides with each of the filters $a.\mathcal{B}$ and $\mathcal{B}.a$; hence the topology is unique, if it exists. Its existence will be established if we show 1) that the filters $a.\mathcal{B}$ are the neighbourhood filters of a topology on $G$, and 2) that this topology is compatible with the group structure of $G$.

1) The filter $a.\mathcal{B}$ satisfies axiom $(V_{III})$ (see Chapter I § 1, no. 2) by reason of $(GV_1)$ and $(GV_{II})$, as we have already seen; hence to show that $a.\mathcal{B}$ is the neighbourhood filter of $a$ in a topology on $G$, we have to verify axiom $(V_{IV})$. Let then $V$ be any set of $\mathcal{B}$, and $W$ a set of $\mathcal{B}$ such that $W.W \subset V$; then for any $x \in a.W$ we have $x.W \subset a.W.W \subset a.V$, so that $a.V$ belongs to the filter $x.\mathcal{B}$; hence $(V_{IV})$ is satisfied.

2) Let us now show that the topology defined by the neighbourhood filters $a.\mathcal{B}$ satisfies $(GT')$. Let $a, b$ be any two points of $G$; if we put $x = au$ and $y = bv$, then we have to show that $xy^{-1}$ is as near as we please to $ab^{-1}$ whenever $u$ and $v$ are close enough to $e$. Now $(ab^{-1})^{-1}(xy^{-1}) = buv^{-1}b^{-1}$; let $U$ be any neighbourhood of $e$, then we shall have $buv^{-1}b^{-1} \in U$ if $uv^{-1} \in b^{-1}Ub = V$, and $V \in \mathcal{B}$ by reason of $(GV_{III})$. But by $(GV_1)$ and $(GV_{II})$ there exists $W \in \mathcal{B}$ such that $W.W^{-1} \subset V$; hence it is enough to take $u \in W$ and $v \in W$ in order to have $xy^{-1} \in (ab^{-1})U$. This completes the proof.

A common method of defining a topology compatible with a group structure on $G$ consists in giving a filter satisfying the axioms $(GV_1)$, $(GV_{II})$ and $(GV_{III})$. The corresponding conditions for a *filter base* $\mathcal{B}$ are as follows:

$(GV'_1).$ *Given any* $U \in \mathcal{B}$, *there exists* $V \in \mathcal{B}$ *such that* $V.V \subset U$.

(GV_{II}). *Given any* $U \in \mathcal{B}$, *there exists* $V \in \mathcal{B}$ *such that* $V^{-1} \subset U$.

(GV'_{III}). *Given any* $a \in G$ *and any* $U \in \mathcal{B}$, *there exists* $V \in \mathcal{B}$ *such that* $V \subset a . U . a^{-1}$.

A neighbourhood of $e$ which coincides with its image under the symmetry $x \to x^{-1}$ is said to be *symmetric*. If $V$ is any neighbourhood of $e$, then $V \cup V^{-1}$, $V \cap V^{-1}$ and $V . V^{-1}$ are symmetric neighbourhoods. By (GV_{II}), the symmetric neighbourhoods form a *fundamental system of neighbourhoods* of $e$. Also it follows from (GV_{I}) that when $V$ runs through a fundamental system of neighbourhoods of $e$, the sets $V^n$ (where $n$ is a fixed integer $\neq 0$) form a fundamental system of neighbourhoods of $e$.

#### Remark {#top-iii-s1-n2-rem-1 .statement}

If $G$ is *commutative*, we have $x . A . x^{-1} = A$ for every subset $A$ of $G$ and every $x \in G$, and therefore (GV_{III}) [resp. (GV'_{III})] is automatically satisfied for every filter (resp. filter base) on $G$. On the other hand, if $G$ is not abelian, then (GV_{III}) is not a consequence of (GV_{I}) and (GV_{II}) [see Exercise 5].

If $G$ is a commutative group, written *additively*, the axioms which characterize the filter $\mathcal{B}$ of neighbourhoods of the origin for a topology compatible with the group structure of $G$ are therefore the following:

(GA_{I}). *Given any* $U \in \mathcal{B}$, *there exists* $V \in \mathcal{B}$ *such that* $V + V \subset U$.

(GA_{II}). *Given any* $U \in \mathcal{B}$, *we have* $-U \in \mathcal{B}$.

#### Proposition 2 {#top-iii-s1-prop-2 .statement}

*A topological group* $G$ *is Hausdorff if and only if the set* $\{e\}$ *is closed*.

Clearly, if $G$ is Hausdorff, then $\{e\}$ is closed. Conversely, if $\{e\}$ is closed, then the diagonal $\Delta$ of $G \times G$ is closed, because it is the inverse image of $\{e\}$ under the continuous mapping $(x, y) \to xy^{-1}$; hence (Chapter I, § 8, no. 1, Proposition 1) $G$ is Hausdorff.

#### Corollary {#top-iii-s1-n2-cor-1 .statement}

*A topological group* $G$ *is Hausdorff if and only if the intersection of the neighbourhoods of* $e$ *consists only of the point* $e$.

The condition is clearly necessary. Conversely, if the intersection of all the neighbourhoods of $e$ is just $\{e\}$, then given any $x \neq e$ there is a neighbourhood $V$ of $e$ such that $x^{-1} \notin V$ and therefore $e \notin xV$. This shows that $x$ is not in the closure of $\{e\}$, and thus $\{e\}$ is closed, so that $G$ is Hausdorff.

#### Example {#top-iii-s1-n2-exa-1 .statement}

*Definition of a topology on a group by means of a set of subgroups.* If $\mathcal{B}$ is a *filter base* on a group $G$, formed of *subgroups* of $G$, then it is immediately seen that $\mathcal{B}$ satisfies axioms (GV_{I}) and (GV_{II}), since $H . H^{-1} = H$ for any subgroup $H$ of $G$. Hence the set $\mathcal{B}$ will be a *fundamental system of neighbourhoods* of $e$ in a topology compatible with the group structure of $G$, provided that $\mathcal{B}$ satisfies (GV_{III}); this will in particular be the case if all the subgroups in $\mathcal{B}$ are normal, hence always if $G$ is *commutative*. The topology thus defined is *Hausdorff*, by Proposition 2, if and only if *the intersection of all the subgroups in $\mathcal{B}$ consists only of* $e$. The most interesting cases are those in which the subgroup $\{ e \}$ *is not in* $\mathcal{B}$ (otherwise the topology defined by $\mathcal{B}$ is the *discrete* topology): if $\{ e \} \notin \mathcal{B}$, the topology defined by $\mathcal{B}$ is Hausdorff only if $\mathcal{B}$ is an *infinite* set.

Since the intersection of two subgroups is a subgroup, we can define a topology on $G$, compatible with its group structure, starting from *any* set $\mathfrak{F}$ of subgroups of $G$: let $\mathfrak{G}$ be the set of all subgroups $a.H.a^{-1}$, where $H \in \mathfrak{F}$ and $a \in G$, and let $\mathcal{B}$ be the set of all *finite* intersections of subgroups belonging to $\mathfrak{G}$. Then $\mathcal{B}$ is a filter base and satisfies (GV$_{\text{III}}$).

Consider in particular the additive group of a *ring* $A$. Every set $\mathfrak{F}$ of *ideals* of $A$ defines a topology compatible with this additive group structure. This topology is Hausdorff if the intersection of all the ideals of $\mathfrak{F}$ is the zero ideal, and it is not discrete if no finite intersection of the ideals of $\mathfrak{F}$ is the zero ideal. Topologies defined in this way play a large part in the theory of numbers (see the Exercises of §§ 6 and 7 of this chapter).

### 3. ISOMORPHISMS AND LOCAL ISOMORPHISMS

In accordance with the general definitions (*Set Theory*, Chapter IV, § 1, no. 5) an *isomorphism* $f$ of a topological group $G$ *onto* a topological group $G'$ is a bijective mapping of $G$ onto $G'$ which is simultaneously an *isomorphism of the group structure of* $G$ onto that of $G'$, and a *homeomorphism of* $G$ onto $G'$. In other words, $f$ is an isomorphism of $G$ onto $G'$ if and only if: 1) $f$ is bijective; 2) $f(xy) = f(x)f(y)$ for all $x, y \in G$; and 3) $f$ is bicontinuous.

For example, if $a$ is any point of $G$, the mapping $x \to axa^{-1}$ is an isomorphism of $G$ onto $G$, that is (*loc. cit.*), an *automorphism* of the topological group $G$. It is called an *inner automorphism*.

If a topology $\mathcal{C}$ is compatible with the group structure of a group $G$, then $\mathcal{C}$ is also compatible with the group structure *opposite* to that of $G$. If $G^0$ denotes the topological group obtained by giving the group opposite to $G$ the topology $\mathcal{C}$, then the symmetry $x \to x^{-1}$ is an *isomorphism* of the topological group $G$ onto the topological group $G^0$.

#### Definition 2 {#top-iii-s1-def-2 .statement}

*If* $G$ *and* $G'$ *are two topological groups, a local isomorphism of* $G$ *with* $G'$ *is a homeomorphism* $f$ *of a neighbourhood* $V$ *of the identity element of* $G$ *onto a neighbourhood* $V'$ *of the identity element of* $G'$ *which satisfies the following conditions:*

1) *For each pair* $x, y$ *of points of* $V$ *such that* $xy \in V$,
$$
f(xy) = f(x)f(y).
$$

2) If g is the mapping inverse to f, then for each pair of points x', y' of V' such that x'y' ∈ V', we have g(x'y') = g(x') g(y').
The mapping g is then a local isomorphism of G' with G.
Two topological groups G, G' are said to be locally isomorphic if there exists a local isomorphism of G with G'.

Isomorphic topological groups are evidently locally isomorphic. The converse is false.

\* For example, we shall see in Chapter V, § 1, that the topological groups R and T are locally isomorphic but not isomorphic. \*

If f is a local isomorphism of G with G', then every restriction of f to a neighbourhood of the identity element of G is again a local isomorphism of G with G'.

A local isomorphism of G with G is called a local automorphism of G.

In general, if f is a homeomorphism of a neighbourhood V of the identity element of G onto a neighbourhood V' of the identity element of G' which satisfies condition 1) of Definition 2, f does not necessarily satisfy condition 2) (see Exercise 7). Nevertheless, G and G' are in fact locally isomorphic.

#### Proposition 3 {#top-iii-s1-prop-3 .statement}

Let G and G' be two topological groups, and let f be a homeomorphism of a neighbourhood V of the identity element of G onto a neighbourhood V' of the identity element of G', which satisfies condition 1) of Definition 2. Then f is an extension of a local isomorphism of G with G'.

For it is not hard to see that if W is a neighbourhood of the identity element of G such that W.W ⊂ V, then the restriction of f to W is a local isomorphism of G with G'.

### Exercises {#top-iii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
