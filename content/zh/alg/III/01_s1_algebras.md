---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 1
section_title: Algebras
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 428-438, 618
pdf_pages: 0452-0462, 0642-0642
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF AN ALGEBRA
      page: 428
      pdf_page: 452
    - "no": 2
      title: SUBALGEBRAS. IDEALS. QUOTIENT ALGEBRAS
      page: 429
      pdf_page: 453
    - "no": 3
      title: DIAGRAMS EXPRESSING ASSOCIATIVITY AND COMMUTATIVITY
      page: 431
      pdf_page: 455
    - "no": 4
      title: PRODUCTS OF ALGEBRAS
      page: 432
      pdf_page: 456
    - "no": 5
      title: RESTRICTION AND EXTENSION OF SCALARS
      page: 433
      pdf_page: 457
    - "no": 6
      title: INVERSE AND DIRECT LIMITS OF ALGEBRAS
      page: 434
      pdf_page: 458
    - "no": 7
      title: BASES OF AN ALGEBRA. MULTIPLICATION TABLE
      page: 436
      pdf_page: 460
statements: 5
exercises: 1
content_sha256: 681aafe37d788a837c177b3e83645c301d918a0a6da9f00fe0fae266cd9a3e4c
translated_from: content/en/alg/III/01_s1_algebras.md
translation_method: google
source_content_sha256: 820912e8d5d630a54cb7380bd85e9cf6d35d1c95d761b599b7ec5d3af2010845
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 67a722628c0393ed7bc81e2ed9e16e791bfdefbf38459ee8fe9c38a9d01757d5
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 1。 代数

### 1. 定义的代数

#### 定义 1 {#alg-iii-s1-def-1 .statement tag=05YR}

设$A$为交换环。 代数超过$A$（或$A$代数，或简单地代数，当不用担心混淆时）是集合$E$，其中结构通过给出以下定义：
(1) $E$上的$A$模块结构；
(2) 将 $E \times E$ 的 $A$ 双线性映射 (II, § 3, no. 5) 转换为 $E$。

这个定义发生的$E \times E$到$E$的$A$双线性映射称为代数$E$的乘法；通常用$(x, y) \mapsto x.y$表示，或简称为$(x, y) \mapsto xy$。

令$(\alpha_i)_{i \in I}$和$(\beta_j)_{j \in J}$为元素、$A$、有限支撑（I, § 2, no. 1）的两个族。那么，对于$E$的元素的所有家庭$(x_i)_{i \in I}$和$(y_j)_{j \in J}$，一般分配律公式（I, § 3, no. 4）

$$
\left( \sum_{i \in I} \alpha_i x_i \right) \left( \sum_{j \in J} \beta_j y_j \right) = \sum_{(i, j) \in I \times J} (\alpha_i \beta_j)(x_i y_j)
$$

持有；特别是

$$
(\alpha x)y = x(\alpha y) = \alpha(xy) \quad \text{for } \alpha \in A, x \in E \text{ and } y \in E.
$$

$E \times E$到$E$的双线性映射$(x, y) \mapsto yx$以及$E$定义上的$A$模结构和$E$上的$A$代数结构，与给定相反代数结构。 集合 $E$ 这个新的结构被称为反代数至代数$E$；它通常用$E^0$表示。如果 $A$ 代数 $E$ 与其相反数相同，则称为可交换的，在其他字中，如果 $E$ 中的乘法是可交换的。 $E$到$E^0$的同构也称为代数$E$的反自同构。

当代数$E$中的乘法是结合律时，$E$称为结合律$A$代数。当$E$中的乘法承认单位元素（必然是唯一的（I, § 2, no. 1））时，这个元素被称为$E$的单位元，而$E$被称为单位代数。

#### 例 {#alg-iii-s1-n1-exa-1 .statement tag=05YS}

(1) 每个交换环 $A$ 都可以被视为一个（结合和交换的）$A$-代数。
(2) 设$E$为伪环(I, § 8, no. 1)。 $E$上的乘法以及$E$定义上的独特$\mathbf{Z}$模块结构$E$关联$\mathbf{Z}$-代数结构。
(3) 设$F$为集合且$A$交换环。将 $F$ 的所有映射中的集合 $A^F$ 合并为 $A$，其中乘积环结构 (I, § 8, no. 10) 和乘积

