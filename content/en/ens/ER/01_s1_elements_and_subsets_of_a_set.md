---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 1
section_title: Elements and subsets of a set
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 347-351
pdf_pages: 0352-0356
extraction: ocr
statements: 0
exercises: 0
content_sha256: 0e243e5f12383731f0a5a2c71334e71b3cefa638eb23c7b52b81096a04bed198
---

## 1. ELEMENTS AND SUBSETS OF A SET

1. A *set* consists of *elements* which are capable of possessing certain *properties* and of having certain *relations* between themselves or with elements of other sets.

2. Sets and elements are denoted in mathematical arguments by graphical symbols, which in general are letters (from various alphabets) or combinations of letters and other signs. Relations between elements of one or more sets are denoted by inserting the symbols which denote these elements into a scheme characteristic of the relation considered [^1]; and similarly for properties.

A letter may denote either a *fixed* element or an *arbitrary* element (also called a *variable*, an *argument*, or a *generic* element) of a set. When an arbitrary element is replaced by a fixed element in a relation (or property), the arbitrary element is said to be given this fixed element as *value*.

In order to indicate the elements which appear in a relation which is not explicitly written down, we represent the relation by a notation such as $\mathrm{R}\{x, y, z\}$ (if $x, y, z$ are the elements in question).

3. A relation or a property in which arbitrary elements feature [^2] is said to be an *identity* if it becomes a true proposition whatever values we give to these arbitrary elements. If R and S denote two relations (or properties), R is said to *imply* S if S is true whenever the arbitrary elements which enter in these relations are fixed in such a way that R is true. The relations (or properties) R and S are said to be *equivalent* if each implies the other.

4. Let $\mathrm{R}\{x,\ y,\ z\}$ be a relation between the variables $x$, $y$, $z$. The phrase "for all $x$, $\mathrm{R}\{x,\ y,\ z\}$" is a relation *between $y$ and $z$*, which will be considered to be true for a system of given values of these latter variables if R is true for these values of $y$ and $z$ and *every* value of $x$. The phrase "there exists $x$ such that $\mathrm{R}\{x,\ y,\ z\}$" (or "for some $x$, $\mathrm{R}\{x,\ y,\ z\}$") is again a relation between $y$ and $z$, which will be considered to be true for a system of given values of $y$ and $z$ if, these variables being thus fixed, there is *at least one* value of $x$ for which R is true. Similarly for a relation between any number of variables.

If $\overline{\mathrm{R}}$ denotes the *negation* of R, then the negation of "for all $x$, R" is "there exists $x$ such that $\overline{\mathrm{R}}$"; the negation of "there exists $x$ such that R" is "for all $x$, $\overline{\mathrm{R}}$".

5. If R, S denote two relations, we regard "R and S" as a *single* relation, which is considered as true whenever *both* R *and* S are true. Likewise, "R or S" is a relation which is considered to be true whenever *at least one* of the relations R, S is true (and, in particular, whenever they are both true. The word "or" thus does not have the disjunctive sense here which it sometimes has in ordinary speech). Let $\overline{\mathrm{R}}$, $\overline{\mathrm{S}}$ denote the negations of R, S, respectively. Then the negation of "R and S" is "$\overline{\mathrm{R}}$ or $\overline{\mathrm{S}}$", and the negation of "R or S" is "$\overline{\mathrm{R}}$ and $\overline{\mathrm{S}}$".

6. By writing two symbols one on each side of the sign "$=$" (read "equals"), we have a relation called the relation of *equality*, which means that the two symbols represent the *same* element. The negation of this relation is obtained by writing the same symbols one on each side of the sign "$\neq$" (read "is not equal to" or "is different from").

7. Given a set E and a *property* of a generic element of E, those of the elements of E which have this property form a new set, called a *subset* of E. Two *equivalent* properties therefore define the *same* subset of E, and conversely.

Let A be a subset of E. When $x$ is a generic element of E, the property "$x$ belongs to A" (i.e., "$x$ is an element of A") is written "$x \in A$"; the set of elements which have this property is clearly just A.

