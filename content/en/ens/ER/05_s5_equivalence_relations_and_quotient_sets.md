---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 5
section_title: Equivalence relations and quotient sets
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 370-373
pdf_pages: 0375-0378
extraction: ocr
statements: 0
exercises: 0
content_sha256: 22c94bcb3e3db436839b071a4604607950bd9f8394f1a692c4accc6bc0101dd5
---

## 5. EQUIVALENCE RELATIONS AND QUOTIENT SETS

1. Let $(A_i)_{i\in I}$ be a partition of a set E. The relation $R\{x,y\}$: “there exists $i\in I$ such that $x\in A_i$ and $y\in A_i$,” between two generic elements $x,y$ of E satisfies the following conditions :

(a) $R\{x,x\}$ is an identity (reflexivity of R).

(b) $R\{x,y\}$ and $R\{y,x\}$ are equivalent (symmetry of R).

(c) The relation $R\{x,y\}$ and $R\{y,z\}$ implies $R\{x,z\}$ (transitivity of R).

If C denotes the subset of $E\times E$ defined by the relation R, the conditions (a), (b), (c) are respectively equivalent to the following conditions : $(a')\ \Delta\subset C$; $(b')\ \overline{C}=C$; $(c')\ C\circ C\subset C$. From $(a')$ and $(c')$ it follows that $C\circ C=C$.

2. Conversely, let $R\{x,y\}$ be a reflexive, symmetric, and transitive relation, and let C be its graph in $E\times E$. Then the image $\mathfrak{P}$ of E under the mapping $x\mapsto C(x)$ of E into $\mathfrak{P}(E)$ is a partition of E, and the relation “there exists a subset X ∈ 𝔖̃ such that x ∈ X and y ∈ X” is equivalent to
$R\{x,y\}$.

Every relation which satisfies conditions (a), (b), and (c) is called an equivalence relation on E. The partition 𝔖̃ which it defines, considered as a subset of 𝒫(E), is called the quotient set of E by the relation R, and is denoted by E/R; its elements are called equivalence classes with respect to R. The mapping $x \mapsto C(x)$ of E onto E/R, which maps each element x of E to the equivalence class which contains x, is called the canonical mapping of E onto E/R.

The relation of equality $x = y$ is an equivalence relation. The canonical mapping of E onto the corresponding quotient set is just $x \mapsto \{x\}$, and is bijective.

If R is an equivalence relation, the notation “$x \equiv y$ (mod R)” is sometimes used as a synonym for $R\{x,y\}$; it is read “x is equivalent to y modulo R”.

3. On a product set $E \times F$, the relation “$\operatorname{pr}_1 z = \operatorname{pr}_1 z'$” between z and z′ is an equivalence relation R, and the quotient set $(E \times F)/R$ can be put in one-to-one correspondence with E (this is the origin of the name quotient set).

More generally, let f be a mapping of a set E into a set F. Then the relation “$f(x)=f(y)$” is an equivalence relation on E. If we denote this relation by R, the mapping $z \mapsto f^{-1}(z)$ (where $f^{-1}(z)$ is considered as an element of E/R) is a bijection of $f(E)$ onto E/R.

It follows that f may be considered as the composition of the following three mappings, in the given order:
(1) the canonical mapping of the subset $f(E)$ of F into the set F;
(2) the bijective mapping of E/R onto $f(E)$, whose inverse has just been defined;
(3) the canonical mapping of E onto E/R.

This decomposition of a mapping is called its canonical decomposition or canonical factorization.

4. Every equivalence relation R on a set E may be defined by means of a mapping as in the previous subsection; for, if C is the graph of R, the relation “$C(x)=C(y)$” is equivalent to $R\{x,y\}$.

5. Let R be an equivalence relation on a set E, and let A be a subset of E. Then the relation $R\{x,y\}$ between two generic elements x, y of A is an equivalence relation on A, called the relation induced by R on A, and denoted by $R_A$. Let f be the canonical mapping of E onto E/R and let g be that of A onto $A/R_A$. By making an element of E/R and an element of $A/R_A$ correspond if they are the images of the same element of E under f and g respectively, we have a one-to-one correspondence between the image $f(A)$ of A under f and the quotient set $A/R_A$. If φ denotes the canonical mapping of A into E, this correspondence is realized by the mapping $z \to f(\varphi(g^{-1}(z)))$ and its inverse, both of which are also called *canonical*.

6. A subset A of E is said to be *saturated* with respect to the equivalence relation R if for each $x \in A$ the equivalence class of $x$ with respect to R is contained in A. In other words, the saturated sets with respect to R are *unions of equivalence classes with respect to R*. If $f$ is the canonical mapping of E onto E/R, then a set is saturated if it is of the form $f^{-1}(X)$, where $X \subset E/R$.

Let A be a subset of E. The intersection of the saturated sets which contain A is $f^{-1}(f(A))$. This set may also be defined as the union of the equivalence classes of the elements of A, and is called the *saturation* of A (with respect to R).

7. Let $P\{x,y,z\}$ be a relation in which there appears a generic element $x$ of E. Then P is said to be *compatible* (in $x$) *with the equivalence relation* R if the relation “$P\{x,y,z\}$ and $x \equiv x'$ (mod R)” *implies* $P\{x',y,z\}$.

