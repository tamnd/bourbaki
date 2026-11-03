---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 14
section_title: Central Simple Algebras
lang: zh
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.251-A VIII.276
pdf_pages: 0268-0293
extraction: native
subsections:
    - "no": 1
      title: Central Simple Algebras
      page: 251
      pdf_page: 268
    - "no": 2
      title: Two Lemmas on Bimodules
      page: 254
      pdf_page: 271
    - "no": 3
      title: Conjugacy Theorems
      page: 256
      pdf_page: 273
    - "no": 4
      title: Automorphisms of Semisimple Algebras
      page: 257
      pdf_page: 274
    - "no": 5
      title: Simple Subalgebras of Simple Algebras
      page: 259
      pdf_page: 276
    - "no": 6
      title: Maximal Commutative Subalgebras
      page: 261
      pdf_page: 278
    - "no": 7
      title: Maximal Étale Subalgebras
      page: 264
      pdf_page: 281
    - "no": 8
      title: Diagonalizable Subalgebras of Simple Algebras
      page: 266
      pdf_page: 283
statements: 36
exercises: 19
content_sha256: 3834ac6fff26b086d0c02803c85da1e60b789466744711c2694c0ce8af4f7967
translated_from: content/en/alg/VIII/14_s14_central_simple_algebras.md
translation_method: google
source_content_sha256: 6b4399d77699c060fb6846778021967e62ae015f18624ee87348066955fdf6f2
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: b639b7169c2a23f3c36d7e2b6ead927cf76b77d52cdafe62d68e92048680f5f9
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 14。中环单代数

在这个截面中，K是交换域。

### 1. 中环单代数

#### 定义 1 {#alg-viii-s14-def-1 .statement tag=00GE}

如果映射 $\lambda \mapsto \lambda 1$ 是从 A 的 K 到中心的双射，我们就说域 K 上的代数 A 是中心的。

中心代数不会减少到0。对于每个整数$n\geqslant 1$，矩阵K-代数$\mathbf{M}_n(K)$是中心（VIII，p. 83，推论2）和简单（VIII，p. 120， 定理1)。更一般地，令 D 为有限次数的中心 K-代数；那么$\mathbf{M}_n(D)$也是中心。设 A 为简单的环；它的中心 Z 是域 (VIII, p. 121, 推论 1)，因而 A 是 Z 上的中心单代数。如果域 K 是代数闭的，则有限次数的单代数在 K 上是中心（VIII、p. 122、推论 3）。中心单代数的反代数是中心简单。

#### 注 1 {#alg-viii-s14-n1-rem-1 .statement tag=00GF}

设 A 和 B 为 K-代数。如果$A\otimes_KB$是中心单代数，则A和B也是中心单代数（III, §4, No. 4，p. 468，推论/命题6和VIII，p. 221，命题6）。相反，如果 A 和 B 是中心单代数并且其中一个在 K 上具有有限次数，则 $A\otimes_KB$ 是中心单代数（命题 6 和 VIII、p. 222 的III, §4, No. 4、p. 468、推论， 推论2)。

#### 注 2 {#alg-viii-s14-n1-rem-2 .statement tag=00GG}

设 A 为域 K 的 K-代数和 L 扩张。如果 L 代数 $A_{(L)}$ 是中心单形，则 K-代数 A 是中心单形。相反，如果次数 [A : K] 和 [L : K] 之一是有限的，并且 A 是中心单K-代数，则 L 代数 $A_{(L)}$ 是中心简单的。这是从VIII、p. 222 的推论 2 得出的。

#### 注 3 {#alg-viii-s14-n1-rem-3 .statement tag=00GH}

令 A 和 B 为森田等价K-代数。 代数 A 是中心简单当且仅当 B 是 (VIII, p. 105, 命题 6; p. 111, 推论; 和 p. 102, 推论 1)。

#### 注 4 {#alg-viii-s14-n1-rem-4 .statement tag=00GI}

特别是，如果 A 为中心单K-代数和 $n\geqslant 1$，则 $\mathbf{M}_n(A)$ 为中心单K-代数（VIII、p. 102、例 1）。

#### 定理 1 {#alg-viii-s14-thm-1 .statement tag=00GJ}

设 A 为有限次数的 K-代数。以下属性是等效的：

(i) 代数 A 是中心简单语。

(ii) 代数 A 是中心且没有根基。

(iii) 从K-代数$A\otimes_KA^o$到K-代数End$_K(A)$的典范同态将$a\otimes a'$到K-线性映射$x\mapsto axa'$从A发送到A是双射的。

(iv) 存在域 K 和整数 $n\geqslant 1$ 的扩张 L，使得L-代数$A_{(L)}$ 和$\mathbf{M}_n(L)$ 同构。

(v) 对于 K 的每个可分闭包 $K'$，都存在整数 $n\geqslant 1$，使得 $K'$-代数 $A_{(K')}$ 和 $\mathbf{M}_n(K')$ 同构。

(vi) 存在有限次数和整数$n\geqslant 1$的域K的伽罗瓦扩张L，使得L-代数$A_{(L)}$和$\mathbf{M}_n(L)$同构。

(vii) 存在有限次数 D 的K-代数，即域、中心 K 和整数 $n\geqslant 1$，使得代数 A 同构于代数 $\mathbf{M}_n(D)$。

环是简单的当且仅当它是半单并且它的中心是域（VIII、p. 143、推论 of 命题 10）。由于A是有限次数的代数除以域K，所以它是左阿廷的环；因而，当且仅当没有根基 (VIII, p. 154, 命题 4) 时，它才是半单。 (i) 和 (ii) 的等价如下。

集合 $E = A\otimes_KA^o$ 且 F = 结束$_K(A)$；表示从 E 到 F 的 $\varphi$ 典范同态，由 A 中的 $x, a, a'$ 的关系 $\varphi (a\otimes a')(x) =axa'$ 定义。如果代数 A 是中心单形，那么 $A^o$ 也是中心单形，因而，E (注 1)，因而 $\varphi$ 是单射的。现在，我们有 $[E : K] = [A : K]^2= [F : K]$，所以 $\varphi$ 是双射的。相反，假设 $\varphi$ 是双射；因为代数 F 是中心单元（因为它与矩阵代数 $\mathbf{M}_m$(K) 同构），所以 E 也是中心简单，因而 A (注 1) 也是。这样我们就证明了(i)和(iii)的等价。

通过注 4，断言 (vii) 意味着断言 (i)。 逆命题蕴涵来自VIII、p. 122的推论3和VIII、p. 83的推论2。

