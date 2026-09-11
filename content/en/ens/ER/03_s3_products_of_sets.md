---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 3
section_title: Products of sets
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 357-362
pdf_pages: 0362-0367
extraction: ocr
statements: 0
exercises: 0
content_sha256: 911c36b076fa6fa142fe625cbd3bb6de17b251c6493dfaffdaf76058fad82252
---

## 3. PRODUCTS OF SETS

1. Let E, F be two sets, which may or may not be distinct. The *ordered pairs* $(x,y)$, whose first element $x$ is any element of E and whose second element $y$ is any element of F, are the elements of a new set, called the *product of E by F*, and denoted by $E\times F$; E and F are called the *factors* of $E\times F$. Two ordered pairs are considered to be identical only if they have the same first element and the same second element; in other words, the relation “$(x,y)=(x',y')$” is equivalent to the relation “$x=x'$ and $y=y'$”. If $z$ is any element of $E\times F$, the relation “$x$ is the first element of the ordered pair $z$” is a functional relation in $x$; it determines a mapping of $E\times F$ onto E, which is called the *first coordinate function*, or the *first projection*, and is denoted by $\operatorname{pr}_1$. Instead of saying “$x$ is the first element of the ordered pair $z$”, we also say “$x$ is the first coordinate (or projection) of $z$" or "$x = \mathrm{pr}_1 z$". Similarly we define the *second coordinate function*, or *second projection*, which is a mapping of $\mathrm{E} \times \mathrm{F}$ *onto* $\mathrm{F}$, denoted by $\mathrm{pr}_2$.

The relation "$x = \mathrm{pr}_1 z$ and $y = \mathrm{pr}_2 z$" is equivalent to "$z = (x, y)$".

The extension of the function $\mathrm{pr}_1$ to sets of subsets is denoted by the same symbol, in accordance with the general conventions, and is again called the *first projection* (here we do not use the term "coordinate"); similarly for the extension of the second projection.

2. A relation R between a generic element $x$ of E and a generic element $y$ of F is a property of the pair $(x, y)$, and consequently defines a subset of the product $\mathrm{E} \times \mathrm{F}$, called the *graph* of R. Conversely, every subset A of $\mathrm{E} \times \mathrm{F}$ is the graph of the relation $(x, y) \in \mathrm{A}$ between $x$ and $y$.

Let A be a subset of E and let B be a subset of F. We denote by $\mathrm{A} \times \mathrm{B}$ the subset of $\mathrm{E} \times \mathrm{F}$ defined by the relation "$x \in \mathrm{A}$ and $y \in \mathrm{B}$" between $x$ and $y$.

3. In the following propositions, X and X$'$ denote arbitrary subsets of E, Y and Y$'$ arbitrary subsets of F, and Z an arbitrary subset of $\mathrm{E} \times \mathrm{F}$.

(a) The relation "$\mathrm{X} \times \mathrm{Y} = \emptyset$" is *equivalent* to "$\mathrm{X} = \emptyset$ or $\mathrm{Y} = \emptyset$".

(b) If $\mathrm{X} \times \mathrm{Y} \neq \emptyset$, the relation "$\mathrm{X} \times \mathrm{Y} \subset \mathrm{X}' \times \mathrm{Y}'$" is *equivalent* to "$\mathrm{X} \subset \mathrm{X}'$ and $\mathrm{Y} \subset \mathrm{Y}'$".

(c) For all X, X$'$, Y we have

$$(\mathrm{X} \times \mathrm{Y}) \cup (\mathrm{X}' \times \mathrm{Y}) = (\mathrm{X} \cup \mathrm{X}') \times \mathrm{Y}. \tag{22}$$

(d) For all X, X$'$, Y, Y$'$ we have

$$(\mathrm{X} \times \mathrm{Y}) \cap (\mathrm{X}' \times \mathrm{Y}') = (\mathrm{X} \cap \mathrm{X}') \times (\mathrm{Y} \cap \mathrm{Y}'). \tag{23}$$

(e) For all X, Y we have

$$\overset{-1}{\mathrm{pr}_1}(\mathrm{X}) = \mathrm{X} \times \mathrm{F}, \qquad \overset{-1}{\mathrm{pr}_2}(\mathrm{Y}) = \mathrm{E} \times \mathrm{Y}. \tag{24}$$

(f) If $\mathrm{Y} \neq \emptyset$, then for all X we have

$$\mathrm{pr}_1(\mathrm{X} \times \mathrm{Y}) = \mathrm{X}. \tag{25}$$

(g) For all Z we have

$$\mathrm{Z} \subset \mathrm{pr}_1(\mathrm{Z}) \times \mathrm{pr}_2(\mathrm{Z}). \tag{26}$$

