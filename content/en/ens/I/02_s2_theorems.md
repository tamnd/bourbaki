---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION OF FORMAL MATHEMATICS
section: 2
section_title: Theorems
lang: en
source: ens-i-iv
source_edition: 2004, Springer
pdf_pages: 0031-0035, 0063-0064
extraction: ocr
subsections:
    - "no": 1
      title: AXIOMS
      page: 0
      pdf_page: 31
    - "no": 2
      title: PROOFS
      page: 0
      pdf_page: 32
    - "no": 3
      title: SUBSTITUTIONS IN A THEORY
      page: 0
      pdf_page: 33
    - "no": 4
      title: COMPARISON OF THEORIES
      page: 0
      pdf_page: 33
statements: 1
exercises: 1
content_sha256: c8b7ac12f220f9f720128bb004ee9ac705cf905ac08dfbc648d08a0ff3975ca7
---

## 2. THEOREMS

*From now on, if $A$ is a relation, we shall write not($A$) instead of $\neg A$. If $A$ and $B$ are relations, we shall write “($A$) or ($B$)” instead of $\vee AB$, and ($A$) $\Rightarrow$ ($B$) instead of $\Rightarrow AB$. Sometimes we shall leave out the brackets. In each case the reader will be able to determine without difficulty the assembly under consideration.*

### 1. AXIOMS

We have already seen that the specific signs determine the terms and the relations in a theory $\mathscr{T}$. To construct $\mathscr{T}$, we proceed as follows :

(1) First we write down a certain number of relations in $\mathscr{T}$; these are called the *explicit axioms* of $\mathscr{T}$. The letters which appear in the explicit axioms are called the *constants* of $\mathscr{T}$.

(2) We lay down one or more rules [^1], called the *schemes* of $\mathscr{T}$, which must have the following properties : (a) the application of such a rule $\mathscr{R}$ furnishes a relation in $\mathscr{T}$; (b) if $T$ is a term in $\mathscr{T}$, if $x$ is a letter, and if $R$ is a relation in $\mathscr{T}$ constructed by applying the scheme $\mathscr{R}$, then the relation $(T|x)R$ can also be constructed by applying $\mathscr{R}$.

In all the cases we envisage, the verification of these conditions is always easy.

Every relation contructed by applying a scheme of $\mathscr{T}$ is called an *implicit axiom* of $\mathscr{T}$.

Intuitively, the axioms represent either self-evident assertions or else hypotheses from which one wishes to draw consequences. The constants represent well-defined objects for which the properties expressed by the explicit axioms are supposed to be true. On the other hand, if the letter $x$ is not a constant, it represents a completely undetermined object; if a property of the object $x$ is assumed to be true by means of an axiom, then this axiom is necessarily implicit, so that the property remains true for any object $T$.

### 2. PROOFS

A *demonstrative text* in a theory $\mathscr{T}$ comprises :

(1) An auxiliary formative construction of relations and terms in $\mathscr{T}$.

(2) A *proof in* $\mathscr{T}$, that is to say a sequence of relations in $\mathscr{T}$ which appear in the auxiliary formative construction, such that for every relation $\mathbf{R}$ in the sequence at least one of the following conditions is satisfied :

(a$_1$) $\mathbf{R}$ is an explicit axiom of $\mathscr{T}$.

(a$_2$) $\mathbf{R}$ results from the application of a scheme of $\mathscr{T}$ to terms or relations which appear in the auxiliary formative construction.

(b) there are two relations $\mathbf{S}$, $\mathbf{T}$ in the sequence which precede $\mathbf{R}$, such that $\mathbf{T}$ is $\mathbf{S} \Rightarrow \mathbf{R}$.

¶ A *theorem* in $\mathscr{T}$ is a relation *which appears in a proof in* $\mathscr{T}$.

This notion is therefore essentially dependent on the state of the theory under consideration, at the time when it is being described. A relation in a theory $\mathscr{T}$ *becomes* a theorem in $\mathscr{T}$ when one succeeds in inserting it into a proof in $\mathscr{T}$. To say that a relation in $\mathscr{T}$ "is not a theorem in $\mathscr{T}$" cannot have any meaning without reference to the stage of development of the theory $\mathscr{T}$.

A theorem in $\mathscr{T}$ is also called a "*true* relation in $\mathscr{T}$" (or "proposition", "lemma", "corollary", etc.). Let $\mathbf{R}$ be a relation in $\mathscr{T}$, let $\mathbf{x}$ be a letter and $\mathbf{T}$ a term in $\mathscr{T}$; if $(\mathbf{T}|\mathbf{x})\mathbf{R}$ is a theorem in $\mathscr{T}$, $\mathbf{T}$ is said to *satisfy the relation* $\mathbf{R}$ in $\mathscr{T}$ (or to be a *solution of* $\mathbf{R}$), when $\mathbf{R}$ is considered as a relation in $\mathbf{x}$.

