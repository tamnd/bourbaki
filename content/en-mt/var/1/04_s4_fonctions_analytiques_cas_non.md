---
book: var
book_title: Variétés différentielles et analytiques
chapter: "1"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 4
section_title: Fonctions analytiques (cas non archimédien)
lang: en
source: var-fr
pdf_pages: 0029-0032
extraction: ocr
subsections:
    - "no": 1
      title: Séries convergentes
      page: 0
      pdf_page: 29
    - "no": 2
      title: Fonctions analytiques
      page: 0
      pdf_page: 31
    - "no": 3
      title: Quelques inégalités
      page: 0
      pdf_page: 32
statements: 0
exercises: 0
content_sha256: 80985f908999f00f998e02079336ec6d5e99b09bf471da981e8d65cac53291cf
translated_from: content/fr/var/1/04_s4_fonctions_analytiques_cas_non.md
source_lang: fr
translation_method: machine
source_content_sha256: 6c33d48ae550ea870abdc7669dc0ffa3b18d55302bafba43eeb9d2a04fcc67f0
translation_model: gpt-5-6
translation_run: translate-en-mt-bf2986a6
glossary_version: 34
glossary_terms_sha256: 59ab868cd4e08ffea482680c524365ccfba8f218be2772edc9f927b313d83627
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 4. Analytic functions (ultrametric case)

In this paragraph, it is assumed that the absolute value of K is ultrametric. We denote by $(E_i)_{1 \leq i \leq n}$ a finite family of normed spaces over K, and by E the product space of the $E_i$, endowed with the norm:

$$
\|x\| = \sup \|x_i\| \quad \text{if } x = (x_i).
$$

We denote by F a separated polynormed space over K.

### 4.1. Convergent series

4.1.1. Let $f = \sum_a f_a$ be a formal series belonging to $\hat{P}(E_1, \ldots, E_n; F)$, (cf. Appendix). If $\gamma$ is a continuous seminorm on F, and $R = (R_i)$ is a system of $n$ real numbers $> 0$, we put

$$
\|f\|_{\gamma, R} = \sup_a \|f_a\|_\gamma R^\alpha.
$$

The definitions and results of No. 3.1.1 (second paragraph) and No. 3.1.2 apply without change; in particular, we define the spaces

$$
\mathcal{H}_R(E_1, \ldots, E_n; F) \quad \text{and} \quad \mathcal{H}(E_1, \ldots, E_n; F).
$$

4.1.2. The canonical isomorphism $j$ of $\hat{P}(E; F)$ onto $\hat{P}(E_1, \ldots, E_n; F)$ gives, by restriction, an isomorphism of topological vector spaces of $\mathcal{H}_R(E; F)$ onto $\mathcal{H}_{(R, \ldots, R)}(E_1, \ldots, E_n; F)$ for every $R \in \mathbf{R}_+^*$; it also gives an isomorphism of $\mathcal{H}(E; F)$ onto $\mathcal{H}(E_1, \ldots, E_n; F)$. More precisely, if $f = \sum_m f_m \in \hat{P}(E; F)$ and if $j(f) = \sum_a f_a$, one has, for every continuous seminorm $\gamma$ on F:

$$
\|f_m\|_\gamma = \sup_{|\alpha|=m} \|f_\alpha\|_\gamma
$$
$$
\|f\|_{\gamma, R} = \|j(f)\|_{\gamma, (R, \ldots, R)}.
$$

4.1.3. Let $f = \sum_a f_a$ be an element of $\mathcal{H}(E_1, \ldots, E_n; F)$; let $I(f)$ be the set of $R \in (\mathbf{R}_+^*)^n$ such that, for every continuous seminorm $\gamma$ on F, the product $\|f_\alpha\|_\gamma R^\alpha$ tends to zero when $|\alpha|$ tends to infinity. The set $I(f)$ is nonempty; it is called the strict convergence indicator of $f$. The set $\Omega(f)$ of the points

$$(\log R_1, \ldots, \log R_n) \quad \text{for } R \in I(f)$$

is a convex subset of $\mathbf{R}^n$.

When $n = 1$, the set $I(f)$ is an interval of $\mathbf{R}$, open on the left and open or closed on the right; its upper bound (finite or $+\infty$) is denoted by $\rho(f)$ and is called the *strict radius of convergence* of $f$.

