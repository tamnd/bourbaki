---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 0
section_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
kind: front
lang: en
source: alg-i-iii
source_edition: 1998, Springer
book_pages: "427"
pdf_pages: 0451-0451
extraction: ocr
statements: 0
exercises: 0
content_sha256: 6265d61279faab9dcf08066eb99e498297b3d05106b7e1efab665fe26a7b784b
---

## CHAPTER III

# Tensor Algebras, Exterior Algebras, Symmetric Algebras

Recall the exponential notation introduced in Chapter I, of which we shall make frequent use (I, § 7, no. 8):

Let $(x_\lambda)_{\lambda \in L}$ be a family of pairwise permutable elements of a ring $A$; for every mapping $\alpha : L \to N$ of finite support we shall write

$$
x^\alpha = \prod_{\lambda \in L} x_\lambda^{\alpha(\lambda)}.
$$

If $\beta$ is another mapping of $L$ into $N$ of finite support, $\alpha + \beta$ denotes the mapping

$$
\lambda \mapsto \alpha(\lambda) + \beta(\lambda)
$$

of $L$ into $N$; with this law of composition the set $N^{(L)}$ of mappings of $L$ into $N$ of finite support is the free commutative monoid derived from $L$ and

$$
x^\alpha x^\beta = x^{\alpha + \beta}.
$$

For all $\alpha \in N^{(L)}$, we write $|\alpha| = \sum_{\lambda \in L} \alpha(\lambda) \in N$; then $|\alpha + \beta| = |\alpha| + |\beta|$; $|\alpha|$ is called the order of the "multiindex" $\alpha$. For all $\lambda \in L$, let $\delta_\lambda$ denote the element of $N^{(L)}$ such that $\delta_\lambda(\lambda) = 1$, $\delta_\lambda(\mu) = 0$ for $\mu \neq \lambda$ (Kronecker index); the $\delta_\lambda$ for $\lambda \in L$ are the only elements of $N^{(L)}$ of order 1. $N^{(L)}$ is given the ordering induced by the product ordering on $N^L$, so that the relation $\alpha \leq \beta$ is equivalent to "$\alpha(\lambda) \leq \beta(\lambda)$ for all $\lambda \in L$"; then the multiindex $\lambda \mapsto \beta(\lambda) - \alpha(\lambda)$ is denoted by $\beta - \alpha$, so that it is the unique multiindex such that $\alpha + (\beta - \alpha) = \beta$. For all $\alpha \in N^{(L)}$, there are only a finite number of multiindices $\beta \leq \alpha$; the $\delta_\lambda$ are the minimal elements of the set $N^{(L)} - \{0\}$; the relation $\alpha \leq \beta$ implies $|\alpha| \leq |\beta|$ and if both $\alpha \leq \beta$ and $|\alpha| = |\beta|$, then $\alpha = \beta$.

Finally, we write $\alpha! = \prod_{\lambda \in L} (\alpha(\lambda))!$, which is meaningful since $0! = 1$.

From § 4 to § 8 inclusive, $A$ denotes a commutative ring and, unless otherwise stated, the algebras considered are assumed to be associative and unital and the algebra homomorphisms are assumed to be unital.