(h) Let $a$ be an element of E. Then the mapping $(a, y) \rightarrow y$ of the set $\{a\} \times \mathrm{F}$ *onto* F (i.e., the restriction of $\mathrm{pr}_2$ to the subset $\{a\} \times \mathrm{F}$) is *one-to-one*.

4. The mapping

(27) $$(x, y) \to (y, x)$$

is a *one-to-one* mapping of $\mathrm{E} \times \mathrm{F}$ *onto* $\mathrm{F} \times \mathrm{E}$, and is called *canonical*. When E and F are the same set, the mapping (27) is called the *canonical symmetry*; it is then *involutory*. The elements $(x, y)$ of $\mathrm{E} \times \mathrm{E}$ which are fixed under this symmetry are those which have the property $x = y$; the set $\Delta$ of these elements is called the *diagonal* of $\mathrm{E} \times \mathrm{E}$. The mapping $x \to (x, x)$ is a *bijection* of E onto $\Delta$, called the *diagonal mapping* of E into $\mathrm{E} \times \mathrm{E}$.

If Z is any subset of $\mathrm{E} \times \mathrm{F}$, the image of Z under the canonical mapping of $\mathrm{E} \times \mathrm{F}$ onto $\mathrm{F} \times \mathrm{E}$ is denoted by $\overset{-1}{\mathrm{Z}}$. If X is any subset of E and Y any subset of F, then

$$\overset{-1}{\overgroup{\mathrm{X} \times \mathrm{Y}}} = \mathrm{Y} \times \mathrm{X}.$$

If a relation R between $x$ and $y$, considered as a property of the ordered pair $(x, y)$, defines a subset A of $\mathrm{E} \times \mathrm{F}$, then the *same* relation, considered as a property of the pair $(y, x)$, defines the subset $\overset{-1}{\mathrm{A}}$ of $\mathrm{F} \times \mathrm{E}$. R is equivalent to each of the relations $(x, y) \in \mathrm{A}$, $(y, x) \in \overset{-1}{\mathrm{A}}$. If E and F are the same set, the relation R and the corresponding subset A are said to be *symmetric* when $\mathrm{A} = \overset{-1}{\mathrm{A}}$. The diagonal $\Delta$ (defined by the relation of equality) is symmetric. If Z is any subset of $\mathrm{E} \times \mathrm{E}$, then $\mathrm{Z} \cup \overset{-1}{\mathrm{Z}}$ and $\mathrm{Z} \cap \overset{-1}{\mathrm{Z}}$ are symmetric.

5. Let A be a subset of a set E, and let $f$ be a mapping of A into a set F. The relation "$x \in \mathrm{A}$ and $y = f(x)$" between a generic element $x$ of E and a generic element $y$ of F defines a subset of $\mathrm{E} \times \mathrm{F}$ called the *graph* of the function $f$. If B is a subset of E which contains A, and if $g$ is an *extension* (§ 2, no. 13) of $f$ to B, then the graph of $f$ is *contained* in the graph of $g$.

Conversely, let C be a subset of $\mathrm{E} \times \mathrm{F}$ such that, for each $x \in \mathrm{E}$, there exists *at most one* $y \in \mathrm{F}$ such that $(x, y) \in \mathrm{C}$. Then the relation $(x, y) \in \mathrm{C}$ between a generic element $x$ *of the set* $\mathrm{pr}_1(\mathrm{C})$ and a generic element $y$ of F is a functional relation in $y$ and determines a mapping of $\mathrm{pr}_1(\mathrm{C})$ into F whose graph is C.

The set of subsets C of $\mathrm{E} \times \mathrm{F}$ which have the property "for all $x \in \mathrm{E}$ there is at most one $y \in \mathrm{F}$ such that $(x, y) \in \mathrm{C}$" (a set which is a subset of $\mathfrak{P}(\mathrm{E} \times \mathrm{F})$) can therefore be put into one-to-one correspondence with *the set of mappings of subsets of* E *into* F.

Let $f$ be an injective mapping of E into F, and let $g$ be the inverse of $f$ considered as a bijection of E onto $f(\mathrm{E})$. If C is the graph of $f$, then the graph of $g$ is $\overset{-1}{\mathrm{C}}$.

6. If $f$ is a mapping of E into F, and C is its graph in E $\times$ F, the relation "$y = f(x)$" is equivalent to "$(x, y) \in \mathrm{C}$". The relation "$y \in f(\mathrm{X})$" is equivalent to "there exists $x$ such that $x \in \mathrm{X}$ and $(x,\ y) \in \mathrm{C}$".

