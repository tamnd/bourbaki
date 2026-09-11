---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 2
section_title: Functions
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 351-357
pdf_pages: 0356-0362
extraction: ocr
statements: 0
exercises: 0
content_sha256: e080ea464bff6a7c05c7dc505f506fc7d9e94e4178becde6cca23d33e3bb7827
---

## 2. FUNCTIONS

1. Let E and F be two sets, which may or may not be distinct. A relation between a variable element $x$ of E and a variable element $y$ of F is called a *functional relation in $y$ if, for all $x \in E$, there exists a unique $y \in F$ which is in the given relation with $x$.*

We give the name of *function* to the operation which in this way associates with every element $x \in E$ the element $y \in F$ which is in the given relation with $x$; $y$ is said to be the *value* of the function at the element $x$, and the function is said to be *determined* by the given functional relation. Two *equivalent* functional relations determine the *same* function. Such a function is said to "take its values in F" and to be "defined on E". More briefly, it is also said to be a *mapping of* E *into* F.

2. The mappings of a set E into a set F are the *elements* of a new set, the *set of mappings of* E *into* F. If $f$ is any element of this set, the value of $f$ at the element $x$ of E is often denoted by $f(x)$. In some situations, the notation $f_x$ (called the *indicial* notation; the set E is then called the *index* set) is preferable. The relation "$y = f(x)$" is a functional relation in $y$, which determines $f$.

When a relation of the form $y = \langle x \rangle$ (where $\langle x \rangle$ denotes a combination of signs in which $x$ may appear) is a functional relation in $y$, the function it determines is often denoted by the notation $x \rightarrow \langle x \rangle$, or even simply by $\langle x \rangle$; this is a very common abuse of language. For example, if X and Y are two generic subsets of a set E, the relation $Y = \complement X$ is functional in Y; the mapping of $\mathfrak{P}(E)$ into $\mathfrak{P}(E)$ it determines is denoted by $X \rightarrow \complement X$, or simply by $\complement X$.

Instead of saying "let $f$ be a mapping of E into F", we shall often say, more simply, "let $f: E \rightarrow F$".

To describe a situation in which several mappings are involved, we shall also make use of *diagrams* such as

$$\begin{array}{ccccc}
 & & \mathrm{C} & & \\
 & \overset{g}{\nearrow} & & \overset{h}{\searrow} & \\
\mathrm{A} \overset{f}{\longrightarrow} \mathrm{B} & \underset{v}{\longrightarrow} & & & \mathrm{E} \\
\downarrow u & & & & \downarrow w \\
\mathrm{D} & \underset{t}{\longleftarrow} & & & \mathrm{F}
\end{array}$$

in which the letter attached to an arrow denotes a mapping of the set at the tail of the arrow into the set at its head.

The relation of equality "$f = g$" between mappings of E into F is equivalent to the relation "for all $x \in \mathrm{E}, f(x) = g(x)$".

3. A function, defined on a set E, which takes the same value $a$ for every element $x$ of E, is called a *constant* function on E; it is determined by the functional relation $y = a$.

The mapping of E into E which associates with each element $x$ of E this same element is called the *identity* mapping. It is determined by the functional relation $y = x$.

If A is any subset of E, the mapping of A into E which associates with each element $x$ of A the same element $x$ considered as an element of E is called the *canonical* mapping of A into E.

Let $f$ be a mapping of a set E into itself. An element $x$ of E is said to be *fixed* (or *invariant*) *under* $f$ if $f(x) = x$.

An element $x$ of E is said to be *fixed* (or *invariant*) under a set of mappings of E into E if it is fixed under each of them.

4. Let $f$ be a mapping of E into F and let X be any subset of E. Then the *image of* X *under* $f$ is the subset Y of F consisting of all elements $y$ which have the property "there exists $x \in$ E such that $x \in$ X and $f(x) = y$".

This defines a relation between X and Y which is functional in Y and therefore determines a mapping of $\mathfrak{P}(\mathrm{E})$ into $\mathfrak{P}(\mathrm{F})$. This mapping is called the *canonical extension of* $f$ *to sets of subsets;* by abuse of language it, too, is denoted by $f$, and we write $\mathrm{Y} = f(\mathrm{X})$.

