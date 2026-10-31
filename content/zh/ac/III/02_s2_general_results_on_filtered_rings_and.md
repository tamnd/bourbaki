---
book: ac
book_title: Commutative Algebra
chapter: III
chapter_title: GRADUATIONS. FILTRATIONS AND TOPOLOGIES
section: 2
section_title: General results on filtered rings and modules
lang: zh
source: ac-i-vii
book_pages: 162-195, 233-245
pdf_pages: 0182-0215, 0253-0265
extraction: ocr
subsections:
    - "no": 1
      title: FILTERED RINGS AND MODULES
      page: 162
      pdf_page: 182
    - "no": 2
      title: THE ORDER FUNCTION
      page: 165
      pdf_page: 185
    - "no": 3
      title: THE GRADED MODULE ASSOCIATED WITH A FILTERED MODULE
      page: 165
      pdf_page: 185
    - "no": 4
      title: HOMOMORPHISMS COMPATIBLE WITH FILTRATIONS
      page: 169
      pdf_page: 189
    - "no": 5
      title: THE TOPOLOGY DEFINED BY A FILTRATION
      page: 170
      pdf_page: 190
    - "no": 6
      title: COMPLETE FILTERED MODULES
      page: 173
      pdf_page: 193
    - "no": 7
      title: LINEAR COMPACTNESS PROPERTIES OF COMPLETE FILTERED MODULES
      page: 176
      pdf_page: 196
    - "no": 8
      title: THE LIFT OF HOMOMORPHISMS OF ASSOCIATED GRADED MODULES
      page: 177
      pdf_page: 197
    - "no": 9
      title: THE LIFT OF FAMILIES OF ELEMENTS OF AN ASSOCIATED GRADED MODULE
      page: 179
      pdf_page: 199
    - "no": 10
      title: 'APPLICATION: EXAMPLES OF NOETHERIAN RINGS'
      page: 183
      pdf_page: 203
    - "no": 11
      title: COMPLETE m-ADIC RINGS AND INVERSE LIMITS
      page: 185
      pdf_page: 205
    - "no": 12
      title: THE HAUSDORFF COMPLETION OF A FILTERED MODULE
      page: 187
      pdf_page: 207
    - "no": 13
      title: THE HAUSDORFF COMPLETION OF A SEMI-LOCAL RING
      page: 192
      pdf_page: 212
statements: 57
exercises: 31
content_sha256: 3fb289c2bf32d665683856c07f0336daef7c6eff482b638340a053bb5a951429
translated_from: content/en/ac/III/02_s2_general_results_on_filtered_rings_and.md
translation_method: google
source_content_sha256: 0a34905c17ca45e9431cd3c4d11e11fd5e18faa0d9245992a206dca25aae5226
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 5bf385348ac2bb6809cc60d33c3ef4fa430a0dd0e2288f4aaa90cab963463e26
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 2。过滤后的环和模的一般结果

### 1.过滤环和模

#### 定义 1 {#ac-iii-s2-def-1 .statement tag=04DH}

An increasing (resp. decreasing) sequence $(G_n)_{n \in \mathbf{Z}}$ of subgroups of a group $G$ is called an increasing (resp. decreasing) filtration on $G$.
A group with a filtration is called a filtered group.

如果$(G_n)_{n \in \mathbf{Z}}$是群$G$上的递增（或递减）过滤，并且我们写成$G'_n = G_{-n}$，则显然$(G'_n)_{n \in \mathbf{Z}}$是$G$上的递减（或递增）过滤。因此，我们可以将我们的研究限制在递减过滤，因此，当我们谈到过滤时，我们指的是递减过滤，否则说明为除非。

给定群$G$上的递减过滤$(G_n)_{n \in \mathbf{Z}}$，显然$\bigcap_{n \in \mathbf{Z}} G_n$和$\bigcup_{n \in \mathbf{Z}} G_n$是$G$的子群；如果$\bigcup_{n \in \mathbf{Z}} G_n$减少到单位元素，则称为分离过滤；如果$\bigcup_{n \in \mathbf{Z}} G_n = G$，则称为彻底过滤。

#### 定义 2 {#ac-iii-s2-def-2 .statement tag=04DI}

给定环$A$，加法群$A$上的过滤$(A_n)_{n \in \mathbf{Z}}$被称为与$A$上的环结构兼容，如果

(1)
$$
A_m A_n \subset A_{m+n} \quad \text{for} \quad m \in \mathbf{Z}, \quad n \in \mathbf{Z}
$$

(2)
$$
1 \in A_0.
$$
经过此过滤的环$A$称为过滤后的环。

条件（1）和（2）表明$A_n$是$A$和$A_n$（左和右）$A_0$模块的子环。 集合$B = \bigcup_{n \in \mathbf{Z}} A_n$是$A$和集合$n = \bigcap_{n \in \mathbf{Z}} A_n$的子环，$B$的两侧理想；对于如果 $x \in n$ 和 $a \in A_k$ 对于所有 $k \in \mathbf{Z}$、$x \in A_{k-p}$、从而 $ax \in A$ 和 $xa \in A$，通过 (1)；因此$ax \in n$和$xa \in n$。

一个重要的特殊情况是 $A_n = A$;那么$A_n = A$对于$n \leq 0$并且所有$A_n$都是$A$的两侧理想。

#### 定义 3 {#ac-iii-s2-def-3 .statement tag=04DJ}

令$A$为过滤后的环，$(A_n)_{n \in \mathbf{Z}}$为过滤后的$E$为$A$模块。 $E$ 上的过滤 $(E_n)_{n \in \mathbf{Z}}$ 被称为与过滤后的环 $A$ 上的模结构兼容，如果
$$
A_m E_n \subset E_{m+n} \quad \text{for} \quad m \in \mathbf{Z}, \quad n \in \mathbf{Z}.
$$
具有此过滤的$A$-模块$E$称为过滤后的模。

The $E_n$ are all $A_n$-modules; if $B = \bigcup_{n \in \mathbf{Z}} A_n$, clearly $\bigcup_{n \in \mathbf{Z}} E_n$ is a $B$-module and so is $\bigcap_{n \in \mathbf{Z}} E_n$ by the same argument as above for $\bigcap_{n \in \mathbf{Z}} A_n$. 如果$A_n = A$，则所有$E_n$都是$E$的子模。

Examples

(1) 设$A$为型$\mathbf{Z}$的分级环；对于所有$i \in \mathbf{Z}$，令$A_{(i)}$为$A$中次数$i$的齐次元素的子群。让我们写$A_n = \sum_{i \geq n} A_{(i)}$；那么就是直接的，$(A_n)$是一个详尽且分离的递减过滤，与$A$上的环结构兼容；据说该过滤与分级$(A_{(i)})_{i \in \mathbf{Z}}$相关，而过滤后的环$A$据说与给定的分级环$A$相关。

现在让$E$是型$\mathbf{Z}$的分级模超过分级环$A$并且对于所有$i \in \mathbf{Z}$让$E_{(i)}$是次数的同质元素的子群 $i$ / $E$。让我们写$E_n = \sum_{i \geq n} E_{(i)}$；那么$(E_n)$是彻底且分离的递减过滤，它与过滤后的环$A$上的$E$上的模结构兼容；据说该过滤与分级$(E_{(i)})_{i \in \mathbf{Z}}$相关，而过滤后的模$E$据说与给定的分级模$E$相关。

(2) Let $A$ be a filtered ring, $(A_n)_{n \in \mathbf{Z}}$ its filtration and $E$ an $A$-module. 让我们写$E_n = A_n E$；由(1)可知
$$
A_m E_n = A_m A_n E \subset A_{m+n} E = E_{m+n},
$$
并从 (2) 得出 $E_0 = E$；那么$(E_n)$是一个穷举过滤，它与$E$上的$A$模块结构兼容。 据说该过滤源自$A$上给定的过滤$(A_n)$； 注它不一定是分离的，即使$(A_n)$被分离并且$E$和$A_n$是有限生成的$A$-模块（cf.，习题2；但是参见§ 3, no. 3，命题5和no. 2， 命题 4) 的推论

(3) 设$A$为环，且$m$为$A$的双面理想。让我们为$n \geq 0$写为$A_n = m^n$，为$n < 0$写为$A_n = A$； 直接的$(A_n)$是$A$的穷举过滤，称为$m$-adic过滤。设$E$为$A$模块；由$A$上的$m$-adic过滤衍生而来的过滤$(E_n)$称为$E$上的$m$-adic过滤；在其他字，$E_n = m^n E$为$n \geq 0$，$E_n = E$为$n < 0$。

如果$A$是可交换的并且$B$是$A$-代数，则$n = mB$是$B$的双面理想，并且对于每个$B$模$F$，$n^k F = m^k F$，因此$n$-adic过滤$F$ 重合带有 $m$-adic 过滤（如果 $F$ 被视为 $A$-模块）。

(4) 如果$A$是过滤后的环且$(A_n)$是其过滤，则左侧$A$模块$A_n$是过滤后的$A$模块且具有过滤$(A_n)$。另一方面，显然$(A_n)$是一个与逆环$A^0$上的环结构兼容的过滤，而$A_n$是一个带有过滤$(A_n)$的过滤（左）$A^0$模块。

(5) 在环 $A$ 集合 $A_n$ 上，$A_n = 0$ $n > 0$，$A_n = A$ $n \leq 0$ 形式与 (例 1) 的平凡毕业相关的所谓平凡过滤$A$；在$A$-模块$E$上，子$A$-模块的每个过滤$(E_n)$由……组成然后与过滤后的环$A$上的$E$上的模结构兼容。那么可以说，如果 $\mathbf{Z}$ 被给予平凡的过滤，则每个过滤交换群 $G$ 都是过滤的 $\mathbf{Z}$ 模块。

设$G$为过滤后的群，$(G_n)_{n \in \mathbf{Z}}$为过滤后的群；显然，对于$G$的每一个子群$H$，$(H \cap G_n)_{n \in \mathbf{Z}}$据说是由$G$上的过滤引起的；如果 $G$ 上的内容是详尽的（或分离的）。类似地，若$H$是$G$的正规子群，$((H.G_n)/H)_{n \in \mathbf{Z}}$族就是群$G/H$的过滤，称为$G$过滤在$H$下的商；如果 $(G_n)$ 是详尽的。如果$G'$是另一个过滤了群并且$(G'_n)_{n \in \mathbf{Z}}$过滤了，那么$(G_n \times G'_n)$是$G \times G'$上的过滤，称为$G$和$G'$上过滤的乘积，这是详尽的（分别是分离的）如果$(G_n)$ 和 $(G'_n)$ 是。

现在让$A$是过滤后的环，$(A_n)$是它的过滤；在$A$的每个子环$B$上，显然$A$上引起的过滤与$B$上的环结构兼容。如果$b$是$A$的双边理想，则$A$在$A/b$上的商过滤与该环的结构兼容，对于
$$
(A_n + b)(A_m + b) \subset A_{n+m} + b.
$$
如果$A'$经过另一个过滤环，则$A \times A'$上的乘积过滤与此环的结构兼容。

Finally let $E$ be a filtered $A$-module and $(E_n)$ its filtration; on every submodule $F$ of $E$, the filtration induced by that on $E$ is compatible with the $A$-module structure on $F$ and, on the quotient module $E/F$, the quotient filtration of that on $E$ is compatible with the $A$-module structure, as
$$
A_n(F + E_m) \subset F + A_n E_m \subset F + E_{m+n}.
$$

注，如果 E 上的过滤源自 A 上的过滤 (例 2)，则 E/F 上的商过滤也是如此，但*不是*一般情况下*F 上的过滤会引起*（习题 1；但请参阅 no. 2、定理 2）

如果E'是另一个过滤A-模，则E×E'上的乘积过滤与其A-模结构兼容。如果 E 和 E' 上的过滤源自 A (例 2) 上的过滤，那么它们的乘积过滤也是如此。

### 2.阶函数

令 A 为过滤后的环，E 为过滤后的 A-模，(E_n) 对 E 进行过滤。对于所有 x ∈ E，让 v(x) 表示集合的 R 中在整数 n ∈ Z 上的*最小* 上界，使得 x ∈ E_n。那么下面的等价成立：

$$
\begin{cases}
v(x) = -\infty \Leftrightarrow x \notin \bigcup_{n \in \mathbf{Z}} E_n \\
v(x) = p \Leftrightarrow x \in E_p \text{ and } x \notin E_{p+1} \\
v(x) = +\infty \Leftrightarrow x \in \bigcap_{n \in \mathbf{Z}} E_n
\end{cases}
$$

映射 v : E → \overline{\mathbf{R}} 被称为过滤后的模 E 的阶函数。如果 v 已知，则 E_n 也已知，因为 E_n 是 x ∈ E 的集合，使得 v(x) ≥ n； E_n 是 E 的加法子群意味着关系

$$
v(x - y) \geq \inf(v(x), v(y)).
$$

上述定义特别适用于过滤后的A-模A；令 w 为其阶函数。由 no. 1 的方程（3）可知，对于 a ε A 且 x ε E，

$$
v(ax) \geq w(a) + v(x)
$$
每当定义右侧时；特别是，对于 a ∈ A 和 b ∈ A，

$$
w(ab) \geq w(a) + w(b)
$$
每当定义右侧时。

*阶函数* 在过滤的群 G 上的定义类似，它不一定是可交换的；然后将相应的关系写成 (5)

$$
v(yx^{-1}) = v(xy^{-1}) \geq \inf(v(x), v(y)).
$$

### 3. 分级模与过滤模相关

设 G 是可交换的群 （加法写）和 (G_n) 对 G 的过滤。让我们写

$$
\begin{align*}
\operatorname{gr}_n(G) &= G_n / G_{n+1} \quad \text{for } n \in \mathbf{Z} \\
\operatorname{gr}(G) &= \bigoplus_{n \in \mathbf{Z}} \operatorname{gr}_n(G).
\end{align*}
$$

那么交换性群 gr(G) 就是型 $\mathbf{Z}$ 的分级群，称为与过滤的群 G 伴随的*分级群，gr(G) 次数 $n$ 的齐次元素是$\mathrm{gr}_n(G)$。

现在让 A 为过滤后的环，(A_n) 为过滤后的 A-模，E 为过滤后的 A-模，(E_n) 为过滤后的。对于所有 $p \in \mathbf{Z}$、$q \in \mathbf{Z}$、映射

$$
\mathrm{gr}_p(A) \times \mathrm{gr}_q(E) \to \mathrm{gr}_{p+q}(E)
$$

is defined as follows: given $a \in \mathrm{gr}_p(A)$, $\xi \in \mathrm{gr}_q(E)$, two representatives $a, a'$ of $a$ and two representatives $x, x'$ of $\xi$, $ax \in E_{p+q}$, $a'x' \in E_{p+q}$ and $ax \equiv a'x'$ (mod. $E_{p+q+1}$), for

