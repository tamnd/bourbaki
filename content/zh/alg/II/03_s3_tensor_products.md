---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 3
section_title: Tensor products
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 243-266, 395-396
pdf_pages: 0267-0290, 0419-0420
extraction: ocr
subsections:
    - "no": 1
      title: TENSOR PRODUCT OF TWO MODULES
      page: 243
      pdf_page: 267
    - "no": 2
      title: TENSOR PRODUCT OF TWO LINEAR MAPPINGS
      page: 245
      pdf_page: 269
    - "no": 3
      title: CHANGE OF RING
      page: 246
      pdf_page: 270
    - "no": 4
      title: OPERATORS ON A TENSOR PRODUCT; TENSOR PRODUCTS AS MULTIMODULES
      page: 247
      pdf_page: 271
    - "no": 5
      title: TENSOR PRODUCT OF TWO MODULES OVER A COMMUTATIVE RING
      page: 249
      pdf_page: 273
    - "no": 6
      title: PROPERTIES OF $E \otimes_A F$ RELATIVE TO EXACT SEQUENCES
      page: 251
      pdf_page: 275
    - "no": 7
      title: TENSOR PRODUCTS OF PRODUCTS AND DIRECT SUMS
      page: 254
      pdf_page: 278
    - "no": 8
      title: ASSOCIATIVITY OF THE TENSOR PRODUCT
      page: 258
      pdf_page: 282
    - "no": 9
      title: TENSOR PRODUCT OF FAMILIES OF MULTIMODULES
      page: 259
      pdf_page: 283
statements: 30
exercises: 4
content_sha256: bfd5c8169856c14036635c784ad78101e3f4d70af598b25058dad09a4e16ad11
translated_from: content/en/alg/II/03_s3_tensor_products.md
translation_method: google
source_content_sha256: 4cc4310afca7381c71a95e1a30d8b454ee7692d8209261c6a3c8ad67f1781a39
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: af4967ecdb818b0da9668219a102b6b4ced0411ff45b401ebcc3887a12b182ef
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 3。 张量积

### 1. 张量积两个模

令$G_1, G_2$为两个$\mathbf{Z}$模块；如果 $u(x_1, x_2)$ 是“相对于 $x_1$ 和$x_2$ 的可加性”，则将集合 $G = G_1 \times G_2$ 的映射 $u$ 转换为 $\mathbf{Z}$ 模，称为双向可加性（或$\mathbf{Z}$-双线性）；准确地说，这意味着，对于$G_1$中的$x_1, y_1$，$G_2$中的$x_2, y_2$，

$$
u(x_1 + y_1, x_2) = u(x_1, x_2) + u(y_1, x_2)
$$
$$
u(x_1, x_2 + y_2) = u(x_1, x_2) + u(x_1, y_2).
$$

注这特别意味着 $u(0, x_2) = u(x_1, 0) = 0$ 对于所有 $x_1 \in G_1, x_2 \in G_2$。

设 A 为环，E 右A-模，F 左A-模。我们将考虑普遍映射问题（集合理论，IV, § 3, no. 1），其中$\Sigma$是$\mathbf{Z}$模块结构的类（态射则为$\mathbf{Z}$线性映射，在其他字中， 加法群同态），$\alpha$-映射是$E \times F$的映射$f$到$\mathbf{Z}$-模块G，其是$\mathbf{Z}$双线性，进一步满足，对于所有$x \in E, y \in F$和$\lambda \in A$

$$(1)$$
$$
f(x \lambda, y) = f(x, \lambda y).
$$

我们证明这个问题承认解。为此，我们考虑$E \times F$的元素的形式线性组合的$\mathbf{Z}$-模块$C = \mathbf{Z}^{(E \times F)}$，其系数为$\mathbf{Z}$（§ 1, no. 11），其中基可以被认为由有序对$(x, y)$组成，其中$x \in E$ 和 $y \in F$。令 D 为由以下型之一的元素生成的 C 的子$\mathbf{Z}$模块：

$$(2)$$
$$
\begin{cases}
(x_1 + x_2, y) - (x_1, y) - (x_2, y) \\
(x, y_1 + y_2) - (x, y_1) - (x, y_2) \\
(x \lambda, y) - (x, \lambda y)
\end{cases}
$$

其中$x, x_1, x_2$在$E$中，$y, y_1, y_2$在$F$中，$\lambda$在$A$中。

#### 定义 1 {#alg-ii-s3-def-1 .statement tag=05OR}

* 右A-模 E 和左A-模 F* 的张量积，用 $E \otimes_A F$ 或 $E \otimes_A F$ 表示（如果不用担心混淆，则简单地用 $E \otimes F$ 表示） * 是商 $\mathbf{Z}$-模* $C/D$（$\mathbf{Z}$-模 C 的商） $E \times F$的元素的正式线性组合的系数在$\mathbf{Z}$中，由型(2))之一的元素生成子模$D$。 *对于$x \in E$和$y \in F$，$E \otimes_A F$的元素即元素的典范像，$C = \mathbf{Z}^{(E \times F)}$的$(x, y)$记为$x \otimes y$，称为$x$的张量积， $y$。

$E \times F$到$E \otimes_A F$的映射$(x, y) \mapsto x \otimes y$被称为*规范*。它是满足条件 (1) 的 $\mathbf{Z}$ 双线性映射。

我们展示了张量积$E \otimes_A F$和上面普遍映射问题的典范映射形式解较早摆出的姿势。准确地说：

#### 命题 1 {#alg-ii-s3-prop-1 .statement tag=05OS}

(a) *令$g$为$E \otimes_A F$到$\mathbf{Z}$模块$G$的$\mathbf{Z}$线性映射。 $E \times F$到$G$的映射$(x, y) \mapsto f(x, y) = g(x \otimes y)$是$\mathbf{Z}$双线性并且满足条件(1)。*

(b) *相反，令$f$是$E \times F$到$\mathbf{Z}$-模块$G$满足条件的$\mathbf{Z}$双线性映射 (1)。那么存在且仅有一个 $\mathbf{Z}$-线性映射 $g$ 将 $E \otimes_A F$ 映射到$G$，使得 $f(x, y) = g(x \otimes y)$ 对应于 $x \in E, y \in F$。*

如果$\phi$将$E \times F$的典范映射代入$E \otimes_A F$，则$f = g \circ \phi$； 从而（一）。为了证明（b），我们注，在定义 1的记号中，$f$扩展到$C$的$\mathbf{Z}$线性映射$\bar{f}$到$G$（§ 1, no. 11，命题） 17）。根据关系 (1)，对于型 (2) 之一的 $C$ 的所有元素，$\bar{f}$ 为零，因此在 $D$ 上。因此，存在$C/D = E \otimes_A F$到$G$的$\mathbf{Z}$线性映射$g$，使得$\bar{f} = g \circ \psi$，其中$\psi : C \to C/D$是典范同态（§ 1, no. 8，*注*）。 $g$的唯一性是直接的，因为$E \otimes_A F$是由形式$x \otimes y$的元素生成为$\mathbf{Z}$模块。

将$\mathbf{Z}$的$\mathbf{Z}$模块的命题 1 定义a *典范同构*将$E \times F$的$f$映射到$G$、满足条件 (1)， $\mathbf{Z}$-模块$\mathrm{Hom}_{\mathbf{Z}}(E \otimes_A F, G)$。

当$A = \mathbf{Z}$、条件(1)自动满足*每个*$\mathbf{Z}$双线性映射$f$和$C$的子模$D$已经由(2)中前两个型的元素生成。

如果现在我们回到一般情况，$E'$和$F'$分别表示$E$和$F$的底层$\mathbf{Z}$模块，则上面的注和定义1立即表明$\mathbf{Z}$模块$E \otimes_A F$可以是由形式$(x \lambda) \otimes y - x \otimes (\lambda y)$的元素生成的子$\mathbf{Z}$模块，以$\mathbf{Z}$模块$E' \otimes_{\mathbf{Z}} F'$的*商*规范地标识，其中$x$贯穿$E$，$y$贯穿$F$和$\lambda$贯穿$A$。

#### 推论 1 {#alg-ii-s3-prop-1-cor-1 .statement tag=05OT}

*令$H$为$\mathbf{Z}$模，$h : E \times F \to H$为$\mathbf{Z}$双线性映射满足条件 (1)，使得$H$由$h(E \times F)$生成。假设对于每个$\mathbf{Z}$-模块$G$和$E \times F$的每个$\mathbf{Z}$双线性映射$f$到$G$满足(1)*，存在一个$\mathbf{Z}$线性映射$g : H \to G$使得$f = g \circ h$。那么，如果$\phi$将$E \times F$的典范映射表示为$E \otimes_A F$，则存在且仅有一个$E \otimes_A F$的同构$\theta$到$H$使得$h = \theta \circ \phi$。

假设 $h(E \times F)$ 生成 $H$ 意味着 $g$ 的唯一性；那么推论就是解普遍映射问题的一般唯一性性质（集合理论，IV, § 3, no. 1）。

#### 推论 2 {#alg-ii-s3-prop-1-cor-2 .statement tag=05OU}

*令* $E^0$（分别$F^0$）*表示模* $E$（分别$F$）*视为左（或右）模超过逆环* $A^0$； *则存在一个且仅有一个* $\mathbf{Z}$*-模块同构* $\sigma : E \otimes_A F \to F^0 \otimes_{A^0} E^0$ *使得* $\sigma(x \otimes y) = y \otimes x$ *对于* $x \in E$ *和* $y \in F$（张量积的“交换律”）。

由$E^0$和$F^0$上的$A^0$模结构的定义，$E \times F$的映射$(x, y) \mapsto y \otimes x$进入$F^0 \otimes_{A^0} E^0$是$\mathbf{Z}$双线性且满足条件(1)， 从而$\mathbf{Z}$-线性映射$\sigma$的存在性和唯一性。类似地，$\mathbf{Z}$-线性映射$\tau : F^0 \otimes_{A^0} E^0 \to E \otimes_A F$被定义为使得$\tau(y \otimes x) = x \otimes y$并且显然$\sigma$和$\tau$是逆同构。

#### 注 {#alg-ii-s3-n1-rem-1 .statement tag=05OV}

非零模的张量积可能是零：对于例，对所有$x \in E$取两个$\mathbf{Z}$模$E = \mathbf{Z}/2\mathbf{Z}$和$F = \mathbf{Z}/3\mathbf{Z}$，$2x = 0$和$3y = 0$， $y \in F$；因此，在$E \otimes_{\mathbf{Z}} F$中，
$$
x \otimes y = 3(x \otimes y) - 2(x \otimes y) = x \otimes (3y) - (2x) \otimes y = 0
$$
对于所有 $x$ 和 $y$（cf. no. 6，推论 4 到命题 6）。

### 2. 张量积两个线性映射

令$A$为环、$E, E'$两个右$A$模块、$F, F'$两个左$A$模块以及$u : E \to E'$和$v : F \to F'$两个$A$线性映射。很容易验证映射
$$
(x, y) \mapsto u(x) \otimes v(y)
$$
$E \times F$ 到 $E' \oplus_A F'$ 是 $\mathbf{Z}$ 双线性，且满足 no. 1 的条件 (1)。因此，通过 no. 1 的命题 1，存在一个且仅有一个$\mathbf{Z}$-线性映射$w : E \otimes_A F \to E' \otimes_A F'$，使得
$$
w(x \otimes y) = u(x) \otimes v(y)
$$
$x \in E, y \in F$。这个映射用$u \otimes v$表示（当不会引起混淆时），称为线性映射$u$和$v$的*张量积*。

