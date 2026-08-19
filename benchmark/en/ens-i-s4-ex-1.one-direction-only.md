Let $A$ and $B$ be relations in $\mathscr{T}$ and let $x$ be a letter which does not appear in $A$.

We argue in the theory $\mathscr{T}'$ obtained from $\mathscr{T}$ by adjoining $A \Rightarrow (\forall x)B$ as an explicit axiom, and we show that $(\forall x)(A \Rightarrow B)$ is a theorem of $\mathscr{T}'$.

Adjoin $A$ to $\mathscr{T}'$ as a further hypothesis and call the resulting theory $\mathscr{T}''$. In $\mathscr{T}''$ both $A$ and $A \Rightarrow (\forall x)B$ are theorems, so $(\forall x)B$ is a theorem of $\mathscr{T}''$ by the criterion of detachment C1 ($\S 2$, no. 2). Since $(\forall x)B$ is a theorem of $\mathscr{T}''$, so is $B$, by C27 ($\S 4$, no. 2), which lets a universal quantifier be removed. By the criterion of deduction C9 ($\S 3$, no. 3), the relation $A \Rightarrow B$ is therefore a theorem of $\mathscr{T}'$.

The letter $x$ is not a constant of $\mathscr{T}'$: it does not appear in $A$, and the only explicit axiom of $\mathscr{T}'$ over those of $\mathscr{T}$ is $A \Rightarrow (\forall x)B$, in which $x$ is bound. Hence C30 ($\S 4$, no. 2) applies to the theorem $A \Rightarrow B$ of $\mathscr{T}'$ and gives that $(\forall x)(A \Rightarrow B)$ is a theorem of $\mathscr{T}'$.

By the criterion of deduction C9 once more, applied now in $\mathscr{T}$,
$$(A \Rightarrow (\forall x)B) \Rightarrow (\forall x)(A \Rightarrow B)$$
is a theorem of $\mathscr{T}$. This is the assertion to be proved, and therefore
$$(\forall x)(A \Rightarrow B) \Leftrightarrow (A \Rightarrow (\forall x)B)$$
is a theorem in $\mathscr{T}$.