$$
ax - a'x' = (a - a')x + a'(x - x')
$$

以及$a - a' \in A_{p+1}$和$x - x' \in E_{q+1}$，因此我们的断言是从no. 1的公式(3)得出的。因此，我们可以用 $\alpha\xi$ 类来表示

$$
E_{p+1}/E_{p+q+1} = \mathrm{gr}_{p+q}(E)
$$

任何代表 $a \in a$ 和任何代表 $x \in \xi$ 的乘积 $ax$。 映射 (9) 是*Z-双线性* 是直接的；通过线性，我们推导出 $\mathbf{Z}$-双线性映射

$$
\mathrm{gr}(A) \times \mathrm{gr}(E) \to \mathrm{gr}(E).
$$

If this definition is first applied to the case $E = A_0$, the mapping (10) is an internal law of composition on $\mathrm{gr}(A)$, which it is immediately verified is *associative* and has an identity element which is the canonical image in $\mathrm{gr}_0(A)$ of the unit element of A; it therefore defines on $\mathrm{gr}(A)$ a ring structure and the graduation $(\mathrm{gr}_n(A))_{n \in \mathbf{Z}}$ is by definition compatible with this structure. 由此定义的分级环$\mathrm{gr}(A)$（型$\mathbf{Z}$）称为与过滤后的环A相关的*分级环；如果 A 是可交换的，那么它显然是可交换的； $\mathrm{gr}_0(A)$ 是$\mathrm{gr}(A)$ 的子环。 另一方面，映射（10）是$\mathrm{gr}(E)$上的$\mathrm{gr}(A)$模外法则，模公理是微不足道的满足，并且$\mathrm{gr}(E)$上的毕业$(\mathrm{gr}_n(E))_{n \in \mathbf{Z}}$显然与这个模结构兼容。 由此定义的分级$\mathrm{gr}(A)$-模块$\mathrm{gr}(E)$（型$\mathbf{Z}$）称为与过滤后的A-模E关联的*分级模。

*例*

#### 例 1 {#ac-iii-s2-n3-exa-1 .statement tag=04DK}

令 A 为 A 的交换环和 $t$ 元素，它不是 0 的除子。让我们给 A *(t)*-*adic 过滤* (no. 1, *例 3*)。那么相关的分级环 $\mathrm{gr}(A)$ 与 *多项式环* $(A/(t))[X]$ 是规范同构的。对于 $\mathrm{gr}_n(A) = 0$ $n < 0$ 以及定义环 $\mathrm{gr}_0(A)$ 是环 $A/(t)$。我们现在注凭借$t$关系$at^n \equiv 0$（mod.$t^{n+1}$）上的假设等价于$a \equiv 0$（mod.$t$）；如果$\tau$是$\mathrm{gr}_1(A)$中$t$的典范像，则$\mathrm{gr}_n(A)$中的每个元素可以唯一地写在形式$\alpha \tau^n$中，其中$\alpha \in \mathrm{gr}_0(A)$； 从而我们的断言。

#### 例 2 {#ac-iii-s2-n3-exa-2 .statement tag=04DL}

设$K$为形式幂级数的交换环、$A$环

$$
K[[X_1,\ldots,X_r]]
$$

(*代数, 章 IV, § 5*) 和 $m$ $A$ 的理想，其中元素是正式的幂级数，没有常数项。让我们给 $A$ $m$-adic *过滤* (no. 1, *例 3*);如果$M_1,\ldots,M_s$是总计次数$n-1$中$X_1,\ldots,X_r$中的不同单项式，则显然总计阶$\omega(u)\geq n$中的每个正式幂级数$u$

*（前述，no. 2）*可写为$\displaystyle\sum_{k=1}^{s}u_kM_k$，其中$u_k$属于至$m$； **看出**，$m^n$是形式幂级数$u$的集合，使得$\omega(u)\geq n$，这表明$\omega$是$m$-adic过滤的*阶函数*。那么显然，对于每个形式的幂级数 $u\in m^n$，在 $X_i$ 中都存在一个唯一的“齐次多项式”次数 $n$，它与 $u$ mod 全等。 $m^{n+1}$，即$u$次数$n$项和；我们结论 $\operatorname{gr}(A)$ 与 *多项式环* $K[X_1,\ldots,X_r]$ 自然同构。

#### 例 3 {#ac-iii-s2-n3-exa-3 .statement tag=04DM}

更一般地，令 $A$ 为交换环，$b$ $A$ 的理想值，并且$A$ 被赋予$b$-adic 过滤。如果我们写$B=\operatorname{gr}_0(A)$，$F=\operatorname{gr}_1(A)=b/b^2$，我们知道（*代数，章III*），$B$模块$F$的恒等映射可以从*对称唯一地扩展到同态$u$ $F$ 的代数* $S(F)$ 到 $B$-代数 $\operatorname{gr}(A)$；从 $\operatorname{gr}(A)$ 的定义可以得出，$u$ 是分级代数* 的 *满同态；对于$n\geq1$，$\operatorname{gr}_n(A)$的每元素是类和模形式$y=x_1x_2\cdots x_n$元素$b^{n+1}$，其中$x_i\in b$$(1\leq i\leq n)$；如果 $\xi_i$ 是 $x_i$ mod 的类。 $b^2$，显然是 $y$ mod 的类。 $b^{n+1}$是元素$u(\xi_1)\cdots u(\xi_n)$，从而我们的断言。特别地，$B$-模$F$的生成元的每个系统是$B$-代数$\operatorname{gr}(A)$的系统或生成元。

如果现在$E$是一个$A$模块，并且$E$被给予$b$-adic过滤，则可以类似地看到分级的$\operatorname{gr}(A)$模块$\operatorname{gr}(E)$是由$\operatorname{gr}_0(E)=E/bE$*生成*的。准确地说，$\operatorname{gr}(A)$-模块$\operatorname{gr}(E)$上外法则的限制$\phi$到$\operatorname{gr}(A)\times\operatorname{gr}_0(E)$是$\operatorname{gr}(A)\times\operatorname{gr}_0(E)$到$\operatorname{gr}(E)$的$\mathbf{Z}$双线性映射；此外，$\operatorname{gr}(A)$是$(\operatorname{gr}_0(A),\operatorname{gr}_0(A))$双模，$\operatorname{gr}_0(E)$是$\operatorname{gr}_0(A)$双模；立即验证，对于$a\in\operatorname{gr}(A)$，$\alpha_0\in\operatorname{gr}_0(A)$，$\xi\in\operatorname{gr}_0(E)$，

$$
\phi(a\alpha_0,\xi)=\phi(a,\alpha_0\xi)
$$

因此 $\phi$ 定义一个*满射* $\operatorname{gr}_1(A)$-线性映射

(11)

$$
\gamma_E:\operatorname{gr}(A)\otimes_{\operatorname{gr}_0(A)}\operatorname{gr}_0(E)\longrightarrow\operatorname{gr}(E)
$$

这被称为*规范*。

#### 例 4 {#ac-iii-s2-n3-exa-4 .statement tag=04DN}

\* 令$K$为交换环，$\mathfrak g$李代数超过$K$，$U$为$\mathfrak g$的包络代数。 *递增过滤*$(U_n)_{n\in\mathbf{Z}}$是在$U$上定义的，右$n<0$取$U_n=\{0\}$并用$U_n$表示，对于$U$的元素的$n\geq0$集合可表示为和的乘积最多 $n$ 元素的 $\mathfrak g$，那么

U_0 = K 且 gr(U) 为交换K-代数（李群和李代数、章 I, § 2, no. 6）。 g 的典范映射到 gr_1(U) = U_1/U_0 可以唯一地扩展到 K-模 g 到 K-代数 gr(U) 的对称代数 $S(g)$ 的同态 h； 同态 h 是满射，如果 K-模 g 是自由的，则 h 是双射（前述，no. 7，定理 1）。

#### 例 5 {#ac-iii-s2-n3-exa-5 .statement tag=04DO}

令A为型$\mathbf{Z}$的分级环，E为型$\mathbf{Z}$的分级A-模；设 $A_{(i)}$（分别为 $E_{(i)}$）为 A（分别为 E）的次数 i 的齐次元素的子群。令 A 和 E 被赋予与其分级相关的过滤（no. 1，例 1），并令 A' 和 E' 表示由此获得的过滤后的环和过滤后的 A-模。那么$A_{(n)}$的映射元素到其典范像的Z线性映射$A \to \mathrm{gr}(A')$就是直接的
$$
\mathrm{gr}_n(A) = \left( \bigoplus_{i \geq n} A_{(i)} \right) / \left( \bigoplus_{i \geq n+1} A_{(i)} \right)
$$
等级为环同构。规范分级 A-模同构 $E \to \mathrm{gr}(E')$ 的定义类似。

#### 命题 1 {#ac-iii-s2-prop-1 .statement tag=04DP}

设 A 为过滤后的环，$(A_n)_{n \in \mathbf{Z}}$ 为过滤函数，v 为其阶函数。假设 $\mathrm{gr}(A)$ 是环，没有除子或零。然后，对于元素 a、环 $B = \bigcup_{n \in \mathbf{Z}} A_n$、$v(ab) = v(a) + v(b)$ 的每个有序对、b。

由于 $n = \bigcap_{n \in \mathbf{Z}} A_n$ 是环 B 的双面理想，因此如果 $v(a)$ 或 $v(b)$ 等于 $+\infty$，则公式成立。如果不是，$v(a) = r$和$v(b) = s$就是整数；模组的类$\alpha$。 b mod 的 A、+ 和 $\beta$。 A，+_1 是 $\mathrm{gr}(A)$ 中的 $\neq 0$ × 定义、从而 × 假设 $\alpha \beta \neq 0$，因此 $ab \notin A_{r+s+1}$，如 $ab \in A_{r+s}$，
$$
v(ab) = v(a) + v(b).
$$

#### 推论{#ac-iii-s2-n3-cor-1 .statement tag=04DQ}

设 A 为过滤后的环和其过滤后的 $(A_n)_{n \in \mathbf{Z}}$；让我们集合$B = \bigcup_{n \in \mathbf{Z}} A_n$，$n = \bigcap_{n \in \mathbf{Z}} A_n$。如果环 $\mathrm{gr}(A)$ 没有零的除子，则也没有环 $B/n$。
如果 a 和 b 是 B 的元素，而不是属于到 n，则 $v(a) \neq +\infty$ 和 $v(b) \neq +\infty$、从而 $v(ab) \neq +\infty$，因此$ab \notin n$。

注，环 A 可以是整环，且过滤 (A_n) 是彻底且分离的，而 $\mathrm{gr}(A)$ 不会是整环 (习题 2)。

#### 注 {#ac-iii-s2-n3-rem-1 .statement tag=04DR}

令 G 为群，它不一定与过滤 $(G_n)_{n \in \mathbf{Z}}$ 交换，使得 $G_{n+1}$ 在 G 中是正规的，对于所有 $n \in \mathbf{Z}$；再次让$\mathrm{gr}_n(G) = G_n/G_{n+1}$。 $(\mathrm{gr}_n(G))_{n \in \mathbf{Z}}$族的受限乘积，即乘积$\prod_{n \in \mathbf{Z}} \mathrm{gr}_n(G)$由……组成的元素$(\xi_n)$的子群，其所有分量（最多除了有限的数）都等于单位元素，也称为与G相关的分级群，记为$\mathrm{gr}(G)$。

### 4. 同态与过滤兼容

令G、G'为两个交换律群（相加地写），(G_n) 对G 的过滤和(G'_n) 对G' 的过滤； 同态 h : G → G' 被称为与 G 和 G' 上的过滤兼容，如果 h(G_n) ⊂ G'_n 对于所有 n ∈ Z。复合同态 G_n $\xrightarrow{h} G'_n \longrightarrow G'_n/G'_{n+1}$ 在 G_{n+1} 上是零，因此通过取商得到定义同态 h_n : G_n/G_{n+1} → G'_n/G'_{n+1};因此，存在唯一的加法群同态 gr(h) : gr(G) → gr(G')，这样，对于所有 n ∈ Z，gr(h) 重合，其中 h_n 位于 gr_n(G) = G_n/G_{n+1} 上。 gr(h) 称为与 h 相关的分级群同态。如果 G'' 是第三个过滤群并且 h' : G' → G'' 同态与过滤兼容，则 h' ∘ h 是同态与过滤兼容并且

(12)
$$
\operatorname{gr}(h' \circ h) = \operatorname{gr}(h') \circ \operatorname{gr}(h)
$$

#### 命题 2 {#ac-iii-s2-prop-2 .statement tag=04DS}

设 G 是 G 的过滤交换群和 H 子群；令 H 为诱导过滤，G/H 为商过滤。如果 j : H → G 为典范嵌入并且 p : G → G/H 典范满射，则 j 和 p 与过滤兼容且序列

(13)
$$
0 \longrightarrow \operatorname{gr}(H) \xrightarrow{\operatorname{gr}(j)} \operatorname{gr}(G) \xrightarrow{\operatorname{gr}(p)} \operatorname{gr}(G/H) \longrightarrow 0
$$
是准确的。

第一个断言很明显；如果(G_n)是G上的过滤，那么
$$
(H \cap G_n) \cap G_{n+1} = H \cap G_{n+1}
$$
因此 gr(j) 是单射的；而且典范映射
$$
G_n \to (H + G_n)/H
$$
是满射，因此 gr(p) 和 gr(p) ∘ gr(j) = 0 by (12) 也是满射。最后令gr(p)的$\xi \in G_n/G_{n+1}$属于到核；则存在 x ε ψ 使得 x ε H + G_{n+1}；但由于 G_{n+1} ⊂ G，
$$
G_n \cap (H + G_{n+1}) = (H \cap G_n) + G_{n+1}
$$
因此 x = y + z 其中 y ∈ H ∩ G，且 z ∈ G, +_1；这证明了 xi 是类 mod。 G，j(y)的+_1，在gr(j)下gr(H)的其他字它属于到像。

注给定正合序列 0 → G' \xrightarrow{u} G \xrightarrow{v} G'' → 0 过滤交换性群，其中 u 和 v 与过滤兼容， 序列 0 \longrightarrow \operatorname{gr}(G') \xrightarrow{\operatorname{gr}(u)} \operatorname{gr}(G) \xrightarrow{\operatorname{gr}(v)} \operatorname{gr}(G'') \longrightarrow 0 不一定是精确的 (习题 4)。

如果现在A和B是两个过滤的环和h：A→B环同态，与过滤兼容，则立即验证分级的群同态gr(h)：gr(A)→gr(B)也是环同态。特别是，如果通过诱导过滤，A' 是 A 的子环，则 gr(A') 可以被规范地识别为 gr(A) 的分级子环 (命题 2)；如果 b 是 A 的两侧理想，并且 A/b 被给予商过滤，则 gr(A/b) 被规范地识别为等级为环 gr(A)/gr(b) (命题 2) 的商。

最后，令 A 为过滤后的环，E、F 为过滤后的 A-模，并且 u : E → F 同态与过滤兼容。那么直接的 gr(u) : gr(E) → gr(F) 是 gr(A)-线性映射，因此是分级 gr(A)-模块的次数 0 的齐次同态。此外，如果 u' : E → F 是另一个 A 同态，与过滤兼容，那么 u + u' 也是如此，并且

