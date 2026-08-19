---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION OF FORMAL MATHEMATICS
section: 4
section_title: Quantified theories
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 36-44, 58-59
pdf_pages: 0043-0051, 0065-0066
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF QUANTIFIERS
      page: 36
      pdf_page: 43
    - "no": 2
      title: AXIOMS OF QUANTIFIED THEORIES
      page: 37
      pdf_page: 44
    - "no": 3
      title: PROPERTIES OF QUANTIFIERS
      page: 38
      pdf_page: 45
    - "no": 4
      title: TYPICAL QUANTIFIERS
      page: 41
      pdf_page: 48
statements: 0
exercises: 8
content_sha256: 925e2bcab4be745aed7f8144472e31fbff6ba56d97432fbf6fd6794efb7b351c
---

## 4. QUANTIFIED THEORIES

### 1. DEFINITION OF QUANTIFIERS

The only logical signs which played a role in § 3 are $\neg$ and $\vee$. The rules we shall now state are essentially concerned with the use of the logical signs $\tau$ and $\square$.

¶ If $R$ is an assembly and $x$ a letter, the assembly $(\tau_x(R)|x)R$ is denoted by "there exists $x$ such that $R$", or by $(\exists x)R$. The assembly

$$\text{"not } ((\exists x) \text{ not } R)\text{"}$$

is denoted by "for all $x$, $R$", or by "given any $x$, $R$", or by $(\forall x)R$. The abbreviating symbols $\exists$ and $\forall$ are called respectively the *existential quantifier* and the *universal quantifier*. The letter $x$ does not appear in the assembly denoted by $\tau_x(R)$ *and therefore does not appear* in the assemblies denoted by $(\exists x)R$ and $(\forall x)R$.

