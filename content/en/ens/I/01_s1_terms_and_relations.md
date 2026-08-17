---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION OF FORMAL MATHEMATICS
section: 1
section_title: Terms and relations
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 15-23, 56
pdf_pages: 0022-0030, 0063-0063
extraction: ocr
subsections:
    - "no": 1
      title: SIGNS AND ASSEMBLIES
      page: 15
      pdf_page: 22
    - "no": 2
      title: CRITERIA OF SUBSTITUTION
      page: 18
      pdf_page: 25
    - "no": 3
      title: FORMATIVE CONSTRUCTIONS
      page: 19
      pdf_page: 26
    - "no": 4
      title: FORMATIVE CRITERIA
      page: 21
      pdf_page: 28
statements: 5
exercises: 6
content_sha256: f1edb54bf5badcc6a09214156341c4f9bad6948839b58b9a54ea7a9fd294886b
---

## 1. TERMS AND RELATIONS

### 1. SIGNS AND ASSEMBLIES

The *signs* of a mathematical theory $\mathscr{T}$ (*)[^1] are the following :

(1) The *logical signs* (†)[^2] : $\square$, $\tau$, $\vee$, $\neg$.
(2) The *letters*.

By letters we mean upper and lower case Roman letters, with or without accents. Thus $A$, $A'$, $A''$, $A'''$, ... are letters. At any place in the text it is possible to introduce letters other than those which have appeared in previous arguments.

(3) The *specific signs*, which depend on the theory under consideration.

In the theory of sets we shall use only the following three specific signs : $=$, $\in$, $\supset$.

An *assembly* in $\mathscr{T}$ is a succession of signs of $\mathscr{T}$ written next to one another; certain signs, other than letters, may be joined in pairs by bars above the line, which are called *links*. \*For example, in the Theory of Sets, in which $\in$ is a specific sign,