¶ A relation is said to be *false* in $\mathscr{T}$ if its negation is a theorem in $\mathscr{T}$. A theory $\mathscr{T}$ is said to be *contradictory* when one has written a relation which is both true and false in $\mathscr{T}$.

Here again, we are dealing with a notion that depends on the particular state of development of a theory. The reader should beware of the confusion (unfortunately suggested by the intuitive meaning of the word "false") which consists in believing that, once one has proved that a relation $\mathbf{R}$ is false in $\mathscr{T}$, one has thereby established that $\mathbf{R}$ "is not true" in $\mathscr{T}$ (strictly speaking, this phrase has no precise meaning *in mathematics*, as we have remarked above).

¶ In what follows we shall give metamathematical criteria, called *deductive criteria*, which will allow us to shorten proofs. These criteria will be denoted by the letter C followed by a number.

C1 (*Syllogism*). *Let $\mathbf{A}$ and $\mathbf{B}$ be relations in a theory $\mathscr{T}$. If $\mathbf{A}$ and $\mathbf{A} \Rightarrow \mathbf{B}$ are theorems in $\mathscr{T}$, then $\mathbf{B}$ is a theorem in $\mathscr{T}$.*

Let $R_1$, $R_2$, ..., $R_n$ be a proof in $\mathscr{T}$ in which $A$ appears, and let $S_1$, $S_2$, ..., $S_p$ be a proof in $\mathscr{T}$ in which $A \Rightarrow B$ appears. Clearly $R_1$, $R_2$, ..., $R_n$, $S_1$, $S_2$, ..., $S_p$ is a proof in $\mathscr{T}$ in which both $A$ and $A \Rightarrow B$ appear. Hence

$$R_1, \; R_2, \; \ldots, \; R_n, \; S_1, \; S_2, \; \ldots, \; S_p, \; B$$

is a proof in $\mathscr{T}$, and therefore $B$ is a theorem in $\mathscr{T}$.

### 3. SUBSTITUTIONS IN A THEORY

Let $\mathscr{T}$ be a theory, let $A_1$, $A_2$, ..., $A_n$ be its explicit axioms, let $x$ be a letter and $T$ a term of $\mathscr{T}$. Let $(T|x)\mathscr{T}$ be the theory whose signs and schemes are the same as those of $\mathscr{T}$, and whose explicit axioms are $(T|x)A_1$, $(T|x)A_2$, ..., $(T|x)A_n$.

C2. *Let $A$ be a theorem in a theory $\mathscr{T}$, let $T$ be a term of $\mathscr{T}$, and let $x$ be a letter. Then $(T|x)A$ is a theorem in the theory $(T|x)\mathscr{T}$.*

Let $R_1$, $R_2$, ..., $R_n$ be a proof in $\mathscr{T}$ in which $A$ appears. Consider the sequence $(T|x)R_1$, $(T|x)R_2$, ..., $(T|x)R_n$, which is a sequence of relations in $\mathscr{T}$ by reason of CF8 (§ 1, no. 4). We shall show that this sequence is a proof in the theory $(T|x)\mathscr{T}$; this will establish the criterion. If $R_k$ is an implicit axiom of $\mathscr{T}$, then $(T|x)R_k$ is again an implicit axiom of $\mathscr{T}$ (no. 1) and therefore of $(T/x)\mathscr{T}$. If $R_k$ is an explicit axiom of $\mathscr{T}$, then $(T|x)R_k$ is an explicit axiom of $(T|x)\mathscr{T}$. Finally, if $R_k$ is preceded by relations $R_i$ and $R_j$, where $R_j$ is $R_i \Rightarrow R_k$, then $(T|x)R_k$ is preceded by $(T|x)R_i$ and $(T|x)R_j$, and the latter is identical with $(T|x)R_i \Rightarrow (T|x)R_k$ (criterion CS5).

C3. *Let $A$ be a theorem of a theory $\mathscr{T}$, let $T$ be a term of $\mathscr{T}$, and let $x$ be a letter which is not a constant of $\mathscr{T}$. Then $(T|x)A$ is a theorem of $\mathscr{T}$.*

This follows immediately from C2, because $x$ does not feature in the explicit axioms of $\mathscr{T}$. More particularly, if $\mathscr{T}$ contains no explicit axioms, or if the explicit axioms contain no letters, then the criterion C3 applies without restriction on the letter $x$.

### 4. COMPARISON OF THEORIES