从 (3) 可以立即得出，$(u, v) \mapsto u \otimes v$ 是一个 $\mathbf{Z}\text{-bilinear}$ 映射，称为*规范*
$$
\operatorname{Hom}_A(E, E') \times \operatorname{Hom}_A(F, F') \to \operatorname{Hom}_{\mathbf{Z}}(E \otimes_A F, E' \otimes_A F').
$$

通过 no. 1 的命题 1 到它有对应一个 $\mathbf{Z}$ 线性映射，称为规范

(4) $$
\operatorname{Hom}_A(E, E') \otimes_{\mathbf{Z}} \operatorname{Hom}_A(F, F') \to \operatorname{Hom}_{\mathbf{Z}}(E \otimes_A F, E' \otimes_A F')
$$
与张量积线性映射$u \otimes v : E \otimes_A F \to E' \otimes_A F'$中的每个元素$u \otimes v$相关联。 注典范映射 (4) *不一定是单射或满射*。因此，记号$u \otimes v$可能会导致混淆，因此有必要根据上下文指示它是否表示元素或张量积或线性映射。

进一步，设$E''$为右$A$模，$F''$为左$A$模，$u' : E' \to E''$、$v' : F' \to F''$$A$线性映射；由(3)可知
(5)
$$
(u' \circ u) \otimes (v' \circ v) = (u' \otimes v') \circ (u \otimes v).
$$

### 3. 变换的环

#### 命题 2 {#alg-ii-s3-prop-2 .statement tag=05OW}

*令$A, B$为两个环、$\rho : B \to A$、环、同态和$E$（分别为$F$）右（分别为左）$A$模块。 Then there exists one and only one $\mathbf{Z}$-linear mapping*
(6)
$$
\phi : \rho_*(E) \otimes_B \rho_*(F) \to E \otimes_A F
$$
*such that, for all $x \in E$ and $y \in F$, the image under $\phi$ of the element $x \otimes y$ of $\rho_*(E) \otimes_B \rho_*(F)$ is the element $x \otimes y$ of $E \otimes_A F$; this $\mathbf{Z}$-linear mapping is surjective.*

我们将$\rho_*(E) \times \rho_*(F)$的映射$(x, y) \mapsto x \otimes y$考虑为$E \otimes_A F$；它是$\mathbf{Z}$双线性的，并且对于所有$\beta \in B$，通过定义$(x \rho(\beta)) \otimes y = x \otimes (\rho(\beta)y)$，因此no. 1的条件（1）成立，从而$\phi$的存在和唯一性（no. 1， 命题1)。后者断言源自元素$x \otimes y$生成$\mathbf{Z}$模块$E \otimes_A F$。

映射 (6) 被称为*规范*。

#### 推论{#alg-ii-s3-n3-cor-1 .statement tag=05OX}

*令$\mathfrak{J}$为$A$的双面理想，使得$\mathfrak{J}$包含在$E$的湮没子和$F$的湮没子中，因此$E$（或$F$）具有规范左（或右） $(A/\mathfrak{J})$-模块结构*（$§ 1$，no. 12）。 *然后典范同态* (6)
$$
\phi : E \otimes_A F \to E \otimes_{A/\mathfrak{J}} F
$$
*相应的到典范同态$\rho : A \to A/\mathfrak{J}$是身份。*

对于所有$\bar{\alpha} \in A/\mathfrak{J}$，所有$x \in E$和所有$y \in F$，$x \bar{\alpha} = x \alpha$（分别为$\bar{\alpha} y = \alpha y$）对于所有$\alpha$，使得$\rho(\alpha) = \bar{\alpha}$。如果$C = \mathbf{Z}^{(E \times F)}$，元素$(x \alpha, y) - (x, \alpha y)$生成的$C$的子模则等于元素$(x \bar{\alpha}, y) - (x, \bar{\alpha} y)$生成的子模。

