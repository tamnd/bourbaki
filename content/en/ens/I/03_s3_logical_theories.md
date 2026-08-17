---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION OF FORMAL MATHEMATICS
section: 3
section_title: Logical theories
lang: en
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 28-36, 57-58
pdf_pages: 0035-0043, 0064-0065
extraction: ocr
subsections:
    - "no": 1
      title: THE AXIOMS
      page: 28
      pdf_page: 35
    - "no": 2
      title: FIRST CONSEQUENCES
      page: 29
      pdf_page: 36
    - "no": 3
      title: METHODS OF PROOF
      page: 30
      pdf_page: 37
    - "no": 4
      title: CONJUNCTION
      page: 33
      pdf_page: 40
    - "no": 5
      title: EQUIVALENCE
      page: 34
      pdf_page: 41
statements: 0
exercises: 5
content_sha256: b429aa448e801f5e6c98174f23720386650518026195c14d31873c2ba51f7dd2
---

## 3. LOGICAL THEORIES

### 1. THE AXIOMS

A *logical theory* is any theory $\mathscr{T}$ in which the schemes S1 to S4 below provide implicit axioms.

S1. *If $A$ is a relation in $\mathscr{T}$, the relation $(A$ or $A) \Rightarrow A$ is an axiom of $\mathscr{T}$* (\*)[^1].

S2. *If $A$ and $B$ are relations in $\mathscr{T}$, the relation $A \Rightarrow (A$ or $B)$ is an axiom of $\mathscr{T}$.*

S3. *If $A$ and $B$ are relations in $\mathscr{T}$, the relation $(A$ or $B) \Rightarrow (B$ or $A)$ is an axiom of $\mathscr{T}$.*

S4. *If $A$, $B$, and $C$ are relations in $\mathscr{T}$, the relation*

$$(A \Rightarrow B) \Rightarrow ((C \text{ or } A) \Rightarrow (C \text{ or } B))$$

*is an axiom of $\mathscr{T}$.*

These rules are in fact schemes; let us verify this, for example for S2. Let $R$ be a relation obtained by applying S2; then there are relations $A$ and $B$ in $\mathscr{T}$ such that $R$ is the relation $A \Rightarrow (A$ or $B)$. Let $T$ be a term in $\mathscr{T}$, let $x$ be a letter, and let $A'$ and $B'$ be the relations $(T|x)A$ and $(T|x)B$; then $(T|x)R$ is the same as $A' \Rightarrow (A'$ or $B')$, and can therefore be obtained by applying S2.

Intuitively, the rules S1 through S4 merely express the meaning which is attached to the words "or" and "implies" in the usual language of mathematics (†)[^2].

If a logical theory $\mathscr{T}$ is contradictory, *every relation in $\mathscr{T}$ is a theorem in $\mathscr{T}$.* For let $A$ be a relation in $\mathscr{T}$ such that $A$ and "not $A$" are theorems in $\mathscr{T}$, and let $B$ be any relation in $\mathscr{T}$. By S2, (not $A$) $\Rightarrow$ ((not $A$) or $B$) is a theorem in $\mathscr{T}$; therefore, by C1 (§ 2, no. 2), "(not $A$) or $B$", that is to say $A \Rightarrow B$, is a theorem in $\mathscr{T}$. A second application of C1 shows that $B$ is a theorem in $\mathscr{T}$.

¶ *From now on $\mathscr{T}$ will denote a logical theory.*

### 2. FIRST CONSEQUENCES

C6. *Let $A$, $B$, $C$ be relations in $\mathscr{T}$. If $A \Rightarrow B$ and $B \Rightarrow C$ are theorems in $\mathscr{T}$, then $A \Rightarrow C$ is a theorem in $\mathscr{T}$.*

For $(B \Rightarrow C) \Rightarrow ((A \Rightarrow B) \Rightarrow (A \Rightarrow C))$ is an axiom of $\mathscr{T}$, by replacing $A$ by $B$, $B$ by $C$, and $C$ by "not $A$" in S4. By C1 (§ 2, no. 2), $(A \Rightarrow B) \Rightarrow (A \Rightarrow C)$ is a theorem in $\mathscr{T}$. A further application of C1 completes the proof.