For all $f$ and $x$ we have

$$f(\emptyset) = \emptyset \quad \text{and} \quad f(\{x\}) = \{f(x)\}.$$

By abuse of language, the *value* $f(x)$ of $f$ at $x$ is also called the *image of* $x$ *under* $f$.

If $y$ is a generic element of F, the property "$y \in f(\mathrm{E})$" may be expressed by saying that "$y$ *is of the form* $f(x)$".

By abuse of language, the image $f(\mathrm{E})$ of E under $f$ is sometimes called the *image of* $f$.

If we have $f(\mathrm{E}) = \mathrm{F}$, that is if for all $y \in$ F there exists $x \in$ E such that $y = f(x)$, then $f$ is said to be a mapping of E *onto* F, or a *surjective* mapping, or a *surjection*.

Let $x$ be any element and X any subset of E. Instead of saying that $f(x)$ is the value of $f$ at $x$, and $f(\mathrm{X})$ the image of X under $f$, it is sometimes said that $f$ *transforms* (or *maps*) $x$ into $f(x)$ and X into $f(\mathrm{X})$; $f(x)$ and $f(\mathrm{X})$ are then called the *transforms* by $f$ of $x$ and X, respectively.

If $f$ is a mapping of E into itself, a subset X of E is said to be *stable under* $f$ if $f(\mathrm{X}) \subset \mathrm{X}$. The subset X is said to be *stable* under a set of mappings of E into E if X is stable under each of these mappings.

5. Let $f$ be a mapping of E into F. Then we have the following propositions, in which X and Y denote arbitrary subsets of E :

(a) The relation $\mathrm{X} \subset \mathrm{Y}$ implies $f(\mathrm{X}) \subset f(\mathrm{Y})$.

(b) The property $\mathrm{X} \neq \emptyset$ is equivalent to $f(\mathrm{X}) \neq \emptyset$.

(c) For all X, Y we have

$$(11) \qquad f(\mathrm{X} \cup \mathrm{Y}) = f(\mathrm{X}) \cup f(\mathrm{Y}),$$

$$(12) \qquad f(\mathrm{X} \cap \mathrm{Y}) \subset f(\mathrm{X}) \cap f(\mathrm{Y}).$$

6. Let $f$ be a mapping of E into F, and let Y be any subset of F. The *inverse image of* Y *under* $f$ is the subset X of E consisting of all elements $x$ which have the property $f(x) \in \mathrm{Y}$.

This defines a relation between X and Y which is functional in X and therefore determines a mapping of $\mathfrak{P}(F)$ into $\mathfrak{P}(E)$, called the *inverse extension of f to sets of subsets*, and denoted by $\overset{-1}{f}$; thus we write $X = \overset{-1}{f}(Y)$.

In particular, if $y$ is an element of F, then $\overset{-1}{f}(\{y\})$ will be the set of all $x \in E$ such that $f(x) = y$. The relations "$f(x) = y$" and "$x \in \overset{-1}{f}(\{y\})$" are equivalent. By abuse of language we often write $\overset{-1}{f}(y)$ in place of $\overset{-1}{f}(\{y\})$.

The *trace* $X_A$ of a subset X of E on a given subset A is the inverse image of X under the canonical mapping of A into E (no. 3).

7. Let $f$ be a mapping of E into F. Then we have the following propositions, in which X and Y denote arbitrary subsets of F :

(a) The relation $X \subset Y$ implies $\overset{-1}{f}(X) \subset \overset{-1}{f}(Y)$.

(b) For all X, Y we have

(13) $$\overset{-1}{f}(X \cup Y) = \overset{-1}{f}(X) \cup \overset{-1}{f}(Y),$$

(14) $$\overset{-1}{f}(X \cap Y) = \overset{-1}{f}(X) \cap \overset{-1}{f}(Y),$$

(15) $$\overset{-1}{f}(\complement X) = \complement \overset{-1}{f}(X).$$