$$\overline{\overline{\tau \vee \neg \in \square} A' \in \square} A''$$

is an assembly.\*

The exclusive use of assemblies would lead to insuperable difficulties both for the printer and for the reader. For this reason current texts use abbreviating symbols (notably words of ordinary speech) which do not belong to formal mathematics. The introduction of such symbols is the object of *definitions*. Their use *is not indispensable to the theory*, and can often lead to confusion which only a certain familiarity with the subject will enable the reader to avoid.

*Examples*

#### Example 1 {#ens-i-s1-n1-exa-1 .statement tag=03P0}

The assembly $\vee 1$ is represented by $\Rightarrow$.

#### Example 2 {#ens-i-s1-n1-exa-2 .statement tag=03P1}

The following symbols represent assemblies (and very long ones at that) :

“3 and 4”

$$\varnothing$$

$$\mathbf{N}$$

$$\mathbf{Z}$$

“the real line”

“the $\Gamma$ function”

$$f\circ g$$

$$\pi=\sqrt{2}+\sqrt{3}$$

$$1\in 2$$

“Every finite division ring is a field”

“The zeros of $\zeta(s)$ other than $-2$, $-4$, $-6$, ... lie on the line

$$R(s)=1/2$$.”

In general, the symbol used to represent an assembly contains all the letters which appear in the assembly. Nevertheless, this principle can sometimes be infringed without risk of confusion. *For example, “the completion of X” represents an assembly which contains the letter X, but which also contains the letter which represents the set of entourages of the uniform structure of X. On the other hand,

$$\int_0^1 f(x)\,dx$$

represents an assembly in which the letter $x$ (and the letter $d$) do not appear; and the assemblies represented by $\mathbf{N}$, $\mathbf{Z}$, “the $\Gamma$ function” do not contain any letters.*

A *mathematical theory* (or simply a *theory*) contains rules which allow us to assert that certain assemblies of signs are *terms or relations* of the theory, and other rules which allow us to assert that certain assemblies are *theorems* of the theory.

The description of these rules, which will appear in this chapter, *does not belong to formal mathematics*; the rules involve assemblies which are more or less undetermined, for example undetermined letters. To

simplify the exposition it is convenient to denote such assemblies by less cumbersome symbols. We shall use, especially, combinations of signs (of a mathematical theory), bold-face italic letters (with or without indices or accents), and particular symbols, of which some examples will be given. *Since our object is only to avoid circumlocutions* (cf. note (*), § 3, no. 1, p. 28) we shall not enunciate strict general rules for the use of these symbols; the reader will be able to reconstruct without trouble the assembly in question, in each particular case. By abuse of language we shall often say that the symbols *are* assemblies, rather than that they *denote* assemblies : expressions such as “the assembly $A$” or “the letter $x$”, in the statements of the following rules, should therefore be replaced by “the assembly denoted by $A$” or “the letter denoted by $x$”.

Let $A$ and $B$ be assemblies. We shall denote by $AB$ the assembly obtained by writing the assembly $B$ on the right of the assembly $A$. We shall denote by $\vee A\neg B$ the assembly obtained by writing, from left to right, the sign $\vee$, the assembly $A$, the sign $\neg$, the assembly $B$. And so on.

Let $A$ be an assembly and let $x$ be a letter. We shall denote by $\tau_x(A)$ the assembly constructed as follows : form the assembly $\tau A$, link each occurrence of $x$ in $A$ to the $\tau$ written on the left of $A$, and then replace $x$ everywhere it occurs by the sign $\square$. The assembly denoted by $\tau_x(A)$ therefore *does not contain* $x$.

#### Example {#ens-i-s1-n1-exa-3 .statement tag=03RY}

The symbol $\tau_x(\in xy)$ represents the assembly

$$
\tau\in\square y.
$$

Let $A$ and $B$ be assemblies and let $x$ be a letter. The assembly obtained by replacing $x$, wherever it occurs in $A$, by the assembly $B$ is denoted by $(B\mathbin{|}x)\,A$ (read : $B$ replaces $x$ in $A$). If $x$ does not appear in $A$, then $(B\mathbin{|}x)\,A$ is identical with $A$; in particular,

$$
(B\mathbin{|}x)\,\tau_x(A)
$$

is identical with $\tau_x(A)$.

#### Example {#ens-i-s1-n1-exa-4 .statement tag=03TO}

If we replace $x$ by $\square$ wherever $x$ occurs in the assembly $\vee\in xy=xx$, we obtain the assembly $\vee\in\square y=\square\square$.

If $A$ is an assembly and we are interested particularly in a letter $x$, or two distinct letters $x$ and $y$ (which may or may not appear in $A$), we shall often write $A\{x\}$ or $A\{x,y\}$. In this case we write $A\{B\}$ instead of $(B\mathbin{|}x)\,A$. We denote by $A\{B,C\}$ the assembly obtained by *simultaneously* replacing $x$ by $B$ and $y$ by $C$ wherever they occur in $A$ (note that $x$ and $y$ may appear in $B$ and in $C$); if $x'$ and $y'$ are distinct letters, other than $x$ and $y$, which appear in neither $A$, $B$, nor $C$, then $A\{B,C\}$ is the same as $(B\mathbin{|}x')(C\mathbin{|}y')(x'\mathbin{|}x)(y'\mathbin{|}y)A$.

#### Remark {#ens-i-s1-n1-rem-1 .statement tag=03P2}

When an abbreviating symbol $\Sigma$ is introduced, by means of a definition, to represent a certain assembly, the (usually tacit) convention is made of representing the assembly obtained by substituting an assembly $B$ for a letter $x$ in the original assembly, by the symbol obtained by the replacing the letter $x$ in $\Sigma$ by the assembly $B$ (or, more often, by an abbreviating symbol representing the assembly $B$).

¶ *For example, having defined what assembly is represented by the symbol $E\otimes F$, where $E$ and $F$ are letters — an assembly which, incidentally, contains other letters besides $E$ and $F$ — the symbol $Z\otimes F$ can be used without further explanation.*

¶ This rule can lead to confusions, which are avoided by the use of various typographical devices; the most common consists in replacing $x$ by $(B)$ in place of $B$.

¶ *For example, $M\cap N$ denotes an assembly containing the letter $N$. If we substitute for $N$ the assembly represented by $P\cup Q$, we get an assembly denoted by $M\cap(P\cup Q)$.*

### 2. CRITERIA OF SUBSTITUTION

Formal mathematics contains only explicitly written assemblies. Nevertheless, even with the use of abbreviating symbols, the development of mathematics strictly in accordance with this principle would lead to extremely long chains of reasoning. For this reason we shall establish criteria relating to indeterminate assemblies; each of these criteria will describe once for all the final result of a definite sequence of manipulations on these assemblies. These criteria are therefore not indispensable to the theory; their justification belongs to metamathematics.

The development of metamathematics itself requires, in practice, the use of abbreviating symbols, some of which have already been indicated. Most of these symbols are also used in mathematics.

We shall make use of the following criteria, called the *criteria of substitution* :

CS1. Let $A$ and $B$ be assemblies and let $x$ and $x'$ be letters. If $x'$ does not appear in $A$, then $(B|x)A$ is identical with $(B|x')(x'|x)A$.

CS2. Let $A$, $B$, and $C$ be assemblies and let $x$ and $y$ be distinct letters (*)[^3]. If $y$ does not appear in $B$, then $(B|x)(C|y)A$ is identical with

$$(C'|y)(B|x)A,$$

where $C'$ is the assembly $(B|x)C$.

CS3. *Let $A$ be an assembly and let $x$ and $x'$ be letters. If $x'$ does not appear in $A$, then $\tau_x(A)$ is identical with $\tau_{x'}(A')$, where $A'$ is the assembly $(x'|x)\,A$.*

CS4. *Let $A$ and $B$ be assemblies and let $x$ and $y$ be distinct letters. If $x$ does not appear in $B$, then $(B|y)\tau_xA$ is identical with $\tau_x(A')$, where $A'$ is the assembly $(B|y)\,A$.*

CS5. *Let $A$, $B$, $C$ be assemblies and let $x$ be a letter. The assemblies $(C|x)(\neg A)$, $(C|x)(\vee AB)$, $(C|x)(\Rightarrow AB)$, $(C|x)(sAB)$ (where $s$ is a specific sign) are respectively identical with $\neg A'$, $\vee A'B'$, $\Rightarrow A'B'$, $sA'B'$, where $A'$, $B'$ are respectively $(C|x)\,A$, $(C|x)\,B$.*

As an example, let us indicate the principle of the verification of CS2. Compare the operation which takes us from $A$ to $(B|x)(C|y)\,A$ with the operation which takes us from $A$ to $(C|y)(B|x)\,A$. In each operation, no sign which appears in $A$ and is distinct from $x$ and $y$ is altered. At every place where $x$ appears in $A$, we have to substitute $B$ for $x$ in the first and in the second operation; this is clear in regard to the first operation, and in regard to the second it follows from the fact that $y$ does not appear in $B$. Finally, at every place where $y$ appears in $A$, the first operation consists in replacing $C$ for $y$, then $B$ for $x$ at every place where $x$ appears in $C$; but it is clear that this comes to the same thing as substituting for $y$, wherever it appears in $A$, the assembly $(B|x)\,C$.

### 3. FORMATIVE CONSTRUCTIONS

Some of the specific signs of a theory are called *relational*, and the others are called *substantific*. With every specific sign is associated a natural number called its *weight* (which is practically always the number 2).

¶ An assembly is said to be of the *first species* if it begins with a $\tau$, or with a substantific sign, or if it consists of a single letter; otherwise it is of the *second species*.

¶ A *formative construction* in a theory $\mathscr{T}$ is a sequence of assemblies which has the following property : for each assembly $A$ of the sequence, one of the following conditions is satisfied :

(a) $A$ is a letter.

(b) There is in the sequence an assembly $B$ of the second species, preceding $A$, such that $A$ is $\neg B$.

(c) There are two assemblies $B$ and $C$ of the second species (distinct or not), preceding $A$, such that $A$ is $\vee BC$.

(d) There is an assembly $B$ of the second species, preceding $A$, and a letter $x$ such that $A$ is $\tau_x(B)$.

(e) There is a specific sign $s$ of weight $n$ (*)[^4] in $\mathscr{T}$, and $n$ assemblies $A_1,A_2,\ldots,A_n$ of the first species, preceding $A$, such that $A$ is $sA_1A_2\ldots A_n$.

¶ The assemblies of the first species (resp. of the second species) which appear in the formative constructions of $\mathscr{T}$ are called terms (resp. relations) in $\mathscr{T}$.

*Example.* *In the theory of sets, in which $\in$ is a relational sign of weight 2, the following sequence of assemblies is a formative construction:*

$$
\begin{array}{c}
A\\
A'\\
A''\\
\in AA'\\
\in AA''\\
\neg\in AA'\\
\vee\neg\in AA'\in AA''
\\[2pt]
\tau\vee\neg\in\square A'\in\square A''
\end{array}
$$

Hence the assembly given as an example in no. 1 is a term in the theory of sets.*

*Remark.* Intuitively, terms are assemblies which represent objects, and relations are assemblies which represent assertions which can be made about these objects. Condition (a) means that the letters represent objects. Condition (b) means that if $B$ is an assertion, then $\neg B$, called the negation of $B$, is an assertion (which is read : not $B$). Condition (c) means that if $B$ and $C$ are assertions, $\vee BC$, which is called the disjunction of $B$ and $C$, is an assertion (which is read : either $B$ or $C$); thus $\neg\to BC$ is an assertion (in words : “either not $B$, or $C$”, or “$B$ implies $C$”). Condition (d) means that if $B$ is an assertion and $x$ a letter, then $\tau_x(B)$ is an object. Let us consider the assertion $B$ as expressing a property of the object $X$; then, if there exists an object which has the property in question, $\tau_x(B)$ represents a distinguished object which has this property; if not, $\tau_x(B)$ represents an object about which nothing can be said. Finally, condition (e) means that if $A_1,A_2,\ldots,A_n$ are objects, and if $s$ is a relational (resp. substantific) sign of weight $n$, then $sA_1A_2\ldots A_n$ is an assertion about the objects $A_1,\ldots,A_n$ (resp. an object depending on $A_1,\ldots,A_n$).

*Examples.* The symbols $\varnothing$, $\mathbf{N}$, “the real line”, “the $\Gamma$ function”, $f\circ g$ represent terms. The symbols $\pi=\sqrt{2}+\sqrt{3}$, $1\in2$, “every finite

division ring is a field”, “the zeros of $\zeta(s)$ other than $-2$, $-4$, $-6$, ... lie on the line $\mathfrak{R}(s)=1/2$” represent relations. The symbol “3 and 4” represents neither a term nor a relation.

The initial sign of a relation is $\vee$, $\neg$, or a relational sign. The initial sign of a term is either $\tau$ or a substantific sign, provided that the term does not consist of a single letter. The latter assertion follows from the fact that a term is an assembly of the first species. If $A$ is a relation, then $A$ features in a formative construction, is not a letter, and does not begin with $\tau$, so that three cases are possible : (1) $A$ is preceded by an assembly $B$ such that $A$ is $\neg B$; (2) $A$ is preceded by two assemblies $B$ and $C$ such that $A$ is $\vee BC$; (3) $A$ is preceded by assemblies $A_1$, $A_2$, ... $A_n$ such that $A$ is $sA_1A_2 ... A_n$, $s$ being a relational sign.

### 4. FORMATIVE CRITERIA

CF1. If $A$ and $B$ are relations in a theory $\mathscr{T}$, then $\vee AB$ is a relation in $\mathscr{T}$.

Consider two formative constructions (in $\mathscr{T}$), one of which contains $A$ and the other $B$. Consider the sequence of assemblies obtained by writing first the assemblies of the first construction, then the assemblies of the second construction, and finally $\vee AB$. Since $A$ and $B$ are of the second species, it is immediately verified that this sequence is a formative construction of $\mathscr{T}$. The assembly $\vee AB$ is of the second species, hence it is a relation in $\mathscr{T}$.

The three following criteria are established similarly :

CF2. If $A$ is a relation in a theory $\mathscr{T}$, then $\neg A$ is a relation in $\mathscr{T}$.

CF3. If $A$ is a relation in a theory $\mathscr{T}$, and if $x$ is a letter, then $\tau_x(A)$ is a term in $\mathscr{T}$.

CF4. If $A_1$, $A_2$, ..., $A_n$ are terms in a theory $\mathscr{T}$, and if $s$ is a relational (resp. substantific) sign of weight $n$ in $\mathscr{T}$, then $sA_1A_2...A_n$ is a relation (resp. a term) in $\mathscr{T}$.

These criteria immediately imply the following :

CF5. If $A$ and $B$ are relations in a theory $\mathscr{T}$, then $\Longrightarrow AB$ is a relation in $\mathscr{T}$.

CF6. Let $A_1$, $A_2$, ..., $A_n$ be a formative construction in a theory $\mathscr{T}$, and let $x$ and $y$ be letters. Suppose that $y$ does not appear in any $A_i$. Then $(y|x) A_1$, $(y|x) A_2$, ..., $(y|x) A_n$ is a formative construction in $\mathscr{T}$.

To prove CF6, let $A_i'$ be the assembly $(y|x)A_i$. If $A_i$ is a letter, then $A_i'$ is a letter. If $A_i$ is of the form $\neg A_j$, where $A_j$ is an assembly of the second species which precedes $A_i$ in the construction, then $A_i'$ is identical with $\neg A_j'$ by CS5, and $A_j'$ is an assembly of the second species. The reasoning is similar if $A_i$ is of the form $\vee A_jA_k$ or $sA_{j_1}A_{j_2}\ldots A_{j_m}$, $s$ being a specific sign of $\mathscr{T}$. If finally $A_i$ is of the form $\tau_z(A_j)$, where $A_j$ is an assembly of the second species which precedes $A_i$ in the construction, there are various cases to consider:

(a) $z$ is a letter distinct from $x$ and $y$. Then $A_i'$ is identical with $\tau_z(A_j')$ by CS4, and $A_j'$ is an assembly of the second species.

(b) $z$ is identical with $x$. Then $A_i$ does not contain $x$, hence $A_i'$ is identical with $A_i$, that is to say with $\tau_x(A_j)$; since $y$ does not appear in $A_j$, $\tau_x(A_j)$ is identical with $\tau_y(A_j)$ by CS3.

(c) $z$ is identical with $y$. Then $A_i$ is the assembly $\tau A_j$, because $y$ does not appear in $A_j$; therefore $A_i'$ is the assembly $\tau A_j'$, that is $\tau_u(A_j')$, where $u$ is a letter which does not appear in $A_j'$.

CF7. *Let $A$ be a relation (resp. a term) in a theory $\mathscr{T}$, and let $x$ and $y$ be letters. Then $(y|x)A$ is a relation (resp. a term) in $\mathscr{T}$.*

Let $A_1,A_2,\ldots,A_n$ be a formative construction in which $A$ appears. We shall show step by step that, if $A_i$ is a relation (resp. a term) then $(y|x)A_i$, which we shall denote by $A_i'$, is also a relation (resp. a term). Suppose that this point has been established for $A_1,A_2,\ldots,A_{i-1}$; let us prove it for $A_i$. If $A_i$ is a letter, then $A_i'$ is a letter. If $A_i$ is preceded in the construction by a relation $A_j$ such that $A_i$ is $\neg A_j$, then $A_i'$ is identical with $\neg A_j'$ by CS5, and $\neg A_j'$ is a relation by CF2. The argument is similar if $A_i$ is preceded by relations $A_j,A_k$ such that $A_i$ is $\vee A_jA_k$, or if $A_i$ is preceded by terms $A_{j_1},\ldots,A_{j_m}$ such that $A_i$ is $sA_{j_1}\cdots A_{j_m}$, where $s$ is a specific sign of $\mathscr{T}$ of weight $m$. Finally, if $A_i$ is preceded by a relation $A_j$ such that $A_i$ is $\tau_z(A_j)$, there are various cases to consider:

(a) $z$ is distinct from both $x$ and $y$. Then $A_i'$ is identical with $\tau_z(A_j')$ by CS4, and we know already that $A_j'$ is a relation; hence $A_i$ is a term, by CF3.

(b) $z$ is identical with $x$. Then $A_i$ does not contain $x$, therefore $A_i'$ is identical with $A_i$, and consequently is a term.

(c) $z$ is identical with $y$. Then let $u$ be a letter, distinct from both $x$ and $y$, which does not appear in $A_1,A_2,\ldots,A_j$. By CF6, the sequence of assemblies $(u|y)A_1,\ldots,(u|y)A_j$, which we shall denote by $A_1'',\ldots,A_j''$, constitutes a formative construction in $\mathscr{T}$. Since $y$ no longer appears in this new construction, $(y|x)A_1'',\ldots,(y|x)A_j''$ is a formative construction by CF6, so that $(y|x)A_j''$ is a relation in $\mathscr{T}$; consequently $\tau_u((y|x)A_j'')$

is a term of $\mathscr{T}$. But this term is identical with $(y|x)\tau_u(A_j'')$ by CS4, hence with $(y|x)\tau_y(A_j)$ by CS3, hence is identical with $A_i$.

CF8. Let $A$ be a relation (resp. a term) in a theory $\mathscr{T}$, let $x$ be a letter and $T$ a term in $\mathscr{T}$. Then $(T|x)A$ is a relation (resp. a term) in $\mathscr{T}$.

Let $A_1, A_2, \ldots, A_n$ be a formative construction in which $A$ appears. Let $x_1, x_2, \ldots, x_p$ be the distinct letters which appear in $T$. Let us associate with each letter $x_i$ a letter $x_i'$, distinct from each of the letters $x_1, \ldots, x_p$ and the letters which appear in $A_1, \ldots, A_n$, in such a way that the letters $x_1', \ldots, x_p'$ are all distinct. The assembly

$$
(x_1'|x_1)(x_2'|x_2)\ldots(x_p'|x_p)T
$$

is a term $T'$ by CF7, and $(T|x)A$ is identical with

$$
(x_1|x_1')(x_2|x_2')\ldots(x_p|x_p')(T'|x)A
$$

by application of CS1. It is therefore enough to show that $(T'|x)\,A$ is a relation (resp. a term); in other words, we may suppose from now on that the letters which appear in $T$ do not appear in $A_1, \ldots, A_n$.

¶ We shall show step by step that, if $A_t$ is a relation (resp. a term), then $(T|x)\,A_t$, which we shall denote by $A_t'$, is a relation (resp. a term). Suppose this point has been established for $A_1,A_2,\ldots,A_{i-1}$, and let us prove it for $A_i$. If $A_i$ is a letter, then $A_i'$ is either the same letter or $T$, and therefore a term. If $A_i$ is of the form $\neg A_j$, where $A_j$ is a relation which precedes $A_i$ in construction, then $A_i$ is identical with $\neg A_j'$ by CS5, and we know already that $A_j'$ is a relation, hence $A_i'$ is a relation by CF2. The proof is analogous if $A_i$ is of the form $\vee A_jA_k$, or $sA_{j_1}\ldots A_{j_m}$. Finally, if $A_i$ is of the form $\tau_z(A_j)$, where $A_j$ is a relation which precedes $A_i$ in the construction, there are various cases to be considered:

(a) $z$ is distinct from $x$ and from the letters which appear in $T$. Then $A_i'$ is identical with $\tau_z(A_j')$ by CS4, and we know already that $A_j'$ is a relation; hence $A_i'$ is a term by CF3.

(b) $z$ is identical with $x$. Then $A_i$ does not contain $x$, hence $A_i'$ is identical with $A_i$ and consequently is a term.

(c) $z$ appears in $T$. Then $z$ does not appear in $A_j$, so that $A_i'$ is identical with $\tau A_j'$; hence $A_i'$ is identical with $\tau A_j'$. Now, we know already that $A_j'$ is a relation, and $\tau A_j'$ is identical with $\tau_u(A_j)$, where $u$ is a letter which does not appear in $A_j$; it follows by CF3 that $A_i'$ is a term.

Intuitively, if $A$ is a relation in $\mathscr{T}$, which we may regard as expressing a property of an object $x$, the assertion $(B|x)\,A$ amounts to saying that the object $B$ has this property. If $A$ is a term in $\mathscr{T}$, it represents an object which depends in some way on the object denoted by $x$; the term $(B|x)\,A$ represents what the object $A$ becomes when we take $x$ to be the object $B$.

### Exercises {#ens-i-s1-exercises}

See the [exercises for § 1](exercises/s1/).

[^1]: (\*) The meaning of this expression will become clear as the chapter progresses.
[^2]: (†) For the intuitive meanings of these signs, see no. 3, Remark.
[^3]: (*) In accordance with what was said in no. 1, the phrase “$x$ and $y$ are distinct letters” is an abuse of language: it means that $x$ and $y$ denote distinct letters in the assemblies under consideration.
[^4]: (*) As was said above, it would be possible, for the development of present-day mathematical theories, to limit our consideration to specific signs of weight 2, and consequently to avoid using the expression “natural number $n$” in the definition of a formative construction.