The negation of this property is written "$x \notin A$" (read "$x$ does not belong to A"); the set of elements of E which have this property is called the *complement* of A and is written $\complement A$ or $E - A$.

8. Some properties, for example $x = x$, are true for *all* elements of E. Any two such properties are equivalent, and the subset they define is the set E itself.

On the other hand, some properties, for example $x \neq x$, are not true for *any* element of E. Again, any two such properties are equivalent, and the subset they define is called the *empty subset* of E, which is denoted by $\emptyset$.

Note that E and $\emptyset$ are *complements* of each other.

9. Let $a$ be a determinate element of E. Some properties, for example $x = a$, are true only for the *single* element $a$. Any two such properties are equivalent; the subset they define is denoted by $\{a\}$, and is called the subset *consisting of a alone*.

10. The set whose elements are all the *subsets* of a set E is called the *set of subsets* of E, and is denoted by $\mathfrak{P}(E)$. We have $\emptyset \in \mathfrak{P}(E)$, $E \in \mathfrak{P}(E)$, and $\{x\} \in \mathfrak{P}(E)$ for all $x \in E$. If $x$ denotes a generic element of E, and X a generic element of $\mathfrak{P}(E)$, the relation "$x \in X$" between $x$ and X is called the *relation of membership*.

11. Let $x$ and $y$ be two elements of E and let X be a generic element of $\mathfrak{P}(E)$. Then the relation of equality "$x = y$" is *equivalent* to the relation "for all X such that $x \in X$, we have $y \in X$".

12. Let X, Y be two subsets of a set E. If the property $x \in X$ implies the property $x \in Y$, in other words if every element of X belongs to Y, then we say that X is *contained in* Y, or that Y *contains* X, or that X *is a subset of* Y. This relation between X and Y is called the relation of *inclusion* (of X in Y), and is denoted by "$X \subset Y$" or "$Y \supset X$". Its negation is denoted by "$X \not\subset Y$" or "$Y \not\supset X$".

For all subsets X of E we have $\emptyset \subset X$ and $X \subset E$. The relation of membership "$x \in X$" is equivalent to "$\{x\} \subset X$".

The relation "$X \subset Y$ and $Y \subset Z$" implies "$X \subset Z$".

The relation "$X \subset Y$" does not exclude the possibility of "$X = Y$". The relation "$X \subset Y$ and $Y \subset X$" is equivalent to "$X = Y$".

13. Let X and Y be any two subsets of E. The set of all elements which have the property "$x \in X$ or $x \in Y$" is denoted by $X \cup Y$ and is called the *union* of X and Y. The set of all elements which have the property "$x \in X$ and $x \in Y$" is denoted by $X \cap Y$ and is called the *intersection* of X and Y.

The union and intersection of several subsets of E are defined in the same way.

If $x$, $y$, $z$ are three elements of E, the union $\{x\} \cup \{y\} \cup \{z\}$ is denoted by $\{x, y, z\}$. Similarly for any number of (individually named) elements.

Let X and Y be two subsets of E. According as $X \cap Y \neq \emptyset$ or $X \cap Y = \emptyset$, we say that X and Y *intersect* or are *disjoint*.

14. In the statements of the following propositions, X, Y, Z denote any subsets of the same set E.

(a) We have $\emptyset = \complement E$, $\quad E = \complement \emptyset$.

(b) For all X we have

(1)
$$\complement(\complement X) = X;$$

(2)
$$X \cup X = X, \qquad X \cap X = X;$$

(3)
$$X \cup (\complement X) = E, \qquad X \cap (\complement X) = \emptyset;$$

(4)
$$X \cup \emptyset = X, \qquad X \cap E = X;$$

(5)
$$X \cup E = E, \qquad X \cap \emptyset = \emptyset.$$

(c) For all X, Y we have

(6)
$$X \cup Y = Y \cup X, \qquad X \cap Y = Y \cap X \quad \text{(commutativity)};$$

