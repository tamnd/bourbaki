---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION OF FORMAL MATHEMATICS
section: 5
section_title: Equalitarian theories
lang: en
source: ens-i-iv
source_edition: 2004, Springer
pdf_pages: 0051-0056, 0066-0067
extraction: ocr
subsections:
    - "no": 1
      title: THE AXIOMS
      page: 0
      pdf_page: 51
    - "no": 2
      title: PROPERTIES OF EQUALITY
      page: 0
      pdf_page: 52
    - "no": 3
      title: FUNCTIONAL RELATIONS
      page: 0
      pdf_page: 54
statements: 0
exercises: 7
content_sha256: b55b4026adbafccd45115f22432627d69b636aae58b1284ed1ad9b6cb8b80051
---

## 5. EQUALITARIAN THEORIES

### 1. THE AXIOMS

An *equalitarian theory* is a theory $\mathscr{T}$ which has a relational sign of weight 2, written $=$ (read "equals"), and in which the schemes S1 through S5 (§§3 and 4), together with the schemes S6 and S7 below, provide implicit axioms. If $T$ and $U$ are terms in $\mathscr{T}$, the assembly $= TU$ is a relation in $\mathscr{T}$ (called the *relation of equality*) by virtue of CF4; in practice it is denoted by $T = U$ or $(T) = (U)$.

S6. *Let $x$ be a letter, let $T$ and $U$ be terms in $\mathscr{T}$, and let $R\{x\}$ be a relation in $\mathscr{T}$; then the relation $(T = U) \Rightarrow (R\{T\} \Leftrightarrow R\{U\})$ is an axiom.*

S7. *If $R$ and $S$ are relations in $\mathscr{T}$ and if $x$ is a letter, then the relation $((\forall x)(R \Leftrightarrow S)) \Rightarrow (\tau_x(R) = \tau_x(S))$ is an axiom.*

To show that the rule S6 is a scheme, let $A$ be an axiom of $\mathscr{T}$, obtained by applying S6; then there is a relation $R$ in $\mathscr{T}$, terms $T$ and $U$ in $\mathscr{T}$,

and a letter $x$, such that $A$ is $(T = U) \Rightarrow ((T|x)R \Leftrightarrow (U|x)R)$. We shall show that if $y$ is a letter and $V$ a term in $\mathscr{T}$, the relation $(V|x)A$ can be obtained by applying S6. By means of CS1 (§1, no. 2) we may assume that $x$ is distinct from $y$ and does not appear in $V$. Let $T'$, $U'$, $R'$ denote the assemblies $(V|y)T$, $(V|y)U$, $(V|y)R$ respectively. By CS2 and CS5 (§1, no. 2), $(V|y)A$ is identical with

$$(T' = U') \Rightarrow ((T'|x')R' \Leftrightarrow (U'|x')R')$$

and the proof is complete. The verification that S7 is a scheme is similar.

Intuitively, the scheme S6 means that if two objects are equal, they have the same properties. Scheme S7 is more remote from everyday intuition; it means that if two properties $R$ and $S$ of an object $x$ are equivalent, then the distinguished objects $\tau_x(R)$ and $\tau_x(S)$ (chosen respectively from the objects which satisfy $R$, and those which satisfy $S$, if such objects exist) are equal. The reader will note that the presence in S7 of the quantifier $\forall x$ is essential (cf. Exercise 7).

The negation of the relation $= TU$ is denoted by $T \neq U$ or $(T) \neq (U)$ (where the sign $\neq$ is read "is different from").

¶ From S6 we deduce the following criterion :

C43. *Let $x$ be a letter, let $T$ and $U$ be terms in $\mathscr{T}$, and let $R\{x\}$ be a relation in $\mathscr{T}$. Then the relations*

$$(T = U \text{ and } R\{T\}), \qquad (T = U \text{ and } R\{U\})$$

*are equivalent.*

For if we adjoin the hypotheses $T = U$ and $R\{T\}$, then $R\{U\}$ is true by S6; therefore $(T = U$ and $R\{U\})$ is true.

