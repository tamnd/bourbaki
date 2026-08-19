Let $G$ be a graph. We write $\overset{-1}{G}(X)$ for the set of $x$ such that there exists $y \in X$ with $(x,y) \in G$.

**(a) implies (b).** Suppose $G$ is a functional graph and let $X$ and $Y$ be any two sets.

The inclusion $\overset{-1}{G}(X \cap Y) \subset \overset{-1}{G}(X) \cap \overset{-1}{G}(Y)$ holds for every graph, functional or not. Indeed, if $x \in \overset{-1}{G}(X \cap Y)$ there is a $y \in X \cap Y$ with $(x,y) \in G$; since $y \in X$ we get $x \in \overset{-1}{G}(X)$, and since $y \in Y$ we get $x \in \overset{-1}{G}(Y)$.

For the other inclusion, let $x \in \overset{-1}{G}(X) \cap \overset{-1}{G}(Y)$. There are $y_1 \in X$ and $y_2 \in Y$ with $(x,y_1) \in G$ and $(x,y_2) \in G$. Since $G$ is functional it has at most one second coordinate over $x$, so $y_1 = y_2$. Call this element $y$. It lies in $X$ and in $Y$, hence in $X \cap Y$, and $(x,y) \in G$, so $x \in \overset{-1}{G}(X \cap Y)$.

The two inclusions give $\overset{-1}{G}(X \cap Y) = \overset{-1}{G}(X) \cap \overset{-1}{G}(Y)$, which is (b).

**(a) implies (c).** Suppose again that $G$ is functional, and let $X$ and $Y$ satisfy $X \cap Y = \emptyset$. If some $x$ belonged to $\overset{-1}{G}(X) \cap \overset{-1}{G}(Y)$, there would be $y_1 \in X$ and $y_2 \in Y$ with $(x,y_1) \in G$ and $(x,y_2) \in G$, and $y_1 = y_2$ because $G$ is functional. That common element would lie in $X \cap Y$, which is empty. So no such $x$ exists and
$$\overset{-1}{G}(X) \cap \overset{-1}{G}(Y) = \emptyset,$$
which is (c).

Both (b) and (c) have been derived from (a), and each of them is a statement about the inverse images under $G$ of arbitrary sets. The three propositions (a), (b) and (c) are therefore equivalent.
