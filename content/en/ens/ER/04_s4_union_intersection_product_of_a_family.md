---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 4
section_title: Union, intersection, product of a family of sets
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 363-370
pdf_pages: 0368-0375
extraction: ocr
statements: 0
exercises: 0
content_sha256: f9b5a61bff54537ebfed0e8bade3350c49d974cf5c55ab2cbce40ab5f4be65d9
---

## 4. UNION, INTERSECTION, PRODUCT OF A FAMILY OF SETS

1. In this section we consider a family $(X_i)_{i\in I}$ of subsets of a set $E$, in which the index set $I$ is arbitrary; the set of subsets of $E$ belonging to the family will be denoted by $\mathfrak{X}$ (which is therefore a subset of $\mathfrak{P}(E)$).

If $I$ is finite, the consideration of the family $(X_i)$ reduces to that of several subsets of $E$, which may or may not be distinct, and in number equal to the number of elements of $I$. For example, any three subsets $X_1,X_2,X_3$ of $E$ form a family of subsets of $E$, the index set here consisting of the numbers 1, 2, 3.

2. Let $J$ be any subset of $I$, and consider the set of all elements $x$ which have the property “there exists $i\in J$ such that $x\in X_i$”. This set is called the union of the family of sets $(X_i)_{i\in J}$, and is denoted by $\displaystyle\bigcup_{i\in J}X_i$.

We may also formulate this definition as follows: to the mapping $i\mapsto X_i$ of $I$ into $\mathfrak{P}(E)$ there corresponds a well-defined subset $C$ of $I\times E$ such that $X_i=C(i)$ (§ 3, no. 7), and we have $\displaystyle\bigcup_{i\in J}X_i=C(J)$.

In particular,

$$
\bigcup_{i\in\varnothing}X_i=C(\varnothing)=\varnothing .
$$

When $J=I$, we often write $\displaystyle\bigcup X_i$, or simply $\displaystyle\bigcup X_i$, in place of $\displaystyle\bigcup_{i\in I}X_i$.

The union $\displaystyle\bigcup_{i\in I}X_i$ depends only on the set $\mathfrak{X}$; in other words, it is the same for two families corresponding to the same subset $\mathfrak{X}$ of $\mathfrak{P}(E)$. In particular, it is equal to the union of the family defined by the canonical mapping of $\mathfrak{X}$ into $\mathfrak{P}(E)$, and we may therefore write $\displaystyle\bigcup_{X\in\mathfrak{X}}X$, which is also called the union of the sets belonging to $\mathfrak{X}$.

When $I$ is a set whose elements are explicitly designated, for example the numbers 1, 2, 3, we have

$$
\bigcup_{i\in I}X_i=X_1\cup X_2\cup X_3,
$$

which justifies the name “union” given in the general case to the set $\displaystyle\bigcup_{i\in I}X_i$.

# SUMMARY OF RESULTS

3. For any $J\subset I$ we have

$$
\bigcup_{\iota\in J}X_{\iota}\subset\bigcup_{\iota\in I}X_{\iota}.
$$

In particular, for all $\iota\in I$, we have

$$
X_{\iota}\subset\bigcup_{\iota\in I}X_{\iota}.
$$

Conversely, if $Y$ is a subset of $E$ such that $X_{\iota}\subset Y$ for all $\iota\in I$, then

$$
\bigcup_{\iota}X_{\iota}\subset Y.
$$

More generally, if $(Y_{\iota})$ is another family of subsets of $E$, indexed by the same set $I$, and if $X_{\iota}\subset Y_{\iota}$ for all $\iota\in I$, then

$$
\bigcup_{\iota}X_{\iota}\subset\bigcup_{\iota}Y_{\iota}.
$$

Let $F$ be another set, and let $X\to K(X)$ be the mapping of $\mathfrak{P}(E)$ into $\mathfrak{P}(F)$ defined by a subset $K$ of $E\times F$. Then we have

(34)

$$
K\left(\bigcup_{\iota\in J}X_{\iota}\right)=\bigcup_{\iota\in J}K(X_{\iota}).
$$

Now let $L$ be another index set, and $(J_{\lambda})_{\lambda\in L}$ a family of subsets of $I$. Then