CS8. *Let $R$ be an assembly and let $x$ and $x'$ be letters. If $x'$ does not appear in $R$, then $(\exists x)R$ and $(\forall x)R$ are respectively identical with $(\exists x')R'$ and $(\forall x')R'$, where $R'$ is $(x'|x)R$.*

For $(\tau_x(R)|x)R$ is identical with $(\tau_x(R)|x')R'$ by CS1 (§ 1, no. 2), and $\tau_x(R)$ is identical with $\tau_{x}'(R')$ by CS3 (§ 1, no. 2). Hence $(\exists x)R$ is identical with $(\exists x')R'$. It follows that $(\forall x)R$ is identical with $(\forall x')R'$.

CS9. *Let $R$ and $U$ be assemblies and let $x$ and $y$ be distinct letters. If $X$ does not appear in $U$, then $(U|y)(\exists x)R$ and $(U|y)(\forall x)R$ are respectively identical with $(\exists x)R'$ and $(\forall x)R'$, where $R'$ is $(U|y)R$.*

For, by CS2 (§ 1, no. 2), $(U|y)(\tau x(R)|x)R$ is identical with

$$(T|x)(U|y)R,$$

where $T$ is $(U|y)\tau_x(R)$, that is $\tau_x(R')$, by CS4 (§ 1, no. 2). Hence $(U|y)(\exists x)R$ is identical with $(\exists x)R'$, and consequently $(U|Y)(\forall x)R$ is identical with $(\forall x)R'$.

CF11. *If $R$ is a relation in a theory $\mathscr{T}$ and if $x$ is a letter, then $(\exists x)R$ and $(\forall x)R$ are relations in $\mathscr{T}$.*

This follows immediately from CF3, CF8, and CF2 (§ 1, no. 4).

Intuitively, let us consider $R$ as expressing a property of the object denoted by $x$. From the intuitive meaning of the term $\tau_x(R)$, the assertion $(\exists x)R$ means that there is an object which has the property $R$. The assertion "not $(\exists x)$(not $R$)" means that there is no object which has the property "not $R$", and therefore that every object has the property $R$.

In a logical theory $\mathscr{T}$, if we have a theorem of the form $(\exists x)R$, in which the letter $x$ is not a constant of $\mathscr{T}$, this theorem can serve as a theorem of legitimation in the method of the auxiliary constant (§ 3, no. 3), because it is identical with $(\tau_x(R)|x)R$. Let $\mathscr{T}'$ be the theory obtained by adjoining $R$ to the axioms of $\mathscr{T}$. If we can prove a relation $S$, in which $x$ does not appear, in the theory $\mathscr{T}'$, then $S$ is a theorem in $\mathscr{T}$.

C26. *Let $\mathscr{T}$ be a logical theory, let $R$ be a relation in $\mathscr{T}$, and let $x$ be a letter. The relations $(\forall x)R$ and $(\tau_x(\text{not } R)|x)R$ are then equivalent in $\mathscr{T}$.*

For $(\forall X)R$ is identical with "not $(\tau_x(\text{not } R)|x)(\text{not } R)$" and therefore with "not not $(\tau_x(\text{not } R)|x)R$".

C27. *If $R$ is a theorem in a logical theory $\mathscr{T}$ in which the letter $x$ is not a constant, then $(\forall x)R$ is a theorem in $\mathscr{T}$.*

For $(\tau_x(\text{not } R)|X)R$ is a theorem in $\mathscr{T}$, by C3 (§ 2, no. 3).

On the other hand, if $x$ is a constant of $\mathscr{T}$, the truth of $R$ does not imply that of $(\forall x)R$. Intuitively, the fact that $R$ is a true property of $x$, which is a definite object of $\mathscr{T}$, clearly does not imply that $R$ is a true property of every object.

C28. *Let $\mathscr{T}$ be a logical theory, let $R$ be a relation in $\mathscr{T}$, and let $x$ be a letter. Then the relations* "not $(\forall x)R$" *and $(\exists x)(\text{not } R)$ are equivalent in $\mathscr{T}$.*

For "not $(\forall x)R$" is identical with "not not $(\exists x)(\text{not } R)$".

### 2. AXIOMS OF QUANTIFIED THEORIES

A *quantified theory* is any theory $\mathscr{T}$ in which the schemes S1 to S4 (§ 3, no. 1) and the scheme S5 below provide implicit axioms.

S5. *If $R$ is a relation in $\mathscr{T}$, if $T$ is a term in $\mathscr{T}$, and if $x$ is a letter, then the relation $(T|x)R \Rightarrow (\exists x)R$ is an axiom.*

This rule is indeed a scheme. For let $A$ be an axiom of $\mathscr{T}$ obtained by applying S5; there is then a relation $R$ in $\mathscr{T}$, a term $T$ in $\mathscr{T}$, and a letter $x$ such that $A$ is $(T|x)R \Rightarrow (\exists x)R$. Let $U$ be a term in $\mathscr{T}$ and let $y$ be a letter. We shall show that $(U|y)A$ can also be obtained by applying S5. Using CS1 (§1, no. 2) and CS8 (no. 1), we can confine ourselves to the case in which $x$ is distinct from $y$ and does not appear in $U$. Let $R'$ be the relation $(U|y)R$ and $T'$ the term $(U|y)T$. The criteria CS2 (§1, no. 2) and CS9 (no. 1) show that $(U|y)A$ is identical with $(T'|x)R' \Rightarrow (\exists x)R'$.

The scheme S5 says that if there is an object $T$ for which the relation $R$, considered as expressing a property of $x$, is true, then $R$ is true for the object $\tau_x(R)$; this accords with the intuitive meaning we have attributed to $\tau_x(R)$ (§1, no. 3, Remark).

### 3. PROPERTIES OF QUANTIFIERS

From now on we shall have to consider only quantified theories. For the rest of this section, $\mathscr{T}$ will denote such a theory, and $\mathscr{T}_0$ will denote the theory without explicit axioms which has the same signs as $\mathscr{T}$ and whose only schemes are S1 through S5. $\mathscr{T}$ is stronger than $\mathscr{T}_0$.

C29. *Let $R$ be a relation in $\mathscr{T}$ and let $x$ be a letter. Then the relations "not $(\exists x)R$" and $(\forall x)(\text{not } R)$ are equivalent in $\mathscr{T}$.*

It is sufficient to prove the criterion in the theory $\mathscr{T}_0$ in which $x$ is not a constant. The theorem $R \Leftrightarrow (\text{not not } R)$ gives us, by C3 (§2, no. 3), the theorems
$$(\exists x)R \Rightarrow (\tau_x(R)|x)(\text{not not } R)$$
and
$$(\exists x)(\text{not not } R) \Rightarrow (\tau_x(\text{not not } R)|X)R.$$

Applying S5, we deduce the theorems in $\mathscr{T}_0$
$$(\exists x)R \Rightarrow (\exists x)(\text{not not } R), \quad (\exists x)(\text{not not } R) \Rightarrow (\exists x)R,$$
whence the theorem $(\exists x)R \Leftrightarrow (\exists x)(\text{not not } R)$. Now
$$(\exists x)(\text{not not } R)$$
is equivalent in $\mathscr{T}_0$ to "not not $(\exists x)(\text{not not } R)$", that is to "not $(\forall x)(\text{not } R)$". Hence the result.

The criteria C28 and C29 enable us to deduce properties of one of the quantifiers from properties of the other.

C30. *Let $R$ be a relation in $\mathscr{T}$, let $T$ be a term in $\mathscr{T}$, and let $x$ be a letter. Then the relation $(\forall x)R\Longrightarrow(T|x)R$ is a theorem in $\mathscr{T}$.*

By S5, $(T|x)(\text{not }R)\Longrightarrow(\tau_x(\text{not }R)|x)(\text{not }R)$ is an axiom. This relation is identical with

$$
(\text{not }(T|x)R)\Longrightarrow\text{not}(\tau_x(\text{not }R)|x)R.
$$

Hence $(\tau_x(\text{not }R)|x)R\Longrightarrow(T|x)R$ is a theorem in $\mathscr{T}$. Now use C26 (no. 1).

Let $R$ be a relation in $\mathscr{T}$. By C26, C27, and C30 it is the same (provided the letter $x$ is not a constant of $\mathscr{T}$) whether we state the theorem $R$ in $\mathscr{T}$, or the theorem $(\forall x)R$, or the metamathematical rule : if $T$ is any term in $\mathscr{T}$, then $(T|x)R$ is a theorem in $\mathscr{T}$.

C31. *Let $R$ and $S$ be relations in $\mathscr{T}$, and let $x$ be a letter which is not a constant of $\mathscr{T}$. If $R\Longrightarrow S$ (resp. $R\Longleftrightarrow S$) is a theorem in $\mathscr{T}$, then*

$$
(\forall x)R\Longrightarrow(\forall x)S,\qquad(\exists x)R\Longrightarrow(\exists x)S
$$

$$
[\text{resp. }(\forall x)R\Longleftrightarrow(\forall x)S,\qquad(\exists x)R\Longleftrightarrow(\exists x)S]
$$

*are theorems in $\mathscr{T}$.*

Suppose that $R\Longrightarrow S$ is a theorem in $\mathscr{T}$. Let us adjoin the hypothesis $(\forall x)R$ (in which $x$ does not appear). Then $R$, hence $S$, and therefore also $(\forall x)S$, are true. Consequently $(\forall x)R\Longrightarrow(\forall x)S$ is a theorem in $\mathscr{T}$. It follows that if $R\Longleftrightarrow S$ is a theorem in $\mathscr{T}$, then so is

$$
(\forall x)R\Longleftrightarrow(\forall x)S.
$$

The rules relating to $\exists$ can now be deduced by using C29.

C32. *Let $R$ and $S$ be relations in $\mathscr{T}$, and let $x$ be a letter. Then the relations*

$$
(\forall x)(R\text{ and }S)\Longleftrightarrow((\forall x)R\text{ and }(\forall x)S),
$$

$$
(\exists x)(R\text{ or }S)\Longleftrightarrow((\exists x)R\text{ or }(\exists x)S)
$$

*are theorems in $\mathscr{T}$.*

It is sufficient to prove these criteria in $\mathscr{T}_0$, in which $x$ is not a constant. If $(\forall x)(R\text{ and }S)$ is true, then “$R$ and $S$” is true, and therefore each of the relations $R$, $S$ is true. Consequently each of the relations $(\forall x)R$, $(\forall x)S$ is true, and hence “$(\forall x)R$ and $(\forall x)S$” is true. Similarly one shows that if “$(\forall x)R$ and $(\forall x)S$” is true, then $(\forall x)(R\text{ and }S)$ is true. Hence the first theorem. The second follows by applying C29.

It should be noted that if $(\forall x) (R$ or $S)$ is a theorem in $\mathscr{T}$, we may not conclude that $((\forall x)R$ or $(\forall x)S)$ is a theorem in $\mathscr{T}$. Intuitively, to say that the relation $(\forall x) (R$ or $S)$ is true means that for each object $x$, at least one of the relations $R$, $S$ is true; but in general only one of the two will be true, and whether it is $R$ or $S$ will depend on the choice of $x$. Likewise, if $((\forall x)R$ and $(\exists x)S)$ is a theorem in $\mathscr{T}$, we may not conclude that $(\exists x)(R$ and $S)$ is a theorem in $\mathscr{T}$. However, there is the following criterion :

C33. *Let $R$ and $S$ be relations in $\mathscr{T}$, and let $x$ be a letter which does not appear in $R$. Then the relations*

$$(\forall x)(R \text{ or } S) \iff (R \text{ or } (\forall x)S),$$
$$(\exists x)(R \text{ and } S) \iff (R \text{ and } (\exists x)S)$$

*are theorems in $\mathscr{T}$.*

It is sufficient to establish the criterion in $\mathscr{T}_0$, in which $x$ is not a constant. Let $\mathscr{T}'$ be the theory obtained by adjoining $(\forall x)(R$ or $S)$ to the axioms of $\mathscr{T}_0$. In $\mathscr{T}'$, "$R$ or $S$", and therefore (not $R$) $\Rightarrow S$, are theorems. If "not $R$" is true (a hypothesis in which $x$ does not feature), then $S$ and therefore also $(\forall x)S$ are true. Consequently

$$(\text{not } R) \Rightarrow (\forall x)S$$

is a theorem in $\mathscr{T}'$, and hence $(\forall x)(R$ or $S) \Rightarrow (R$ or $(\forall x)S)$ is a theorem in $\mathscr{T}_0$. Likewise, if "$R$ or $(\forall x)S$" is true, then "$R$ or $S$" and therefore $(\forall x)(R$ or $S)$ are true. Consequently

$$(R \text{ or } (\forall x)S) \Rightarrow (\forall x)(R \text{ or } S)$$

is a theorem in $\mathscr{T}_0$. The rule relating to $\exists$ follows by applying C29.

C34. *Let $R$ be a relation and let $x$ and $y$ be letters. Then the relations*

$$(\forall x)(\forall y)R \iff (\forall y)(\forall x)R,$$
$$(\exists x)(\exists y)R \iff (\exists y)(\exists x)R,$$
$$(\exists x)(\forall y)R \implies (\forall y)(\exists x)R$$

*are theorems in $\mathscr{T}$.*

It is sufficient to prove these theorems in $\mathscr{T}_0$, in which $x$ and $y$ are not constants. If $(\forall x)(\forall y)R$ is true, then $(\forall y)R$, and therefore $R$, hence $(\forall x)R$, hence $(\forall y)(\forall x)R$, are true. Likewise, if $(\forall y)(\forall x)R$ is true, then $(\forall x)(\forall y)R$ is true; and the first theorem follows. The second now follows by use of C29. Finally, since $(\forall y)R \Rightarrow R$ is a theorem in $\mathscr{T}_0$, so is $(\exists x)(\forall y)R \Rightarrow (\exists x)R$ by C31; if $(\exists x)(\forall y)R$ is true, then $(\exists x)R$ is true, and therefore so is $(\forall y)(\exists x)R$. Hence the third theorem.

On the other hand, if $(\forall y)(\exists x)R$ is a theorem in $\mathscr{T}$, we may not conclude that $(\exists x)(\forall y)R$ is a theorem in $\mathscr{T}$. Intuitively, to say that the relation $(\forall y)(\exists x)R$ is true means that, given any object $y$, there is an object $x$ such that $R$ is a true relation between the objects $x$ and $y$. But in general the object $x$ will depend on the choice of the object $y$, whereas to say that $(\exists x)(\forall y)R$ is true means that there is a *fixed* object $x$ such that $R$ is a true relation between this object and *any* object $y$.

### 4. TYPICAL QUANTIFIERS

Let $A$ and $R$ be assemblies and let $x$ be a letter. We denote the assembly $(\exists x)(A$ and $R)$ by $(\exists_A x)R$, and the assembly

$$\text{“not } (\exists_A x) \text{ (not } R)\text{”}$$

by $(\forall_A x)R$. The abbreviating symbols $\exists_A$ and $\forall_A$ are called *typical quantifiers*. Observe that the letter $x$ does not appear in the assemblies denoted by $(\exists_A x)R$, $(\forall_A x)R$.

CS10. *Let $A$ and $R$ be assemblies and let $x$ and $x'$ be letters. If $x$ appears neither in $R$ nor in $A$, then $(\exists_A x)R$ and $(\forall_A x)R$ are respectively identical with $(\exists_{A'} x')R'$ and $(\forall_{A'} x')R'$, where $R'$ is $(x'|x)R$ and $A'$ is $(x'|x)A$.*

CS11. *Let $A$, $R$, $U$ be assemblies, and let $x$, $y$ be distinct letters. If $x$ does not appear in $U$, the assemblies $(U|y)(\exists_A x)R$ and $(U|y)(\forall_A x)R$ are respectively identical with $(\exists_{A'} x')R'$ and $(\forall_{A'} x')R'$, where $R'$ is $(U|y)R$ and $A'$ is $(U|y)A$.*

These rules are immediate consequences of criteria CS8, CS9 (no. 1), CS5 (§ 1, no. 2), and CS6 (§ 3, no. 4).

CF12. *Let $A$ and $R$ be relations in $\mathscr{T}$, and let $x$ be a letter. Then*

$$(\exists_A x)R \quad \text{and} \quad (\forall_A x)R$$

*are relations in $\mathscr{T}$.*

This follows directly from CF11 (no. 1), CF9 (§ 3, no. 4), and CF2 (§ 1, no. 4).

Intuitively, consider $A$ and $R$ as expressing properties of $x$. It may happen that in a series of proofs, we are concerned only with objects satisfying $A$. To say that there exists an object satisfying $A$ such that $R$ means that there exists an object such that “$A$ and $R$”; whence the definition of $\exists_A$. To say that all objects which satisfy $A$ have the property $R$ means that there is no object satisfying $A$ such that "not $R$"; whence the definition of $\forall_A$. In practice, these signs are replaced by various phrases, depending on the nature of the relation $A$. \* For example : "for all integers $x$, $R$"; "there exists an element $x$ of the set E such that $R$"; and so on. \*

C35. *Let $A$ and $R$ be relations in $\mathscr{T}$, and let $x$ be a letter. Then the relations $(\forall_A x)R$ and $(\forall x)(A \Rightarrow R)$ are equivalent in $\mathscr{T}$.*

For the relation $(\forall_A x)R$ is identical with

$$\text{"not}(\exists x)(A \text{ and } (\text{not } R))\text{"}.$$

Now, "$A$ and (not $R$)" is equivalent in $\mathscr{T}_0$ to "not $(A \Rightarrow R)$"; therefore "not $(\exists x)(A$ and (not $R$))" is equivalent in $\mathscr{T}_0$ to

$$\text{"not } (\exists x)(\text{not } (A \Rightarrow R))\text{"},$$

by C31 (no. 3), and the latter relation is identical with $(\forall x)(A \Rightarrow R)$. The criterion is therefore established in $\mathscr{T}_0$, and consequently in $\mathscr{T}$.

We shall often have to prove relations of the form $(\forall_A x)R$; generally we shall use one of the following two criteria :

C36. *Let $A$ and $R$ be relations in $\mathscr{T}$, and let $x$ be a letter. Let $\mathscr{T}'$ be the theory obtained by adjoining $A$ to the axioms of $\mathscr{T}$. If $x$ is not a constant of $\mathscr{T}$, and if $R$ is a theorem in $\mathscr{T}'$, then $(\forall_A x)R$ is a theorem in $\mathscr{T}$.*

For $A \Rightarrow R$ is a theorem in $\mathscr{T}$, by the criterion of deduction, therefore $(\forall_A x)R$ is a theorem in $\mathscr{T}$ by C27 (no. 1) and C35.

In practice, we indicate that we are going to use this rule by a phrase such as "Let $x$ be any element such that $A$". In the theory $\mathscr{T}'$ so defined, we seek to prove $R$. Of course, we cannot assert that $R$ itself is a theorem in $\mathscr{T}$.

C37. *Let $A$ and $R$ be relations in $\mathscr{T}$ and let $x$ be a letter. Let $\mathscr{T}'$ be the theory obtained by adjoining the relations $A$ and "not $R$" to the axioms of $\mathscr{T}$. If $x$ is not a constant of $\mathscr{T}$, and if $\mathscr{T}'$ is contradictory, then $(\forall_A x)R$ is a theorem in $\mathscr{T}$.*

For the theory $\mathscr{T}'$ is equivalent to the theory obtained by adjoining "not $(A \Rightarrow R)$" to the axioms of $\mathscr{T}$. By the method of *reductio ad absurdum*, $A \Rightarrow R$ is a theorem in $\mathscr{T}$, and therefore so is $(\forall_A x)R$ by C27 (no. 1) and C35.

In practice we say : "Suppose that there exists an object $x$ satisfying $A$ for which $R$ is false", and seek to establish a contradiction.

The properties of typical quantifiers are analogous to those of quantifiers :

C38. *Let $A$ and $R$ be relations in $\mathscr{T}$, and let $x$ be a letter. Then the relations*

$$\text{not } (\forall_A x)R \Leftrightarrow (\exists_A x)(\text{not } R),$$
$$\text{not } (\exists_A x)R \Leftrightarrow (\forall_A x)(\text{not } R)$$

*are theorems in $\mathscr{T}$.*

C39. *Let $A$, $R$, and $S$ be relations in $\mathscr{T}$, and let $x$ be a letter which is not a constant of $\mathscr{T}$. If the relation $A \Rightarrow (R \Rightarrow S)$ [resp. $A \Rightarrow (R \Leftrightarrow S)$] is a theorem in $\mathscr{T}$, then the relations*

$$(\exists_A x)R \Rightarrow (\exists_A x)S, \qquad (\forall_A x)R \Rightarrow (\forall_A x)S$$
$$[\text{resp. } (\exists_A x)R \Leftrightarrow (\exists_A x)S, \qquad (\forall_A x)R \Leftrightarrow (\forall_A x)S]$$

*are theorems in $\mathscr{T}$.*

C40. *Let $A$, $R$, and $S$ be relations in $\mathscr{T}$ and let $x$ be a letter. Then the relations*

$$(\forall_A x)(R \text{ and } S) \Leftrightarrow ((\forall_A x)R \text{ and } (\forall_A x)S),$$
$$(\exists_A x)(R \text{ or } S) \Leftrightarrow ((\exists_A x)R \text{ or } (\exists_A x)S)$$

*are theorems in $\mathscr{T}$.*

C41. *Let $A$, $R$, and $S$ be relations in $\mathscr{T}$, and let $x$ be a letter which does not appear in $R$. Then the relations*

$$(\forall_A x)(R \text{ or } S) \Leftrightarrow (R \text{ or } (\forall_A x)S),$$
$$(\exists_A x)(R \text{ and } S) \Leftrightarrow (R \text{ and } (\exists_A x)S)$$

*are theorems in $\mathscr{T}$.*

C42. *Let $A$, $B$, $R$ be relations in $\mathscr{T}$ and let $x$ and $y$ be letters. If $x$ does not appear in $B$, and if $y$ does not appear in $A$, then the relations*

$$(\forall_A x)(\forall_B y)R \Leftrightarrow (\forall_B y)(\forall_A x)R,$$
$$(\exists_A)x(\exists_B y)R \Leftrightarrow (\exists_B y)(\exists_A x)R,$$
$$(\exists_A x)(\forall_B y)R \Rightarrow (\forall_B y)(\exists_A x)R$$

*are theorems in $\mathscr{T}$.*

By way of example, let us prove part of C42. The relation

$$(\exists_A x)(\exists_B y) R$$

is identical with $(\exists x)(A$ and $(\exists y)(B$ and $R))$, and therefore (because $y$ does not appear in $A$) is equivalent in $\mathscr{T}_0$ to

$$(\exists x)(\exists y)(A \text{ and } (B \text{ and } R))$$

by C33 and C31. Likewise, $(\exists_B x)(\exists_A y)R$ is equivalent to

$$(\exists y)(\exists x)(B \text{ and } (A \text{ and } R)).$$

Now apply C31 and C34 (no. 3).

\* As an example of the application of these criteria, consider the following relation : "the sequence of real-valued functions $(f_n)$ converges uniformly to 0 in $[0, 1]$". This means "for each $\varepsilon > 0$ there exists an integer $n$ such that for each $x \in [0, 1]$ and each integer $m \geqslant n$ we have $|f_m(x)| \leqslant \varepsilon$". Suppose we wish to take the negation of this relation (for example, to obtain a proof by contradiction); the criterion C38 shows that this negation is equivalent to the following relation : " there exists an $\varepsilon > 0$ such that for each integer $n$ there exists an $x \in [0, 1]$ and an $m \geqslant n$ for which $|f_m(x)| > \varepsilon$".

### Exercises {#ens-i-s4-exercises}

*In all the Exercises for* § 4, $\mathscr{T}$ *denotes a quantified theory.*

See the [exercises for § 4](exercises/s4/).