C7. *If $A$ and $B$ are relations in $\mathscr{T}$, then $B \Rightarrow (A$ or $B)$ is a theorem in $\mathscr{T}$.*

For $B \Rightarrow (B$ or $A)$ and $(B$ or $A) \Rightarrow (A$ or $B)$ are axioms of $\mathscr{T}$ by virtue of S2 and S3. Now use C6.

C8. *If $A$ is a relation in $\mathscr{T}$, $A \Rightarrow A$ is a theorem in $\mathscr{T}$.*

For $A \Rightarrow (A$ or $A)$ and $(A$ or $A) \Rightarrow A$ are axioms, by S2 and S1. Now use C6.

C9. *If $A$ is a relation and $B$ a theorem in $\mathscr{T}$, then $A \Rightarrow B$ is a theorem in $\mathscr{T}$.*

For $B \Rightarrow ((\text{not } A)$ or $B)$ is a theorem by C7, and therefore "(not $A$) or $B$", that is to say $A \Rightarrow B$, is a theorem by C1.

C10. *If $A$ is a relation in $\mathscr{T}$, then "$A$ or (not $A$)" is a theorem in $\mathscr{T}$.*

For "(not $A$) or $A$" is a theorem by C8; now use S3 and C1.

C11. *If $A$ is a relation in $\mathscr{T}$, "$A \Rightarrow$ (not not $A$)" is a theorem in $\mathscr{T}$.*

For this relation is "(not $A$) or (not not $A$)", and the result follows from C10.

C12. *Let $A$ and $B$ be two relations in $\mathscr{T}$. Then the relation*

$$(A \Rightarrow B) \Rightarrow ((\text{not } B) \Rightarrow (\text{not } A))$$

*is a theorem in $\mathscr{T}$.*

For

$$((\text{not } A) \text{ or } B) \Rightarrow ((\text{not } A) \text{ or } (\text{not not } B))$$

is a theorem, by C11, S4 and C1. On the other hand,

$$((\text{not } A) \text{ or } (\text{not not } B)) \Rightarrow ((\text{not not } B) \text{ or } (\text{not } A))$$

is an axiom, by S3. Therefore

$$((\text{not } A) \text{ or } B) \Rightarrow ((\text{not not } B) \text{ or } (\text{not } A))$$

is a theorem by C6. Hence the result.

C13. *Let $A$, $B$, $C$ be relations in $\mathscr{T}$. If $A \Rightarrow B$ is a theorem in $\mathscr{T}$, then $(B \Rightarrow C) \Rightarrow (A \Rightarrow C)$ is a theorem in $\mathscr{T}$.*

For $(\text{not } B) \Rightarrow (\text{not } A)$ is a theorem, by C12 and C1. Therefore $(C \text{ or } (\text{not } B)) \Rightarrow (C \text{ or } (\text{not } A))$ is a theorem, by S4 and C1. By a double application of S3 and C6 we infer that

$$((\text{not } B) \text{ or } C) \Rightarrow ((\text{not } A) \text{ or } C)$$

is a theorem; but this is the given relation.

¶ *From now on, we shall generally use* C1 *and* C6 *without quoting them explicitly.*

### 3. METHODS OF PROOF

I. *Method of the auxiliary hypothesis.* This rests on the following rule :

C14 (*Criterion of deduction*). *Let $A$ be a relation in $\mathscr{T}$, and let $\mathscr{T}'$ be the theory obtained by adjoining $A$ to the axioms of $\mathscr{T}$. If $B$ is a theorem in $\mathscr{T}'$, then $A \Rightarrow B$ is a theorem in $\mathscr{T}$.*