A-模结构 (II, § 1, no. 5) 是结合律和交换律 A-代数。

(4) 设E为A-代数；内部律$(x, y) \mapsto xy + yx$和$(x, y) \mapsto xy - yx$定义（E上有A-模结构）E上的两个A-代数结构，它们一般不具有结合律；第一个律

$$(x, y) \mapsto xy + yx$$

总是可交换的。

#### 定义 2 {#alg-iii-s1-def-2 .statement tag=05YT}

*给定两个代数* E，E' *超过交换环* A，*同态* E *进入* E' *是映射* $f : E \to E'$ *这样*
(1) *f 是一个* A*-模同态*；
(2) $f(xy) = f(x)f(y)$ *对于所有* $x \in E$ *和* $y \in E$。

显然，两个A-代数同态中的合成是A-代数同态。每个双射代数同态都是同构。因此A-代数同态可以被视为A-代数结构类*态射*（*集合理论*，IV，2，no. 1）。接下来我们总是假设态射的这个选择已经被制作出来了。如果E、E'是两个A-代数，则令$\operatorname{Hom}_{A\text{-alg}}(E, E')$表示E的A-代数同态的集合到E'中。

令 E、E' 为两个代数，每个单位元。 E 的同态到 E' 映射单位元到 E' 的单位元称为*单位同态*（或*单位代数态射*）。

### 2.子代数。理想。商代数

设 A 为交换环，E A-代数。如果F是W的子A模，在E上乘法下稳定，限制到E定义的乘法的F×F（与F上的A-模结构）F上的A-代数结构，则结构，称为 A-代数 E 的 *子代数*。E 的子代数的每个交是 E 的子代数。对于 E 的元素的每个$(x_i)_{i \in I}$，E 的交 E 包含的子代数的所有 $x_i$ 被称为由 $(x_i)_{i \in I}$ 族*生成*的 E 的子代数，而 $(x_i)_{i \in I}$ 被称为该族的 *生成的系统*（或 *生成的族*） 子代数。如果$u : E \to E'$是A-代数同态，则E的每个子代数F的像$u(F)$是E'的子代数。

令 E 为*结合* 代数。对于E的每个子集M，E的元素的集合$M'$可与M的所有元素置换，是E的子代数，称为E中M的*中心化器*子代数（I, § 1, no. 5）。 E 中$M'$ 的扶正器$M''$ 也称为 M 的*双扶正器*；显然$M \subset M''$。由此可见，$M'$包含在其双中心化器$M''$中，而它正是$M''$的中心化器；但关系$M \subset M''$隐含$M'' \subset M'$，因此$M' = M''$（cf.*集合理论*，III, § 1, no. 7，命题2）。如果F是E的子代数，则F的*中心*是F及其在E中的扶正器$F'$的交$F \cap F'$。注如果

F 是*可交换的*，则$F \subset F'$，因此$F' \supset F''$；在这种情况下，F 的双中心化器 $F''$ 是 F 的 *中心*。

对于某些非关联的代数（对于例李代数），子代数和中心的扶正器概念定义不同（*李群和李代数*，I, § 1, no. 6）。

当$a$是E的子A模且关系$x \in a,\ y \in E$暗示$yx \in a$（或$xy \in a$）时，A-代数E的子集$a$称为E的*左理想*（或*右理想*）​​。这相当于说$a$是E的左理想或反代数$E^0$的右理想。 E 的*双边理想*是 E 的子集 $a$，它既是左理想又是右理想。当 E 是结合律并承认单位元 $e$ 时，对于 $\alpha \in A$ 和 $x \in E$，$\alpha x = (\alpha e)x = x(\alpha e)$ 凭借 (2) (no. 1)，因此 *环* E (I, § 8, no. 6) 的（右、左、两侧）理想为与 *代数* E 的（右、左、两侧）理想相同。 代数 E 的左（右、两侧）理想的每个和和每个交都是左（右、两侧）理想。 E 的左（或右，或两侧）理想包含子集 X 的交被称为由 X *生成*的 E 的左（或右，或两侧）理想。