With the notation of 4.1.2, one has $R \in I(f)$ if and only if
$$
(R, \ldots, R) \in I(j(f)).
$$
The set of points $x = (x_i)$ such that there exists $R = (R_i) \in I(f)$ with $\|x_i\| \leq R_i$ for $1 \leq i \leq n$ is called the *strict domain of convergence* of $f$ and is denoted by $C(f)$. It is an open subset of $E$, union of the polyballs
$$
B(R) = \{ x \in E \mid \|x_i\| \leq R_i \text{ for } 1 \leq i \leq n \},
$$
for $R \in I(f)$.

4.1.4. The results of 3.1.7 and 3.1.8 remain exact, on replacing everywhere $\tilde{C}(f)$ by $C(f)$ and $\tilde{\mathcal{H}}_R$ by $\mathcal{H}_R$.

4.1.5. Let $F_1, \ldots, F_m$ be complete normed spaces and suppose that $F$ is quasi-complete. Let $f = (f_i)_{1 \leq i \leq m}$, with $f_i \in \mathcal{H}(E_1, \ldots, E_n; F_i)$ and let $g \in \mathcal{H}(F_1, \ldots, F_m; F)$, such that the point $(f_i(0))_{1 \leq i \leq m}$ of $E$ belong to the strict domain of convergence of $g$. Then, for every $\alpha \in \mathbf{N}^m$, the formal series $g_\alpha \circ f$ belong to $\mathcal{H}(E_1, \ldots, E_n; F)$ and the family of the $g_\alpha \circ f$ is summable in $\mathcal{H}(E_1, \ldots, E_n; F)$ (therefore *a fortiori* in $\hat{P}(E_1, \ldots, E_n; F)$). Its sum will be denoted by $g \circ f$.

More precisely, there exist $R \in \bigcap_i I(f_i)$ and $R' \in I(g)$ such that
$$
\sup_{|\alpha| > 0} \|f_{i,\alpha}\| R^\alpha < R'_i \quad (\text{for } 1 \leq i \leq m).
$$
Under these conditions the formal series $g_\alpha \circ f$ belong to $\mathcal{H}_R(E_1, \ldots, E_n; F)$ and the family of the $g_\alpha \circ f$ is summable in $\mathcal{H}_R(E_1, \ldots, E_n; F)$. Finally, if $x \in B(R)$, then $f(x) = (f_i(x))$ belong to $C(g)$ and one has:
$$
g(f(x)) = (g \circ f)(x).
$$

Suppose moreover that, for each $i$, there exists a family $(e_j^i)$ of elements of $E_i$ such that every element $x$ of $E_i$ is the sum of a summable family $(\lambda_j e_j^i)$ (with $\lambda_j \in K$) such that $\|x\| = \sup_j |\lambda_j|$. One can then in the preceding paragraph replace the condition $\sup_{|\alpha| > 0} \|f_{i,\alpha}\| R^\alpha < R'_i$ by the condition $\|f_i\|_R \leq R'_i$.

4.1.6. Suppose that $E_i = K$ for $1 \leq i \leq n$. The space $\hat{P}(K^n; F)$ then identifies with the space of formal series in $n$ indeterminates $X_1, \ldots, X_n$ with coefficients in $F$ and an element $f$ of $\hat{P}(K^n; F)$ is written:
$$
f = \sum_a X^a c_a \quad \text{with } c_a \in F.
$$
If $R \in (\mathbf{R}_+^*)^n$ and if $\gamma$ is a continuous seminorm on $F$, one has:
$$
\|f\|_{\gamma, R} = \sup \|c_a\|_\gamma \cdot R^\alpha.
$$

The last paragraph of 3.1.10 remains valid, as does 3.1.11.

4.1.7. Suppose that K is a closed subfield of a complete valued field (necessarily ultrametric) L. For $y \in E_i \otimes_K L$, put:

$$
\|y\| = \inf_k (\sup |a_k| \cdot \|x_k\|)
$$

the greatest lower bound being extended to all finite families of pairs $(x_k, a_k) \in E_i \times L$ such that $y = \sum_k x_k \otimes a_k$. One thus obtains a norm on the L-vector space $E_i \otimes_K L$, which induces on $E_i$ the given norm. The completion of $E_i \otimes_K L$ for this norm is denoted by $E_i^L$.