根据命题 2 的假设和记号，令$E'$ 为右$B$ 模，$F'$ 为左$B$ 模，并考虑两个*半线性* 映射 $u : E' \to E$，v:F' \to F 相对于同态$\rho : B \to A$； $u$（分别$v$）可以被视为$B$线性映射$E' \to \rho_*(E)$（分别$F' \to \rho_*(F')$），从而一个$\mathbf{Z}$线性映射$w : E' \otimes_B F' \to \rho_*(E) \otimes_B \rho_*(F)$，使得$w(x' \otimes y') = u(x') \otimes v(y')$对应于$x' \in E',\ y' \in F'$；将典范映射 (6) 与映射组合，从而获得$\mathbf{Z}$-线性映射$w' : E' \otimes_B F' \to E \otimes_A F$，使得$w'(x' \otimes y') = u(x') \otimes v(y')$ 对于$x' \in E',\ y' \in F'$；这是映射，如果不会引起混淆，通常用 $u \otimes v$ 表示。显然 $(u, v) \mapsto u \otimes v$ 是 $\mathbf{Z}$ 双线性映射

$$
\operatorname{Hom}_B(E', \rho_*(E)) \times \operatorname{Hom}_B(F', \rho_*(F)) \to \operatorname{Hom}_\mathbf{Z}(E' \otimes_B F', E \otimes_A F).
$$

此外，如果$C$是第三个环，$\sigma : C \to B$同态，$E''$右$C$模块，$F''$左$C$模块，$u' : E'' \to E'$和$v' : F'' \to F'$相对于的半线性映射$\sigma$，那么

$$
(u \circ u') \otimes (v \circ v') = (u \otimes v) \circ (u' \otimes v').
$$

### 4. 张量积上的操作员； 张量积作为多模块

根据假设和no. 1的记号，对于$A$-模块$E$（或$F$）的每个自同态$u$（或$v$），$u \otimes 1_F$（或$1_E \otimes v$）为$\mathbf{Z}$模块$E \otimes_A F$的自同态；从 (5) (no. 2) 可以立即得出，映射 $u \mapsto u \otimes 1_F$（分别为 $v \mapsto 1_E \otimes v$）是 *环同态*

$$
\operatorname{End}_A(E) \to \operatorname{End}_\mathbf{Z}(E \otimes_A F)
$$

（分别$\operatorname{End}_A(F) \to \operatorname{End}_\mathbf{Z}(E \otimes_A F)$）；此外，

$$
(u \otimes 1_F) \circ (1_E \otimes v) = (1_E \otimes v) \circ (u \otimes 1_F) = u \otimes v
$$

因此 (§ 1, no. 14) $E \otimes_A F$ 相对于环 $\operatorname{End}_A(E)$ 和 $\operatorname{End}_A(F)$ 具有规范的 *left 双模* 结构。

既然如此，假设在 $E$ 上给出一个 $((B'_i); A, (C'_j))$-多模块结构和在 $F$ 上给出一个 $(A, (B''_h); (C''_{k_c}))$-多模块结构 (§ 1, no. 14)；这相当于说环同态 $B'_i \to \operatorname{End}_A(E)$、$C'_j{}^0 \to \operatorname{End}_A(E)$ 是用成对可置换像给出的，环同态 $B''_h \to \operatorname{End}_A(F)$、$C''_{k_c}{}^0 \to \operatorname{End}_A(F)$ 是用成对可置换像给出的。如果这些同态分别与上面定义的典范同态、$\operatorname{End}_A(E) \to \operatorname{End}_\mathbf{Z}(E \otimes_A F)$和$\operatorname{End}_A(F) \to \operatorname{End}_\mathbf{Z}(E \otimes_A F)$组成，可以看出（考虑（7））环同态

$$
\begin{align*}
B'_i &\to \operatorname{End}_\mathbf{Z}(E \otimes_A F), & C'_j{}^0 &\to \operatorname{End}_\mathbf{Z}(E \otimes_A F) \\
B''_h &\to \operatorname{End}_\mathbf{Z}(E \otimes_A F), & C''_{k_c}{}^0 &\to \operatorname{End}_\mathbf{Z}(E \otimes_A F)
\end{align*}
$$

定义为 *pairwise permutable* 像；在其他字中，$E \otimes_A F$上定义了一个$((B'_i), (B''_h); (C'_j), (C''_{k_c}))$-多模块结构；正是这个多模块也被称为*张量积*（相对于$A$）*

((B'_i); A, (C'_j))-多模块 E 和 (A, (B''_h); (C''_k))-多模块 F。该多模块是普遍映射问题的解，类似于 no. 1 中考虑的；准确地说：

#### 命题 3 {#alg-ii-s3-prop-3 .statement tag=05OY}

令 G 为 ((B'_i), (B''_h); (C'_j), (C''_k))-多模块。

(a) 设 g 为多模 E $\otimes_A$ F 到 G 的线性映射。E $\times$ F 到 G 的映射 $f : (x, y) \mapsto g(x \otimes y)$ 是 $\mathbf{Z}$ 双线性，并且满足 no. 1 和条件的关系 (1)

$$
\begin{cases}
f(\mu'_i x, y) = \mu'_i f(x, y), & f(x v'_j, y) = f(x, y) v'_j \\
f(x, \mu''_h y) = \mu''_h f(x, y), & f(x, y v''_k) = f(x, y) v''_k
\end{cases}
$$

对于所有 $x \in E, y \in F, \mu'_i \in B'_i, v'_j \in C'_j, \mu''_h \in B''_h, v''_k \in C''_k, i, j, h, k$ 任意。

(b) 相反，令 f 为 E $\times$ F 到 G 满足条件 (1) (no. 1) 和 (8) 的 $\mathbf{Z}$ 双线性映射。则多模 E $\otimes_A$ F 中存在且仅有一个线性映射 g 进入多模 G，使得 $f(x, y) = g(x \otimes y)$ 对应 $x \in E, y \in F$。

断言 (a) 紧跟在 E $\otimes_A$ F 上多模块结构的定义之后，因为对于例 $(x \otimes y)v'_j = (xv'_j) \otimes y$。为了证明(b)，我们首先注no. 1的命题1给出$\mathbf{Z}$线性映射g的存在性和唯一性，使得$g(x \otimes y) = f(x, y)$对于$x \in E, y \in F$；所需要做的只是验证 g 对于多模结构是线性的。作为元素 $x \otimes y$ 生成 $\mathbf{Z}$-模块 E $\otimes_A$ F，足以验证关系 $g(\mu'(x \otimes y)) = \mu'_i g(x \otimes y)$ 及其类似物；但这是紧随公式$g(x \otimes y) = f(x, y)$和关系（8）而来的。

#### 学院{#alg-ii-s3-n4-sch-1 .statement tag=05OZ}

E $\otimes_A$ F 的元素通常可以用多种方式写成形式 $\sum_i (x_i \otimes y_i)$，其中 $x_i \in E$ 和 $y_i \in F$；但要将多模E $\otimes_A$ F 的定义线性映射 g 转化为多模G，则无需验证，如果$\sum_i (x_i \otimes y_i) = \sum_j (x'_j \otimes y'_j)$，则$\sum_i g(x_i \otimes y_i) = \sum_j g(x'_j \otimes y'_j)$；对于$x \in E$和$y \in F$给出$g(x \otimes y)$就足够了，并且验证$(x, y) \mapsto g(x \otimes y)$是$\mathbf{Z}$双线性并且满足条件(1)(no. 1)和(8)。

令 E' 为 ((B'_i), A, (C'_j))-多模块，F' 为 (A, (B''_h); (C''_k))-多模块，且多模块的 $u : E \to E', v : F \to F'$ 线性映射；紧接着从定义 (no. 2) 可以得出，$u \otimes v$ 是多模块 E $\otimes_A$ F 的线性映射到多模块 E' $\otimes_A$ F'。

由于 E 始终表示右A-模，令 $_sA_d$ 表示环 A 被视为 (A, A)-双模 (§ 1, no. 14, 例 1)；由上可知，张量积 E $\otimes_A (_sA_d)$ 具有规范的右A-模结构，使得 $(x \otimes \lambda)\mu = x \otimes (\lambda \mu)$ 对应 $x \in E, \lambda \in A, \mu \in A$。 E $\times (_sA_d)$ 到 E 的映射 $(x, \lambda) \mapsto x \lambda$ 是 $\mathbf{Z}$ 双线性，并且满足条件 (1) (no. 1) 和 (8) （其中，在后者中，$B'_i, C'_j$ 和 $B''_h$ 不存在，族 $(C''_k)$ 约化至$A$）；因此（命题 3），存在$E \otimes_A (sA_d)$到$E$的$A$线性映射$g$（称为规范），使得$g(x \otimes \lambda) = x\lambda$对应于$x \in E, \lambda \in A$。

#### 命题 4 {#alg-ii-s3-prop-4 .statement tag=05P0}

*如果$E$是右$A$-模块，$E$到$E \otimes_A (sA_d)$的映射$h : x \mapsto x \otimes 1$是右$A$-模块同构，其逆同构$g$是这样的$g(x \otimes \lambda) = x\lambda$ $x \in E, \lambda \in A$。*

如果 $g$ 为典范映射，$g \circ h$ 为恒等映射 $1_E$，并且 $h \circ g$ 重合与 $E \otimes_A (sA_d)$ 的恒等映射自身相加，为形式的元素 $x \otimes y$，其中生成后者$\mathbf{Z}$-模块；因此得出结论。

我们通常会写$E \otimes_A A$而不是$E \otimes_A (sA_d)$，并且经常通过上面的典范同构来写认同$E \otimes_A A$和$E$。观察到，如果$E$也有一个（左或右）$B$-模块结构与其右$A$-模块结构兼容，则对于$E$和$E \otimes_A A$上的$B$-模块结构，$g$和$h$也是同构（因此是多节点） 模同构）。

现在让 $F$ 成为左 $A$ 模块； $(sA_d) \otimes_A F$（也由$A \otimes_A F$表示）则具有规范的左$A$模块结构，如命题 4 典范同构所示，将$A \otimes_A F$定义到$F$ 映射 $\lambda \otimes x$ $\lambda x$，其逆同构为$x \mapsto 1 \otimes x$。

特别地，存在$(A, A)$双模$(sA_d) \otimes_A (sA_d)$到$sA_d$的典范同构，其中映射$\lambda \otimes \mu$到$\lambda \mu$。

### 5. 两个模超过交换环中的张量积

设 $C$ 是一个*可交换的* 环；对于每个$C$-模块$E$，$E$上的模结构*与其自身兼容*（§ 1, no. 14）。如果$E$和$F$是两个$C$模块，则no. 4的考虑允许我们在张量积和$E \otimes_C F$上分别构建定义*两个*$C$模块结构，使得$\gamma(x \otimes y) = (\gamma x) \otimes y$和这样$\gamma(x \otimes y) = x \otimes (\gamma y)$；但是，通过 no. 1 的定义 1，在本例中为 $(\gamma x) \otimes y = x \otimes (\gamma y)$，这两个结构 *相同*。从此以后，当我们将 $E \otimes_C F$ 称为 $C$-*模* 时，我们将指的是如此定义的结构，否则将说明除非。 典范同构。

$$
\sigma : F \otimes_C E \to E \otimes_C F
$$

（no. 1，推论 2 到命题 1）则为$C$-模块同构。

由此定义可以得出，如果$(a_\lambda)_{\lambda \in L}$（或$(b_\mu)_{\mu \in M}$）是$C$模块$E$（或$F$）的*生成的系统*，则$(a_\lambda \otimes b_\mu)$是*生成的 $C$模块$E \otimes_C F$的系统*；特别是，如果$E$和$F$是*有限生成的*$C$模块，那么$E \otimes_C F$也是。

对于每个$C$-模块$G$，$E \times F$的$\mathbf{Z}$双线性映射$f$到$G$，其中

$$
f(\gamma x, y) = f(x, \gamma y) = \gamma f(x, y) \quad \text{for } x \in E, y \in F, \gamma \in C
$$

则称为 C-双线性，形式 C-模表示为 $\mathscr{L}_2(E, F; G)$； 命题 3 (no. 4) 定义一个规范的 C-模同构 (cf. § 1, no. 14, 注 1)。

$$
\mathscr{L}_2(E, F; G) \to \mathrm{Hom}_C(E \otimes_C F, G).
$$

令E'，F'为两个C-模和$u : E \to E'$，$v : F \to F'$两个C线性映射；那么 (no. 4) $u \otimes v$ 是 $E \otimes_C F$ 到 $E' \otimes_C F'$ 的 C 线性映射。进一步地，$(u, v) \mapsto u \otimes v$是$\mathrm{Hom}_C(E, E') \times \mathrm{Hom}_C(F, F')$到$\mathrm{Hom}_C(E \otimes_C F, E' \otimes_C F')$的C双线性映射，直接的；因此，它有一个规范的对应 C 线性映射，称为规范：

$$
\mathrm{Hom}_C(E, E') \otimes_C \mathrm{Hom}_C(F, F') \to \mathrm{Hom}_C(E \otimes_C F, E' \otimes_C F')
$$

与张量积中的每一个元素 $u \otimes v$ 相关联

$$
\mathrm{Hom}_C(E, E') \otimes_C \mathrm{Hom}_C(F, F')
$$

线性映射$u \otimes v$。 注典范映射 (11) *不一定是单射或满射*（§ 4，习题 2）。

#### 注 {#alg-ii-s3-n5-rem-1 .statement tag=05P1}

(1) 设A、B为两个交换环、$\rho : B \to A$环同态，E、F为两个A-模；那么no. 3的典范映射(6)是B-线性映射

$$
\rho_*(E) \otimes \rho_*(F) \to \rho_*(E \otimes_A F).
$$

(2) 本号中所说的内容。可以推广到以下情况：设 E 为 C 的右A-模、F 左A-模、C 交换环和 $\rho : C \to A$ 同态到 A 中，使得 $\rho(C)$ 包含在 A 的中心中（cf. III, § 1, no. 3）。然后我们可以认为$\rho$上的C-模$\rho_*(E)$和$\rho_*(F)$和假设意味着这些C-模结构分别与E和F（§ 1, no. 14）上的A-模结构兼容。因此，张量积$E \otimes_A F$（凭借no. 4）给出两个C-模结构，使得$\gamma(x \otimes y) = (x \rho(\gamma)) \otimes y$和

$$
\gamma(x \otimes y) = x \otimes (\rho(\gamma)y)
$$

分别对于 $\gamma \in C$、$x \in E$、$y \in F$ 和定义 1 (no. 1) 也表明这两个结构是相同的。如果 E'（或 F'）是右（或左）A-模且 $u : E \to E'$、$v : F \to F'$ 是两个 A-线性映射，则 $u \otimes v : E \otimes_A F \to E' \otimes_A F'$ 对于刚刚定义的 C-模结构是 C 线性的； 映射$(u, v) \mapsto u \otimes v$：

$$
\mathrm{Hom}_A(E, E') \times \mathrm{Hom}_A(F, F') \to \mathrm{Hom}_C(E \otimes_A F, E' \otimes_A F')
$$

是 C-双线性（对于 $\mathrm{Hom}_A(E, E')$ 和 $\mathrm{Hom}_A(F, F')$ 上的 C-模结构）在 § 1, no. 14、*注* 1 中定义），从而我们还推导出一个 *C-线性* 映射，称为 *规范*

（13）$\operatorname{Hom}_A(E, E') \otimes_C \operatorname{Hom}_A(F, F') \to \operatorname{Hom}_C(E \otimes_A F, E' \otimes_A F')$。

(3) 设A为整环，K为分数的域。如果 E 和 F 是两个向量 K 空间，典范映射

$$
(E_{[A]}) \otimes_A (F_{[A]}) \to E \otimes_K F
$$

(no. 3 和 § 1, no. 13) 是*双射的*。只要证明（no. 4），如果$f$是$E \times F$的*A双线性*映射进入向量K空间G，$f$也是*K双线性*。现在，对于 A 中的所有 $\alpha \neq 0$。

$$
\alpha f(\alpha^{-1}x, y) = f(x, y) = \alpha f(x, \alpha^{-1}y)
$$
从而
$$
f(\alpha^{-1}x, y) = f(x, \alpha^{-1}y) = \alpha^{-1}f(x, y)
$$
因为 G 是向量 K 空间。

### 6. $E \otimes_A F$ 相对于正合序列的性质

#### 命题 5 {#alg-ii-s3-prop-5 .statement tag=05P2}

*设* E、E'、E'' *为右* A-*模*，F *左* A-*模* 且

(14)

$$
E' \xrightarrow{u} E \xrightarrow{v} E'' \to 0
$$

*正合序列 / 线性映射.* *写作* $\bar{u} = u \otimes 1_F, \bar{v} = v \otimes 1_F,$ *序列*

(15)

$$
E' \otimes_A F \xrightarrow{\bar{u}} E \otimes_A F \xrightarrow{\bar{v}} E'' \otimes_A F \to 0
$$

*的*$\mathbf{Z}$-*同态**是准确的*。

凭借no. 2、公式(5)、$\bar{v} \circ \bar{u} = (v \circ u) \otimes 1_F = 0$； 像$H = \bar{u}(E' \otimes F)$包含在核$L = \operatorname{Ker}(\bar{v})$中；通过经过求商，因此我们从 $\bar{v}$ 导出 $\bar{u}$ 的余核 $M = (E \otimes F)/H$ 的 $\mathbf{Z}$ 线性映射 $f$ 到 $E'' \otimes F$；必须证明$f$是*双射的*，因此它足以满足定义一个$\mathbf{Z}$线性映射$g : E'' \otimes F \to M$，使得$g \circ f$和$f \circ g$是恒等映射。

设$x'' \in E''$，$y \in F$；到假设，存在$x \in E$，使得$v(x) = x''$。我们证明，如果$x_1, x_2$是E的两个元素，使得$v(x_1) = v(x_2) = x''$和$\phi : E \otimes F \to M$是典范映射，则$\phi(x_1 \otimes y) = \phi(x_2 \otimes y)$。只要证明如果$v(x) = 0$则$\phi(x \otimes y) = 0$即可，这是从$x = u(x')$与$x' \in E'$、从而$x \otimes y = u(x') \otimes y = \bar{u}(x' \otimes y) \in H$这一事实得出的。如果对于所有$x \in E$，将$(x'', y)$映射到$\phi(x \otimes y)$的唯一值，使得$v(x) = x''$，映射将$E'' \times F$定义到M中；这个映射是$\mathbf{Z}$双线性并且满足条件 (1) (no. 1)，因为$v(x \lambda) = x'' \lambda$和$(x \lambda) \otimes y = x \otimes (\lambda y)$对于$x \in E$；因此，存在$E'' \otimes F$到M的$\mathbf{Z}$线性映射$g$，使得$g(x'' \otimes y) = \phi(x \otimes y)$对应于$y \in F, x \in E$和$x'' = v(x)$。这个定义进一步证明了$f \circ g$重合和恒等映射对于元素的

形式 $x'' \otimes y$ 的$E'' \otimes F$，因此$f \circ g$ 是$E'' \otimes F$ 的恒等映射；另一方面，对于$x \in E$和$y \in F$，$f(\phi(x \otimes y)) = v(x) \otimes y$乘以定义，因此$g(f(\phi(x \otimes y))) = \phi(x \otimes y)$，并且，作为形式$\phi(x \otimes y)$生成M的元素，$g \circ f$是恒等映射 M 的。

#### 推论{#alg-ii-s3-n6-cor-1 .statement tag=05P3}

*设 F、F'、F'' 为左A-模，E 右A-模且*
$$
\begin{array}{ccccc}
F' & \xrightarrow{s} & F & \xrightarrow{t} & F'' \longrightarrow 0
\end{array}
$$
*(16)*
*正合序列 / 线性映射。写出 \bar{s} = l_E \otimes s, \bar{t} = l_E \otimes t, \mathbf{Z} 同态* 的序列
$$
\begin{array}{cccccc}
E \otimes_A F' & \xrightarrow{\bar{s}} & E \otimes_A F & \xrightarrow{\bar{t}} & E \otimes_A F'' & \longrightarrow 0
\end{array}
$$
*(17)*
*准确。*

当 E（或 F）被视为左（或右）A^0 模时，F \otimes_{A^0} E 被识别为 E \otimes_A F，并且 F' \otimes_{A^0} E 和 F'' \otimes_{A^0} E 也有类似的识别（no. 1，推论 2 到命题 1）；推论立即从命题 5 得出。

#### 注 {#alg-ii-s3-n6-rem-1 .statement tag=05P4}

注一般来说，如果 E' 是右A-模 E 的子模且 j : E' \to E 典范嵌入, 典范映射
$$
j \otimes 1_F : E' \otimes F \to E \otimes F
$$
*不一定是单射的。* 在其他字中，对于正合序列
$$
\begin{array}{ccccccc}
0 & \longrightarrow & E' & \xrightarrow{u} & E & \xrightarrow{v} & E'' \longrightarrow 0
\end{array}
$$
*(18)*
不能一般可以得出序列
$$
\begin{array}{ccccccc}
0 & \longrightarrow & E' \otimes F & \xrightarrow{u} & E \otimes F & \xrightarrow{v} & E'' \otimes F \longrightarrow 0
\end{array}
$$
*(19)*
*准确。*

取例 A = \mathbf{Z}，E = \mathbf{Z}，E' = 2\mathbf{Z}，F = \mathbf{Z}/2\mathbf{Z}。由于 E' 与 E 同构的，E' \otimes F 与 E \otimes F 同构的，而 E \otimes F 本身又与 F (no. 4, 命题 4) 同构的。但对于所有 x' = 2x \in E' （其中 x \in E）和所有 y \in F，j(x') \otimes y = (2x) \otimes y = x \otimes (2y) = 0，因为 2y = 0，并且 E' \otimes F in E \otimes F 约化的典范像为 0。

在其他字中，对于 E 的子模 E' 和元素 x \in E' ，必须注意区分元素 x \otimes y “在 E' \otimes F' 中计算”和元素 x \otimes y “在 E \otimes F' 中计算”（在其他字，元素 j(x) \otimes y)。

稍后我们将在单位模，模 F 的名称下进行研究，使得序列(19)对于每个正合序列(18)都是精确的(*交换代数*，I, § 2)。

#### 命题 6 {#alg-ii-s3-prop-6 .statement tag=05P5}

*给定两个正合序列 (14) 和 (16)，同态 v \otimes t : E \otimes_A F \to E'' \otimes_A F'' 是满射，其核等于*
$$
\operatorname{Im}(u \otimes 1_F) + \operatorname{Im}(l_E \otimes s)
$$

现在 $v \otimes t = (v \otimes 1_{F''}) \circ (1_E \otimes t)$ (no. 2, 公式 (5)) 和 $v \otimes t$ 因此是满射的，根据命题 5 及其推论，它是两个满同态的合成。另一方面，要使$z \in E \otimes F$在$v \otimes t$的核内，$(1_E \otimes t)(z)$属于到$v \otimes 1_{F''}$的核是充分必要的，即，凭借（15）到像

$$
u \otimes 1_{F''}: E' \otimes F'' \to E \otimes F''.
$$

但由于同态 $t: F \to F''$ 是满射，所以也是

$$
1_{E'} \otimes t: E' \otimes F \to E' \otimes F''
$$

由命题 5 的推论，因此 $z$ 约化上的条件存在$a \in E' \otimes F$，使得

$$
(l_E \otimes t)(z) = (u \otimes t)(a).
$$

令 $b = z - (u \otimes 1_F)(a)$；然后$(l_E \otimes t)(b) = 0$，并凭借(17)，$l_E \otimes s$的$b$属于到像，从而证明命题。

其他字：

#### 推论 1 {#alg-ii-s3-prop-6-cor-1 .statement tag=05P6}

*令$E'$为右$A$模块$E$的子模，左$A$模块$F$的$F'$子模以及$\operatorname{Im}(E' \otimes_A F)$和$\operatorname{Im}(E \otimes_A F')$ $E \otimes_A F$的子$\mathbf{Z}$模块，典范映射$E' \otimes_A F \to E \otimes_A F$各自的像，

$$
E \otimes_A F' \to E \otimes_A F.
$$

然后是一个规范的 $\mathbf{Z}$-模块同构*

$$(20)\quad \pi : (E/E') \otimes_A (F/F') \to (E \otimes_A F)/(\operatorname{Im}(E' \otimes_A F) + \operatorname{Im}(E \otimes_A F'))$$

*这样，对于 $\xi \in E/E'$、$\eta \in F$、$\pi(\xi \otimes \eta)$ 是所有元素 $x \otimes y \in E \otimes_A F$ 中的类，使得 $x \in \xi$ 和 $y \in \eta$。

注，当$E$是$((B'_i); A, (C'_j))$多模块时，$F$是$(A, (B''_h); (C''_k))$多模块，并且$E'$和$F'$分别是$E$和$F$的*子多模块*，同构 (20) 对于两侧 (no. 3) 的$((B'_i), (B''_h); (C'_j), (C''_k))$-多模结构来说，是同构。

#### 推论 2 {#alg-ii-s3-prop-6-cor-2 .statement tag=05P7}

*令$a$为$A$的右理想，$F$为左$A$模，$aF$由形式$\lambda x$的元素生成$F$的子$\mathbf{Z}$模，其中$\lambda \in a$ 和 $x \in F$。然后是一个规范的 $\mathbf{Z}$-模块同构*

$$(21)\quad \pi : (A/a) \otimes_A F \to F/aF$$

*这样，对于所有 $\bar{\lambda} \in A/a$ 和所有 $x \in F$，$\pi(\bar{\lambda} \otimes x)$ 是类 mod。 $\lambda x$的$aF$，其中$\lambda \in \bar{\lambda}$。

特别是，对于$A = \mathbf{Z}$，可以看出，对于每个整数$n$和每个$\mathbf{Z}$-模$F$，$(\mathbf{Z}/n\mathbf{Z}) \otimes_{\mathbf{Z}} F$都被规范地标识为商$\mathbf{Z}$-模$F/nF$。

#### 推论 3 {#alg-ii-s3-prop-6-cor-3 .statement tag=05P8}

令$A$为交换环，$a$为$A$和$E$以及$F$两个$A$模的理想，使得$a$包含在$F$的湮没子中。那么$(A/a)$-模块$E \otimes_A F$和$(E/aE) \otimes_{A/a} F$是规范同构的。

$F$和$E \otimes_A F$被$a$消灭，因此具有规范的$(A/a)$模块结构（$§ 1$，no. 12），如果我们写$E' = aE$，则$\operatorname{Im}(E' \otimes_A F) = 0$；那么$E \otimes_A F$的典范同构(20)到$(E/aE) \otimes_A F$，后者本身与$(E/aE) \otimes_{A/a} F$相同（no. 3，命题2的推论）。

#### 推论 4 {#alg-ii-s3-prop-6-cor-4 .statement tag=05P9}

令$a, b$为交换环$C$中的两个理想；那么 $C$-模块 $(C/a) \otimes_C (C/b)$ 与 $C(a + b)$ 是规范同构的。

### 7. 张量积乘积和直和

令$(E_\lambda)_{\lambda \in L}$为右$A$模块族，$(F_\mu)_{\mu \in M}$为左$A$模块族，并考虑乘积模$C = \prod_{\lambda \in L} E_\lambda, D = \prod_{\mu \in M} F_\mu$。 映射 $((x_\lambda), (y_\mu)) \mapsto (x_\lambda \otimes y_\mu)$ / $C \times D$ 进入乘积 $\mathbf{Z}$-模块
$$
\prod_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_A F_\mu)
$$
是 $\mathbf{Z}$ 双线性且显然满足条件 (1) (no. 1)。因此存在 (no. 1, 命题 1) $\mathbf{Z}$-线性映射，称为规范
$$
f : \left( \prod_{\lambda \in L} E_\lambda \right) \otimes_A \left( \prod_{\mu \in M} F_\mu \right) \to \prod_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_A F_\mu)
$$
这样$f((x_\lambda) \otimes (y_\mu)) = (x_\lambda \otimes y_\mu)$。

当$C = R^L, D = S^M, R$（或$S$）是右（或左）$A$模块时，典范映射（22）与每个张量积$u \otimes v$关联，其中$u$是$L$到$R$的映射，并且将$M$中的$v$映射转换为$S$，将$L \times M$中的映射$(\lambda, \mu) \mapsto u(\lambda) \otimes v(\mu)$转换为$R \otimes_A S$；即使在这种情况下，典范映射 (22) 通常既不是单射也不是满射（习题 3；cf. 推论 3 到命题 7）。

当$E_\lambda$为$((B'_i); A, (C'_j))$-多模块且$F_\mu$$(A, (B''_h); (C''_{k_c}))$-多模块时，同态(22)对于两侧的$((B'_i), (B''_h); (C'_j), (C''_{k_c}))$-多模块结构来说也是同态。

现在考虑$C$（或$D$）的子模$E = \bigoplus_{\lambda \in L} E_\lambda$（或$\bigoplus_{\mu \in M} F_\mu$）； 典范嵌入 $E \to C, F \to D$ 定义典型的$\mathbf{Z}$线性映射$E \otimes_A F \to C \otimes_A D$，与映射 (22) 组合，给出$E \otimes_A F$到$\prod_{\lambda, \mu} (E_\lambda \otimes_A F_\mu)$的$\mathbf{Z}$线性映射$g$，使得
$$
g((x_\lambda) \otimes (y_\mu)) = (x_\lambda \otimes y_\mu);
$$

此外，由于家庭$(x_\lambda)$和$(y_\mu)$有有限支撑，$(x_\lambda \otimes y_\mu)$也是如此，因此最终$g$是典范同态

$$
g : \left( \bigoplus_{\lambda \in L} E_\lambda \right) \otimes_A \left( \bigoplus_{\mu \in M} F_\mu \right) \to \bigoplus_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_A F_\mu),
$$

这是与（22）相同的条件下的多模块同态。

#### 命题 7 {#alg-ii-s3-prop-7 .statement tag=05PA}

*典范映射 (23) 是双射的。*

为了证明这一点，只需将直和$G = \bigoplus_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_A F_\mu)$的定义$\mathbf{Z}$线性映射$h$映射到$E \otimes_A F$，使得$g \circ h$和$h \circ g$是恒等映射。但是，对于 $G$ 到 $E \otimes_A F$ 的定义 $\mathbf{Z}$ 线性映射，(§ 1, no. 6, 命题 6) 到定义 $\mathbf{Z}$ 线性映射就足够了