$$
\operatorname{gr}(u + u') = \operatorname{gr}(u) + \operatorname{gr}(u').
$$

Remarks

(1) 与过滤兼容的清晰过滤环同态（在给定的过滤环 A 上分别过滤的模的同态）可以视为过滤的环结构的态射（分别过滤的A-模结构）(集合)理论，章IV, § 2, no. 1）。

(2) 令 E 和 F 是经过过滤的环 A 上的两个模，并让它们具有从 A 上的过滤 (A_n) 导出的过滤 (no. 1，例 2)。那么每个 A-线性映射 u : E → F 都与过滤兼容，因为

$$
u(A_nE) = A_nu(E) \subset A_nF.
$$

(3) 注与过滤兼容的过滤后的 A-模同态 u : E → F 可以满足 gr(u) = 0 而不是零；对于自同态 x ↦ nx 的加法群 $\mathbf{Z}$ 的例以及 (n)-adic 过滤（对于任何整数 n > 1）都是如此。对于 E 到 F 的两个同态 u, v，关系 gr(u) = gr(v)，与过滤兼容，因此并不一定意味着 u = u。

(4) 定义在本号开头。 扩展立即到两个群 G, G'，它们不一定是可交换的，并通过子群 $G_n, G'_n$ 过滤，使得 $G_{n+1}$（或 $G'_{n+1}$）在 G 中是正规的，（或$G'_n$）。 命题 2 对于 G 的相同假设也是有效的，并且假设 H 在 G 中是不变的，证明除了记号之外保持不变。

### 5. 由过滤定义的拓扑

Let G be a group filtered by a family $(G_n)_{n \in \mathbf{Z}}$ of normal subgroups of G. G上存在唯一的拓扑，它与群结构兼容，并且G_n构成G的单位元素e的邻域的基系统（通则拓扑、章III, § 1, no. 2、例）；它在由过滤 (G_n) 定义的 G 上称为拓扑。 当我们使用关于过滤的群的拓扑概念时，我们的意思是，另外说明的除非，而拓扑由过滤定义。 注 G_n，即 G 的子群，既是开闭的（一般拓扑、章 III, § 2, no. 1，命题 4 的推论）。

由于每个G，在G上都是正规的，所以G上的左右均匀性重合；我们推断 G 承认 Hausdorff 完成群$\hat{G}$（一般拓扑、章III, § 3, no. 4、定理 1 和no. 1、命题 2）。

对于 G 的每个子集 M，G 中 M 的闭包等于

$$
\bigcap_{n \in \mathbf{Z}} (M . G_n) = \bigcap_{n \in \mathbf{Z}} (G_n . M)
$$

（一般拓扑、章III, § 3, no. 1、公式(1)）；特别是$\bigcap_{n \in \mathbf{Z}} G$，是$\{e\}$的闭包；因此可以看出，对于 G 上的拓扑来说，要成为 Hausdorff，过滤 (G_n) 被分离是必要且充分的。为了使G上的拓扑是离散的，存在$n \in \mathbf{Z}$使得$G_+ = \{e\}$是必要且充分的（在这种情况下$G_m = \{e\}$对于$m \geq n$）；那么过滤（G_n）称为离散的。

由于与 G 伴随的 Hausdorff 群为 $H = G / \left( \bigcap_{n \in \mathbf{Z}} G_n \right)$，因此可以规范地识别关联的分级群 gr(G) 和 gr(H)（如果对 H 进行商过滤）。

不让G'被另一个过滤群和$u : G \to G'$同态与过滤兼容； G 和 G' 上的拓扑定义立即表明$u$ 是连续的 (*)。如果 H 是 G 的子群（或正常子群），则 G 上的拓扑（或 G 上相对于 H 的商拓扑）在 H 上诱导的拓扑是 H 上的拓扑（或 G/H），由 G 上的商（或商拓扑）诱导的过滤定义G) 上的那个。 G 和 G' 上的乘积拓扑是由 G 和 G' 上的过滤乘积定义的拓扑。

令 v 为 G 上的阶函数 (no. 2)。G 上的假设意味着对于 G 中的所有 x、y 而言，$v(xy x^{-1}) = v(y)$ 以及$v(xy^{-1}) = v(yx^{-1}) = v(x^{-1}y) = v(y^{-1}x)$。令 $\rho$ 为实数，使得$0 < \rho < 1$（对于例取

(*) 在整个章中，我们将在一般拓扑、章III, § 2, no. 8中所谓的“连续表示”的意义上使用字“连续同态”； 字“同态”永远不会用于一般意义上的拓扑、章、III, § 2, no. 8、定义 1；对于这个概念，我们将始终在阶中使用项“严格态射”以避免任何混淆。

$\rho = 1/e$ 并令 $d(x, y) = \rho^{v(xy^{-1})}$ 对于 G 中的所有 $x, y$。然后 no. 2 的 $d(x, x) = 0, d(x, y) = d(y, x)$ 和不等式 (5') 给出

$$
(15) \quad d(x, y) \leq \sup(d(x, z), d(y, z))
$$

对于 G 中的所有 $x, y, z$，这意味着三角形不等式

$$
d(x, y) \leq d(x, z) + d(y, z).
$$

因此 $d$ 是 G 上的一个“伪计量”，它在左平移和右平移下保持不变，并且 G_n 是 $x \in G$ 的集合，使得 $d(e, x) < \rho^n$；由$d$定义的均匀结构则为拓扑群G上的均匀结构。如果G是Hausdorff，则G是*零维*可度量拓扑空间（*一般拓扑*，章 IX, § 6, no. 4);如果过滤 (G_n) 也是详尽的，则$d$ 是 G 上的*距离*。

给定一个拓扑环 A，回想一下，*左拓扑 A-模* 是 A-模 E，其中拓扑与其加法群结构兼容，并且从 $A \times E$ 到 E 的映射 $(a, x) \mapsto ax$ 是连续的（*一般拓扑*、章III, § 6, no. 6）。

#### 命题 3 {#ac-iii-s2-prop-3 .statement tag=04DT}

*设A是过滤后的环，(A_n)其过滤，A的B子环$\bigcup_{n \in \mathbf{Z}} A_n$，E是过滤后的B-模，(E_n)其过滤，F是E的子B模块$\bigcup_{n \in \mathbf{Z}} E_n$。然后映射$(a, x) \mapsto ax$ $B \times F$ 到 F 是连续的。*

令 $a, \in B, x_0 \in F$；存在假设整数$r, s$使得$a_0 \in A_r$和$x_0 \in E_s$。 关系

$$
ax - a_0x_0 = (a - a_0)x_0 + a_0(x - x_0) + (a - a_0)(x - x_0)
$$

表明如果 $a - a_0 \in A_i$ 和 $x - x_0 \in E_j$，则 $ax - a_0x_0$ 属于为

$$
E_{i+s} + E_{j+r} + E_{i+j}.
$$

然后，给定整数$n$，$ax - a_0x_0 \in E_n$提供$i \geq n - s, j \geq n - r$和$i + j \geq n$，即只要$i$和$j$是足够大。

#### 推论{#ac-iii-s2-n5-cor-1 .statement tag=04DU}

*环 B 是拓扑环，B-模 F 是拓扑B-模。*

第一个断言是由应用命题3到$F = B$得到的。

特别可以看出，过滤“穷举”的过滤环 A 是拓扑环；如果是这样的话，每个过滤“详尽”的过滤A-模都是拓扑A-模。

#### 命题 4 {#ac-iii-s2-prop-4 .statement tag=04DV}

*设 A 为交换环，通过穷举过滤 (A_n) 过滤，p 为 A 的理想。假设环 $\operatorname{gr}(A)$ 的理想 $\operatorname{gr}(p) = \bigoplus_{n \in \mathbf{Z}} (p \cap A_n)/(p \cap A_{n+1})$ 是素数。那么 A 中 p 的闭包是一个素理想。*

我们知道 gr(A/p) 与 gr(A)/gr(p) (no. 4, 命题 2) 同构的，因此整环；我们结论，$A / \bigcap_{n \in \mathbf{Z}} (p + A_n)$是整环（no. 3，命题1的推论）。那么$p$的闭包$\bigcap_{n \in \mathbf{Z}} (p + A_n)$就是素理想。

令$A$为环，且$m$为$A$的双面理想；通过 $m$-adic 过滤（no. 1、例 3）在 $A$ 上定义的拓扑称为 *m-adic 拓扑*；由于 *m*-adic 过滤是详尽的，$A$ 是一个拓扑环与此拓扑（命题 3 的推论）。类似地，对于每个$A$-模块$E$，由$m$-adic 过滤定义的拓扑称为$E$ 上的*m-adic 拓扑*； $E$是拓扑下的拓扑$A$模块。

令$m'$为$A$的另一个两侧理想；为了使$A$上的$m'$-adic 拓扑比$m$-adic 拓扑*更细*，存在整数$n > 0$使得${m'}^n \subset m$是充分必要的； 条件是必要的，如果满足，则${m'}^{hn} \subset m^h$ 对于所有$h > 0$，因此条件就足够了。如果$A$是*可交换的诺特环*，则相当于说$V(m) \subset V(m')$在$A$的素数谱中（章II, § 4, no. 3，推论2到命题11和§ 2, no. 6， 命题15)。

### 6. 完全过滤模

#### 命题 5 {#ac-iii-s2-prop-5 .statement tag=04DW}

*令$G$为过滤后的群，其过滤$(G_n)$由$G$的不变式子群组成。以下条件是等效的：*

(a) $G$ 是完全拓扑群。

(b) *伴随的 Hausdorff 群* $G' = G / (\bigcap_{n \in \mathbf{Z}} G_n)$ *已完成*。

(c) *$G$ 中的每个柯西序列都是收敛的*。

*如果 $G$ 是可交换的并且可加法书写，则这些条件也等价于以下内容：*

(d) *对于$L$的有限子集的补集的过滤器$\mathscr{F}$收敛到0的$G'$的元素的*每个族*$(x_\lambda)_{\lambda \in L}$*可在$G'$*中求和。

对于 $G$ 上的滤波器作为柯西滤波器（或收敛滤波器），其在典范映射 $G \to G'$ 下的像是柯西（或收敛）滤波器是必要且充分的（*一般拓扑*、章 II, § 3, no. 1， 命题 4); 从而首先是(a)和(b)的等价；另一方面，由于$G'$是可度量的，(b)和(c)的等价来自*一般拓扑*的命题9，章IX, § 2, no. 6。

现在假设 $G$ 是可交换的。假设$G'$是完备的，并令$(x_\lambda)_{\lambda \in L}$是$G'$的元素族，相对于$\mathscr{F}$收敛于0。对于$G$中0的每个邻域$V'$，即$G'$的子群，存在$L$的有限子集$J$，使得条件$\lambda \in L - J$蕴含$x_\lambda \in V'$；那么对于$L$的每一个有限子集$H$不满足$J$，$\sum_{\lambda \in H} x_\lambda \in V'$，这表明$(x_\lambda)_{\lambda \in L}$是可求和的（*一般拓扑*，章III, § 5, no. 2，定理1）。

相反，假设条件(d)成立，并令$(x_n)$是$G'$上的柯西序列；那么族 $(x_{n+1} - x_n)$ 是可求和的，特别是级数与一般项 $x_{n+1} - x_n$ 是收敛的，因此序列 $(x_n)$ 是收敛的。

令$G$为过滤后的群，其过滤$(G_r)$由$G$的正常子群组成； 商群 $G/G_n$ 是*离散*，因此是完整的，因为 $G_r$ 在 $G$ 中开放。令$f_n$为典范映射$G \to G/G_n$，对于$m \leq n$令$f_{mn}$为典范映射$G/G_n \to G/G_m$； $(G/G_n, f_{mn})$ 是离散群的逆系，其中 $\mathbf{Z}$ 作为索引集合（*常规拓扑*、章 III, § 7, no. 3）。令$\tilde{G}$为该逆系的拓扑群逆极限，并且对于所有$n$，令$g_n : \tilde{G} \to G/G_n$为典范映射；设$f : G \to \tilde{G}$为映射$(f_n)$的逆系逆极限，使得$f_n = g_n \circ f$对于所有$n$；最后，让$j$是$G$的典范映射到其豪斯多夫完成$\hat{G}$；当$G/G_n$完整时，存在一个独特的拓扑群同构$i : \hat{G} \to \tilde{G}$，使得$f = i \circ j$（*loc.cit.*，推论1到命题2）；我们将其称为$\hat{G}$到$\tilde{G}$的*规范*同构。

令$H$为另一个过滤群，其过滤$(H_r)$由$H$的正常子群组成，并令$u : G \to H$为同态与过滤（no. 4）相容的。 集合$\tilde{H} = \lim H/H_n$；对于所有$n$、$u$定义，通过对同态$u_n : G/G_n \to H/H_n$求商，而$u_n$显然是形式逆系与映射； 集合$\tilde{u} = \lim u_n$。此外，令$\hat{H}$为$H$和$ti : \hat{G} \to H$同态的豪斯多夫完成，由$u$通过经过导出到豪斯多夫完成（*一般拓扑*，章II, § 3, no. 7， 命题15)。紧随定义，如果$\hat{G}$通过典范同构与$\tilde{G}$识别，$\hat{H}$与$\tilde{H}$识别，则$ti$与$\tilde{u}$识别。我们结论特别指出，如果对于所有$n$，$u_n$是同构，那么$ti$是拓扑群的同构。

*完全过滤的群和环的例*

#### 例 1 {#ac-iii-s2-n6-exa-1 .statement tag=04DX}

令$G$为完全过滤后的群。带有诱导过滤的$G$的每个*关闭*子群均已完成（*常规拓扑*、章II, § 3, no. 4、命题8）。 $G$的每一个商群加上商过滤就完成了（*通用拓扑*、章IX, § 3, no. 1、*注* 1）。

#### 例 2 {#ac-iii-s2-n6-exa-2 .statement tag=04DY}