(35)

$$
\bigcup_{\iota\in\bigcup_{\lambda\in L}J_{\lambda}}X_{\iota}
=
\bigcup_{\lambda\in L}\left(\bigcup_{\iota\in J_{\lambda}}X_{\iota}\right).
$$

This is the general *associativity* formula for unions. When $I$ and $L$ are sets whose elements are explicitly designated, the relations we obtain have already been given (see § 1, no. 14). If $L$ alone satisfies this condition and consists, say, of the numbers 1, 2, we have

(36)

$$
\bigcup_{\iota\in J_1\cup J_2}X_{\iota}
=
\left(\bigcup_{\iota\in J_1}X_{\iota}\right)\cup
\left(\bigcup_{\iota\in J_2}X_{\iota}\right).
$$

Let $(X_{\iota})_{\iota\in I}$ and $(Y_{\chi})_{\chi\in K}$ be any two families of subsets of $E$. Then we have

(37)

$$
\left(\bigcup_{\iota\in I}X_{\iota}\right)\cap
\left(\bigcup_{\chi\in K}Y_{\chi}\right)
=
\bigcup_{(\iota,\chi)\in I\times K}(X_{\iota}\cap Y_{\chi}).
$$

the *distributivity* formula, which includes the second formula of (10) as a particular case.

If $(X_i)_{i\in I}$ is a family of subsets of E, and if $(Y_x)_{x\in K}$ is a family of subsets of F, then

(38)

$$
\left(\bigcup_{i\in I}X_i\right)\times\left(\bigcup_{x\in K}Y_x\right)=\bigcup_{(i,x)\in I\times K}(X_i\times Y_x).
$$

4. A family $(X_i)_{i\in I}$ of subsets of E is a *covering* of a subset A of E, or covers A, if

$$
A\subset\bigcup_{i\in I}X_i.
$$

In particular, if $(X_i)$ is a covering of E, we have

$$
\bigcup_{i\in I}X_i=E.
$$

A *partition* of E is a covering $(X_i)$ of E such that

(a) $X_i\neq\varnothing$ for all $i\in I$;

(b) $X_i\cap X_j=\varnothing$ for each pair of *different* indices $i,\ j$ in I. (This second condition may be expressed by saying that the $X_i$ are *pairwise disjoint*.)

These conditions imply that $i\mapsto X_i$ is a *bijection* of I onto the set $\mathfrak{P}$ of subsets of the partition. Hence, if $\mathfrak{P}$ is given, the family is determined to within a one-to-one correspondence of index sets. In particular, a partition may be considered indifferently as a set of subsets or as a *family* of subsets.

5. Let $(X_i)_{i\in I}$ be any family of non-empty subsets of a set E. In the product $I\times E$, let $X'_i$ denote the subset $\{i\}\times X_i$ for each $i\in I$. The set

$$
S=\bigcup_{i\in I}X'_i
$$