$$
h_{\lambda \mu} : E_\lambda \otimes_A F_\mu \to E \otimes_A F
$$

对于每个有序对$(\lambda, \mu)$，我们取$h_{\lambda \mu} = i_\lambda \otimes j_\mu$，其中$i_\lambda : E_\lambda \to E$和$j_\mu : F_\mu \to F$是典范嵌入。然后显然 $h \circ g$ 重合和恒等映射为形式 $\left( \sum_\lambda x_\lambda \right) \otimes \left( \sum_\mu y_\mu \right)$ 的元素，其中生成 $\mathbf{Z}$-模块 $E \otimes_A F$；类似地，$g \circ h$重合和恒等映射对于形式$\sum_{\lambda, \mu} (x_\lambda \otimes y_\mu)$的元素，其中生成$\mathbf{Z}$-模块$G$，因为对于每个有序对$(\lambda, \mu)$ 乘积

$$
x_\lambda \otimes y_\mu \quad (x_\lambda \in E_\lambda, y_\mu \in F_\mu)
$$

生成 $\mathbf{Z}$-模块$E_\lambda \otimes_A F_\mu$。 从而命题。

令$u_\lambda : E_\lambda \to E'_\lambda$、$v_\mu : F_\mu \to F'_\mu$为$A$-同态；显然图表