令 $b$ 为 A-代数 E 的*双面*理想。如果 $x \equiv x' \pmod{b}$ 和 $y \equiv y' \pmod{b}$，则
$$
x(y - y') \in b \quad \text{and} \quad (x - x')y' \in b
$$
因此$xy \equiv x'y' \pmod{b}$。因此，内部律可以定义在商 A-模 $E/b$ 上，即 E 的乘法律 $(x, y) \mapsto xy$ 除以等价关系 $x \equiv x' \pmod{b}$ (I, § 1, no. 6) 的商。立即验证该商律是$(E/b) \times (E/b)$到$E/b$的A双线性映射；因此，定义与$E/b$A-代数结构在$E/b$上A-模结构。 $E/b$，加上代数结构，被称为双面理想$b$ 代数 E 的*商代数*。 典范映射$p : E \to E/b$是代数同态。

令E，$E'$为两个A-代数和$u : E \to E'$代数同态。 像$u(E)$是$E'$的子代数，核$b = u^{-1}(0)$是E的双面理想；此外，在 $u$ 的规范分解中：
$$
E \xrightarrow{p} E/b \xrightarrow{v} u(E) \xrightarrow{j} E'
$$
$v$ 是 *代数同构*。更一般地，当字“环”替换为“代数”时，章I, § 8, no. 9的所有结果仍然有效（以及它们的证明）。

设 A 为交换环，E A-代数。在集合$\tilde{E} = A \times E$，我们定义以下律/合成：
$$
\begin{align*}
(\lambda, x) + (\mu, y) &= (\lambda + \mu, x + y) \\
(\lambda, x)(\mu, y) &= (\lambda \mu, xy + \mu x + \lambda y) \\
\lambda(\mu, x) &= (\lambda \mu, \lambda x).
\end{align*}
$$

立即验证，$\tilde{E}$与合成的这些律相比，代数超过$A$，并且$(1,0)$是这个代数的单位元。 集合$\{0\} \times E$是$\tilde{E}$和$x \mapsto (0,x)$的双面理想，代数$E$到子代数$\{0\} \times E$的同构，由此$E$和$\{0\} \times E$是确定。 $\tilde{E}$ 称为代数，源自 $E$ 通过邻接单位元；当且仅当 $E$ 是结合律（或可交换）。

### 3. 图表表达结合性和交换律

令$A$为交换环，且$E$为$A$模；给出 $E \times E$ 到 $E$ 的双线性映射相当于给出 $A$ 线性映射：

$$
m : E \otimes_A E \to E
$$

（II, § 3, no. 5）。因此，$E$上的$A$代数结构是通过在$E$上给出$A$模结构以及$E \otimes_A E$到$E$的$A$线性映射来定义的。

令$E'$为另一个$A$-代数，$m' : E' \otimes_A E' \to E'$为$A$-线性映射，定义$E'$的乘法。 映射 $f : E \to E'$ 是$A$-代数同态当且仅当 $f$ 是映射呈现交换律图表

$$
\begin{array}{ccc}
E \otimes_A E & \xrightarrow{f \otimes f} & E' \otimes_A E' \\
\downarrow m & & \downarrow m' \\
E & \xrightarrow{f} & E'
\end{array}
$$

对于 $A$-代数 $E$ 的关联性，$A$ 的图表线性映射是必要且充分的（考虑张量积的结合性、cf. II, § 3, no. 8）

$$
\begin{array}{ccc}
E \otimes_A E \otimes_A E & \xrightarrow{m \otimes 1_E} & E \otimes_A E \\
\downarrow 1_E \otimes m & & \downarrow m \\
E \otimes_A E & \xrightarrow{m} & E
\end{array}
$$

是可交换的。类似地，对于$A$-代数$E$是可交换的，$A$-线性映射的图表是必要且充分的

$$
\begin{array}{ccc}
E \otimes_A E & \xrightarrow{\sigma} & E \otimes_A E \\
\downarrow m & & \downarrow m \\
E & & E
\end{array}
$$