显然，(vi) 隐含 (iv)，(iv) 通过注 2 隐含 (i)。

仍有待证明含义 (i)$\Rightarrow$(v)$\Rightarrow$(vi)。假设 A 是中心简单，并令 $K'$ 为 K (V, §7, No. 8, p. 45) 的可分闭包 。那么$A_{(K')}$是有限次数在$K'$上的中心单代数（VIII，p. 251，注2）。由VIII、p. 231的推论，因此存在从$A_{(K')}$到$\mathbf{M}_n(K')$的$K'$代数的整数$n\geqslant 1$和同构；观察$K'$-代数$\mathbf{M}_n(K')$和$\mathbf{M}_n(K)_{(K')}$是同构的。通过VIII、p. 234的引理 4，存在$K'$的子扩张L，在K上有限生成，使得L-代数$A_{(L)}$和$\mathbf{M}_n(K)_{(L)}$是同构的。那么L是可分的并且有限次数在K上，因此包含在$K'$的子外延$L'$中，即伽罗瓦和有限次数在K上（V, §10, No. 1，p. 57，命题2）。那么$L'$-代数$A_{(L')}$和$\mathbf{M}_n(L')$是同构的。

#### 推论 1 {#alg-viii-s14-thm-1-cor-1 .statement tag=00GK}

设A是可分闭域K上有限次数的中心单代数。存在整数$n\geqslant 1$使得A与矩阵代数$\mathbf{M}_n(K)$同构。

事实上，K 的每个伽罗瓦扩张都等于 K；只需应用定理 1 的属性 (i) 和 (v) 中的等价即可。

#### 推论 2 {#alg-viii-s14-thm-1-cor-2 .statement tag=00GL}

令 A 为 K 上有限次数的中心单代数（例如，K 上有限次数的域和中心 K）。存在整数$n\geqslant 1$使得$[A : K] =n^2$。

令 L 为 K 的扩张，并且 $n$ 严格为正整数，使得 L 代数 $A_{(L)}$ 和 $\mathbf{M}_n(L)$ 同构。我们有

$$
[A : K] = [A_{(L)}: L] = [\mathbf{M}_n(L) : L] =n^2
$$

在推论2的记号中，整数$n$称为A的约化次数。

#### 注 5 {#alg-viii-s14-n1-rem-5 .statement tag=00GM}

设A是K上有限次数的中心单代数，其约简次数是素数数$\ell$。那么要么 A 是域，要么 A 与 $\mathbf{M}_{\ell}(K)$ 同构。事实上，A 同构于形式 $\mathbf{M}_n$(D) 的代数，其中 D 是域，中心 K，并且我们有

$$
\ell^2= [A : K] =n^2[D : K]
$$

如果 A 不是域，则 $n\not= 1$，因此 $n=\ell$ 并且 D = K。

### 2. 双模的两个引理

设 A 和 B 为环。对于从 B 到 A 的任何同态 $f$，我们用 $A^f$ 表示 $(B$，A)-双模，其底层右A-模 $A_d$ 和外法则表示由 $(b, a)\mapsto f(b)a$ 给出的左B-模结构。

#### 引理 1 {#alg-viii-s14-lem-1 .statement tag=00GN}

令从B到A的$f$和$g$为同态。以下条件是等价的：

(i) $(B,A)$双模$A^f$和$A^g$是同构的。

(ii) A 存在内自同构 (I, §8, No. 4, p. 102, 例 2) $\theta$，使得$g=\theta \circ f$。

右A-模 $A_d$的自同构是映射$x\mapsto ax$，其中$a$是A的可逆元。这样的自同构是从$A^f$到$A^g$的B-线性映射当且仅当我们有

$$
g(b)ax=af(b)x
$$

对于A中的每个$x$和B中的每个$b$。这个关系相当于B中每个$b$的$g(b) =af(b)a^{-1}$，即$g=\theta \circ f$，其中$\theta$是A的内自同构$x\mapsto axa^{-1}$。

#### 引理 2 {#alg-viii-s14-lem-2 .statement tag=00GO}

假设 B 是半单环，即有限生成模超过其中心 Z。令 M 和 N 为 $(B,A)$ 双模。假设它们有有限长度（尤其是当它们是右A-模或有限长度时）。如果 M 和 N 同构为 $(Z,A)$-双模，则它们同构为 $(B,A)$-双模。

A) 首先考虑 B 为向量空间 S 的自同态环有限维 $d$ 超过交换域 L 的情况。那么我们有 Z = L；我们将 S 视为 $(B$, Z)-双模。 环 B 是简单的，S 是单B-模，Z 是 S 的交换子；每个 B-模都是型 S (VIII, p. 122, 命题 2 a)) 的同型。令$(V, \alpha )$（或$(W, \beta )$）为描述 / B-模 M（或N）。 集合 V（分别为W）被赋予了$(Z$，A）-双模结构，使得$\alpha$（分别为$\beta$）是$(B$，A）-双模（VIII，p. 64，的同构， 注2)。作为$(Z$，A)-双模，M与$V^d$同构，N与$W^d$同构，并且存在从$(Z$的集合到同构，V的子双模，按包含排序，到$(B$， A)-M 的子双模（loc. cit.）。因此V是有限长度的$(Z$，A)双模，W也是。由于$(Z,A)$-双模$V^d$和$W^d$同构，$(Z$，A)-双模V和W同构定理 2，VIII、p. 37 的 d) 适用于环 $Z\otimes_{\mathbf{Z}}A^o$。最后，$(B$，A)-双模M和N是同构的。

B) 现在考虑 B 是作为 Z 模块有限生成的简单环的情况。则Z为域，B为域Z上有限次数的中心单代数。由VIII、p. 252的定理1，存在有限次数Z的扩张$Z'$在Z上，这样$Z'$-代数$B'= B_{(Z')}$同构于有限维$Z'$向量空间的内同态代数。 集合$M'= M_{(Z')}$和$N'= N_{(Z')}$。那么$M'$和$N'$是$(B'$，A)-有限长度的双模；视为 $(Z'$，A)-双模，$M'$ 和 $N'$ 是同构的。根据情况，$A), M'$和$N'$同构为$(B'$，A)-双模，更不必说同构为$(B$，A)-双模。 集合$r= [Z': Z]$。 $(B$，A)-双模$M'= Z'\otimes_ZM$同构于$M^r$，同样，$(B$，A)-双模$N'$同构于$N^r$。由于 M 和 N 是有限长度的 $(B$，A) 双模，因此从 VIII，p. 37 的定理 2, d) 可以得出，$(B$，A)-双模 M 和 N 是同构的。

C) 最后，考虑一般情况，当 B 为半单环时，它作为 Z 模有限生成。设$\mathscr{S}$为单B-模类集合；它是有限的（VIII、p. 136、命题 1）。对于任何 $\lambda \in \mathscr{S}$，用 $M_{\lambda}$（分别为 $N_{\lambda}$）表示型 $\lambda$ 和 B-模 M（分别为 N）的同型分量；它是 M（或 N）（注，VIII，p. 67）的$(B$，A）子双模。对于$\lambda \in \mathscr{S}$，用$\mathfrak{b}_{\lambda}$和集合$B_{\lambda}= B/\mathfrak{b}_{\lambda}$表示B-模$\lambda$的湮没子；令 $Z_{\lambda}$ 为 $B_{\lambda}$ 的中心。对于$\lambda \in \mathscr{S}$，$(B_{\lambda}$、A)-双模$M_{\lambda}$和$N_{\lambda}$有有限长度。然后我们可以将认同 B 与简单的环 $B_{\lambda}$ 的乘积相结合，将 Z 与 $Z_{\lambda}$ 的乘积相结合（VIII、p. 141、命题 8）。此外，我们将可以确定 M 与 $\prod_{\lambda\in\mathscr{S}}M_{\lambda}$ 组合，将 N 与 $\prod_{\lambda\in\mathscr{S}}N_{\lambda}$ 组合。通过假设，M和N同构为$(Z$，A)-双模；由此可见，$\lambda \in \mathscr{S}, M_{\lambda}$ 和 $N_{\lambda}$ 是同构的 $(Z_{\lambda}$，A)-双模。根据B)中处理的情况，$(B_{\lambda}$，A)-双模$M_{\lambda}$和$N_{\lambda}$是同构的，因而$(B$，A)-双模M和N是同构的。

#### 注 {#alg-viii-s14-n2-rem-1 .statement tag=00GP}

由引理 2 的证明得出，M和N是有限长度的$(Z,A)$双模。因而，如果 B 和 A 是两个半单环，它们各自的中心 Z(B) 和 Z(A) 上的有限生成模，则有限长度的两个 $(B$, A)-双模同构，与 (Z(B),Z(A))-双模同构。

### 3. 共轭定理

#### 定理 2 {#alg-viii-s14-thm-2 .statement tag=00GQ}

设B为半单环，Z为中心；假设 B 是有限生成的 Z 模块。设A为右阿廷环，并令从B到A的$f$和$g$为环同态；将$f$和$g$的限制写成$f_Z$和$g_Z$到Z。以下性质是等价的：

(i) A 存在内自同构$\theta$使得$g=\theta \circ f$。

(ii) A 存在内自同构$\theta$使得$g_Z=\theta \circ f_Z$。

由于环 A 是右阿廷，$A_d$ 是有限长度中的右A-模（VIII、p. 6、定理 1）。因而$A^f$和$A^g$是$(B$，A)-有限长度的双模。通过引理 1 (VIII, p. 254)，断言 (i) 表示 $A^f$ 和 $A^g$ 同构 $(B$, A)-双模，断言 (ii) 表示它们同构$(Z,A)$-双模块。因而，(i) 和 (ii) 的等价由引理 2 (VIII，p. 254) 得出。

#### 推论 {#alg-viii-s14-n3-cor-1 .statement tag=00GR}

设 A 和 B 为代数超过域 K。假设 B 是中心简单且为有限次数，并且 A 为右阿廷。令从B到A的$f$和$g$为K-代数同态。A存在内自同构$\theta$使得$g=\theta \circ f$。

在定理 2 的记号中，我们有 Z = K，因此有 $f_Z= 1_Z=g_Z$。

#### 定理 3（斯科伦-诺特）{#alg-viii-s14-thm-3 .statement tag=00S9}

设 A 和 B 为单K-代数，Z(A) 和 Z(B) 为中心。假设代数 B 在 K 上有有限次数，并且代数 $Z(A)\otimes_KZ(B)$ 是域（特别是当 A 或 B 是中心时的情况）。设$f$和$g$为从B到A的K-代数同态。A存在内自同构$\theta$使得$g=\theta \circ f$。

通过VIII、p. 254的引理 1，足以证明$(B,A)$双模$A^f$和$A^g$是同构的。现在，我们可以将$A^f$和$A^g$视为左模超过代数$C = B\otimes_KA^o$，这很简单，可以通过VIII、p. 221的命题7来实现。由于右A-模、$A^f$和$A^g$与$A_d$同构，因此有有限长度，因为环 A 是简单的（VIII、p. 121、推论 1）。 更不必说、$A^f$和$A^g$是C-有限长度的模块。设 S 是一个简单的 C 模块；严格存在正整数、$m$和$n$，使得$A^f$与$S^m$同构，$A^g$与$S^n$同构。因此右A-模 S 有非零的有限长度。由于$A^f$和$A^g$底层的右A-模同构，因此它们具有相同的长度；因此我们有$m=n$，因此C模块$A^f$和$A^g$是同构的。

#### 推论 1 {#alg-viii-s14-thm-3-cor-1 .statement tag=00GS}

设A是K上的中心单代数，并令L是有限次数的K的扩张。如果从L到A，$f$和$g$是K-代数同态，则A存在内自同构$\theta$使得$g=\theta \circ f$。

#### 推论 2 {#alg-viii-s14-thm-3-cor-2 .statement tag=00GT}

设 A 为 K 上的中心单代数，并令 L 为 A 的子代数，即域。 A 的每个 K-代数同态从 L 到扩展到内自同构。

#### 推论 3 {#alg-viii-s14-thm-3-cor-3 .statement tag=00GU}

设 D 为 K 上有限次数的域和中心 K。D 的每个元素都是 K 上的代数。设 $x$ 和 $y$ 为 D 的元素；存在$D^*$的元素$a$使得$y=axa^{-1}$当且仅当$x$和$y$在K上具有相同的最小多项式。

第一个断言源自推论 1 of V, §3, No. 1、p. 17。

假设存在$D^*$的元素$a$使得$y=axa^{-1}$；对于 K[X] 的每个多项式 P，我们有 $P(y) =aP(x)a^{-1}$，特别是，当且且仅当 $P(y) = 0$ 时，我们才有 $P(x) = 0$。因而，$x$ 和 $y$ 在 K 上具有相同的最小多项式（V, §3, No. 1、p. 16、定理 1）。

相反，假设 $x$ 和 $y$ 具有相同的最小多项式。按地点。如上所述，存在从$K[x]$到$K[y]$的K-同构$u$，使得$u(x) =y$，并且$K[x]$是域。由 D 的推论 2$,u$ 扩展到内自同构 $\theta :z\mapsto aza^{-1}$，因此我们有 $y=\theta (x) =axa^{-1}$。

#### 命题 1 {#alg-viii-s14-prop-1 .statement tag=00GV}

设 A 为 K 上有限次数的中心单代数。设 B 为 K-代数，并令 $f$ 和 $g$ 为从 B 到 A 的代数同态。以下性质是等效的：

(i) A 存在内自同构$\theta$使得$g=\theta \circ f$。

(ii) 由于左B-模，$A^f$和$A^g$是同构的。

通过引理 1 (VIII, p. 254)，性质 (i) 等价于$A^f$ 和$A^g$ 同构为$(B$, A)-双模。由于 A 是 $K, A^f$ 和 $A^g$ 上的有限维，因此是 B-模或有限长度。由于 A 的中心等于 K，(i) 和 (ii) 的等价由 VIII 的引理 2 得出，p. 254 应用于 $(A^o,B^o$) 双模 $A^f$ 和 $A^g$。

### 4. 自同构 / 半单代数

#### 定理 4 {#alg-viii-s14-thm-4 .statement tag=00GW}

设 A 为半单环，Z 为中心，A 的 $u$ 自同构。假设 A 是有限生成的 Z 模，并且对于 Z 中的每个 $z$，我们都有 $u(z) =z$。则 $u$ 为内自同构。

这是从应用$f=$Id$_A$和$g=u$应用VIII、p. 256的定理2开始的。

#### 例 {#alg-viii-s14-n4-exa-1 .statement tag=00RH}

定理4适用于以下两种具体情况：

a) 设 D 为域，Z 为中心。如果 D 在 Z 上有有限次数，则固定 Z 的元素的 D 的每个自同构都是内自同构。 D 比 Z 具有有限次数的假设是必要的（VIII、p. 269、习题 4）。

b) 令V在域K上成为有限维向量空间。K-代数End$_K(V)$的每一个自同构都是内自同构；这个结果扩展适用于空间V不是K上的有限维（VIII，p. 272，习题13）。

