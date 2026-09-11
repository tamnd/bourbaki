---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 6
section_title: Ordered sets
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 373-380
pdf_pages: 0378-0385
extraction: ocr
statements: 0
exercises: 0
content_sha256: 971a0a96b2a9c9ae41e13935799a40e904d52151f935272d34c3c4e23f4b84cc
---

## 6. ORDERED SETS

1. A relation $\omega\{x,y\}$ between two generic elements x, y of a set E is said to be an order relation on E, if it satisfies the following two conditions:
(a) The relation “$\omega\{x,y\}$ and $\omega\{y,z\}$” implies “$\omega\{x,z\}$” (transitivity).
(b) The relation “$\omega\{x,y\}$ and $\omega\{y,x\}$” is equivalent to “$x=y$”.
Condition (b) implies that $\omega$ is reflexive.

Let C be the subset of $E\times E$ defined by the relation $\omega\{x,y\}$ as a property of the pair $(x,y)$. Then conditions (a) and (b) are respectively equivalent to the following: (a′) $C \circ C \subset C$; (b′) $C \cap \overline{C}^{-1} = \Delta$. These imply that $C \circ C = C$.

When we consider a particular order relation on a set $E$, we say that $E$ is ordered by this relation, and that the relation defines an order structure (cf. §8) (or an ordering) on $E$.

If $\omega\{x,y\}$ is an order relation on $E$, then so is $\omega^{-1}\{x,y\}$. These two order relations, and the orderings they define, are said to be opposites of each other.

Let $\omega\{x,y\}$ be an order relation on $E$, and let $A$ be any subset of $E$. The relation $\omega\{x,y\}$ between two generic elements $x,y$ of $A$ is then an order relation on $A$, and the ordering it defines on $A$ is said to be induced by the ordering defined by $\omega\{x,y\}$ on $E$. The given ordering on $E$ is said to be an extension of the induced ordering on $A$.

A reflexive and transitive relation $\overline{\omega}\{x,y\}$ between two generic elements $x,y$ of $E$ is called a preorder relation on $E$. The relation “$\overline{\omega}\{x,y\}$ and $\overline{\omega}\{y,x\}$” is an equivalence relation $R$ on $E$, and $\overline{\omega}\{x,y\}$ is compatible (in $x$ and $y$) with this relation. Passing to the quotient (with respect to $x$ and $y$), $\overline{\omega}\{x,y\}$ induces on the set $E/R$ an order relation, said to be associated with $\overline{\omega}\{x,y\}$. A set endowed with a preorder relation is called a preordered set.

2. The inclusion relation “$Y \subset X$” is an order relation on the set of subsets $\mathfrak{P}(E)$ of any set $E$.

If $E$ and $F$ are two sets, which may or may not be distinct, the relation “$g$ extends $f$” is an order relation on the set of all mappings of subsets of $E$ into $F$.

The set $\mathbf{N}$ of natural integers [^1] is ordered by the relation “$x \leq y$”.

3. By analogy with this last example, when a set $E$ is ordered by a relation $\omega\{x,y\}$, it is often convenient to denote the relation $\omega\{x,y\}$ by $x \leq y$, or $y \geq x$; these relations are read “$x$ is less than $y$”, or “$y$ is greater than $x$” [^2]. The relations “$x<y$” and “$y>x$” (read “$x$ is strictly less than $y$”, or “$y$ is strictly greater than $x$”) are by definition equivalent to “$x\leq y$ and $x\neq y$”.

The relation “$x\leq y$” is equivalent to “$x<y$ or $x=y$”. The relation “$x\leq y$ and $y<z$” implies “$x<z$”; similarly, “$x<y$ and $y\leq z$” implies “$x<z$”.