is called the *sum* of the family $(X_i)_{i\in I}$. It is clear that the family $(X'_i)_{i\in I}$ is a partition of S and that for each $i\in I$ the mapping $x_i\mapsto(i,x_i)$ is a bijection of $X_i$ onto $X'_i$. By abuse of language, any set in one-to-one correspondence with S is often called the sum of the family $(X_i)_{i\in I}$, and the $X_i$ are usually identified with the subsets of this set to which they correspond.

The sum of two non-empty sets E and F is often said to be obtained by *adjoining* the set F to E.

6. With the notation of no. 2, the set of elements $x$ of E which have the property “for all $i\in J$, $x\in X_i$” is called the *intersection of the family of sets*

$(X_\iota)_{\iota\in J}$, and is denoted by $\displaystyle\bigcap_{\iota\in J}X_\iota$; when $J=I$, we often write $\displaystyle\bigcap_\iota X_\iota$, or simply $\displaystyle\cap X_\iota$, instead of $\displaystyle\bigcap_{\iota\in I}X_\iota$.

We have

(39)
$$
\mathrm{C}\left(\bigcup_{\iota\in J}X_\iota\right)=\bigcap_{\iota\in J}(\mathrm{C}X_\iota).
$$

In particular, if $J=\varnothing$,

(40)
$$
\bigcap_{\iota\in\varnothing}X_\iota=E.
$$

The intersection $\displaystyle\bigcap_\iota X_\iota$ depends only on the set $\mathfrak{F}$, and may be written $\displaystyle\bigcap_{X\in\mathfrak{F}}X$. For example, if $I$ consists of the numbers $1$, $2$, $3$, we have

$$
\bigcap_\iota X_\iota=X_1\cap X_2\cap X_3.
$$

7. Formula (39) allows us to generalize the *duality rule*. If a subset A of E is obtained from other subsets X, Y, Z and families $(X_\iota)$, $(Y_\iota)$, $(Z_\lambda)$ of subsets of E by applying (in any order) *only* the operations $\mathrm{C}$, $\cup$, $\cap$, $\displaystyle\bigcup$, $\displaystyle\bigcap$, then we shall obtain the complement $\mathrm{C}A$ by replacing the subsets X, Y, Z, $X_\iota$, $Y_\iota$, $Z_\lambda$ by their complements, and the operations $\cup$, $\cap$, $\displaystyle\bigcup$, $\displaystyle\bigcap$ by $\cap$, $\cup$, $\displaystyle\bigcap$, $\displaystyle\bigcup$, respectively, the order of operations being preserved; of course, the operations of intersection and union are not to be altered where they apply to *index* sets written under the signs $\displaystyle\bigcup$ and $\displaystyle\bigcap$.

As in § 1, no. 15, we define the *dual* of a relation A = B or A $\subset$ B where A and B are subsets of E of the above form.

8. For all $J\subset I$ we have

$$
\bigcap_{\iota\in I}X_\iota\subset\bigcap_{\iota\in J}X_\iota.
$$

In particular, for all $x\in I$ we have

$$
\bigcap_\iota X_\iota\subset X_x.
$$

Conversely, if $Y\subset X_\iota$ for all $\iota\in I$, then

$$
Y\subset\bigcap_\iota X_\iota.
$$

More generally, if $(Y_i)$ is another family of subsets of E, indexed by the same set I, and if $X_i\subset Y_i$ for all $i\in I$, then

$$\bigcap_{i}X_i\subset\bigcap_iY_i.$$

The union of the sets $X_i$ is the intersection of all sets $Y$ such that $X_i\subset Y$ for all $i\in I$. The intersection of the $X_i$ is the union of all $Z$ such that $Z\subset X_i$ for all $i\in I$.

The following formulae are the duals of (35) and (37), respectively:

(41)

$$\bigcap_{i\in\bigcup_{\lambda\in L}J_\lambda}X_i=\bigcap_{\lambda\in L}\left(\bigcap_{i\in J_\lambda}X_i\right)\qquad\text{(associativity)};$$

(42)

$$\left(\bigcap_{i\in I}X_i\right)\cup\left(\bigcap_{x\in K}Y_x\right)=\bigcap_{(i,x)\in I\times K}(X_i\cup Y_x)\qquad\text{(distributivity)}.$$

If $(X_i)_{i\in I}$ is a family of subsets of E, and $(Y_x)_{x\in K}$ a family of subset of F, then

(43)

$$\left(\bigcap_{i\in I}X_i\right)\times\left(\bigcap_{x\in K}Y_x\right)=\bigcap_{(i,x)\in I\times K}(X_i\times Y_x).$$

Moreover, if $(X_i)$ and $(Y_i)$ are families of subsets of E and F, respectively, indexed by the same set I, then

(44)

$$\left(\bigcap_{i\in I}X_i\right)\times\left(\bigcap_{i\in I}Y_i\right)=\bigcap_{i\in I}(X_i\times Y_i).$$

The formula (34) has no dual; in general all we can say is

(45)

$$K\left(\bigcap_{i\in J}X_i\right)\subset\bigcap_{i\in J}K(X_i).$$

We have equality in (45) for all families $(X_i)$ only if $X\mapsto K(X)$ is the inverse extension of a mapping of a subset of F into E. Consequently, if $f$ is a mapping of F into E, we have (generalizing (14))

(46)

$$\overline{f}^{\, -1}\left(\bigcap_{i\in J}X_i\right)=\bigcap_{i\in J}\overline{f}^{\, -1}(X_i).$$

9. Let E be any set and let I be any index set. The set of all families $(x_i)_{i\in I}$ of elements of E, indexed by I, is denoted by $E^I$, and the operation of passing from E to $E^I$ is called exponentiation. $E^I$ is thus in one-to-one correspondence with the set of all mappings of I into E (which for this reason is often denoted by $E^I$, by abuse of language), as well as with a subset of $\mathfrak{P}(I \times E)$, by considering the graphs of these mappings. The sets $E^J$ corresponding to subsets $J$ of the set I may therefore be considered all as subsets of the same set, which is in one-to-one correspondence with a subset of $\mathfrak{P}(I \times E)$.

Now let $(X_\ell)_{\ell\in I}$ be a *family of subsets* of E, indexed by the same set I, and let J be any subset of I. The property “for all $\ell\in J$, $x_\ell\in X_\ell$,” of the family $(x_\ell)_{\ell\in J}$ defines a subset of $E^J$, called the *product of the family of sets* $(X_\ell)_{\ell\in J}$, and denoted by $\displaystyle\prod_{\ell\in J} X_\ell$ (or simply $\displaystyle\prod_\ell X_\ell$ when $J=I$). The $X_\ell$ are called the *factors* of the product. Note that $\displaystyle\prod_{\ell\in\varnothing} X_\ell$ is a set consisting of one element (corresponding to the empty subset of $I\times E$). If $X_\ell=E$ for all $\ell\in J$, then we have

$$
\prod_{\ell\in J} X_\ell=E^J.
$$

If, for example, I consists of the three numbers 1, 2, 3, then $\displaystyle\prod_{\ell\in J} X_\ell$ is in one-to-one correspondence with the set $X_1\times X_2\times X_3$.

10. If $R\{x,y\}$ is a relation between a generic element $x$ of a set E and a generic element $y$ of a set F, then the following propositions are *equivalent*:

“for each $x$ there exists $y$ such that $R\{x,y\}$”

and

“there exists a mapping $f$ of E into F such that $R\{x,f(x)\}$ for all $x”$.

The assertion of this equivalence is known as the *axiom of choice* (or *Zermelo’s axiom*). We shall sometimes indicate whether the proof of a theorem depends on it.

The axiom of choice is *equivalent* to the following proposition : “if, for each $\ell\in I$, we have $X_\ell\ne\varnothing$, then $\displaystyle\prod_{\ell\in I}X_\ell\ne\varnothing$”.

11. In this and the following subsection, we shall consider a non-empty product $\displaystyle\prod_{\ell\in I}A_\ell$, where $(A_\ell)$ is any *family* of (non-empty) subsets of E.

Let J be a subset of I. The mapping $(x_\ell)_{\ell\in I}\to(x_\ell)_{\ell\in J}$ of $\displaystyle\prod_{\ell\in I}A_\ell$ onto $\displaystyle\prod_{\ell\in J}A_\ell$ is called the *projection* of $\displaystyle\prod_{\ell\in I}A_\ell$ onto $\displaystyle\prod_{\ell\in J}A_\ell$, and is denoted by $\operatorname{pr}_J$.

In particular, the mapping $(x_\ell)_{\ell\in I}\to x_\kappa$ of $\displaystyle\prod_{\ell\in I}A_\ell$ onto $A_\kappa$ is called the *coordinate function* (or *projection*) of *index* $\kappa$, and is denoted by $\operatorname{pr}_\kappa$.

If $z$ is an element of $\displaystyle\prod_{\ell\in I}A_\ell$, we have $z=(\operatorname{pr}_\ell z)_{\ell\in I}$.

Let $J_1, J_2$ be two sets forming a partition of $I$. Then $z\mapsto(\operatorname{pr}_{J_1}z,\operatorname{pr}_{J_2}z)$ is a one-to-one mapping of $\prod_{i\in I}A_i$ onto $\prod_{i\in J_1}A_i\times\prod_{i\in J_2}A_i$.

In general, if $(J_\lambda)_{\lambda\in L}$ is any partition of the set $I$, the mapping $z\mapsto(\operatorname{pr}_{J_\lambda}z)_{\lambda\in L}$ is a bijection (called canonical) of $\prod_{i\in I}A_i$ onto the product $\prod_{\lambda\in L}(\prod_{i\in J_\lambda}A_i)$. This may also be expressed by saying that the product of a family of sets is associative.

12. The following propositions generalize those of §3, no. 3; $(X_i)$, $(Y_i)$ denote families of subsets of $E$ such that $X_i\subset A_i$, and $Y_i\subset A_i$, for all $i\in I$; $Z$ denotes any subset of $\prod A_i$.

(a) If $\prod_iX_i\neq\varnothing$, the relation “$\prod_iX_i\subset\prod_iY_i$” is equivalent to “for all $i\in I$, $X_i\subset Y_i$”.

(b) We have $\operatorname{pr}_x^{-1}(X_x)=\prod_iY_i$, where $Y_x=X_x$ and $Y_i=A_i$ whenever $i\neq x$. Hence

$$
\prod_{i\in I}X_i=\bigcap_{i\in I}\operatorname{pr}_i^{-1}(X_i).
$$

(c) If $\prod_iX_i\neq\varnothing$, then

$$
\operatorname{pr}_x\left(\prod_iX_i\right)=X_x.
$$

(d) For all $Z$ we have

$$
Z\subset\prod_i\operatorname{pr}_i(Z).
$$

(e) Let $(J_1,J_2)$ be a partition of $I$ into two sets, let $(a_i)_{i\in J_1}$ be a family of elements of $E$, and let $(X_i)_{i\in J_2}$ be a family of subsets of $E$, such that $a_i\in A_i$ for all $i\in J_1$, and $X_i\subset A_i$ for all $i\in J_2$. Then the product $\prod_iY_i$, where $Y_i=\{a_i\}$ when $i\in J_1$, and $Y_i=X_i$ when $i\in J_2$, can be put in one-to-one correspondence with $\prod_{i\in J_2}X_i$ by projecting onto this latter set.

13. Let $(A_i)_{i\in I}$ be a family of subsets of a set $F$, and let $f$ be a mapping of a set $E$ into the product $\prod_iA_i$. If we put $f_i(x)=\operatorname{pr}_i(f(x))$, then $f_i$ is a mapping of $E$ into $A_i$, and $f$ is the mapping $x\mapsto(f_i(x))$. Conversely, if for each index $i\in I$, $f_i$ is a mapping of $E$ into $A_i$, then

$$
x\mapsto(f_i(x))
$$

is a mapping of E into $\prod_{i\in I} A_i$, which is denoted by $(f_i)$ (by abuse of language, because this notation already denotes the family of mappings $f_i$). Thus we define a bijection (called canonical) of the set $(\prod_{i\in I} A_i)^E$ onto the set $\prod_{i\in I}(A_i^E)$.

14. Let E, F, G be three sets. For each mapping $f$ of $F \times G$ into $E$ and for each $y\in G$, let $f_y$ denote the partial mapping $x\mapsto f(x,y)$ of $F$ into $E$. Then $y\mapsto f_y$ is a mapping of $G$ into $E^F$. Conversely, for each mapping $g$ of $G$ into $E^F$ there exists a unique mapping $f$ of $F\times G$ into $E$ such that $f_y=g(y)$ for all $y\in G$. Thus we define a bijection (called canonical) of the set $E^{F\times G}$ onto the set $(E^F)^G$.

15. Let $(A_i)_{i\in I}$ be a family of non-empty subsets of a set E. For each $i\in I$ let $f_i$ be a mapping of $A_i$ into a set F such that, for each pair of indices $(i,x)$, $f_i$ and $f_x$ agree on $A_i\cap A_x$. Then, if

$$
A=\bigcup_{i\in I}A_i,
$$

there exists a unique mapping $f$ of A into F such that the restriction of $f$ to each $A_i$ is equal to $f_i$. In particular, if $A_i\cap A_x=\varnothing$ whenever $i\ne x$, we see that sets $F^A$ and $\prod_{i\in I}F^{A_i}$ are in one-to-one correspondence (called canonical).