Let now F be a separated complete polynormed L-vector space. For every K-continuous polynomial $f_\alpha$, homogeneous of multidegree $\alpha$, on $E_1 \times \cdots \times E_n$, with values in the underlying polynormed K-vector space $F_K$ of F, there exists one and only one L-continuous polynomial $\tilde{f}_\alpha$, homogeneous of the same multidegree, on $E_1^L \times \cdots \times E_n^L$, with values in F, which extends $f_\alpha$. For every continuous seminorm on the L-vector space F, one has

$$
\|\tilde{f}_\alpha\|_i = \|f_\alpha\|_i.
$$

If $f = \sum f_\alpha \in \mathcal{H}(E_1, \ldots, E_n; F_K)$, then $\tilde{f} = \sum \tilde{f}_\alpha \in \mathcal{H}(E_1^L, \ldots, E_n^L; F)$.

The series $f$ and $\tilde{f}$ have the same strict convergence indicator (and the same strict radius of convergence when $n = 1$).

Conversely, let L be a closed non-discrete subfield of K and let $E_i^0$ and $F^0$ be the spaces over L obtained by restriction of scalars from the $E_i$ and F. If $f = \sum f_\alpha \in \mathcal{H}(E_1, \ldots, E_n; F)$, then $f_\alpha \in P_\alpha(E_1^0, \ldots, E_n^0; F^0)$; if one sets $f^0 = \sum \tilde{f}_\alpha \in \hat{P}(E_1^0, \ldots, E_n^0; F^0)$, then $f^0 \in \mathcal{H}(E_1^0, \ldots, E_n^0; F^0)$.

One has $C(f) \subset C(f^0)$ and $f(x) = f^0(x)$ for every $x \in C(f)$.

### 4.2. Analytic functions

4.2.1. The definitions and results of 3.2.1 and 3.2.2 remain valid without changes.

4.2.2. With the notation of 3.2.2, the strict convergence indicator of the power series expansion of $\Delta^a f$ at a point $a$ of U contains that of the power series expansion of $f$ at $a$.

4.2.3. The results of 3.2.4, 3.2.5, 3.2.7, 3.2.8 and 3.2.11 remain exact. That of 3.2.6 also, provided in addition that K is assumed to be of characteristic zero.

4.2.4. Suppose F quasi-complete and let $f \in \mathcal{H}(E_1, \ldots, E_n; F)$. The mapping $x \mapsto f(x)$ is analytic in $C(f)$. For every $a \in C(f)$, the convergence indicator of the power series expansion of $f$ at $a$ is equal to that of $f$.

### 4.3. Some inequalities

4.3.1. It is assumed that K satisfies at least one of the following conditions:
(a) the residue field of K is infinite ;
(b) the image of K by the mapping $a \mapsto |a|$ is dense in $\mathbf{R}_+$. (In other words, it is assumed that K is not locally compact).
Let $f = \sum_\alpha f_\alpha \in \mathcal{H}(E_1, \ldots, E_n; F)$ and let $R \in I(f)$. One has:
$$
\sup_{x \in B(R)} \|f(x)\|_y = \sup_\alpha \sup_{x \in B(R)} \|f_\alpha(x)\|_y
$$
for every continuous seminorm $\gamma$ on F (“Cauchy inequalities”).

4.3.2. There exists a constant $a > 0$ such that for every continuous homogeneous polynomial $f_\alpha \in P_\alpha(E_1, \ldots, E_n; F)$ and every $R \in (\mathbf{R}_+^*)^n$, one has:
$$
a^{|\alpha|} R^{\alpha} |\alpha|! \|f_\alpha\|_y \leq \sup_{x \in B(R)} \|f_\alpha(x)\|_y \leq \|f_\alpha\|_y R^\alpha
$$
for every continuous seminorm $\gamma$ on F. If K satisfies condition (b) of 4.3.1 or if the image of $E_i$ by the mapping $x \mapsto \|x\|$ is contained in the image of K by the mapping $a \mapsto |a|$ and contains $R_i$ (for $1 \leq i \leq n$), one can take $a = 1$.

4.3.3. If K is of characteristic zero, the formal series $f = \sum_\alpha f_\alpha$ belongs to $\mathcal{H}(E_1, \ldots, E_n; F)$ if and only if there exists $R \in (\mathbf{R}_+^*)^n$ such that
$$
\sup_\alpha \sup_{x \in B(R)} \|f_\alpha(x)\|_y < +\infty
$$
for every continuous seminorm $\gamma$ on F.