是可交换的，其中$\sigma$表示由$\sigma(x \otimes y) = y \otimes x$为$x \in E, y \in E$定义的规范$A$线性映射（II, § 3, no. 1，推论2到命题1）。

对于所有$c \in E$，让$\eta_c$表示由条件$\eta_c(1) = c$定义的A到E中的A-线性映射。为了使$c$成为E的单位元，两个图表是充分必要的

$$
\begin{array}{ccc}
A \otimes_A E & \xrightarrow{\eta_c \otimes 1_E} & E \otimes_A E \\
\downarrow i & & \downarrow m \\
E & & E \\
& \uparrow & \\
E \otimes_A A & \xrightarrow{1_E \otimes \eta_c} & E \otimes_A E \\
& \downarrow i' & \downarrow m \\
E & & E
\end{array}
$$

是可交换的（$i$和$i'$表示典范同构（II, § 3, no. 4，命题4））。

设 E 为 A-代数，其中单位元 e，并设 $\eta = \eta_e$（也用 $\eta_E$ 表示）；那么 $\eta(\alpha \beta) = \eta(\alpha) \eta(\beta) = \alpha \eta(\beta)$，对于 (2) (no. 1)，

$$(\alpha e)(\beta e) = (\alpha \beta)e = \alpha(\beta e);$$

因此$\eta$是A-代数同态。观察 E 上的 A-模结构可以使用 $\eta$ 定义，对于

$$(3)$$
$$\alpha x = \eta(\alpha) \cdot x \quad \text{for } \alpha \in A, x \in E$$

（其中，在右侧，乘法在 E 中）。 同态 $\eta$ 像是 E 的子代数，其元素与所有 E 通勤。 同态 $\eta$ 核是元素 A-模 e 的湮没子 E;由(3)可知，它也是A-模E(II, § 1, no. 12)的湮没子。

当代数 E 为酉结合律时，$\eta$ 为环同态。相反，令$\rho : A \to B$为环同态，使得像$\rho(A)$包含在B的中心中，同时假设环A是可交换的；那么 A-代数结构定义在结合且单位的 B 上，写为 (cf. (3))

$$\lambda x = \rho(\lambda) \cdot x \quad \text{for } \lambda \in A, x \in E.$$

### 4.乘积代数

设$(E_i)_{i \in I}$是代数在同一个交换环A上的一个族。立即验证在乘积集合$E = \prod_{i \in I} E_i$，乘积A-模结构（II, § 1, no. 5）和乘法

$$(4)$$
$$((x_i), (y_i)) \mapsto (x_i y_i)$$

定义A-代数结构；有了这个结构，集合E就被称为代数$(E_i)_{i \in I}$家族的乘积代数。

当所有代数 $E_i$ 都是结合律（分别是交换律、单位律）时，它们的乘积也是结合律。此外，I, § 8, no. 10、扩展中所述的所有属性无需修改为代数的任意乘积。

### 5. 标量的限制和扩张

令$A_0$和A为两个交换环和$\rho : A_0 \to A$环同态。如果E是A-代数，我们用$\rho_* (E)$表示（与II, § 1, no. 13一致）由E上的加法和外法则定义的$A_0$模

$$
\lambda . x = \rho(\lambda)x \quad \text{for all } \lambda \in A_0 \text{ and all } x \in E.
$$

E 中的乘法以及$\rho_* (E)$ 定义上的$A_0$ 模结构以及$\rho_* (E)$ 上的$A_0$ 代数结构。当$A_0$是A的子环且$\rho$典范嵌入时，代数$\rho_* (E)$据说是通过将标量的环A限制为$A_0$从E获得的。滥用语言，当$\rho$任意时，这也是有时说的。