Now let K be *any* subset of E $\times$ F, and let X be any subset of E. Let K(X) denote the subset of F consisting of all elements $y$ which satisfy the relation "there exists $x$ such that $x \in \mathrm{X}$ and $(x, y) \in \mathrm{K}$"; this relation is thus equivalent to "$y \in \mathrm{K}(\mathrm{X})$". The mapping $\mathrm{X} \rightarrow \mathrm{K}(\mathrm{X})$ of $\mathfrak{P}(\mathrm{E})$ into $\mathfrak{P}(\mathrm{F})$ is said to be *defined by the subset* K of E $\times$ F. Note that K(X) is the second projection of the set $\mathrm{K} \cap (\mathrm{X} \times \mathrm{F})$. If K is the graph of a mapping $f$ of E into F, then the mapping $\mathrm{X} \rightarrow \mathrm{K}(\mathrm{X})$ is the canonical extension of $f$ to sets of subsets.

7. If $x$ is a generic element of E, then $x \rightarrow \mathrm{K}(\{x\})$ is a mapping of E into $\mathfrak{P}(\mathrm{F})$ whose value $\mathrm{K}(\{x\})$ (denoted also by $\mathrm{K}(x)$, by abuse of language) is called the *section of* K *at* $x$. The relation $(x,\ y) \in \mathrm{K}$ is equivalent to $y \in \mathrm{K}(x)$.

Conversely, *every* mapping $x \rightarrow \Phi(x)$ of E into $\mathfrak{P}(\mathrm{F})$ can be obtained in this way; for the relation $y \in \Phi(x)$ defines a subset K of E $\times$ F, and $\Phi(x)$ is precisely the section of K at $x$. The set $\mathfrak{P}(\mathrm{E} \times \mathrm{F})$ and the set of mappings of E into $\mathfrak{P}(\mathrm{F})$ are thus in one-to-one correspondence.

8. Every mapping $\mathrm{X} \rightarrow \mathrm{K}(\mathrm{X})$ defined by a subset K of E $\times$ F has the following properties, which generalize those of the canonical extension of a mapping of E into F (§2, nos. 4 and 5) :
(a)  $\mathrm{K}(\emptyset) = \emptyset$.
(b)  "$\mathrm{X} \subset \mathrm{Y}$" implies "$\mathrm{K}(\mathrm{X}) \subset \mathrm{K}(\mathrm{Y})$".
(c)  For all X, Y we have

(28) $$\mathrm{K}(\mathrm{X} \cup \mathrm{Y}) = \mathrm{K}(\mathrm{X}) \cup \mathrm{K}(\mathrm{Y}),$$
(29) $$\mathrm{K}(\mathrm{X} \cap \mathrm{Y}) \subset \mathrm{K}(\mathrm{X}) \cap \mathrm{K}(\mathrm{Y}).$$

If K and K$'$ are two subsets of E $\times$ F such that $\mathrm{K} \subset \mathrm{K}'$, then we have $\mathrm{K}(\mathrm{X}) \subset \mathrm{K}'(\mathrm{X})$ for all $\mathrm{X} \subset \mathrm{E}$; in particular, $\mathrm{K}(x) \subset \mathrm{K}'(x)$ for all $x \in \mathrm{E}$. Conversely, if $\mathrm{K}(x) \subset \mathrm{K}'(x)$ for all $x \in \mathrm{E}$, then $\mathrm{K} \subset \mathrm{K}'$.

9. A relation between a generic element of E and a generic element of F defines a subset K of E $\times$ F and a subset $\overset{-1}{\mathrm{K}}$ of F $\times$ E, and hence a mapping $\mathrm{X} \rightarrow \mathrm{K}(\mathrm{X})$ of $\mathfrak{P}(\mathrm{E})$ into $\mathfrak{P}(\mathrm{F})$ and a mapping $\mathrm{Y} \rightarrow \overset{-1}{\mathrm{K}}(\mathrm{Y})$ of $\mathfrak{P}(\mathrm{F})$ into $\mathfrak{P}(\mathrm{E})$.

If K is the graph of a mapping $f$ of E into F, the mapping $\mathrm{Y} \rightarrow \overset{-1}{\mathrm{K}}(\mathrm{Y})$ is the inverse extension of $f$.

It should be noted that the relations (18) and (19) do not generalize to the mappings $X \to K(X)$ and $Y \to \overset{-1}{K}(Y)$, when $K$ is an arbitrary subset of $E \times F$.

10. Let E, F, G be three sets, which may or may not be distinct, let A be a subset of $E \times F$ and let B be a subset of $F \times G$. Then the elements $(x, z)$ of $E \times G$ which have the property "there exists $y \in F$ such that $(x, y) \in A$ and $(y, z) \in B$" form a subset of $E \times G$, called the *composition of* B *and* A, and denoted by $B \circ A$, or simply BA when there is no risk of confusion. Here again, the order of composition is essential.

¶ The mapping $X \to BA(X)$ of $\mathfrak{P}(E)$ into $\mathfrak{P}(G)$ is the composition of $Y \to B(Y)$ and $X \to A(X)$; in other words, for all $X \subset E$ we have

$$(30) \qquad BA(X) = B(A(X)).$$