Let $B_1$, $B_2$, ..., $B_n$ be a proof in $\mathscr{T}'$ in which $B$ appears. We shall show, step by step, that the relations $A \Rightarrow B_k$ are theorems in $\mathscr{T}$. Suppose that this has been established for the relations which precede $B_i$, and let us show that $A \Rightarrow B_i$ is a theorem in $\mathscr{T}$. If $B_i$ is an axiom of $\mathscr{T}'$, then $B_i$ is either an axiom of $\mathscr{T}$ or is $A$. In both cases, $A \Rightarrow B_i$ is a theorem in $\mathscr{T}$ by applying C9 or C8. If $B_i$ is preceded by relations $B_j$ and $B_j \Rightarrow B_i$, we know that $A \Rightarrow B_j$ and $A \Rightarrow (B_j \Rightarrow B_i)$ are theorems in $\mathscr{T}$. Hence $(B_j \Rightarrow B_i) \Rightarrow (A \Rightarrow B_i)$ is a theorem in $\mathscr{T}$ by C13. Hence, by C6, $A \Rightarrow (A \Rightarrow B_i)$, that is to say "$(\text{not } A)$ or $(A \Rightarrow B_i)$", is a theorem in $\mathscr{T}$, and therefore so is "$(A \Rightarrow B_i)$ or $(\text{not } A)$" by S3. Now, $(\text{not } A) \Rightarrow ((\text{not } A) \text{ or } B_i)$, that is to say $(\text{not } A) \Rightarrow (A \Rightarrow B_i)$, is a theorem in $\mathscr{T}$, by S2. By application of S4 we see then that

$$((A \Rightarrow B_i) \text{ or } (\text{not } A)) \Rightarrow ((A \Rightarrow B_i) \text{ or } (A \Rightarrow B_i))$$

is a theorem in $\mathscr{T}$, and hence that "$(A \Rightarrow B_i)$ or $(A \Rightarrow B_i)$" is a theorem in $\mathscr{T}$. By S1 we conclude that $A \Rightarrow B_i$ is a theorem in $\mathscr{T}$.

In practice we indicate that we are going to use this criterion by a phrase such as "suppose that $A$ is true". This phrase means that for the time being the reasoning will be performed in the theory $\mathscr{T}'$, until the relation $B$ has been proved. When this has been achieved it has been established that $A \Rightarrow B$ is a theorem in $\mathscr{T}$, and one continues thereafter to reason in $\mathscr{T}$ without in general indicating that one has abandoned the theory $\mathscr{T}'$. The relation $A$ introduced as a new axiom is called the *auxiliary hypothesis*. \* For example, when we say "let $x$ be a real number", we are constructing a theory in which the relation "$x$ is a real number" is an auxiliary hypothesis. \*

II. *Method of reductio ad absurdum.* This is founded on the following rule :

C15. *Let $A$ be a relation in $\mathscr{T}$, and let $\mathscr{T}'$ be the theory obtained by adjoining the axiom* "not $A$" *to the axioms of $\mathscr{T}$. If $\mathscr{T}'$ is contradictory, then $A$ is a theorem in $\mathscr{T}$.*

For $A$ is a theorem in $\mathscr{T}'$; consequently (method of the auxiliary hypothesis) "(not $A$) $\Rightarrow A$" is a theorem in $\mathscr{T}$. By S4,

$$(A \text{ or } (\text{not } A)) \Rightarrow (A \text{ or } A)$$

is a theorem in $\mathscr{T}$; by C10, "$A$ or $A$" is a theorem in $\mathscr{T}$. Now use S1.

In practice, we indicate that we are going to use this criterion by a phrase such as "suppose that $A$ is false". This phrase means that for the time being the reasoning will be performed in the theory $\mathscr{T}'$, until two theorems of the form $B$ and "not $B$" have been proved. When this has been achieved it is then established that $A$ is a theorem in $\mathscr{T}$, which is generally indicated by a phrase such as "Now this (i.e., in the preceding notation, $B$ and "not $B$") is absurd; hence $A$ is true". One then continues in the original theory $\mathscr{T}$.

¶ As first applications of these methods, let us establish the following criteria :