令$A$为过滤后的交换环，其过滤我们用$(a_n)_{n \in \mathbf{Z}}$表示；设$A'$为正式幂级数$A[[X_1, \ldots, X_s]]$的环。对于所有$e = (e_1, \ldots, e_s) \in \mathbf{N}^s$，我们写成$|e| = \sum_{i=1}^s e_i$，$X^e = \prod_{i=1}^s X_i^{e_i}$，这样每个元素$P \in A'$都可以唯一地写成$P = \sum_{e \in \mathbf{N}^s} \alpha_{e,P} X^e$，其中$\alpha_{e,P} \in A$。对于所有$n \in \mathbf{Z}$，令$a'_n$表示$P \in A'$的集合，使得$\alpha_{e,P} \in a_{n-|e|}$对于所有$e \in \mathbf{N}^s$；我们证明$a'_n$是$A'$的*理想*。显然$a'_n$是$A'$的加法子群；另一方面，如果$P \in a'_n$和$Q \in A'$，那么对于所有$e \in \mathbf{N}^s$，$\alpha_{e,PQ} = \sum_{e'+e''=e} \alpha_{e',Q}\alpha_{e'',P}$；因为关系$e' + e'' = e$意味着$|e''| \leq |e|$，$PQ \in a'_n$。此外，如果$Q \in a'_m$，那么，对于$e' + e'' = e$，$\alpha_{e',Q}\alpha_{e'',P} \in a_{m-|e'|}a_{n-|e''|} \subset a_{m+n-|e|}$，这证明$(a'_n)_{n \in \mathbf{Z}}$是与$A'$上的环结构兼容的“过滤”（显然对于$1 \in a'_0$）。当将来我们将 $A'$ 称为过滤后的环时，我们的意思是，除非另有说明，经过过滤（啊）。显然，$\bigcap_{n \in \mathbf{Z}} a'_n$ 是形式幂级数的集合，其所有系数为属于至 $\bigcap_{n \in \mathbf{Z}} a_n$；那么，如果$A$是Hausdorff，那么$A'$也是Hausdorff。如果$a_0 = A$，则$a'_0 = A'$。

#### 命题 6 {#ac-iii-s2-prop-6 .statement tag=04DZ}

*对于上面的记号，假设$a_0 = A$，并让$h$表示映射$P \mapsto (\alpha_{e,P})_{e \in \mathbf{N}^s}$。那么$h$就是加法拓扑群$A$到加法拓扑群$A^{\mathbf{N}^s}$的同构。 多项式环 $A[X_1, \ldots, X_s]$ 密集于 $A'$；如果 $A$ 完整，则 $A'$ 也完整。*

显然 $h$ 是双射的； $V_n = h(a'_n)$是$(a_e) \in A^{\mathbf{N}^s}$的集合，使得$a_e \in a_{n-|e|}$对于所有$e \in \mathbf{N}^s$使得$|e| \leq n$；由于元素$e$在数中是有限的，$V_n$在$A^{\mathbf{N}^s}$中是0的邻域。相反，如果$V$是$A^{\mathbf{N}^s}$中0的邻域，则存在$\mathbf{N}^s$和整数$v$的有限子集$E$，使得所有$e \in E$都有条件$a_e \in a_v$暗示$(a_e) \in V$；如果对于$e \in E$，$n$是整数$v + |e|$的最大的，则$h(a'_n) \subset V$，这就证明了命题6的第一个断言。

此外，根据上面定义的$n$和$E$，$h(P - \sum_{e \in E} \alpha_{e,P}X^e) \in V$对于所有$P \in A'$，这表明$A[X_1, \ldots, X_s]$在$A'$中是稠密的。 最后一个断言从第一个开始，并且完整的空间的乘积是完整的。

令$m$为$A$的理想，并假设$(a_i)$为$m$-adic过滤；那么，如果$n$是由$m$和$X_i$（$1 \leq i \leq s$）生成的$A'$的理想，则过滤$(a_i)$是$n$-adic过滤。显然，对于所有$k \geq 0$，$n^k$由元素$aX^e$生成，使得$a \in m^{k-|e|}$对于所有$e \in \mathbf{N}^s$，使得$|e| \leq k$，从而$n^k \subset a \&$。让我们反过来证明$a'_k \subset n^k$。对于所有 $P \in a'_k$、$P = P' + P''$，其中 $P' = \sum_{|e| < k} \alpha_{e,P}X^e$、$P'' = \sum_{|e| \geq k} \alpha_{e,P}X^e$。显然可以写成$P'' = \sum_{|e|=k} X^e Q_e$，其中$Q_e$分别是$A'$、从而、$P'' \in n^k$的元素；另一方面，显然 $\alpha_{e,P}X^e \in n^k$ 对于所有 $e \in \mathbf{N}^s$，从而 $P' \in n^k$。然后$n^k = a'_k$。

#### 推论 {#ac-iii-s2-n6-cor-1 .statement tag=04E0}

*令$A$为交换环，

$$
A' = A[[X_1, \ldots, X_s]]
$$

*$s$中形式幂级数的环在$A$和$n$上不确定，形式幂级数的理想$A'$由……组成没有常数项。 环 $A'$ 是 Hausdorff 且完整*，其中 n 进数拓扑和多项式环 $A[X_1, \ldots, X_s]$ 在 $A'$ 中处处稠密。

将刚刚所说的内容应用到案例$m = \{0\}$就足够了。

### 7.完全滤波模的线性紧致性

回想一下，如果 E 是 A-模，E 的仿射子集（或仿射线性簇）是任何空的子集 F 或形式 $a + M$，其中 $a \in E$ 且 M 是 E 的子模，称为 F 的方向（代数， 章II, § 9，第 1 和第 3）。

#### 命题 7 {#ac-iii-s2-prop-7 .statement tag=04E1}

设A为过滤后的环，E为过滤后的A-模，E为过滤后的$(E_n)$；假设$E_0 = E$，$E_n$是E的子模，A-模$E/E_n$是阿廷的，最后拓扑群E是Hausdorff且完备的。则E的非空闭仿射子集递减序列交非空。

我们在no. 6中看到，由于E是豪斯多夫且完备的，所以它与$\tilde{E} = \lim_{\leftarrow} E/E_n$一致。令$(W_p)$为E的非空闭仿射子集的递减序列，并且对于所有$n \geq 0$，令$W_{p,n}$为$E/E_n$中$W_p$的典范像；我们将构造序列 $x = (x_n) \in \tilde{E}$ 使得 $x_n \in W_{p,n}$ 对于所有 $p$ 和所有 $n$；因此$x \in W_p + E_n$对于所有$p$和所有$n$，并且由于$W_p$是封闭的，$x \in W_p$对于所有$p$（no. 5），这将证明命题。

作为$E/E_0 = 0$，我们取$x_0 = 0$。假设为$0 \leq i \leq n - 1$定义了$x_i$，令$W'_{p,n}$为$W_{p,n}$的元素的集合，其中$E/E_{n-1}$中的典范像为$x_{n-1}$；由于$x_{n-1} \in W_{p,n-1}$和$W_{p,n-1}$是$W_{p,n}$的典范像，$W'_{p,n}$非空，显然是$E/E_n$的仿射子集；而且序列$(W'_{p,n})_{p \in \mathbf{N}}$是递减。由于$E/E_n$是阿廷的，所以这个序列是静止的（否则$E/E_n$的子模的序列（即$W'_{p,n}$的方向）将是严格递减，这是荒谬的）。那么将$x_n$取为$\bigcap_{p \in \mathbf{N}} W'_{p,n}$的元素就足够了，然后可以通过归纳来执行$(x_n)$的构造。

#### 命题 8 {#ac-iii-s2-prop-8 .statement tag=04E2}

假设 A 和 E 满足命题 7 的假设。令 $(F_p)$ 为 E 的闭子模的递减序列，使得 $\bigcap F_p = 0$。那么，对于E中0的每个邻域V，存在$p$使得$F_p \subset V$（在其他字中，滤波器$(F_p)$的基收敛于0）。

我们可以假设V是$E_n$之一，在这种情况下$E/V$是阿廷的。让我们写$F'_p = (F_p + V)/V$；作为$E/V$的子模的$F'_p$形式递减序列，存在整数$j$使得对于所有$p > j$有$F'_p = F'_j$。我们将看到$F'_j = \{0\}$，它将完成证明。设$x \in F'_j$并设W，为F的元素集合，其$E/V$中的像为$x$($p \geq j$)；通过j（W）的定义，是E的非空闭仿射子集，显然$W_{p+1} \subset W$；

那么从命题 7 出发，对于所有 W, 都存在元素 y 属于。作为W，$\subset F,$和$\bigcap_{p \in \mathbf{N}} F_p = \{0\}, y = 0$；因为 x 是 E/V 中 y 的典范像，$x = 0$（cf.习题 15 到 21）。

### 8. 相关分级模中的同态提升

#### 定理 1 {#ac-iii-s2-thm-1 .statement tag=04E3}

令X，Y为两个过滤的群，其过滤$(X_n), (Y_n)$由正常的子群组成；令 $u : X \to Y$ 为同态与过滤兼容。

(i) 假设过滤$(X_n)$ 是彻底的。为了使$\mathrm{gr}(u)$是单射的，$\bar{u}^{-1}(Y_n) = X_n$对于所有$n \in \mathbf{Z}$是必要且充分的。

(ii) 假设以下假设之一成立： (α) X 完备且 Y Hausdorff； (β) Y 是离散的。那么，要使 $\mathrm{gr}(u)$ 成为满射，$Y_n = u(X_n)$ 对于所有 $n \in \mathbf{Z}$ 是充分必要的。

(i) 说映射 $\mathrm{gr}_n(u)$ 是单射意味着
$$
X_n \cap \bar{u}^{-1}(Y_{n+1}) \subset X_{n+1}.
$$
如果$(Y_{n+1}) = X_{n+1}$，显然就是这种情况。相反，如果
$$
X_n \cap \bar{u}^{-1}(Y_{n+1}) \subset X_{n+1}
$$
对于所有$n$，我们通过归纳在$k$上推断出$X_{n-k} \cap \bar{u}^{-1}(Y_{n+1}) \subset X_{n+1}$对于所有$n \in \mathbf{Z}$和所有$k \geq 0$。由于过滤$(X_n)$是详尽的，我们看到，对于所有$n$，$X_n$是$X_{n-k}$（$k \geq 0$）的并，因此对于所有$n$来说$\bar{u}^{-1}(Y_{n+1}) \subset X_{n+1}$，因此$X_{n+1} \subset \bar{u}^{-1}(Y_{n+1})$，完成证明。

(ii) 说映射 $\mathrm{gr}_n(u)$ 是满射意味着
$$
Y_n = u(X_n)Y_{n+1}.
$$
如果 $Y_n = u(X_n)Y_{n+1}$ 对于所有$n \in \mathbf{Z}$，显然就是这种情况。设$n$为整数且$y$元素为$Y_n$；我们将对 $X_n$ 的定义序列 $(x_k)_{k \geq 0}$ 进行元素的$x_k \in X_n$、$x_{k+1} \equiv x_k \pmod{X_{n+k}}$ 和 $u(x_k) \equiv y \pmod{Y_{n+k}}$ 对于所有$k \geq 0$。我们取$x_0$等于X的单位元素，这肯定会给出$u(x_0) \equiv y \pmod{Y_n}$。假设已构造 $x_k \in X_n$ 使得 $u(x_k) \equiv y \pmod{Y_{n+k}}$；然后$(u(x_k))^{-1}y \in Y_{n+k}$； 假设意味着存在$t \in X_{n+k}$使得$u(t) \equiv (u(x_k))^{-1}y \pmod{Y_{n+k+1}}$因此存在$u(x_k t) \equiv y \pmod{Y_{n+k+1}}$；执行归纳需要$x_{k+1} = x_k t$就足够了。因此，如果 Y 是离散的，则存在 $k \geq 0$ 使得 $Y_{n+k} = \{e'\}$（Y 的单位元素）、从而 $u(x_k) = y$，因此在这种情况下，已经证明对于所有 $n$ 都有$u(X_n) = Y$。现在假设 X 是完备的且 Y Hausdorff。由于$x_h^{-1} x_k \in X_{n+k}$对于$h \geq k \geq 0$来说，$(x_k)$是$X_n$中的柯西序列；作为

X_n 在 X 中闭合，因此是完备的，这个序列在 X_n 中至少有一个极限 x。由于u的连续性，u(x)是Y中序列(u(x_k))唯一的极限，Y为Hausdorff。但关系 u(x_k) \equiv y (\text{mod. } Y_{n+k+1}) 表明y 也是这个序列、从而 $u(x) = y$ 的极限并且还证明了$u(X_n) = Y_n$。

#### 推论 1 {#ac-iii-s2-thm-1-cor-1 .statement tag=04E4}

*假设 X 是 Hausdorff 并且其过滤是详尽的。那么，如果 gr(u) 是单射的，则 u 是单射的。*

令 e、e' 分别为 X 和 Y 的单位元素。然后
$$
\bar{u}^{-1}(e') \subset \bigcap_n \bar{u}^{-1}(Y_n) = \bigcap_n X_n = \{e\}
$$
由假设，从而推论。

#### 推论 2 {#ac-iii-s2-thm-1-cor-2 .statement tag=04E5}

*假设以下假设之一成立：*
$(\alpha)$ *X 完整，Y 为 Hausdorff，其过滤是详尽的；*
$(\beta)$ *Y 是离散的，其过滤是详尽的。*
*那么，如果 gr(u) 是满射，则 u 是满射。*

在这种情况下$Y = \bigcup_n Y_n = \bigcup_n u(X_n) \subset u(X)$。

#### 推论 3 {#ac-iii-s2-thm-1-cor-3 .statement tag=04E6}

*假设X和Y是Hausdorff，X和Y的过滤是穷举的，X是完整的。那么，如果 gr(u) 是双射的，则 u 也是双射的。*

设A为局部环，m为最大理想，M为A-模；令 A 和 M 被赋予 *m-adic* 过滤，并令 gr(A) 和 gr(M) 为分级环以及与 A 和 M 相关的分级 gr(A) 模块。我们已经看到 (no. 3, 例 3) 典范映射 (11) 始终是*满射*；我们将考虑 M 的以下性质：
*（GR）* *典范映射*
$$
\gamma_M : \operatorname{gr}(A) \otimes_{\operatorname{gr}_0(A)} \operatorname{gr}_0(M) \to \operatorname{gr}(M)
$$
*是双射的*。

#### 命题 9 {#ac-iii-s2-prop-9 .statement tag=04E7}

*设 A 为局部环，m 为其最大理想值，M、N 为两个 A-模，u : N \to M 为 A 同态。 M 和 N 被赋予 m-adic 过滤并假设： (1) M 满足性质 (GR)； (2) \operatorname{gr}_0(u) : \operatorname{gr}_0(N) \to \operatorname{gr}_0(M) 是单射的。那么 \operatorname{gr}(u) : \operatorname{gr}(N) \to \operatorname{gr}(M) 是单射的，N 和 P = \operatorname{Coker}(u) 满足性质 (GR) 和 $m^n N = \bar{u}^{-1}(m^n M)$ 对于每个整数 $n > 0$。*

立即验证图表
$$
\begin{array}{ccc}
\operatorname{gr}(A) \otimes_{\operatorname{gr}_0(A)} \operatorname{gr}_0(N) & \xrightarrow{1 \otimes \operatorname{gr}_0(u)} & \operatorname{gr}(A) \otimes_{\operatorname{gr}_0(A)} \operatorname{gr}_0(M) \\
\downarrow \gamma_N & & \downarrow \gamma_M \\
\operatorname{gr}(N) & \xrightarrow{\operatorname{gr}(u)} & \operatorname{gr}(M)
\end{array}
$$

是可交换的。由于$\mathrm{gr}_0(A) = A/m$是域，假设意味着$1 \otimes \mathrm{gr}_0(u)$是单射的；因为假设 $\gamma_M$ 是单射的，$\gamma_M \circ (1 \otimes \mathrm{gr}_0(u))$ 也是单射的。这首先意味着$\gamma_N$是单射的，因此是双射的，因此$\mathrm{gr}(u)$是单射的。 公式$\tilde{u}^1(m^nM) = m^nN$则为定理1(i)中的推论。

另外，让我们写 $N' = u(N)$ 并让 $j : N' \to M$ 为典范嵌入。如果$p : M \to P = M/N'$是典范同态，那么在交换律中图表

$$
\begin{array}{ccccccccc}
\mathrm{gr}(A) \otimes \mathrm{gr}_0(N') & \xrightarrow{1 \otimes \mathrm{gr}_0(j)} & \mathrm{gr}(A) \otimes \mathrm{gr}_0(M) & \xrightarrow{1 \otimes \mathrm{gr}_0(p)} & \mathrm{gr}(A) \otimes \mathrm{gr}_0(P) & \to & 0 \\
\downarrow \gamma_{N'} & & \downarrow \gamma_M & & \downarrow \gamma_P & & \\
\mathrm{gr}(N') & \xrightarrow{\mathrm{gr}(j)} & \mathrm{gr}(M) & \xrightarrow{\mathrm{gr}(p)} & \mathrm{gr}(P) & \to & 0
\end{array}
$$

下排是精确的（no. 4，命题 2），上排也是如此，因为no. 4的命题 2以及$\mathrm{gr}_0(A)$是域。此外，$\mathrm{gr}(j)$是单射的（no. 4，命题2），因此$\mathrm{gr}_0(j)$是单射的，应用于$j$的参数的第一个部分表明$\gamma_{N'}$是双射的；由于$\gamma_M$也是假设的双射，我们结论认为$\gamma_P$是双射的（章I, § 1, no. 4，推论2到命题2）。

#### 推论{#ac-iii-s2-n8-cor-1 .statement tag=04E8}

在命题 9 的假设下，如果我们还假设$N$ 是具有$m$-adic 过滤的Hausdorf，则$u$ 是单射的。

这是因为 $\mathrm{gr}(u)$ 是单射的（推论 1 到定理 1）。

\* 注。假设命题 9 的假设成立，并且以下条件之一也成立：
(1) $m$ 幂零的；
(2) $A$ 是诺特，$P$ 理想的是 Hausdorff (cf. § 5, no. 1)；
那么 $P$ 是一个扁平的 $A$ 模块。这是因为$\gamma_P$是双射且§ 5, no. 2、定理 1 (iv)，因为$A/m$是域。 \*

### 9. 相关分级模元素的家庭提升

令$A$为过滤后的交换环，$(A_n)_{n \in \mathbf{Z}}$为其过滤，$C$子环为$A$，这样$C \cap A_1 = \{0\}$。 典范映射 $A_0 \to A_0/A_1 = \mathrm{gr}_0(A)$ 的限制到 $C$ 是单射的，这使得我们可以用 $\mathrm{gr}_0(A)$ 的子模进行认同 $C$；这是我们在类似情况下通常会做的。 如果 $A_1 \neq A$ 和 $K$ 是 $A$ 中的任意子域，则 $K \cap A_1 = (0)$ 因为 $K \cap A_1$ 是 $K$ 而不是包含 1 的理想；那么$K$可以用$\mathrm{gr}_0(A)$的子域来识别。

#### 命题 10 {#ac-iii-s2-prop-10 .statement tag=04E9}

设$A$为过滤后的交换环，$(A_n)$为过滤后的交换环；假设存在$A_0$的子环$C$，使得$C \cap A_n = \{0\}$和$C$可以与$\mathrm{gr}_0(A)$的子环识别。设$(x_i)_{1 \leq i \leq q}$是$A$的元素的有限族；假设$x_i \in A_n$对于$1 \leq i \leq q$，并让$\xi_i$是对于$1 \leq i \leq q$的$\mathrm{gr}_{n_i}(A)$中$x_i$的类。

(i) 如果$\mathrm{gr}(A)$的元素的族$(\xi_i)$在$C$上是代数自由的，则族$(x_i)$在$C$上是代数自由的。

(ii) 如果$A$上的过滤是详尽且离散的，并且$(\xi_i)$是$C$-代数$\mathrm{gr}(A)$的生成元的系统，则$(x_i)$是$C$-代数的生成元的系统 $A$。

令$A'$为代数$\mathbf{C}[X_1, \ldots, X_q]$除以$\mathbf{C}$的多项式；让$A'$得到型$\mathbf{Z}$的分级$(A'_n)$，其中$A_n$是$\mathbf{C}$的集合-单项式$X_1^{s(1)} \ldots X_q^{s(q)}$的线性组合，使得$\sum_{i=1}^q n_i s(i) = n$。设$u$为同态$f \mapsto f(x_1, \ldots, x_q)$，从$\mathbf{C}$-代数$A'$到$\mathbf{C}$-代数$A$；通过定义，$u(A'_n) \subset A_n$对于所有$n \in \mathbf{Z}$，因此$u$与过滤$(A')$相容的，其过滤后的环结构与其分级环结构，cf.no. 1，例1)。既然如此，(i) 的假设意味着

$$
\mathrm{gr}(u): A' = \mathrm{gr}(A') \to \mathrm{gr}(A)
$$

是单射的；由于$A'$上的过滤是穷举且分离的，因此可以应用no. 8的推论1至定理1，并且$u$是单射的，这证明了(i)的结论。类似地，(\&) 上的假设 (ii) 意味着 $\mathrm{gr}(u)$ 是满射；由于$A$是离散的，其过滤是穷举的，因此可以应用no. 8的推论2至定理1，并且$u$是满射的，这证明了(ii)的结论。

#### 命题 11 {#ac-iii-s2-prop-11 .statement tag=04EA}

令 $A$ 为 $A_0$ 的完整豪斯多夫过滤交换环、$C$ 子环，使得 $C \cap A_n = 0$ 和 $(x_i)_{1 \leq i \leq q}$ 为 $A$ 的元素的有限族，使得 $x_i \in A_{n_i}$ 其中$n_i > 0$ 为 $1 \leq i \leq q$；对于$1 \leq i \leq q$，令$\xi_i$为$\mathrm{gr}_{n_i}(A)$中$x_i$的类。

(i) 从形式幂级数$A'' = \mathbf{C}[[X_1, \ldots, X_q]]$到$A$，从代数存在唯一的$C$同态$v$，使得$v(X_i) = x_i$对应于$1 \leq i \leq q$。

(ii) 如果族 $(\xi_i)$ 在 $C$ 上是代数自由的，则同态 $v$ 是单射的。

(iii) 如果对 $A$ 的过滤是穷举的，并且$(\xi_i)$族是$C$代数$\mathrm{gr}(A)$的生成元的系统，则同态$v$是满射的。

对于所有$i$，$n_i \geq 1$，对于每个单项式$X_1^{s(1)} \ldots X_q^{s(q)}$，$\sum_{i=1}^q n_i s(i) \geq \sum_{i=1}^q s(i)$，另一方面，如果$r$是$n_i$的最大的，则$\sum_{i=1}^q n_i s(i) \leq r \cdot \sum_{i=1}^q s(i)$。如果$A''_n$表示形式幂级数的集合，其非零项$a_s X_1^{s(1)} \ldots X_q^{s(q)}$满足$\sum_{i=1}^q n_i s(i) \geq n$，则从no. 6推论命题6 $A''$ 是 Hausdorff，并配有彻底的过滤 $(A''_n)$ 并且

$$
A' = \mathbf{C}[X_1, \ldots, X_q]
$$

$A''$ 是稠密的；此外，命题 10 的证明中定义的同态$u$在$A'$上是连续的，并且可以唯一地扩展到连续的同态$v : A \to A$，因为$A$是Hausdorff且完备的（通则拓扑， 章 III, § 3, no. 3, 命题 5)，证明(i)；还有，$\mathrm{gr}(A'') = \mathrm{gr}(A')$和$\mathrm{gr}(v) = \mathrm{gr}(u)$；鉴于$A$的假设，(ii)和(iii)分别由推论1和2得出no. 8的定理1。

命题 (ii) (或 (iii)) 的结论是有时，由说表达，家庭$(x_i)$在$C$上正式自由（或$A$的生成元的正式系统）。

#### 命题 12 {#ac-iii-s2-prop-12 .statement tag=04EB}

令$A$为过滤后的环，$E$为过滤后的$A$模块，$(A_n)$和$(E_n)$分别对$A$和$E$进行过滤。假设$A$已完成，且过滤$(E_n)$已彻底分离。令$(x_i)_{i \in I}$为$E$的元素的有限族，对于$i \in I$，令$n(i)$为整数，使得$x_i \in E_{n(i)}$；最后令$\xi_i$为$\mathrm{gr}_{n(i)}(E)$中$x_i$的类。那么，如果$(\xi_i)$是$\mathrm{gr}(A)$-模块$\mathrm{gr}(E)$的生成元的系统，则$(x_i)$是$A$-模块$E$的生成元的系统。

在$A$-模块$L = A'$中，令$L_0$表示集合$(a_i)$，使得$a_i \in A_{n - n(i)}$对于所有$i \in I$；如果$p$和$q$是$n(i)$中最小的且最大的，则定义$(L_n)$在$L$上定义的$A^I_{n-q} \supset L_0 \supset A^I_{n-p}$和拓扑与乘积拓扑相同；因此 $L$ 是一个完整的过滤 $A$ 模块。由于$L$是自由的，因此存在$A$-线性映射$u : L \to E$使得$u((a_i)) = \sum_{i \in I} a_i x_i$并且它显然与过滤兼容；我们必须证明 $u$ 是满射的，为此，根据推论 2 到定理 1、no. 8 就足以证明

$$
\mathrm{gr}(u) : \mathrm{gr}(L) \to \mathrm{gr}(E)
$$

是满射的，或者对于所有$x \in E_n$，存在一个族$(a_i)$，使得$a_i \in A_{n-n(i)}$对于所有$i \in I$和$x \equiv \sum_{i \in I} a_i x_i \pmod{E_{n+1}}$。令$\xi$为$\mathrm{gr}_n(E)$中$x$的类；由于$\xi_i$生成$\mathrm{gr}(A)$-模块$\mathrm{gr}(E)$，存在$\alpha_i \in \mathrm{gr}(A)$使得$\xi = \sum_{i \in I} \alpha_i \xi_i$，如果需要的话我们可以假设$\alpha_i \in \mathrm{gr}_{n-n(i)}(A)$乘以替换是$\alpha_i$乘以次数的同质分量$n - n(i)$。那么$\alpha_i$是元素$a_i \in A_{n-n(i)}$中的像，而家庭$(a_i)$有所需的性质。

#### 推论 1 {#ac-iii-s2-prop-12-cor-1 .statement tag=04EC}

令$A$是一个完整的过滤环，而$E$是一个过滤的$A$模块，其过滤是彻底且分离的。如果 $\mathrm{gr}(E)$ 是有限生成的（分别为诺特）$\mathrm{gr}(A)$ 模块，则 $E$ 是有限生成的（分别为诺特）$A$ 模块。

如果 $\mathrm{gr}(E)$ 是有限生成的，则存在齐次生成元的有限系统，并且命题 12 表明 $E$ 是有限生成的。现在假设$\mathrm{gr}(E)$是诺特，并令$F$是$E$的子模；由$E$在$F$上引起的过滤是详尽且分离的，并且$\mathrm{gr}(F)$被识别为gr(E)的子gr(A)模块(no. 4，命题2)，因此由假设有限生成；我们结论F是有限生成A-模，因此E是诺特。

#### 推论 2 {#ac-iii-s2-prop-12-cor-2 .statement tag=04ED}

设 A 是一个完整的豪斯多夫过滤环，其过滤是详尽的。如果 gr(A) 是左诺特环，则 A 也是。

应用推论 1 且 E = A 就足够了。

#### 推论 3 {#ac-iii-s2-prop-12-cor-3 .statement tag=04EE}

设 A 为完全过滤的环，(A_n) 为它的过滤，E 为 Hausdorff 过滤的 A-模，(E_n) 为它的过滤，F 为 E 的有限生成的子模；假设 A_∞ = A 且 E_0 = E。

(i) 如果对于所有 k ≥ 0，E_k = E_{k+1} + A_k F，则 F = E。
(ii) 如果进一步假设 E 上的过滤源自 A 上的过滤 (no. 1, 例 2)，关系 E = E_1 + F 意味着 F = E。

令 xi_i (1 ≤ i ≤ n) 为类 mod。 F 的生成元的有限系统的 E_1。根据给定的假设，对于所有 k ≥ 0，gr_k(E) 的每个元素都可以用形式 $\sum_{i=1}^n \alpha_i \xi_i$ 表示，其中 $\alpha_i \in \mathrm{gr}(A)$; $\xi_i$ 因此生成 gr(A)-模 gr(E)，它凭借命题 12 证明了 (i)。如果 E 上的过滤源自 A 上的过滤，则关系 E = E_1 + F 意味着

$$
E_k = A_k E = A_k E_1 + A_k F = A_k A_1 E + A_k F \subset A_{k+1} E + A_k F \\
= E_{k+1} + A_k F \subset E_k,
$$

从而（二）。

#### 命题 13 {#ac-iii-s2-prop-13 .statement tag=04EF}

设A为环，m是A的双面理想，包含在A和E的雅各布森根中A-模。让 A 和 E 接受 m 进过滤 (no. 1, 例 3)。假设以下条件之一成立：
(a) E 为有限生成A-模，A 为豪斯多夫；
(b) m 是幂零的。

对于 E 为自由A-模，E/mE 是自由 (A/m) 模且 E 满足性质 (GR) (no. 8) 是必要且充分的。

如果E是E的自由A-模和$(e_\lambda)$基，则对于所有$k > 0$（代数，章II, § 3, no. 7，$m^k E$是E的子模$m^k e_\lambda$中的直和， 注);则 $m^k E / m^{k+1} E$ 与 $m^k e_\lambda / m^{k+1} e_\lambda$ 的直和进行识别（代数、章 11、§ 1, no. 6、命题 7）。我们首先（对于$k = 0$）推导出（A/m）模块$E / mE$的$E / mE = (A / m) \otimes_A E$形式基中$e_\lambda$的类$1 \otimes e_\lambda$，因为典范映射

$$
(m^k / m^{k+1}) \otimes_A (E / mE) \to m^k E / m^{k+1} E
$$

对于所有 $k \geq 0$ 都是双射的；因此 $\gamma_E$ 是双射的。 注证明的这个部分既不使用条件(a)也不使用条件(b)。

相反，假设叙述的条件成立，并令$(x_i)_{i \in I}$是E的元素族，其类模。 $(A/m)$模块$E/mE$的$mE$形式基；令L为自由A-模$A_s^{(I)}$，$(f_i)_{i \in I}$为典范基，$u : L \to E$A-线性映射，使得$u(f_i) = x_i$对于所有$i \in I$。假设已经暗示 $u$ 是满射（章 II, § 3, no. 2，推出 1 到命题 4），还需要证明 $u$ 是单射。现在，每个假设 (a) 和 (b) 都意味着 A 是 Hausdorff，因此使用 m-adic 过滤，L 也是 Hausdorff，因为 $m^kL = (m^k)^{(I)}$ (代数, 章 II, § 3, no. 7, 注) 和 $\operatorname{gr}(L)$ 被标识为从证明的第一个部分开始$\operatorname{gr}(A) \otimes_{A/m} (L/mL)$； 同态 $u$ 与过滤兼容，并且可以将 $\operatorname{gr}(u) = \gamma_E \circ v$ 写入其中 $v$ 是 $\operatorname{gr}(L)$ 的双射到
$$
\operatorname{gr}(A) \otimes_{A/m} (E/mE)
$$
映射类关闭，模组。 mM 到 $1 \otimes \bar{x}_i$，其中 $\bar{x}_i$ 是 $x_i$ mod 的类。 $mE$。那么假设意味着$\operatorname{gr}(u)$是单射的，并且借助推论1到定理1、no. 8得出结论。

### 10. 应用：例诺特环

#### 引理 1 {#ac-iii-s2-lem-1 .statement tag=04EG}

令A为型$\mathbf{Z}$的分级环，其分级$(A_n)$使得对于所有$n < 0$为$A_n = 0$或对于所有$n > 0$为$A_n = 0$。令 M 为型 $\mathbf{Z}$ 的分级 A-模。为了使M成为诺特A-模，M的每个分级子模是有限生成的充分必要。

由于$n \mapsto -n$是群$\mathbf{Z}$中的自同构，我们可能会将注意力限制在所有$n > 0$的案例$A_n = 0$上。令 A' 和 M' 分别表示环 A 和模 M，以及与它们各自的等级（no. 1，例 1）相关的过滤，它们是详尽且分离的； A 上的假设意味着 A' 是离散的，因此是完整的。如果E是M的子A-模，则对E进行诱导过滤得到的过滤后的A'-模E'是Hausdorff，其过滤是穷举的；此外，$\operatorname{gr}(E')$ 与 $M = \operatorname{gr}(M')$ 的分级子 A 模块相同，因此由假设有限生成。然后从no. 9的推论1到命题12得出结论。

#### 定理 2 {#ac-iii-s2-thm-2 .statement tag=04EH}

令A为型$\mathbf{N}$的分级环，M为型$\mathbf{N}$的A-模分级，以及$(A_n)$和$(M_n)$各自的分级。假设存在元素 $a \in A_0$，使得所有 $n > 0$ 都存在 $A_n = A_0 a^n$ 和 $M_n = a^n M_0$。那么，如果M是诺特$A_0$模，则M是诺特A-模。

凭借引理 1 足以证明 M 的每个分级子模 N 都是有限生成的。对于所有$r \geq 0$，令$N_r = N \cap M_r$且令L_r为$m \in M_0$的集合，使得$a^r m \in N_r$。作为
$$
a^r A_0 \subset A_r = A_0 a^r, \quad a^r A_0 L_r \subset A_0 a^r L_r \subset A_0 N_r \subset N_r
$$

因此 L, 是 M, 的子 A, 模块；此外，

$$
aN_r \subset N \cap aM_r = N \cap M_{r+1} = N_{r+1}
$$

因此序列$(L_r)_{r \geq 0}$是递增。 假设意味着存在整数$n \geq 0$使得$L_r = L_n$对应$r \geq n$。对于每个$r \leq n$，令$(m_{r,s})_{1 \leq s \leq k_r}$为A,-模$L_r$的生成元中的系统。我们将证明$1 \leq s \leq k_r$的元素$a^r m_{r,s}$，A-模N的生成元的$0 \leq r \leq n$形式系统。作为所有$r$的$M_r = a^r M_0$， $N_r = a^r L_r$ 为所有 $r$ 减定义共 $L_r$。那么，对于$r \leq n$，

$$
N_r = a^r L_r = \sum_{s=1}^{k_r} a^r A_0 m_{r,s} \subset \sum_{s=1}^{k_r} A_0 a^r m_{rs},
$$

并且，对于$r > n$，

$$
N_r = a^r L_n = \sum_{s=1}^{k_n} a^r A_0 m_{n,s} \subset \sum_{s=1}^{k_n} A_0 a^r m_{n,s} \subset \sum_{s=1}^{k_n} A_0 a^{r-n} \cdot (a^n m_{n,s})
$$

完成证明 (cf. 习题 10)。

#### 推出 1（希尔伯特定理）{#ac-iii-s2-thm-2-cor-1 .statement tag=04EI}

*对于每个交换律诺特环 C、多项式环 C[X] 都是诺特* (cf. 习题 10)。

#### 推出 2 {#ac-iii-s2-thm-2-cor-2 .statement tag=04EJ}

*对于每个交换律诺特环 C 和每个整数 $n > 0$、多项式环 C[X_1, ..., X_n] 都是诺特。*

这是从归纳在 $n$ 上得出的推论 1 得出的。

#### 推出 3 {#ac-iii-s2-thm-2-cor-3 .statement tag=04EK}

*如果 C 是交换律诺特环，则每个有限生成的交换律 C 代数都是诺特环。*

这样的代数同构于多项式代数 C[X_1, ..., X_n] (§ 1, no. 1) 的商。

#### 推出 4 {#ac-iii-s2-thm-2-cor-4 .statement tag=04EL}

*设 A 为型 $\mathbf{N}$ 的等级交换环，并令 $(A_n)$ 为其毕业。对于 A 为诺特，$A_n$ 为诺特且 A 为 ajinitely 生成的 A,-代数是充分必要的。*

根据推论3，条件是充分的。反之，假设A是诺特； $m = \sum_{n \geq 1} A_n$是A的理想，然后有限生成；那么 A 是有限生成的 A,-代数（§ 1, no. 2，命题 1 的推论）；另一方面，与$A/m$同构的$A_n$是诺特环。

#### 推出 5 {#ac-iii-s2-thm-2-cor-5 .statement tag=04EM}

*设 A 为交换环，m 是 A 的一个理想，使得 $A/m$ 为诺特，$m/m^2$ 是 ajinitely 生成的 $(A/m)$ 模，A 是 Hausdorff，并由 m 进数拓扑完成。那么 gr(A) 和 A 是诺特。*

gr(A) 是由 $m/m^2$ (no. 3, 例 3) 生成的 $(A/m)$ 模，因此根据推论 3，环 gr(A) 是诺特。 由此我们推断 A 本身是诺特 (no. 9,推出 2 至命题 12)。

#### 推出 6 {#ac-iii-s2-thm-2-cor-6 .statement tag=04EN}

对于每个可交换的诺特环 C 和每个整数 n > 0，形式幂级数 $\mathbf{C}[[X_1, \ldots, X_n]]$ 的环是诺特。

这是从推论 5 和 no. 6 得出的，推论到命题 6，因为如果 m 是形式幂级数的理想$A = \mathbf{C}[[X_1, \ldots, X_n]]$ 由……组成，且没有常数项，$A/m$ 同构于C 和 $m/m^2$ 到C-模块$\mathbf{C}"$。

注

(1) 如果 C 是交换域，则推论 2、3 和 6 特别适用。

\* (2) 设 g 在可交换的诺特环 C 上为李代数，并假设 g 是有限生成的 C 模。令 g 的包络代数 U 给出在 no. 3、例 4 中定义的递增过滤 $(U_n)$。 对于相应的拓扑，U 是离散的，因此是 Hausdorff 和完备的；关联的分级环 gr(U) 是有限生成的 C 代数，是对称代数 $\mathscr{S}(g)$ 的商，因此 gr(U) 是诺特环 （推出 3），我们推断出 U 是左且右诺特环（no. 9，推出 2 至命题 12）。 \*

### 11. 完整的 m-ADIC 环和逆极限

我们在no. 6中看到，如果A是交换环并且m是A的理想，使得A是Hausdorf并且与m进数拓扑完成，则拓扑环$A$规范地等同于离散环的逆极限 $A_i = A/m^{i+1} \ (i \in \mathbf{N})$ 相对于典范映射

$$
h_{ij}: A/m^{j+1} \to A/m^{i+1} \quad (i \leq j);
$$

注 $h_{ij}$ 是满射，如果 $n_{ij}$ 是它的核，那么

$$
n_{ij} = m^{i+1}/m^{j+1} = (m/m^{j+1})^{i+1} =
$$

特别是$(n_{0j})^{j+1} = 0$。反之：

#### 命题 14 {#ac-iii-s2-prop-14 .statement tag=04EO}

令$(A_i, h_{ij})$为离散交换环的逆系，其索引集合为$\mathbf{N}$，并令$(M_i, u_{ij})$为模的逆系超过环的逆系 $(A_i, h_{ij})$。让$n_j$表示$h_{0j}: A \to A$的核，并且集合$A = \lim A_i$，$M = \lim M_i$。假设

(a) 对于所有 $i \in \mathbf{N}$，$h_{ii}$ 是 A 上的恒等映射，并且对于 $i \leq j$，$h_{ij}$ 和 $u_{ij}$ 是满射；
(b) 对于$i \leq j$，$h_{ij}$和$u_{ij}$的核分别是$n_j^{i+1}$和$n_j^{i+1} M_j$。

然后：
(i) $A$ 是完全 Hausdorff 拓扑环、$M$ 是完全 Hausdorff 拓扑 A-模和典范映射 $h_i : A \to A_i$、$u_i : M \to M_i$ 是满射。
(ii) 如果$M_0$是有限生成的A,-模，则$M$是有限生成A-模；

准确地说，M 的每个有限子集 S 使得 $u_0(S)$ 生成 M，是 M 的生成元的系统。

(i)中的断言遵循一般拓扑、章II, § 3, no. 5、命题10的推论以及定理1的推论1。

对于所有$i \in \mathbf{N}$，让我们写成$m_{i+1} = \mathrm{Ker}(h_i), N_{i+1} = \mathrm{Ker}(u_i)$；那么

$$
m_{i+1} = \lim_{k \geq 0} h_{i,t+k}^{-1}(0) = \lim_{\leftarrow} n_{i+1}^{t+k}
$$

和$N_{i+1} = \lim_{\leftarrow} n_{i+k}^{t+1} M_{i+k}$；由于 $h_{i+k}$ 和 $u_{i+k}$ 是满射，

$$
h_{i+k}(m_{i+1}) = n_{i+k}^{t+1}, \quad u_{i+k}(N_{i+1}) = n_{i+k}^{t+1} M_{i+k}.
$$

让我们证明$m_i N_j \subset N_{i+j}$对应于$i \geq 1$和$j \geq 1$，相当于证明即$u_{i+j-1}(m_i N_j) = 0$；现在

$$
u_{i+j-1}(m_i N_j) = h_{i+j-1}(m_i) u_{i+j-1}(N_j)
$$

等于$n_{i+j-1}^{t'}(n_{i+j-1}^{t'} M_{i+j-1}) = 0$，因为对于所有$k \geq 0$，$n_k^{k+1}$（即$h_{kk}$的核）等于0。我们类似地看到$m_i m_j \subset m_{i+j}$。如果对于$i \leq 0$我们集合$m_i = A$和$N_i = M$，$(m_i)_{i \in \mathbf{Z}}$是A的过滤，$(N_i)_{i \in \mathbf{Z}}$是与A上的过滤兼容的M的过滤； A 和 M 上的拓扑显然是由这些过滤定义的。既然如此，令$a$为A的理想，使得S生成M的$h_1(a) = n_1$和$M'$子模；我们将证明这一点

$$
N_i = a^i M' + N_{i+1} \quad \text{for } i \geq 0.
$$

让我们写$a_i = h_i(a), M'_i = u_i(M')$；足以表明

$$
u_i(N_i) = a_i^i M'_i.
$$

如果 $i = 0$ 为 $N_0 = M$ 且 $M'_0 = M$ 为假设，则这是正确的。如果$i \geq 1$，则$u_i(N_i) = n_i^i M_i$乘以(16)。由于$h_{1i}$是满射，$h_{0i} = h_{01} \circ h_{1i}$、$h_i$的$h_{1i}$映射核$n_i$，到$h_1$的核$n_1$和$n_i = h_{1i}(n_1)$；那么

$$
h_{1i}(a_i) = h_1(a) = n_1 = h_{1i}(n_i)
$$

并且，由于$h_{1i}$的核是$n_i^2$、$n_i \subset a_i + n_i^2$和$a_i \subset n_i$，所以从而$n_i = a_i + n_i^2$。此外$u_{0i}(M'_i) = u_0(M') = M, = u_{0i}(M_i)$以及$\mathrm{Ker}(u_{0i}) = n_i M_i$、$M_i = M'_i + n_i M_i$； 从而

$$
n_i^i M_i = (a_i + n_i^2)^i (M'_i + n_i M_i).
$$

现在，$a_i^k n_i^{i+1-k} \subset n_i^{i+1} = 0$代表$0 \leq k \leq i$；那么它肯定遵循$u_i(N_i) = n_i M_i = a_i^i M'_i$，从而证明了（17）。

此外$m_1 = h_1(n_1)$，从而$a \subset m_1$，因此$a^i \subset m_1^i \subset m_i$，从而

$N_i \subset m_i M' + N_{i+1}$；另一方面，显然$m_i M \subset N_i$，因此对于所有$i \geq 0$，$N_i = m_i M' + N_{i+1}$；那么从推论3到no. 9的命题12即$M' = M$，从而完成证明。

#### 推论 1 {#ac-iii-s2-prop-14-cor-1 .statement tag=04EP}

*使用记号和命题14的假设，进一步假设$M_0$是有限生成的$A$模块，并且$A$的理想$n_1$是有限生成的。设$m_1$为$h_1$的核； $A$和$M$上的拓扑分别是环和模上的$m_1$-adic拓扑；准确地说，对于$h_i$和$u_i$的所有$i \geq 0$、核分别是$m_1^{i+1}$和$m_1^{i+1} M$；进一步 $m_1 / m_1^2$ 是有限生成的 $A$ 模块。*

我们保留命题 14 证明记号；这里的假设允许我们假设理想的 $a$ 是有限生成的。令$i \geq 0$为任意整数；对于所有 $j \geq 0$，通过 (17)，$N_{i+j} = a^j(a^i M) + N_{i+j+1} \subset m_j(a^i M) + N_{i+j+1}$；反之，$m_j(a^i M) \subset m_j m_i M \subset m_{i+j} M \subset N_{i+j}$、从而

$$
N_{i+j} = m_j(a^i M) + N_{i+j+1}.
$$

由于 $a$ 和 $M$ 是有限生成的 $A$ 模，$a^i M$ 也是如此。 应用 no. 9到模$N_i$的推论3到命题12，通过$N_{ij} = N_i$定义的过滤$(N_{ij})_{j \in \mathbf{Z}}$，如果$j < 0$，$N_{ij} = N_{i+j}$如果$j \geq 0$，我们得到$N_i = a^i M$， 从而$N_i \subset m_1^i M$。还有$m_1^i M \subset m_i M \subset N_i$、从而$N_i = m_1^i M$。 应用对于$M = A$、$u_{ij} = h_{ij}$的情况，我们得到$m_i = m_1^i$。此外，由(17)得到$m_1 = a + m_1^2$，从而证明了推论的最后一个断言。

#### 推论 2 {#ac-iii-s2-prop-14-cor-2 .statement tag=04EQ}

*在推论1的假设下，$A$为诺特，$A$为诺特是充分必要的。*

条件是必要的，因为 $A$ 同构于 $A$ 的商；根据 no. 10、推出 5 到定理 2 就足够了。

### 12. 过滤后的模的 HAUSDOFF 完成

令$G$为过滤后的群，其过滤$(G_n)$由$G$的正常子群组成；我们已经回忆过（no. 6），拓扑群$G$的*豪斯多夫完成*$\hat{G}$被规范地等同于*离散*群$G/G_n$、典范同态的逆极限$\lim \leftarrow G/G_n$ $i : G \to \hat{G}$具有与$G$相关的像豪斯多夫群（$\hat{G}$中处处密集）和核$G$中$\{0\}$的闭包$\bigcap G_n$。 子群 $G_n$ $G$ 的 Hausdorff 完成$\hat{G}_n$ 与 $\hat{G}$ 中$i(G_n)$ 的闭包一致（*一般拓扑*，章 II, § 3, no. 9，推出 1 到命题） 18) 并且，自 $G$ 起，于 $\hat{G}$ 关闭，

$$
G, = i^{-1}(\hat{G}_n) = i^{-1}(\hat{G}_n \cap i(G)).
$$

此外，$\hat{G}$中$\hat{G}_n$形式为0的邻域的基本系统（*常规拓扑*、章111、§ 3, no. 4、命题7），因此为常开子群共$\hat{G}$（一般拓扑、章111、§ 2, no. 3、命题8）； $\hat{G}$ 上的拓扑由过滤$(\hat{G}_n)$ 定义，始终由定义分隔。由于 $i(G)$ 在 $\hat{G}$ 中是稠密的，并且 $\hat{G}_n$ 是开集，

$$
\hat{G} = i(G) \cdot \hat{G}_n
$$

和类似地

$$
= i(G_{n-1}) \cdot \hat{G}_n.
$$

我们从 (18) 和 (19) 推断，当且仅当 $(G_n)$ 时，过滤 $(\hat{G}_n)$ 是穷举的。

第二个同构定理（代数，章I, § 6, no. 13，定理6（d））和方程（18），（19）和（20）表明典范同态

$$
G_{n-1}/G_n \to \hat{G}_{n-1}/\hat{G}_n, \quad G/G_n \to \hat{G}/\hat{G}_n,
$$

是双射的，因此典范同态也是双射的

$$
\operatorname{gr}(G) \to \operatorname{gr}(\hat{G}).
$$

现在让$A$是过滤后的环，$E$是过滤后的$A$模块，$(A_n)$和$(E_n)$分别是$A$和$E$的过滤；我们假设这些过滤是详尽的，因此对于相应的拓扑，$A$是拓扑环，$E$是拓扑$A$模块（no. 5，命题3）。然后我们定义了（常规拓扑，章111，§6，第5和6号）$\hat{A}$作为拓扑环和$\hat{E}$作为拓扑$\hat{A}$模块。如果$i : A \to \hat{A}$是典范同态，则通过乘法在$A$的连续性得到$i(A_m)i(A_n) \subset i(A_{m+n})$、从而，

$$
\hat{A}_m \hat{A}_n \subset \hat{A}_{m+n}
$$

因为$A_n$是$i(A_n)$在$\hat{A}$的闭包。类似地可以证明

$$
\hat{A}_m \hat{E}_n \subset \hat{E}_{m+n};
$$

其他字：

#### 命题 15 {#ac-iii-s2-prop-15 .statement tag=04ER}

令$A$为过滤后的环，$E$为过滤后的$A$模块，$A$和$E$各自的过滤$(A_n), (E_n)$是详尽的。那么$(\hat{A}_n)$是与$\hat{A}$上的环结构兼容的过滤，而$(\hat{E}_n)$是在过滤后的环$\hat{A}$上与$\hat{E}$上的模结构兼容的过滤；此外，这些过滤是详尽的，并且分别$\hat{A}$和$\hat{E}$上的拓扑定义。最后，分级$\mathbf{Z}$-模块中的典范映射$\operatorname{gr}(A) \to \operatorname{gr}(\hat{A})$和$\operatorname{gr}(E) \to \operatorname{gr}(\hat{E})$分别是分级环同构和分级$\operatorname{gr}(A)$-模块同构。

接下来，对于每个制服空间$X$，$j_X$将表示从$X$到其Hausdorff完成$\hat{X}$的典范映射和$X_0 = j_X(X)$$\hat{X}$的制服子空间，这是Hausdorff 空间与 $X$ 相关。回想一下，$X$上的拓扑是$X_0$上的$j_X$下的逆像（一般拓扑，

章II, § 3, no. 7、命题12)。还记得，对于每个均匀连续的映射$f : X \to Y$，$\hat{f}$表示从$\hat{X}$到$\hat{Y}$均匀连续的映射，使得$\hat{f} \circ j_X = j_Y \circ f$（前述，命题15）；如果$X$是$Y$的制服子空间和$\mathscr{E}$典范嵌入，则$\hat{X}$被识别为$\hat{Y}$的制服子空间，并且$\hat{f}$是$X$的典范嵌入到$\hat{Y}$（前述，no. 9。推论 1 至命题 18）。

#### 引理 2 {#ac-iii-s2-lem-2 .statement tag=04ES}

*令$X \xrightarrow{f} Y \xrightarrow{g} Z$为拓扑群严格态射的正合序列（代数、章II, § 1, no. 4、注）。假设$X, Y, Z$承认豪斯多夫完成群并且单位元素$\mathscr{E} X, Y, Z$承认邻域的可数基数系统。那么$\hat{X} \xrightarrow{\hat{f}} \hat{Y} \xrightarrow{\hat{g}} \hat{Z}$就是严格态射的正合序列。*

令$N_1, N_g$分别为核关闭和$g$；让我们写

$$
f = f_3 \circ f_2 \circ f_1
$$

其中$f_1$是典范映射$X \to X/N_f$，$f_2$是$X/N_f$到$N$的同构，$f_3$是典范嵌入$N \to Y$。我们已经知道$f_2$是$(X/N_f)^*$到$\hat{N}_g$的同构，并且我们刚刚回想起$f_1$是$N$到$\hat{Y}$的单射严格态射；如果我们证明$\hat{f}_1$是一个满射严格态射，那么$\hat{f}$是一个严格态射（一般拓扑，章III, § 2, no. 8，注2）。设$g_1$为典范映射$Y \to Y/N_g$；如果我们证明$\hat{g}_1$是核$\hat{N}_g$的满射严格态射，我们将如上所述看到$\hat{g}$是严格的态射并且序列$\hat{X} \xrightarrow{\hat{f}} \hat{Y} \xrightarrow{\hat{g}} \hat{Z}$将是精确的。因此，我们将问题减少到证明，如果$Y = X/N$（其中$N$是$X$的正常子群）并且$f : X \to Y$是典范映射，$\hat{f}$是一个*满射严格态射， 核* $\hat{N}$。

设$f_0 : X_0 \to Y_0$为映射，其中重合与$f$在$X_0$上；因为 $j_X$（分别为 $j_Y$）是 $X$ 到 $X$ 的满射严格态射，（分别为 $Y$ 到 $Y_0$），$f_0$ 是满射严格态射（一般拓扑、章、III, § 2, no. 8、注 3)。现在$X_0$和$Y_0$是可度量的（一般拓扑，章IX, § 3, no. 1，命题1）；那么从一般拓扑，章IX, § 3, no. 1，推论1到命题4和引理1，$\hat{f}_0 = \hat{f}$是满射严格态射并且有核闭包$\hat{N}_0'$*in* $X$ 核 $N_0'$ $f_0$。那么我们只要证明$\hat{N}_0' = \hat{N}$就足够了。现在$N_0'$显然是包含$N_0 = j_X(N)$；足以证明$N_0'$包含在$N_0$*in*$X$的闭包$\overline{N}_0$中。现在，

$$
u = j_X^{-1}(X_0 - \overline{N}_0) = X - j_X^{-1}(\overline{N}_0)
$$

是$X$中的开集合，且不满足$N$；由于$f$是满射严格态射，$V = f(U)$是$Y$中的开集合，而不是$Y$的包含单位元素$e'$，因此不满足$e'$的闭集；那么 $j_Y(V)$ 不等于 $Y_0$ 的包含单位元素。但是 $j_Y(V) = f_0(X_0 - \overline{N}_0)$ 以及$N'_0 \subset \overline{N}_0$，完成引理 2 的证明。

#### 命题 16 {#ac-iii-s2-prop-16 .statement tag=04ET}

*令$A$为已过滤的环，($A,$)其过滤，$E$为$A$模块，且($E_n$)$E$上的过滤源自于$E_n = A_n E$的$A$由……组成上的过滤。假设过滤 ($A,$) 是详尽的，并且模 $E$ 是有限生成的。如果 $i : E \to \hat{E}$ 是典范映射，那么，对于所有 $n \in \mathbf{Z}$，*
$$
8_n = \hat{A}_n \hat{E} = \hat{A}_n i(E) \quad \text{and} \quad \hat{E} = \hat{A}.i(E).
$$
*特别是$\hat{E}$是有限生成的$\hat{A}$模块。*

The equation $A_n E = E_n$ implies, by virtue of the continuity of the external law on the $A$-module $8, \hat{A}_n \hat{E} \subset 8$, and obviously $\hat{A}_n \hat{E} \supset \hat{A}_n i(E)$. 到假设时，存在满同态$u : L \to E$，其中$L = A_s^I$、$I$是有限的集合；让$L$被给予乘积过滤，$L_n = A_n^I$的由……组成，其中定义在$L$乘积拓扑；然后是$\hat{L} = \hat{A}_s^I$和$\hat{L}_n = \hat{A}_n^I$（*一般拓扑*、章II, § 3, no. 9、推论2到命题18）。 设$j : L \to \hat{L}$为典范映射且$(e_i)_{i \in I}$典范基为$L$；对于元素$\sum_{i \in I} a_{ij}(e_i)$（其中$a_i \in \hat{A}$代表所有$i \in I$）到属于到$\hat{L}_n$，$a_i \in \hat{A}_n$对于所有$i$是必要且充分的；然后$\hat{L}_n = \hat{A}_n . j(L)$。 正是如此，通过定义$u(\hat{L}_n) = A_n E = E_n$，因此$u$是$L$到$E$的*严格态射*（*一般拓扑*，章III, § 2, no. 8，命题24）。 引理 2 然后表明$\hat{u} : \hat{L} \to \hat{E}$ 是一个*满射严格态射*。 由于$\hat{L}_n$是开子群关，$\hat{u}(\hat{L}_n)$是$\hat{E}$的开（因此闭）子群；但是$\hat{u}(\hat{L}_n) = \hat{A}_n \hat{u}(j(L)) = \hat{A}_n i(E)$，以及$i(E_n) \subset A_n i(E) \subset \hat{A}_n i(E)$，最后$\hat{E}_n \subset \hat{A}_n i(E) \subset \hat{A}_n \hat{E} \subset \hat{E}_n$，因此$\hat{E}_n = \hat{A}_n \hat{E} = \hat{A}_n i(E)$； 设定$n = 0$，我们得到(25)的第二个公式。

#### 推论 1 {#ac-iii-s2-prop-16-cor-1 .statement tag=04EU}

*在命题 16 的条件下，如果$A$完整，$E$也完整。*

由于典范映射 $A \to \hat{A}$ 是满射 (no. 6, 命题 5)，$\hat{E} = i(E)$ 由 (25) 得出，结论由 no. 6 的命题 5 得出。

#### 推论 2 {#ac-iii-s2-prop-16-cor-2 .statement tag=04EV}

*令$A$为交换环，$m$为$A$和$\hat{A}$的有限生成理想，$A$相对于$m$进数拓扑的豪斯多夫完成。那么$\hat{A}$上的每个整数$n > 0$和拓扑的$\hat{m}^n = (\hat{m})^n = m^n . \hat{A}$就是$\hat{m}$-adic拓扑。*

让我们写出$A_n = m^n$，它是$A$的有限生成理想。 公式 $m^p A_n = m^{n+p}$ 显示$A$ 上的拓扑由$m$-adic 拓扑重合和$m$-adic 拓扑在$A$-模块$A_n$ 上诱导（no. 1，*例3*）。

将命题 16 应用于其他字 $\hat{m}^n = m^n . \hat{A}$ 中的$E = A_n$、$\hat{A}_n = \hat{A}.A_n$。特别是$m = m . \hat{A}$、从而
$$
(\hat{m})^n = m^n . \hat{A} = \hat{A}.A_n
$$
（cf.习题12）。

过滤环的 Hausdorff 补全的例

(1) 令$A$为型$\mathbf{N}$的分级环，令$(A_n)_{n \geq 0}$为其毕业；让它被给予相关的分离和详尽的过滤（no. 1，例1）。 加法群 $A$ 与 $B = \prod_{n \in \mathbf{N}} A_n$ 的子群被规范地标识；如果$B$给定离散拓扑的拓扑乘积，则在$A$上诱导的拓扑是由$A$上的过滤定义的拓扑；另外，$B$是完全拓扑群，$A$在$B$中是稠密的（一般拓扑、章III, §2, no. 9、命题25）。然后，加法拓扑群 $B$ 与 Hausdorff 加法群 $A$ 的完备性 $\hat{A}$ 进行识别，并且从命题 15 可以得出，它具有唯一的环结构，这使其成为拓扑环的完备性$A$。对于环、注中的定义乘法，如果我们写成$A'_n = \sum_{i > n} A_i$，则双边理想$A'_n$在$B$中的闭包是集合$B$，$x = (x_i) \in B$使得$x_i = 0$ 换$i \leq n$。然后令$x = (x_i), y = (y_i)$为$B$和$z = (z_i)$的两个元素和它们的乘积。然后，对于所有 $n > 0$、$x \equiv x'_n$ (mod. $B_n$)、$y \equiv y'_n$ (mod. $B_n$)，其中 $x'_n = (x_i)_{0 \leq i \leq n}$、$y'_n = (y_i)_{0 \leq i \leq n}$、从而 $z \equiv x'_n y'_n$ (mod. $B_n$)。但是$x'_n$和$y'_n$属于到$A$，因此可以看出，对于所有$n \in \mathbf{N}$，

$$
z_n = \sum_{j=0}^n x_j y_{n-j}.
$$

特别是，我们再次获得no. 6的命题 6的推论：如果$C$是交换环，多项式环$C[X_1, \ldots, X_r]$的完成，以及与其通常毕业相关的过滤（总计次数）被规范地识别为正式的环幂级数$C[[X_1, \ldots, X_r]]$（cf.代数、章IV, §5, no. 10）。

*(2) 设$K$为完整的交换域，并有估价。在$K$上的$r$变量中收敛级数的环被规范地等同于形式幂级数$K[[X_1, \ldots, X_r]]$的环。 \*

(3) 令$a$为主理想整环的非零不可逆元素； $A$ 上的 (a)-adic 拓扑也称为 $a$-adic 拓扑；它是 Hausdorff，对于理想 $(a^n)$ 约化到 0（代数、章 VII, §1, no. 3）的交。 注相对于此拓扑完成$A$不一定是整环（cf.no. 13，注3）。相关的分级环 $\mathrm{gr}(A) = \mathrm{gr}(\hat{A})$ 与 $(A/a)[X]$ (no. 3, 例 1) 自然同构。如果$A = \mathbf{Z}$，则$\mathbf{Z}$相对于n进数拓扑（$n > 1$）的补全用$\mathbf{Z}_n$表示，其元素称为$n$-adic整数。

$\mathbf{Z}/n^k \mathbf{Z}$的每个元素都承认形式$\sum_{i=0}^{k-1} a_i n^i$的唯一代表，其中$0 \leq a_i \leq n - 1$代表所有$i$；而且，$\mathbf{Z}/n^{k-1} \mathbf{Z}$中的典范像是$\sum_{i=0}^{k-2} a_i n^i$的类。这些注以及 $Z$ 与逆极限 $\lim_{\leftarrow} \mathbf{Z}/n^k \mathbf{Z}$ 的规范标识立即表明，$Z$ 中的每个元素都可以唯一地写在形式 $\sum_{i=0}^{\infty} a_i n^i$ 其中 $0 \leq a_i < n$ 中，反之亦然级数收敛于$\mathbf{Z}$。

### 13. 半局部环的 HAUSDOFF 补全

#### 命题 17 {#ac-iii-s2-prop-17 .statement tag=04EW}

令$A$为交换环和$(m_{\lambda})_{\lambda \in L}$一组$A$的理想，与$A$不同，使得$m_{\lambda}$和$m_{\mu}$对于$\lambda \neq \mu$互质。对于整数$\geq 0$、有限支撑、集合$a_s = \bigcap_{\lambda \in L} m_{\lambda}^{s(\lambda)}$的每个家庭$s = (s(\lambda))_{\lambda \in L}$（等于$\lambda$的$m_{\lambda}^{s(\lambda)}$的乘积，使得$s(\lambda) \neq 0$；cf. 章 11、§ 1, no. 2、命题 3 和 5)； $a_s$形式相对于拓扑$\mathscr{T}$与$A$上的环结构兼容，邻域的基本系统为0；令 $\hat{A}$ 为 $A$ 相对于此拓扑的 Hausdorff 完成。另一方面，对于所有$\lambda \in L$，令$A_{\lambda}$为环$A$，并带有$m_{\lambda}$进数拓扑，并令$\hat{A}_{\lambda}$为其Hausdorff补全。如果 $u : A \to \prod_{\lambda \in L} A_{\lambda}$ 表示对角线同态，则 $u$ 是连续的且相应的同态 $\hat{u} :$