When a relation of the form $T = U$ has been proved in a theory $\mathscr{T}$, it is often said (by abuse of language) that $T$ and $U$ "are the same" or are "identical". Likewise, when $T \neq U$ is true in $\mathscr{T}$, we say that $T$ and $U$ "are distinct" in place of saying that $T$ is different from $U$.

### 2. PROPERTIES OF EQUALITY

From now on we shall consider only equalitarian theories. Let $\mathscr{T}$ be such a theory, and let $\mathscr{T}_0$ be the theory whose signs are those of $\mathscr{T}$ and whose only axioms are those provided by schemes S1 through S7. The theory $\mathscr{T}_0$ is weaker than $\mathscr{T}$ (§2, no. 4) and has no constants. The following three theorems are theorems in $\mathscr{T}_0$.

**Theorem 1.** $x = x$.

Let $S$ denote the relation $x = x$ in $\mathscr{T}_0$. By C27 (§4, no. 1), for every relation $R$ in $\mathscr{T}_0$, $(\forall x)(R \Leftrightarrow R)$ is a theorem in $\mathscr{T}_0$, and therefore, by S7, $\tau_x(R) = \tau_x(R)$, that is to say $(\tau_x(R)|x)S$, is a theorem in $\mathscr{T}_0$. Taking $R$ to be the relation "not $S$" and considering C26 (§4, no. 1), we see that $(\forall x)S$ is a theorem in $\mathscr{T}_0$. By C30 (§4, no. 3), $S$ is therefore a theorem in $\mathscr{T}_0$.

The relation $(\forall x)(x = x)$ is also a theorem in $\mathscr{T}_0$; and if $T$ is a term in $\mathscr{T}_0$, then $T = T$ is a theorem in $\mathscr{T}_0$ (cf. §4, no. 3). It is possible to transform later theorems in the same way into theorems in which no letter appears or into metamathematical criteria. From now on we shall not explicitly perform these transformations, but we shall often implicitly make use of them.

**Theorem 2.** $(x = y) \Leftrightarrow (y = x)$.

Suppose that the relation $x = y$ is true. By S6, the relation

$$(x = y) \Rightarrow ((x|y)(y = x) \Leftrightarrow (y|y)(y = x)),$$

that is

$$(x = y) \Rightarrow ((x = x) \Leftrightarrow (y = x)),$$

is true. Therefore $(x = x) \Leftrightarrow (y = x)$ is true. By Theorem 1 it follows that $y = x$ is true, and the theorem is proved.

**Theorem 3.** $((x = y) \text{ and } (y = z)) \Rightarrow (x = z)$.

Let us adjoin the hypotheses $x = y$, $y = z$ to the axioms of $\mathscr{T}_0$. By S6 the relation $(x = y) \Rightarrow ((x = z) \Leftrightarrow (y = z))$ is true. Hence

$$(x = z) \Leftrightarrow (y = z),$$

and consequently $x = z$, are true.

C44. *Let $x$ be a letter and let $T$, $U$, $V\{x\}$ be terms in $\mathscr{T}_0$. Then the relation $(T = U) \Rightarrow (V\{T\} = V\{U\})$ is a theorem in $\mathscr{T}_0$.*

For let $y$ and $z$ be two distinct letters which are distinct from $x$ and from the letters which appear in $T$, $U$, $V$. Adjoin the hypothesis $y = z$. Then, by S6,

$$((Y|z)(V\{y\} = V\{z\})) \Leftrightarrow (V\{y\} = V\{z\}),$$

that is to say $(V\{y\} = V\{y\}) \Leftrightarrow (V\{y\} = V\{z\})$, is true. Now, $V\{y\} = V\{y\}$ is true by Theorem 1; hence $V\{y\} = V\{z\}$ is true.

From all this it follows that $(y = z) \Rightarrow (V\{y\} = V\{z\})$ is a theorem in $\mathscr{T}_0$, say $A$. But $(T|y)(U|z)A$ is precisely

$$(T = U) \Rightarrow (V\{T\} = V\{U\}).$$

