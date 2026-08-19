Let $R\{x,y\}$ be a relation, $x$ and $y$ distinct letters, and let $z$ be a letter distinct from both which does not appear in $R\{x,y\}$.

Every ordered pair $(x,y)$ satisfies $\operatorname{pr}_1 (x,y) = x$ and $\operatorname{pr}_2 (x,y) = y$ ($\S 2$, no. 1), and conversely every $z$ satisfies $z = (\operatorname{pr}_1 z, \operatorname{pr}_2 z)$. So the passage from the two letters $x$, $y$ to the single letter $z$ costs nothing, and we may read $R\{\operatorname{pr}_1 z, \operatorname{pr}_2 z\}$ as $R\{x,y\}$ with $x$ and $y$ recovered from $z$.

Suppose first that $(\exists x)(\exists y)R\{x,y\}$. Put $z = (x,y)$. Then $\operatorname{pr}_1 z = x$ and $\operatorname{pr}_2 z = y$, so $R\{\operatorname{pr}_1 z, \operatorname{pr}_2 z\}$ holds, and therefore $(\exists z)R\{\operatorname{pr}_1 z, \operatorname{pr}_2 z\}$.

Suppose conversely that $(\exists z)R\{\operatorname{pr}_1 z, \operatorname{pr}_2 z\}$, and let $z$ be such a $z$. Put $x = \operatorname{pr}_1 z$ and $y = \operatorname{pr}_2 z$. Then $R\{x,y\}$ holds, and therefore $(\exists x)(\exists y)R\{x,y\}$.

The two implications give
$$(\exists x)(\exists y)R\{x,y\} \iff (\exists z)R\{\operatorname{pr}_1 z, \operatorname{pr}_2 z\},$$
which is the first assertion.

For the second, apply what has just been proved to the relation $\neg R\{x,y\}$, which is a relation in the same theory and in which $z$ likewise does not appear. We obtain
$$(\exists x)(\exists y)\neg R\{x,y\} \iff (\exists z)\neg R\{\operatorname{pr}_1 z, \operatorname{pr}_2 z\}.$$
Negating both sides, and using that $\neg(\exists x)\neg S$ is equivalent to $(\forall x)S$ ($\S 4$, no. 1), we get
$$(\forall x)(\forall y)R\{x,y\} \iff (\forall z)R\{\operatorname{pr}_1 z, \operatorname{pr}_2 z\},$$
which is the second assertion.