特别是，矩阵代数 $\mathbf{M}_n(K)$（与$n\geqslant$ 1）中的每个自同构都是内自同构。该结果承认以下推广。

#### 命题 2 {#alg-viii-s14-prop-2 .statement tag=00GX}

令L为交换环，V为有限维$m$的自由L模块。假设每个$M^m$同构于$L^m$的L模M也同构于L。那么L代数End$_L(V)$的每个自同构都是内自同构。

集合 B = 结束$_L(V)$。令$u$为L-代数B的自同构。我们将V视为左B-模；令$u_*(V)$为与$u$相关的左B-模，以及外法则$(b, v)\mapsto u(b)(v)$（II, §1, No. 13，p. 221）。设$(e_1, . . . , e_m)$为L模块V的基；给定V的元素$v_1, . . . , v_m$，存在B的唯一元素$b$，这样我们就有$b(e_i) =v_i$对应$1\leqslant i\leqslant m$。在其他字、$V^m$的元素$e= (e_1, . . . , e_m)$提供B-模$V^m$的基。由于$u$是自同构，$e$也给出B-模$u_*(V^m) =u_*(V)^m$的基，因此与$V^m$同构。 $(B$, L)-双模 V 是可逆的 (VIII, p. 102, 例 1)。根据VIII、p. 103的定理 2, b)，因此存在L模M，使得B-模$u_*(V)$同构于$V\otimes_LM$。 B-模 $V\otimes_LL^m$ 和 $V\otimes_LM^m$ 分别同构于 $V^m$ 和 $u_*(V)^m$，因此是同构的。按地点。如上所述，L模块$L^m$和$M^m$是同构的。给定假设，M 与 L 同构；因而，与$V\otimes_LM$同构的B-模$u_*$(V)也与V同构。设$h$从V到$u_*(V)$为B-模同构；特别是，它是L模块V的自同构，即B的可逆元。对于B中的$b$和V中的$v$，我们有$h(b(v)) =u(b)(h(v))$，因此有$u(b) =hbh^{-1}$。