$$
\begin{array}{ccc}
\left( \bigoplus_\lambda E_\lambda \right) \otimes_A \left( \bigoplus_\mu F_\mu \right) & \longrightarrow & \bigoplus_{\lambda, \mu} (E_\lambda \otimes_A (F_\mu)) \\
(\bigoplus u_\lambda) \otimes (\bigoplus v_\mu) \downarrow & & \downarrow (\bigoplus (u_\lambda \otimes v_\mu)) \\
\left( \bigoplus_\lambda E'_\lambda \right) \otimes_A \left( \bigoplus_\mu F'_\mu \right) & \longrightarrow & \bigoplus_{\lambda, \mu} (E'_\lambda \otimes_A F'_\mu)
\end{array}
$$

是可交换的。

#### 推论 1 {#alg-ii-s3-prop-7-cor-1 .statement tag=05PB}

*如果左$A$-模块$F$承认基$(b_\mu)_{\mu \in M}$，则$E \otimes_A F$的每个元素都可以唯一地写在形式$\sum_\mu (x_\mu \otimes b_\mu)$中，其中$x_\mu \in E$和族$(x_\mu)$有有限支撑。 $\mathbf{Z}$-模块 $E \otimes_A F$ 与 $E^{(M)}$ 同构的，被视为 $\mathbf{Z}$-模块。*

The basis $(b_\mu)$ defines an isomorphism of $F$ onto $\bigoplus_{\mu \in M} Ab_\mu$, whence there is an isomorphism $E \otimes_A F \to \bigoplus_{\mu \in M} (E \otimes_A Ab_\mu)$ by virtue of Proposition 7; as ξ ↦ ξb_μ is an isomorphism of A_s onto Ab_μ, x ↦ x ⊗ b_μ is an isomorphism of E onto E ⊗_A (Ab_μ) by virtue of Proposition 4 of no. 4, whence the corollary.

如果 E 是 ((B'_i); A, (C'_j))-多模，典范同构 E ⊗_A F → E^{(M)} 是 ((B'_i); (C'_j))-多模同构。

特别是，如果 E 也承认基 (a_λ)_{λ ε L}，则每个 z ∈ E ⊗_A F 都可以以一种且仅一种方式写成形式 $\sum_{\lambda, \mu} (a_\lambda \xi_{\lambda\mu}) \otimes b_\mu$，其中 xi_{λμ} 属于到 A（以及形式有限支撑族）；对于 \mathbf{Z} 模结构，映射 $z \mapsto (\xi_{\lambda\mu})_{(\lambda, \mu) \in L \times M}$ 是 E ⊗_A F 的同构到 A^{(L × M)} 上（甚至是 A 的中心上的模结构）。更具体地说：

#### 推论 2 {#alg-ii-s3-prop-7-cor-2 .statement tag=05PC}

*如果 E 和 F 是交换环 C 上的两个自由模，并且 (a_λ)（分别为 (b_μ)）是 C-模 E（分别为 F）的基，则 (a_λ ⊗ b_μ) 是 C-模 E ⊗_C F 的基。*

滥用语言，基 (a_λ ⊗ b_μ) 是有时，称为基 (a_λ) 和 (b_μ) 的 *张量积*。

*注(1)*。设 E 为自由右A-模，F 为自由左A-模，E 的 (a_λ)_{λ ∈ L} 基和 F 的 (b_μ)_{μ ∈ M} 基。每个元素 z ∈ E ⊗_A F 可以唯一地写为 $\sum_\lambda a_\lambda \otimes y_\lambda$，其中 y_λ ∈ F，并且也唯一为 $\sum_\mu x_\mu \otimes b_\mu$，其中 x_μ ∈ E。如果我们写 $y_\lambda = \sum_\mu \eta_{\lambda\mu} b_\mu$，$x_\mu = \sum_\lambda a_\lambda \xi_{\lambda\mu}$，其中 xi_{λμ} 和 η_{λμ} 属于为 A，则 $\xi_{\lambda\mu} = \eta_{\lambda\mu}$ 对于所有 (λ, μ)，对于

$$
\sum_\lambda \left( a_\lambda \otimes \left( \sum_\mu \eta_{\lambda\mu} b_\mu \right) \right) = \sum_{\lambda, \mu} ((a_\lambda \eta_{\lambda\mu}) \otimes b_\mu) = \sum_\mu \left( \left( \sum_\lambda a_\lambda \eta_{\lambda\mu} \right) \otimes b_\mu \right).
$$

#### 推论 3 {#alg-ii-s3-prop-7-cor-3 .statement tag=05PD}

*设 (E_λ)_{λ ∈ L} 为右A-模族，F 为自由（或有限生成的自由）左A-模。那么典范映射 (22)

$$
\left( \prod_{\lambda \in L} E_\lambda \right) \otimes_A F \to \prod_{\lambda \in L} (E_\lambda \otimes_A F)
$$

是单射（或双射）。

如果(b_μ)是F的基，则$\left( \prod_{\lambda \in L} E_\lambda \right) \otimes_A F$的每个元素都可以唯一地写成$z = \sum_\mu ((x_\lambda^{(\mu)}) \otimes b_\mu)$（推论1）；说它的典范像是零意味着，对于所有 λ ∈ L，$\sum_\mu (x_\lambda^{(\mu)} \otimes b_\mu) = 0$，因此对于所有 λ ∈ L 和所有 μ（推论 1），$x_\lambda^{(\mu)} = 0$，因此$z = 0$。

证明当 F 承认有限基时典范映射是双射的，凭借命题 7，立即减少到以下情况：

F = A_s；但随后两侧都被规范地标识为$\prod_{\lambda \in L} E_\lambda$（no. 4，命题 4）和之后，这些标识典范映射（22）成为身份。

#### 推论 4 {#alg-ii-s3-prop-7-cor-4 .statement tag=05PE}

*设 A 为环，没有除子或零，E 为自由右A-模，F 为自由左A-模。那么 E $\otimes_A$ F 中的关系 x $\otimes$ y = 0 意味着 x = 0 或 y = 0。*