$$
\hat{A} \to \left( \prod_{\lambda \in L} A_{\lambda} \right)^{\hat{}} = \prod_{\lambda \in L} \hat{A}_{\lambda}
$$

（一般拓扑、章III, § 6, no. 5和章II, § 3, no. 9，推论2至命题18）是拓扑环同构。

第一个断言源自一般拓扑、章III, § 6, no. 3、例3。让我们集合$B = \prod_{\lambda \in L} A_{\lambda}$；由于$A$上的拓扑比每个$m_{\lambda}$进拓扑中的更细，映射$\mathrm{pr}_{\lambda} \circ u$是连续的，因此$u$是连续的。另外，$u(a_s)$是$B$的对角线$A$和$B$的开集合$\bigcap_{\lambda \in L} \mathrm{pr}_{\lambda}^{-1}(m_{\lambda}^{s(\lambda)})$的交；由此可见，$u$是从加法群$A$到$B$以及像$A$的严格态射。现在$\Delta$在$B$中是稠密的。令$b = (a_{\lambda})_{\lambda \in L}$为$B$的元素； $B$ 包含集合（共形式 $b + V$）中的每个$b$邻域，其中$V = \bigcap_{\lambda \in L} \mathrm{pr}_{\lambda}^{-1}(m_{\lambda}^{s(\lambda)})$为家庭$s = (s(\lambda))_{\lambda \in L}$，有限支撑为整数 $\geq 0$。由于$m_{\lambda}^{s(\lambda)}$在对（章II, § 1, no. 2，命题3）中互质，因此存在$x \in A$使得$x \equiv a_{\lambda} \pmod{m_{\lambda}^{s(\lambda)}}$对于所有$\lambda$（前述，命题5），因此$(b + V) \cap A \neq \varnothing$。 群 $B/\Delta$ 的 Hausdorff 完成度为 $\{0\}$； 应用引理 2 of no. 12到正合序列$0 \to A \xrightarrow{u} B, A \xrightarrow{u} B \to B/\Delta$，我们看到$\hat{u}$是$\hat{A}$的同构到$\hat{B}$。