特别是，当交换环L是主理想域（VII, §3，p. 15，推论3）或者是Artinian环（VIII，p. 37，定理2，d））或局部环（VIII，p. 36，推论6）时，命题2的​​条件得到满足。

### 5. 单子代数 / 单代数

#### 定理 5 {#alg-viii-s14-thm-5 .statement tag=00GY}

设A为中心单K-代数，设B为有限次数的A在K上的半单子代数。

a) A中B的交换子$B'$为单子代数，B为A中$B'$的交换子。此外，K上的代数$B\cap B'$为有限次数的半单交换代数；是B的公共中心和$B'$。

b) 假设 B 是简单的。那么$B'$很简单，我们有等式

$$
[A : B']_s= [B : K],[A : B]_s= [B': K],[A : K] = [B : K][B': K]
$$

（左侧次数$[A : B]_s.$的定义参见VIII、p. 124、定义2）

K-代数$A^o$是中心简单，K-代数B是半单和有限次数。 推论 VIII、p. 221、代数 $C = B\otimes_KA^o$ 中的 1 个为半单。令 M 为与 A 具有相同加法群且外法则由 A 中的 $a, a'$ 和 B 中的 $b$ 的公式 $(b\otimes a)a'=ba'a$ 给出的 C 模。令 $u$ 为 End$_{\mathbf{Z}}(A)$ 的元素。那么C模M的$u$属于到交换子$C'_M$当且仅当$u$是右A线性且左B线性，在其他字中，当且仅当$u$属于到A-模$A_s$同位环中$B_M$的交换子。因而，我们将定义同构$\gamma$从$B'$到$C'_M$通过关系$\gamma (b')(x) =b'x$为$B'$中的$b'$和M中的$x$。现在，环 C为半单，C模M由A的元素1生成。由VIII的命题6生成，p. 139，环$C'_M$为半单，所以代数$B'$为半单。

令$\varphi$为从$A\otimes_KA^o$到End$_K(M)$的K-代数同态，将$a\otimes a'$到K-线性映射$x\mapsto axa'$从M到M。由于K-代数A和$A^o$是中心简单，所以唯一$A\otimes_KA^o$ 的两侧理想是 0 和 $A\otimes_KA^o$ (VIII, p. 218, 推论)。我们有$C_M=\varphi (B\otimes A^o)$和$C'_M=\varphi (B'\otimes K)$。 同态 $\varphi$ 不是零；因此它是单射的。由于环C是半单，我们有$C''_M= C_M$乘命题5个VIII，p. 139。由此可见，$A\otimes_KA^o$的子代数$B\otimes_KA^o$是子代数$B'\otimes_KK$的交换子。因而，$A\otimes_KK$中$B'\otimes_KK$的交换子等于$(B\otimes_KA^o)\cap (A\otimes_KK)$，即$B\otimes K$乘以II, §7, No. 9、p. 311的命题 19。因而，A 中 $B'$ 的交换子等于 B。代数 $L = B\cap B'$ 是 B 的中心。由于 B 是 K 上有限次数的半单代数，所以代数 L 是可交换的，并且半单并且对 K 具有有限次数。由于 B 是 A 中 $B'$ 的交换子，因而 $B'$ 的中心也等于 $L = B\cap B'$（VIII，p. 77）。我们已经证明了a）。

现在假设代数 B 是简单的。通过VIII、p. 222、环C中的推论 2 很简单。通过VIII的命题 4，p. 123应用于C模M，其交换子与$B'$同构的，环$B'$是简单的，并且M是有限长度的$B'$模。在其他字中，$B'$是简单环A的简单子环，而左边的次数$[A : B']_s$是整数$m\geqslant 1$。作为左 $B'$ 模，A 具有有限的基 $(a_1, . . . , a_m)$。此外（前述），$\varphi$诱导由限制同构从C到$C''_M=$结束$_{B'}$（A），以及映射$c\mapsto (ca_1, . . . , ca_m)$从C到$A^m$是因此是双射的。因而，C 是维数 $m$ 的免费右A-模。现在，我们有$C = B\otimes A^o$，所以C是维数的免费右A-模[B : K]；由此可见$[A : B']_s=m= [B : K]$。从VIII、p. 125的命题 6，我们推导出

$$
[A : K] = [A : B']_s[B': K] = [B : K] [B': K]
$$

因为我们也有

$$
[A : K] = [A : B]_s[B : K]
$$

[B : K] 是有限的，非零的，我们结论，我们有等式 $[A : B]_s= [B': K] ($集合理论，III, §6, No. 3，p. 188，推出 3)。我们已经证明了b）。

设 A 为有限次数的中心单K-代数。可以存在满足$[A : K]\not=$$[B : K] [B': K]$的半单交换子代数B（VIII、p. 269中的习题1）。

#### 定理 6 {#alg-viii-s14-thm-6 .statement tag=00GZ}

设A为中心单K-代数，B为有限次数的A的子代数，$B'$为A中的交换子。

a) 假设 B 是中心简单的。那么$B'$是中心简单，将$b\otimes b'$发送到$bb'$的K-代数同态$\theta : B\otimes_KB'\rightarrow A$是同构。

b) 假设B是半单，令$L = B\cap B'$。那么$B'$就是半单代数。 A中L的交换子$L'$为半单环和中心L，将$b\otimes b'$发送至$bb'$的环同态$\psi : B\otimes_LB'\rightarrow L'$为同构。

让我们证明a）。如果 B 是中心单形，则 $B'$ 是VIII、p. 259 的定理 5 的中心单形。因而 K-代数 $B\otimes_KB'$ 是简单的（VIII、p. 222、推出 2），同态 $\theta : B\otimes_KB'\rightarrow A$ 是单射的。现在，通过$[A : B']_s$的等式和[B : K] (定理 5)，左边的$B'$-模块$B\otimes_KB'$和A不再有相同的有限维；因而，它们是相同有限长度的 $B'$ 模块。由推论 2（共 II, §1, No. 10），第 1 页$213,\theta$ 是双射的。

让我们证明b)。到定理 5，代数 L 是可交换的，有限次数超过 K，并且半单。按地点。引用。应用于L，其A中的交换子$L'$为半单代数，L为A中$L'$的交换子，所以L为$L'$的中心。由于 L 是半单环 $L', B$ 的中心和 $B'$，因此我们可以确定 $L'$ 具有简单环 $L'_i$ 的有限乘积 （对于$i\in I$），这样我们就有

$$
L =\prod_{i\in I}L_i,B =\prod_{i\in I}B_i,B'=\prod_{i\in I}B'_i
$$

其中$L_i$是$L'_i$的中心，$B_i$和$B'_i$是$L'_i$的子代数，中心和$L_i$互为$L'_i$中彼此的交换子。我们将$L'_i$视为交换域$L_i$的中心单代数，并将$B_i$视为有限次数的中心简单$L_i$代数。通过断言a)，将$b_i\otimes b'_i$发送到$b_ib'_i$的典范映射$\psi_i: B_i\otimes_{L_i}B'_i\rightarrow L'_i$是环同构。现在，我们将可以确定 $B\otimes_LB'$ 与 $\prod_{i\in I}(B_i\otimes_{L_i}B'_i)$ 相结合，这样 $\psi$ 就是映射 $(\psi_i)_{i\in I}$ 家族的乘积。因而，$\psi$是环同构。

#### 推论 {#alg-viii-s14-n5-cor-1 .statement tag=00H0}

假设域 K 是代数闭集，并且 A 是 K 上有限次数的单代数。设 B 是 A 的单子代数，设 $B'$ 是 A 中 B 的交换子。那么 $B'$ 是单K-代数，B 是交换子 $B'$，我们有$[A : K] = [B : K][B': K]$，从$B\otimes_KB'$到A的典范同态是K-代数同构。

由于 K 上有限次数的每个单代数都是中心，推论由定理 5 和 6 得出。

### 6. 最大交换子代数

如果K-代数 A 的子代数是A 的交换子代数的集合极大元素，则我们说交换子代数是A 的最大交换子代数。

#### 引理 3 {#alg-viii-s14-lem-3 .statement tag=00H1}

设 A 为 A 的 K-代数和 L 子代数。

a) 代数 L 是 A 的最大值交换子代数当且仅当 L 等于 A 中的交换子 $L'$。