A theory $\mathscr{T}'$ is said to be *stronger* than a theory $\mathscr{T}$ if all the signs of $\mathscr{T}$ are signs of $\mathscr{T}'$, all the explicit axioms of $\mathscr{T}$ are theorems in $\mathscr{T}'$, and the schemes of $\mathscr{T}$ are schemes of $\mathscr{T}'$.

C4. *If a theory $\mathscr{T}'$ is stronger than a theory $\mathscr{T}$, then all the theorems of $\mathscr{T}$ are theorems of $\mathscr{T}'$.*

Let $R_1$, $R_2$, ..., $R_n$ be a proof in $\mathscr{T}$. We shall show, step by step, that each $R_i$ is a theorem in $\mathscr{T}'$. Suppose that this is true for the relations preceding $R_k$. If $R_k$ is an axiom of $\mathscr{T}$, it is a theorem in $\mathscr{T}'$ by hypothesis. If $R_k$ is preceded by relations $R_i$ and $R_i \Rightarrow R_k$, we know already that $R_i$ and $R_i \Rightarrow R_k$ are theorems in $\mathscr{T}'$, and therefore $R_k$ is a theorem in $\mathscr{T}'$ by virtue of C1. Hence, in every case, $R_k$ is a theorem in $\mathscr{T}'$, and the proof is complete.

If each of two theories $\mathscr{T}$ and $\mathscr{T}'$ is stronger than the other, $\mathscr{T}$ and $\mathscr{T}'$ are said to be *equivalent*. Then every theorem of $\mathscr{T}$ is a theorem of $\mathscr{T}'$, and vice versa.

C5. *Let $\mathscr{T}$ be a theory, let $A_1$, $A_2$, ..., $A_n$ be its explicit axioms, $a_1$, $a_2$, ..., $a_h$ its constants, and let $T_1$, $T_2$, ..., $T_h$ be terms in $\mathscr{T}$. Suppose that*

$$(T_1|a_1) \, (T_2|a_2) \, \ldots \, (T_h|a_h)A_i \qquad (\text{for} \quad i = 1, 2, \ldots, n)$$

*are theorems in a theory $\mathscr{T}'$, that the signs of $\mathscr{T}$ are signs of $\mathscr{T}'$, and that the schemes of $\mathscr{T}$ are schemes of $\mathscr{T}'$. Then, if $A$ is a theorem in $\mathscr{T}$,*

$$(T_1|a_1) \, \ldots \, (T_h|a_h)A$$

*is a theorem in $\mathscr{T}'$.*

For $\mathscr{T}'$ is stronger than the theory $(T_1|a_1) \ldots (T_n|a_n) \mathscr{T}$, and we can apply C2 and C4.

When we use this procedure to deduce a theorem in $\mathscr{T}'$ from a theorem in $\mathscr{T}$, we say that *we are applying in $\mathscr{T}'$ the results of $\mathscr{T}$*. Intuitively, the axioms of $\mathscr{T}$ express properties of $a_1, a_2, ..., a_h$, and $A$ expresses a property which is a consequence of these axioms. If the objects $T_1, T_2, ..., T_h$ in $\mathscr{T}'$ have the properties expressed by the axioms of $\mathscr{T}$, then they also have the property $A$.

\*For example, in the theory of groups $\mathscr{T}$, the explicit axioms contain two constants G and $\mu$ (the group and the law of composition). In the theory of sets $\mathscr{T}'$, we define two terms : the real line and addition of real numbers. If we substitute these terms for G and $\mu$ respectively in the explicit axioms of $\mathscr{T}$, we obtain theorems in $\mathscr{T}'$. Moreover, the schemes and signs of $\mathscr{T}$ and $\mathscr{T}'$ are the same. We may therefore "apply the results of group theory to the additive group of real numbers". We say that we have constructed a *model* for group theory in the theory of sets. (Note that since the theory of groups is stronger than the theory of sets, we can also apply the results of the theory of sets to the theory of groups.)\*

#### Remark {#ens-i-s2-n4-rem-1 .statement tag=03G7}

Under the hypotheses of C5, if the theory $\mathscr{T}$ turns out to be contradictory, the same will be true of $\mathscr{T}'$. For if $A$ and "not $A$" are theorems in $\mathscr{T}$, then $(T_1|a_1) \ldots (T_h|a_h)A$ and $\mathrm{not}(T_1|a_1) \ldots (T_h|a_h)A$ are theorems in $\mathscr{T}'$. \* For example, if the theory of groups were contradictory, the theory of sets would also be contradictory. \*

### Exercises {#ens-i-s2-exercises}

See the [exercises for § 2](exercises/s2/).

[^1]: For the sake of brevity, these rules are expressed by using the symbols mentioned in § 1, no. 1 (and especially bold-faced italic letters); but it would be easy to avoid the use of these symbols completely in the formulation of the rules (see § 3, no. 1, note (*) on p. 28).