Note the difference between formulae (12) and (14); (14) would not be true for all X and Y if we replaced $\overset{-1}{f}$ by an arbitrary mapping of F into E. Again, there is no analogue of (15) for the extension of an arbitrary mapping.

Furthermore, we have $\overset{-1}{f}(\emptyset) = \emptyset$; but we can also have $\overset{-1}{f}(X) = \emptyset$ for a non-empty subset X of F. In order that $X \neq \emptyset$ should imply $\overset{-1}{f}(X) \neq \emptyset$, it is necessary and sufficient that $f$ should be a mapping of E *onto* F.

8. If a mapping $f$ of E into F is such that for all $y \in F$ there exists *at most one* $x \in E$ such that $y = f(x)$ (in other words, the set $\overset{-1}{f}(y)$ is either empty or consists of a single element), then $f$ is said to be a *one-to-one* mapping of E into F, or an *injective* mapping, or an *injection*. We have then, for all subsets X, Y of E,

(16) $$f(X \cap Y) = f(X) \cap f(Y).$$

9. If a mapping $f$ of E into F is such that for all $y \in F$ *there exists exactly one* $x \in E$ such that $y = f(x)$ (in other words, $\overset{-1}{f}(y)$ consists of a single element), then $f$ is said to be a *one-to-one* mapping of E *onto* F, or a *bijective* mapping, or a *bijection*. Such a mapping may be characterized as being both a mapping of E onto F and a *one-to-one* mapping of E into F.

If $f$ is a one-to-one mapping of E onto F, the relation $y=f(x)$ is not only functional in $y$, but also *functional in $x$. As a functional relation in $x$, it determines a one-to-one mapping of F onto E, called the *inverse* of the mapping $f$.

Note that the *extension of the inverse of $f$ is the same as the inverse of the extension of $f$.

Let $g$ be the inverse of $f$. Then the relations “$y=f(x)$” and “$x=g(y)$” are *equivalent*. The inverse of $g$ is $f$. If $f$ is a one-to-one mapping of E onto F, we have not only the relation (16) but also, for all subsets X of E,

$$f(\mathrm{C}X)=\mathrm{C}f(X).$$

Moreover, the extension of $f$ is a one-to-one mapping of $\wp(E)$ onto $\wp(F)$.

A one-to-one mapping of E onto F, together with its inverse mapping, are said to *realize a one-to-one correspondence between E and F*; alternatively, we say that E and F *are put in one-to-one correspondence by these mappings*.

A one-to-one mapping of a set E onto itself is called a *permutation* of E. The identity mapping is a permutation. If a permutation is identical with its inverse, it is said to be *involutory*; for example, the mapping $X\rightarrow \mathrm{C}X$ of $\wp(E)$ onto itself is involutory.

10. In the following propositions, X denotes an arbitrary subset of E, and Y an arbitrary subset of F:

(a) If $f$ is a mapping of E *into* F, we have

(17)
$$f^{-1}(Y)=f^{-1}(Y\cap f(E)),$$

(18)
$$X\subset f^{-1}(f(X)),$$

(19)
$$f(f^{-1}(Y))\subset Y.$$

(b) The properties “for all Y, $f(f^{-1}(Y))=Y$” and “$f$ is a mapping of E onto F” are *equivalent*.

(c) The properties “for all X, $f^{-1}(f(X))=X$” and “$f$ is a *one-to-one* mapping of E into F” are *equivalent*.

(d) The properties “for all X and Y,

$$f^{-1}(f(X))=X\qquad\text{and}\qquad f(f^{-1}(Y))=Y$$

and “$f$ is a *one-to-one* mapping of E onto F” are *equivalent*.

11. Let E, F, G be three sets, which may or may not be distinct. Let $f$ be a mapping of E into F, and let $g$ be a mapping of F into G. The mapping of E into G whose value at any element $x$ of E is $g(f(x))$ is called the *composition* of $g$ and $f$, and is denoted by $g \circ f$, or simply $gf$ if there is no risk of ambiguity.

The equality $h = g \circ f$ is called a *factorization* of $h$.