C16. *If $A$ is a relation in $\mathscr{T}$, then* (not not $A$) $\Rightarrow A$ *is a theorem in $\mathscr{T}$.*

For suppose that "not not $A$" is true; then we have to prove $A$. Suppose $A$ is false. In the theory so defined, "not not $A$" and "not $A$" are theorems, which is absurd; therefore $A$ is true.

C17. *If $A$ and $B$ are relations in $\mathscr{T}$, then*

$$((\text{not } B) \Rightarrow (\text{not } A)) \Rightarrow (A \Rightarrow B)$$

*is a theorem in $\mathscr{T}$.*

For suppose that $(\text{not }B) \Rightarrow (\text{not }A)$ is true. We have to show that $A \Rightarrow B$ is true. Suppose that $A$ is true, and let us show that $B$ is true. Suppose “not $B$” is true. Then “not $A$” is true, which is absurd.

III. *Method of disjunction of cases.* This rests on the following rule :

C18. *Let $A$, $B$, $C$ be relations in $\mathscr{T}$. If “$A$ or $B$” $A \Rightarrow C$, $B \Rightarrow C$ are theorems in $\mathscr{T}$, then $C$ is a theorem in $\mathscr{T}$.*

For, by S4, “$(A\text{ or }B) \Rightarrow (A\text{ or }C)$” and “$(C\text{ or }A) \Rightarrow (C\text{ or }C)$” are theorems in $\mathscr{T}$. By S3 and S1, it follows that $(A\text{ or }B) \Rightarrow C$ is a theorem in $\mathscr{T}$; hence the result.

To prove $C$ it is therefore enough, when we have at our disposal a theorem “$A$ or $B$”, first to prove $C$ by adjoining $A$ to the axioms of $\mathscr{T}$, and then to prove $C$ by adjoining $B$ to the axioms of $\mathscr{T}$. The interesting feature of this method lies in the fact that if “$A$ or $B$” is true, we cannot in general assert either that $A$ is true or that $B$ is true.

In particular, by C10, if “$A \Rightarrow C$” and “$(\text{not }A) \Rightarrow C$” are both theorems in $\mathscr{T}$, then $C$ is a theorem in $\mathscr{T}$.

IV. *Method of the auxiliary constant.* This is founded on the following rule :

C19. *Let $x$ be a letter and let $A$ and $B$ be relations in $\mathscr{T}$ such that :*

(1) *the letter $x$ is not a constant of $\mathscr{T}$ and does not appear in $B$;*
(2) *there is a term $T$ in $\mathscr{T}$ such that $(T|x)A$ is a theorem in $\mathscr{T}$.*

*Let $\mathscr{T}'$ be the theory obtained by adjoining $A$ to the axioms of $\mathscr{T}$. If $B$ is a theorem in $\mathscr{T}'$, then $B$ is a theorem in $\mathscr{T}$.*

Indeed, $A \Rightarrow B$ is a theorem in $\mathscr{T}$ (criterion of deduction). Since $x$ is not a constant of $\mathscr{T}$, $(T|x)(A \Rightarrow B)$ is a theorem in $\mathscr{T}$ by virtue of C3. Since $x$ does not appear in $B$, $(T|x)(A \Rightarrow B)$ is identical with $((T|x)A) \Rightarrow B$, by CS5 (§ 1, no. 2). Finally, $(T|x)A$ is a theorem in $\mathscr{T}$, and therefore so is $B$.

Intuitively, the method consists in using, in order to prove $B$, an arbitrary object $x$ (the *auxiliary constant*) which is supposed to be endowed with certain properties, denoted by $A$. * For example, in a proof in geometry which involves, among other things, a line $D$, we may “take” a point $x$ on this line; the relation $A$ is then $x \in D$. * In order that one should be able to use an object endowed with certain properties during the course of a proof, it is clearly necessary that such objects should exist. The theorem $(T|x)A$, called the *theorem of legitimation*, guarantees this existence.