令 F 为 $A_0$ 代数。 $A_0$-代数同态$F \to \rho_* (E)$称为半同态（相对于$\rho$）或F到A-代数E的$\rho$同态；如果不引起混淆，它也称为 $A_0$ 同态。如果E，$E'$是两个A-代数，则每个A-代数同态$E \to E'$也是一个$A_0$-代数同态$\rho_* (E) \to \rho_* (E')$。

现在考虑两个交换环 A 和 B 以及环同态 $\rho : A \to B$。对于每个 A-模 E，B-模 $\rho^*(E) = E \otimes_A B$（通过将标量的环 A 扩展到 B）从 E 获得，已定义 (II, § 5, no. 1)。如果 E 也是 A-代数，我们将在 $\rho^*(E)$ 上计算定义 B 代数结构。为此，观察 $(E \otimes_A B) \otimes_B (E \otimes_A B)$ 与 $(E \otimes_A E) \otimes_A B$ (II, § 5, no. 1，命题 3) 自然同构。如果 $m : E \otimes_A E \to E$ 定义乘法在 E 上，映射 $m \otimes 1_B : (E \otimes_A E) \otimes_A B \to E \otimes_A B$ 因此被规范地标识为 B-线性映射

$$
m' : \rho^*(E) \otimes_B \rho^*(E) \to \rho^*(E)
$$

其中定义是 $\rho^*(E)$ 上所需的 B 代数结构。因此

(5)

$$
(x \otimes \beta)(x' \otimes \beta') = (xx') \otimes (\beta \beta')
$$

对于E中的$x, x'$，B中的$\beta$和$\beta'$。B代数$\rho^*(E)$据说是通过将标量的环A扩展到B（通过$\rho$）从A-代数E导出的。它也用$E_{(B)}$或$E \otimes_A B$表示。当 E 是结合律（或可交换、或单位）时，$\rho^*(E)$ 也是如此。

#### 命题 1 {#alg-iii-s1-prop-1 .statement tag=05YU}

对于每个 A-代数 E，E 的典范映射 $\phi_E : x \mapsto x \otimes 1$ 到 $E_{(B)}$ 是代数的 A 同态。此外，对于每个 B 代数 F 和每个 $A$ 同态 $f : E \to F$，存在且仅有一个 $B$ 同态 $\bar{f} : E_{(B)} \to F$，使得对于所有 $x \in E$ 都有 $\bar{f}(x \otimes 1) = f(x)$。

第一个断言紧随$E_{(B)}$中乘法的定义，这为$x \in E$和$x' \in E$提供了$(x \otimes 1)(x' \otimes 1) = (xx') \otimes 1$。对于所有$x \in E$，$E_{(B)}$到$F$满足关系$\bar{f}(x \otimes 1) = f(x)$的$B$线性映射$\bar{f}$的存在性和唯一性从II, § 5, no. 1，命题1得出；这里，这一切都相当于验证 $y$ 中的 $\bar{f}(yy') = \bar{f}(y)\bar{f}(y')$ 和 $E_{(B)}$ 中的 $y'$；作为形式$x \otimes 1$（与$x \in E$）生成的元素$B$-模块$E_{(B)}$，注意力可能仅限于$y = x \otimes 1, y' = x' \otimes 1$与$x \in E, x' \in E$的情况；因为 $yy' = (xx') \otimes 1$、关系 $\bar{f}(yy') = \bar{f}(y)\bar{f}(y')$ 则从 $f(xx') = f(x)f(x')$ 得出。

也可以说$f \mapsto \bar{f}$是规范的双射

$$
\text{Hom}_{A\text{-alg.}}(E, \rho_*(F)) \to \text{Hom}_{B\text{-alg.}}(\rho^*(E), F).
$$

因此，$E_{(B)}$和$\phi_E$的有序对由……组成是普遍映射问题的解（集合理论，IV, § 3, no. 1），其中$\Sigma$是类 $B$-代数结构和$\alpha$-将$A$-同态从$E$映射到$B$-代数。

#### 推论{#alg-iii-s1-n5-cor-1 .statement tag=05YV}

*令$E, E'$为两个$A$-代数；对于代数$u : E \to E', u \otimes 1_B$的每个$A$同态都是代数$v : E \otimes_A B \to E' \otimes_A B$的唯一$B$同态，呈现可交换的图表*

$$
\begin{array}{ccc}
E & \xrightarrow{\phi_E} & E \otimes_A B \\
u \downarrow & & \downarrow v \\
E' & \xrightarrow{\phi_{E'}} & E' \otimes_A B
\end{array}
$$