b) 设$K'$为非零的交换K-代数。那么L是A的最大值交换子代数当且仅当$L_{(K')}$是$A_{(K')}$的最大值交换子代数。

让我们证明a）。首先假设L等于$L'$。那么 L 是可交换的；如果 M 是包含 L 中的交换子代数，则 L 中的 $x$ 有 $xy=yx$，M 中有 $y$，因此有 $M\subset L'$，因而 M = L。因而，L 是 A 的最大值交换子代数。

相反，假设L是A的最大值交换子代数，并令$x$是$L'$的元素。由$L\cup  \{x\}$生成的A的子代数M则可交换并且包含L。因为 L 是最大的，所以我们有 M = L，因而 $x\in L$，最后是 $L = L'$，这给出了 a)。

根据III, §4, No. 4、p. 468的命题6，$L_{(K')}$在$A_{(K')}$中的交换子是$L'_{(K')}$。 由于等式 $L = L'$ 和 $L_{(K')}= L'_{(K')}$ 是等价的（II, §7, No. 9、p. 311、命题 19），断言 b) 由 a) 得出。

#### 命题 3 {#alg-viii-s14-prop-3 .statement tag=00H2}

设 A 为有限次数的中心单K-代数，并令 L 为 A 的半单交换子代数。以下属性是等效的：

