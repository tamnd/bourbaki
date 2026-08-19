Let us proceed by induction on the length of a formative construction of $\mathscr{T}$ that produces the term or relation $A$. Suppose that every assembly in the formative construction preceding $A$ satisfies the required condition: every specific sign (if present) is followed by $\square$, $\tau$, a letter, or a substantific sign. We verify that $A$ also satisfies the condition.

- **Condition (a):** $A$ is a single letter. The statement holds vacuously since there are no specific signs.

- **Condition (b):** $A = \neg B$ where $B$ is a relation. The specific signs in $A$ are those in $B$, which satisfy the condition by hypothesis. Hence $A$ does too.

- **Condition (c):** $A = \vee BC$ with $B$ and $C$ relations. The specific signs in $A$ are inherited from $B$ and $C$, which satisfy the condition.

- **Condition (d):** $A = \tau_x(B)$ where $B$ is a relation. By definition, $\tau_x(B)$ is $\tau$ followed by the assembly $B$ with each occurrence of $x$ replaced by $\square$ and linked to $\tau$. The $\tau$ here is a logical sign. The next signs after any specific sign in $B$ are either unchanged (and thus satisfy the hypothesis) or $\tau$ followed by $\square$ (in the case where a specific sign in $B$ was followed by $x$, now replaced by $\square$). Thus $\tau_x(B)$ satisfies the condition.

- **Condition (e):** $A = sA_1A_2 \dots A_n$, where $s$ is a specific sign and $A_1, \dots, A_n$ are terms. Since $A$ is a term or relation, $s$ must be a substantific sign (if $A$ is a term) or a relational sign (if $A$ is a relation). The first sign after $s$ is the first sign of $A_1$. Each $A_i$ is a term, hence of first species, so $A_1$ begins with $\tau$, a substantific sign, or is a single letter. These are allowed after $s$, as $\square$, $\tau$, or a letter. Remaining specific signs in $A$ come from the $A_i$, which satisfy the condition by hypothesis. Thus $A$ satisfies the condition.

By induction, every term or relation $A$ has the desired property.