In practice we indicate that we are going to use this method by a phrase such as “let $x$ be an object such that $A$”. By contrast with the method of the auxiliary hypothesis, the conclusion of the argument does not involve $x$.

### 4. CONJUNCTION

Let $A$, $B$ be assemblies. The assembly

$$
\text{not } ((\text{not } A) \text{ or } (\text{not } B))
$$

will be denoted by “$A$ and $B$”.

CS6.  Let $A$, $B$, $T$ be assemblies and $x$ a letter.  Then the assembly

$$
(T|x)(A\text{ and }B)
$$

is identical with “$(T|x)A$ and $(T|x)B$”.

This is an immediate consequence of CS5 (§ 1, no. 2).

CF9.  If $A$, $B$ are relations in $\mathscr{T}$, then “$A$ and $B$” is a relation in $\mathscr{T}$ (called the conjunction of $A$ and $B$).

This follows immediately from CF1 and CF2 (§ 1, no. 4).

C20.  If $A$, $B$ are theorems in $\mathscr{T}$, then “$A$ and $B$” is a theorem in $\mathscr{T}$.

Suppose that “$A$ and $B$” is false, that is to say,

$$
\text{not not } ((\text{not } A) \text{ or } (\text{not } B))
$$

is true.  By C16, “$(\text{not } A)$ or $(\text{not } B)$”, that is to say, $A \Longrightarrow (\text{not } B)$ is true, hence “not $B$” is true; but this is absurd.  Hence “$A$ and $B$” is true.

C21.  If $A$, $B$ are relations in $\mathscr{T}$, then

$$
(A\text{ and }B) \Longrightarrow A,\qquad (A\text{ and }B) \Longrightarrow B
$$

are theorems in $\mathscr{T}$.

The relations $(\text{not } A) \Longrightarrow ((\text{not } A) \text{ or } (\text{not } B))$, $(\text{not } B) \Longrightarrow ((\text{not } A) \text{ or } (\text{not } B))$ are theorems in $\mathscr{T}$, by S2 (no. 1) and C7 (no. 2).  Now $((\text{not } A) \text{ or } (\text{not } B)) \Longrightarrow (\text{not } (A\text{ and }B))$ is a theorem in $\mathscr{T}$ by C11.  Hence $(\text{not } A) \Longrightarrow (\text{not } (A\text{ and }B))$, $(\text{not } B) \Longrightarrow (\text{not } (A\text{ and }B))$ are theorems in $\mathscr{T}$.  The result follows by applying C17.

¶ We shall denote by "$A$ and $B$ and $C$" (resp. "$A$ or $B$ or $C$") the relation "$A$ and ($B$ and $C$)" (resp. "$A$ or ($B$ or $C$)"). More generally, if

$$A_1, \quad A_2, \quad \ldots, \quad A_n$$

are relations, we denote by "$A_1$ and $A_2$, and ... and $A_p$" a relation which is constructed step by step by means of the convention that "$A_1$ and $A_2$ and ... and $A_h$" denotes the same relation as "$A_1$ and ($A_2$ and ... and $A_h$)". The relation "$A_1$ or $A_2$ or ... or $A_h$" is defined similarly. The relation "$A_1$ and $A_2$ and ... and $A_h$" is a theorem in $\mathscr{T}$ if and only if each of the relations $A_1$, $A_2$, ..., $A_h$ is a theorem in $\mathscr{T}$.