(7)
$$X \subset X \cup Y, \qquad X \cap Y \subset X;$$

(8)
$$\complement(X \cup Y) = (\complement X) \cap (\complement Y), \qquad \complement(X \cap Y) = (\complement X) \cup (\complement Y).$$

(d) The relations $X \subset Y$, $\complement X \supset \complement Y$, $X \cup Y = Y$, $X \cap Y = X$ are *equivalent*.

(e) The relations $X \cap Y = \emptyset$, $X \subset \complement Y$, $Y \subset \complement X$ are *equivalent*.

(f) The relations $X \cup Y = E$, $\complement X \subset Y$, $\complement Y \subset X$ are *equivalent*.

(g) For all X, Y, Z we have

(9)
$$\left.\begin{array}{l} X \cup (Y \cup Z) = (X \cup Y) \cup Z = X \cup Y \cup Z \\ X \cap (Y \cap Z) = (X \cap Y) \cap Z = X \cap Y \cap Z \end{array}\right\} \quad \text{(associativity)};$$

(10)
$$\left.\begin{array}{l} X \cup (Y \cap Z) = (X \cup Y) \cap (X \cup Z) \\ X \cap (Y \cup Z) = (X \cap Y) \cup (X \cap Z) \end{array}\right\} \quad \text{(distributivity)}.$$

(h) The relation "$X \subset Y$" implies the relations "$X \cup Z \subset Y \cup Z$" and "$X \cap Z \subset Y \cap Z$".

(i) The relation "$Z \subset X$ and $Z \subset Y$" is equivalent to "$Z \subset X \cap Y$". The relation "$X \subset Z$ and $Y \subset Z$" is equivalent to "$X \cup Y \subset Z$".

15. From the identities (8) we conclude that if a subset A of E is obtained from other subsets X, Y, Z of E by applying *only* the operations $\complement$, $\cup$, $\cap$ (in any order), then the complement $\complement A$ can be obtained by replacing the subsets X, Y, Z by their respective complements, and the operations $\cup$, $\cap$ by $\cap$, $\cup$, respectively, while preserving the order of the operations. This is the *duality rule*. Given an equality $A = B$ between subsets of the above form, consider the equivalent equality $\complement A = \complement B$. If we replace $\complement A$ and $\complement B$ by the expressions obtained by applying the duality rule, and if then we replace $\complement X$, $\complement Y$, $\complement Z$ by X, Y, Z, respectively, and vice versa, we obtain an equality called the *dual* of $A = B$. We can do the same for an inclusion relation $A \subset B$, but then we must take care to replace the sign " $\subset$ " by " $\supset$ ".

The identities above which carry the same number are duals of each other.

16. In certain questions we have to consider a fixed subset A of a set E. If X is any arbitrary subset of E, the set $A \cap X$ is called the *trace* of X on A, and is sometimes denoted by $X_A$; it is considered, in this case, as a subset of A. For all subsets X, Y of E we have

$$(X \cup Y)_A = X_A \cup Y_A, \qquad (X \cap Y)_A = X_A \cap Y_A,$$

and
$$\complement_A X_A = (\complement_E X)_A,$$

where $\complement_E X$ denotes the complement of X in E and $\complement_A X_A$ denotes the complement of $X_A$ in A.

If $\mathfrak{S}$ denotes a set of subsets of E, then the set $\mathfrak{S}_A$ of the traces on A of the sets of $\mathfrak{S}$ is called the *trace* of $\mathfrak{S}$ on A.

[^1]: When the symbol which denotes an element is a combination of several signs and is to be inserted into a relation in the place of a single letter, it is customary to put it in brackets in order to avoid possible confusion.
[^2]: It should be emphasized that, when we speak of a *property of a generic* element of a set E, this in no way implies that the property is true for *every* element of E, but simply that it *has a meaning* for *every* element of E; it may be true for some of these elements and false for others. Similarly for relations.