¶ A relation of the form $T = U$, where $T$ and $U$ are terms in $\mathscr{T}$, is called an *equation*; a *solution* (in $\mathscr{T}$) of the relation $T = U$, considered as an equation in a letter $x$, is therefore (§2, no. 2) a term $V$ in $\mathscr{T}$ such that $T\{V\} = U\{V\}$ is a theorem in $\mathscr{T}$.

¶ Let $T$ and $U$ be two terms in $\mathscr{T}$, and let $x_1$, $x_2$, ..., $x_n$ be the letters which appear in $T$ but not in $U$. If the relation

$$(\exists x_1)\ldots(\exists x_n)(T = U)$$

is a theorem in $\mathscr{T}$, we say that *U can be put in the form* $T$ (in $\mathscr{T}$). Let $R$ be a relation in $\mathscr{T}$ and let $y$ be a letter. Let $V$ be a solution (in $\mathscr{T}$) of $R$, considered as a relation in $y$. If every solution (in $\mathscr{T}$) of $R$, considered as a relation in $y$, can be put in the form $V$, then $V$ is said to be the *complete solution* (or *general solution*) of $R$ (in $\mathscr{T}$).

### 3. FUNCTIONAL RELATIONS

Let $R$ be an assembly and $x$ a letter. Let $y$ and $z$ be distinct letters which are distinct from $x$ and which do not appear in $R$. Let $y'$, $z'$ be two other letters with the same properties. By CS8, CS9 (§4, no. 1), CS2, CS5 (§1, no. 2), and CS6 (§3, no. 4), the assemblies

$$(\forall y)(\forall z)(((y|x)R \text{ and } (z|x)R) \Rightarrow (y = z))$$

and

$$(\forall y')(\forall z')(((y'|x)R \text{ and } (z'|x)R) \Rightarrow (y' = z'))$$

are identical. If $R$ is a relation in $\mathscr{T}$, the assembly thus defined is a relation in $\mathscr{T}$ which is denoted by "there exists at most one $x$ such that $R$"; the letter $x$ does not appear in this relation. When this relation is a theorem in $\mathscr{T}$, $R$ is said to be *single-valued* in $X$ in $\mathscr{T}$. To prove that $R$ is single-valued in the theory $\mathscr{T}$, it is enough to prove $y = z$ in the theory obtained by adjoining to $\mathscr{T}$ the axioms $(y|x)R$ and $(z|x)R$, where $y$ and $z$ are distinct letters which are distinct from $x$ and appear neither in $R$ nor in the explicit axioms of $\mathscr{T}$.

C45. *Let $R$ be a relation in $\mathscr{T}$, and let $x$ be a letter which is not a constant of $\mathscr{T}$. If $R$ is single-valued in $x$ in $\mathscr{T}$, then $R \Rightarrow (x = \tau_x(R))$ is a theorem in $\mathscr{T}$. Conversely if, for some term $T$ in $\mathscr{T}$ which does not contain $x$, $R \Rightarrow (x = T)$ is a theorem in $\mathscr{T}$, then $R$ is single-valued in $x$ in $\mathscr{T}$.*

Suppose $R$ is single-valued in $x$ in $\mathscr{T}$, and let us show that

$$R \Rightarrow (x = \tau_x(R))$$

is a theorem in $\mathscr{T}$. Adjoin the hypothesis $R$. Then $(\tau_x(R)|x)R$ is true by S5, and hence "$R$ and $(\tau_x(R)|x)R$" is true. Now, since $R$ is single-valued in $x$,

$$(R \text{ and } (\tau_x(R)|x)R) \Rightarrow (x = \tau_x(R))$$

is a theorem in $\mathscr{T}$ by C30 (§4, no. 3). Therefore $x = \tau_x(R)$ is true.

¶ Conversely, suppose that $R \Rightarrow (x = T)$ is a theorem in $\mathscr{T}$. Let $y$, $z$ be distinct letters which are distinct from $x$ and which appear neither in $R$ nor in the explicit axioms of $\mathscr{T}$. Since $x$ is not a constant of $\mathscr{T}$ and does not appear in $T$, the relations