令$C$为第三个交换环且$\sigma : B \to C$环同态；典范的 $C$ 同态是直接的

$$
\sigma^*(\rho^*(E)) \to (\sigma \circ \rho)^*(E)
$$

对于所有 $x \in E$（II, § 5, no. 1、命题 2），映射 $(x \otimes 1) \otimes 1$ 到 $x \otimes 1$ 为代数同构。

### 6. 代数的逆与直极限

令$I$为*交换环*的预定集合和$(A_i, \phi_{ij})$逆系，其中$I$作为索引集合。令$(E_i, f_{ij})$为$A_i$-模块的逆系，以$I$作为索引集合（II, § 6, no. 1），并进一步假设每个$E_i$都有一个$A_i$-代数结构，并且对于$i \leq j$， $f_{ij}$ 是代数的 $A_j$ 同态（相对于 $\phi_{ij}$）(no. 5)。设$A = \lim \leftarrow A_i$和$E = \lim \leftarrow E_i$，其具有$A$模块结构，$A_i$模块$E_i$(II, § 6, no. 1)的结构的逆极限；立即验证，$E$上的合成的律，被视为$E_i$的逆极限，被视为乘法（I, § 10, no. 1）下的岩浆，$E$、定义上的$A$模块结构关于 $E$ 和 $A$-代数结构； $(E_i, f_{ij})$ 称为 $A_i$ 代数的 *逆系*，$A$ 代数 $E$ 称为其 *逆极限*。如果$f_i : E \to E_i$、$\phi_i : A \to A_i$是典范映射，$f_i$是代数的*$A$*同态（相对于$\phi_i$）。如果 $E_i$ 是结合律（或可交换），则 $E$ 也是；如果每个$E_i$对于$i \leq j$承认单位元$e_i$和$f_{ij}(e_j) = e_i$，则$e = (e_i)$是代数$E$的单位元。

令$(E'_i, f'_{ij})$为$A_i$代数的另一个逆系，对于所有$i$，令$u_i : E_i \to E'_i$为$A_i$代数同态，这些映射形成*逆系*；那么$u = \lim u_i$是一个*$A$*-代数同态。

现在假设所有$A_i$都等于*相同*交换律*环*$A$以及$\phi_{ij}$到$\mathrm{Id}_A$，因此$E = \lim \leftarrow E_i$是一个$A$代数。令$F$为$A$代数，对于所有$i \in I$，令$u_i : F \to E_i$为$A$代数同态，使得$(u_i)$为映射的逆系；那么$u = \lim \leftarrow u_i$就是代数$F$的同态变成代数$E$。 *相反*，对于每个$A$-代数同态$v : F \to E$，$v_i = f_i \circ v$族是$A$-代数同态中的逆系，使得$v = \lim \leftarrow v_i$。而且，写$\bar{f}_{ij} = \mathrm{Hom}(1_F, f_{ij})$、$(\mathrm{Hom}_{A\text{-alg.}}(F, E_i), \bar{f}_{ij})$显然是集合的逆系，可见上面的注也可以用说来表示，典范映射$v \mapsto (f_i \circ v)$是一个*双射*

$$
l_F : \mathrm{Hom}_{A\text{-alg.}}(F, \lim \leftarrow E_i) \to \lim \leftarrow \mathrm{Hom}_{A\text{-alg.}}(F, E_i).
$$

此外，对于每个 $A$-代数同态 $w : F \to F'$，