#### 推论{#ac-iii-s2-n13-cor-1 .statement tag=04EX}

令$A$为主理想整环，$P$为$A$的极值元素的代表系统（代数，章VII, § 1, no. 3）。 $A$上的拓扑相对于$\mathbf{A}$形式的理想$\neq 0$，邻域的基本系统为0，与$\mathbf{A}$上的环结构兼容，是Hausdorff，并且$\mathbf{A}$的完备性为对于$x$进拓扑，这个拓扑与$\mathbf{A}$补全的乘积规范同构，其中$x$贯穿$P$。

主要理想 $(x)$ 其中 $\pi \in P$ 是最大且不同的，因此相对素数，我们已经看到 (no. 12, 例 3) $x$-adic 拓扑是 Hausdorff，因此拓扑在命题 17 的叙述中定义，即更细比每个 $x$-adic 拓扑。

如果在$\mathbf{A} = \mathbf{Z}$时应用命题 17的推论，我们用$\hat{\mathbf{Z}}$表示$\mathbf{Z}$相对于拓扑的完成，其中$\mathbf{Z}$形式的所有理想$\neq 0$是邻域的基本系统 0，环同构于$p$进数整数环乘积$\prod_{p \in P} \mathbf{Z}_p$（P为素数数的集合）。

Remarks