Let H be another set, not necessarily distinct from E, F, G, and let C be a subset of $G \times H$. Then we have $C \circ (B \circ A) = (C \circ B) \circ A$; this set is also denoted by $C \circ B \circ A$ (or simply CBA) and is called the *composition* of C, B, A taken in this order.

Let $f$ be a mapping of E into F, and let $g$ be a mapping of F into G. If A (resp. B) is the graph of $f$ (resp. $g$), then the composition BA is the graph of the composite mapping $g \circ f$.

11. We have

$$(31) \qquad \overset{-1}{\overbrace{B \circ A}} = \overset{-1}{A} \circ \overset{-1}{B}.$$

Let A, A′ be two subsets of $E \times F$, and let B, B′ be two subsets of $F \times G$. Then the relation

$$\text{“}A \subset A' \text{ and } B \subset B'\text{”} \qquad \text{implies} \qquad \text{“}B \circ A \subset B' \circ A'\text{”}.$$

Let A be a subset of $E \times F$, $\Delta$ the diagonal of $E \times E$, and $\Delta'$ the diagonal of $F \times F$. Then we have

$$(32) \qquad A \circ \Delta = \Delta' \circ A = A.$$

12. Let E, F, G be three sets, which may or may not be distinct. Their *product* $E \times F \times G$ is the set of ordered *triples* $(x, y, z)$, where $x \in E$, $y \in F$, and $z \in G$, the relation "$(x, y, z) = (x', y', z')$" being equivalent to "$x = x'$ and $y = y'$ and $z = z'$". The three mappings $(x, y, z) \to x$, $(x, y, z) \to y$, $(x, y, z) \to z$ of $E \times F \times G$ onto E, F, G respectively are called the *first, second,* and *third coordinate functions* (or *projections*); similarly, for example, the *projection with indices* 1, 2 is the mapping

$$
(x, y, z) \mapsto (x, y)
$$

of $E \times F \times G$ onto $E \times F$, and is denoted by $\mathrm{pr}_{1,2}$.

The definitions and propositions of nos. 2, 3, and 4 generalize easily to the product of three sets.

Furthermore, instead of considering the product $E \times F \times G$ of three sets, we may equivalently consider the product $(E \times F) \times G$, obtained by a double application of the operation of forming the product of two sets. In fact, $(x, y, z) \mapsto ((x, y), z)$ is a one-to-one mapping of $E \times F \times G$ onto $(E \times F) \times G$, called *canonical*. Similarly we define one-to-one mappings of $E \times F \times G$ onto the set $E \times (F \times G)$, and onto all the sets obtained from $E \times F \times G$, $(E \times F) \times G$, and $E \times (F \times G)$ by permuting the three letters E, F, G.

There are analogous definitions and properties for the product of more than three sets.

13. If a function $f$, which takes its values in any set $E'$, is defined on a product of three sets $E$, $F$, $G$, it is said to be a function of *three variables*, each of which runs through one of the sets $E$, $F$, $G$. The value of $f$ at the element $(x, y, z)$ of $E \times F \times G$ is denoted by $f(x, y, z)$.

Let $a$ be any element of $E$. Then $(y, z) \mapsto f(a, y, z)$ is a mapping of $F \times G$ into $E'$, called a *partial mapping (or function) determined by $f$ corresponding to the value $a$ of $x$; it is also the composite of $f$ and the mapping $(y, z) \mapsto (a, y, z)$ of $F \times G$ into $E \times F \times G$.

Likewise, if $b$ is an element of $F$, then $z \mapsto f(a, b, z)$ is a mapping of $G$ into $E'$, called the partial mapping determined by $f$ corresponding to the values $a$, $b$ of $x$, $y$.

Inversely, let $g$ be a mapping of $E$ into $E'$. Then $(x, y, z) \mapsto g(x)$ is a mapping $h$ of $E \times F \times G$ into $E'$ such that every partial mapping of $E$ into $E'$ determined by $h$, corresponding to any values of $y$ and $z$, is identical with $g$. This fact is often expressed by saying that a function of an argument $x$ can always be envisaged as a function of all the arguments which need to be considered at a given moment and which will, of course, include $x$.

14. Let $f$, $g$, $h$ be the three mappings of $E$ into $E'$, $F$ into $F'$, $G$ into $G'$, respectively. The mapping $(x, y, z) \mapsto (f(x), g(y), h(z))$ of $E \times F \times G$ into $E' \times F' \times G'$ is denoted by $f \times g \times h$ and is called the *extension of $f$, $g$, $h$ to products*. If all three of $f$, $g$, $h$ are injective (resp. surjective, bijective), then $f \times g \times h$ is injective (resp. surjective, bijective).

In this and the previous subsection we have considered only the case of *three* sets merely to fix the ideas; analogous considerations hold for any finite number of sets.