Note that, if G is distinct from E, we may not speak of the composition of $f$ and $g$ (in that order), and the notation $f \circ g$ has no meaning. If G is identical with E, then $f \circ g$ and $g \circ f$ are not elements of the same set unless F is also identical with E; and even when this is so, it is usually the case that $f \circ g \neq g \circ f$. Thus the *order* of composition of $f$ and $g$ is essential.

Let $\varphi$ be the composition of $g$ and $f$, let X be any subset of E, and let Z be any subset of G. Then we have

(20) $$\varphi(\mathrm{X}) = g(f(\mathrm{X})),$$
(21) $$\overset{-1}{\varphi}(\mathrm{Z}) = \overset{-1}{f}(\overset{-1}{g}(\mathrm{Z})).$$

If $f$ is a *one-to-one* mapping of E *onto* F, and if $g$ is a *one-to-one* mapping of F *onto* G, then $g \circ f$ is a *one-to-one* mapping of E *onto* G.

Let $h$ be a mapping of G into a set H. Then we have

$$h \circ (g \circ f) = (h \circ g) \circ f;$$

this mapping of E into H is written $h \circ g \circ f$, and is called the *composition* of the three mappings $h$, $g$, $f$ in this order. The composition of more than three mappings is defined similarly.

If $f$ is a mapping of E into itself, the *iterates* of $f$ are defined to be the mappings $f^n$ ($n$ an integer $\geqslant 1$) of E into itself, defined by induction on $n$ by means of the relations $f^1 = f$, $f^n = f^{n-1} \circ f$; $f^n$ is called the *nth iterate* of $f$. We have $f^{m+n} = f^m \circ f^n$.

12. In general, the composition $\overset{-1}{f} \circ f$ of the inverse extension and the extension of a mapping $f$ is not the identity mapping of $\mathfrak{P}(\mathrm{E})$ onto itself. Likewise, $f \circ \overset{-1}{f}$ is not usually the identity mapping of $\mathfrak{P}(\mathrm{E})$ onto itself. These two conditions are satisfied simultaneously only if $f$ is a *bijection* of E onto F.

If $f$ is a bijection of E onto F, and if $g$ denotes the inverse of $f$, then the compositions $g \circ f$ and $f \circ g$ are respectively the identity mapping of E onto E and the identity mapping of F onto F.

Conversely, if $f$ is a mapping of E into F, and $g$ a mapping of F into E, such that $g \circ f$ is a permutation of E and $f \circ g$ is a permutation of F, then $f$ is a bijection of E onto F and $g$ is a bijection of F onto E.

If, moreover, $g\circ f$ is the identity mapping of E onto itself, then $g$ is the inverse of $f$.

13. Let $f$ be a mapping of E into F, and let A be any subset of E. The mapping $f_A$ of A into F whose value at any element $x$ of A is $f(x)$ is called the *restriction of $f$ to the subset A*; it is just the composition of $f$ and the canonical mapping of A into E. If two mappings $f$, $g$ of E into F have the same restriction to A, they are said to *agree (or coincide)* on A. Conversely, $f$ is said to be an *extension* of $f_A$ to E.

14. A mapping of a set E *onto* a set F is also called a *parametric representation* of F *by means of* E; E is then called the *parameter set* of this representation, and the elements of E take the name of *parameters*.

A *family of elements* of a set F is by definition a subset of F endowed with a parametric representation; in other words, to be given a family of elements of F is equivalent to being given a mapping of some set E into F. The image of E under this mapping is called the *set of elements of the family*. Note that two distinct families of elements of F may have the same subset of F as the set of their elements.

With each subset A of a set F we may always associate a family of elements whose set of elements is A. It is enough to consider the family defined by the *canonical mapping* of A into F.

A family of elements of F, defined by a mapping $\iota\mapsto x_\iota$ of a set I into F, is denoted by $(x_\iota)_{\iota\in I}$, or simply $(x_\iota)$ if there is no possible ambiguity about the index set.

If J is a subset of I, the family $(x_\iota)_{\iota\in J}$ is called the *subfamily* corresponding to J of the family $(x_\iota)_{\iota\in I}$; it is defined by the restriction to J of the mapping $\iota\mapsto x_\iota$.