$$(y|x)R \Rightarrow (y = T), \qquad (z|x)R \Rightarrow (z = T)$$

are theorems in $\mathscr{T}$. Adjoin the hypotheses $(y|x)R$ and $(z|x)R$. Then $y = T$ and $z = T$ are true, hence $y = z$ is true.

¶ Let $R$ be a relation in $\mathscr{T}$. The relation

$$\text{“}(\exists x)R \text{ and there exists at most one } x \text{ such that } R\text{”}$$

is denoted by "there exists exactly one $x$ such that $R$". If this relation is a theorem in $\mathscr{T}$, $R$ is said to be a *functional relation in* $x$ in the theory $\mathscr{T}$.

C46. *Let $R$ be a relation in $\mathscr{T}$, and let $x$ be a letter which is not a constant of $\mathscr{T}$. If $R$ is functional in $x$ in $\mathscr{T}$, then $R \Leftrightarrow (x = \tau_x(R))$ is a theorem in $\mathscr{T}$. Conversely, if for some term $T$ in $\mathscr{T}$ which does not contain $x$,*

$$R \Leftrightarrow (X = T)$$

*is a theorem in $\mathscr{T}$, then $R$ is functional in $x$ in $\mathscr{T}$.*

Suppose $R$ is functional in $x$ in $\mathscr{T}$. Then $R \Rightarrow (x = \tau_x(R))$ is a theorem in $\mathscr{T}$ by C45. On the other hand, $(\exists x)R$ is a theorem in $T$. By S6 the relation

$$(x = \tau_x(R)) \Rightarrow (R \Leftrightarrow (\exists x)R)$$

is a theorem in $\mathscr{T}$. If we adjoin the hypothesis $x = \tau_x(R)$, it follows that $R$ is true. Therefore $(x = \tau_x(R)) \Rightarrow R$ is a theorem in $\mathscr{T}$.

¶ Conversely, if $R \Leftrightarrow (x = T)$ is a theorem in $\mathscr{T}$, then $R$ is single-valued in $x$ in $\mathscr{T}$, by C45. Moreover, $(T|x)R \Leftrightarrow (T = T)$ is a theorem in $\mathscr{T}$; hence $(T|x)R$ and therefore $(\exists x)R$ are theorems in $\mathscr{T}$.

¶ If a relation $R$ is functional in $x$ in T, then $R$ is equivalent to the relation $x = \tau_x(R)$, which is often more manageable. Generally an abbreviating symbol $\Sigma$ is introduced to represent the term $\tau_x(R)$. Such a symbol is called a *functional symbol* in $\mathscr{T}$.

Intuitively, $\Sigma$ represents the unique object which has the property defined by $R$. \* For example, in a theory where "$y$ is a real number $\geqslant 0$" is a theorem, the relation "$x$ is a real number $\geqslant 0$ and $y = x^2$" is functional in $x$. The corresponding functional symbol is taken to be either $\sqrt{y}$ or $y^{1/2}$. \*

C47. *Let $x$ be a letter which is not a constant of $\mathscr{T}$, and let $R\{x\}$ and $S\{x\}$ be two relations in $\mathscr{T}$. If $R\{x\}$ is functional in $x$ in $\mathscr{T}$, then the relation $S\{\tau_x(R)\}$ is equivalent to $(\exists x)(R\{x\}$ and $S\{x\})$.*

For it follows from C46 and C43 that $(R\{x\}$ and $S\{x\})$ is equivalent to $(R\{x\}$ and $S\{\tau_x(R)\})$; since $S\{\tau_x(R)\}$ does not contain $x$,

$$(\exists x)(R\{x\} \ \text{ and } \ S\{\tau_x(R)\})$$

is equivalent to $(S\{\tau_x(R)\}$ and $(\exists x)R)$ by C33 (§ 4, no. 3); and the result follows from the fact that $(\exists x)R$ is true, because $R$ is functional in $x$.

### Exercises {#ens-i-s5-exercises}

*In all the Exercises for* § 5, $\mathscr{T}$ *denotes an equalitarian theory.*

See the [exercises for § 5](exercises/s5/).