It follows that every logical theory $\mathscr{T}$ is equivalent to a logical theory $\mathscr{T}'$ which has at most one explicit axiom. This is clear if $\mathscr{T}$ has no explicit axiom. If $\mathscr{T}$ has explicit axioms $A_1$, $A_2$, ..., $A_h$, let $\mathscr{T}'$ be the theory which has the same signs and schemes as $\mathscr{T}$, and the explicit axiom "$A_1$ and $A_2$ and ... and $A_h$". It is immediately seen that every axiom of $\mathscr{T}$ (resp. $\mathscr{T}'$) is a theorem of $\mathscr{T}'$ (resp. $\mathscr{T}$).

Let $\mathscr{T}_0$ be the theory with no explicit axioms which has the same signs as $\mathscr{T}$ and S1, S2, S3, S4 as its only schemes. Then the study of $\mathscr{T}$ reduces, in principle, to the study of $\mathscr{T}_0$ : for the relation $A$ to be a theorem in $\mathscr{T}$ it is necessary and sufficient that there exist axioms $A_1$, $A_2$, ..., $A_h$ of $\mathscr{T}$ such that $(A_1$ and $A_2$ and ... and $A_h) \Rightarrow A$ is a theorem in $\mathscr{T}_0$. This condition is evidently sufficient. Suppose conversely that $A$ is a theorem in $\mathscr{T}$, and let $A_1$, $A_2$, ..., $A_h$ be the axioms of $\mathscr{T}$ appearing in a proof in $\mathscr{T}$ which contains $A$. Let $\mathscr{T}'$ (resp. $\mathscr{T}''$) be the theory constructed from $\mathscr{T}_0$ by adjoining the axioms $A_1$, $A_2$, ..., $A_h$ (resp. the axiom "$A_1$ and $A_2$ and ... and $A_h$"). The proof of $A$ in $\mathscr{T}$ is a proof of $A$ in $\mathscr{T}'$, therefore $A$ is a theorem in $\mathscr{T}'$ and consequently in $\mathscr{T}''$, because (as we noted above) $\mathscr{T}'$ and $\mathscr{T}''$ are equivalent. By the criterion of deduction, $(A_1$ and $A_2$ and ... and $A_h) \Rightarrow A$ is a theorem in $\mathscr{T}_0$.

If $\mathscr{T}$ is contradictory, then it follows from what has been said that there exists a conjunction $A$ of axioms of $\mathscr{T}$ and a relation $R$ in $\mathscr{T}$ such that $A \Rightarrow (R$ and (not $R$)) is a theorem in $\mathscr{T}_0$. Therefore

$$((\text{not } R) \text{ or } (\text{not not } R)) \Rightarrow (\text{not } A)$$

is a theorem in $\mathscr{T}_0$, and since "(not $R$) or (not not $R$)" is a theorem in $\mathscr{T}_0$, "not $A$" is a theorem in $\mathscr{T}_0$. Conversely, if there exists a conjunction $A$ of axioms of $\mathscr{T}$ such that "not $A$" is a theorem in $\mathscr{T}_0$, then $A$ and "not $A$" are theorems in $\mathscr{T}$, so that $\mathscr{T}$ is contradictory.

### 5. EQUIVALENCE

Let $A$ and $B$ be assemblies. The assembly

$$(A \Rightarrow B) \text{ and } (B \Rightarrow A)$$

will be denoted by $A \Leftrightarrow B$.

CS7. *Let $A$, $B$, $T$ be assemblies, and let $x$ be a letter. Then the assembly $(T|x)(A \Leftrightarrow B)$ is identical with $(T|x)A \Leftrightarrow (T|x)B$.*

This follows immediately from CS5 (§ 1, no. 2) and CS6 (no. 4).

CF10. *If $A$ and $B$ are relations in $\mathscr{T}$, then $A \Leftrightarrow B$ is a relation in* **T**.

This follows immediately from CF5 (§ 1, no. 4) and CF9 (no. 4).

¶ If $A \Leftrightarrow B$ is a theorem in $\mathscr{T}$, we shall say that $A$ and $B$ are *equivalent* in $\mathscr{T}$; if $x$ is a letter which is not a constant of $\mathscr{T}$, and if $A$ and $B$ are considered as relations in $x$, then every term in $\mathscr{T}$ which satisfies one also satisfies the other.

¶ It follows from the criteria C20, C21 (no. 4) that in order to prove a theorem in $\mathscr{T}$ of the form $A \Leftrightarrow B$, it is necessary and sufficient to be able to prove $A \Rightarrow B$ and $B \Rightarrow A$ in $\mathscr{T}$. This is often done by proving $B$ in the theory deduced from $\mathscr{T}$ by adjoining the axiom $A$, and then by proving $A$ in the theory deduced from $\mathscr{T}$ by adjoining the axiom $B$. These remarks lead immediately to the following criteria, whose proofs we leave to the reader :

C22. *Let $A$, $B$, $C$ be relations in $\mathscr{T}$. If $A \Leftrightarrow B$ is a theorem in $\mathscr{T}$, then $B \Leftrightarrow A$ is a theorem in $\mathscr{T}$. If $A \Leftrightarrow B$ and $B \Leftrightarrow C$ are theorems in $\mathscr{T}$, then $A \Leftrightarrow C$ is a theorem in $\mathscr{T}$.*

C23. *Let $A$, $B$ be equivalent relations in $\mathscr{T}$, and let $C$ be a relation in $\mathscr{T}$. Then the following are theorems in $\mathscr{T}$ :*

$$(\text{not } A) \Leftrightarrow (\text{not } B); \qquad (A \Rightarrow C) \Leftrightarrow (B \Rightarrow C);$$
$$(C \Rightarrow A) \Leftrightarrow (C \Rightarrow B);$$
$$(A \text{ and } C) \Leftrightarrow (B \text{ and } C); \qquad (A \text{ or } C) \Leftrightarrow (B \text{ or } C).$$

C24. *Let $A$, $B$, $C$ be relations in $\mathscr{T}$. Then the following are theorems in $\mathscr{T}$ :*

$$(\text{not not } A) \Leftrightarrow A; \qquad (A \Rightarrow B) \Leftrightarrow ((\text{not } B) \Rightarrow (\text{not } A));$$
$$(A \text{ and } A) \Leftrightarrow A; \qquad (A \text{ and } B) \Leftrightarrow (B \text{ and } A);$$
$$(A \text{ and } (B \text{ and } C)) \Leftrightarrow ((A \text{ and } B) \text{ and } C);$$
$$(A \text{ or } B) \Leftrightarrow \text{not } ((\text{not } A) \text{ and } (\text{not } B));$$
$$(A \text{ or } A) \Leftrightarrow A; \qquad (A \text{ or } B) \Leftrightarrow (B \text{ or } A);$$
$$(A \text{ or } (B \text{ or } C)) \Leftrightarrow ((A \text{ or } B) \text{ or } C);$$
$$(A \text{ and } (B \text{ or } C)) \Leftrightarrow ((A \text{ and } B) \text{ or } (A \text{ and } C));$$
$$(A \text{ or } (B \text{ and } C)) \Leftrightarrow ((A \text{ or } B) \text{ and } (A \text{ or } C));$$
$$(A \text{ and } (\text{not } B)) \Leftrightarrow \text{not } (A \Rightarrow B);$$
$$(A \text{ or } B) \Leftrightarrow ((\text{not } A) \Rightarrow B).$$

C25. *If $A$ is a theorem in $\mathscr{T}$ and $B$ is a relation in $\mathscr{T}$, then*

$$(A \text{ and } B) \Leftrightarrow B$$

*is a theorem in $\mathscr{T}$. If "not $A$" is a theorem in $\mathscr{T}$, then $(A$ or $B) \Rightarrow B$ is a theorem in $\mathscr{T}$.*

¶ *In principle, from now on throughout the rest of this series, criteria* C1 *through* C25 *will be used without reference.*

### Exercises {#ens-i-s3-exercises}

See the [exercises for § 3](exercises/s3/).

[^1]: (\*) This scheme may be expressed without using the letter $A$ or the abbreviating symbol $\Rightarrow$ as follows : *whenever we have a relation, we obtain a theorem by writing, from left to right,* $\vee$, $\neg$, $\vee$, *and then the given relation three times*. The reader may, as an exercise, translate in a similar way the expressions of the other schemes.
[^2]: (†) In everyday speech, the word "or" has two different meanings, according to the context : when we link two statements by the word "or" we may mean to assert at least one of the two (and possibly both together), or we may mean to assert one to the exclusion of the other.