(1) 显然，在命题 17 的条件下，拓扑 $\mathscr{T}$ 是$\mathbf{A}$ 上$m_\lambda$-adic 拓扑中最小的上界。

(2) $\prod_{\lambda \in L} \hat{A}_\lambda$的每一个闭理想$a$都与其投影$a_\lambda = \mathrm{pr}_\lambda(a)$的乘积相同，都是$A_\lambda$中的闭理想；对于 $\hat{A}_\lambda$ 来说，规范地用 $\prod_{\lambda} \hat{A}_\lambda$ 和 $a_\lambda$ 的封闭理想 $A'_\lambda$ 和 $a \cap A'_\lambda$ (代数, 章 I, §8, no. 10, 命题 6), $a_\lambda$ 的和来标识密集在乘积$\prod_\lambda a_\lambda$（一般拓扑，章III, §2, no. 9，命题25），后者在$\prod_\lambda \hat{A}_\lambda$，从而我们的断言关闭。

#### 命题 18 {#ac-iii-s2-prop-18 .statement tag=04EY}

令 $\mathbf{A}$ 为交换环，$(m_i)_{1 \leq i \leq q}$ $\mathbf{A}$、t 乘积理想$m_1 m_2 \ldots m_q = m_1 \cap m_2 \cap \ldots \cap m_q$ 和$S$ 乘法子集 $\bigcap_{i=1}^q (\mathbf{A} - m_i)$ 的有限族。让 $\mathbf{A}$ 被赋予 $r$-adic 拓扑，环 $B = S^{-1} \mathbf{A}$ $rB$-adic 拓扑以及每个局部环 $A_n$ $(m_i A_{m_i})$-adic 拓扑。设$u : \mathbf{A} \to B$、$v_i : B \to A_{m_i}$为典范同态（章II, §2, no.1，推论2到命题2）和$v$同态$(v_i) : B \to \prod_{i=1}^q A_n$。 同态 $u$ 和 $v$ 是连续的，相应的同态 $\hat{u} : \hat{\mathbf{A}} \to$ 和 $\hat{v} : \hat{B} \to \prod_{n} (A_n)^*$ 是拓扑环同构。

