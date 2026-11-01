---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 2
section_title: A connectedness property
appendix: true
lang: zh
source: lie-vii-ix
book_pages: 48-49, 67
pdf_pages: 0058-0059, 0076-0076
extraction: native
statements: 3
exercises: 2
content_sha256: e9a1e159856fe9b53930c5cd884e0987ab14aba0ef9a81d289e5db16bf9e8e83
translated_from: content/en/lie/VII/A2_a2_a_connectedness_property.md
translation_method: google
source_content_sha256: e52c40721671251b25cbd21bd6c6376bf20e17aa16de77c1b806f74183e1c74a
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 14b0871249455cad8117d6ad0eb4c97fc6322bb62b6a5ff240543b5c4d7f94c2
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 附录 II 一个连通性质

#### 引理 1 {#lie-vii-a2-lem-1 .statement tag=00XN}

令X为连通拓扑空间，$\Omega$为X的稠密开子集。如果对于任意$x\in X$，存在$x$的邻域V使得$V\cap \Omega$连通，则$\Omega$连通。

事实上，让$\Omega_0$是$\Omega$的非空开闭子集。令 $x\in X$ 且令 V 为 $x$ 的邻域，使得 $V\cap \Omega$ 相连。如果$x\in \overline{\Omega}_0$，

$$
(V\cap \Omega )\cap \Omega_0= V\cap \Omega_0\not=\emptyset
$$

所以$V\cap \Omega \subset \Omega_0$。因而，由于$\Omega$在$X,\overline{\Omega}_0$中是稠密的，因此邻域是$x$。因而，$\Omega_0$非空、开闭，并且由于X是连通的，因而$\overline{\Omega}_0= X$。由于$\Omega_0$在$\Omega$中是闭合的，这意味着$\Omega_0=\Omega \cap \overline{\Omega}_0=\Omega$，从而证明$\Omega$是连通的。

#### 引理 2 {#lie-vii-a2-lem-2 .statement tag=00XO}

设 U 为 $\mathbf{C}^n$ 中的开球，$f: U\rightarrow \mathbf{C}$ 为全纯函数，但与零不同。设 A 为 U 的子集，使得 A 上的 $f= 0$。则 U **--** A 在 U 中稠密且连通。

U**--** A 的密度由可微分和解析流形，结果，3.2.5 得出。首先假设$n= 1$。如果$f$的$a\in A$，幂级数展开关于$a($可微分和解析流形，结果，3.2.1）不减少到0，则存在邻域$V_a$ $a$ 在 U 中，使得 $f$ 不会在 $V_a$ **--** $\{a\}$ 上消失。因而，$a$在A中是孤立的，这证明A是U的离散子集，因此可数，因为U在无穷大是可数的。令 $x, y\in U$ **--** A. 连接 $x$（分别为 $y$）到 A 的点的实仿射线的并是微不足道的（一般拓扑，第 IX, §5, no. 2，定义 2）。因而，存在 $z\in U$ **--** A，使得段 $[x, z]$ 和 $[y, z]$ 都不满足 A。 点 $x, y, z$ 因此属于与 U **--** A 的相同连通分量，这证明了在这种情况下的引理 $n= 1$。我们转向一般情况。我们可以假设A是$f($一般拓扑的零的集合，第1章。 I, §11, no. 1，提案 1)。设 $x, y\in U$**--** A 并设 L 为仿射线包含 $x$ 和 $y$。自$x\in L\cap U$以来，$f$到$L\cap U$的限制与零不相同。通过已经证明的，$x$和$y$属于到$(L\cap U)$**--**$(L\cap A)$的同一个连通分量，因此到U**--**A的同一个连通分量。

#### 引理 3 {#lie-vii-a2-lem-3 .statement tag=00XP}

令X为有限维连通复解析流形，并令A为X满足以下条件的子集：

对于任何$x\in X$，都存在一个解析的函数胚芽$f_x$，并且不会消失

在$x$处，使得$x$处的A的胚芽包含在集合处的$x$处的胚芽中

零 $f_x$。

那么 X **--** A 在 X 中是密集的并且是连通的。

密度 of X**--** A 由可微分和解析流形，结果，3.2.5 得出。我们可以假设 A 是封闭的（通则拓扑，第 I, §11, no. 1 章，命题 1）。对于任何$x\in X$，存在$x$的开邻域V和同构$c$，从V到$\mathbf{C}^n$中的开球，使得$c(A\cap V)$包含在a的零的集合中全纯函数与$c(V)$ 上的零不相同。然后，通过引理 $2, V\cap (X$ **--** A) 连接起来。鉴于引理 1，这证明X **--** A 是连通的。

### 习题 {#lie-vii-a2-exercises}

参见[习题附录 2](exercises/a2/)。