$$
\bar{w}_i = \mathrm{Hom}(w, 1_{E_i}) : \mathrm{Hom}_{A\text{-alg.}}(F', E_i) \to \mathrm{Hom}_{A\text{-alg.}}(F, E_i)
$$

形式逆系 / 映射和图表

$$
\begin{array}{ccc}
\mathrm{Hom}_{A\text{-alg.}}(F', \lim \leftarrow E_i) & \xrightarrow{l_{F'}} & \lim \leftarrow \mathrm{Hom}_{A\text{-alg.}}(F', E_i) \\
\downarrow \mathrm{Hom}(w, 1_E) & & \downarrow \lim \bar{w}_i \\
\mathrm{Hom}_{A\text{-alg.}}(F, \lim \leftarrow E_i) & \xrightarrow{l_F} & \lim \leftarrow \mathrm{Hom}_{A\text{-alg.}}(F, E_i)
\end{array}
$$

是可交换的。

现在假设$I$是正确的*有向*。考虑交换环$(A_i, \phi_{ji})$的直接系统和$A_i$模块的直接系统$(E_i, f_{ji})$，其中$I$作为索引集合；假设每个$E_i$都有一个$A_i$-代数结构，并且对于$i \leq j$，$f_{ji}$是代数的$A_i$同态（相对于$\phi_{ji}$）（no. 5）。令$A = \lim \to A_i$，$E = \lim \to E_i$； $E$具有$A$模块结构，$A_i$模块$E_i$的结构中的直极限 (II, § 6, no. 2)；此外，E上合成的律被视为E_i的直极限，被视为乘法（I, § 10, no. 3）下的岩浆，其中E上的A-模结构，定义A-代数结构在E上； (E_i, f_{ji}) 称为 A_i 代数的直接系统，A-代数 E 称为其直极限。如果 f_i : E_i \to E、\phi_i : A_i \to A 是典范映射，则 f_i 是代数的 A_i 同态（相对于 \phi_i）。如果 E_i 是关联的（或可交换的），则 E 也是如此；如果每个 E_i 对于 i \leq j 承认单位元 e_i 且 f_{ji}(e_i) = e_j，则 E 承认单位元 e，使得对于 I 中的所有 i，f_i(e_i) = e。

设 (E'_i, f'_{ji}) 为 A_i 代数的另一个直接系统，对于所有 i 令 u_i : E_i \to E'_i 为 A_i 代数同态，这些映射形成直接系统；那么 u = \lim \to u_i 是 A-代数同态。

现在假设所有环 A_i 都等于相同的环 A 以及 Id_A 的 \phi_{ji}，因此 E = \lim \to E_i 为 A-代数。设 F 为 A-代数，对于所有 i 令 u_i : E_i \to F A-代数同态，使得 (u_i) 为映射的直接系统；那么 u = \lim \to u_i 是代数 E 的同态到代数 F。相反，对于每个 A-代数同态 v : E \to F， v_i = v \circ f_i 族是 A-代数的直接系统同态使得 v = \lim \to v_i。而且，写成 \vec{f}_{ij} = \mathrm{Hom}(f_{ij}, 1_F), (\mathrm{Hom}_{A\text{-alg.}}(E_i, F), \vec{f}_{ij}) 显然是集合的逆系，可见上面的注也可以用说表示典范映射 v \mapsto (v \circ f_i) 是双射

$$
d_F : \mathrm{Hom}_{A\text{-alg.}}(\lim \to E_i, F) \to \lim \leftarrow \mathrm{Hom}_{A\text{-alg.}}(E_i, F).
$$

此外，对于每个 A-代数同态 w : F \to F'，

$$
\bar{w}_i = \mathrm{Hom}(1_{E_i}, w) : \mathrm{Hom}_{A\text{-alg.}}(E_i, F) \to \mathrm{Hom}_{A\text{-alg.}}(E_i, F')
$$

形式逆系共映射和图表

$$
\begin{array}{ccc}
\mathrm{Hom}_{A\text{-alg.}}(\lim \to E_i, F) & \xrightarrow{d_F} & \lim \mathrm{Hom}_{A\text{-alg.}}(E_i, F) \\
\downarrow \mathrm{Hom}(1_E, w) & & \downarrow \lim \bar{w}_i \\
\mathrm{Hom}_{A\text{-alg.}}(\lim \to E_i, F') & \xrightarrow{d_{F'}} & \lim \mathrm{Hom}_{A\text{-alg.}}(E_i, F')
\end{array}
$$

是可交换的。

### 7. 基的代数。 乘法表

通过定义，A-代数 E 的基等于 E 的 A-模结构的基。设 (a_i)_{i \in I} 为 E 的基； 环 A 的元素存在一个唯一族 (\gamma^k_{ij})_{(i, j, k) \in I \times I \times I}，使得对于每个有序对 (i, j) \in I \times k \in I 的 I, 集合使得 \gamma^j_{ij} \neq 0 是有限的并且

$$
a_i a_j = \sum_{k \in I} \gamma^k_{ij} a_k.
$$

$\gamma_{ij}^k$ 被称为代数 E 的结构* 相对于基 $(a_i)$ 和关系 (7) 构成乘法表* 的代数 E（相对于基$(a_i)$）。

关系 (7) 可以想象为在平方表中这些关系的右侧写下设定

$$
\begin{array}{c|ccc}
 & \cdots & a_j & \cdots \\
\hline
 & & & \\
\vdots & & & \\
\hline
a_i & & \sum_k \gamma_{ij}^k a_k & \\
\vdots & & &
\end{array}
$$

可以理解，出现在指标$j$的指标$i$和列行中的元素等于乘积$a_i a_j$。

相反，给定 E 的 *A-模* E、基 $(a_i)_{i \in I}$ 和 A 的元素族$(\gamma_{ij}^k)$，使得对于 $k \in I$ 的每个有序对 $(i, j) \in I \times I$ 集合，使得 $\gamma_{ij}^k \neq 0$ 是有限的，则在 E 上且只有一个A-代数结构，其中关系(7)成立，因为A-模$E \otimes_A E$是自由的并且承认为基$(a_i \otimes a_j)_{(i, j) \in I \times I}$（cf.II, § 3, no. 7，推论2至命题7）。

令 E 为 A-模 E 中的 A-代数和 $(a_i)_{i \in I}$ 生成的系统（对于例基）。为了使 E 具有*结合性*，$a_i$ 满足 *结合性关系* 是必要且充分的

$$(8)$$
$$(a_i a_j) a_k = a_i (a_j a_k) \quad \text{for all } i, j, k$$

映射 $(x, y, z) \mapsto (xy)z - x(yz)$ 是 A-三线性映射
$$
E \times E \times E \to E
$$
因此定义 A-线性映射 $E \otimes_A E \otimes_A E \to E$；如果对于所有元素$a_i \otimes a_j \otimes a_k$，后者映射是零，其中A-模$E \otimes_A E \otimes_A E$的形式生成的系统，则它等同于零。

类似地，对于 E 是*可交换的*，$a_i$ 满足 *交换律关系* 是必要且充分的

$$(9)$$
$$a_i a_j = a_j a_i \quad \text{for all } i, j.$$

证明类似，这次考虑 A 双线性映射 $(x, y) \mapsto xy - yx$。最后，要使元素 $e \in E$ 成为单位元，$a_i$ 满足关系是充分必要的

$$(10)$$
$$a_i = e a_i = a_i e \quad \text{for all } i,$$

这次通过考虑 A-线性映射 $x \mapsto x - xe$ 和 $x \mapsto x - ex$ 可以看出。

当$(a_i)_{i \in I}$是E的基且$(\gamma_{ij}^k)$相应的常数族结构时，关系(8)等价于关系

$$
\sum_r \gamma_{ij}^r \gamma_{rk}^s = \sum_r \gamma_{ir}^s \gamma_{jk}^r
$$

对于所有$i, j, k, s$。类似地，对于所有 $i, j, k$，关系 (9) 等价于 $\gamma_{ij}^k = \gamma_{ji}^k$。

设$(a_i)_{i \in I}$为A-代数E中的基；如果$\rho : A \to B$是环同态，则$(a_i \otimes 1)$是B代数$\rho^*(E) = E \otimes_A B$（II, § 5, no. 1，命题4）的基。如果$(\gamma_{ij}^k)$是结构相对于基$(a_i)$的常数族，则$(\rho(\gamma_{ij}^k))$族是$\rho^*(E)$相对于基$(a_i \otimes 1)$的结构常数族。

### 习题 {#alg-iii-s1-exercises}

§ 1](exercises/s1/)参见[习题。