4. A subset X of a set E, ordered by a relation “$\leq$”, is said to be *totally ordered* by this relation if, for all $x\in X$ and all $y\in X$, we have either $x\leq y$ or $y\leq x$ (or, equivalently, either $x<y$ or $x=y$ or $x>y$, these three relations being mutually exclusive).
The empty subset of an ordered set is always totally ordered. It may happen that the whole set E is totally ordered, as is the case for the set $\mathbf{N}$ and the relation $x\leq y$.
Every subset of a totally ordered set is totally ordered by the induced ordering.
In an ordered set E, if $a$ and $b$ are two elements such that $a\leq b$, the subset of E consisting of the elements $x$ such that $a\leq x\leq b$ is called the *closed interval with left-hand endpoint a and right-hand endpoint b*, and is denoted by $[a,b]$. The set of all $x\in E$ such that $a\leq x<b$ (resp. $a<x\leq b$) is called the *interval half-open on the right* (resp. *on the left*) with endpoints $a$ and $b$, and is denoted by $[a,b[$ (resp. $]a,b]$). The set of all $x\in E$ such that $a<x<b$ is called the *open interval* with endpoints $a$ and $b$, and is denoted by $]a,b[$.
The set of all $x\in E$ such that $x\leq a$ (resp. $x<a$) is called the *closed* (resp. *open*) *interval unbounded on the left, with right-hand endpoint a*, and is denoted by $] \leftarrow,a]$ (resp. $]\leftarrow,a[$); likewise, the set of all $x\in E$ such that $x\geq a$ (resp. $x>a$) is called the *closed* (resp. *open*) *interval unbounded on the right, with left-hand endpoint a*, and is denoted by $[a,\rightarrow[$ (resp. $]a,\rightarrow[$). Finally, we consider E itself as an *open interval unbounded in both directions*, and such we denote it by $]\leftarrow,\rightarrow[$.

5. If X is a subset of an ordered set E, there is at most one element $a$ of X such that $a\leq x$ for all $x\in X$; when there exists an element $a$ with this property, it is called the *least element of X*. Likewise, there exists at most one element $b$ such that $x\leq b$ for all $x\in X$; $b$, if it exists, is called the *greatest element of X*.
In a *totally ordered set E*, every *finite* non-empty subset has a greatest element and a least element, called the *maximum and minimum* elements respectively of the subset.
An ordered set in which every non-empty subset has a least element is said to be *well-ordered*. The set $\mathbf{N}$ of natural integers is well-ordered; a subset of $\mathbf{N}$ has a greatest element if and only if it is finite and non-empty. It is shown, by use of the axiom of choice, that on every set there exists a well-ordering (*Zermelo’s theorem*).
In the set $\mathfrak{P}(E)$ of subsets of a set E, ordered by inclusion, a subset $\mathfrak{F}$ of $\mathfrak{P}(E)$ has a least element if and only if the intersection of the sets of $\mathfrak{F}$ belongs to $\mathfrak{F}$, and this intersection is then the least element. Similarly, $\mathfrak{F}$ has a greatest element if and only if the union of the sets of $\mathfrak{F}$ belongs to $\mathfrak{F}$, and this union is then the greatest element.
A subset X of an ordered set E is said to be *cofinal* (resp. *coinitial*) in E if, for each $y\in E$, there exists $x\in X$ such that $y\leq x$ (resp. $y\geq x$). To say that an ordered set $E$ has a greatest (resp. least) element means that there exists a cofinal (resp. coinitial) subset of $E$ consisting of a single element.

6. Let $X$ be a subset of an ordered set $E$. Every $x\in X$ such that there exists no element $z\in X$ for which $z<x$ is called a *minimal element* of $X$. Every $y\in X$ such that there exists no element $z\in X$ for which $z>y$ is called a *maximal element* of $X$. The set of maximal elements (or the set of minimal elements) may be empty; it may also be infinite. If $X$ has a least element $a$, then $a$ is the *only* minimal element of $X$; likewise, if $X$ has a greatest element $b$, then $b$ is the *only* maximal element of $X$.

7. Let $X$ be a subset of an ordered set $E$. If an element $x\in E$ is such that $z\leq x$ for all $z\in X$, then $x$ is called *an upper bound* of $X$. Similarly, an element $y\in E$ such that $z\geq y$ for all $z\in X$ is called *a lower bound* of $X$.

The set of upper bounds (or the set of lower bounds) of a subset $X$ may be empty. A subset $X$ whose set of upper (resp. lower) bounds is not empty is said to be *bounded above* (resp. *bounded below*). A set which is bounded both above and below is said simply to be *bounded*. Every element greater than an upper bound of $X$ is an upper bound of $X$; every element less than a lower bound of $X$ is a lower bound of $X$.

If the set of upper bounds of a subset $X$ has a least element $a$, then $a$ is called the *least upper bound* or *supremum* of $X$. If the set of lower bounds of $X$ has a greatest element $b$, then $b$ is called the *greatest lower bound* or *infimum* of $X$. If these bounds exist, they are unique by definition, and they are denoted respectively by $\sup_E X$ (or $\sup X$), $\inf_E X$ (or $\inf X$). If $X$ has a greatest element, it is its least upper bound; if $X$ has a least element, it is its greatest lower bound. Conversely, if the least upper bound (resp. greatest lower bound) of $X$ exists and belongs to $X$, it is the greatest (resp. least) element of $X$.

Let $f$ be a mapping of a set $A$ into $E$. If $f(A)$ is bounded above (resp. bounded below, bounded), $f$ is said to be *bounded above* (resp. *bounded below, bounded*). If $f(A)$ has a least upper bound (resp. greatest lower bound) in $E$, this bound is called the *least upper bound* (resp. *greatest lower bound*) of $f$ and is denoted by $\sup_{x\in A} f(x)$ (resp. $\inf_{x\in A} f(x)$).

8. A preordered set $E$ in which every *finite non-empty* subset of $E$ is *bounded above* (resp. *bounded below*) is said to be *right directed* (or *directed*) (resp. *left directed*).

An ordered set $E$ in which every *finite non-empty* subset of $E$ has a least upper bound and a greatest lower bound is called a *lattice*.

The set of subsets of any set, ordered by inclusion, is a *lattice*. Every totally ordered set is a lattice.

9. An ordered set E is said to be *inductive* if it satisfies the following condition: *every totally ordered subset of E has an upper bound*.

The set $\mathfrak{P}(E)$, ordered by inclusion, is inductive. So is the set of mappings of subsets of a set E into a set F when ordered by the relation “g extends f” between f and g.

An arbitrary subset of an inductive set is not in general inductive. But if a is any element of an inductive set E, then the subset of E consisting of all elements $x \in E$ such that $x \geq a$ is inductive.

10. The following proposition is proved with the help of the axiom of choice, and is known as *Zorn’s lemma*:

*Every inductive ordered set has at least one maximal element.*

11. In the set of subsets $\mathfrak{P}(E)$ of a set E, ordered by inclusion, the least upper bound of a set $\mathfrak{F}$ of subsets of E is the *union* of the sets of $\mathfrak{F}$. Application of Zorn’s lemma gives the following result:

*If $\mathfrak{F}$ is a set of subsets of a set E such that, for each subset $\mathfrak{G}$ of $\mathfrak{F}$ which is totally ordered by the relation of inclusion, the union of the sets of $\mathfrak{G}$ belongs to $\mathfrak{F}$, then $\mathfrak{F}$ has at least one maximal element* (that is, a subset of E which belongs to $\mathfrak{F}$ but is not contained in any other subset of E belonging to $\mathfrak{F}$).

A set $\mathfrak{F}$ of subsets of a set E is said to be *of finite character* if the property “$X \in \mathfrak{F}$” is *equivalent* to the property “every *finite* subset of X belongs to $\mathfrak{F}$”. With this definition, we have the following theorem:

*Every set of subsets of E of finite character has at least one maximal element.*

12. A mapping f of a subset A of an ordered set E into an ordered set F is said to be *increasing* (resp. *decreasing*) if the relation $x \leq y$ between generic elements of A implies $f(x) \leq f(y)$ (resp. $f(y) \leq f(x)$). Every constant function on A is thus both increasing and decreasing, and the converse is true if A is (right or left) directed.

A mapping f is said to be *strictly increasing* (resp. *strictly decreasing*) if the relation $x < y$ implies $f(x) < f(y)$ (resp. $f(x) < f(y)$).

If E is *totally ordered*, every *strictly increasing* (or *strictly decreasing*) mapping of a subset A of E into an ordered set F is *injective*.

If I is an *ordered* set of indices, a family $(X_i)_{i \in I}$ of subsets of a set E is said to be *increasing* (resp. *decreasing*) if the mapping $i \to X_i$ of I into $\mathfrak{P}(E)$, ordered by inclusion, is increasing (resp. decreasing).

13. Let I be a directed set, and let $(E_\alpha)_{\alpha \in I}$ be a family of sets indexed by I. For each pair $(\alpha, \beta)$ of indices in I such that $\alpha \leq \beta$, let $f_{\beta \alpha}$ be a mapping *of* $E_\alpha$ *into* $E_\beta$, and suppose that the relations $\alpha \leq \beta \leq \gamma$ imply $f_{\gamma \alpha} = f_{\gamma \beta} \circ f_{\beta \alpha}$.

Let F be the sum of the family of sets $(E_\alpha)_{\alpha \in I}$. By abuse of language, we shall identify the $E_\alpha$ with the corresponding subsets of F. Given two elements x and y in F, let R $\{x, y\}$ be the following relation (where $\alpha$ and $\beta$ denote the elements of $I$ such that $x\in E_\alpha$ and $y\in E_\beta$): “there exists $\gamma\in I$ such that $\gamma\geq\alpha$ and $\gamma\geq\beta$ and $f_{\gamma\alpha}(x)=f_{\gamma\beta}(y)$”. Then $R$ is an equivalence relation on $F$. Let $E$ be the quotient set $F/R$, and let $f$ be the canonical mapping $F\to F/R$. The set $E$ is called the *direct limit of the family* $(E_\alpha)_{\alpha\in I}$ *with respect to the family of mappings* $(f_{\beta\alpha})$, and the restriction $f_\alpha$ of $f$ to $E_\alpha$ is called the *canonical mapping of $E_\alpha$ into $E$. We have $f_\beta\circ f_{\beta\alpha}=f_\alpha$ whenever $\alpha\leq\beta$. We write

$$
E=\underset{\longrightarrow}{\lim}\,(E_\alpha,f_{\beta\alpha})
$$

or simply $E=\underset{\longrightarrow}{\lim}\,E_\alpha$ when there is no risk of confusion. By abuse of language, the pair $((E_\alpha),(f_{\beta\alpha}))$ is called a *direct system of sets relative to* $I$.

If the $f_{\beta\alpha}$ are injective, then the $f_\alpha$ are injective. In this case we shall usually identify $E_\alpha$ and $f_\alpha(E_\alpha)$, and thus consider $E$ as the *union* of the $E_\alpha$. Conversely, if a set $E'$ is the union of a family $(E'_\alpha)_{\alpha\in I}$ of subsets such that the relation $\alpha\leq\beta$ implies $E'_\alpha\subset E'_\beta$, and if (for $\alpha\leq\beta$) $j_{\beta\alpha}$ denotes the canonical injection of $E'_\alpha$ into $E'_\beta$, then we may identify $\underset{\longrightarrow}{\lim}\,(E'_\alpha,j_{\beta\alpha})$ with $E'$, and the canonical mappings of the $E'_\alpha$ into $\underset{\longrightarrow}{\lim}\,(E'_\alpha,j_{\beta\alpha})$ with the canonical injections of the $E'_\alpha$ into $E$.

More generally, let $(E_\alpha,f_{\beta\alpha})$ be a direct system of sets relative to $I$, and for each $\alpha\in I$ let $g_\alpha$ be a mapping of $E_\alpha$ into a set $E'$ such that the relation $\alpha\leq\beta$ implies $g_\beta\circ f_{\beta\alpha}=g_\alpha$. Then there exists a unique mapping $g$ of $E=\underset{\longrightarrow}{\lim}\,E_\alpha$ into $E'$ such that $g_\alpha=g\circ f_\alpha$ for all $\alpha\in I$. The mapping $g$ is surjective if and only if $E'$ is the union of the $g_\alpha(E_\alpha)$. The mapping $g$ is injective if and only if, for each $\alpha\in I$, the relations $x\in E_\alpha$, $y\in E_\alpha$, $g_\alpha(x)=g_\alpha(y)$ imply that there exists $\beta\geq\alpha$ such that $f_{\beta\alpha}(x)=f_{\beta\alpha}(y)$. If $g$ is bijective, $E'$ is sometimes identified with the direct limit of the $E_\alpha$.

Let $(A_\alpha,\varphi_{\beta\alpha})$ and $(B_\alpha,\psi_{\beta\alpha})$ be two direct systems of sets relative to the same index set $I$. Let $A=\underset{\longrightarrow}{\lim}\,(A_\alpha,\varphi_{\beta\alpha})$, $B=\underset{\longrightarrow}{\lim}\,(B_\alpha,\psi_{\beta\alpha})$, and for each $\alpha\in I$ let $\varphi_\alpha$ (resp. $\psi_\alpha$) denote the canonical mapping of $A_\alpha$ into $A$ (resp. of $B_\alpha$ into $B$). For each $\alpha\in I$ let $u_\alpha$ be a mapping of $A_\alpha$ into $B_\alpha$ such that $u_\beta\circ\varphi_{\beta\alpha}=\psi_{\beta\alpha}\circ u_\alpha$ whenever $\alpha\leq\beta$. The family $(u_\alpha)$ is called a *direct system of mappings of* $(A_\alpha,\varphi_{\beta\alpha})$ *into* $(B_\alpha,\psi_{\beta\alpha})$. Under these conditions there exists a unique mapping $u:A\to B$ such that $u\circ\varphi_\alpha=\psi_\alpha\circ u_\alpha$ for all $\alpha\in I$. The mapping $u$ is called the *direct limit of the* $u_\alpha$, and is written $u=\underset{\longrightarrow}{\lim}\,u_\alpha$, provided that there is no risk of confusion. Let $(C_\alpha,\theta_{\beta\alpha})$ be another direct system of sets relative to $I$, let $(v_\alpha)$ be a direct system of mappings of $(B_\alpha,\psi_{\beta\alpha})$ into $(C_\alpha,\theta_{\beta\alpha})$, and let $v=\underset{\longrightarrow}{\lim}\,v_\alpha$. Then

$$
\underset{\longrightarrow}{\lim}\,(v_\alpha\circ u_\alpha)=v\circ u.
$$

Keeping the above notation, let $D_\alpha=A_\alpha\times B_\alpha$ and $\omega_{\beta\alpha}=\varphi_{\beta\alpha}\times\psi_{\beta\alpha}$. Then the family $(D_\alpha,\omega_{\beta\alpha})$ is a direct system of sets. Let $D=\underset{\longrightarrow}{\lim}\,(D_\alpha,\omega_{\beta\alpha})$, let $\omega_\alpha$ be the canonical mapping of $D_\alpha$ into $D$, let $D'=A\times B$, and let $\omega'_\alpha=\varphi_\alpha\times\psi_\alpha$. Then there exists a unique bijection (called canonical) $f:D\to D'$ such that $f\circ\omega_\alpha=\omega'_\alpha$ for all $\alpha\in I$. We shall usually identify the product $D'$ of the direct limits with the direct limit $D$ of the products $D_\alpha$.

Let $J$ be a cofinal subset of $I$; then $J$ is also directed. If $( (E_\alpha)_{\alpha\in I},(f_{\beta\alpha})_{\alpha,\beta\in I})$ is a direct system of sets relative to $I$, then $( (E_\alpha)_{\alpha\in J},(f_{\beta\alpha})_{\alpha,\beta\in J})$ is a direct system of sets relative to $J$. Let $E'$ be its direct limit, and let $f'_\alpha$ be the canonical mapping of $E_\alpha$ into $E'$ for all $\alpha\in J$. Then there exists a unique mapping $g:E'\to E$ such that $g(f'_\alpha(x))=f_\alpha(x)$ for all $\alpha\in J$ and all $x\in E_\alpha$ (where $f_\alpha$ denotes the canonical mapping of $E_\alpha$ into $E$). This mapping is a bijection, by means of which $E'$ is usually identified with $E$.

14. Let $I$ be a preordered set and let $(E_\alpha)_{\alpha\in I}$ be a family of sets indexed by $I$. For each pair $(\alpha,\beta)$ of indices of $I$ such that $\alpha\leq\beta$, let $f_{\alpha\beta}$ be a mapping of $E_\beta$ into $E_\alpha$, and suppose that the relations $\alpha\leq\beta\leq\gamma$ imply $f_{\alpha\gamma}=f_{\alpha\beta}\circ f_{\beta\gamma}$.

Let $G$ be the product of the family of sets $(E_\alpha)_{\alpha\in I}$. Let $E$ be the subset of $G$ consisting of all elements $x$ which satisfy all the relations $pr_\alpha x=f_{\alpha\beta}(pr_\beta x)$, for every pair of indices $\alpha,\beta$ such that $\alpha\leq\beta$. The set $E$ is called the inverse limit of the family $(E_\alpha)_{\alpha\in I}$ with respect to the family of mappings $(f_{\alpha\beta})$, and the restriction $f_\alpha$ of $pr_\alpha$ to $E$ is called the canonical mapping of $E$ into $E_\alpha$. We have $f_\alpha=f_{\alpha\beta}\circ f_\beta$ whenever $\alpha\leq\beta$. We write

$$
E=\lim (E_\alpha,f_{\alpha\beta}),
$$

or simply

$$
E=\lim E_\alpha
$$

when there is no risk of confusion.

By abuse of language, the pair $((E_\alpha),(f_{\alpha\beta}))$ is called an inverse system of sets relative to $I$.

It should be mentioned that $E$ can be empty, even when all the $E_\alpha$ are non-empty and all the mappings $f_{\alpha\beta}$ are surjective.

For each $\alpha\in I$ let $g_\alpha$ be a mapping of a set $E'$ into $E_\alpha$ such that the relation $\alpha\leq\beta$ implies $f_{\alpha\beta}\circ g_\beta=g_\alpha$. Then there exists a unique mapping $g$ of $E'$ into $E$ such that $g_\alpha=f_\alpha\circ g$ for all $\alpha\in I$. For $g$ to be injective it is necessary and sufficient that for each pair of distinct elements $x',y'$ of $E'$, there should exist $\alpha\in I$ such that $g_\alpha(x')\neq g_\alpha(y')$.

Let $(A_\alpha,\varphi_{\alpha\beta})$ and $(B_\alpha,\psi_{\alpha\beta})$ be two inverse systems of sets relative to the same index set $I$. Let $A=\lim(A_\alpha,\varphi_{\alpha\beta})$, $B=\lim(B_\alpha,\psi_{\alpha\beta})$, and for each $\alpha\in I$ let $\varphi_\alpha$ (resp. $\psi_\alpha$) be the canonical mapping of $A$ into $A_\alpha$ (resp. of $B$ into $B_\alpha$). For each $\alpha\in I$ let $u_\alpha$ be a mapping of $A_\alpha$ into $B_\alpha$ such that $\psi_{\alpha\beta}\circ u_\beta=u_\alpha\circ\varphi_{\alpha\beta}$ whenever $\alpha\leq\beta$. The family $(u_\alpha)$ is called an inverse system of mappings of $(A_\alpha,\varphi_{\alpha\beta})$ into $(B_\alpha,\psi_{\alpha\beta})$. Under these conditions there exists a unique mapping $u:A\to B$ such that $\psi_\alpha\circ u=u_\alpha\circ\varphi_\alpha$ for all $\alpha\in I$. The mapping $u$ is called the inverse limit of the $u_\alpha$, and is written $u=\underset{\longleftarrow}{\lim}\,u_\alpha$ when there is no risk of confusion. Let $(C_\alpha,\theta_{\alpha\beta})$ be another inverse system of sets relative to $I$, let $v_\alpha$ be an inverse system of mappings of $(B_\alpha,\psi_{\alpha\beta})$ into $(C_\alpha,\theta_{\alpha\beta})$, and let $v=\underset{\longleftarrow}{\lim}\,v_\alpha$. Then we have $\underset{\longleftarrow}{\lim}\,(v_\alpha\mathbin{\circ}u_\alpha)=v\mathbin{\circ}u$.
Let $J$ be a cofinal subset of $I$, and suppose that $J$ is *directed* (with respect to the ordering induced from $I$). If $((E_\alpha)_{\alpha\in I},(f_{\alpha\beta})_{\alpha,\beta\in I})$ is an inverse system of sets relative to $I$, with inverse limit $E$, then $((E_\alpha)_{\alpha\in J},(f_{\alpha\beta})_{\alpha,\beta\in J})$ is also an inverse system of sets, relative to $J$. Let $E'$ be its inverse limit and let $f'_\alpha$ be the canonical mapping of $E'$ into $E_\alpha$, where $\alpha\in J$. For each $x\in E$ let $g(x)=(f_\alpha(x))_{\alpha\in J}\in E'$ (where $f_\alpha$ denotes the canonical mapping of $E$ into $E_\alpha$). Then $g$ is a *bijection* of $E$ onto $E'$, by means of which $E'$ is usually identified with $E$.

[^1]: In accordance with our point of view in this Summary of Results, we assume the theory of integers as known. But it should not be thought that this theory is necessary for building up the theory of sets; the reader will see, by referring to Chapter III that, on the contrary, the integers can be defined, and all their known properties proved, from the results of the theory of sets. In our terminology, $0$ belongs to $\mathbf{N}$.
[^2]: Thus, in our terminology, “less than” and “greater than” do not exclude “equal to”.