(i) 代数 L 是 A 的最大值交换子代数。

(ii) 维数 [L : K] 的左侧L-模块 A 是自由的。

(iii) 我们有$[A : K] = [L : K]^2$。

此外，假设 A 是代数 End$_K(V)$，其中 V 是 K 上非零有限维的向量空间。那么前面的性质也等价于以下：

(iv) V 是维数 1 的免费 L 模块。

A) 假设 A 属于形式 End$_K$(V)，其中 V 是非零有限维的向量空间在域 K 上。我们将根据图表建立条件 (i) 到 (iv) 的等价

(i) $=\Rightarrow$ (iv) $=\Rightarrow$ (ii) $=\Rightarrow$ (iii) $=\Rightarrow$ (i) 。

由于L是K上有限次数的半单交换代数，我们用有限次数的K的扩张的有限乘积$\prod_{i\in I}L_i$来计算可以确定（VIII，p. 137，命题） 3）。对于每个$i\in I$，令$V_i$为L模V的型$L_i$的同型分量；它是非零有限维的向量空间超过$L_i$，因为V是忠实的L模块（VIII，p. 144，推论）。然后我们可以用$\prod_{i\in I}V_i$来认同V。在这些条件下，A中L的交换子$L'$，简单来说就是代数End$_L$(V)，可以用乘积$\prod_{i\in I}$End$_{L_i}(V_i)$来识别。

假设L是End$_K(V)$的最大值交换子代数。到引理 3, a) 时，我们有 $L = L'$，因而 $L'$ 是可交换的，并且对于每个 $i\in I$，我们都有暗淡$_{L_i}(V_i) = 1$。因而 (i) 意味着 (iv)。

假设L模V不含维数 1。令$(e_1, . . . , e_r)$为K上V的基。映射$a\mapsto (ae_1, . . . , ae_r)$为左A-模的同构，因此为L-从A到$V^r$的模块。因而，A 是维数 $r$ 的自由左L模，我们有$r=$暗淡$_K(V) = [L : K]$。因而 (iv) 意味着 (ii)。

显然，(i) 意味着(iii)。

最后，假设我们有$[A : K] = [L : K]^2$，在其他字，暗淡$_K(V) = [L : K]$。然后我们就有了 $\sum_i$ 暗淡$_{L_i}(V_i)[L_i: K] =\sum_i[L_i: K]$，因此对于每个 $i$，$V_i$ 的维数比 $L_i$ 多 1。然后，对于每个$i$，我们都有End$_{L_i}(V_i) = L_i$，所以$L'= L$。通过引理 3，a)，L 是 A 的最大值交换子代数。因而 (iii) 蕴涵 (i)。

B) 让我们继续讨论一般情况。通过VIII、p. 252的定理 1，存在有限次数的K的可分扩张$K'$，使得$K'$-代数$A_{(K')}$同构于代数End$_{K'}(V')$，其中$V'$ 是非零有限维中的向量空间超过$K'$。那么 $K'$-代数 $L_{(K')}$ 是可交换的且半单 (VIII, p. 222, 推论 2)。通过证明的第一个部分，以下属性是等效的：

(i$'$)代数$L_{(K')}$是$A_{(K')}$的最大交换子代数。

(ii$'$) 左边的$L_{(K')}$模块$A_{(K')}$是免费的，维数$[L_{(K')}: K']$。

(iii$'$) 我们有$[A_{(K')}: K'] = [L_{(K')}: K']^2$。

通过引理 3, b)，性质 (i) 和 (i’) 是等价的。

