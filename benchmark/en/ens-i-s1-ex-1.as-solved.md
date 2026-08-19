Let $\mathscr{T}$ be a theory with no specific signs.
By the definition of species, an assembly is of the first species if it begins with $\tau$, or with a substantific sign, or consists of a single letter; otherwise it is of the second species. Since $\mathscr{T}$ has no specific signs, it has no substantific signs. Hence an assembly in $\mathscr{T}$ is of the first species exactly when it begins with $\tau$ or is a single letter; all other assemblies are of the second species.

A formative construction in $\mathscr{T}$ is a sequence of assemblies such that each assembly $A$ satisfies one of the following conditions (by the definition of formative construction):
(a) $A$ is a letter;
(b) there exists a preceding assembly $B$ of the second species with $A = \neg B$;
(c) there exist two preceding assemblies $B$, $C$ of the second species with $A = \vee BC$;
(d) there exist a preceding assembly $B$ of the second species and a letter $x$ with $A = \tau_x(B)$;
(e) there exist a specific sign $s$ of weight $n$ and $n$ preceding assemblies $A_1,\dots,A_n$ of the first species with $A = sA_1\dots A_n$.

Because $\mathscr{T}$ has no specific signs, condition (e) can never be satisfied.

We prove by induction on the length of a formative construction that every assembly in it is a single letter.
The first assembly of the construction cannot satisfy (b), (c), or (d) because these require a preceding assembly of the second species, and there is none. It cannot satisfy (e) because there are no specific signs. Hence it must satisfy (a); i.e., it is a letter.
Assume that all assemblies up to some position are letters. The next assembly again cannot satisfy (b), (c), or (d) because all preceding assemblies are letters, which are of the first species (a single letter is explicitly of the first species by definition), so no preceding assembly of the second species exists. Condition (e) remains impossible. Therefore this assembly must also be a letter. By induction, every assembly in the construction is a letter.

Consequently, no assembly of the second species ever appears in any formative construction of $\mathscr{T}$. By definition, the relations of $\mathscr{T}$ are exactly the assemblies of the second species that appear in its formative constructions; hence $\mathscr{T}$ has no relations.

The terms of $\mathscr{T}$ are the assemblies of the first species that appear in its formative constructions. The only such assemblies are the letters themselves (each consisting of a single letter). Assemblies beginning with $\tau$ would be of the first species, but they would have to be produced by condition (d), which requires a preceding assembly of the second species; since no such assembly exists, no assembly beginning with $\tau$ can appear. Thus the only terms in $\mathscr{T}$ are assemblies consisting of a single letter.