Let $f$ be the canonical mapping of E onto E/R, and let $t$ be a generic element of E/R. The relation “there exists $x \in f^{-1}(t)$ such that $P\{x,y,z\}$” is then equivalent to “for all $x \in f^{-1}(t)$, $P\{x,y,z\}$”; the latter is a relation between $t$, $y$, $z$, said to be *induced* by P *on passing to the quotient* (with respect to $x$). If we denote it by $P'\{t,y,z\}$, then $P\{x,y,z\}$ is equivalent to $P'\{f(x),y,z\}$.

There are analogous definitions for a relation involving any number of arguments, and for the case in which the relation is compatible with R in *several* of its arguments. For example, if A is a subset of E, to say that the relation “$x \in A$” is compatible (in $x$) with R is equivalent to saying that A is saturated with respect to R. If $\varphi$ is a mapping of E into a set F, to say that the functional relation “$y=\varphi(x)$” is compatible (in $x$) with R is to say that $\varphi$ is constant on each equivalence class with respect to R. Passing to the quotient, R therefore induces a relation between $y$ and a generic element $t$ of E/R; this relation is functional in $y$ and so determines a mapping $\varphi'$ of E/R into F, satisfying the identity $\varphi(x)=\varphi'(f(x))$.

8. Let R be an equivalence relation on a set E, let S be an equivalence relation on a set F, and let $f$ be a mapping of E into F. The mapping $f$ is said to be *compatible with R and S* if the relation $x \equiv x'$ (mod R) *implies* $f(x) \equiv f(x')$ (mod S). If $g$ is the canonical mapping of F onto F/S, then the composite function $g \circ f$ has the same value at all elements of an equivalence class $z$ with respect to R; if we denote this common value by $h(z)$, then $h$ is a mapping of E/R into F/S, and is said to be *induced by f on passing to the quotients*.

9. Let R be an equivalence relation on E, and let S be an equivalence relation on E/R. If $f$ is the canonical mapping of E onto E/R, then “$f(x)\equiv f(y)\pmod S$” is an equivalence relation T on E. An equivalence class with respect to T is therefore the union in E of equivalence classes with respect to R which are equivalent to each other with respect to S; and the relation “$x\equiv y\pmod R$” implies “$x\equiv y\pmod T$”. If $g$ and $\varphi$ are the canonical mappings of $E$ onto $E/R$ and $E/T$, respectively, we obtain a one-to-one correspondence (called canonical) between $(E/R)/S$ and $E/T$ by making an element of $(E/R)/S$ and an element of $E/T$ correspond to each other if they are the images of the same element of E under $g$ and $\varphi$, respectively.

Conversely, let R and T be two equivalence relations on E such that “$x\equiv y\pmod R$” implies “$x\equiv y\pmod T$”. Then T is compatible (in the sense of no. 7) with R, both in x and in y; by passing to the quotient $E/R$ (with respect to x and y), T induces an equivalence relation S on $E/R$. If $\varphi$ again denotes the canonical mapping of E onto $E/R$, the relation “$\varphi(x)=\varphi(y)\pmod S$” is equivalent to “$x\equiv y\pmod T$”. The equivalence relation S is called the quotient of T by R, and is denoted by T/R. From the previous paragraph we see that there exists a one-to-one correspondence (the canonical correspondence) between $(E/R)/(T/R)$ and $E/T$.

10. Now let E, F be any two sets, which may or may not be distinct. Let $\{x, y\}$ be an equivalence relation on E and let $\{z, t\}$ be an equivalence relation on F. Then the relation $\{x, y\}\times\{z, t\}$ between elements $(x,z)$ and $(y,t)$ of the product set $E\times F$ is an equivalence relation on $E\times F$, called the product of R by S, and denoted by $R\times S$. Every equivalence class with respect to $R\times S$ is the product of an equivalence class with respect to R and an equivalence class with respect to S. If u denotes a generic element of $E/R$, and v a generic element of $F/S$, then $(u,v)\mapsto u\times v$ is a bijection (called canonical) of $(E/R)\times(F/S)$ onto $(E\times F)/(R\times S)$.
