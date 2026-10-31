---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 9
section_title: Affine spaces and projective spaces
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 325-337, 410-417
pdf_pages: 0349-0361, 0434-0441
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF AFFINE SPACES
      page: 325
      pdf_page: 349
    - "no": 2
      title: BARYCENTRIC CALCULUS
      page: 326
      pdf_page: 350
    - "no": 3
      title: AFFINE LINEAR VARIETIES
      page: 327
      pdf_page: 351
    - "no": 4
      title: AFFINE LINEAR MAPPINGS
      page: 329
      pdf_page: 353
    - "no": 5
      title: DEFINITION OF PROJECTIVE SPACES
      page: 331
      pdf_page: 355
    - "no": 6
      title: HOMOGENEOUS COORDINATES
      page: 331
      pdf_page: 355
    - "no": 7
      title: PROJECTIVE LINEAR VARIETIES
      page: 332
      pdf_page: 356
    - "no": 8
      title: PROJECTIVE COMPLETION OF AN AFFINE SPACE
      page: 333
      pdf_page: 357
    - "no": 9
      title: EXTENSION OF RATIONAL FUNCTIONS
      page: 334
      pdf_page: 358
    - "no": 10
      title: PROJECTIVE LINEAR MAPPINGS
      page: 335
      pdf_page: 359
    - "no": 11
      title: PROJECTIVE SPACE STRUCTURE
      page: 337
      pdf_page: 361
statements: 12
exercises: 19
content_sha256: 99a58bf9cc55474653034970d70c7750b0486152078721d088edbd209c991b1d
translated_from: content/en/alg/II/09_s9_affine_spaces_and_projective_spaces.md
translation_method: google
source_content_sha256: deaf2e284f8df7e22f7c5da850928b8f961fc09326f976f2aed34d10f8f21e0e
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 32adc2e7cb250aaabfcced36f56cad004632a325fe9cb975f8b3e3f4e2405cee
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 9。仿射空间和射影空间

### 1.仿射定义空间

#### 定义 1 {#alg-ii-s9-def-1 .statement tag=05VM}

*给定左（或右）向量空间 T 在域 K 上，附加到 T 的仿射空间是加法群 T* (I, § 5, no. 5) 的任何齐次空间 E *这样 0 是 T 中唯一使 E* 的所有元素保持不变的运算符（即， T * 在 E * 上忠实且传递地运行）。 *在这些条件下，T称为E的翻译空间，其元素称为E*的翻译（或*E*的免费向量）。

接下来，我们将把注意力集中在 T 是 K 上的左向量空间的情况。仿射空间 E 的平移向量空间 T 的维数（在 K 上）被称为 E（在 K 上）的 *维数*，并用暗淡 E 或 $\dim_K E$ 表示。 维数一（或二）的仿射空间称为*仿射线*（或*仿射平面*）。仿射空间的元素也称为*点*。

在定义1的条件下，对于$t \in T$和$a \in E$，我们将用t下的点a的$t + a$或$a + t$变换来表示。然后关系

$$
s + (t + a) = (s + t) + a, \quad 0 + a = a
$$

保持$s \in T, t \in T, a \in E$。 映射 $x \mapsto x + t$ 是 E 自身的双射，我们用 t 来认同。 定义 1 此外意味着，对于所有 $a \in E$，映射 $t \mapsto t + a$ 是 T 到 E 的 *双射*。在其他字中，给定 E 的两个点 $a, b$，存在一个且仅有一个翻译 t，使得$b = t + a$；我们用$b - a$来表示这个翻译；然后公式

$$
a - a = 0, \quad a - b = -(b - a), \quad b = (b - a) + a
$$
$$
(c - b) + (b - a) = c - a
$$

保持$a \in E, b \in E, c \in E$。如果 E 的四个点 $a, b, a', b'$ 使得 $b - a = b' - a'$, 公式

