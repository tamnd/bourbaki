---
book: alg
book_title: Algebra
chapter: III
chapter_title: ALGÈBRES TENSORIELLES, ALGÈBRES EXTÉRIEURES, ALGÈBRES SYMÉTRIQUES
section: 0
section_title: ALGÈBRES TENSORIELLES, ALGÈBRES EXTÉRIEURES, ALGÈBRES SYMÉTRIQUES
kind: front
lang: fr
source: alg-i-iii-fr
pdf_pages: 0388-0388
extraction: ocr
statements: 0
exercises: 0
content_sha256: 380c252d0d80d76a8eb6a81c6e6aeec31ffe094d2729be4a076947624ba9c783
---

## CHAPITRE III

# Algèbres tensorielles, algèbres extérieures, algèbres symétriques

Rappelons les notations exponentielles introduites au chapitre I et dont nous ferons un fréquent usage (I, p. 89):

Soit $(x_\lambda)_{\lambda \in L}$ une famille d’éléments d’un anneau $A$, deux à deux permutables; pour toute application $\alpha : L \to \mathbf{N}$, de support fini, nous poserons

$$
x^\alpha = \prod_{\lambda \in L} x_{\lambda}^{\alpha(\lambda)}.
$$

Si $\beta$ est une seconde application de $L$ dans $\mathbf{N}$, de support fini, on note $\alpha + \beta$ l’application $\lambda \mapsto \alpha(\lambda) + \beta(\lambda)$ de $L$ dans $\mathbf{N}$; muni de cette loi de composition, l’ensemble $\mathbf{N}^{(L)}$ des applications de $L$ dans $\mathbf{N}$, de support fini, est le monoïde commutatif libre déduit de $L$, et l’on a

$$
x^\alpha x^\beta = x^{\alpha + \beta}.
$$

Pour tout $\alpha \in \mathbf{N}^{(L)}$, on pose $|\alpha| = \sum_{\lambda \in L} \alpha(\lambda) \in \mathbf{N}$; on a donc $|\alpha + \beta| = |\alpha| + |\beta|$; on dit que $|\alpha|$ est l’ordre du « multiindice » $\alpha$. Pour tout $\lambda \in L$, on note $\delta_\lambda$ l’élément de $\mathbf{N}^{(L)}$ tel que $\delta_\lambda(\lambda) = 1$, $\delta_\lambda(\mu) = 0$ pour $\mu \neq \lambda$ (indice de Kronecker); les $\delta_\lambda$ pour $\lambda \in L$ sont les seuls éléments de $\mathbf{N}^{(L)}$ qui sont d’ordre 1. On munit $\mathbf{N}^{(L)}$ de l’ordre induit par l’ordre produit sur $\mathbf{N}^L$, de sorte que la relation $\alpha \leq \beta$ équivaut à « $\alpha(\lambda) \leq \beta(\lambda)$ pour tout $\lambda \in L$ »; on note alors $\beta - \alpha$ le multiindice $\lambda \mapsto \beta(\lambda) - \alpha(\lambda)$, de sorte que c’est l’unique multiindice tel que $\alpha + (\beta - \alpha) = \beta$. Pour tout $\alpha \in \mathbf{N}^{(L)}$, il n’y a qu’un nombre fini de multiindices $\beta \leq \alpha$; les $\delta_\lambda$ sont les éléments minimaux de l’ensemble $\mathbf{N}^{(L)} - \{0\}$; la relation $\alpha \leq \beta$ entraîne $|\alpha| \leq |\beta|$, et si l’on a à la fois $\alpha \leq \beta$ et $|\alpha| = |\beta|$, on en tire $\alpha = \beta$. Enfin, on pose $\alpha! = \prod_{\lambda \in L} (\alpha(\lambda))!$, ce qui a un sens puisque $0! = 1$.