令$(a_\lambda)$为E的基，F的$(b_\mu)$基，并令$x = \sum_\lambda a_\lambda \xi_\lambda, y = \sum_\mu \eta_\mu b_\mu$；那么$x \otimes y = \sum_{\lambda, \mu} ((a_\lambda \xi_\lambda \eta_\mu) \otimes b_\mu$和关系$x \otimes y = 0$意味着$\xi_\lambda \eta_\mu = 0$对于指标$(\lambda, \mu)$的每一个有序对（推论1）。因此，如果$x \neq 0$，即至少一个$\lambda$的$\xi_\lambda \neq 0$，那么$\eta_\mu = 0$对于所有$\mu$，从而$y = 0$。

#### 推论 5 {#alg-ii-s3-prop-7-cor-5 .statement tag=05PF}

*设 E 为 E 的右A-模、F 左A-模、M 子模和 F 的 N 子模。如果 M 为 E 的直因子且 F 的 N 直因子，则典范同态 $M \otimes_A N \to E \otimes_A F$ 是单内射，在此情况下$M \otimes_A N$ 的像同态是 $\mathbf{Z}$ 模块 $E \otimes_A F$ 的直因子。*

这紧随命题 7 而来。

注，如果 E 是$((B'_i); A, (C'_j))$-多模块，F 是$(A, (B''_h); (C''_k))$-多模块，并且这些多模块中的 M 和 N 直因子，则 $M \otimes N$ 是 $((B'_i), (B''_h); (C'_j), (C''_k))$-多模块 $E \otimes F$ 的直因子。

#### 推论 6 {#alg-ii-s3-prop-7-cor-6 .statement tag=05PG}

*设 P 为射影左A-模，E、F 为两个右A-模。对于每个单同态 $u : E \to F$、同态*
$$
u \otimes 1_P : E \otimes_A P \to F \otimes_A P
$$
*是单射的。*

存在左A-模 Q 使得 $L = P \oplus Q$ 是自由的 (§ 2, no. 2, 命题 4) 并且 $u \otimes 1_L$ 被识别 (命题 7)
$$(u \otimes 1_P) \oplus (u \otimes 1_Q);$$
因此，只要证明 P 是*自由*时的推论就足够了（§ 1, no. 6，推论 1 到命题 7）。与 $P = A_s$ 的情况相同的参数约化问题，它紧随 no. 4、命题 4。

#### 推论 7 {#alg-ii-s3-prop-7-cor-7 .statement tag=05PH}

*设C为交换环。如果 E 和 F 是两个射影 C-模，则 $E \otimes_C F$ 是一个射影 C-模。*

这直接从推论 5 和两个自由 C-模中的张量积是一个自由 C-模的事实得出（推论 2）。

#### 注 2 {#alg-ii-s3-n7-rem-2 .statement tag=05PI}

在命题7的假设下，令$E'_\lambda$为$E_\lambda$的子模，$F'_\mu$子模或$F_\mu$，并令$E' = \bigoplus_{\lambda \in L} E'_\lambda$，$F' = \bigoplus_{\mu \in M} F'_\mu$。令 Im$(E' \otimes_A F')$ (或 Im(E'_λ ⊗_A F'_μ)) 表示典范映射下 E' ⊗_A F' (或 E'_λ ⊗_A F'_μ) 中 E ⊗_A F (或 E_λ ⊗_A F_μ) 的像；然后同构 (23) 识别子$\mathbf{Z}$模块

$$
\operatorname{Im}(E' \otimes_A F') \quad \text{and} \quad \bigoplus_{(\lambda, \mu) \in I \times M} \operatorname{Im}(E'_\lambda \otimes_A F'_\mu);
$$

这紧接着从交换律到图表

$$
\begin{array}{ccc}
\left( \bigoplus_\lambda E'_\lambda \right) \otimes_A \left( \bigoplus_\mu F'_\mu \right) & \longrightarrow & \left( \bigoplus_\lambda E_\lambda \right) \otimes_A \left( \bigoplus_\mu F_\mu \right) \\
\downarrow & & \downarrow \\
\bigoplus_{\lambda, \mu} (E'_\lambda \otimes_A F'_\mu) & \longrightarrow & \bigoplus_{\lambda, \mu} (E_\lambda \otimes_A F_\mu)
\end{array}
$$

其中垂直箭头是典范同构。

### 8. 张量积的结合性

#### 命题 8 {#alg-ii-s3-prop-8 .statement tag=05PJ}

*设 A、B 为两个环，E 右A-模，F 为 (A, B) 双模，G 左B-模。则 E ⊗_A F 为右B-模，F ⊗_BG 左A-模且存在且仅有一个 $\mathbf{Z}$-线性映射*

$$
\phi : (E \otimes_A F) \otimes_B G \to E \otimes_A (F \otimes_B G)
$$

*使得*$\phi((x \otimes y) \otimes z) = x \otimes (y \otimes z)$*对于*$x \in E,\ y \in F,\ z \in G;$此外*这个$\mathbf{Z}$线性映射是双射的*（张量积的“结合性”）。

E ⊗_A F 上的右B-模结构和 F ⊗_B G 上的左A-模结构已在no. 4 中定义。 $\phi$的唯一性是显而易见的，因为元素$(x \otimes y) \otimes z$生成$\mathbf{Z}$-模块$(E \otimes_A F) \otimes_B G$。为了证明$\phi$的存在，我们注认为，对于所有$z \in G,\ h_z : y \mapsto y \otimes z$来说，左A-模F到左A-模F⊗_B G的A-线性映射。我们写成$g_z = 1_E \otimes h_z$，因此它是E⊗_A F到E的$\mathbf{Z}$线性映射⊗_A (F ⊗_B G) 并考虑从 $(E \otimes_A F \times G$ 到 $E \otimes_A (F \otimes_B G)$ 的映射 $(t, z) \mapsto g_z(t)$；正如$h_{z + z'} = h_z + h_{z'}$对于$z \in G,\ z' \in G$来说，上面的映射是$\mathbf{Z}$双线性就是直接的。此外，我们证明对于所有 $\mu \in B,\ g_{\mu z}(t) = g_z(t \mu)$；显然，对于$t = x \otimes y$这样做就足够了，其中$x \in E$和$y \in F$；现在和

$$
g_{\mu z}(x \otimes y) = x \otimes (y \otimes \mu z)
$$
$$
g_z((x \otimes y)\mu) = g_z(x \otimes y\mu) = x \otimes (y\mu \otimes z).
$$

命题 1 (no. 1) 然后证明$\mathbf{Z}$-线性映射的存在

$$
\phi : (E \otimes_A F) \otimes_B G \to E \otimes_A (F \otimes_B G)
$$

这样$\phi(t \otimes z) = g_z(t)$，因此$\phi((x \otimes y) \otimes z) = x \otimes (y \otimes z)$。类似地，$\mathbf{Z}$-线性映射

$$
\psi : E \otimes_A (F \otimes_B G) \to (E \otimes_A F) \otimes_B G
$$

被定义为使得$\psi(x \otimes (y \otimes z)) = (x \otimes y) \otimes z$并且显然$\psi \circ \phi$和$\phi \circ \psi$分别是$(E \otimes_A F) \otimes_B G$和$E \otimes_A (F \otimes_B G)$的恒等映射，因为它们在这些$\mathbf{Z}$模块的生成的系统上是约化到恒等映射。

直接的，如果$E$是$((C'_i); A, (D'_j))$多模块，$F$是$(A, (C''_h); B, (D''_k))$多模块，$G$是$(B, (C'''_l); (D'''_m))$多模块，命题8中定义的典范同构是$((C'_i), (C''_h), (C'''_l); (D'_j), (D''_k), (D'''_m))$多模块同构。特别是，如果 $C$ 是一个*可交换的* 环和 $E, F, G$ 三个 $C$ 模块，则存在一个规范的 $C$ 模块同构

$$
(E \otimes_C F) \otimes_C G \to E \otimes_C (F \otimes_C G).
$$

我们将在下面看到，在某些条件下，张量积的定义可以推广到一系列多模块，这将特别在命题8的假设下为我们提供一个$\mathbf{Z}$-模块$E \otimes_A F \otimes_B G$，它与每个$\mathbf{Z}$-模块$(E \otimes_A F) \otimes_B G$和$E \otimes_A (F \otimes_B G)$，后者将被识别。

### 9. 张量积多模块系列

令$(G_\lambda)_{\lambda \in L}$为$\mathbf{Z}$模块族；如果 $(x_\lambda) \mapsto u((x_\lambda))$ 相对于每个变量 $x_\lambda$ 是可加的，则将集合 $G = \prod_{\lambda \in L} G_\lambda$ 的映射 $u$ 放入$\mathbf{Z}$-模块中被称为*多重可加性*（或$\mathbf{Z}$-*多重线性*）；准确地说，这意味着，对于所有 $\mu \in L$ 和每个元素 $(a_\lambda) \in \prod_{\lambda \neq \mu} G_\lambda$，规范地识别 $G$ 与 $G_\mu \times \prod_{\lambda \neq \mu} G_\lambda$，

$$
u(x_\mu + y_\mu, (a_\lambda)) = u(x_\mu, (a_\lambda)) + u(y_\mu, (a_\lambda)) \quad \text{for } x_\mu, y_\mu \text{ in } G_\mu.
$$

这特别意味着如果$x_\lambda$之一是零，则$u((x_\lambda)) = 0$。

我们还考虑*普遍映射问题*，其中$\Sigma$是$\mathbf{Z}$模块结构的类，$\alpha$映射是$G$到$\mathbf{Z}$模块的多重加法映射。 解仍然是通过考虑$G$的元素的形式线性组合的$\mathbf{Z}$-模$C = \mathbf{Z}^{(G)}$（系数在$\mathbf{Z}$）和$C$的子$\mathbf{Z}$-模$D$生成元素 / 形式

$$
(x_\mu + y_\mu, (z_\lambda)_{\lambda \neq \mu}) - (x_\mu, (z_\lambda)_{\lambda \neq \mu}) - (y_\mu, (z_\lambda)_{\lambda \neq \mu})
$$

其中 $\mu \in L, x_\mu \in G_\mu, y_\mu \in G_\mu$ 和 $z_\lambda \in G_\lambda$ ($\lambda \neq \mu$) 是任意的。 $\mathbf{Z}$-模$C/D$称为$\mathbf{Z}$-*模*的族*$(G_\lambda)_{\lambda \in L}$的*张量积（大于$\mathbf{Z}$），记为$\bigotimes_{\lambda \in L} G_\lambda$；对于$G$的每个元素$(x_\lambda)_{\lambda \in L}$，即$C$的典范基元素，$\bigotimes_{\lambda \in L} x_\lambda$表示C/D中该元素的典范像。从上面的定义可以得出，G到$\bigotimes_{\lambda \in L} G_\lambda$的映射$\phi : (x_\lambda) \mapsto \bigotimes_{\lambda \in L} x_\lambda$是$\mathbf{Z}$-多重线性，并且对于G的每个$\mathbf{Z}$-多重线性映射$f$到$\mathbf{Z}$-模块H，存在一个且仅有一个$\mathbf{Z}$-线性映射$g : \bigotimes_{\lambda \in L} G_\lambda \to H$使得$f = g \circ \phi$； 有序对$\left( \bigotimes_{\lambda \in L} G_\lambda, \phi \right)$因此解决了有问题的普遍映射问题。

令$(G'_\lambda)_{\lambda \in L}$为$\mathbf{Z}$模块的另一个族，对于所有$\lambda \in L$，令$v_\lambda : G_\lambda \to G'_\lambda$为$\mathbf{Z}$线性映射（在可交换群的其他字同态中）。然后映射
$$
(x_\lambda) \mapsto \bigotimes_{\lambda \in L} v_\lambda(x_\lambda)
$$
G 到 $\bigotimes_{\lambda \in L} G'_\lambda$ 的映射是 $\mathbf{Z}$-多重线性的，因此定义典型地是 $\bigotimes_{\lambda \in L} G_\lambda$ 到 $\bigotimes_{\lambda \in L} G'_\lambda$ 的 $\mathbf{Z}$ 线性映射，用 $\bigotimes_{\lambda \in L} v_\lambda$ 表示，这样
$$
\left( \bigotimes_{\lambda \in L} v_\lambda \right) \left( \bigotimes_{\lambda \in L} x_\lambda \right) = \bigotimes_{\lambda \in L} v_\lambda(x_\lambda).
$$
特别是，我们考虑，对于 $\mu \in L$、自同态 $\theta$ 或 $G_\mu$；我们用$\bigotimes_{\lambda \in L} G_\lambda$的$\tilde{\theta}$自同态等于$\bigotimes_{\lambda \in L} v_\lambda$来表示，其中$v_\mu = \theta$和$v_\lambda = 1_{G_\lambda}$代表$\lambda \neq \mu$。

然后我们假设给定集合 $\Omega$, 映射
$$
c : \omega \mapsto (\rho(\omega), \sigma(\omega))
$$
将 $\Omega$ 转换为 $L \times L$，并且对于所有 $\omega \in \Omega$、$G_{\rho(\omega)}$ 的自同态 $p_\omega$ 和 $G_{\sigma(\omega)}$ 的自同态 $q_\omega$；他们有对应两个自同态 $\tilde{p}_\omega$ 和$\tilde{q}_\omega$ $P = \bigotimes_{\lambda \in L} G_\lambda$。令 R 为当 $\omega$ 穿过 $\Omega$ 时，由自同态* $\tilde{p}_\omega - \tilde{q}_\omega$ 的像的并生成的 P * 的子 $\mathbf{Z}$ 模。 $\mathbf{Z}$模$P/R$称为族*$(G_\lambda)_{\lambda \in L}$*相对于*c、p、q的*张量积，并用$\bigotimes_{(c, p, q)} G_\lambda$表示；将典范同态$P \to P/R$与上面定义的映射$\phi : G \to \bigotimes_{\lambda \in L} G_\lambda$组合，我们得到一个$\mathbf{Z}$-多重线性映射$\phi_{(c, p, q)} : G \to \bigotimes_{(c, p, q)} G_\lambda$并写成$\phi_{(c, p, q)}((x_\lambda)) = \bigotimes_{(c, p, q)} x_\lambda$或简称$\bigotimes_{(c)} x_\lambda$。 $\bigotimes_{(c, p, q)} x_\lambda$ 和 $\phi_{(c, p, q)}$ 的有序对由……组成解决以下问题 *普遍映射问题*：令 $\bar{p}_\omega$（或 $\bar{q}_\omega$）表示映射
$$
(x_{\rho(\omega)}, (x_\lambda)_{\lambda \neq \rho(\omega)}) \mapsto (p_\omega(x_{\rho(\omega)}), (x_\lambda)_{\lambda \neq \rho(\omega)})
$$
（分别$(x_{\sigma(\omega)}, (x_\lambda)_{\lambda \neq \sigma(\omega)}) \mapsto (q_\omega(x_{\sigma(\omega)}), (x_\lambda)_{\lambda \neq \sigma(\omega)})$）
G 进入自身。然后$\Sigma$被视为$\mathbf{Z}$模块结构的类，并且将$G$的$\mathbf{Z}$-多线性映射$u$的α-映射到$\mathbf{Z}$模块，进一步满足条件

$$(26)$$
$$
u \circ \bar{p}_\omega = u \circ \bar{q}_\omega
$$

对于所有$\omega \in \Omega$。从上面的定义可以明显看出证明。

这个构造特别恢复了no. 1中描述的$E \otimes_A F$：在这种情况下，我们采用$L = \{1, 2\}$，$G_1 = E$，$G_2 = F$，$\Omega = A$；此外，对于所有$\omega \in A$，我们必须有$\rho(\omega) = 1$，$\sigma(\omega) = 2$，$\omega$是$\mathbf{Z}$模块$E$的自同态$x \mapsto x\omega$和$q_\omega$自同态$y \mapsto \omega y$ $\mathbf{Z}$-模块$F$。

令$(G'_\lambda)_{\lambda \in L}$为$\mathbf{Z}$模块的第二个家族；保持映射$c$相同，假设给定$G'_{\rho(\omega)}$的所有$\omega \in \Omega$、自同态$p'_\omega$和$G'_{\sigma(\omega)}$的自同态$q'_\omega$。对于所有 $\lambda \in L$，则令 $v_\lambda : G_\lambda \to G'_\lambda$ 为 $\mathbf{Z}$ 线性映射，使得对于所有 $\omega \in \Omega$，

$$(27)$$
$$
v_{\rho(\omega)} \circ p_\omega = p'_\omega \circ v_{\rho(\omega)} \quad \text{and} \quad v_{\sigma(\omega)} \circ q_\omega = q'_\omega \circ v_{\sigma(\omega)}
$$

（在其他字中，对于所有$\lambda \in L$，$v_\lambda$对于$G_\lambda$（或$G'_\lambda$）上定义的$p_\xi$和$q_\eta$（或$p'_\xi$和）上的作用的律来说是态射 $q'_\eta$）与$\xi$和$\eta$，使得$\rho(\xi) = \lambda$和$\sigma(\eta) = \lambda$）。然后映射
$$
u : (x_\lambda) \mapsto \bigotimes_{(c, p', q')} v_\lambda(x_\lambda)
$$
$G$ 到 $\bigotimes_{(c, p', q')} G'_\lambda$ 的映射是 $\mathbf{Z}$ 多重线性，并且满足条件 (26)，因此定义是 $\bigotimes_{(c, p, q)} G_\lambda$ 到 $\bigotimes_{(c, p', q')} G'_\lambda$ 的 $\mathbf{Z}$ 线性映射，如果不会混淆的话，我们将简单地用 $\bigotimes_{(c)} v_\lambda$ 来表示出现。

现在我们将为如此定义的一般张量积给出“结合性”性质。令$(L_i)_{1 \leq i \leq n}$为$L$的有限划分；对于每个指标$i$，令$\Omega_i$表示$\Omega$由……组成或元素的子集，使得$\rho(\omega) \in L_i$和$\sigma(\omega) \in L_i$；显然$\Omega_i$是成对的不相交的；我们集合$\Omega' = \Omega - \left( \bigcup_i \Omega_i \right)$。对于每个指标$i$，$c^{(i)}$将把$\Omega_i$中的映射$\omega \mapsto (\rho(\omega), \sigma(\omega))$表示为$L_i \times L_i$；对于$\omega \in \Omega_i$，我们写为$p^{(i)}_\omega$和$q^{(i)}_\omega$，而不是$p_\omega$和$q_\omega$。那么对于每个 $i$ 都有一个“部分”张量积
$$
F_i = \bigotimes_{(c^{(i)}, p^{(i)}, q^{(i)})} G_\lambda.
$$

我们进一步做出以下“可置换性”假设：

(P) *如果$\omega \in \Omega'$、$p_\omega$（分别$q_\omega$）与$G_{\rho(\omega)}$（分别$G_{\sigma(\omega)}$）的自同态、$p_\xi$和$q_\eta$进行排列，使得$\xi \notin \Omega'$、$\eta \notin \Omega'$和$\rho(\omega) = \rho(\xi) = \sigma(\eta)$ （分别$\sigma(\omega) = \rho(\xi) = \sigma(\eta)$）。*

对于每个$\omega \in \Omega'$，令$i$为指标，使得$\rho(\omega) \in L_i$；然后考虑家庭$(v_\lambda)_{\lambda \in L_i}$，其中$v_{\rho(\omega)} = p_\omega$和$v_\lambda = 1_{G_\lambda}$代表$\lambda \neq \rho(\omega)$； 假设（P）意味着族$(v_\lambda)$满足条件（27）（其中$p'$和$p$必须由$p^{(i)}$、$q'$和$q$替换为$q^{(i)}$、$\omega$替换为元素$\xi$贯穿$\Omega_i$）；因此自同态$\bigotimes_{(c^{(i)})} v_\lambda = r_\omega$源自$\mathbf{Z}$-模块$F_i$。类似地，自同态$s_\omega$是从$q_\omega$开始的$\mathbf{Z}$模块$F_j$的定义，$j$是指标，使得$\sigma(\omega) \in L_j$；最后让$d(\omega) = (i, j)$。然后我们可以定义 *张量积* $\bigotimes_{(d, r, s)} F_i$ 和相应的典范映射

$$
\phi_{(d, r, s)} : \prod_{i=1}^n F_i \to \bigotimes_{(d, r, s)} F_i.
$$

另一方面，对于每个$i$，典范映射

$$
\psi_i = \phi_{(c^{(i)}, p^{(i)}, q^{(i)})} : \prod_{\lambda \in L_i} G_\lambda \to F_i;
$$

使用集合的乘积的结合性，导出$G$到$\bigotimes_{(d, r, s)} F_i$的$\mathbf{Z}$-多重线性映射$\psi = \phi_{(d, r, s)} \circ (\psi_i)$。我们证明*有序对* $\left( \bigotimes_{(d, r, s)} F_i, \psi \right)$ *是相同通用问题的解* $\left( \bigotimes_{(c, p, q)} G_\lambda, \phi_{(c, p, q)} \right)$，从而将遵循*唯一* $\mathbf{Z}$-模块*同构*的存在

$$
\theta : \bigotimes_{(c, p, q)} G_\lambda \to \bigotimes_{(d, r, s)} F_i
$$

这样$\psi = \theta \circ \phi_{(c, p, q)}$（*集合理论*，IV, § 3, no. 1）。

到$n$的归纳，证明减少到$n = 2$；为简单起见，我们写为 $F_1 \otimes_{(d)} F_2$ 和 $y_1 \otimes_{(d)} y_2$ 而不是 $\bigotimes_{(d, r, s)} F_i$ 和 $\bigotimes_{(d, r, s)} y_i$。考虑从$G$到$F_1 \otimes_{(d)} F_2$的映射

$$
h : (x_\lambda) \to \left( \bigotimes_{(c^{(1)})} x_\lambda \right) \otimes_{(d)} \left( \bigotimes_{(c^{(2)})} x_\lambda \right).
$$

显然是$\mathbf{Z}$-多重线性；我们证明它对于所有 $\omega \in \Omega$ 都满足条件 (26)。如果$\omega \in \Omega_1$或$\omega \in \Omega_2$，这是显而易见的；否则，假设在阶中修正思路，$\rho(\omega) \in L_1$和$\sigma(\omega) \in L_2$，$h \circ \bar{p}_\omega$的值和$h \circ \bar{q}_\omega$在$(x_\lambda)$分别是

$$
\left( r_\omega \left( \bigotimes_{(c^{(1)})} x_\lambda \right) \right) \otimes_{(d)} \left( \bigotimes_{(c^{(2)})} x_\lambda \right) \quad \text{and} \quad \left( \bigotimes_{(c^{(1)})} x_\lambda \right) \otimes_{(d)} \left( s_\omega \left( \bigotimes_{(c^{(2)})} x_\lambda \right) \right)
$$

也等于定义或 $F_1 \otimes_{(d)} F_2$。

既然如此，让$u$是$G$到$\mathbf{Z}$-模块$H$，满足条件的$\mathbf{Z}$多线性映射（26）；我们将定义一个$\mathbf{Z}$线性映射$v : F_1 \otimes_{(d)} F_2 \to H$，这样$u = v \circ h$将证明我们的断言（重复no. 1的论证，推论1到命题1）。对于所有$z_2 = (x_\lambda)_{\lambda \in L_2}$，我们将$\prod_{\lambda \in L_1} G_\lambda$的“部分”线性映射考虑为$H$

$$
u(., z_2): (x_\lambda)_{\lambda \in L_1} \mapsto u((x_\lambda)_{\lambda \in L_1}, z_2) = u((x_\lambda)_{\lambda \in L}).
$$

显然它是 $\mathbf{Z}$-多重线性且对于 $\omega \in \Omega_1$ 满足条件 (26)；通过定义，因此存在$F_1$到$H$的$\mathbf{Z}$线性映射$y_1 \mapsto w_1(y_1, x_2)$，使得

$$
w_1\left( \bigotimes_{(c^{(1)})} x_\lambda, z_2 \right) = u((x_\lambda)_{\lambda \in L_1}, z_2)
$$

我们接下来考虑映射

$$
u_2: (x_\lambda)_{\lambda \in L_2} \mapsto w_1(., (x_\lambda)_{\lambda \in L_2})
$$

$\prod_{\lambda \in L_2} G_\lambda$ 变为 $\mathrm{Hom}_\mathbf{Z}(F_1, H)$；显然，它是$\mathbf{Z}$-多线性的，并且凭借$u$和关系（28）和（29）上的假设，并且考虑到形式的元素这一事实，对于$\omega \in \Omega_2$满足条件（26） $\bigotimes_{(c^{(1)})} x_\lambda$生成$\mathbf{Z}$-模块$F_1$。因此存在$\mathbf{Z}$-线性映射

$$
w_2: F_2 \to \mathrm{Hom}_\mathbf{Z}(F_1, H)
$$

这样

$$
w_2\left( \bigotimes_{(c^{(2)})} x_\lambda \right) = u_2((x_\lambda)_{\lambda \in L_2})
$$

或者也

$$
\left( w_2\left( \bigotimes_{(c^{(2)})} x_\lambda \right) \right)\left( \bigotimes_{(c^{(1)})} x_\lambda \right) = u((x_\lambda)_{\lambda \in L}).
$$

我们现在考虑，对于$y_1 \in F_1, y_2 \in F_2$，元素 of $H$

$$
w(y_1, y_2) = (w_2(y_2))(y_1).
$$

显然，$w$ 是$F_1 \times F_2$ 到$H$ 的$\mathbf{Z}$ 双线性映射。我们进一步表明，对于所有$\omega \in \Omega'$，（假设，为了修正想法，$\rho(\omega) \in L_1$和$\sigma(\omega) \in L_2$）

$$
w(r_\omega(y_1), y_2) = w(y_1, s_\omega(y_2)).
$$

It suffices to verify this relation when $y_1$ (resp. $y_2$) is of the form $\bigotimes_{(c^{(1)})} x_\lambda$ (resp. $\bigotimes_{(c^{(2)})} x_\lambda$), since these elements generate the $\mathbf{Z}$-module $F_1$ (resp. $F_2$). 但通过定义、$r_\omega\left( \bigotimes_{(c^{(1)})} x_\lambda \right) = \bigotimes_{(c^{(1)})} x'_\lambda$，其中 $x'_{\rho(\omega)} = p_\omega(x_{\rho(\omega)})$ 和 $x'_\lambda = x_\lambda$，对于 L₁ 中的 λ ≠ ρ(ω)；类似地 $s_\omega\left( \bigotimes_{(c^{(2)})} x_\lambda \right) = \bigotimes_{(c^{(2)})} x''_\lambda$，其中 $x''_{\sigma(\omega)} = q_\omega(x'_{\sigma(\omega)})$ 和 $x''_\lambda = x_\lambda$，对于 L2 中的 λ ≠ σ(ω)；使用（30）和（31），然后从（26）得出关系（32）。 因此，存在 F₁ ⊗ F2 到 H 的 $\mathbf{Z}$ 线性映射 v，使得 $v(y_1 \otimes y_2) = w(y_1, y_2)$，然后从 (30) 和 (31) 得出 $v \circ h = u$。

上面定义的一般张量积最重要的特殊情况如下：我们从环的族$(A_i)_{1 \leq i \leq n-1}$和族$(E_i)_{1 \leq i \leq n}$开始，其中$E_1$是右$A_1$模块，$E_n$是左$A_{n-1}$模，并且$2 \leq i \leq n-1$、$E_i$ 是$(A_{i-1}, A_i)$ 双模。那么上面的定义应用如下：L是集合$[1, n]$，$G_i = E_i$，Ω是$A_i$（$1 \leq i \leq n-1$）的集合和。对于$\omega \in A_i$ ($1 \leq i \leq n-1$)，取$\rho(\omega) = i$、$\sigma(\omega) = i + 1$、$p_\omega$ 为$Z$-模$E_i$ 和$q_\omega$ 自同态的自同态 $x \mapsto x\omega$ $Z$-模块$E_{i+1}$的$y \mapsto \omega y$； 相应的张量积表示为

$$
E_1 \otimes_{A_1} E_2 \otimes_{A_2} E_3 \otimes \cdots \otimes_{A_{n-2}} E_{n-1} \otimes_{A_{n-1}} E_n
$$

（记号，其中$A_i$偶尔会被抑制）和张量积的元素$\bigotimes_{(c, p, q)} x_i$，对于$(x_i)$家庭，$x_i \in E_i$代表$1 \leq i \leq n$，如果不会引起混淆，可以写成$x_1 \otimes x_2 \otimes \cdots \otimes x_n$；类似的记号用于$Z$线性映射$\bigotimes_{(c)} v_i$。 假设 (P) 对于$[1, n]$的每一个划分都成立，因为$E_i$对于$2 \leq i \leq n-1$来说是双模。当$n = 3$时，我们定义了no. 8中提到的$Z$模块$E \otimes_A F \otimes_B G$，并恢复了命题8（no. 8）。

当每个 $E_i$ 都是多模块时（对于 $2 \leq i \leq n-1$，$A_{i-1}$ 环之一在左侧运行，$A_i$ 环之一在右侧运行，并且类似的条件对于 $i = 1$ 和 $i = n$），如下所示no. 4，多模块结构在$E_1 \otimes_{A_1} E_2 \otimes \cdots \otimes_{A_{n-1}} E_n$上定义，相对于所有环，除了在$E_i$（$1 \leq i \leq n$）上运行的$A_i$之外。

特别地，令 C 为交换环，$(E_i)_{1 \leq i \leq n}$ C-模的族。通过给定 $E_1$ 和 $E_n$ 两个 C-模结构与给定的结构相同，以及 $E_i$ 给定 $2 \leq i \leq n-1$ 三个 C-模结构与给定的结构相同，我们就得到定义张量积

$$
E_1 \otimes_C E_2 \otimes_C E_3 \otimes \cdots \otimes_C E_{n-1} \otimes_C E_n
$$

$n$ C-模结构与一个另一个兼容，并且实际上是相同的，因为对于所有 $\gamma \in C$ 和 $(x_i) \in \prod_{i=1}^n E_i$，通过定义

$$
(\gamma x_1) \otimes x_2 \otimes \cdots \otimes x_n \\
= x_1 \otimes (\gamma x_2) \otimes \cdots \otimes x_n = \cdots = x_1 \otimes x_2 \otimes \cdots \otimes (\gamma x_n).
$$

当我们将张量积 (34) 称为 C-模时，我们总是指的是结构，另外提到的除非，并且在不引起混淆的情况下，张量积 (34) 也用 $\bigotimes_{1 \leq i \leq n} E_i$ 表示。对于每个 C-模 G，$\prod_{i=1}^n E_i$ 到 G 的 $\mathbf{Z}$ 多线性映射，对于每个指标 i，满足关系

$$
f(x_1, \ldots, x_{i-1}, \gamma x_i, x_{i+1}, \ldots, x_n) = \gamma f(x_1, \ldots, x_n)
$$

对于 $\gamma \in \mathbf{C}$ 和 $(x_i) \in \prod_i E_i$ 则称为 C-多重线性，形式 C-模表示为 $\mathscr{L}_n(E_1, \ldots, E_n; G)$； 泛性质 of 张量积 (34) 然后允许我们定义一个规范的 C-模同构

$$
\mathscr{L}_n(E_1, \ldots, E_n; G) \to \operatorname{Hom}_\mathbf{C}(E_1 \otimes_\mathbf{C} E_2 \otimes \cdots \otimes_\mathbf{C} E_n, G)
$$

它与每个 C 多重线性映射 f 和 C 线性映射 g 相关联，使得

$$
f(x_1, \ldots, x_n) = g(x_1 \otimes x_2 \otimes \cdots \otimes x_n).
$$

$E_1 \times \cdots \times E_n$ 到 $\mathbf{C}$ 的 C 多重线性映射也称为 $n$ 线性形式。

设$(F_i)_{1 \leq i \leq n}$为另一个族C-模；对于 n 个 C 线性映射中的每一个系统 $u_i : E_i \to F_i, u_1 \otimes u_2 \otimes \cdots \otimes u_n$（也用 $\bigotimes_{1 \leq i \leq n} u_i$ 表示）是一个 C 线性映射

$$
E_1 \otimes_\mathbf{C} E_2 \otimes \cdots \otimes_\mathbf{C} E_n \text{ into } F_1 \otimes_\mathbf{C} F_2 \otimes \cdots \otimes_\mathbf{C} F_n.
$$

此外，$(u_1, \ldots, u_n) \mapsto u_1 \otimes u_2 \otimes \cdots \otimes u_n$ 是 $\prod_i \operatorname{Hom}_\mathbf{C}(E_i, F_i)$ 的 C 多重线性映射

$$
\operatorname{Hom}_\mathbf{C}(E_1 \otimes_\mathbf{C} E \otimes \cdots \otimes_\mathbf{C} E_n, F_1 \otimes_\mathbf{C} F_2 \otimes \cdots \otimes_\mathbf{C} F_n).
$$

因此，对于后者映射，存在对应规范的 C 线性映射，称为规范

$$
\operatorname{Hom}_\mathbf{C}(E_1, F_1) \otimes_\mathbf{C} \operatorname{Hom}_\mathbf{C}(E_2, F_2) \otimes \cdots \otimes_\mathbf{C} \operatorname{Hom}_\mathbf{C}(E_n, F_n)
$$
$$
\to \operatorname{Hom}_\mathbf{C}(E_1 \otimes_\mathbf{C} E_2 \otimes \cdots \otimes_\mathbf{C} E_n, F_1 \otimes_\mathbf{C} F_2 \otimes \cdots \otimes_\mathbf{C} F_n)
$$

将 no. 5 中定义的内容概括为 $n = 2$。

前面看到的通用结合性性质可以在这里特殊化如下。给定$\mathbf{N}$的区间$\{1, n\}$的划分$(J_k)_{1 \leq k \leq m}$，让对于每个$k$，$F_k$为张量积$E_{i_1} \otimes_\mathbf{C} E_{i_2} \otimes \cdots \otimes_\mathbf{C} E_{i_r}$，其中$(i_1, \ldots, i_r)$为严格递增的序列元素 $J_k$。然后是一个规范的 C-模同构 （称为“结合性同构”）

$$
F_1 \otimes_C F_2 \otimes \cdots \otimes_C F_m \to E_1 \otimes_C E_2 \otimes \cdots \otimes_C E_n
$$

其中，上面的记号、映射张量积

$$
y_1 \otimes y_2 \otimes \cdots \otimes y_m, \quad \text{where } y_k = x_{i_1} \otimes x_{i_2} \otimes \cdots \otimes x_{i_r},
$$

到张量积$x_1 \otimes x_2 \otimes \cdots \otimes x_n$（其中$x_i \in E_i$代表所有$i$）。

特别是，如果$\pi$是$\{1, n\}$的置换，将$J_k = \{\pi(k)\}$写成$1 \leq k \leq n$，我们得到一个规范的（“交换律”）同构

$$
E_{\pi(1)} \otimes_C E_{\pi(2)} \otimes \cdots \otimes_C E_{\pi(n)} \to E_1 \otimes_C E_2 \otimes \cdots \otimes_C E_n
$$

其中映射 $x_{\pi(1)} \otimes x_{\pi(2)} \otimes \cdots \otimes x_{\pi(n)}$ 至 $x_1 \otimes x_2 \otimes \cdots \otimes x_n$。我们经常将认同各种张量积其中对应转换为这些典范同构下的一个另一个。

对于$1 \leq i \leq n$，假设$E_i$承认基$(b^{(i)}_{\lambda_i})_{\lambda_i \in L_i}$；由$n$上的归纳，从no. 7，推论2到命题7，$(b^{(1)}_{\lambda_1} \otimes b^{(2)}_{\lambda_2} \otimes \cdots \otimes b^{(n)}_{\lambda_n})$族，其中$(\lambda_1, \ldots, \lambda_n)$贯穿$\prod_{1 \leq i \leq n} L_i$，是$\bigoplus_{1 \leq i \leq n} E_i$的基，有时称为*有问题的基 $(b^{(1)}_{\lambda_1})$ 中的张量积*。

#### 注 {#alg-ii-s3-n9-rem-1 .statement tag=05PK}

(1) 上述关于模超过交换环的情况的注一般化为no. 5，*注* 2，当存在张量积$E_1 \otimes_{A_1} E_2 \otimes \cdots \otimes_{A_{n-1}} E_n$时，其中环$A_i$不一定是可交换的，并且对于每个$i$，存在相同*可交换*环$C$的同态$\rho_i : C \to A$，使得： (1) $\rho_i(C)$包含在$A_i$的*中心*中； (2) 对于$2 \leq i \leq n - 1$，使用同态$\rho_{i-1}$和$\rho_i$*重合*获得$E_i$上的$C$模块结构。那么类似于(13)(no. 5)在$E_1 \otimes_{A_1} E_2 \otimes \cdots \otimes_{A_{n-1}} E_n$和典范映射上得到一个$C$-*模*结构，留给读者自己描述。

(2) 设$A, B$为两个环，$E$为右$A$模块，$E'$为左$A$模块，$F$为右$B$模块，$F'$为左$B$模块。然后，将 $(E \otimes_A E') \times (F \otimes_B F')$ 的 $\mathbf{Z}\text{-bilinear}$ 映射转换为 $\mathbf{Z}\text{-module}$ $G$，然后与 $E \times E' \times F \times F'$ 的 $\mathbf{Z}\text{-multilinear}$ 映射 $f$ 进行*一对一的对应* 转换为 $G$ 满足条件

$$
\begin{cases}
f(x \lambda, x', y, y') = f(x, \lambda x', y, y') \\
f(x, x', y \mu, y') = f(x, x', y, \mu y')
\end{cases}
$$

$\lambda \in A, \mu \in B, x \in E, x' \in E', y \in F, y' \in F'$。本号中给出的一般构造。 约化证明定义了$(E \otimes_A E') \otimes_{\mathbf{Z}} (F \otimes_B F')$和$E \otimes_A E' \otimes_{\mathbf{Z}} F \otimes_B F'$之间的规范$\mathbf{Z}\text{-module}$同构，它源自形式的张量积的结合性性质（33）。

### 习题{#alg-ii-s3-exercises}

§ 3](exercises/s3/)参见[习题。