$m_i \cap S = \varnothing$ 对于 $1 \leq i \leq q$，因此 $B$ 的理想 $m'_i = m_i B$ 是最大的（章 II, §2, no. 5，命题 11）并且
$$
rB = m'_1 \cap m'_2 \cap \cdots \cap m'_q
$$

（章II, § 2, no. 4）；最后，$B_{m'_i} = A_i$，直至典范同构（章 11、§ 2, no. 5、命题 11）。由于$\bar{u}^1(rB) = r$和$\bar{v}_i^1(m_iA_{m_i}) \supset rB$，$u$和$v$是连续的。那么就足以证明，

$$
w = v \circ u : A \to \prod_{i=1}^4 A_{m_i},
$$

$\hat{w}$ 是 $\hat{A}$ 的同构到 $\prod_{i=1}^q \hat{A}_{m_i}$，因为将此结果应用于$B$，$m'_i$ 将显示$\hat{v}$ 是同构，因此也是 $\hat{u}$。 注 $m_i$ 包含幂 $c$ 中的幂的每一个乘积，因此$r$-adic 拓扑是 $m_i$-adic 中最小的上界拓扑结构；此外，如果$A_i$用$m_i$-adic拓扑和$\phi : A \to \prod_{i=1}^q A$表示环$A$，则映射、$\hat{\phi} : \hat{A} \to \prod_{i=1}^4 \hat{A}_i$的对角线为同构（命题17）。那么，如果$u_i : A_i \to A_{m_i}$是典范映射，那么$\hat{u}_i : \hat{A}_i \to \hat{A}_{m_i}$就是同构，那么这一切就等于证明。现在，对于所有$n$，映射

$$
u_{i,n} : A/m_i^n \to A_{m_i}/m_i^n A_{m_i}
$$

由 $u_i$ 取商得出同构 (章 II, §3, no. 3, 命题 9)；我们的断言源自以下事实：$\hat{A}_i$（分别为 $\hat{A}_{m_i}$）是离散环 $A/m_i^n$（分别为 $A_{m_i}/m_i^n A_{m_i}$）（cf. no. 6）的逆极限。

注 (3)。我们看到整环$A$可以使得它的Hausdorff完成$\hat{A}$承认零的非零除数。

#### 命题 19 {#ac-iii-s2-prop-19 .statement tag=04EZ}

令$A$为交换环，且$m$为$A$的最大理想。 $A$相对于$m$进数拓扑的豪斯多夫完成$\hat{A}$是局部环，其最大理想是$m$。

如果 $a = \bigcap_{k \geq 1} m^k$、$\hat{A}$ 是与 $A$ 相关的 Hausdorff 环 $A/a$ 的完成，并且由于 $m/a$ 在 $A/a$ 中最大，我们可以假设 $A$ 是相对于$m$-adic 拓扑。由于$A/m$和$\hat{A}/\hat{m}$同构环（no. 12，公式（21）），$m$在$\hat{A}$中最大。由于$\hat{A}$上的拓扑由过滤$(m^n)^*$（no. 12）定义，命题将是以下引理的推论：

#### 引理 3 {#ac-iii-s2-lem-3 .statement tag=04F0}

设$A$是一个完整的Hausdorf拓扑环，其中存在$A$的0由……组成的加法子群的邻域的基系统$\mathscr{G}$。
(i) 对于所有$x \in A$，使得$\lim_{n \to m} x^n = 0$、$1 - x$在$A$中可逆，并且其逆等于$\sum_{n=0}^\infty x^n$。
(ii) 设$a$为$A$的双面理想，使得$\lim_{n \to \infty} x^n = 0$对于所有$x \in a$。为了使 $\mathbf{A}$ 的元素 y 可逆，其类 mod 是充分必要的。 a 在 $\mathbf{A}/a$ 中可逆；特别是a包含在$\mathbf{A}$的雅各布森根中。

(一) 作为

$$
(1 - x)(1 + x + \cdots + x^n) = (1 + x + \cdots + x^n)(1 - x) = 1 - x^{n+1},
$$

证明级数与一般项 $x^n$ 收敛于 $\mathbf{A}$；现在，到假设，对于$\mathbf{A}$中0的每个邻域$V \in \mathfrak{S}$，存在整数$p > 0$，这样对于所有$n \geq p$都有$x^n \in V$。我们结论

$$
x^p + x^{p+1} + \ldots + x^q \in V
$$

对于所有$q \geq p$和我们的断言则遵循柯西准则（*一般拓扑*，章III, § 5, no. 2，定理1）。

(ii) 假设存在$y' \in \mathbf{A}$使得$yy' \equiv 1$(mod.a)和$y'y \equiv 1$(mod.a)。 a 上的假设通过(i)暗示$yy'$和$y'y$在$\mathbf{A}$中可逆，因此$y$在$\mathbf{A}$中可逆。特别是，每个$x \in a$使得$1 - x$在$\mathbf{A}$中可逆，并且由于a是$\mathbf{A}$的双面理想，因此它包含在$\mathbf{A}$的Jacobson根式中（*代数*，章VIII, § 6, no. 3， 定理1)。

建立了这个引理后，就足以将其应用于拓扑环$\hat{\mathbf{A}}$和理想$\hat{\mathfrak{m}}$，因为对于所有$x \in \hat{\mathfrak{m}}$，$x^n \in (\hat{\mathfrak{m}})^n \subset (\mathfrak{m}^n)^{\wedge}$和序列$(x^n)$因此趋于0。

如果我们取$\mathbf{A} = \mathbf{Z}$，$\mathbf{Z}$的每个最大理想都是形式$p\mathbf{Z}$，其中$p$是素数。 $p$-adic 数 $\mathbf{Z}_p$的环则为局部环，其中$p\mathbf{Z}_p$是最大理想（推论2到命题16），并且其剩余类域同构于$\mathbf{Z}/p\mathbf{Z} = \mathbf{F}_p$，并且$\mathbf{Z}_{(p)}$ 与$p\mathbf{Z}_{(p)}$-adic 拓扑被识别为$\mathbf{Z}$、包含于 $\mathbf{Z}$ 的拓扑子环。

#### 推论{#ac-iii-s2-n13-cor-2 .statement tag=04F1}

令 $\mathbf{A}$ 为半局部环 (章 II, § 3, no. 5)，$m_i$ 其独特的最大理想 $(1 \leq i \leq q)$ 和

$$
r = m_1 \cap m_2 \cap \cdots \cap m_q
$$

这是雅各布森激进的。 $\mathbf{A}$ 相对于 r-adic 拓扑的 Hausdorff 补全 $\hat{\mathbf{A}}$ 是一个半局部环，与乘积 $\prod_{i=1}^q \hat{\mathbf{A}}_{m_i}$ 自然同构，其中 $\hat{\mathbf{A}}_{m_i}$ 是局部环 $\mathbf{A}_{m_i}$ 的 Hausdorff 补全环到 $(m_i \mathbf{A}_{m_i})$-adic 拓扑。

### 习题 {#ac-iii-s2-exercises}

§ 2](exercises/s2/)参见[习题。