集合$n= [L : K]$；然后$n= [L_{(K')}: K']$。 性质 (ii) 表示左侧L-模A与$L^n$同构；通过VIII、p. 37的定理 3，这相当于$L_{(K')}$模块$A_{(K')}$和$(L_{(K')})^n$是同构的。 (ii) 和 (ii$'$) 的等价如下。

最后，我们有$[A : K] = [A_{(K')}: K']$和$[L : K] = [L_{(K')}: K']$，它们给出了属性(iii)和(iii$'$)的等价。这样我们就证明了性质 (i)、(ii) 和 (iii) 的等价。

#### 推论 {#alg-viii-s14-n6-cor-1 .statement tag=00H3}

设 A 为 K 上有限次数的中心单代数，并令 L 为半单交换K-代数，使得 [A : K] 等于 $[L : K]^2$。令$f$和$g$为从L到A的单同态。A存在内自同构$\theta$使得$g=\theta \circ f$。

集合$n= [L : K]$。当左模超过子环$f$(L)时，A不包含维数$n$；这是从命题的属性(ii)和(iii)的等价得出的。由于$f$是从L到$f$(L)的同构，所以左边的L-模块$A^f$（其律作用由 $(x, a)\mapsto f(x)a$ 给出）与维数 $n$ 无关。这同样适用于$A^g$，因此它与$A^f$同构的。我们对命题 1 (VIII, p. 257) 的属性 (i) 和 (ii) 利用得出等价。

假设 A 是 K 上有限次数的中心单代数。 A 可能存在不是半单且 $[A : K]\not= [L : K]^2$ (VIII, p. 270, 习题 5) 的最大值交换子代数 L。

### 7. 极大étale子代数

#### 引理 4 {#alg-viii-s14-lem-4 .statement tag=00H4}

设 A 是 K 上有限次数的中心单代数，与 K 不同。存在与 K 不同的 A 的 étale (V, §6, No. 3, p. 28, 定义 1) 子代数。

根据 Wedderburn 的定理 (VIII, p. 120, 定理 1)，我们可以假设 A 是形式 $\mathbf{M}_n$(D)，其中 $n$ 是严格的正整数，D 域与中心 K。

假设$n >1$。 K 中包含条目的对角线矩阵的代数是与 K 不同的 A 的既约子代数。

假设$n= 1$。令$p$为D的特征指数。通过VIII、p. 230的引理 1，存在D的元素$a$，使得对于任何自然数，$a^{p^m}$不会属于到K $m$。因而，对于 $m$ 足够大，元素 $x=a^{p^m}$ 在 K (V, §7, No. 7, p. 44, 命题 13) 上可分离，但它不能属于到 K。 A 的子代数 $K(x)$ 是可分扩张域 K 有限次数，因此既约子代数大于 K；它与 K 不同。

#### 命题 4 {#alg-viii-s14-prop-4 .statement tag=00H5}

令 A 为 K 上有限次数的中心单代数。令 L 为 A 的子代数，令 $L'$ 为 A 中L 的交换子。

a) 如果L是A的半单交换子代数中最大的，则我们有$L = L'$，L是A的最大交换子代数。

b) 如果L是A的既约子代数中最大的，则我们有$L = L'$，L是A的最大交换子代数。

我们知道关系$L = L'$意味着L是A的最大交换子代数（VIII，p. 261，引理3，a））。假设 L 是半单，可交换，且不同于 $L'$。到VIII的定理5时，p. 259$, L'$是半单，L是$L'$的交换子，因而$L'$的中心； consequently, $L'$ is not commutative.只要证明 A 存在半单交换子代数 M，它不同于 L 和包含 L，并且如果 L 是 étale，那么它也是 étale。

通过结构定理对于半单环（VIII，p. 135，定理1），从$L'$到$B_1\times  \cdots  \times B_r$存在简单的环$B_1, . . . ,B_r$和同构$\varphi$。对于$1\leqslant i\leqslant r$，用$E_i$表示$B_i$的中心；那么我们就有$\varphi (L) = E_1\times  \cdots  \times E_r$。由于 $L'$ 不可交换，我们可以假设 $B_1$ 不可交换；因而，我们有$B_1\not= E_1$，并且到引理 4，存在$B_1$的子代数$M_1$，它是可交换的，与$E_1$不同，并且在$E_1$之上。 集合$M =\varphi^{-1}(M_1\times E_2\times  \cdots  \times E_r)$；它是包含 L 中的半单交换子代数，与 L 不同。假设 L 是 K 上的 étale；让我们证明 M 是 étale。 K 的扩张 $E_i$ 是可分离的 (V, §6, No. 4, p. 30, 命题 3)。此外，由于$E_1$-代数$M_1$和K-代数$E_1$是étale，K-代数$M_1$也是étale（V, §6, No. 5，p. 32，推论2）。因而 K-代数 $M_1\times E_2\times  \cdots  \times E_r$ 是 étale，因而 M 也是如此。

设A是K上有限次数的中心单代数。A的半单交换子代数中最大的子代数称为A的最大半单交换子代数。通过命题4，项“最大”指的是性质可交换或半单且可交换。 A的既约子代数中最大的A的子代数称为A的极大étale子代数。

#### 推论 1 {#alg-viii-s14-prop-4-cor-1 .statement tag=00H6}

设 A 为有限次数的中心单K-代数。 A 的每个半单（分别为 étale）交换子代数都包含在 A 的最大交换子代数中，即半单（分别为 étale）。

#### 推论 2 {#alg-viii-s14-prop-4-cor-2 .statement tag=00H7}

设 D 为 K 上的有限次数的域，其中中心 K。

a) D 的极大交换子域是 D 的极大交换子代数，也是 D 的极大半单交换子代数。D 的每个可交换子域 L 都包含在极大交换子域中。

b) 令 L 为 D 的交换律子域，即 K 的可分扩张；它包含在 D 的极大交换子域中，即 K 的可分扩张中。

c) 令 L 为 D 的交换律子域。则当且仅当我们有 $[D : K] = [L : K]^2$ 时，L 为 D 的极大交换子域。

D 的子代数是域 (V, §2, No. 2, p. 10, 命题 1)，因此是半单。此外，D 包含于 K 的极大交换子域。 断言 a) 和 b) 则由推论 1 和断言 c) 的命题 3 (VIII，p. 262) 得出。

#### 命题 5 {#alg-viii-s14-prop-5 .statement tag=00H8}

设 A 为 K 上有限次数的中心单代数。设 B 为 A 的半单子代数，设 $B'$ 为 B 的交换子。

a) 代数 B 包含于 A 的最大半单交换子代数当且仅当 B 包含于 $B'$。

b) 假设 B 包含于 $B'$，并设 $g$ 为K-代数同态，从 B 到 A，存在 A 的内自同构 $\theta$，重合与 B 上的 $g$。

令L为A的最大交换子代数；除 VIII、p. 261、L 的引理 3 等于 A 中的交换子 $L'$。如果 B 包含于 L，则其交换子 $B'$ 包含在 $L'$ 中，因此也包含在 B 中。

相反，假设$B'$包含在B中。 那么$B'$就是B的中心，就是半单交换代数（VIII，p. 137，命题2）。 到推论 1 时，存在最大半单交换子代数 L 包含于 $B'$。 L的交换子等于L（VIII，p. 261，引理3，a）），$B'$的VIII，p. 259，定理5）。 因此关系$L\supset B'$意味着$L\subset B$。 我们已经证明了a）。

让我们证明b)。假设 B 包含于 $B'$，且选择 B 中包含的 A 的最大半单交换子代数 L，由 a) 存在。令$g$为从B到A的同态。通过VIII、p. 262中的命题 3，我们有等式$[A : K] = [L : K]^2$；通过VIII的推论，p. 263，存在A的内自同构$\theta_1$，即重合和L上的$g$。如果$f$是B到A中的典范嵌入，则同态$g$和$\theta_1\circ f$具有相同的B的限制到中心$B'$，因为$B'$包含在L中。由VIII、p. 256的定理2，存在A的内自同构$\theta$使得$g=\theta \circ f$；其他字、$\theta$扩展$g$。

### 8. 可对角化子代数 / 单代数

令 D 为 K-代数，即域，并令 V 为 D 上的有限维右向量空间。令 L 为 End$_D(V)$ 的 K-子代数，即可对角化的K-代数（V, §6, No. 3，p. 28）。到定义，L在K上有有限次数，并且在K上存在L的基$(\varepsilon_i)_{i\in I}$，具有以下性质：

$\varepsilon^2_i=\varepsilon_i, \varepsilon_i\varepsilon_j= 0$如果$i\not=j ,\sum_{i\in I}\varepsilon_i= 1$。