$$
b' = (b' - b) + (b - a) + a = (b' - a') + (a' - a) + a
$$

T中加法的交换律表明$b' - b = a' - a$。

给定点$a \in E$，映射$x \mapsto x - a$是$E$的双射到$T$；当$E$在这个映射下与$T$等同时，我们说$E$被认为是$E$中*以$a$为原点*得到的向量空间。相反，每个向量空间$T$都具有典型的结构仿射空间附加到$T$，即齐次空间结构相应的到子群 $\{0\}$ 共 $T$ (I, § 5, no. 6)。

#### 注 {#alg-ii-s9-n1-rem-1 .statement tag=05VN}

此编号的定义。以及紧随扩展之后的一些结果，我们考虑带有运算符*$T$的任意*可交换群，而不是向量空间$T$。

### 2. 重心演算

#### 命题 1 {#alg-ii-s9-prop-1 .statement tag=05VO}

*设*$(x_i)_{i \in I}$*是点的仿射空间*$E$*和*$(\lambda_i)_{i \in L}$*元素的*$K$*有限支撑的家族，使得*$\sum_{i \in I} \lambda_i = 1$ *（*分别$\sum_{i \in I} \lambda_i = 0$*）。 *如果* $a$ *是* $E$、*点* $x \in E$ *中的任何点 *定义为*
$$
x - a = \sum_{i \in I} \lambda_i (x_i - a)
$$
*（分别是免费的向量* $\sum_{i \in I} \lambda_i (x_i - a)$）*独立于所考虑的点。*

如果$a'$是$E$的另一个点，那么
$$
\sum_i \lambda_i (x_i - a') = \sum_i \lambda_i ((x_i - a) + (a - a')) = \sum_i \lambda_i (x - a) + \left( \sum_i \lambda_i \right) (a - a').
$$
如果$\sum_i \lambda_i = 1$，则$\sum_i \lambda_i (x_i - a) = (x - a) + (a - a') = x - a'$；如果$\sum_i \lambda_i = 0$，则$\sum_i \lambda_i (x - a') = \sum_i \lambda_i (x - a)$； 从而命题。

在命题 1 的条件下，点 $x$ 定义为
$$
x - a = \sum_{i \in I} \lambda_i (x_i - a)
$$
*（分别是免费的向量*$\sum_{i \in I} \lambda_i (x_i - a)$）*由*$\sum_{i \in I} \lambda_i x_i$表示。

因此，特别是恢复了在no. 1中引入的记号$b - a$。当$\sum_i \lambda_i = 1$时，点$x = \sum_i \lambda_i x_i$被称为*点*$x_i$的重心*给定质量*$\lambda_i$。

给定$E$的$m$点$a_1, \ldots, a_m$，其数$m$不是$K$（V, § 1）特征的倍数，点$g = \sum_{i=1}^m \frac{1}{m} a_i$被调用（通过滥用

语言）点* $a_i$ ($1 \leq i \leq m$) 的*重心（对于$m = 2$，我们说“中点”而不是“重心”）；它的特点是关系
$$
\sum_{i=1}^m (a_i - g) = 0.
$$

### 3. 仿射线性簇

#### 定义 2 {#alg-ii-s9-def-2 .statement tag=05VP}

*给定一个仿射空间* $E$，*子集* $V$ ** $E$ *被称为仿射线性簇*（或简称为*线性簇*或*$E$的*仿射子集*）*如果，对于每个家庭* $(x_i)_{i \in I}$ * 点的* $V$ * 和每个家庭* $(\lambda_i)_{i \in I}$ * 元素的* $K$ * 有限支撑这样* $\sum_{i \in I} \lambda_i = 1$，*重心* $\sum_{i \in I} \lambda_i x_i$ *属于到* $V$。

这相当于说，定义 2 的条件对于$V$ 的点的每个“有限”族都成立。

空集是线性簇；每交个线性簇都是一个线性簇。

令$V$为$E$的非空子集和$a$点的$V$； 关系
$$
x - a = \sum_{i=1}^n \lambda_i (x_i - a)
$$
意味着$x$是$x_i$和$a$家族由……组成的重心$\sum_{i=1}^n \lambda_i x_i + \left(1 - \sum_{i=1}^n \lambda_i\right)a$。因此：

#### 命题 2 {#alg-ii-s9-prop-2 .statement tag=05VQ}

*对于仿射空间* $E$ 的非空子集* $V$ *作为线性簇，满足以下条件是必要且充分的：* $V$ *对于向量空间结构为向量子空间* $E$ *以* $V$ *的点为原点获得。*

特别是，向量空间$T$的非空仿射线性簇（被视为仿射空间）只是$T$的向量子空间的*翻译*；因此，$T$的向量子空间是线性簇包含0。

令 $V$ 为仿射空间 $E$ 的非空线性簇；自由向量$x - y$的集合，其中$x$和$y$贯穿$V$，是$E$的翻译空间$T$的向量子空间$D$称为$V$的*方向*：对于，如果$a \in V$，那么
$$
x - y = (x - a) - (y - a)
$$
我们的断言源自命题2。$D$在$V$上忠实且传递地运行是直接的，因此它具有规范的结构的*仿射空间附加到*$D$。仿射簇$V$的*维数*，我们指的是$V$的维数与此仿射空间结构，即向量空间$D$的维数。 维数 0 的线性簇是$E$的点； 维数 1（或 2）的线称为 $E$ 的*线*（或*平面*）。

一条线方向的每一个向量$\neq 0$属于称为该线的一个*方向向量*；其相对于 T 形式的基的分量，即相关线路的“方向参数”的所谓系统。

E 中线性簇 V 的*余维*是其方向 D 在 T 中的余维； E 中余维 1 的线性变化称为 E 的（仿射）*超平面*。

具有相同方向的两个线性品种称为“平行”；说一个是通过翻译从另一个衍生出来的，这与说一个是从另一个衍生而来的意思是一样的。如果 V 是 T 中的线性簇（视为仿射空间），则其方向是平行于 V 和包含 0 的线性簇。

#### 命题 3 {#alg-ii-s9-prop-3 .statement tag=05VR}

*给定一个仿射空间* E 的点的族* $(a_i)_{i \in I}$ *，*集合* V *重心* $\sum_{i \in I} \lambda_i a_i$ *((\lambda_i) of 有限支撑, $\sum_{i \in I} \lambda_i = 1$) 是* E 的线性簇。

如果家庭$(a_i)$是空的，那么$V = \varnothing$是因为条件$\sum_i \lambda_i = 1$。因此可以假设族$(a_i)$非空，在这种情况下命题是明显的，将$a_i$之一作为E中的原点。

簇V显然是最小的线性簇包含$a_i$；据说它是由$(a_i)$家族“生成”的，这个家族被称为V的*生成的系统*。

在命题 3 的记号中，假设族$(a_i)$非空，对于形式$x = \sum_i \lambda_i a_i$中每个点$x \in V$的表达式是*唯一的*，有充分必要，表示任意指标 $\kappa$的I，向量$a_i - a_\kappa$的族，其中$i$贯穿指标$\neq \kappa$的集合，在T中是自由的。那么E的点的族$(a_v)_{v \in I}$据说是*亲和地自由* （或者它的元素形式是一个*仿射自由系统*，或者是*仿射独立*）并且$\lambda_i$是指标$i$的$x$相对于仿射自由族$(a_i)$的*重心坐标*。

E 的点的族 $(a_i)_{i \in I}$ 不是亲缘自由的，被称为“亲缘相关”。

#### 命题 4 {#alg-ii-s9-prop-4 .statement tag=05VS}

*对于仿射空间* E 中的非空族* $(a_i)_{i \in I}$ *点 *要具有亲缘关系，存在一个族* $(\lambda_i)_{i \in I}$ *元素 *并非所有零在* K、*有限支撑中，使得* $\sum_{i \in I} \lambda_i = 0$ *和*$\sum_{i \in I} \lambda_i a_i = 0$。

给定指标$\kappa \in I$，要说向量$(a_i - a_\kappa)$的族，其中$i$贯穿指标$\neq \kappa$的集合，在T中相关，意味着存在一个标量族$(\lambda_i)_{i \neq \kappa}$，而不是全部零，使得$\sum_{i \neq \kappa} \lambda_i (a_i - a_\kappa) = 0$，也可以写成$\sum_{i \in I} \lambda_i a_i = 0$，与$\lambda_\kappa = -\sum_{i \neq \kappa} \lambda_i$，其他字$\sum_{i \in I} \lambda_i = 0$。

#### 命题 5 {#alg-ii-s9-prop-5 .statement tag=05VT}

对于仿射空间 $E$ 的点的非空族 $(a_i)_{i \in I}$ 是仿射自由的，对于每个指标 $\kappa \in I$，$a_\kappa$ 不属于 $a_i$ 生成的线性簇是充分必要的指标$\neq \kappa$。

如果$I$只有一个元素，命题是显而易见的。否则，以指标$\neq \kappa$、命题的$a_i$之一为$E$为原点，从§ 7, no. 1、注得出。

### 4.仿射线性映射

#### 定义 3 {#alg-ii-s9-def-3 .statement tag=05VU}

给定两个仿射空间$E, E'$附加到两个向量空间$T, T'$在相同的域$K$，$E$的映射$u$到$E'$称为仿射线性映射（或仿射映射）如果，对于$E$的点的每个家庭$(x_i)_{i \in I}$以及每个家庭$(\lambda_i)_{i \in I}$使得$\sum_{i \in I} \lambda_i = 1$，

$$
u\left( \sum_{i \in I} \lambda_i x_i \right) = \sum_{i \in I} \lambda_i u(x_i).
$$

(3)

#### 命题 6 {#alg-ii-s9-prop-6 .statement tag=05VV}

令$u$为$E$到$E'$的仿射映射。 $T$ 到 $T'$ 中存在且仅有一个线性映射 $v$ 使得

$$
u(x + t) = u(x) + v(t)
$$

对于所有$x \in E, t \in T$。

令$a$为$E$中的任意点。 映射

$$
t \mapsto u(a + t) - u(a)
$$

$T$ 的线性映射 $v_a$ 变成 $T'$，因为我们可以写

$$
a + \lambda t = \lambda (a + t) + (1 - \lambda)a \\
a + s + t = (a + s) + (a + t) - a
$$

由(3)可知$v_a(\lambda t) = \lambda v_a(t)$和$v_a(s + t) = v_a(s) + v_a(t)$。此外，如果$b$是$E$中的另一个点，则$v_a = v_b$； 关系

$$
(a + t) - a + b = b + t
$$

意味着

$$
u(a + t) - u(a) + u(b) = u(b + t)
$$

即$u(a + t) - u(a) = u(b + t) - u(b)$。 从而$v$的存在； 唯一性是直接的。

$v$ 被称为$T$ 的线性映射到与$u$ 相关的$T'$。相反，对于$T$的每个线性映射$v$到$T'$以及点$a \in E, a' \in E'$的每个有序对，立即验证

$$
x \mapsto a' + v(x - a)
$$

是 E 到 E' 的仿射映射 ，其关联的线性映射是 v。 因此，说 u 是 E 到 E' 的仿射映射也意味着，如果将 E 中的任意点 a 和 E' 中的点 u(a) 作为原点，则 u 是线性映射对于这两个由此得到向量空间。

令 E'' 为第三个仿射空间，T'' 其平移空间，u' 为 E' 的仿射映射到 E''，以及 T' 的 v' 线性映射到与 u' 伴随的 T''。显然 u' o u 是 E 到 E'' 的仿射映射；此外，对于 a \in E 和 t \in T，
$$
u'(u(a + t)) = u'(u(a) + v(t)) = u'(u(a)) + v'(v(t))
$$
因此 v' o v 是 T 的线性映射到与 u' o u 相关的 T''。对于仿射映射 u 是双射的，关联的线性映射 v 是双射的是必要且充分的，并且 u^{-1} 是一个仿射映射，其关联的线性映射是 v^{-1}。

特别是，E 对其自身形式群 G 的仿射双射，称为 E 的仿射群。与 u \in G 线性映射 v 关联的映射与 u 关联，通过上述，G 的同态到线性群 \mathbf{GL}(T)。如果 u 是翻译，则 v 是恒等式，反之亦然。因此，上述同态的核是E的平移群T，因此是G的正常子群。

如果 u \in G，T 的自同构 t \mapsto utu^{-1} （其中 t 通过平移 x \mapsto x + t 来标识）是与 u 关联的线性映射 v。对于 x \in E 和 t \in T，通过定义
$$
x + utu^{-1} = u(u^{-1}(x) + t) = u(u^{-1}(x)) + v(t) = x + v(t)
$$
因此 utu^{-1} = v(t)。

令 a \in E 和 G_a 为 u \in G 的 G 由……组成的子群，使得 u(a) = a。如果以a为原点将E与T标识，则G_a与\mathbf{GL}(T)标识。 G 中的每个 u \in 都可以在形式 u = t_1u_1 中唯一表示（分别在形式 u = u_2t_2 中），其中 u_1、u_2 在 G_a 中，t_1、t_2 在 T 中：对于，写 t_1 = u(a) - a, u^{-1}t_1 \in G_a， 从而u_1和t_1存在；类似地得到u_2和t_2的存在性。 唯一性由 G_a \cap T 约化到 G 的单位元素得出。此外
$$
t_1u_1 = u_1(u_1^{-1}t_1u_1)
$$
从而 u_2 = u_1, t_2 = u_1^{-1}t_1u_1。最后，与 u 和 u_1 关联的线性映射是相同的，因此，如果如上所述 G_a 用 \mathbf{GL}(T) 标识，则 u_1 是从 T 到与 u 关联的自身的线性映射。由此可见G是G_a乘以T(I, § 6, no. 1)的半直乘积。

设 E、E' 是 K 上的两个仿射空间。在 E 到 E' 的仿射映射 u 下，E（分别为 E'）的线性簇的直（或逆）像是 E'（分别为 E）的线性簇； u 的秩是 u(E) 的定义维数；它等于与 u 关联的线性映射的秩。如果V、V'分别是E、E'中相同有限维 m的线性簇，则存在$E$到$E'$的仿射映射$u$，使得$u(V) = V'$：以$E$为原点，分别为$V$和$V'$的$E'$点，然后取$E$（分别为$E'$）基，其中第一个$m$向量形式基为$V$ （分别为$V'$），命题紧随§ 1, no. 11，推论3到命题17。

由于域$K$在$K$上具有规范的左向量空间结构（维数1），因此可以将其视为维数1的仿射空间。仿射的仿射映射空间$D$（超过$K$）到仿射空间$K$也称为*仿射线性函数*（或*仿射函数*）。如果点$a$作为$E$的原点，则$E$上的每个仿射函数可以唯一地写为$x \mapsto \alpha + v(x)$，其中$\alpha \in K$和$v$是向量空间上的线性形式由此得到$E$； $E$ 上的仿射函数，因此形式维数 $1 + \dim E$ 的 *右向量空间超过*$K$。如果$u$是$E$和$\lambda \in K$上的非常数仿射函数，$x \in E$满足的集合，则方程$u(x) = \lambda$是超平面；相反，对于$E$中的每个超平面$H$，在$E$上存在一个仿射函数$u_0$，使得$H = u_0^{-1}(0)$以及每个仿射函数$u$使得$H = u^{-1}(0)$是形式$u_0 \mu$，其中$\mu \in K$（§ 7, no. 5，命题11）。如果 $u$ 是 $E$ 上的仿射函数，则超平面与方程 $u(x) = \alpha$ 和 $u(x) = \beta$ 是平行的。

### 5. 投影定义空间

#### 定义 4 {#alg-ii-s9-def-4 .statement tag=05VW}

*给定左（或右）向量空间* $V$ *超过域* $K$，*左（或右）射影空间源自* $V$，*表示为* $\mathbf{P}(V)$，*是补集* $V - \{0\}$ *的商* $\{0\}$ *在* $V$ *通过等价关系* $\Delta(V)$ *“存在* $\lambda \neq 0$ *在* $K$ *使得* $y = \lambda x$ *（或* $y = x \lambda$）*在* $x$ *和* $y$之间*在*$V - \{0\}$。

当$V = K_s^{n+1}$时，我们也写$\mathbf{P}_n(K)$代替$\mathbf{P}(K_s^{n+1})$，写$\Delta_n(K)$代替$\Delta(V)$。

定义 4 也可以用说来表示，$\mathbf{P}(V)$ 是$V$ 中移除原点的行（经过到 0）的集合；因此，$\mathbf{P}(V)$ 被规范地标识为$V$ 中的集合行（经过到 0）。射影空间的元素称为空间的 *点*。

当$V$为维数$n$时，如果$n$有限，整数$n - 1$称为射影空间$\mathbf{P}(V)$的*维数*，否则称为基数$n$；该基数用 $\dim_K \mathbf{P}(V)$ 或 $\dim \mathbf{P}(V)$ 表示。因此，维数$-1$的射影空间是空的，维数0的射影空间是单个点。 维数 1（或 2）的投影空间称为*投影线*（或*投影平面*）。

今后我们只考虑左射影空间。

### 6.齐次坐标

令$V$为有限维$n + 1$在$K$上的向量空间，$\mathbf{P}(V)$由$V$和$(e_i)_{0 \leq i \leq n}$基衍生的维数$n$的投影空间 $V$。让$\pi$表示$V - \{0\}$到商集$\mathbf{P}(V)$的典范映射。对于$V - \{0\}$的每个点$x = \sum_{i=0}^{n} \xi_i e_i$，$(\xi_0, \xi_1, \ldots, \xi_n)$被称为点$\pi(x)$的齐次坐标*系统相对于$V$的基$(e_i)$。 $n + 1$ 元素的每个系统 $(\xi_i)$ *并非 $K$ 的所有零*因此都是 $P(V)$ 的点相对于 $(e_i)$ 的齐次坐标的系统；对于这样的两个系统$(\xi_i)$、$(\xi'_i)$来说，$P(V)$的相同点的齐次坐标系统相对于相同的基$(e_i)$，存在元素$\lambda \neq 0$是充分必要的$K$，使得$\xi'_i = \lambda \xi_i$对应$0 \leq i \leq n$。

这个定义立即推广到$V$是无限维的情况。

给定 $V$ 的另一个基 $(\tilde{e}_i)$，使得 $\pi(x)$ 的齐次坐标$e_i = \sum_{j=0}^{n} \alpha_{ij} \tilde{e}_j$ ($0 \leq i \leq n$) 和系统 $(\xi_i)$ 相对于基 $(e_i)$，对于$K$的$n + 1$元素的系统$(\bar{\xi}_i)$是$\pi(x)$的齐次坐标系统相对于基$(\tilde{e}_i)$，存在$\lambda \neq 0$是充分必要的$K$ 这样

$$
\lambda \bar{\xi}_i = \sum_{j=0}^{n} \xi_j \alpha_{ji} \quad \text{for } 0 \leq i \leq n.
$$

特别是，如果 $e_i = \gamma_i \tilde{e}_i$ 与 $\gamma_i \neq 0$ ($0 \leq i \leq n$)，则 $\bar{\xi}_i = \mu \xi_i \gamma_i$ 其中 $\mu \neq 0$。

### 7. 投影线性簇

设$W$为向量空间$V$中的向量子空间；从 $V$ 导出的射影空间 $P(V)$ 中的 $W - \{0\}$ 的典范像被称为“射影线性簇”（或者在不用担心混淆时简称为“线性簇”）；由于$W - \{0\}$上的等价关系$\Delta(W)$是由关系$\Delta(V)$诱导的，$P(V)$中$W - \{0\}$的投影线性变化像可以与从$W$导出的投影空间$P(W)$识别，并且因此我们可以说维数就是这样一个品种。在空间 $P(V)$ 中，超平面（已移除原点）$V$ 的典范像是一个称为*射影超平面*（或简称为 *超平面*）的线性簇；如果$P(V)$在$P(V)$中属于有限维$n$超平面，则维数$n - 1$的线性簇。

向量空间中涉及向量子空间的每个命题都会转到关于射影线性簇的命题。对于例，如果射影空间$P(V)$是有限维$n$并且$(e_i)_{0 \leq i \leq n}$是$V$的基，维数$r$的每个线性簇$L \subset P(V)$可以是由系统或 $n - r$ 齐次线性方程组定义

$$
\sum_{i=0}^{n} \xi_i \alpha_{ij} = 0 \qquad (1 \leq j \leq n - r)
$$

在 $\mathbf{P}(V)$ 的点的齐次坐标 $\xi_i$ ($0 \leq i \leq n$) 相对于基 $(e_i)$ 之间，(4) 的左手边与 V 线性无关形式。特别是，射影超平面由单个齐次线性方程定义，其系数不全为零。相反，$\mathbf{P}(V)$满足的点任意系统齐次线性方程关于$\xi_i$形式线性簇L；如果系统被认为由 $k \leq n + 1$ 方程组组成，则 L 为维数 $\geq n - k$。

$\mathbf{P}(V)$的线性簇中的每一个交都是一个线性簇；对于$\mathbf{P}(V)$的每个子集 A，存在最小的线性簇L 包含 A；它被称为由* A *生成的线性簇，并且 A 被称为 L 的 *生成的系统*。

如果W是$\pi^{-1}(A)$生成的V的向量子空间，则$L = \mathbf{P}(W)$。

如果L和M是$\mathbf{P}(V)$中的任意两个线性簇，N是$L \cup M$生成的簇，那么（§ 7, no. 3，推论3到命题4）

$$
\text{dim } L + \text{dim } M = \text{dim}(L \cap M) + \text{dim } N.
$$

特别是，如果 $\mathbf{P}(V)$ 是有限维且 $\text{dim } L + \text{dim } M \geq \text{dim } \mathbf{P}(V)$，则从 (5) 可以得出 $L \cap M$ 非空。

令$(x_i), (y_i)$是向量空间V中点的两个族，具有相同的索引集合，这样$y_i = \lambda_i x_i$，其中$\lambda_i \neq 0$代表所有$i$。如果家庭$(x_i)$是免费的，那么$(y_i)$也是免费的，反之亦然；那么据说点 $\pi(x_i)$ $\mathbf{P}(V)$ 的家族是*投影自由*（或简单地*自由*）。这相当于说，对于每个指标$\kappa$，点$\pi(x_\kappa)$不属于到$\pi(x_i)$为$i \neq \kappa$生成的线性变化。 点的 $\mathbf{P}(V)$ 不是投影自由的，称为“投影相关”（或简称“相关”）。

对于$V - \{0\}$的点的族$(x_i)$来说，要使族$(\pi(x_i))$投射自由并且生成$\mathbf{P}(V)$，$(x_i)$是V的基是必要且充分的。如果$\mathbf{P}(V)$是维数，$n$数是元素，那么在这样的家庭中就是$n + 1$。 注在$\mathbf{P}(V)$中给出这样一个族$(\pi(x_i))$不会确定（甚至在左因子之内）$\mathbf{P}(V)$的给定点相对于V的基$(y_i)$的齐次坐标，使得$\pi(y_i) = \pi(x_i)$ 对于所有 $i$ (cf. no. 6)。

### 8. 仿射空间的投影完成

令 V 为域 K 上的（左）向量空间，并考虑 K 上的向量空间 $K_s \times V$；射影空间 $\mathbf{P}(K_s \times V)$ 称为射影空间 *与向量空间 V *规范相关*。如果 V 属于维数 $n$，则$\mathbf{P}(K_s \times V)$ 也属于维数 $n$。考虑$K_s \times V$中的仿射超平面$V_1 = \{1\} \times V$，其方向（no. 3）为子空间$V_0 = \{0\} \times V$；如果$K_s \times V$的一行（经过到0）不包含在$V_0$中，则它包含点$(\alpha, x)$与$\alpha \neq 0$和$x \in V$，因此它包含也点 $\alpha^{-1}(\alpha, x) = (1, \alpha^{-1}x)$共$V_1$； 逆命题是直接的，可以看出，$V_1$的点和$V_0$中未包含的$K_s \times V$的线（经过到0）之间存在一一对应的对应，后者中的每一个都与$V_1$相交只有一个点。由此可见，映射 $x \mapsto \phi(x) = \pi(1, x)$ 是 $V$ 的单射（称为规范）到射影空间 $P(K_s \times V)$； $V$ 通常在单射下与它的像一起识别。 $P(K_s \times V)$中$\phi(V)$的补集是超平面$P(V_0)$在$P(K_s \times V)$无穷大处称为超平面（或$V$，滥用语言）；它的点也称为$P(K_s \times V)$（或$V$）的“无穷远点”。如果$(a_i)$是$V$的基并且在$K_s \times V$基中取元素$e_i = (0, a_i)$的由……组成和元素$e_\omega = (1, 0)$，点在$P(K_s \times V)$中的无穷大是指标$\omega$齐次坐标为0的那些。

令 $M$ 为$V$ (no. 3) 和 $D$ 方向的仿射线性簇； $P(K_s \times V)$中的$M$的典范像$\phi(M)$包含在由$K_s \times V$的仿射簇$M_1 = \{1\} \times M$生成的$K_s \times V$的向量子空间$M_2$的典范像$\overline{M} = \pi(M_2)$中。更准确地说，如果 $(a_i)$ 是 $M$ 生成的 $M$ 的仿射自由系统，则 $M_2$ 的元素 $(1, a_i)$ 形式基，因此 $\overline{M}$ 只是由 $\phi(M)$ 生成的投影线性变化；如果 $M$ 是有限维的，$\overline{M}$ 与 $M$ 具有相同的维数。 $\overline{M}$中$\phi(M)$的补集是$\overline{M}$和超平面无穷大的交，并且等于典范像$\pi(M_0)$，其中$M_0 = \{0\} \times D$。

相反，令 $N$ 为无穷远处不包含在超平面中的射影线性簇，并令 $R = \pi^{-1}(N)$； $R \cap V_1$是形式$\{1\} \times M$的$K \times V$的仿射线性簇，其中$M$是$V$的仿射线性簇，并且立即可以看出$N$是由$\phi(M)$生成的仿射线性簇$\overline{M}$。

因此，$V$的仿射线性簇和$P(K_s \times V)$的射影线性簇（不包含在无穷远超平面中）之间存在一对一的对应；对于 $V$ 的两个仿射线性簇平行，其生成的射影线性簇在无穷远处与超平面具有相同的交是必要且充分的（即，所讨论的两个仿射线性簇在无穷远处具有相同的点，即用说表示有时）无穷大）。

### 9.理性的扩张函数

如果将no. 8的结果应用到维数1的向量空间$V = K_s$，可以看出在射影线$P_1(K) = P(K_s \times K_s)$中存在$K_s$的典范嵌入$\phi$；对于所有 $\xi \in K$，$\phi(\xi)$ 是点，齐次坐标 $(1, \xi)$ 相对于 $K_s \times K_s$ 的典范基 (§ 1, no. 11)。 $P_1(K)$中$\phi(K)$的补集由相对于上述基具有齐次坐标$(0, 1)$的单个点组成；它被称为“无穷远点”。 $P_1(K)$也称为与$K$相关的射影域，并用$\tilde{K}$表示，$\tilde{K}$中无穷远的点用$\infty$表示。

*特别考虑$K$为交换域的情况，并令f \in K(X)为K(IV, § 4)上的一个不定数中的有理函数；如果$f \neq 0$，则存在唯一的表达式$f = \alpha p/q$，其中$\alpha \in K^*$和$p$和$q$是两个互质一元多项式（VII, § 1）；令$m$和$n$分别为次数，并令$r = \sup(m, n)$。我们写
$$
p_1(T, X) = T^r p(X/T), \qquad q_1(T, X) = T^r q(X/T);
$$
$p_1$和$q_1$是次数$r$在$K$上的两个齐次多项式，使得$p(X) = p_1(1, X)$、$q(X) = q_1(1, X)$。因此，对于每个元素$\xi \in K$（不是$q(X)$的零），定义了$f(\xi) = \alpha p(\xi)/q(\xi)$，我们可以写
$$
f(\xi) = \alpha p_1(1, \xi)/q_1(1, \xi) = \alpha p_1(\lambda, \lambda \xi)/q_1(\lambda, \lambda \xi)
$$
对于$K$中的所有$\lambda \neq 0$。那么考虑映射
$$
(\eta, \xi) \mapsto (q_1(\eta, \xi), p_1(\eta, \xi))
$$
$K^2$ 自身；它与等价关系 $\Delta(K^2)$ 相容的，因此定义，当经过为商时，$\tilde{K}$ 的映射 $\tilde{f}$ 为自身，其中重合与 $\xi \mapsto f(\xi)$ 在点 ，其中此有理数定义函数；据说，通过滥用语言，$\tilde{f}$是$f$到$\tilde{K}$的规范扩张。

对于例，如果$f = 1/X$，则$\tilde{f}(0) = \infty$和$\tilde{f}(\infty) = 0$；如果
$$
f = (aX + b)/(cX + d)
$$
$ad - bc \neq 0$，则$\tilde{f}(-d/c) = \infty$，如果$c \neq 0$则为$\tilde{f}(\infty) = a/c$，如果$c = 0$则为$\tilde{f}(\infty) = \infty$。如果 $f = a_0 X^n + \cdots + a_n$ 是次数 $n > 0$ 的多项式，则 $\tilde{f}(\infty) = \infty$*

### 10.投影线性映射

设$V, V'$是域$K$的两个左向量空间，$V$的$f$线性映射变成$V'$，$N = \overline{f}(0)$是核。 It is immediate that the image under $f$ of a line (passing through 0) in $V$ not contained in $N$ is a line (passing through 0) in $V'$; hence, on passing to the quotients, $f$ defines a mapping $g$ of $P(V) - P(N)$ into $P(V')$. 这样的映射称为射影线性映射（或者简单地称为射影映射）；尽管它是在$P(V) - P(N)$上定义的，而不是在$P(V)$上定义的（当$N \neq \{0\}$时），但我们会滥用语言说$g$是$P(V)$到$P(V')$的投影映射。 射影线性簇 $P(N)$（其中 $g$ 未定义）称为 $g$ 的中心。

注，当$g$定义在$P(V)$的整体上时（即$N = \{0\}$时），$g$是$P(V)$的单射到$P(V')$。

当 $V$ 和 $V'$ 分别给出基 $(a_\lambda)_{\lambda \in L}, (b_\mu)_{\mu \in M}$ 时，$P(V)$ 的投影映射到 $P(V)$ 的 $P(V')$ 映射点，齐次坐标为 $\xi_\lambda$ ($\lambda \in L$)到 $\mathbf{P}(V')$ 的点以及形式齐次坐标 $\eta_\mu$ ($\mu \in M$) 的系统

$$
\eta_\mu = \sum_{\lambda \in L} \xi_\lambda \alpha_{\lambda \mu} \quad (\alpha_{\lambda \mu} \in K).
$$

$g$ 的中心是由方程定义的线性变化

$$
\sum_{\lambda \in L} \xi_\lambda \alpha_{\lambda \mu} = 0 \quad (\mu \in M).
$$

如果$C$是$g$的中心，$M$是$\mathbf{P}(V)$的线性簇，$M - (M \cap C)$的$g$下的像是$\mathbf{P}(V')$的线性簇，用$g(M)$表示（滥用语言）。然后

$$
\dim g(M) + \dim(M \cap C) + 1 = \dim M
$$

（§ 7, no. 4，公式（12））。如果$M'$是$\mathbf{P}(V')$的线性簇，$g^{-1}(M') \cup C$是$\mathbf{P}(V)$的线性簇并且

$$
\dim(g^{-1}(M') \cup C) = \dim C + \dim(M' \cap g(\mathbf{P}(V))) + 1.
$$

滥用语言，据说$g^{-1}(M') \cup C$是$M'$在$g$下的*逆像*。

由于线性映射在$V$的基$(e_i)$上取值可以在$V'$中任意选择，因此可以看出，$\mathbf{P}(V)$存在射影线性映射到$\mathbf{P}(V')$在取*任意*值点$\pi(e_i)$。 但是（即使 $g$ 到处都有定义）给出 $g(\pi(e_i))$ 并不唯一地给出确定 $g$ (习题 10)。

两个射影映射（双射）的合成是射影映射； 双射的逆映射也是如此。射影空间$\mathbf{P}(V)$自身的双射射影映射因此形式群，称为$\mathbf{P}(V)$的*射影群*并用$\mathbf{PGL}(V)$表示；我们写 $\mathbf{PGL}_n(K)$ 或 $\mathbf{PGL}(n, K)$ 而不是 $\mathbf{PGL}(K^n_s)$。

#### 注 {#alg-ii-s9-n10-rem-1 .statement tag=05VX}

在域 $K$ 的射影空间 $\mathbf{P}(V)$ 中，令 $H = \mathbf{P}(W)$ 为超平面。存在$V$到$K_s \times W$的双射线性映射$f$使得$f(W) = W$；令 $g$ 为从 $f$ 通过经过到商的投影映射。已经看出(no. 8)，$\mathbf{P}(K_s \times W)$中$\mathbf{P}(W)$的补集可以用仿射空间来识别，其平移空间是$W$。当$\mathbf{P}(V)$通过$g$与$\mathbf{P}(K_s \times W)$等同时，就说$H$*已在$\mathbf{P}(V)$中被视为无穷远*处的超平面；然后，$\mathbf{P}(V)$中$H$的补集被识别为仿射空间，其平移空间为$W$。

### 11.投影空间结构

Given a set E and a field K, a (left) projective space structure on E with respect to the field K is defined by giving a non-empty set $\Phi$ of bijections of subsets of the projective space $\mathbf{P}(K_s^{(E)})$ onto E satisfying the following axioms:

每映射$f \in \Phi$定义$$(\mathrm{EP}_I)$$*集合是$\mathbf{P}(K_s^{(E)})$的线性簇。*

$$(\mathrm{EP}_{II})$$ *For every ordered pair of elements $f, g$ of $\Phi$ defined respectively on the linear varieties $\mathbf{P}(V)$ and $\mathbf{P}(W)$, the bijection $h = g^{-1} \circ f$ of $\mathbf{P}(V)$ onto $\mathbf{P}(W)$ is a projective mapping.*

$$(\mathrm{EP}_{III})$$ *相反，如果 $f \in \Phi$ 定义在线性簇 $\mathbf{P}(V)$ 上并且 $h$ 是 $\mathbf{P}(V)$ 的双射射影映射到线性簇 $\mathbf{P}(W) \subset \mathbf{P}(K_s^{(E)})$，则 $f \circ h^{-1} \in \Phi$。*

令 E 为集合，$(V_\lambda)_{\lambda \in L}$ K 上的向量空间族，并假设将 $\mathbf{P}(V_\lambda)$ 的每个 $\lambda \in L$ 双射的 $f_\lambda$ 赋给 E，使得对于指标 $\lambda, \mu, f_\lambda^{-1} \circ f_\mu$ 的每个有序对是一个 *射影$\mathbf{P}(V_\mu)$ 的映射* 到$\mathbf{P}(V_\lambda)$。 那么我们可以在E上定义关于K的射影空间结构如下：令$(e_i)_{i \in I}$为空间$V_\lambda$的基并写成$a_i = f_\lambda(\pi(e_i))$；令$b_i$为$K_s^{(E)}$(§ 1, no. 11)的典范基中的指标$a_i$元素。 关系 $i \neq \kappa$ 隐含$b_i \neq b_\kappa$，因为假设 $f_\lambda$ 是双射；因此，$K_s^{(E)}$的向量子空间$W_0$的$b_i$形式基，因此存在$\mathbf{P}(W_0)$的双射射影映射$h$到$\mathbf{P}(V_\lambda)$，使得$h(\pi(b_i)) = \pi(e_i)$ 对于所有 $i \in I$。 如果$\Phi$被取为所有双射射影映射$f_\lambda \circ h \circ g^{-1}$的集合，其中$g$贯穿所有双射射影映射$\mathbf{P}(W) \subset \mathbf{P}(K_s^{(E)})$的集合，则立即验证$\Phi$满足公理（EP_I）， （EP_{II}）和（EP_{III}）。 此外，直接的，$\Phi$既不依赖于指标$\lambda \in L$的选择，也不依赖于$V_\lambda$中的基$(e_i)$的选择，也不依赖于$h$的选择。

特别是（将L由单个元素组成），从向量空间V（no. 5，定义4）派生的每个射影空间$\mathbf{P}(V)$因此具有明确确定的“射影空间结构”，其含义为定义在此编号中给出。因此，任何带有射影空间结构的集合都可以称为*射影空间*。

对于相同的记号，射影空间 E 中的*线性簇*是 E 的子集 M，这样，对于在 $\mathbf{P}(V) \subset \mathbf{P}(K_s^{(E)})$ 上定义的至少*一个* 双射的 $f \in \Phi$，$f^{-1}(M)$ 是 $\mathbf{P}(V)$ 中 no. 7 意义上的线性簇（这性质则适用于*所有* $f \in \Phi$）。从上面可以看出，射影空间中的每个线性簇都典型地具有射影空间结构。

如果 $f \in \Phi, f^{-1}(E)$ 是维数 n 的线性变体，则射影空间 E 被称为 *of 维数 n*（只要满足 *one* 映射 $f \in \Phi$ 就足够了）。

### 习题{#alg-ii-s9-exercises}

§ 9](exercises/s9/)参见[习题。
