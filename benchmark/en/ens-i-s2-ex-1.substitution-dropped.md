**(a)** Let $\mathscr{T}'$ be the theory whose signs and schemes are those of $\mathscr{T}$ and whose explicit axioms are $A_1,\dots,A_{n-1}$. Every explicit axiom of a theory is a theorem of that theory, since it is on its own a proof of length one. Hence $A_1,\dots,A_{n-1}$ are theorems of $\mathscr{T}$, and as the two theories have the same signs and the same schemes, $\mathscr{T}$ is stronger than $\mathscr{T}'$.

Two theories are equivalent when each is stronger than the other. Since $\mathscr{T}$ is stronger than $\mathscr{T}'$ in any case, $\mathscr{T}'$ and $\mathscr{T}$ are equivalent exactly when $\mathscr{T}'$ is stronger than $\mathscr{T}$, that is, exactly when every explicit axiom of $\mathscr{T}$ is a theorem of $\mathscr{T}'$. The axioms $A_1,\dots,A_{n-1}$ are explicit axioms of $\mathscr{T}'$ and so are theorems of it, and nothing else is at stake. Therefore $\mathscr{T}'$ is equivalent to $\mathscr{T}$ if and only if $A_n$ is a theorem of $\mathscr{T}'$, and $A_n$ is independent of the other axioms if and only if $A_n$ is not a theorem of $\mathscr{T}'$.

**(b)** Write $\sigma$ for the substitution $(T_1|a_1)(T_2|a_2)\dots(T_h|a_h)$. We are given that $\sigma A_i$ is a theorem of $\mathscr{T}''$ for $i=1,\dots,n-1$, and that not $\sigma A_n$ is a theorem of $\mathscr{T}''$. Let $\mathscr{T}'$ be the theory of part (a).

Suppose that $A_n$ is not independent of the other axioms of $\mathscr{T}$. By (a), $A_n$ is then a theorem of $\mathscr{T}'$.

The theories $\mathscr{T}''$ and $\mathscr{T}'$ have the same signs and the same schemes. The explicit axioms of $\mathscr{T}'$ are $A_1,\dots,A_{n-1}$, and by hypothesis each of them is a theorem of $\mathscr{T}''$. Therefore $\mathscr{T}''$ is stronger than $\mathscr{T}'$, and by Criterion C4 every theorem of $\mathscr{T}'$ is a theorem of $\mathscr{T}''$. In particular $\sigma A_n$, being a theorem of $\mathscr{T}'$, is a theorem of $\mathscr{T}''$.

But not $\sigma A_n$ is a theorem of $\mathscr{T}''$ as well, and a theory in which a relation and its negation are both theorems is contradictory. Hence $\mathscr{T}''$ is contradictory.

We have shown that if $A_n$ is not independent then $\mathscr{T}''$ is contradictory. Consequently either $A_n$ is independent of the other axioms of $\mathscr{T}$, or $\mathscr{T}''$ is contradictory.