集合$V_i=\varepsilon_i(V)$对应于I中的每个$i$；那么$(V_i)_{i\in I}$是V的非零的线性子空间与直和V（II, §1, No. 8，p. 209，命题12）的族。设$u$为V中的自同态；那么$u$属于到L当且仅当对于每个$i\in I$，存在K的元素$\lambda_i$，使得对于每个$x\in V_i$有$u(x) =\lambda_ix$。

相反，假设V是非零的线性子空间的族$(V_i)_{i\in I}$的直和。对于$K^I$的任何元素$\boldsymbol{\lambda }= (\lambda_i)_{i\in I}$，用D-向量空间V的$u_{\boldsymbol{\lambda }}$自同态表示，使得$u_{\boldsymbol{\lambda }}(x) =\lambda_ix$代表$x\in V_i$。 $\boldsymbol{\lambda }\in K^I$的自同态$u_{\boldsymbol{\lambda }}$的集合L是End$_D(V)$的可对角化子代数，其中家庭$(\varepsilon_i)_{i\in I}$为基，其中$\varepsilon_i$是投影算子和像 $V_i$ 和核 $\sum_{j\not=i}V_j$。我们说L是与直和分解$V =\oplus_{i\in I}V_i$相关的End$_D(V)$的可对角化子代数。我们有 [L : K] = Card(I) $\leqslant$ 暗淡$_D(V)$。

#### 命题 6 {#alg-viii-s14-prop-6 .statement tag=00H9}

令L为与直和分解$V =\oplus_{i\in I}V_i$相关联的End$_D(V)$的可对角化子代数。

a) 代数L在K-代数End$_D(V)$的可对角化子代数中最大当且仅当每个$V_i$有维数1超过D。

b) 代数 L 是 End$_D(V)$ 的最大值交换子代数当且仅当我们有 D = K 并且每个 $V_i$ 在 K 上有维数 1。

如果每个向量空间$V_i$都有维数1超过D，那么我们有

[L : K] = 卡(I) = 暗淡$_D(V)$,

所以L是End$_D(V)$的可对角化子代数中最大的。在相反的情况下，存在指标$j\in I$使得dim$_D(V_j)\geqslant 2$。 选择两个非零的线性子空间 $V'_j$ 和$V''_j$ $V_j$ 与直和 $V_j$。 End$_D(V)$的可对角化子代数与直和分解$V = (\oplus_{i\in I-\{j\}}V_i)\oplus V'_j\oplus V''_j$包含L相关且不等于L； 断言a)如下。

End$_D(V)$中L的交换子$L'$由形式$(x_i)\mapsto (u_i(x_i))$的自同态和$(u_i)\in \prod_{i\in I}$End$_D(V_i)$组成。当且仅当我们有 $L = L'$ (VIII, p. 261, 引理 3, a)) 时，代数 L 是 End$_D(V)$ 的最大值交换子代数。因而，这个关系相当于“每$i\in$I结束$_D(V_i) = K$”； 断言 b)如下。

#### 命题 7 {#alg-viii-s14-prop-7 .statement tag=00HA}

令 L 为有限次数在 K 上的交换代数。以下属性是等效的：

(i) 代数 L 是 étale。

(ii) 存在有限次数的 K 可分扩张对角化 K。

蕴涵 (ii)$\Rightarrow$(i) 由 V, §6, No. 3、p. 29、命题 2 得出。

让我们证明蕴涵 (i)$\Rightarrow$(ii)。令Ω为K的可分闭包。由V, §6, No. 7、p. 34的定理 4，Ω中包含有限次数的K的扩张$L_1, . . . ,L_n$，使得L同构于乘积$L_1\times  \cdots  \times L_n$。令 N 为 K 的伽罗瓦扩张，包含于 $L_i$ (V, §10, No. 1, p. 58)，并证明 $L_{(N)}$ 可对角化。根据原语元素定理 (V, §7, No. 4, p. 40, 定理 1)，对于每个 $i\in [1, n]$，存在一个不可约可分多项式 $P_i\in K[X]$，使得 $L_i$ 同构于 $K[X]/(P_i)$。由于 N 是 K 的正规扩张，其中 $P_i$ 承认根，因而 N[X] 中的多项式 $P_i$ 分裂的，具有简单的根。因而，与 $N[X]/(P_i)$ 同构的 N 代数 $L_{i(N)}$ 也与 $N^{[L_i:K]}$ 同构。因而 $L_{(N)}$ 是可对角化的。

#### 定理 7 {#alg-viii-s14-thm-7 .statement tag=00HB}

设 A 为有限次数的中心单K-代数和 A 的 L 子代数。以下属性是等效的：

(i) 代数 L 是 A 的极大étale子代数。

(ii) K 存在扩张 $K'$、整数 $n\geqslant 1$、以及从$A_{(K')}$到$\mathbf{M}_n(K')$的同构$\theta$，将$L_{(K')}$发送到集合对角线矩阵。

(iii) 存在如(ii)中那样的$K',n$和$\theta$，其中扩张$K'$此外是假定的伽罗瓦和有限次数。

显然，(iii) 暗示着(ii)。

如果性质 (ii) 成立，则 $L_{(K')}$ 是 $A_{(K')}$ (命题 6) 的最大值交换子代数，且可对角化。 K-代数 L 则为 étale (V, §6, No. 3, p. 28, 定义 1)，并且它是 A 的最大交换子代数 (VIII, p. 261, 引理 3, b))。我们已经证明(ii)蕴涵(i)。

假设性质 (i) 成立。由于L是K上的étale，到命题7，存在有限次数的K的伽罗瓦扩张$K_1$，使得$K_1$-代数$L_{(K_1)}$可对角化的。 代数 A 是中心简单；由(VIII，p. 252，定理1)，$K_2$上存在有限维$n$的伽罗瓦扩张$K_2$，向量空间V，以及同构 $\theta$从$A_{(K_2)}$到结束$_{K_2}(V)$。通过V、p. 55的命题 1，我们可以假设$K_1= K_2$。由VIII、p. 264的命题4、b)和VIII的引理3、b)，p. 261$, L_{(K')}$是$A_{(K')}$的最大交换子代数，所以$\theta (L_{(K')})$是最大结束$_{K'}(V')$的交换子代数。让我们应用命题 6 到可对角化代数 $\theta (L_{(K')}):$，在 $K'$ 上存在 $V'$ 的基 $(e_1, . . . , e_n)$，使得 $\theta (L_{(K')})$ 由 $V'$ 的自同态和对角矩阵组成关于这个基。因此 (i) 意味着 (iii)。

### 习题{#alg-viii-s14-exercises}

参见[习题为 § 14](exercises/s14/)。
